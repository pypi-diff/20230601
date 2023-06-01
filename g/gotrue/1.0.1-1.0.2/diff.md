# Comparing `tmp/gotrue-1.0.1.tar.gz` & `tmp/gotrue-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrue-1.0.1.tar", max compression
+gzip compressed data, was "gotrue-1.0.2.tar", max compression
```

## Comparing `gotrue-1.0.1.tar` & `gotrue-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-11-05 22:33:59.239689 gotrue-1.0.1/LICENSE
--rw-r--r--   0        0        0     5053 2022-11-05 22:33:59.239892 gotrue-1.0.1/README.md
--rw-r--r--   0        0        0      751 2023-04-03 15:22:04.578272 gotrue-1.0.1/gotrue/__init__.py
--rw-r--r--   0        0        0       35 2022-11-05 22:33:59.240564 gotrue-1.0.1/gotrue/_async/__init__.py
--rw-r--r--   0        0        0    19223 2023-01-29 06:28:16.626281 gotrue-1.0.1/gotrue/_async/api.py
--rw-r--r--   0        0        0    22648 2023-02-05 13:49:37.789911 gotrue-1.0.1/gotrue/_async/client.py
--rw-r--r--   0        0        0     5182 2023-01-29 14:15:19.161481 gotrue-1.0.1/gotrue/_async/gotrue_admin_api.py
--rw-r--r--   0        0        0      947 2023-01-29 14:15:19.161743 gotrue-1.0.1/gotrue/_async/gotrue_admin_mfa_api.py
--rw-r--r--   0        0        0     3718 2023-01-29 14:15:19.161955 gotrue-1.0.1/gotrue/_async/gotrue_base_api.py
--rw-r--r--   0        0        0    30749 2023-01-29 14:15:19.162126 gotrue-1.0.1/gotrue/_async/gotrue_client.py
--rw-r--r--   0        0        0     3956 2023-02-05 13:49:31.139486 gotrue-1.0.1/gotrue/_async/gotrue_mfa_api.py
--rw-r--r--   0        0        0      925 2022-11-05 22:33:59.240887 gotrue-1.0.1/gotrue/_async/storage.py
--rw-r--r--   0        0        0       35 2023-01-29 14:59:14.000000 gotrue-1.0.1/gotrue/_sync/__init__.py
--rw-r--r--   0        0        0    18964 2023-01-29 14:59:14.000000 gotrue-1.0.1/gotrue/_sync/api.py
--rw-r--r--   0        0        0    22135 2023-02-05 13:49:37.790515 gotrue-1.0.1/gotrue/_sync/client.py
--rw-r--r--   0        0        0     5054 2023-01-29 14:59:14.000000 gotrue-1.0.1/gotrue/_sync/gotrue_admin_api.py
--rw-r--r--   0        0        0      934 2023-01-29 14:59:14.000000 gotrue-1.0.1/gotrue/_sync/gotrue_admin_mfa_api.py
--rw-r--r--   0        0        0     3652 2023-01-29 14:59:14.000000 gotrue-1.0.1/gotrue/_sync/gotrue_base_api.py
--rw-r--r--   0        0        0    30139 2023-01-29 15:00:13.055483 gotrue-1.0.1/gotrue/_sync/gotrue_client.py
--rw-r--r--   0        0        0     3913 2023-01-29 14:59:14.000000 gotrue-1.0.1/gotrue/_sync/gotrue_mfa_api.py
--rw-r--r--   0        0        0      886 2023-01-29 14:59:14.000000 gotrue-1.0.1/gotrue/_sync/storage.py
--rw-r--r--   0        0        0      329 2023-01-29 14:15:19.164045 gotrue-1.0.1/gotrue/constants.py
--rw-r--r--   0        0        0     2893 2023-01-29 14:15:19.164103 gotrue-1.0.1/gotrue/errors.py
--rw-r--r--   0        0        0     3020 2023-04-03 15:21:37.659728 gotrue-1.0.1/gotrue/helpers.py
--rw-r--r--   0        0        0      202 2022-11-05 22:33:59.241561 gotrue-1.0.1/gotrue/http_clients.py
--rw-r--r--   0        0        0     1366 2023-01-29 14:15:19.164263 gotrue-1.0.1/gotrue/timer.py
--rw-r--r--   0        0        0    15530 2023-01-29 14:15:19.164533 gotrue-1.0.1/gotrue/types.py
--rw-r--r--   0        0        0     1546 2023-04-03 15:21:54.630866 gotrue-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5870 1970-01-01 00:00:00.000000 gotrue-1.0.1/setup.py
--rw-r--r--   0        0        0     5962 1970-01-01 00:00:00.000000 gotrue-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-11-05 22:33:59.239689 gotrue-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5041 2023-06-01 10:45:55.707482 gotrue-1.0.2/README.md
+-rw-r--r--   0        0        0      751 2023-06-01 05:34:22.268497 gotrue-1.0.2/gotrue/__init__.py
+-rw-r--r--   0        0        0       35 2022-11-05 22:33:59.240564 gotrue-1.0.2/gotrue/_async/__init__.py
+-rw-r--r--   0        0        0    19223 2023-01-29 06:28:16.626281 gotrue-1.0.2/gotrue/_async/api.py
+-rw-r--r--   0        0        0    22648 2023-02-05 13:49:37.789911 gotrue-1.0.2/gotrue/_async/client.py
+-rw-r--r--   0        0        0     5182 2023-01-29 14:15:19.161481 gotrue-1.0.2/gotrue/_async/gotrue_admin_api.py
+-rw-r--r--   0        0        0      947 2023-01-29 14:15:19.161743 gotrue-1.0.2/gotrue/_async/gotrue_admin_mfa_api.py
+-rw-r--r--   0        0        0     3718 2023-01-29 14:15:19.161955 gotrue-1.0.2/gotrue/_async/gotrue_base_api.py
+-rw-r--r--   0        0        0    30677 2023-06-01 05:34:22.269640 gotrue-1.0.2/gotrue/_async/gotrue_client.py
+-rw-r--r--   0        0        0     3956 2023-02-05 13:49:31.139486 gotrue-1.0.2/gotrue/_async/gotrue_mfa_api.py
+-rw-r--r--   0        0        0      925 2022-11-05 22:33:59.240887 gotrue-1.0.2/gotrue/_async/storage.py
+-rw-r--r--   0        0        0       35 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/__init__.py
+-rw-r--r--   0        0        0    18964 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/api.py
+-rw-r--r--   0        0        0    22135 2023-06-01 10:47:25.880339 gotrue-1.0.2/gotrue/_sync/client.py
+-rw-r--r--   0        0        0     5054 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/gotrue_admin_api.py
+-rw-r--r--   0        0        0      934 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/gotrue_admin_mfa_api.py
+-rw-r--r--   0        0        0     3652 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/gotrue_base_api.py
+-rw-r--r--   0        0        0    30067 2023-06-01 10:47:26.012486 gotrue-1.0.2/gotrue/_sync/gotrue_client.py
+-rw-r--r--   0        0        0     3913 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/gotrue_mfa_api.py
+-rw-r--r--   0        0        0      886 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/storage.py
+-rw-r--r--   0        0        0      329 2023-01-29 14:15:19.164045 gotrue-1.0.2/gotrue/constants.py
+-rw-r--r--   0        0        0     2893 2023-01-29 14:15:19.164103 gotrue-1.0.2/gotrue/errors.py
+-rw-r--r--   0        0        0     3035 2023-06-01 05:34:22.270484 gotrue-1.0.2/gotrue/helpers.py
+-rw-r--r--   0        0        0      202 2022-11-05 22:33:59.241561 gotrue-1.0.2/gotrue/http_clients.py
+-rw-r--r--   0        0        0     1366 2023-01-29 14:15:19.164263 gotrue-1.0.2/gotrue/timer.py
+-rw-r--r--   0        0        0    15550 2023-06-01 05:34:22.270717 gotrue-1.0.2/gotrue/types.py
+-rw-r--r--   0        0        0     1551 2023-06-01 05:34:34.007395 gotrue-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 gotrue-1.0.2/PKG-INFO
```

### Comparing `gotrue-1.0.1/LICENSE` & `gotrue-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/README.md` & `gotrue-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 ## Usage (outdated)
 
 **Important:** This section is outdated, you can be guided by the [JS client documentation](https://supabase.github.io/gotrue-js) because this Python client has a lot of parity with the JS client.
 
 To instantiate the client, you'll need the URL and any request headers at a minimum.
 
 ```python
-from gotrue import Client
+from gotrue import SyncGoTrueClient
 
 headers = {
     "apiKey": "my-mega-awesome-api-key",
     # ... any other headers you might need.
 }
-client: Client = Client(url="www.genericauthwebsite.com", headers=headers)
+client: SyncGoTrueClient = SyncGoTrueClient(url="www.genericauthwebsite.com", headers=headers)
 ```
 
 To send a magic email link to the user, just provide the email kwarg to the `sign_in` method:
 
 ```python
 user: Dict[str, Any] = client.sign_up(email="example@gmail.com")
 ```
@@ -92,10 +92,7 @@
 assert client.user() is not None
 assert client.session() is not None
 ```
 
 ## Contributions
 
 We would be immensely grateful for any contributions to this project. In particular are the following items:
-
-- Add documentation
-- Update `README.md`
```

### Comparing `gotrue-1.0.1/gotrue/__init__.py` & `gotrue-1.0.2/gotrue/__init__.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_async/api.py` & `gotrue-1.0.2/gotrue/_async/api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_async/client.py` & `gotrue-1.0.2/gotrue/_async/client.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_async/gotrue_admin_api.py` & `gotrue-1.0.2/gotrue/_async/gotrue_admin_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_async/gotrue_admin_mfa_api.py` & `gotrue-1.0.2/gotrue/_async/gotrue_admin_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_async/gotrue_base_api.py` & `gotrue-1.0.2/gotrue/_async/gotrue_base_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_async/gotrue_client.py` & `gotrue-1.0.2/gotrue/_async/gotrue_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from json import loads
 from time import time
 from typing import Callable, Dict, List, Tuple, Union
-from urllib.parse import parse_qs, quote, urlencode, urlparse
+from urllib.parse import parse_qs, urlencode, urlparse
 from uuid import uuid4
 
 from ..constants import (
     DEFAULT_HEADERS,
     EXPIRY_MARGIN,
     GOTRUE_URL,
     MAX_RETRIES,
@@ -825,16 +825,15 @@
         return "access_token" in params or "error_description" in params
 
     def _get_url_for_provider(
         self,
         provider: Provider,
         params: Dict[str, str],
     ) -> str:
-        params = {k: quote(v) for k, v in params.items()}
-        params["provider"] = quote(provider)
+        params["provider"] = provider
         query = urlencode(params)
         return f"{self._url}/authorize?{query}"
 
     def _decode_jwt(self, jwt: str) -> DecodedJWTDict:
         """
         Decodes a JWT (without performing any validation).
         """
```

### Comparing `gotrue-1.0.1/gotrue/_async/gotrue_mfa_api.py` & `gotrue-1.0.2/gotrue/_async/gotrue_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_async/storage.py` & `gotrue-1.0.2/gotrue/_async/storage.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_sync/api.py` & `gotrue-1.0.2/gotrue/_sync/api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_sync/client.py` & `gotrue-1.0.2/gotrue/_sync/client.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_sync/gotrue_admin_api.py` & `gotrue-1.0.2/gotrue/_sync/gotrue_admin_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_sync/gotrue_admin_mfa_api.py` & `gotrue-1.0.2/gotrue/_sync/gotrue_admin_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_sync/gotrue_base_api.py` & `gotrue-1.0.2/gotrue/_sync/gotrue_base_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_sync/gotrue_client.py` & `gotrue-1.0.2/gotrue/_sync/gotrue_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from json import loads
 from time import time
 from typing import Callable, Dict, List, Tuple, Union
-from urllib.parse import parse_qs, quote, urlencode, urlparse
+from urllib.parse import parse_qs, urlencode, urlparse
 from uuid import uuid4
 
 from ..constants import (
     DEFAULT_HEADERS,
     EXPIRY_MARGIN,
     GOTRUE_URL,
     MAX_RETRIES,
@@ -823,16 +823,15 @@
         return "access_token" in params or "error_description" in params
 
     def _get_url_for_provider(
         self,
         provider: Provider,
         params: Dict[str, str],
     ) -> str:
-        params = {k: quote(v) for k, v in params.items()}
-        params["provider"] = quote(provider)
+        params["provider"] = provider
         query = urlencode(params)
         return f"{self._url}/authorize?{query}"
 
     def _decode_jwt(self, jwt: str) -> DecodedJWTDict:
         """
         Decodes a JWT (without performing any validation).
         """
```

### Comparing `gotrue-1.0.1/gotrue/_sync/gotrue_mfa_api.py` & `gotrue-1.0.2/gotrue/_sync/gotrue_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/_sync/storage.py` & `gotrue-1.0.2/gotrue/_sync/storage.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/errors.py` & `gotrue-1.0.2/gotrue/errors.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/helpers.py` & `gotrue-1.0.2/gotrue/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         and "refresh_token" in data
         and "expires_in" in data
         and data["access_token"]
         and data["refresh_token"]
         and data["expires_in"]
     ):
         session = Session.parse_obj(data)
-    user = User.parse_obj(data["user"]) if "user" in data else User.parse_obj(data)
+    user_data = data.get("user", data)
+    user = User.parse_obj(user_data) if user_data else None
     return AuthResponse(session=session, user=user)
 
 
 def parse_link_response(data: Any) -> GenerateLinkResponse:
     properties = GenerateLinkProperties(
         action_link=data.get("action_link"),
         email_otp=data.get("email_otp"),
```

### Comparing `gotrue-1.0.1/gotrue/timer.py` & `gotrue-1.0.2/gotrue/timer.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.1/gotrue/types.py` & `gotrue-1.0.2/gotrue/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 class UserIdentity(BaseModel):
     id: str
     user_id: str
     identity_data: Dict[str, Any]
     provider: str
     created_at: datetime
-    last_sign_in_at: datetime
+    last_sign_in_at: Union[datetime, None] = None
     updated_at: Union[datetime, None] = None
 
 
 class Factor(BaseModel):
     """
     A MFA factor.
     """
```

### Comparing `gotrue-1.0.1/pyproject.toml` & `gotrue-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gotrue"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python Client Library for GoTrue"
 authors = ["Joel Lee <joel@joellee.org>"]
 homepage = "https://github.com/supabase-community/gotrue-py"
 repository = "https://github.com/supabase-community/gotrue-py"
 documentation = "https://github.com/supabase-community/gotrue-py"
 readme = "README.md"
 license = "MIT"
@@ -12,23 +12,23 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.23.0"
+httpx = ">=0.23,<0.25"
 pydantic = "^1.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 flake8 = "^5.0.4"
 black = "^23.1.0"
 isort = "^5.12.0"
-pre-commit = "^3.1.1"
+pre-commit = "^3.2.2"
 pytest-cov = "^4.0.0"
 pytest-depends = "^1.0.1"
 pytest-asyncio = "^0.20.3"
 Faker = "^18.3.1"
 unasync-cli = "^0.0.9"
 python-semantic-release = "^7.33.2"
```

### Comparing `gotrue-1.0.1/setup.py` & `gotrue-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,122 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gotrue
+Version: 1.0.2
+Summary: Python Client Library for GoTrue
+Home-page: https://github.com/supabase-community/gotrue-py
+License: MIT
+Author: Joel Lee
+Author-email: joel@joellee.org
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: httpx (>=0.23,<0.25)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Project-URL: Documentation, https://github.com/supabase-community/gotrue-py
+Project-URL: Repository, https://github.com/supabase-community/gotrue-py
+Description-Content-Type: text/markdown
 
-packages = \
-['gotrue', 'gotrue._async', 'gotrue._sync']
+# gotrue-py
 
-package_data = \
-{'': ['*']}
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)
+[![CI](https://github.com/supabase-community/gotrue-py/actions/workflows/ci.yml/badge.svg)](https://github.com/supabase-community/gotrue-py/actions/workflows/ci.yml)
+[![Python](https://img.shields.io/pypi/pyversions/gotrue)](https://pypi.org/project/gotrue)
+[![Version](https://img.shields.io/pypi/v/gotrue?color=%2334D058)](https://pypi.org/project/gotrue)
+[![Codecov](https://codecov.io/gh/supabase-community/gotrue-py/branch/main/graph/badge.svg)](https://codecov.io/gh/supabase-community/gotrue-py)
+[![Last commit](https://img.shields.io/github/last-commit/supabase-community/gotrue-py.svg?style=flat)](https://github.com/supabase-community/gotrue-py/commits)
+[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/supabase-community/gotrue-py)](https://github.com/supabase-community/gotrue-py/commits)
+[![Github Stars](https://img.shields.io/github/stars/supabase-community/gotrue-py?style=flat&logo=github)](https://github.com/supabase-community/gotrue-py/stargazers)
+[![Github Forks](https://img.shields.io/github/forks/supabase-community/gotrue-py?style=flat&logo=github)](https://github.com/supabase-community/gotrue-py/network/members)
+[![Github Watchers](https://img.shields.io/github/watchers/supabase-community/gotrue-py?style=flat&logo=github)](https://github.com/supabase-community/gotrue-py)
+[![GitHub contributors](https://img.shields.io/github/contributors/supabase-community/gotrue-py)](https://github.com/supabase-community/gotrue-py/graphs/contributors)
 
-install_requires = \
-['httpx>=0.23.0,<0.24.0', 'pydantic>=1.10.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'gotrue',
-    'version': '1.0.1',
-    'description': 'Python Client Library for GoTrue',
-    'long_description': '# gotrue-py\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)\n[![CI](https://github.com/supabase-community/gotrue-py/actions/workflows/ci.yml/badge.svg)](https://github.com/supabase-community/gotrue-py/actions/workflows/ci.yml)\n[![Python](https://img.shields.io/pypi/pyversions/gotrue)](https://pypi.org/project/gotrue)\n[![Version](https://img.shields.io/pypi/v/gotrue?color=%2334D058)](https://pypi.org/project/gotrue)\n[![Codecov](https://codecov.io/gh/supabase-community/gotrue-py/branch/main/graph/badge.svg)](https://codecov.io/gh/supabase-community/gotrue-py)\n[![Last commit](https://img.shields.io/github/last-commit/supabase-community/gotrue-py.svg?style=flat)](https://github.com/supabase-community/gotrue-py/commits)\n[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/supabase-community/gotrue-py)](https://github.com/supabase-community/gotrue-py/commits)\n[![Github Stars](https://img.shields.io/github/stars/supabase-community/gotrue-py?style=flat&logo=github)](https://github.com/supabase-community/gotrue-py/stargazers)\n[![Github Forks](https://img.shields.io/github/forks/supabase-community/gotrue-py?style=flat&logo=github)](https://github.com/supabase-community/gotrue-py/network/members)\n[![Github Watchers](https://img.shields.io/github/watchers/supabase-community/gotrue-py?style=flat&logo=github)](https://github.com/supabase-community/gotrue-py)\n[![GitHub contributors](https://img.shields.io/github/contributors/supabase-community/gotrue-py)](https://github.com/supabase-community/gotrue-py/graphs/contributors)\n\nThis is a Python port of the [supabase js gotrue client](https://github.com/supabase/gotrue-js). The current state is that there is a features parity but with small differences that are mentioned in the section **Differences to the JS client**.\n\n## Installation\n\nWe are still working on making the `gotrue` python library more user-friendly. For now here are some sparse notes on how to install the module.\n\n### Poetry\n\n```bash\npoetry add gotrue\n```\n\n### Pip\n\n```bash\npip install gotrue\n```\n\n## Differences to the JS client\n\nIt should be noted there are differences to the [JS client](https://github.com/supabase/gotrue-js). If you feel particulaly strongly about them and want to motivate a change, feel free to make a GitHub issue and we can discuss it there.\n\nFirstly, feature pairity is not 100% with the [JS client](https://github.com/supabase/gotrue-js). In most cases we match the methods and attributes of the [JS client](https://github.com/supabase/gotrue-js) and api classes, but is some places (e.g for browser specific code) it didn\'t make sense to port the code line for line.\n\nThere is also a divergence in terms of how errors are raised. In the [JS client](https://github.com/supabase/gotrue-js), the errors are returned as part of the object, which the user can choose to process in whatever way they see fit. In this Python client, we raise the errors directly where they originate, as it was felt this was more Pythonic and adhered to the idioms of the language more directly.\n\nIn JS we return the error, but in Python we just raise it.\n\n```js\nconst { data, error } = client.sign_up(...)\n```\n\nThe other key difference is we do not use pascalCase to encode variable and method names. Instead we use the snake_case convention adopted in the Python language.\n\nAlso, the `gotrue` library for Python parses the date-time string into `datetime` Python objects. The [JS client](https://github.com/supabase/gotrue-js) keeps the date-time as strings.\n\n## Usage (outdated)\n\n**Important:** This section is outdated, you can be guided by the [JS client documentation](https://supabase.github.io/gotrue-js) because this Python client has a lot of parity with the JS client.\n\nTo instantiate the client, you\'ll need the URL and any request headers at a minimum.\n\n```python\nfrom gotrue import Client\n\nheaders = {\n    "apiKey": "my-mega-awesome-api-key",\n    # ... any other headers you might need.\n}\nclient: Client = Client(url="www.genericauthwebsite.com", headers=headers)\n```\n\nTo send a magic email link to the user, just provide the email kwarg to the `sign_in` method:\n\n```python\nuser: Dict[str, Any] = client.sign_up(email="example@gmail.com")\n```\n\nTo login with email and password, provide both to the `sign_in` method:\n\n```python\nuser: Dict[str, Any] = client.sign_up(email="example@gmail.com", password="*********")\n```\n\nTo sign out of the logged in user, call the `sign_out` method. We can then assert that the session and user are null values.\n\n```python\nclient.sign_out()\nassert client.user() is None\nassert client.session() is None\n```\n\nWe can refesh a users session.\n\n```python\n# The user should already be signed in at this stage.\nuser = client.refresh_session()\nassert client.user() is not None\nassert client.session() is not None\n```\n\n## Contributions\n\nWe would be immensely grateful for any contributions to this project. In particular are the following items:\n\n- Add documentation\n- Update `README.md`\n',
-    'author': 'Joel Lee',
-    'author_email': 'joel@joellee.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/supabase-community/gotrue-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+This is a Python port of the [supabase js gotrue client](https://github.com/supabase/gotrue-js). The current state is that there is a features parity but with small differences that are mentioned in the section **Differences to the JS client**.
+
+## Installation
+
+We are still working on making the `gotrue` python library more user-friendly. For now here are some sparse notes on how to install the module.
+
+### Poetry
+
+```bash
+poetry add gotrue
+```
+
+### Pip
+
+```bash
+pip install gotrue
+```
+
+## Differences to the JS client
+
+It should be noted there are differences to the [JS client](https://github.com/supabase/gotrue-js). If you feel particulaly strongly about them and want to motivate a change, feel free to make a GitHub issue and we can discuss it there.
+
+Firstly, feature pairity is not 100% with the [JS client](https://github.com/supabase/gotrue-js). In most cases we match the methods and attributes of the [JS client](https://github.com/supabase/gotrue-js) and api classes, but is some places (e.g for browser specific code) it didn't make sense to port the code line for line.
+
+There is also a divergence in terms of how errors are raised. In the [JS client](https://github.com/supabase/gotrue-js), the errors are returned as part of the object, which the user can choose to process in whatever way they see fit. In this Python client, we raise the errors directly where they originate, as it was felt this was more Pythonic and adhered to the idioms of the language more directly.
+
+In JS we return the error, but in Python we just raise it.
+
+```js
+const { data, error } = client.sign_up(...)
+```
+
+The other key difference is we do not use pascalCase to encode variable and method names. Instead we use the snake_case convention adopted in the Python language.
+
+Also, the `gotrue` library for Python parses the date-time string into `datetime` Python objects. The [JS client](https://github.com/supabase/gotrue-js) keeps the date-time as strings.
+
+## Usage (outdated)
+
+**Important:** This section is outdated, you can be guided by the [JS client documentation](https://supabase.github.io/gotrue-js) because this Python client has a lot of parity with the JS client.
+
+To instantiate the client, you'll need the URL and any request headers at a minimum.
+
+```python
+from gotrue import SyncGoTrueClient
+
+headers = {
+    "apiKey": "my-mega-awesome-api-key",
+    # ... any other headers you might need.
 }
+client: SyncGoTrueClient = SyncGoTrueClient(url="www.genericauthwebsite.com", headers=headers)
+```
+
+To send a magic email link to the user, just provide the email kwarg to the `sign_in` method:
+
+```python
+user: Dict[str, Any] = client.sign_up(email="example@gmail.com")
+```
+
+To login with email and password, provide both to the `sign_in` method:
+
+```python
+user: Dict[str, Any] = client.sign_up(email="example@gmail.com", password="*********")
+```
+
+To sign out of the logged in user, call the `sign_out` method. We can then assert that the session and user are null values.
+
+```python
+client.sign_out()
+assert client.user() is None
+assert client.session() is None
+```
+
+We can refesh a users session.
+
+```python
+# The user should already be signed in at this stage.
+user = client.refresh_session()
+assert client.user() is not None
+assert client.session() is not None
+```
+
+## Contributions
 
+We would be immensely grateful for any contributions to this project. In particular are the following items:
 
-setup(**setup_kwargs)
```

