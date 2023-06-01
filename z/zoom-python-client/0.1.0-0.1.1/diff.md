# Comparing `tmp/zoom_python_client-0.1.0.tar.gz` & `tmp/zoom_python_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoom_python_client-0.1.0.tar", max compression
+gzip compressed data, was "zoom_python_client-0.1.1.tar", max compression
```

## Comparing `zoom_python_client-0.1.0.tar` & `zoom_python_client-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-05-30 09:35:24.927101 zoom_python_client-0.1.0/LICENSE
--rw-r--r--   0        0        0     3306 2023-05-30 09:35:24.927101 zoom_python_client-0.1.0/README.md
--rw-r--r--   0        0        0     1381 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/__init__.py
--rw-r--r--   0        0        0     2401 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/api_client.py
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/meeting_livestreams/__init__.py
--rw-r--r--   0        0        0     1722 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/meetings/__init__.py
--rw-r--r--   0        0        0      624 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/meetings/meetings_component.py
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/users/__init__.py
--rw-r--r--   0        0        0     1286 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/users/users_component.py
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/webinar_livestreams/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/webinars/__init__.py
--rw-r--r--   0        0        0      401 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/webinars/webinars_component.py
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/utils/__init__.py
--rw-r--r--   0        0        0      221 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/utils/file_system.py
--rw-r--r--   0        0        0      731 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/utils/logger.py
--rw-r--r--   0        0        0     5954 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/zoom_api_client.py
--rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/zoom_auth_api/__init__.py
--rw-r--r--   0        0        0     4629 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
--rw-r--r--   0        0        0      817 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/zoom_client_interface.py
--rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 zoom_python_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-06-01 10:22:42.927116 zoom_python_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3306 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/README.md
+-rw-r--r--   0        0        0     1346 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/__init__.py
+-rw-r--r--   0        0        0     2401 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/api_client.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/meeting_livestreams/__init__.py
+-rw-r--r--   0        0        0     1722 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/meetings/__init__.py
+-rw-r--r--   0        0        0      624 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/meetings/meetings_component.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/users/__init__.py
+-rw-r--r--   0        0        0     1286 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/users/users_component.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/webinar_livestreams/__init__.py
+-rw-r--r--   0        0        0     1583 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/webinars/__init__.py
+-rw-r--r--   0        0        0      401 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/client_components/webinars/webinars_component.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/utils/file_system.py
+-rw-r--r--   0        0        0      731 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/utils/logger.py
+-rw-r--r--   0        0        0     8132 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/zoom_api_client.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/zoom_auth_api/__init__.py
+-rw-r--r--   0        0        0     4629 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
+-rw-r--r--   0        0        0      817 2023-06-01 10:22:42.931116 zoom_python_client-0.1.1/zoom_python_client/zoom_client_interface.py
+-rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 zoom_python_client-0.1.1/PKG-INFO
```

### Comparing `zoom_python_client-0.1.0/README.md` & `zoom_python_client-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 # Zoom Python client
 
 [![Python tests](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml) [![pre-commit](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml) [![CodeQL](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml) [![codecov](https://codecov.io/gh/cern-vc/zoom-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/cern-vc/zoom-python-client)
 
-> ⚠️ WIP: This project is a WIP and therefore may contain bugs. Use it at your own risk and keep this in mind if you decide to use it in production environments.
-
 Zoom API Python client with support for [Server to Server Oauth tokens](https://developers.zoom.us/docs/internal-apps/s2s-oauth/)
 
+## Install
+
+This package is [available on Pypi](https://pypi.org/project/zoom-python-client/)
+
+```bash
+pip install zoom-python-client
+```
+
+## Requirements
+
+- Python >= 3.9
+
 ## Usage
 
 ### Defining your env variables
 
 Define the following variables in your `env` or your `.env` file:
 
 - ZOOM_ACCOUNT_ID
@@ -71,15 +81,15 @@
 result = zoom_client.meetings.get_meeting(MEETING_ID)
 print(result)
 ```
 
 ## Optional: How to configure the logging
 
 ```python
-from zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.utils.logger import setup_logs
 
 setup_logs(log_level=logging.DEBUG)
 ```
 
 ## Available endpoints
 
 ### **users**:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zoom_python_client-0.1.0/pyproject.toml` & `zoom_python_client-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "zoom-python-client"
-version = "0.1.0"
+version = "0.1.1"
 authors = ["Rene Fernandez Sanchez <rene.fernandez@cern.ch>"]
 maintainers = ["Rene Fernandez Sanchez <rene.fernandez@cern.ch>"]
 classifiers = [
   "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+  "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
 description = "Zoom API client for Python using server to server tokens"
 homepage = "https://github.com/cern-vc/zoom-python-client"
 keywords = ["zoom", "api"]
-license = "GPL-3.0-only"
+license = "MIT"
 packages = [{ include = "zoom_python_client" }]
 readme = "README.md"
 repository = "https://github.com/cern-vc/zoom-python-client"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^0.21"
```

### Comparing `zoom_python_client-0.1.0/zoom_python_client/api_client.py` & `zoom_python_client-0.1.1/zoom_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.0/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py` & `zoom_python_client-0.1.1/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.0/zoom_python_client/client_components/meetings/meetings_component.py` & `zoom_python_client-0.1.1/zoom_python_client/client_components/meetings/meetings_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.0/zoom_python_client/client_components/users/users_component.py` & `zoom_python_client-0.1.1/zoom_python_client/client_components/users/users_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.0/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py` & `zoom_python_client-0.1.1/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.0/zoom_python_client/utils/logger.py` & `zoom_python_client-0.1.1/zoom_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.0/zoom_python_client/zoom_api_client.py` & `zoom_python_client-0.1.1/zoom_python_client/zoom_api_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -108,15 +108,18 @@
         token_from = "file" if self.use_path else "environment"
         if (
             not access_token
             or not expire_seconds
             or self.authentication_client.is_zoom_access_token_expired(expire_seconds)
             or force_token
         ):
-            logger.debug(f"Token is not in the {token_from}. Requesting new token.")
+            if force_token:
+                logger.debug("Forcing token refresh")
+            else:
+                logger.debug(f"Token is not in the {token_from}. Requesting new token.")
             access_token = self.authentication_client.get_acceess_token()
         else:
             logger.debug(f"The token is the {token_from}. No need for a new token.")
         zoom_headers = {"Authorization": "Bearer " + access_token}
         headers = self.api_client.build_headers(extra_headers=zoom_headers)
         return headers
 
@@ -129,31 +132,82 @@
 
     def make_get_request(
         self, api_path: str, parameters: dict = {}
     ) -> Union[requests.Response, None]:
         headers = self.build_zoom_authorization_headers()
         # convert parameters dict to query string
         query_string = self.build_query_string_from_dict(parameters)
+        response = requests.Response()
+        try:
+            response = self.api_client.make_get_request(
+                api_path + query_string, headers=headers
+            )
+        # Handle 401 error from requests
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code == 401:
+                logger.debug(
+                    f"Got 401 error from Zoom API Get ({error}). Retrying with a new token."
+                )
+                response = self.retry_get_request(api_path, query_string)
+        return response
+
+    def retry_get_request(self, api_path, query_string):
+        headers = self.build_zoom_authorization_headers(force_token=True)
         response = self.api_client.make_get_request(
             api_path + query_string, headers=headers
         )
+
         return response
 
     def make_post_request(
         self, api_path: str, data: Mapping[str, Any]
     ) -> Union[requests.Response, None]:
         headers = self.build_zoom_authorization_headers()
         response = requests.Response()
+        try:
+            response = self.api_client.make_post_request(
+                api_path, headers=headers, data=data
+            )
+        # Handle 401 error from requests
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code == 401:
+                logger.debug(
+                    f"Got 401 error from Zoom API Post ({error}). Retrying with a new token."
+                )
+                response = self.retry_post_request(api_path, data)
+
+        return response
+
+    def retry_post_request(self, api_path, data):
+        headers = self.build_zoom_authorization_headers(force_token=True)
         response = self.api_client.make_post_request(
             api_path, headers=headers, data=data
         )
+
         return response
 
     def make_patch_request(
         self, api_path: str, data: Mapping[str, Any]
     ) -> Union[requests.Response, None]:
         headers = self.build_zoom_authorization_headers()
+        response = requests.Response()
+        try:
+            response = self.api_client.make_patch_request(
+                api_path, headers=headers, data=data
+            )
+        # Handle 401 error from requests
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code == 401:
+                # Retry generating a new token
+                logger.debug(
+                    f"Got 401 error from Zoom API Patch ({error}). Retrying with a new token."
+                )
+                response = self.retry_patch_request(api_path, data)
+        return response
 
+    def retry_patch_request(self, api_path, data):
+        headers = self.build_zoom_authorization_headers(force_token=True)
         response = self.api_client.make_patch_request(
             api_path, headers=headers, data=data
         )
+
         return response
```

### Comparing `zoom_python_client-0.1.0/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py` & `zoom_python_client-0.1.1/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.0/zoom_python_client/zoom_client_interface.py` & `zoom_python_client-0.1.1/zoom_python_client/zoom_client_interface.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.1.0/PKG-INFO` & `zoom_python_client-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zoom-python-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Zoom API client for Python using server to server tokens
 Home-page: https://github.com/cern-vc/zoom-python-client
-License: GPL-3.0-only
+License: MIT
 Keywords: zoom,api
 Author: Rene Fernandez Sanchez
 Author-email: rene.fernandez@cern.ch
 Maintainer: Rene Fernandez Sanchez
 Maintainer-email: rene.fernandez@cern.ch
 Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-dotenv (>=0.21,<0.22)
 Requires-Dist: requests (>=2.23,<3.0)
@@ -23,18 +23,28 @@
 Project-URL: Repository, https://github.com/cern-vc/zoom-python-client
 Description-Content-Type: text/markdown
 
 # Zoom Python client
 
 [![Python tests](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml) [![pre-commit](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml) [![CodeQL](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml) [![codecov](https://codecov.io/gh/cern-vc/zoom-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/cern-vc/zoom-python-client)
 
-> ⚠️ WIP: This project is a WIP and therefore may contain bugs. Use it at your own risk and keep this in mind if you decide to use it in production environments.
-
 Zoom API Python client with support for [Server to Server Oauth tokens](https://developers.zoom.us/docs/internal-apps/s2s-oauth/)
 
+## Install
+
+This package is [available on Pypi](https://pypi.org/project/zoom-python-client/)
+
+```bash
+pip install zoom-python-client
+```
+
+## Requirements
+
+- Python >= 3.9
+
 ## Usage
 
 ### Defining your env variables
 
 Define the following variables in your `env` or your `.env` file:
 
 - ZOOM_ACCOUNT_ID
@@ -96,15 +106,15 @@
 result = zoom_client.meetings.get_meeting(MEETING_ID)
 print(result)
 ```
 
 ## Optional: How to configure the logging
 
 ```python
-from zoom_python_client.zoom_api_client import ZoomApiClient
+from zoom_python_client.utils.logger import setup_logs
 
 setup_logs(log_level=logging.DEBUG)
 ```
 
 ## Available endpoints
 
 ### **users**:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

