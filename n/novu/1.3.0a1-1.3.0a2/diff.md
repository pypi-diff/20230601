# Comparing `tmp/novu-1.3.0a1.tar.gz` & `tmp/novu-1.3.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novu-1.3.0a1.tar", max compression
+gzip compressed data, was "novu-1.3.0a2.tar", max compression
```

## Comparing `novu-1.3.0a1.tar` & `novu-1.3.0a2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1079 2023-05-25 16:55:32.086368 novu-1.3.0a1/LICENSE
--rw-r--r--   0        0        0     2297 2023-05-25 16:55:32.086368 novu-1.3.0a1/README.md
--rw-r--r--   0        0        0      475 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/__init__.py
--rw-r--r--   0        0        0     2209 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/base.py
--rw-r--r--   0        0        0     2263 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/change.py
--rw-r--r--   0        0        0     2148 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/environment.py
--rw-r--r--   0        0        0     8377 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/event.py
--rw-r--r--   0        0        0     1293 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/execution_detail.py
--rw-r--r--   0        0        0     1457 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/feed.py
--rw-r--r--   0        0        0     3690 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/integration.py
--rw-r--r--   0        0        0     2681 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/layout.py
--rw-r--r--   0        0        0     1927 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/message.py
--rw-r--r--   0        0        0     1391 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/notification_group.py
--rw-r--r--   0        0        0     4121 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/notification_template.py
--rw-r--r--   0        0        0     7163 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/subscriber.py
--rw-r--r--   0        0        0     3910 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/api/topic.py
--rw-r--r--   0        0        0      745 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/config.py
--rw-r--r--   0        0        0      637 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/constants.py
--rw-r--r--   0        0        0     2576 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/__init__.py
--rw-r--r--   0        0        0     5825 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/base.py
--rw-r--r--   0        0        0     2156 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/change.py
--rw-r--r--   0        0        0     1942 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/environment.py
--rw-r--r--   0        0        0     1269 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/event.py
--rw-r--r--   0        0        0     2185 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/execution_detail.py
--rw-r--r--   0        0        0     1066 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/feed.py
--rw-r--r--   0        0        0     1213 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/field.py
--rw-r--r--   0        0        0     1942 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/integration.py
--rw-r--r--   0        0        0     2672 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/layout.py
--rw-r--r--   0        0        0     3107 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/message.py
--rw-r--r--   0        0        0     1449 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/notification_group.py
--rw-r--r--   0        0        0     8288 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/notification_template.py
--rw-r--r--   0        0        0      865 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/step_filter.py
--rw-r--r--   0        0        0     4565 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/subscriber.py
--rw-r--r--   0        0        0     1491 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/dto/topic.py
--rw-r--r--   0        0        0     1425 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/__init__.py
--rw-r--r--   0        0        0      635 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/change.py
--rw-r--r--   0        0        0     1542 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/channel.py
--rw-r--r--   0        0        0      547 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/event.py
--rw-r--r--   0        0        0     1002 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/execution.py
--rw-r--r--   0        0        0     2171 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/field.py
--rw-r--r--   0        0        0      723 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/notification.py
--rw-r--r--   0        0        0     4038 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/provider.py
--rw-r--r--   0        0        0      762 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/step_filter.py
--rw-r--r--   0        0        0      371 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/enums/template.py
--rw-r--r--   0        0        0     1263 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/helpers.py
--rw-r--r--   0        0        0        0 2023-05-25 16:55:32.086368 novu-1.3.0a1/novu/py.typed
--rw-r--r--   0        0        0     2589 2023-05-25 16:55:32.090368 novu-1.3.0a1/pyproject.toml
--rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 novu-1.3.0a1/setup.py
--rw-r--r--   0        0        0     3927 1970-01-01 00:00:00.000000 novu-1.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-01 09:35:18.163324 novu-1.3.0a2/LICENSE
+-rw-r--r--   0        0        0     2297 2023-06-01 09:35:18.163324 novu-1.3.0a2/README.md
+-rw-r--r--   0        0        0      475 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/__init__.py
+-rw-r--r--   0        0        0     1079 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/__init__.py
+-rw-r--r--   0        0        0     2814 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/base.py
+-rw-r--r--   0        0        0     2475 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/change.py
+-rw-r--r--   0        0        0     2360 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/environment.py
+-rw-r--r--   0        0        0     8589 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/event.py
+-rw-r--r--   0        0        0     1505 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/execution_detail.py
+-rw-r--r--   0        0        0     1669 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/feed.py
+-rw-r--r--   0        0        0     1165 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/inbound_parse.py
+-rw-r--r--   0        0        0     3902 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/integration.py
+-rw-r--r--   0        0        0     2893 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/layout.py
+-rw-r--r--   0        0        0     2139 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/message.py
+-rw-r--r--   0        0        0     1603 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/notification_group.py
+-rw-r--r--   0        0        0     4333 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/notification_template.py
+-rw-r--r--   0        0        0     7375 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/subscriber.py
+-rw-r--r--   0        0        0     4122 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/api/topic.py
+-rw-r--r--   0        0        0      745 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/config.py
+-rw-r--r--   0        0        0      682 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/constants.py
+-rw-r--r--   0        0        0     2576 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/__init__.py
+-rw-r--r--   0        0        0     5825 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/base.py
+-rw-r--r--   0        0        0     2156 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/change.py
+-rw-r--r--   0        0        0     1942 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/environment.py
+-rw-r--r--   0        0        0     1269 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/event.py
+-rw-r--r--   0        0        0     2185 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/execution_detail.py
+-rw-r--r--   0        0        0     1066 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/feed.py
+-rw-r--r--   0        0        0     1213 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/field.py
+-rw-r--r--   0        0        0     1942 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/integration.py
+-rw-r--r--   0        0        0     2672 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/layout.py
+-rw-r--r--   0        0        0     3107 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/message.py
+-rw-r--r--   0        0        0     1449 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/notification_group.py
+-rw-r--r--   0        0        0     8288 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/notification_template.py
+-rw-r--r--   0        0        0      865 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/step_filter.py
+-rw-r--r--   0        0        0     4565 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/subscriber.py
+-rw-r--r--   0        0        0     1491 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/dto/topic.py
+-rw-r--r--   0        0        0     1425 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/__init__.py
+-rw-r--r--   0        0        0      635 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/change.py
+-rw-r--r--   0        0        0     1542 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/channel.py
+-rw-r--r--   0        0        0      547 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/event.py
+-rw-r--r--   0        0        0     1002 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/execution.py
+-rw-r--r--   0        0        0     2171 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/field.py
+-rw-r--r--   0        0        0      723 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/notification.py
+-rw-r--r--   0        0        0     4038 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/provider.py
+-rw-r--r--   0        0        0      762 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/step_filter.py
+-rw-r--r--   0        0        0      371 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/enums/template.py
+-rw-r--r--   0        0        0     1263 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:35:18.163324 novu-1.3.0a2/novu/py.typed
+-rw-r--r--   0        0        0     2589 2023-06-01 09:35:18.163324 novu-1.3.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 novu-1.3.0a2/setup.py
+-rw-r--r--   0        0        0     3927 1970-01-01 00:00:00.000000 novu-1.3.0a2/PKG-INFO
```

### Comparing `novu-1.3.0a1/LICENSE` & `novu-1.3.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/README.md` & `novu-1.3.0a2/README.md`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/api/__init__.py` & `novu-1.3.0a2/novu/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 In this SDK, we choose to split the Novu API by business resource to simplify its complexity.
 """
 from novu.api.change import ChangeApi
 from novu.api.environment import EnvironmentApi
 from novu.api.event import EventApi
 from novu.api.execution_detail import ExecutionDetailApi
 from novu.api.feed import FeedApi
+from novu.api.inbound_parse import InboundParseApi
 from novu.api.integration import IntegrationApi
 from novu.api.layout import LayoutApi
 from novu.api.message import MessageApi
 from novu.api.notification_group import NotificationGroupApi
 from novu.api.notification_template import NotificationTemplateApi
 from novu.api.subscriber import SubscriberApi
 from novu.api.topic import TopicApi
 
 __all__ = [
     "ChangeApi",
     "EnvironmentApi",
     "EventApi",
     "ExecutionDetailApi",
     "FeedApi",
+    "InboundParseApi",
     "IntegrationApi",
     "LayoutApi",
     "MessageApi",
     "NotificationGroupApi",
     "NotificationTemplateApi",
     "SubscriberApi",
     "TopicApi",
```

### Comparing `novu-1.3.0a1/novu/api/base.py` & `novu-1.3.0a2/novu/api/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 """This module is used to defined an abstract class for all reusable methods to communicate with the Novu API"""
 import copy
 import logging
+import os
 from json.decoder import JSONDecodeError
 from typing import Optional
 
 import requests
 
 from novu.config import NovuConfig
 from novu.helpers import SentryProxy
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Api:  # pylint: disable=R0903
     """Base class for all API in the Novu client"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
+    requests_timeout: int = 5
+    """This field allow you to change the :param:`~requests.request.timeout` params which is used during API calls."""
+
+    session: Optional[requests.Session] = None
+    """This field allow you to use a :class:`~requests.Session` during API calls."""
+
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
         config = NovuConfig()
 
         url = url or config.url
         api_key = api_key or config.api_key
 
         self._url = url
         self._headers = {"Authorization": f"ApiKey {api_key}"}
 
+        self.requests_timeout = requests_timeout or int(os.getenv("NOVU_PYTHON_REQUESTS_TIMEOUT", "5"))
+        self.session = session
+
     def handle_request(
         self,
         method: str,
         url: str,
         json: Optional[dict] = None,
         payload: Optional[dict] = None,
         headers: Optional[dict] = None,
@@ -50,21 +66,21 @@
         """
         if headers:
             _headers = copy.deepcopy(self._headers)
             _headers.update(copy.deepcopy(headers))
         else:
             _headers = self._headers
 
-        res: requests.Response = requests.request(
+        res = (self.session.request if self.session else requests.request)(
             method=method,
             url=url,
             headers=_headers,
             json=json,
             params=payload,
-            timeout=5,
+            timeout=self.requests_timeout,
             **kwargs,
         )
 
         if not res.ok:
             try:
                 detail = res.json()
                 SentryProxy().set_extra("error_details", detail)
```

### Comparing `novu-1.3.0a1/novu/api/change.py` & `novu-1.3.0a2/novu/api/change.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
 This module is used to define the ``ChangeApi``, a python wrapper to interact with ``Changes`` in Novu.
 """
 from typing import Dict, Generator, List, Optional, Union
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import CHANGES_ENDPOINT
 from novu.dto.change import ChangeDto, PaginatedChangeDto
 
 
 class ChangeApi(Api):
     """This class aims to handle all API methods around changes in API"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._change_url = f"{self._url}{CHANGES_ENDPOINT}"
 
     def list(self, page: Optional[int] = None, limit: Optional[int] = None) -> PaginatedChangeDto:
         """List existing changes
 
         Args:
```

### Comparing `novu-1.3.0a1/novu/api/environment.py` & `novu-1.3.0a2/novu/api/environment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
 This module is used to define the ``EnvironmentApi``, a python wrapper to interact with ``Environments`` in Novu.
 """
 from typing import Dict, Iterator, Optional
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import ENVIRONMENTS_ENDPOINT
 from novu.dto import EnvironmentApiKeyDto, EnvironmentDto
 
 
 class EnvironmentApi(Api):
     """This class aims to handle all API methods around environments in Novu"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._environment_url = f"{self._url}{ENVIRONMENTS_ENDPOINT}"
 
     def list(self) -> Iterator[EnvironmentDto]:
         """List existing environments
 
         Yields:
```

### Comparing `novu-1.3.0a1/novu/api/event.py` & `novu-1.3.0a2/novu/api/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """
 This module is used to define the ``EventApi``, a python wrapper to interact with ``Events`` in Novu.
 """
 from collections.abc import Iterable
 from typing import Dict, Iterable as _Iterable, List, Optional, Union
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import EVENTS_ENDPOINT
 from novu.dto.event import EventDto, InputEventDto
 from novu.dto.topic import TriggerTopicDto
 
 
 class EventApi(Api):
     """This class aims to handle all API methods around events in Novu"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._event_url = f"{self._url}{EVENTS_ENDPOINT}"
 
     def trigger(
         self,
         name: str,
         recipients: Union[str, List[str]],
```

### Comparing `novu-1.3.0a1/novu/api/execution_detail.py` & `novu-1.3.0a2/novu/api/execution_detail.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """
 This module is used to define the ``ExecutionDetailApi``, a python wrapper
 to interact with ``ExecutionDetails`` in Novu.
 """
 from typing import Iterator, Optional
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import EXECUTION_DETAILS_ENDPOINT
 from novu.dto import ExecutionDetailDto
 
 
 class ExecutionDetailApi(Api):
     """This class aims to handle all API methods around execution details in Novu"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._execution_detail_url = f"{self._url}{EXECUTION_DETAILS_ENDPOINT}"
 
     def list(self, notification_id: str, subscriber_id: str) -> Iterator[ExecutionDetailDto]:
         """List existing execution details using provided notification and subscriber IDs
 
         Args:
```

### Comparing `novu-1.3.0a1/novu/api/integration.py` & `novu-1.3.0a2/novu/api/integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """
 This module is used to define the ``IntregrationApi``, a python wrapper to interact with ``Intregrations`` in Novu.
 """
 from typing import Iterator, Optional
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import INTEGRATIONS_ENDPOINT
 from novu.dto.integration import IntegrationChannelUsageDto, IntegrationDto
 from novu.enums import Channel, ProviderIdEnum
 
 
 class IntegrationApi(Api):
     """This class aims to handle all API methods around integrations in API"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._integration_url = f"{self._url}{INTEGRATIONS_ENDPOINT}"
 
     def list(self, only_active: bool = False) -> Iterator[IntegrationDto]:
         """List configured integrations
 
         Args:
```

### Comparing `novu-1.3.0a1/novu/api/layout.py` & `novu-1.3.0a2/novu/api/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
 This module is used to define the ``LayoutApi``, a python wrapper to interact with ``Layouts`` in Novu.
 """
 from typing import Optional
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import LAYOUTS_ENDPOINT
 from novu.dto.layout import LayoutDto, PaginatedLayoutDto
 
 
 class LayoutApi(Api):
     """This class aims to handle all API methods around layout in API"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._layout_url = f"{self._url}{LAYOUTS_ENDPOINT}"
 
     def list(self, page: Optional[int] = None, limit: Optional[int] = None) -> PaginatedLayoutDto:
         """List existing layouts
 
         Args:
```

### Comparing `novu-1.3.0a1/novu/api/message.py` & `novu-1.3.0a2/novu/api/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
 This module is used to define the ``MessageApi``, a python wrapper to interact with ``Messages`` in Novu.
 """
 from typing import Dict, Optional, Union
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import MESSAGES_ENDPOINT
 from novu.dto.message import PaginatedMessageDto
 
 
 class MessageApi(Api):
     """This class aims to handle all API methods around messages in Novu"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._message_url = f"{self._url}{MESSAGES_ENDPOINT}"
 
     def list(
         self, limit: int = 10, page: int = 0, channel: Optional[str] = None, subscriber_id: Optional[str] = None
     ) -> PaginatedMessageDto:
         """List messages
```

### Comparing `novu-1.3.0a1/novu/api/notification_group.py` & `novu-1.3.0a2/novu/api/notification_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """
 This module is used to define the ``NotificationGroupApi``, a python wrapper
 to interact with ``NotificationGroup`` in Novu.
 """
 from typing import Optional
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import NOTIFICATION_GROUPS_ENDPOINT
 from novu.dto.notification_group import (
     NotificationGroupDto,
     PaginatedNotificationGroupDto,
 )
 
 
 class NotificationGroupApi(Api):
     """This class aims to handle all API methods around notification groups in API"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._notification_group_url = f"{self._url}{NOTIFICATION_GROUPS_ENDPOINT}"
 
     def list(self) -> PaginatedNotificationGroupDto:
         """Method to list notification groups
 
         Returns:
```

### Comparing `novu-1.3.0a1/novu/api/notification_template.py` & `novu-1.3.0a2/novu/api/notification_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 """
 This module is used to define the ``NotificationTemplateApi``, a python wrapper
 to interact with ``NotificationTemplate`` in Novu.
 """
 from typing import Optional
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import NOTIFICATION_TEMPLATES_ENDPOINT
 from novu.dto.notification_template import (
     NotificationTemplateDto,
     NotificationTemplateFormDto,
     PaginatedNotificationTemplateDto,
 )
 
 
 class NotificationTemplateApi(Api):
     """This class aims to handle all API methods around notification templates in API"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._notification_template_url = f"{self._url}{NOTIFICATION_TEMPLATES_ENDPOINT}"
 
     def list(self, page: Optional[int] = None, limit: Optional[int] = None) -> PaginatedNotificationTemplateDto:
         """Method to list notification templates
 
         Returns:
```

### Comparing `novu-1.3.0a1/novu/api/subscriber.py` & `novu-1.3.0a2/novu/api/subscriber.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 """
 This module is used to define the ``SubscriberApi``, a python wrapper to interact with ``Subscribers`` in Novu.
 """
 from typing import Dict, Iterator, List, Optional, Union
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import SUBSCRIBERS_ENDPOINT
 from novu.dto.subscriber import (
     PaginatedSubscriberDto,
     SubscriberDto,
     SubscriberPreferenceDto,
 )
 from novu.enums import Channel
 
 
 class SubscriberApi(Api):
     """This class aims to handle all API methods around subscribers in API"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._subscriber_url = f"{self._url}{SUBSCRIBERS_ENDPOINT}"
 
     def list(self, page: Optional[int] = None) -> PaginatedSubscriberDto:
         """Method to list subscriber
 
         Args:
```

### Comparing `novu-1.3.0a1/novu/api/topic.py` & `novu-1.3.0a2/novu/api/topic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
 This module is used to define the ``TopicApi``, a python wrapper to interact with ``Topics`` in Novu.
 """
 from typing import Dict, List, Optional, Tuple, Union
 
+import requests
+
 from novu.api.base import Api
 from novu.constants import TOPICS_ENDPOINT
 from novu.dto.topic import PaginatedTopicDto, TopicDto
 
 
 class TopicApi(Api):
     """This class aims to handle all API methods around topics in API"""
 
-    def __init__(self, url: Optional[str] = None, api_key: Optional[str] = None) -> None:
-        super().__init__(url, api_key)
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        requests_timeout: Optional[int] = None,
+        session: Optional[requests.Session] = None,
+    ) -> None:
+        super().__init__(url=url, api_key=api_key, requests_timeout=requests_timeout, session=session)
 
         self._topic_url = f"{self._url}{TOPICS_ENDPOINT}"
 
     def list(
         self, page: Optional[int] = None, limit: Optional[int] = None, key: Optional[str] = None
     ) -> PaginatedTopicDto:
         """List existing topics
```

### Comparing `novu-1.3.0a1/novu/config.py` & `novu-1.3.0a2/novu/config.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/constants.py` & `novu-1.3.0a2/novu/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module is used to gather all constants and magic number used in the Novu client."""
 
 CHANGES_ENDPOINT = "/v1/changes"
 ENVIRONMENTS_ENDPOINT = "/v1/environments"
 EVENTS_ENDPOINT = "/v1/events/trigger"
 EXECUTION_DETAILS_ENDPOINT = "/v1/execution-details"
 FEEDS_ENDPOINT = "/v1/feeds"
+INBOUND_PARSE_ENDPOINT = "/v1/inbound-parse"
 INTEGRATIONS_ENDPOINT = "/v1/integrations"
 LAYOUTS_ENDPOINT = "/v1/layouts"
 MESSAGES_ENDPOINT = "/v1/messages"
 NOTIFICATION_GROUPS_ENDPOINT = "/v1/notification-groups"
 NOTIFICATION_TEMPLATES_ENDPOINT = "/v1/notification-templates"
 SUBSCRIBERS_ENDPOINT = "/v1/subscribers"
 TOPICS_ENDPOINT = "/v1/topics"
```

### Comparing `novu-1.3.0a1/novu/dto/__init__.py` & `novu-1.3.0a2/novu/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/base.py` & `novu-1.3.0a2/novu/dto/base.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/change.py` & `novu-1.3.0a2/novu/dto/change.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/environment.py` & `novu-1.3.0a2/novu/dto/environment.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/event.py` & `novu-1.3.0a2/novu/dto/event.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/execution_detail.py` & `novu-1.3.0a2/novu/dto/execution_detail.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/feed.py` & `novu-1.3.0a2/novu/dto/feed.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/field.py` & `novu-1.3.0a2/novu/dto/field.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/integration.py` & `novu-1.3.0a2/novu/dto/integration.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/layout.py` & `novu-1.3.0a2/novu/dto/layout.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/message.py` & `novu-1.3.0a2/novu/dto/message.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/notification_group.py` & `novu-1.3.0a2/novu/dto/notification_group.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/notification_template.py` & `novu-1.3.0a2/novu/dto/notification_template.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/step_filter.py` & `novu-1.3.0a2/novu/dto/step_filter.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/subscriber.py` & `novu-1.3.0a2/novu/dto/subscriber.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/dto/topic.py` & `novu-1.3.0a2/novu/dto/topic.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/__init__.py` & `novu-1.3.0a2/novu/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/change.py` & `novu-1.3.0a2/novu/enums/change.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/channel.py` & `novu-1.3.0a2/novu/enums/channel.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/event.py` & `novu-1.3.0a2/novu/enums/event.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/execution.py` & `novu-1.3.0a2/novu/enums/execution.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/field.py` & `novu-1.3.0a2/novu/enums/field.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/notification.py` & `novu-1.3.0a2/novu/enums/notification.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/provider.py` & `novu-1.3.0a2/novu/enums/provider.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/enums/step_filter.py` & `novu-1.3.0a2/novu/enums/step_filter.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/novu/helpers.py` & `novu-1.3.0a2/novu/helpers.py`

 * *Files identical despite different names*

### Comparing `novu-1.3.0a1/pyproject.toml` & `novu-1.3.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 description = "This project aims to provide a wrapper for the Novu API."
 keywords = ["novu", "python", "sdk", "api", "wrapper"]
 name = "novu"
-version = "1.3.0-alpha.1"
+version = "1.3.0-alpha.2"
 
 documentation = "https://novu-python.readthedocs.io/en/latest"
 homepage = "https://novu-python.readthedocs.io/en/latest"
 repository = "https://github.com/novuhq/novu-python"
 
 authors = ["oscar.marie-taillefer <oscar.marie-taillefer@spikeelabs.fr>"]
 maintainers = ["oscar.marie-taillefer <oscar.marie-taillefer@spikeelabs.fr>"]
```

### Comparing `novu-1.3.0a1/setup.py` & `novu-1.3.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'novu',
-    'version': '1.3.0a1',
+    'version': '1.3.0a2',
     'description': 'This project aims to provide a wrapper for the Novu API.',
     'long_description': '# Python Novu SDK\n\n[![PyPI](https://img.shields.io/pypi/v/novu?color=blue)](https://pypi.org/project/novu/)\n![Tests Status](https://github.com/novuhq/novu-python/actions/workflows/.github/workflows/tests.yml/badge.svg)\n[![codecov](https://codecov.io/gh/novuhq/novu-python/branch/main/graph/badge.svg?token=RON7F8QTZX)](https://codecov.io/gh/novuhq/novu-python)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/novu)\n![PyPI - License](https://img.shields.io/pypi/l/novu)\n[![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)\n\n---\n\nThe [Python Novu](https://novu.co) SDK and package provides a fluent and expressive interface for interacting with [Novu\'s API](https://api.novu.co/api) and managing notifications.\n\n## Install\n\nTo install this package\n\n```shell\n# Via pip\npip install novu\n\n# Via poetry\npoetry add novu\n```\n\n## Quick start\n\nThis package is a wrapper of all the resources offered by Novu, we will just start by triggering an event on Novu.\n\nTo do this, you will need to:\n\n1. Create your first notification template and keep in mind the identifier to trigger the template: https://docs.novu.co/overview/quick-start#create-a-notification-template\n2. Retrieve your API key from the Novu dashboard directly in the settings section: https://web.novu.co/settings\n3. Write code to trigger your first event:\n\n```python\nfrom novu.api import EventApi\n\nevent_api = EventApi("https://api.novu.co/api/", "<NOVU_API_TOKEN>")\nevent_api.trigger(\n    name="<YOUR_TEMPLATE_NAME>",\n    recipients="<YOUR_SUBSCRIBER_ID>",\n    payload={},  # Your Novu payload goes here\n)\n```\n\nThis will trigger a notification to the subscribers.\n\n## Development\n\n```bash\n# install deps\npoetry install\n\n# pre-commit\npoetry run pre-commit install --install-hook\npoetry run pre-commit install --install-hooks --hook-type commit-msg\n```\n',
     'author': 'oscar.marie-taillefer',
     'author_email': 'oscar.marie-taillefer@spikeelabs.fr',
     'maintainer': 'oscar.marie-taillefer',
     'maintainer_email': 'oscar.marie-taillefer@spikeelabs.fr',
     'url': 'https://novu-python.readthedocs.io/en/latest',
```

### Comparing `novu-1.3.0a1/PKG-INFO` & `novu-1.3.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novu
-Version: 1.3.0a1
+Version: 1.3.0a2
 Summary: This project aims to provide a wrapper for the Novu API.
 Home-page: https://novu-python.readthedocs.io/en/latest
 License: MIT
 Keywords: novu,python,sdk,api,wrapper
 Author: oscar.marie-taillefer
 Author-email: oscar.marie-taillefer@spikeelabs.fr
 Maintainer: oscar.marie-taillefer
```

