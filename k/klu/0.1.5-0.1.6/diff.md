# Comparing `tmp/klu-0.1.5.tar.gz` & `tmp/klu-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klu-0.1.5.tar", max compression
+gzip compressed data, was "klu-0.1.6.tar", max compression
```

## Comparing `klu-0.1.5.tar` & `klu-0.1.6.tar`

### file list

```diff
@@ -1,84 +1,54 @@
--rw-r--r--   0        0        0     1070 2023-04-02 23:20:08.165888 klu-0.1.5/LICENSE
--rw-r--r--   0        0        0     2957 2023-05-26 00:37:42.513833 klu-0.1.5/README.md
--rw-r--r--   0        0        0      150 2023-05-27 14:30:24.721088 klu-0.1.5/klu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/action/__init__.py
--rw-r--r--   0        0        0    11171 2023-05-26 00:17:00.539207 klu-0.1.5/klu/action/client.py
--rw-r--r--   0        0        0      280 2023-05-27 13:56:44.465656 klu-0.1.5/klu/action/constants.py
--rw-r--r--   0        0        0      542 2023-05-01 22:54:25.386914 klu-0.1.5/klu/action/errors.py
--rw-r--r--   0        0        0     1700 2023-05-24 12:53:09.893852 klu-0.1.5/klu/action/models.py
--rw-r--r--   0        0        0        0 2023-04-16 12:33:25.776741 klu-0.1.5/klu/api/__init__.py
--rw-r--r--   0        0        0     3039 2023-05-25 23:34:25.415214 klu-0.1.5/klu/api/client.py
--rw-r--r--   0        0        0      199 2023-05-27 14:00:15.080309 klu-0.1.5/klu/api/config.py
--rw-r--r--   0        0        0      118 2023-05-25 23:21:28.634469 klu-0.1.5/klu/api/constants.py
--rw-r--r--   0        0        0     1429 2023-05-26 00:23:42.481009 klu-0.1.5/klu/api/sse_client.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648620 klu-0.1.5/klu/application/__init__.py
--rw-r--r--   0        0        0     7677 2023-05-22 23:57:57.911029 klu-0.1.5/klu/application/client.py
--rw-r--r--   0        0        0      259 2023-05-27 13:56:44.512450 klu-0.1.5/klu/application/constants.py
--rw-r--r--   0        0        0      325 2023-05-18 00:09:26.025264 klu-0.1.5/klu/application/errors.py
--rw-r--r--   0        0        0     1303 2023-05-16 01:32:56.622223 klu-0.1.5/klu/application/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/client/__init__.py
--rw-r--r--   0        0        0      794 2023-05-26 00:09:53.956182 klu-0.1.5/klu/client/klu.py
--rw-r--r--   0        0        0        0 2023-04-17 20:44:45.994154 klu-0.1.5/klu/common/__init__.py
--rw-r--r--   0        0        0     3146 2023-05-27 13:10:59.677590 klu-0.1.5/klu/common/client.py
--rw-r--r--   0        0        0     2967 2023-05-18 00:09:26.039775 klu-0.1.5/klu/common/errors.py
--rw-r--r--   0        0        0     2268 2023-05-07 22:15:35.049953 klu-0.1.5/klu/common/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/data/__init__.py
--rw-r--r--   0        0        0     2240 2023-05-17 21:42:29.875608 klu-0.1.5/klu/data/client.py
--rw-r--r--   0        0        0       25 2023-05-27 12:58:54.884230 klu-0.1.5/klu/data/constants.py
--rw-r--r--   0        0        0      281 2023-05-18 00:09:26.054468 klu-0.1.5/klu/data/errors.py
--rw-r--r--   0        0        0     2537 2023-05-16 00:57:12.476673 klu-0.1.5/klu/data/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/data_index/__init__.py
--rw-r--r--   0        0        0     8445 2023-05-22 18:49:52.214610 klu-0.1.5/klu/data_index/client.py
--rw-r--r--   0        0        0      287 2023-05-27 13:56:44.504025 klu-0.1.5/klu/data_index/constants.py
--rw-r--r--   0        0        0      316 2023-05-18 00:09:26.046973 klu-0.1.5/klu/data_index/errors.py
--rw-r--r--   0        0        0     3263 2023-05-21 21:41:28.245219 klu-0.1.5/klu/data_index/models.py
--rw-r--r--   0        0        0       19 2023-04-02 23:20:08.167789 klu-0.1.5/klu/klu.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/model/__init__.py
--rw-r--r--   0        0        0     3450 2023-05-22 18:50:10.373905 klu-0.1.5/klu/model/client.py
--rw-r--r--   0        0        0       28 2023-05-27 12:58:54.475873 klu-0.1.5/klu/model/constants.py
--rw-r--r--   0        0        0      454 2023-05-18 00:09:26.016842 klu-0.1.5/klu/model/errors.py
--rw-r--r--   0        0        0     1193 2023-05-17 00:20:41.308393 klu-0.1.5/klu/model/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/session/__init__.py
--rw-r--r--   0        0        0     1412 2023-05-16 01:10:51.006332 klu-0.1.5/klu/session/client.py
--rw-r--r--   0        0        0       32 2023-05-27 12:58:54.666310 klu-0.1.5/klu/session/constants.py
--rw-r--r--   0        0        0     1094 2023-05-16 00:57:12.477952 klu-0.1.5/klu/session/models.py
--rw-r--r--   0        0        0      111 2023-05-11 23:52:15.155255 klu-0.1.5/klu/utils/dict_helpers.py
--rw-r--r--   0        0        0      719 2023-05-01 22:31:07.149352 klu-0.1.5/klu/utils/file_upload.py
--rw-r--r--   0        0        0     2308 2023-05-22 23:37:24.956177 klu-0.1.5/klu/utils/paginator.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/klu/workspace/__init__.py
--rw-r--r--   0        0        0     7968 2023-05-23 00:00:29.836509 klu-0.1.5/klu/workspace/client.py
--rw-r--r--   0        0        0      321 2023-05-27 13:56:44.493674 klu-0.1.5/klu/workspace/constants.py
--rw-r--r--   0        0        0      244 2023-05-18 00:09:26.033318 klu-0.1.5/klu/workspace/errors.py
--rw-r--r--   0        0        0      815 2023-05-15 22:31:50.548346 klu-0.1.5/klu/workspace/models.py
--rw-r--r--   0        0        0     2820 2023-05-27 14:30:24.732873 klu-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-02 23:20:08.169124 klu-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      103 2023-05-15 22:17:30.645200 klu-0.1.5/tests/integration/__init__.py
--rw-r--r--   0        0        0      128 2023-05-26 00:17:59.829216 klu-0.1.5/tests/integration/conftest.py
--rw-r--r--   0        0        0      252 2023-05-27 14:00:25.824775 klu-0.1.5/tests/integration/constants.py
--rw-r--r--   0        0        0        0 2023-05-17 01:53:20.259063 klu-0.1.5/tests/integration/files/__init__.py
--rw-r--r--   0        0        0   108574 2021-08-07 16:43:25.870000 klu-0.1.5/tests/integration/files/test-file-upload.pdf
--rw-r--r--   0        0        0     4826 2023-05-27 14:02:35.049808 klu-0.1.5/tests/integration/test_actions.py
--rw-r--r--   0        0        0     3749 2023-05-27 14:01:15.447974 klu-0.1.5/tests/integration/test_applications.py
--rw-r--r--   0        0        0     1148 2023-05-17 01:34:42.355919 klu-0.1.5/tests/integration/test_data.py
--rw-r--r--   0        0        0     2864 2023-05-21 21:55:43.590354 klu-0.1.5/tests/integration/test_data_index.py
--rw-r--r--   0        0        0      958 2023-05-17 01:35:15.023120 klu-0.1.5/tests/integration/test_models.py
--rw-r--r--   0        0        0     2212 2023-05-27 14:01:44.839869 klu-0.1.5/tests/integration/test_workspaces.py
--rw-r--r--   0        0        0     1435 2023-05-24 12:44:20.921698 klu-0.1.5/tests/integration/utils/actions.py
--rw-r--r--   0        0        0      752 2023-05-17 01:19:00.668605 klu-0.1.5/tests/integration/utils/applications.py
--rw-r--r--   0        0        0       68 2023-05-15 22:17:30.698602 klu-0.1.5/tests/integration/utils/common.py
--rw-r--r--   0        0        0     1555 2023-05-17 01:27:25.631403 klu-0.1.5/tests/integration/utils/data.py
--rw-r--r--   0        0        0      816 2023-05-17 01:27:25.638985 klu-0.1.5/tests/integration/utils/data_index.py
--rw-r--r--   0        0        0      830 2023-05-24 23:19:18.771498 klu-0.1.5/tests/integration/utils/models.py
--rw-r--r--   0        0        0      842 2023-05-17 01:19:00.583265 klu-0.1.5/tests/integration/utils/sessions.py
--rw-r--r--   0        0        0      658 2023-05-17 01:19:00.519346 klu-0.1.5/tests/integration/utils/workspace.py
--rw-r--r--   0        0        0        0 2023-05-08 13:03:00.679856 klu-0.1.5/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/tests/unit/action/__init__.py
--rw-r--r--   0        0        0     1692 2023-05-23 00:20:51.639436 klu-0.1.5/tests/unit/action/test_client.py
--rw-r--r--   0        0        0     1156 2023-05-15 21:48:29.904995 klu-0.1.5/tests/unit/action/utils.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/tests/unit/application/__init__.py
--rw-r--r--   0        0        0     1433 2023-05-23 00:20:51.607538 klu-0.1.5/tests/unit/application/test_client.py
--rw-r--r--   0        0        0     1170 2023-05-16 00:57:16.848585 klu-0.1.5/tests/unit/application/utils.py
--rw-r--r--   0        0        0      156 2023-05-21 22:55:55.517974 klu-0.1.5/tests/unit/conftest.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.5/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      768 2023-05-01 22:56:20.546102 klu-0.1.5/tests/unit/utils/mock.py
--rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 klu-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-01 11:32:44.968401 klu-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2840 2023-06-01 11:32:44.968401 klu-0.1.6/README.md
+-rw-r--r--   0        0        0      150 2023-06-01 11:32:44.968401 klu-0.1.6/klu/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/__init__.py
+-rw-r--r--   0        0        0    11322 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/client.py
+-rw-r--r--   0        0        0      280 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/constants.py
+-rw-r--r--   0        0        0      547 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/errors.py
+-rw-r--r--   0        0        0     1980 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/models.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/__init__.py
+-rw-r--r--   0        0        0     2998 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/client.py
+-rw-r--r--   0        0        0      199 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/config.py
+-rw-r--r--   0        0        0      118 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/constants.py
+-rw-r--r--   0        0        0     1406 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/sse_client.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/__init__.py
+-rw-r--r--   0        0        0     7753 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/client.py
+-rw-r--r--   0        0        0      259 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/constants.py
+-rw-r--r--   0        0        0      318 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/errors.py
+-rw-r--r--   0        0        0     1464 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/models.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/client/__init__.py
+-rw-r--r--   0        0        0      794 2023-06-01 11:32:44.968401 klu-0.1.6/klu/client/klu.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/common/__init__.py
+-rw-r--r--   0        0        0     3086 2023-06-01 11:32:44.968401 klu-0.1.6/klu/common/client.py
+-rw-r--r--   0        0        0     2975 2023-06-01 11:32:44.968401 klu-0.1.6/klu/common/errors.py
+-rw-r--r--   0        0        0     2209 2023-06-01 11:32:44.968401 klu-0.1.6/klu/common/models.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/__init__.py
+-rw-r--r--   0        0        0     2332 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/client.py
+-rw-r--r--   0        0        0       25 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/constants.py
+-rw-r--r--   0        0        0      274 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/errors.py
+-rw-r--r--   0        0        0     3199 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/models.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/__init__.py
+-rw-r--r--   0        0        0     8672 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/client.py
+-rw-r--r--   0        0        0      287 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/constants.py
+-rw-r--r--   0        0        0      309 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/errors.py
+-rw-r--r--   0        0        0     3415 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/models.py
+-rw-r--r--   0        0        0       19 2023-06-01 11:32:44.968401 klu-0.1.6/klu/klu.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/__init__.py
+-rw-r--r--   0        0        0     3505 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/client.py
+-rw-r--r--   0        0        0       28 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/constants.py
+-rw-r--r--   0        0        0      447 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/errors.py
+-rw-r--r--   0        0        0     1397 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/models.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/session/__init__.py
+-rw-r--r--   0        0        0     1488 2023-06-01 11:32:44.968401 klu-0.1.6/klu/session/client.py
+-rw-r--r--   0        0        0       32 2023-06-01 11:32:44.968401 klu-0.1.6/klu/session/constants.py
+-rw-r--r--   0        0        0     1264 2023-06-01 11:32:44.968401 klu-0.1.6/klu/session/models.py
+-rw-r--r--   0        0        0      111 2023-06-01 11:32:44.972401 klu-0.1.6/klu/utils/dict_helpers.py
+-rw-r--r--   0        0        0      752 2023-06-01 11:32:44.972401 klu-0.1.6/klu/utils/file_upload.py
+-rw-r--r--   0        0        0     2407 2023-06-01 11:32:44.972401 klu-0.1.6/klu/utils/paginator.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/__init__.py
+-rw-r--r--   0        0        0     8052 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/client.py
+-rw-r--r--   0        0        0      321 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/constants.py
+-rw-r--r--   0        0        0      244 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/errors.py
+-rw-r--r--   0        0        0      943 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/models.py
+-rw-r--r--   0        0        0     1952 2023-06-01 11:32:44.972401 klu-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3698 1970-01-01 00:00:00.000000 klu-0.1.6/PKG-INFO
```

### Comparing `klu-0.1.5/LICENSE` & `klu-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `klu-0.1.5/README.md` & `klu-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
 Once you have a `KluClient` object, you can access the different models available in the Klu API:
 
 ```python
 from klu import KluClient
 
 client = KluClient("YOUR_API_KEY")
-
 models = await client.models.get("model_guid")
 
 ```
 
 There is also a separate function to stream action prompt
 
 Each of these objects provides methods for interacting with the corresponding model in the Klu API. For example, to list all applications in your workspace, you can use:
@@ -78,17 +77,12 @@
 client = KluClient("YOUR_API_KEY")
 
 prompt_response = await client.actions.run_action_prompt("action_guid", "prompt", streaming=True)
 async for message in client.sse_client.get_streaming_data(prompt_response.streaming_url):
     print(message)
 ```
 
-## Development
-For more detailed developer information, please refer to the [Developer's README](README.dev.md).
-
 ## Documentation
-
 For more detailed information on how to use the Klu.AI Python SDK, please refer to the [API documentation](https://docs.klu.ai/).
 
 ## Credits
-
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.
```

### Comparing `klu-0.1.5/klu/action/client.py` & `klu-0.1.6/klu/action/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import aiohttp
-
-from typing import Optional, List
+# mypy: disable-error-code="override"
+from typing import List, Optional
 
+import aiohttp
 from aiohttp import ClientResponseError
-from aiohttp.web_exceptions import HTTPNotFound
 
-from klu.common.errors import (
-    UnknownKluError,
-    UnknownKluAPIError,
-    InvalidUpdateParamsError,
-)
 from klu.action.constants import (
-    ACTION_ENDPOINT,
     ACTION_DATA_ENDPOINT,
+    ACTION_ENDPOINT,
     CREATE_ACTION_ENDPOINT,
-    PLAYGROUND_PROMPT_ENDPOINT,
     DEFAULT_ACTIONS_PAGE_SIZE,
+    PLAYGROUND_PROMPT_ENDPOINT,
 )
-from klu.data.models import Data
-from klu.utils.paginator import Paginator
+from klu.action.errors import ActionNotFoundError, InvalidActionPromptData
+from klu.action.models import Action, PromptResponse
 from klu.common.client import KluClientBase
+from klu.common.errors import (
+    InvalidUpdateParamsError,
+    UnknownKluAPIError,
+    UnknownKluError,
+)
+from klu.data.models import Data
 from klu.utils.dict_helpers import dict_no_empty
-from klu.action.models import PromptResponse, Action
+from klu.utils.paginator import Paginator
 from klu.workspace.errors import WorkspaceOrUserNotFoundError
-from klu.action.errors import ActionNotFoundError, InvalidActionPromptData
 
 
 class ActionsClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, ACTION_ENDPOINT, Action)
         self._paginator = Paginator(ACTION_ENDPOINT)
 
+    # type: ignore
     async def create(
         self,
         name: str,
         prompt: str,
         app_guid: str,
-        model_guid: int,
+        model_guid: str,
         action_type: str,
         description: str,
         model_config: Optional[dict] = None,
     ) -> Action:
         """
         Creates new action instance
 
@@ -49,85 +49,91 @@
             prompt (str): Action prompt
             model_guid (int): Guid of a model used for action
             app_guid (str): GUID of the application for an action to be attached to
             action_type (str): The type of the action. Can be one of [simple, complex, document-search, full-ai, custom]
             description (str): The description of the action
             model_config (str): Optional action model configuration dict
 
-        Returns: Newly created Action object
+        Returns:
+            Newly created Action object
         """
         return await super().create(
             name=name,
             prompt=prompt,
             app_guid=app_guid,
             model_guid=model_guid,
             agent_type=action_type,
             description=description,
             model_config=model_config,
             url=CREATE_ACTION_ENDPOINT,
         )
 
-    async def get(self, id: str) -> Action:
+    # type: ignore
+    async def get(self, guid: str) -> Action:
         """
         Get an action defined by the id
 
         Args:
-            id (str): The id of an action to retrieve
+            guid (str): The id of an action to retrieve
 
-        Returns: Retrieved Action object.
+        Returns:
+            Retrieved Action object.
         """
-        return await super().get(id)
+        return await super().get(guid)
 
+    # type: ignore
     async def update(
         self,
         guid: str,
         name: Optional[str] = None,
         prompt: Optional[str] = None,
         description: Optional[str] = None,
         model_config: Optional[str] = None,
     ) -> Action:
         """
         Update action instance with provided data. At least one of parameters should be present.
 
         Args:
-            guid (str) The GUID of the action to update
-            name: Optional[str]. New action name
-            prompt: Optional[str]. New action type
-            description: Optional[str]. New action description
-            model_config: Optional[dict]. New action model_config
+            guid (str): The GUID of the action to update.
+            name: Optional[str]. New action name.
+            prompt: Optional[str]. New action type.
+            description: Optional[str]. New action description.
+            model_config: Optional[dict]. New action model_config.
 
-        Returns: Action with updated data
+        Returns:
+            Action with updated data
         """
         if not name and not prompt and not description and not model_config:
             raise InvalidUpdateParamsError()
 
         return await super().update(
             **{
-                "id": guid,
+                "guid": guid,
                 **dict_no_empty(
                     {
                         "name": name,
                         "prompt": prompt,
                         "description": description,
                         "model_config": model_config,
                     }
                 ),
             }
         )
 
-    async def delete(self, id: str) -> Action:
+    async def delete(self, guid: str) -> Action:
         """
         Delete an action defined by the id
 
         Args:
-            id (str): The id of an action to delete
+            guid (str): The id of an action to delete
 
-        Returns: Deleted Action object.
+        Returns:
+            Deleted Action object.
         """
-        return await super().delete(id)
+        return await super().delete(guid)
 
     async def run_action_prompt(
         self,
         action_guid: str,
         prompt: str,
         filter: Optional[str] = None,
         streaming: Optional[bool] = False,
@@ -141,15 +147,16 @@
             action_guid (str): The GUID of the agent to run the prompt with.
             prompt (str): The prompt to run with the agent.
             filter (Optional[str]): The filter to use when running the prompt.
             session_guid (Optional[str]): The GUID of the session to run the prompt with.
             streaming (Optional[bool]): Flag that defines whether to use streaming or not.
             async_mode (Optional[bool]): Boolean that identifies whether the async mode should be used. Defaults to False.
 
-        Returns: An object result of running the prompt with the message and a feedback_url for providing feedback.
+        Returns:
+            An object result of running the prompt with the message and a feedback_url for providing feedback.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
 
             try:
                 response = await client.post(
                     ACTION_ENDPOINT,
@@ -159,15 +166,15 @@
                         "action": action_guid,
                         "streaming": streaming,
                         "async_mode": async_mode,
                         "sessionGuid": session_guid,
                     },
                 )
                 return PromptResponse(**response)
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise ActionNotFoundError(action_guid)
 
                 raise UnknownKluAPIError(e.status, e.message)
             except Exception:
                 raise UnknownKluError()
 
@@ -185,15 +192,16 @@
         Args:
             prompt (str): The prompt to run.
             model_id (int): The ID of the model to use. Can be retrieved by querying the model by guid
             tool_ids (list): Optional list of tool IDs to use. Defaults to an empty array
             index_ids (list): Optional list of index IDs to use. Defaults to an empty array
             model_config (dict): Optional configuration of the model
 
-        Returns: An object result of running the prompt with the message and a feedback_url for providing feedback.
+        Returns:
+            An object result of running the prompt with the message and a feedback_url for providing feedback.
         """
         tool_ids = tool_ids or []
         index_ids = index_ids or []
 
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
 
@@ -205,15 +213,15 @@
                         "toolIds": tool_ids,
                         "modelId": model_id,
                         "indexIds": index_ids,
                         "modelConfig": model_config,
                     },
                 )
                 return PromptResponse(**response)
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise WorkspaceOrUserNotFoundError()
                 if e.status == 400:
                     raise InvalidActionPromptData(e.message)
 
                 raise UnknownKluAPIError(e.status, e.message)
             except Exception:
@@ -222,36 +230,37 @@
     async def get_action_data(self, guid: str) -> List[Data]:
         """
         Retrieves data information for an action.
 
         Args:
             guid (str): Guid of an action to fetch data for.
 
-        Returns: An array of actions found by provided app id.
+        Returns:
+            An array of actions found by provided app id.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
 
             try:
                 response = await client.get(ACTION_DATA_ENDPOINT.format(id=guid))
                 return [Data._from_engine_format(data) for data in response]
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise ActionNotFoundError(guid)
 
                 raise UnknownKluAPIError(e.status, e.message)
             except Exception:
                 raise UnknownKluError()
 
     async def list(self) -> List[Action]:
         """
         Retrieves all actions for a user represented by the used API_KEY.
         Does not rely on internal paginator state, so `reset_pagination` method call can be skipped
 
-        Returns: An array of all actions
+        Returns (List[Action]): An array of all actions
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_all(client)
 
             return [Action._from_engine_format(action) for action in response]
 
@@ -263,37 +272,39 @@
         Can be used to fetch a specific page of actions provided a certain per_page config.
         Does not rely on internal paginator state, so `reset_pagination` method call can be skipped
 
         Args:
             page_number (int): Number of the page to fetch
             limit (int): Number of instances to fetch per page. Defaults to 50
 
-        Returns: An array of actions fetched for a queried page. Empty if queried page does not exist
+        Returns:
+            An array of actions fetched for a queried page. Empty if queried page does not exist
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_single_page(
                 client, page_number, limit=limit
             )
 
             return [Action._from_engine_format(action) for action in response]
 
     async def fetch_next_page(
-        self, limit: int = DEFAULT_ACTIONS_PAGE_SIZE, offset: int = None
+        self, limit: int = DEFAULT_ACTIONS_PAGE_SIZE, offset: Optional[int] = None
     ) -> List[Action]:
         """
         Retrieves the next page of actions. Can be used to fetch a flexible number of pages starting.
         The place to start from can be controlled by the offset parameter.
         After using this method, we suggest to call `reset_pagination` method to reset the page cursor.
 
         Args:
             limit (int): Number of instances to fetch per page. Defaults to 50
             offset (int): The number of instances to skip. Can be used to query the pages of actions skipping certain number of instances.
 
-        Returns: An array of actions fetched for a queried page. Empty if the end was reached at the previous step.
+        Returns:
+            An array of actions fetched for a queried page. Empty if the end was reached at the previous step.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_next_page(
                 client, limit=limit, offset=offset
             )
```

### Comparing `klu-0.1.5/klu/action/errors.py` & `klu-0.1.6/klu/action/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 class ActionNotFoundError(Exception):
-    application_id: str = None
+    application_id: str
 
     def __init__(self, action_id: str):
         self.application_id = action_id
         self.message = f"Action with id {action_id} was not found."
         super().__init__(self.message)
 
 
 class InvalidActionPromptData(Exception):
     def __init__(self, response_message: str):
         self.message = (
-            f"Failed to run the action due to the invalid request parameters. " f"Response message: {response_message}"
+            f"Failed to run the action due to the invalid request parameters. "
+            f"Response message: {response_message}"
         )
         super().__init__(self.message)
```

### Comparing `klu-0.1.5/klu/api/client.py` & `klu-0.1.6/klu/api/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-import aiohttp
-
 from functools import wraps
-from typing import List, Union, Optional
+from typing import List, Optional, Union
 
+import aiohttp
 from aiohttp import ClientResponseError
-from aiohttp.web_exceptions import HTTPNotFound
 
+from klu.api.config import get_api_url
 from klu.common.errors import (
-    UnknownKluError,
+    BadRequestAPIError,
+    InvalidApiMethodUsedError,
     InvalidDataSent,
     UnauthorizedError,
-    BadRequestAPIError,
     UnknownKluAPIError,
-    InvalidApiMethodUsedError,
+    UnknownKluError,
 )
-from klu.api.config import get_api_url
 
 
 def _handle_http_exception(func):
     @wraps(func)
     async def wrapper(*args, **kwargs):
         try:
             return await func(*args, **kwargs)
-        except (HTTPNotFound, ClientResponseError) as e:
+        except ClientResponseError as e:
             if e.status == 400:
                 raise BadRequestAPIError(e.status, e.message)
             if e.status == 500:
                 raise UnknownKluAPIError(e.status, e.message)
             if e.status == 401:
                 raise UnauthorizedError()
             if e.status == 405:
@@ -45,15 +43,17 @@
 class APIClient:
     def __init__(self, session: aiohttp.ClientSession, api_key: str):
         self.session = session
         self.api_url = get_api_url()
         self.headers = {"Authorization": f"Bearer {api_key}"}
 
     @_handle_http_exception
-    async def get(self, path: str, params: dict = None) -> Union[dict, List[dict]]:
+    async def get(
+        self, path: str, params: Optional[dict] = None
+    ) -> Union[dict, List[dict]]:
         url = f"{self.api_url}{path}"
         async with self.session.get(
             url, params=params, headers=self.headers
         ) as response:
             response.raise_for_status()
             return await response.json()
```

### Comparing `klu-0.1.5/klu/api/sse_client.py` & `klu-0.1.6/klu/api/sse_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
-
 from typing import AsyncIterator
 
 from aiohttp_sse_client import client as sse_client
 
 from klu.api.constants import (
+    BEGIN_STREAM_CONTENT,
     END_STREAM_CONTENT,
     NO_MESSAGES_CONTENT,
-    BEGIN_STREAM_CONTENT,
 )
 from klu.common.errors import UnknownKluError
 
 
 class SSEClient:
     @staticmethod
     async def get_streaming_data(streaming_url: str) -> AsyncIterator[str]:
@@ -19,18 +18,16 @@
         Get a streams of messages from an SQS queue for a specific channel.
 
         Args:
             streaming_url (str): The url you received from run_action_prompt with streaming param set to True.
 
         Returns:
             An asynchronous generator, which can be used to read chunks of data from the streaming url. Usage example:
-
-            async for chunk in get_streaming_data():
-                # Process the chunk of data here
-                print(chunk)
+                async for chunk in get_streaming_data():
+                    # Process the chunk of data here
         """
         try:
             async with sse_client.EventSource(streaming_url) as event_source:
                 async for event in event_source:
                     message = event.data
                     if message == END_STREAM_CONTENT or message == NO_MESSAGES_CONTENT:
                         await event_source.close()
```

### Comparing `klu-0.1.5/klu/application/client.py` & `klu-0.1.6/klu/application/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,61 @@
+# mypy: disable-error-code="override"
 from typing import List, Optional
 
 import aiohttp
 from aiohttp import ClientResponseError
-from aiohttp.web_exceptions import HTTPNotFound
 
 from klu.action.models import Action
 from klu.application.constants import (
+    APPLICATION_ACTIONS_ENDPOINT,
+    APPLICATION_DATA_ENDPOINT,
     APPLICATION_ENDPOINT,
     DEFAULT_APPS_PAGE_SIZE,
-    APPLICATION_DATA_ENDPOINT,
-    APPLICATION_ACTIONS_ENDPOINT,
 )
-from klu.data.models import Data
-from klu.utils.paginator import Paginator
-from klu.common.client import KluClientBase
-from klu.application.models import Application
-from klu.utils.dict_helpers import dict_no_empty
 from klu.application.errors import ApplicationNotFoundError
+from klu.application.models import Application
+from klu.common.client import KluClientBase
 from klu.common.errors import InvalidUpdateParamsError, UnknownKluAPIError
+from klu.data.models import Data
+from klu.utils.dict_helpers import dict_no_empty
+from klu.utils.paginator import Paginator
 
 
 class ApplicationsClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, APPLICATION_ENDPOINT, Application)
         self._paginator = Paginator(APPLICATION_ENDPOINT)
 
     async def create(self, name: str, app_type: str, description: str) -> Application:
         """
         Creates new application instance
 
         Args:
             name: str. Name of a new application
-            app_type: str. Type of a new application
+            app_type: str. Type of new application
             description: str. Description of a new application
 
-        Returns: Newly created Application object
+        Returns:
+            Newly created Application object
         """
         return await super().create(
             name=name,
             app_type=app_type,
             description=description,
         )
 
     async def get(self, guid: str) -> Application:
         """
         Retrieves app  information based on the app id.
 
         Args:
             guid (str): GUID of an application to fetch. The one that was used during the app creation
 
-        Returns: Application object
+        Returns:
+            Application object
         """
         return await super().get(guid)
 
     async def update(
         self,
         guid: str,
         name: Optional[str] = None,
@@ -65,90 +67,95 @@
 
         Args:
             guid (str): GUID of an application to fetch. The one that was used during the app creation
             name: Optional[str]. New application name
             app_type: Optional[str]. New application type
             description: Optional[str]. New application description
 
-        Returns: Updated application instance
+        Returns:
+            Updated application instance
         """
 
         if not name and not app_type and not description:
             raise InvalidUpdateParamsError()
 
         return await super().update(
             **{
-                "id": guid,
+                "guid": guid,
                 **dict_no_empty(
                     {"name": name, "app_type": app_type, "description": description}
                 ),
             }
         )
 
     async def delete(self, guid: str) -> Application:
         """
         Delete existing application information defined by the app id.
 
         Args:
             guid (str): The id of an application to delete.
 
-        Returns: Deleted application object
+        Returns:
+            Deleted application object
         """
         return await super().delete(guid)
 
     async def get_app_data(self, app_guid: str) -> List[Data]:
         """
         Retrieves app data information based on the app GUID.
 
         Args:
             app_guid (str): GUID of an application to fetch data for. The one that was returned during the app creation
 
-        Returns: An array of data objects, found by provided app id.
+        Returns:
+            An array of data objects, found by provided app id.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.get(
                     APPLICATION_DATA_ENDPOINT.format(id=app_guid)
                 )
                 return [Data._from_engine_format(data) for data in response]
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise ApplicationNotFoundError(app_guid)
 
                 raise UnknownKluAPIError(e.status, e.message)
 
     async def get_app_actions(self, app_guid: str) -> List[Action]:
         """
         Retrieves app actions information based on the app GUID.
 
         Args:
             app_guid (str): GUID of an application to fetch actions for. The one that was used during the app creation
 
-        Returns: An array of actions, found by provided app id.
+        Returns:
+            An array of actions, found by provided app id.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.get(
                     APPLICATION_ACTIONS_ENDPOINT.format(id=app_guid)
                 )
                 return [Action._from_engine_format(action) for action in response]
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise ApplicationNotFoundError(app_guid)
 
                 raise UnknownKluAPIError(e.status, e.message)
 
     async def list(self) -> List[Application]:
         """
         Retrieves all apps attached to a workspace.
         Does not rely on internal paginator state, so `reset_pagination` method call can be skipped
 
-        Returns: An array of all apps
+        Returns:
+            An array of all apps
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_all(client)
 
             return [
                 Application._from_engine_format(application) for application in response
@@ -162,39 +169,41 @@
         Can be used to fetch a specific page of applications provided a certain per_page config.
         Does not rely on internal paginator state, so `reset_pagination` method call can be skipped
 
         Args:
             page_number (int): Number of the page to fetch
             limit (int): Number of instances to fetch per page. Defaults to 50
 
-        Returns: An array of apps fetched for a queried page. Empty if queried page does not exist
+        Returns:
+            An array of apps fetched for a queried page. Empty if queried page does not exist
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_single_page(
                 client, page_number, limit=limit
             )
 
             return [
                 Application._from_engine_format(application) for application in response
             ]
 
     async def fetch_next_page(
-        self, limit: int = DEFAULT_APPS_PAGE_SIZE, offset: int = None
+        self, limit: int = DEFAULT_APPS_PAGE_SIZE, offset: Optional[int] = None
     ) -> List[Application]:
         """
         Retrieves the next page of applications. Can be used to fetch a flexible number of pages starting.
         The place to start from can be controlled by the offset parameter.
         After using this method, we suggest to call `reset_pagination` method to reset the page cursor.
 
         Args:
             limit (int): Number of instances to fetch per page. Defaults to 50
             offset (int): The number of apps to skip. Can be used to query the pages of applications skipping certain number of instances.
 
-        Returns: An array of apps fetched for a queried page. Empty if the end was reached at the previous step.
+        Returns:
+            An array of apps fetched for a queried page. Empty if the end was reached at the previous step.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_next_page(
                 client, limit=limit, offset=offset
             )
```

### Comparing `klu-0.1.5/klu/application/models.py` & `klu-0.1.6/klu/application/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,23 @@
-from typing import Optional
+"""
+This module provides data models for the Application.
+"""
+from dataclasses import asdict, dataclass
 from datetime import datetime
-from dataclasses import dataclass, asdict
+from typing import Optional
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
 class Application(BaseEngineModel):
+    """
+    This class represents the Application data model returned from the Klu engine
+    """
+
     id: int
     guid: str
     name: str
     app_type: str
     enabled: bool
 
     workspace_id: int
```

### Comparing `klu-0.1.5/klu/client/klu.py` & `klu-0.1.6/klu/client/klu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from klu.data.client import DataClient
+from klu.action.client import ActionsClient
 from klu.api.sse_client import SSEClient
+from klu.application.client import ApplicationsClient
+from klu.data.client import DataClient
+from klu.data_index.client import DataIndexClient
 from klu.model.client import ModelsClient
-from klu.action.client import ActionsClient
 from klu.session.client import SessionClient
 from klu.workspace.client import WorkspaceClient
-from klu.data_index.client import DataIndexClient
-from klu.application.client import ApplicationsClient
 
 
 class KluClient:
     def __init__(self, api_key: str):
         self.sse_client = SSEClient()
 
         self.data = DataClient(api_key)
```

### Comparing `klu-0.1.5/klu/common/client.py` & `klu-0.1.6/klu/common/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from abc import abstractmethod
 from typing import Type, TypeVar
 
 import aiohttp
-
 from aiohttp import ClientResponseError
-from aiohttp.web_exceptions import HTTPNotFound
 
+from klu.api.client import APIClient
 from klu.common.errors import (
     IdNotProvidedError,
     InstanceNotFoundError,
     InstanceRelationshipNotFoundError,
 )
-from klu.api.client import APIClient
-from klu.common.models import BaseEngineModel, KluId
+from klu.common.models import BaseEngineModel
 
 T = TypeVar("T", bound=BaseEngineModel)
 
 
 class KluClientBase:
-    def __init__(self, api_key: str, base_path: str, model: Type[BaseEngineModel]):
+    def __init__(self, api_key: str, base_path: str, model: Type[T]):
         self._model = model
         self._api_key = api_key
         self._base_path = base_path
 
     def _get_api_client(self, session):
         return APIClient(session, self._api_key)
 
@@ -31,58 +29,58 @@
         # Some endpoints use a different url for creation
         # TODO ideally, this should be the same. Create a task on the engine side.
         url = kwargs.pop("url", None)
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.post(url or self._base_path, kwargs)
-                return self._model._from_engine_format(response)
-            except (HTTPNotFound, ClientResponseError) as e:
+                return self._model._from_engine_format(response)  # type: ignore
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise InstanceRelationshipNotFoundError(
                         self._model.__name__, e.message
                     )
 
                 raise e
 
     @abstractmethod
-    async def get(self, id: KluId) -> T:
+    async def get(self, guid: str) -> T:
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
-                response = await client.get(f"{self._base_path}{id}")
-                return self._model._from_engine_format(response)
-            except (HTTPNotFound, ClientResponseError) as e:
+                response = await client.get(f"{self._base_path}{guid}")
+                return self._model._from_engine_format(response)  # type: ignore
+            except ClientResponseError as e:
                 if e.status == 404:
-                    raise InstanceNotFoundError(self._model.__name__, id)
+                    raise InstanceNotFoundError(self._model.__name__, guid)
 
                 raise e
 
     @abstractmethod
     async def update(self, **kwargs) -> T:
-        id = kwargs.pop("id", None)
+        id = kwargs.pop("guid", None)
         if not id:
             raise IdNotProvidedError()
 
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.put(f"{self._base_path}{id}", kwargs)
-                return self._model._from_engine_format(response)
-            except (HTTPNotFound, ClientResponseError) as e:
+                return self._model._from_engine_format(response)  # type: ignore
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise InstanceNotFoundError(self._model.__name__, id)
 
                 raise e
 
     @abstractmethod
-    async def delete(self, id: KluId) -> T:
+    async def delete(self, guid: str) -> T:
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
-                response = await client.delete(f"{self._base_path}{id}")
-                return self._model._from_engine_format(response)
-            except (HTTPNotFound, ClientResponseError) as e:
+                response = await client.delete(f"{self._base_path}{guid}")
+                return self._model._from_engine_format(response)  # type: ignore
+            except ClientResponseError as e:
                 if e.status == 404:
-                    raise InstanceNotFoundError(self._model.__name__, id)
+                    raise InstanceNotFoundError(self._model.__name__, guid)
 
                 raise e
```

### Comparing `klu-0.1.5/klu/common/errors.py` & `klu-0.1.6/klu/common/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from klu.common.models import KluId
-
-
 class BaseKluError(Exception):
     __suppress_context__ = True
 
 
 class IdNotProvidedError(BaseKluError):
     def __init__(self):
         self.message = f"Received invalid parameters. id cannot be None. Please, provide a valid id."
@@ -14,15 +11,15 @@
 class InstanceRelationshipNotFoundError(BaseKluError):
     def __init__(self, instance_name: str, message: str):
         self.message = f"One of the relationships for new {instance_name} was not found. Message from server: {message}"
         super().__init__(self.message)
 
 
 class InstanceNotFoundError(BaseKluError):
-    def __init__(self, instance_name: str, instance_id: KluId):
+    def __init__(self, instance_name: str, instance_id: str):
         self.message = f"{instance_name} with id {instance_id} was not found."
         super().__init__(self.message)
 
     def __str__(self):
         return f'{self.__class__.__name__}: {self.message}'
 
 
@@ -30,15 +27,17 @@
     def __init__(self):
         self.message = "Unknown error in Klu SDK. Please contact the support team."
         super().__init__(self.message)
 
 
 class UnknownKluAPIError(BaseKluError):
     def __init__(self, status: int, message: str):
-        self.message = f"Unknown error in Klu API.\nstatus_code: {status},\nmessage: {message}"
+        self.message = (
+            f"Unknown error in Klu API.\nstatus_code: {status},\nmessage: {message}"
+        )
         super().__init__(self.message)
 
 
 class UnauthorizedError(BaseKluError):
     def __init__(self):
         self.message = (
             f"Wrong credentials used to access the API. "
@@ -63,15 +62,17 @@
             f"Please, contact Klu support team so we could fix this.\nstatus_code: {status},\nmessage: {message}"
         )
         super().__init__(self.message)
 
 
 class BadRequestAPIError(BaseKluError):
     def __init__(self, status: int, message: str):
-        self.message = f"BadRequest error in Klu API.\nstatus_code: {status},\nmessage: {message}"
+        self.message = (
+            f"BadRequest error in Klu API.\nstatus_code: {status},\nmessage: {message}"
+        )
         super().__init__(self.message)
 
 
 class InvalidUpdateParamsError(BaseKluError):
     def __init__(self):
         self.message = "No update params have been provided. At least one of parameters should be sent."
         super().__init__(self.message)
```

### Comparing `klu-0.1.5/klu/common/models.py` & `klu-0.1.6/klu/common/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from enum import Enum
 from abc import ABCMeta, abstractmethod
-from typing import Optional, Union, NewType
-
-KluId = NewType("KluId", Union[int, str])
+from enum import Enum
+from typing import Optional
 
 
 class BasicEnum(Enum):
     """
     Basic class for enums across the projects. Adds basic functions to list names and values.
     Overrides comparison function to allow comparing against string values.
     """
```

### Comparing `klu-0.1.5/klu/data/client.py` & `klu-0.1.6/klu/data/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# mypy: disable-error-code="override"
 from typing import Optional
 
-from klu.data.models import Data
 from klu.common.client import KluClientBase
 from klu.data.constants import DATA_ENDPOINT
+from klu.data.models import Data
 
 
 class DataClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, DATA_ENDPOINT, Data)
 
     async def create(
@@ -31,46 +32,49 @@
             action (str): Data action value
             rating (int): Data rating
             action_guid (str): Guid of an action data belongs to
             session_guid (str): Guid of a session data belongs to
             meta_data (dict): Data meta_data
             correction (str): Data correction
 
-        Returns: Created Data object
+        Returns:
+            Created Data object
         """
         return await super().create(
             issue=issue,
             input=input,
             output=output,
             action=action,
             rating=rating,
             meta_data=meta_data,
             correction=correction,
             action_guid=action_guid,
             session_guid=session_guid,
         )
 
-    async def get(self, id: str) -> Data:
+    async def get(self, guid: str) -> Data:
         """
         Retrieves data information based on the data ID.
 
         Args:
-            id (str): ID of a datum object to fetch.
+            guid (str): ID of a datum object to fetch.
 
-        Returns: An object
+        Returns:
+            An object
         """
-        return await super().get(id)
+        return await super().get(guid)
 
-    async def update(self, id: str, output: str) -> Data:
+    async def update(self, guid: str, output: str) -> Data:
         """
         Updated data information based on the data ID and provided payload. Currently, only supports `output` update.
 
         Args:
-            id (str): ID of a datum object to update.
+            guid (str): ID of a datum object to update.
             output (str): New 'output' data field value.
 
-        Returns: Newly updated Data object
+        Returns:
+            Newly updated Data object
         """
-        return await super().update(id=id, output=output)
+        return await super().update(guid=guid, output=output)
 
-    async def delete(self, id: str) -> Data:
-        return await super().delete(id)
+    async def delete(self, guid: str) -> Data:
+        return await super().delete(guid)
```

### Comparing `klu-0.1.5/klu/data/models.py` & `klu-0.1.6/klu/data/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,44 @@
+"""
+This module provides data models for the Data.
+"""
+
 from abc import ABC
-from typing import Optional
+from dataclasses import asdict, dataclass
 from datetime import datetime
-from dataclasses import dataclass, asdict
+from typing import Optional
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
 class DataWithId(BaseEngineModel, ABC):
+    """
+    This class represents the base data with Id after it has been persisted into the Klu Database
+    """
+
     id: int
     guid: str
 
 
 @dataclass
 class DataWithFeedbackUrl(BaseEngineModel, ABC):
+    """
+    This class represents the data specific to the model returned from the Action prompting
+    """
+
     feedback_url: int
 
 
 @dataclass
 class DataBaseClass(BaseEngineModel):
+    """
+    This class represents the generic data information that is stored in the Klu database
+    """
+
     issue: Optional[int] = None
     input: Optional[str] = None
     action: Optional[int] = None
     output: Optional[str] = None
     rating: Optional[int] = None
     metadata: Optional[dict] = None
     correction: Optional[str] = None
@@ -36,56 +52,70 @@
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
+        base_dict = asdict(
+            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
+        )
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
 
         return base_dict
 
 
 # We need this way of inheritance to append optional field after the required ones.
 @dataclass
 class Data(DataBaseClass, DataWithId):
+    """
+    This class represents the Data model returned from the Klu engine
+    """
+
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Data":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
+        base_dict = asdict(
+            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
+        )
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
 
         return base_dict
 
 
 @dataclass
 class ActionData(DataBaseClass, DataWithFeedbackUrl):
+    """
+    This class represents the Data model returned from the Klu engine in response to Action data request
+    """
+
     @classmethod
     def _from_engine_format(cls, data: dict) -> "ActionData":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
+        base_dict = asdict(
+            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
+        )
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
 
         return base_dict
```

### Comparing `klu-0.1.5/klu/data_index/client.py` & `klu-0.1.6/klu/data_index/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
+# mypy: disable-error-code="override"
 from typing import Optional
 
 import aiohttp
 from aiohttp import ClientResponseError
-from aiohttp.web_exceptions import HTTPNotFound
 
-from klu.data_index.models import (
-    FileData,
-    DataIndex,
-    PreSignUrlPostData,
-    DataIndexStatusEnum,
+from klu.common.client import KluClientBase
+from klu.common.errors import (
+    InvalidUpdateParamsError,
+    UnknownKluAPIError,
+    UnknownKluError,
 )
 from klu.data_index.constants import (
     DATA_INDEX_ENDPOINT,
     DATA_INDEX_STATUS_ENDPOINT,
     PROCESS_DATA_INDEX_ENDPOINT,
     UPLOAD_PRE_SIGNED_URL_ENDPOINT,
 )
-from klu.common.client import KluClientBase
-from klu.utils.dict_helpers import dict_no_empty
 from klu.data_index.errors import DataIndexNotFoundError
+from klu.data_index.models import (
+    DataIndex,
+    DataIndexStatusEnum,
+    FileData,
+    PreSignUrlPostData,
+)
+from klu.utils.dict_helpers import dict_no_empty
 from klu.utils.file_upload import upload_to_pre_signed_url
 from klu.workspace.errors import WorkspaceOrUserNotFoundError
-from klu.common.errors import (
-    UnknownKluAPIError,
-    UnknownKluError,
-    InvalidUpdateParamsError,
-)
 
 
 class DataIndexClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, DATA_INDEX_ENDPOINT, DataIndex)
 
     async def create(
@@ -46,117 +46,130 @@
             name (str): The name of the index
             description (str): The description of the index
             file_data (Optional[FileData]): Metadata of the file to be uploaded.
                 Can be omitted if only the data_index skeleton has to be created
             splitter (Optional[str]): The column splitter - filter by the user when they are dealing with a multi
                 tenanted environment.
 
-        Returns: dict with a message about successful index creation and id of a newly created index file.
+        Returns:
+            dict with a message about successful index creation and id of a newly created index file.
         Use this id to check the status of dataIndex processing.
         """
         file_url = await self.upload_index_file(file_data) if file_data else None
         data_index = {
             "name": name,
             "splitter": splitter,
             "description": description,
         }
         if file_url:
             data_index["file_url"] = file_url
 
         return await super().create(**data_index)
 
-    async def get(self, guid: int) -> DataIndex:
+    # type: ignore
+    async def get(self, guid: str) -> DataIndex:
         """
         Retrieves data_index information based on the id.
 
         Args:
             guid (str): id of a data_index object to fetch.
 
-        Returns: DataIndex object found by provided id
+        Returns:
+            DataIndex object found by provided id
         """
         return await super().get(guid)
 
-    async def update(self, guid: str, name: Optional[str] = None, description: Optional[str] = None) -> DataIndex:
+    # type: ignore
+    async def update(
+        self, guid: str, name: Optional[str] = None, description: Optional[str] = None
+    ) -> DataIndex:
         """
         Update data_index data. At least one of the params has to be provided
 
         Args:
             guid (str): ID of a data_index to update.
             name: Optional[str]. New data_index name
             description: Optional[str]. New data_index description
 
-        Returns: Updated application instance
+        Returns:
+            Updated application instance
         """
 
         if not name and not description:
             raise InvalidUpdateParamsError()
 
         return await super().update(
             **{
-                "id": guid,
+                "guid": guid,
                 **dict_no_empty({"name": name, "description": description}),
             }
         )
 
-    async def delete(self, guid: int) -> DataIndex:
+    # type: ignore
+    async def delete(self, guid: str) -> DataIndex:
         """
         Delete existing data_index information defined by the id.
 
         Args:
             guid (str): The id of a data_index to delete.
 
-        Returns: Deleted DataIndex object
+        Returns:
+            Deleted DataIndex object
         """
         return await super().delete(guid)
 
     async def get_status(self, guid: int) -> DataIndexStatusEnum:
         """
         Retrieves the status of an index creation task based on the provided index ID.
 
         Args:
             guid (int): The ID of the data index.
 
-        Returns: string representing te data_index status
+        Returns:
+            string representing te data_index status
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.post(DATA_INDEX_STATUS_ENDPOINT.format(id=guid))
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise DataIndexNotFoundError(guid)
 
                 raise UnknownKluAPIError(e.status, e.message)
 
-            return DataIndexStatusEnum.get(response.get("status"))
+            return DataIndexStatusEnum.get(response.get("status"))  # type: ignore
 
-    async def process_data_index(self, data_index_guid: str, file_name: str, splitter: Optional[str] = None) -> dict:
+    async def process_data_index(
+        self, data_index_guid: str, file_name: str, splitter: Optional[str] = None
+    ) -> dict:
         """
         Processes existing index identified by provided data_index id using provider column splitter
 
         Args:
             data_index_guid (str): Guid of data index to process
             file_name (str): Name of the file uploaded before that should be used for DataIndex processing.
-            splitter (Optional[str]): The column splitter - filter by the user when they are dealing with a multi
-            tenanted environment.
+                splitter (Optional[str]): The column splitter - filter by the user when they are dealing with a multi
+                tenanted environment.
 
-        Returns: dict with a message about successful index creation
+        Returns:
+            dict with a message about successful index creation
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.post(
                     PROCESS_DATA_INDEX_ENDPOINT,
                     {
                         "splitter": splitter,
                         "filename": file_name,
                         "guid": data_index_guid,
                     },
                 )
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 # TODO differentiate between missing data_index and missing user 404. Change the engine accordingly
                 if e.status == 404:
                     raise WorkspaceOrUserNotFoundError()
 
                 raise UnknownKluAPIError(e.status, e.message)
             except Exception:
                 raise UnknownKluError()
@@ -166,33 +179,41 @@
     async def upload_index_file(self, file_data: FileData) -> str:
         """
         Upload system file to Klu storage for later usage in data_index creation. Maximum supported file size is 50 MB.
 
         Args:
             file_data (FileData): Metadata of the file to be uploaded. For more details, see the FileData class docs.
 
-        Returns: URL to the uploaded file. This URL should be used during the data_index creation flow.
+        Returns:
+            URL to the uploaded file. This URL should be used during the data_index creation flow.
         """
         async with aiohttp.ClientSession() as session:
-            pre_signed_url_data = await self.get_index_upload_pre_signed_url(file_data.file_name)
-            await upload_to_pre_signed_url(session, pre_signed_url_data, file_data.file_path)
+            pre_signed_url_data = await self.get_index_upload_pre_signed_url(
+                file_data.file_name
+            )
+            await upload_to_pre_signed_url(
+                session, pre_signed_url_data, file_data.file_path
+            )
 
             return pre_signed_url_data.object_url
 
-    async def get_index_upload_pre_signed_url(self, file_name: str) -> PreSignUrlPostData:
+    async def get_index_upload_pre_signed_url(
+        self, file_name: str
+    ) -> PreSignUrlPostData:
         """
         Get pre-signed url to upload files to use for data_indexes creation. Maximum supported file size is 50 MB.
         This method should only be used if you don't want to use `upload_model_file` function to upload the file without
         the need to get into pre_signed_url upload flow.
 
         Args:
             file_name (str): The name of the file to be uploaded. Has to be unique among the files you uploaded before.
-            Otherwise, the new file will override the previously uploaded one by the same file_name
+                Otherwise, the new file will override the previously uploaded one by the same file_name
 
-        Returns: pre-signed url data including url, which is the pre-signed url that can be used to upload the file.
+        Returns:
+            pre-signed url data including url, which is the pre-signed url that can be used to upload the file.
             Also includes 'fields' property that contains dict with data that
             has to be passed alongside the file during the upload
             And object_url property that contains the url that can be used to access the file location after the upload.
             This same object_url can be used during the data_index creation.
             For a usage example check out the `upload_index_file` function
         """
         async with aiohttp.ClientSession() as session:
@@ -200,15 +221,15 @@
             try:
                 response = await client.post(
                     UPLOAD_PRE_SIGNED_URL_ENDPOINT,
                     {
                         "file_name": file_name,
                     },
                 )
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 # TODO differentiate between missing data_index and missing user 404. Change the engine accordingly
                 if e.status == 404:
                     raise WorkspaceOrUserNotFoundError()
 
                 raise UnknownKluAPIError(e.status, e.message)
 
             return PreSignUrlPostData(**response)
```

### Comparing `klu-0.1.5/klu/data_index/models.py` & `klu-0.1.6/klu/data_index/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from typing import Optional
+"""
+This module provides data models for the DataIndex.
+"""
+from dataclasses import asdict, dataclass
 from datetime import datetime
-from dataclasses import dataclass, asdict
+from typing import Optional
 
-from klu.common.models import BasicStringEnum, BaseEngineModel, BaseDataClass
+from klu.common.models import BaseDataClass, BaseEngineModel, BasicStringEnum
 
 
 class DataIndexStatusEnum(BasicStringEnum):
     """The enum used to represent DataIndex processing task status. Based on celery statuses."""
 
     # The task is waiting for execution.
     PENDING = "PENDING"
@@ -19,14 +22,18 @@
     FAILURE = "FAILURE"
     # The task executed successfully.
     SUCCESS = "SUCCESS"
 
 
 @dataclass
 class DataIndex(BaseEngineModel):
+    """
+    This class represents the DataIndex model returned from the Klu engine
+    """
+
     guid: str
     name: str
     processed: bool
 
     type_id: int
     task_id: str
     file_url: str
```

### Comparing `klu-0.1.5/klu/model/client.py` & `klu-0.1.6/klu/model/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,106 @@
+# mypy: disable-error-code="override"
 from typing import Optional
 
 import aiohttp
-
 from aiohttp import ClientResponseError
-from aiohttp.web_exceptions import HTTPNotFound
 
-from klu.model.models import Model
-from klu.common.models import KluId
 from klu.common.client import KluClientBase
+from klu.common.errors import InvalidUpdateParamsError, UnknownKluAPIError
 from klu.model.constants import MODEL_ENDPOINT
-from klu.utils.dict_helpers import dict_no_empty
 from klu.model.errors import UnknownModelProviderError
-from klu.common.errors import InvalidUpdateParamsError, UnknownKluAPIError
+from klu.model.models import Model
+from klu.utils.dict_helpers import dict_no_empty
 
 
 class ModelsClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, MODEL_ENDPOINT, Model)
 
     async def create(self, llm: str, workspace_model_provider_id: int) -> Model:
         """
-        Creates a model based on the data provided.
+                Creates a model based on the data provided.
 
-        Args:
-            llm (str): Model llm. Required
-            workspace_model_provider_id (str): Unique identifier of model provider.
-                Can be retrieved from a model providers listing endpoint.
+                Args:
+                    llm (str): Model llm. Required
+                    workspace_model_provider_id (str): Unique identifier of model provider.
+                        Can be retrieved from a model providers listing endpoint.
 
-        Returns: A newly created Model object.
+                Returns:
+        A newly created Model object.
         """
         return await super().create(
             llm=llm, workspaceModelProviderId=workspace_model_provider_id
         )
 
     async def get(self, guid: str) -> Model:
         """
         Retrieves model  information based on the id.
 
         Args:
             guid (str): GUID of a model to fetch. The one that was used during the model creation
 
-        Returns: Model object
+        Returns:
+            Model object
         """
         return await super().get(guid)
 
     async def update(
-        self, id: str, llm: Optional[str] = None, key: Optional[str] = None
+        self, guid: str, llm: Optional[str] = None, key: Optional[str] = None
     ) -> Model:
         """
         Update model data. At least one of the params has to be provided
 
         Args:
-            id (str): ID of a data_index to update.
+            guid (str): Guid of a data_index to update.
             llm: Optional[str]. New data_index name
             key: Optional[str]. New data_index description
 
-        Returns: Updated application instance
+        Returns:
+            Updated application instance
         """
         if not llm and not key:
             raise InvalidUpdateParamsError()
 
         return await super().update(
-            **{"id": id, **dict_no_empty({"llm": llm, "key": key})}
+            **{"guid": guid, **dict_no_empty({"llm": llm, "key": key})}
         )
 
-    async def delete(self, id: KluId) -> Model:
+    async def delete(self, guid: str) -> Model:
         """
         Delete model based on the id.
 
         Args:
-            id (str): ID of a model to delete.
+            guid (str): ID of a model to delete.
 
-        Returns: Deleted model object
+        Returns:
+            Deleted model object
         """
-        return await super().delete(id)
+        return await super().delete(guid)
 
     async def validate_provider_api_key(self, api_key: str, provider: str) -> bool:
         """
         Validates API keys for provided api_key and provider values.
 
         Args:
             api_key (str): Model api_key
             provider (str): Model provider. Required. Should be one of the following: [OpenAI, HuggingFace, NLPCloud, GooseAI, AI21 & Anthropic]
 
-        Returns: A JSON response with a message about successful creation if model was created.
+        Returns:
+            A JSON response with a message about successful creation if model was created.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.post(
                     MODEL_ENDPOINT,
                     {
                         "api_key": api_key,
                         "provider": provider,
                     },
                 )
                 return bool(response.get("validated"))
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise UnknownModelProviderError(provider)
 
                 raise UnknownKluAPIError(e.status, e.message)
```

### Comparing `klu-0.1.5/klu/model/models.py` & `klu-0.1.6/klu/model/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,24 @@
-from typing import Optional
+"""
+This module provides data models for the Model.
+"""
+
+from dataclasses import asdict, dataclass
 from datetime import datetime
-from dataclasses import dataclass, asdict
+from typing import Optional
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
 class Model(BaseEngineModel):
+    """
+    This class represents the Model data returned from the Klu engine
+    """
+
     id: int
     llm: str
     guid: str
     model_name: str
     created_by_id: str
     workspace_model_provider_id: int
     updated_at: Optional[datetime] = None
@@ -19,21 +27,25 @@
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Model":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
                 "created_by_id": data.pop("createdById", None),
-                "workspace_model_provider_id": data.pop("workspaceModelProviderId", None),
+                "workspace_model_provider_id": data.pop(
+                    "workspaceModelProviderId", None
+                ),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
+        base_dict = asdict(
+            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
+        )
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
         base_dict.pop("created_by_id", None)
         base_dict.pop("workspace_model_provider_id", None)
 
         return base_dict
```

### Comparing `klu-0.1.5/klu/session/client.py` & `klu-0.1.6/klu/session/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,51 @@
+# mypy: disable-error-code="override"
 from typing import NoReturn
 
-from klu.session.models import Session
 from klu.common.client import KluClientBase
 from klu.common.errors import NotSupportedError
 from klu.session.constants import SESSION_ENDPOINT
+from klu.session.models import Session
 
 
 class SessionClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, SESSION_ENDPOINT, Session)
 
-    async def create(self, action_guid: int) -> Session:
+    async def create(self, action_guid: str) -> Session:
         """
         Creates a session based on the data provided.
 
         Args:
             action_guid (str): Guid of the action object this session is attached to.
 
-        Returns: A newly created Session object.
+        Returns:
+            A newly created Session object.
         """
         return await super().create(action_guid=action_guid)
 
     async def get(self, guid: str) -> Session:
         """
         Retrieves session information based on the unique Session guid, created during the Session creation.
 
         Args:
             guid (str): GUID of a session to fetch. The one that was used during the session creation
 
-        Returns: Session object
+        Returns:
+            Session object
         """
         return await super().get(guid)
 
     async def update(self) -> NoReturn:
         raise NotSupportedError()
 
     async def delete(self, guid: str) -> Session:
         """
         Delete session based on the id.
 
         Args:
             guid (str): Unique Guid of a session to delete.
 
-        Returns: Deleted session object
+        Returns:
+            Deleted session object
         """
-        return await super().delete(id)
+        return await super().delete(guid)
```

### Comparing `klu-0.1.5/klu/session/models.py` & `klu-0.1.6/klu/session/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,24 @@
-from typing import Optional
+"""
+This module provides data models for the Session.
+"""
+
+from dataclasses import asdict, dataclass
 from datetime import datetime
-from dataclasses import dataclass, asdict
+from typing import Optional
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
 class Session(BaseEngineModel):
+    """
+    This class represents the Session data returned from the Klu engine
+    """
+
     id: int
     guid: str
     action_id: int
     created_by_id: str
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
 
@@ -23,15 +31,17 @@
                 "created_at": data.pop("createdAt", None),
                 "created_by_id": data.pop("createdById", None),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
+        base_dict = asdict(
+            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
+        )
 
         base_dict.pop("action_id", None)
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
         base_dict.pop("created_by_id", None)
 
         return base_dict
```

### Comparing `klu-0.1.5/klu/utils/file_upload.py` & `klu-0.1.6/klu/utils/file_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-import aiohttp
 import aiofiles
-
+import aiohttp
 from aiohttp import ClientResponse
 
 from klu.data_index.models import PreSignUrlPostData
 
 
 async def upload_to_pre_signed_url(
-    session: aiohttp.ClientSession, pre_signed_url_data: PreSignUrlPostData, file_path: str
+    session: aiohttp.ClientSession,
+    pre_signed_url_data: PreSignUrlPostData,
+    file_path: str,
 ) -> ClientResponse:
-    pre_signed_url, pre_signed_fields = pre_signed_url_data.url, pre_signed_url_data.fields
+    pre_signed_url, pre_signed_fields = (
+        pre_signed_url_data.url,
+        pre_signed_url_data.fields,
+    )
 
     data = aiohttp.FormData()
     for key, value in pre_signed_fields.items():
         data.add_field(key, value)
 
     async with aiofiles.open(file_path, mode="rb") as file:
         data.add_field("file", await file.read())
```

### Comparing `klu-0.1.5/klu/utils/paginator.py` & `klu-0.1.6/klu/utils/paginator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from klu.api.client import APIClient
+from typing import Optional
 
+from klu.api.client import APIClient
 
 DEFAULT_PAGE_SIZE = 100
 
 
 class Paginator:
     def __init__(self, endpoint, limit=DEFAULT_PAGE_SIZE):
         self.endpoint = endpoint
@@ -12,18 +13,18 @@
         self.current_page = 0
         self.total_count = None
         self.has_next_page = True
 
     async def _get_paginated_results(
         self,
         api_client: APIClient,
-        skip: int = None,
-        limit: int = None,
-        offset: int = None,
-        **params
+        skip: Optional[int] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        **params,
     ):
         limit = limit if limit is not None else self.limit
         skip = skip if skip is not None else self.current_page * limit
 
         if offset is not None:
             skip = skip + offset
 
@@ -34,43 +35,43 @@
         results = response.get("data", [])
 
         self.total_count = response.get("total_count", 0)
         self.has_next_page = response.get("has_next_page", False)
 
         return results
 
-    async def fetch_all(self, api_client: APIClient, limit: int = None):
+    async def fetch_all(self, api_client: APIClient, limit: Optional[int] = None):
         results = []
         self._reset_paginator()
 
         while self.has_next_page:
             results.extend(await self._get_paginated_results(api_client, limit=limit))
             self.current_page += 1
 
         self._reset_paginator()
         return results
 
     async def fetch_single_page(
-        self, api_client: APIClient, page_number: int, limit: int = None
+        self, api_client: APIClient, page_number: int, limit: Optional[int] = None
     ):
         self._reset_paginator()
 
         limit = self.limit if limit is None else limit
         skip = (page_number - 1) * limit
 
         results = await self._get_paginated_results(api_client, skip=skip, limit=limit)
 
         self._reset_paginator()
         return results
 
     async def fetch_next_page(
         self,
         api_client: APIClient,
-        limit: int = None,
-        offset: int = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
     ):
         if not self.has_next_page:
             return []
 
         curr_page_results = await self._get_paginated_results(
             api_client, limit=limit, offset=offset
         )
```

### Comparing `klu-0.1.5/klu/workspace/client.py` & `klu-0.1.6/klu/workspace/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import List
+# mypy: disable-error-code="override"
+from typing import List, Optional
 
 import aiohttp
 from aiohttp import ClientResponseError
-from aiohttp.web_exceptions import HTTPNotFound
 
+from klu.application.models import Application
+from klu.common.client import KluClientBase
 from klu.common.errors import UnknownKluAPIError
+from klu.data_index.models import DataIndex
 from klu.model.models import Model
 from klu.utils.paginator import Paginator
 from klu.workspace.constants import (
-    WORKSPACE_ENDPOINT,
+    DEFAULT_WORKSPACE_PAGE_SIZE,
     WORKSPACE_APPS_ENDPOINT,
-    WORKSPACE_MODELS_ENDPOINT,
+    WORKSPACE_ENDPOINT,
     WORKSPACE_INDICES_ENDPOINT,
-    DEFAULT_WORKSPACE_PAGE_SIZE,
+    WORKSPACE_MODELS_ENDPOINT,
 )
-from klu.workspace.models import Workspace
-from klu.common.client import KluClientBase
-from klu.data_index.models import DataIndex
-from klu.application.models import Application
 from klu.workspace.errors import WorkspaceOrUserNotFoundError
+from klu.workspace.models import Workspace
 
 
 class WorkspaceClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, WORKSPACE_ENDPOINT, Workspace)
         self._paginator = Paginator(WORKSPACE_ENDPOINT)
 
@@ -30,130 +30,138 @@
         """
         Creates a Workspace based on the data provided.
 
         Args:
             name (str): Model key. Required
             slug (str): Workspace slug. The unique name you would prefer to use to access the model.
 
-        Returns: A newly created Workspace object.
+        Returns:
+            A newly created Workspace object.
         """
         return await super().create(name=name, slug=slug)
 
     async def get(self, guid: str) -> Workspace:
         """
         Retrieves a single workspace object by provided workspace id
 
         Args:
             guid (str): The ID of a workspace to fetch. project_guid you sent during the workspace creation
 
-        Returns: A workspace object
+        Returns:
+            A workspace object
         """
         return await super().get(guid)
 
     async def update(self, guid: str, name: str) -> Workspace:
         """
         Update workspace data. Currently, only name update is supported.
 
         Args:
             guid (str): ID of a data_index to update. project_guid you sent during the workspace creation
             name: str. New workspace name.
 
-        Returns: Updated workspace instance
+        Returns:
+            Updated workspace instance
         """
-        return await super().update(id=guid, name=name)
+        return await super().update(guid=guid, name=name)
 
     async def delete(self, guid: str) -> Workspace:
         """
         Delete Workspace based on the id.
 
         Args:
             guid (str): ID of a workspace to delete. project_guid you sent during the workspace creation
 
-        Returns: Deleted workspace object
+        Returns:
+            Deleted workspace object
         """
         return await super().delete(guid)
 
     async def get_workspace_apps(self, guid: str) -> List[Application]:
         """
         Retrieves the list of applications for workspace defined by provided guid
 
         Args:
             guid (str): The ID of workspace to fetch applications for.
 
-        Returns: List of applications found in a workspace
+        Returns:
+            List of applications found in a workspace
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.get(
                     WORKSPACE_APPS_ENDPOINT.format(id=guid),
                 )
                 return [
                     Application._from_engine_format(application)
                     for application in response
                 ]
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise WorkspaceOrUserNotFoundError()
 
                 raise UnknownKluAPIError(e.status, e.message)
 
     async def get_workspace_indices(self, guid: str) -> List[DataIndex]:
         """
         Retrieves the list of data_indices for workspace defined by provided guid
 
         Args:
             guid (str): The ID of workspace to fetch data_indices for.
                 project_guid you sent during the workspace creation
 
-        Returns: List of DataIndex objects found on a workspace.
+        Returns:
+            List of DataIndex objects found on a workspace.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.get(
                     WORKSPACE_INDICES_ENDPOINT.format(id=guid),
                 )
                 return [
                     DataIndex._from_engine_format(data_index) for data_index in response
                 ]
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise WorkspaceOrUserNotFoundError()
 
                 raise UnknownKluAPIError(e.status, e.message)
 
     async def get_workspace_models(self, guid: str) -> List[Model]:
         """
         Retrieves the list of models for provided workspace id
 
         Args:
             guid (str): The ID of workspace to fetch models for. project_guid you sent during the workspace creation
 
-        Returns: List of Model objects found on a workspace.
+        Returns:
+            List of Model objects found on a workspace.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.get(
                     WORKSPACE_MODELS_ENDPOINT.format(id=guid),
                 )
                 return [Model._from_engine_format(model) for model in response]
-            except (HTTPNotFound, ClientResponseError) as e:
+            except ClientResponseError as e:
                 if e.status == 404:
                     raise WorkspaceOrUserNotFoundError()
 
                 raise UnknownKluAPIError(e.status, e.message)
 
     async def list(self) -> List[Workspace]:
         """
         Retrieves all workspaces for a user represented by the used API_KEY.
         Does not rely on internal paginator state, so `reset_pagination` method call can be skipped
 
-        Returns: An array of all workspaces
+        Returns:
+            An array of all workspaces
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_all(client)
 
             return [Workspace._from_engine_format(workspace) for workspace in response]
 
@@ -165,37 +173,39 @@
         Can be used to fetch a specific page of workspaces provided a certain per_page config.
         Does not rely on internal paginator state, so `reset_pagination` method call can be skipped
 
         Args:
             page_number (int): Number of the page to fetch
             limit (int): Number of instances to fetch per page. Defaults to 50
 
-        Returns: An array of workspaces fetched for a queried page. Empty if queried page does not exist
+        Returns:
+            An array of workspaces fetched for a queried page. Empty if queried page does not exist
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_single_page(
                 client, page_number, limit=limit
             )
 
             return [Workspace._from_engine_format(workspace) for workspace in response]
 
     async def fetch_next_page(
-        self, limit: int = DEFAULT_WORKSPACE_PAGE_SIZE, offset: int = None
+        self, limit: int = DEFAULT_WORKSPACE_PAGE_SIZE, offset: Optional[int] = None
     ) -> List[Workspace]:
         """
         Retrieves the next page of workspaces. Can be used to fetch a flexible number of pages starting.
         The place to start from can be controlled by the offset parameter.
         After using this method, we suggest to call `reset_pagination` method to reset the page cursor.
 
         Args:
             limit (int): Number of instances to fetch per page. Defaults to 50
             offset (int): The number of instances to skip. Can be used to query the pages of workspaces skipping certain number of instances.
 
-        Returns: An array of workspaces fetched for a queried page. Empty if the end was reached at the previous step.
+        Returns:
+            An array of workspaces fetched for a queried page. Empty if the end was reached at the previous step.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             response = await self._paginator.fetch_next_page(
                 client, limit=limit, offset=offset
             )
```

