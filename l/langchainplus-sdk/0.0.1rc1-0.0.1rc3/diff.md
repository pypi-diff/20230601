# Comparing `tmp/langchainplus_sdk-0.0.1rc1.tar.gz` & `tmp/langchainplus_sdk-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.1rc1.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.1rc3.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.1rc1.tar` & `langchainplus_sdk-0.0.1rc3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      604 2023-05-31 03:06:17.895497 langchainplus_sdk-0.0.1rc1/README.md
--rw-r--r--   0        0        0      119 2023-05-31 01:18:44.687819 langchainplus_sdk-0.0.1rc1/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0    17009 2023-05-31 02:59:28.603476 langchainplus_sdk-0.0.1rc1/langchainplus_sdk/client.py
--rw-r--r--   0        0        0     6647 2023-05-31 02:59:33.535466 langchainplus_sdk-0.0.1rc1/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     1315 2023-05-31 01:24:33.402976 langchainplus_sdk-0.0.1rc1/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      796 2023-05-31 04:00:02.925774 langchainplus_sdk-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      757 2023-06-01 21:49:55.754293 langchainplus_sdk-0.0.1rc3/README.md
+-rw-r--r--   0        0        0      119 2023-06-01 21:49:55.754293 langchainplus_sdk-0.0.1rc3/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0    17480 2023-06-01 21:49:55.754293 langchainplus_sdk-0.0.1rc3/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0     6994 2023-06-01 21:49:55.754293 langchainplus_sdk-0.0.1rc3/langchainplus_sdk/run_trees.py
+-rw-r--r--   0        0        0     6893 2023-06-01 21:49:55.754293 langchainplus_sdk-0.0.1rc3/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     2801 2023-06-01 21:49:55.754293 langchainplus_sdk-0.0.1rc3/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      796 2023-06-01 21:49:55.754293 langchainplus_sdk-0.0.1rc3/pyproject.toml
+-rw-r--r--   0        0        0     1393 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.1rc3/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.1rc1/README.md` & `langchainplus_sdk-0.0.1rc3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # LangChainPlus Client SDK
 
-This package contains the Python client for interacting with the LangChainPlus platform.
+This package contains the Python client for interacting with the [LangChainPlus platform](https://www.langchain.plus/).
 
 LangChainPlus helps you and your team develop and evaluate language models and intelligent agents. It works
 with any LLM Application, including a seamless integration with [LangChain](https://github.com/hwchase17/langchain), a widely recognized open-source framework that simplifies the process for developers to create powerful language model applications.
 
 LangChainPlus is developed and maintained by [LangChain](https://langchain.com/), the company behind the LangChain framework.
 
+
+## Documentation
+
+To learn more about the LangChainPlus platform, check out the [docs](https://docs.langchain.plus/docs/)
```

### Comparing `langchainplus_sdk-0.0.1rc1/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.1rc3/langchainplus_sdk/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 )
 from urllib.parse import urlsplit
 from uuid import UUID
 
 import requests
 from pydantic import BaseSettings, Field, root_validator
 from requests import Response
-from tenacity import retry, stop_after_attempt, wait_fixed
+from tenacity import (
+    before_sleep_log,
+    retry_if_exception_type,
+    stop_after_attempt,
+    wait_exponential,
+)
 
 from langchainplus_sdk.schemas import (
     APIFeedbackSource,
     Dataset,
     DatasetCreate,
     Example,
     ExampleCreate,
@@ -36,15 +41,20 @@
     FeedbackSourceType,
     ListFeedbackQueryParams,
     ListRunsQueryParams,
     ModelFeedbackSource,
     Run,
     TracerSession,
 )
-from langchainplus_sdk.utils import raise_for_status_with_text, xor_args
+from langchainplus_sdk.utils import (
+    LangChainPlusAPIError,
+    raise_for_status_with_text,
+    request_with_retries,
+    xor_args,
+)
 
 if TYPE_CHECKING:
     import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
@@ -54,19 +64,34 @@
         netloc = urlsplit(url).netloc.split(":")[0]
         ip = socket.gethostbyname(netloc)
         return ip == "127.0.0.1" or ip.startswith("0.0.0.0") or ip.startswith("::")
     except socket.gaierror:
         return False
 
 
+ID_TYPE = Union[UUID, str]
+
+
+def _default_retry_config() -> Dict[str, Any]:
+    return dict(
+        stop=stop_after_attempt(3),
+        wait=wait_exponential(multiplier=1, min=4, max=10),
+        retry=retry_if_exception_type(LangChainPlusAPIError),
+        before_sleep=before_sleep_log(logger, logging.WARNING),
+    )
+
+
 class LangChainPlusClient(BaseSettings):
     """Client for interacting with the LangChain+ API."""
 
     api_key: Optional[str] = Field(default=None, env="LANGCHAIN_API_KEY")
     api_url: str = Field(default="http://localhost:1984", env="LANGCHAIN_ENDPOINT")
+    retry_config: Mapping[str, Any] = Field(
+        default_factory=_default_retry_config, exclude=True
+    )
 
     @root_validator(pre=True)
     def validate_api_key_if_hosted(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Verify API key is provided if url not localhost."""
         api_url: str = values.get("api_url", "http://localhost:1984")
         api_key: Optional[str] = values.get("api_key")
         if not _is_localhost(api_url):
@@ -94,18 +119,22 @@
     def _headers(self) -> Dict[str, str]:
         """Get the headers for the API request."""
         headers = {}
         if self.api_key:
             headers["x-api-key"] = self.api_key
         return headers
 
-    def _get(self, path: str, params: Optional[Dict[str, Any]] = None) -> Response:
-        """Make a GET request."""
-        return requests.get(
-            f"{self.api_url}{path}", headers=self._headers, params=params
+    def _get_with_retries(
+        self, path: str, params: Optional[Dict[str, Any]] = None
+    ) -> Response:
+        return request_with_retries(
+            "get",
+            f"{self.api_url}{path}",
+            request_kwargs={"params": params, "headers": self._headers},
+            retry_config=self.retry_config,
         )
 
     def upload_dataframe(
         self,
         df: pd.DataFrame,
         name: str,
         description: str,
@@ -145,42 +174,49 @@
         # TODO: Make this more robust server-side
         if "detail" in result and "already exists" in result["detail"]:
             file_name = csv_file if isinstance(csv_file, str) else csv_file[0]
             file_name = file_name.split("/")[-1]
             raise ValueError(f"Dataset {file_name} already exists")
         return Dataset(**result)
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
-    def read_run(self, run_id: Union[str, UUID]) -> Run:
+    def read_run(self, run_id: ID_TYPE) -> Run:
         """Read a run from the LangChain+ API."""
-        response = self._get(f"/runs/{run_id}")
-        raise_for_status_with_text(response)
+        response = self._get_with_retries(f"/runs/{run_id}")
         return Run(**response.json())
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
     def list_runs(
         self,
         *,
-        session_id: Optional[str] = None,
+        session_id: Optional[ID_TYPE] = None,
         session_name: Optional[str] = None,
         run_type: Optional[str] = None,
         **kwargs: Any,
     ) -> Iterator[Run]:
         """List runs from the LangChain+ API."""
         if session_name is not None:
             if session_id is not None:
                 raise ValueError("Only one of session_id or session_name may be given")
             session_id = self.read_session(session_name=session_name).id
         query_params = ListRunsQueryParams(
             session_id=session_id, run_type=run_type, **kwargs
         )
-        response = self._get("/runs", params=query_params.dict(exclude_none=True))
-        raise_for_status_with_text(response)
+        response = self._get_with_retries(
+            "/runs", params=query_params.dict(exclude_none=True)
+        )
         yield from [Run(**run) for run in response.json()]
 
+    def delete_run(self, run_id: ID_TYPE) -> None:
+        """Delete a run from the LangChain+ API."""
+        response = requests.delete(
+            f"{self.api_url}/runs/{run_id}",
+            headers=self._headers,
+        )
+        raise_for_status_with_text(response)
+        return
+
     def create_session(
         self, session_name: str, session_extra: Optional[dict] = None
     ) -> TracerSession:
         """Create a session on the LangChain+ API."""
         endpoint = f"{self.api_url}/sessions?upsert=true"
         body = {
             "name": session_name,
@@ -190,50 +226,45 @@
             endpoint,
             headers=self._headers,
             json=body,
         )
         raise_for_status_with_text(response)
         return TracerSession(**response.json())
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
     @xor_args(("session_id", "session_name"))
     def read_session(
         self, *, session_id: Optional[str] = None, session_name: Optional[str] = None
     ) -> TracerSession:
         """Read a session from the LangChain+ API."""
         path = "/sessions"
         params: Dict[str, Any] = {"limit": 1}
         if session_id is not None:
             path += f"/{session_id}"
         elif session_name is not None:
             params["name"] = session_name
         else:
-            raise ValueError("Must provide dataset_name or dataset_id")
-        response = self._get(
+            raise ValueError("Must provide session_name or session_id")
+        response = self._get_with_retries(
             path,
             params=params,
         )
-        raise_for_status_with_text(response)
-        response = self._get(
+        response = self._get_with_retries(
             path,
             params=params,
         )
-        raise_for_status_with_text(response)
         result = response.json()
         if isinstance(result, list):
             if len(result) == 0:
-                raise ValueError(f"Dataset {session_name} not found")
+                raise ValueError(f"Session {session_name} not found")
             return TracerSession(**result[0])
         return TracerSession(**response.json())
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
     def list_sessions(self) -> Iterator[TracerSession]:
         """List sessions from the LangChain+ API."""
-        response = self._get("/sessions")
-        raise_for_status_with_text(response)
+        response = self._get_with_retries("/sessions")
         yield from [TracerSession(**session) for session in response.json()]
 
     @xor_args(("session_name", "session_id"))
     def delete_session(
         self, *, session_name: Optional[str] = None, session_id: Optional[str] = None
     ) -> None:
         """Delete a session from the LangChain+ API."""
@@ -260,49 +291,51 @@
             self.api_url + "/datasets",
             headers=self._headers,
             data=dataset.json(),
         )
         raise_for_status_with_text(response)
         return Dataset(**response.json())
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
     @xor_args(("dataset_name", "dataset_id"))
     def read_dataset(
-        self, *, dataset_name: Optional[str] = None, dataset_id: Optional[str] = None
+        self,
+        *,
+        dataset_name: Optional[str] = None,
+        dataset_id: Optional[ID_TYPE] = None,
     ) -> Dataset:
         path = "/datasets"
         params: Dict[str, Any] = {"limit": 1}
         if dataset_id is not None:
             path += f"/{dataset_id}"
         elif dataset_name is not None:
             params["name"] = dataset_name
         else:
             raise ValueError("Must provide dataset_name or dataset_id")
-        response = self._get(
+        response = self._get_with_retries(
             path,
             params=params,
         )
-        raise_for_status_with_text(response)
         result = response.json()
         if isinstance(result, list):
             if len(result) == 0:
                 raise ValueError(f"Dataset {dataset_name} not found")
             return Dataset(**result[0])
         return Dataset(**result)
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
     def list_datasets(self, limit: int = 100) -> Iterator[Dataset]:
         """List the datasets on the LangChain+ API."""
-        response = self._get("/datasets", params={"limit": limit})
-        raise_for_status_with_text(response)
+        response = self._get_with_retries("/datasets", params={"limit": limit})
         yield from [Dataset(**dataset) for dataset in response.json()]
 
     @xor_args(("dataset_id", "dataset_name"))
     def delete_dataset(
-        self, *, dataset_id: Optional[str] = None, dataset_name: Optional[str] = None
+        self,
+        *,
+        dataset_id: Optional[ID_TYPE] = None,
+        dataset_name: Optional[str] = None,
     ) -> Dataset:
         """Delete a dataset by ID or name."""
         if dataset_name is not None:
             dataset_id = self.read_dataset(dataset_name=dataset_name).id
         if dataset_id is None:
             raise ValueError("Must provide either dataset name or ID")
         response = requests.delete(
@@ -312,18 +345,18 @@
         raise_for_status_with_text(response)
         return Dataset(**response.json())
 
     @xor_args(("dataset_id", "dataset_name"))
     def create_example(
         self,
         inputs: Mapping[str, Any],
-        dataset_id: Optional[UUID] = None,
+        dataset_id: Optional[ID_TYPE] = None,
         dataset_name: Optional[str] = None,
         created_at: Optional[datetime] = None,
-        outputs: Mapping[str, Any] | None = None,
+        outputs: Optional[Mapping[str, Any]] = None,
     ) -> Example:
         """Create a dataset example in the LangChain+ API."""
         if dataset_id is None:
             dataset_id = self.read_dataset(dataset_name=dataset_name).id
 
         data = {
             "inputs": inputs,
@@ -336,45 +369,41 @@
         response = requests.post(
             f"{self.api_url}/examples", headers=self._headers, data=example.json()
         )
         raise_for_status_with_text(response)
         result = response.json()
         return Example(**result)
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
-    def read_example(self, example_id: Union[str, UUID]) -> Example:
+    def read_example(self, example_id: ID_TYPE) -> Example:
         """Read an example from the LangChain+ API."""
-        response = self._get(f"/examples/{example_id}")
-        raise_for_status_with_text(response)
+        response = self._get_with_retries(f"/examples/{example_id}")
         return Example(**response.json())
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
     def list_examples(
-        self, dataset_id: Optional[str] = None, dataset_name: Optional[str] = None
+        self, dataset_id: Optional[ID_TYPE] = None, dataset_name: Optional[str] = None
     ) -> Iterator[Example]:
         """List the datasets on the LangChain+ API."""
         params = {}
         if dataset_id is not None:
             params["dataset"] = dataset_id
         elif dataset_name is not None:
             dataset_id = self.read_dataset(dataset_name=dataset_name).id
             params["dataset"] = dataset_id
         else:
             pass
-        response = self._get("/examples", params=params)
-        raise_for_status_with_text(response)
+        response = self._get_with_retries("/examples", params=params)
         yield from [Example(**dataset) for dataset in response.json()]
 
     def update_example(
         self,
         example_id: str,
         *,
         inputs: Optional[Dict[str, Any]] = None,
         outputs: Optional[Mapping[str, Any]] = None,
-        dataset_id: Optional[str] = None,
+        dataset_id: Optional[ID_TYPE] = None,
     ) -> Dict[str, Any]:
         """Update a specific example."""
         example = ExampleUpdate(
             inputs=inputs,
             outputs=outputs,
             dataset_id=dataset_id,
         )
@@ -382,25 +411,34 @@
             f"{self.api_url}/examples/{example_id}",
             headers=self._headers,
             data=example.json(exclude_none=True),
         )
         raise_for_status_with_text(response)
         return response.json()
 
+    def delete_example(self, example_id: ID_TYPE) -> Example:
+        """Delete an example by ID."""
+        response = requests.delete(
+            f"{self.api_url}/examples/{example_id}",
+            headers=self._headers,
+        )
+        raise_for_status_with_text(response)
+        return Example(**response.json())
+
     def create_feedback(
         self,
-        run_id: str,
+        run_id: ID_TYPE,
         key: str,
         *,
         score: Union[float, int, bool, None] = None,
         value: Union[float, int, bool, str, dict, None] = None,
         correction: Union[str, dict, None] = None,
         comment: Union[str, None] = None,
         source_info: Optional[Dict[str, Any]] = None,
-        feedback_source_type: FeedbackSourceType = FeedbackSourceType.API,
+        feedback_source_type: Union[FeedbackSourceType, str] = FeedbackSourceType.API,
     ) -> Feedback:
         """Create a feedback in the LangChain+ API.
 
         Args:
             run_id: The ID of the run to provide feedback on.
             key: The name of the metric, tag, or 'aspect' this
                 feedback is about.
@@ -427,43 +465,41 @@
             value=value,
             correction=correction,
             comment=comment,
             feedback_source=feedback_source,
         )
         response = requests.post(
             self.api_url + "/feedback",
-            headers=self._headers,
+            headers={**self._headers, "Content-Type": "application/json"},
             data=feedback.json(),
         )
         raise_for_status_with_text(response)
         return Feedback(**feedback.dict())
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
-    def read_feedback(self, feedback_id: str) -> Feedback:
+    def read_feedback(self, feedback_id: ID_TYPE) -> Feedback:
         """Read a feedback from the LangChain+ API."""
-        response = self._get(f"/feedback/{feedback_id}")
-        raise_for_status_with_text(response)
+        response = self._get_with_retries(f"/feedback/{feedback_id}")
         return Feedback(**response.json())
 
-    @retry(stop=stop_after_attempt(3), wait=wait_fixed(0.5))
     def list_feedback(
         self,
         *,
-        run_ids: Optional[Sequence[Union[str, UUID]]] = None,
+        run_ids: Optional[Sequence[ID_TYPE]] = None,
         **kwargs: Any,
     ) -> Iterator[Feedback]:
         """List the feedback objects on the LangChain+ API."""
         params = ListFeedbackQueryParams(
             run=run_ids,
             **kwargs,
         )
-        response = self._get("/feedback", params=params.dict(exclude_none=True))
-        raise_for_status_with_text(response)
+        response = self._get_with_retries(
+            "/feedback", params=params.dict(exclude_none=True)
+        )
         yield from [Feedback(**feedback) for feedback in response.json()]
 
-    def delete_feedback(self, feedback_id: str) -> None:
+    def delete_feedback(self, feedback_id: ID_TYPE) -> None:
         """Delete a feedback by ID."""
         response = requests.delete(
             f"{self.api_url}/feedback/{feedback_id}",
             headers=self._headers,
         )
         raise_for_status_with_text(response)
```

### Comparing `langchainplus_sdk-0.0.1rc1/langchainplus_sdk/schemas.py` & `langchainplus_sdk-0.0.1rc3/langchainplus_sdk/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Schemas for the langchainplus API."""
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
-from typing import Any, ClassVar, Dict, List, Mapping, Optional, Sequence, Union
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Union
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field, root_validator
+from typing_extensions import Literal
 
 
 class ExampleBase(BaseModel):
     """Example base model."""
 
     dataset_id: UUID
     inputs: Dict[str, Any]
@@ -82,15 +83,15 @@
 
 class RunBase(BaseModel):
     """Base Run schema."""
 
     id: Optional[UUID]
     start_time: datetime = Field(default_factory=datetime.utcnow)
     end_time: datetime = Field(default_factory=datetime.utcnow)
-    extra: dict
+    extra: dict = Field(default_factory=dict)
     error: Optional[str]
     execution_order: int
     child_execution_order: Optional[int]
     serialized: dict
     inputs: dict
     outputs: Optional[dict]
     reference_example_id: Optional[UUID]
@@ -108,14 +109,22 @@
     def assign_name(cls, values: dict) -> dict:
         """Assign name to the run."""
         if "name" not in values:
             values["name"] = values["serialized"]["name"]
         return values
 
 
+class RunUpdate(BaseModel):
+    end_time: Optional[datetime]
+    error: Optional[str]
+    outputs: Optional[dict]
+    parent_run_id: Optional[UUID]
+    reference_example_id: Optional[UUID]
+
+
 class ListRunsQueryParams(BaseModel):
     """Query params for GET /runs endpoint."""
 
     id: Optional[List[UUID]]
     """Filter runs by id."""
     parent_run: Optional[UUID]
     """Filter runs by parent run."""
@@ -155,31 +164,31 @@
         end_time = values.get("end_time")
         if start_time and end_time and start_time > end_time:
             raise ValueError("start_time must be <= end_time")
         return values
 
 
 class FeedbackSourceBase(BaseModel):
-    type: ClassVar[str]
-    metadata: Dict[str, Any] | None = None
+    type: str
+    metadata: Optional[Dict[str, Any]] = None
 
     class Config:
         frozen = True
 
 
 class APIFeedbackSource(FeedbackSourceBase):
     """API feedback source."""
 
-    type: ClassVar[str] = "api"
+    type: Literal["api"] = "api"
 
 
 class ModelFeedbackSource(FeedbackSourceBase):
     """Model feedback source."""
 
-    type: ClassVar[str] = "model"
+    type: Literal["model"] = "model"
 
 
 class FeedbackSourceType(Enum):
     """Feedback source type."""
 
     API = "api"
     """General feedback submitted from the API."""
```

### Comparing `langchainplus_sdk-0.0.1rc1/pyproject.toml` & `langchainplus_sdk-0.0.1rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.1-rc1"
+version = "0.0.1-rc3"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
 [tool.poetry.dependencies]
```

### Comparing `langchainplus_sdk-0.0.1rc1/PKG-INFO` & `langchainplus_sdk-0.0.1rc3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchainplus-sdk
-Version: 0.0.1rc1
+Version: 0.0.1rc3
 Summary: Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,18 @@
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Description-Content-Type: text/markdown
 
 # LangChainPlus Client SDK
 
-This package contains the Python client for interacting with the LangChainPlus platform.
+This package contains the Python client for interacting with the [LangChainPlus platform](https://www.langchain.plus/).
 
 LangChainPlus helps you and your team develop and evaluate language models and intelligent agents. It works
 with any LLM Application, including a seamless integration with [LangChain](https://github.com/hwchase17/langchain), a widely recognized open-source framework that simplifies the process for developers to create powerful language model applications.
 
 LangChainPlus is developed and maintained by [LangChain](https://langchain.com/), the company behind the LangChain framework.
 
 
+## Documentation
+
+To learn more about the LangChainPlus platform, check out the [docs](https://docs.langchain.plus/docs/)
```

