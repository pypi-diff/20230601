# Comparing `tmp/smart-rest-client-0.4.2.tar.gz` & `tmp/smart-rest-client-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart-rest-client-0.4.2.tar", last modified: Mon Jul 18 17:54:34 2022, max compression
+gzip compressed data, was "smart-rest-client-0.4.3.tar", last modified: Thu Jun  1 17:54:03 2023, max compression
```

## Comparing `smart-rest-client-0.4.2.tar` & `smart-rest-client-0.4.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.599979 smart-rest-client-0.4.2/
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)      605 2022-07-18 17:53:56.000000 smart-rest-client-0.4.2/CHANGES.rst
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)       89 2020-02-05 23:52:55.000000 smart-rest-client-0.4.2/MANIFEST.in
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     8316 2022-07-18 17:54:34.599702 smart-rest-client-0.4.2/PKG-INFO
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)     5645 2021-05-01 18:04:45.000000 smart-rest-client-0.4.2/README.pt.rst
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)     5951 2021-05-01 17:55:38.000000 smart-rest-client-0.4.2/README.rst
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.576814 smart-rest-client-0.4.2/docs/
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.576571 smart-rest-client-0.4.2/docs/en/
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.584070 smart-rest-client-0.4.2/docs/en/_static/
--rw-r--r--   0 rafaelhenter   (502) staff       (20)      286 2020-07-23 15:28:04.000000 smart-rest-client-0.4.2/docs/en/_static/file.png
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.585621 smart-rest-client-0.4.2/docs/en/_static/img/
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     8777 2020-07-25 23:07:54.000000 smart-rest-client-0.4.2/docs/en/_static/img/glyphicons-halflings-white.png
--rw-r--r--   0 rafaelhenter   (502) staff       (20)    12799 2020-07-25 23:07:54.000000 smart-rest-client-0.4.2/docs/en/_static/img/glyphicons-halflings.png
--rw-r--r--   0 rafaelhenter   (502) staff       (20)       90 2020-07-23 15:28:04.000000 smart-rest-client-0.4.2/docs/en/_static/minus.png
--rw-r--r--   0 rafaelhenter   (502) staff       (20)       90 2020-07-23 15:28:04.000000 smart-rest-client-0.4.2/docs/en/_static/plus.png
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.576889 smart-rest-client-0.4.2/docs/pt-br/
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.587884 smart-rest-client-0.4.2/docs/pt-br/_static/
--rw-r--r--   0 rafaelhenter   (502) staff       (20)      286 2020-07-23 15:28:04.000000 smart-rest-client-0.4.2/docs/pt-br/_static/file.png
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.589145 smart-rest-client-0.4.2/docs/pt-br/_static/img/
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     8777 2020-07-25 23:07:54.000000 smart-rest-client-0.4.2/docs/pt-br/_static/img/glyphicons-halflings-white.png
--rw-r--r--   0 rafaelhenter   (502) staff       (20)    12799 2020-07-25 23:07:54.000000 smart-rest-client-0.4.2/docs/pt-br/_static/img/glyphicons-halflings.png
--rw-r--r--   0 rafaelhenter   (502) staff       (20)       90 2020-07-23 15:28:04.000000 smart-rest-client-0.4.2/docs/pt-br/_static/minus.png
--rw-r--r--   0 rafaelhenter   (502) staff       (20)       90 2020-07-23 15:28:04.000000 smart-rest-client-0.4.2/docs/pt-br/_static/plus.png
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)       61 2021-04-30 20:48:56.000000 smart-rest-client-0.4.2/requirements-ci.txt
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)      155 2020-07-25 23:36:06.000000 smart-rest-client-0.4.2/requirements-dev.txt
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)       38 2022-07-18 17:52:53.000000 smart-rest-client-0.4.2/requirements.txt
--rw-r--r--   0 rafaelhenter   (502) staff       (20)       38 2022-07-18 17:54:34.600086 smart-rest-client-0.4.2/setup.cfg
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)     2312 2021-04-30 20:50:34.000000 smart-rest-client-0.4.2/setup.py
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.597633 smart-rest-client-0.4.2/smart_rest_client/
--rwxr-xr-x   0 rafaelhenter   (502) staff       (20)      147 2020-02-05 23:52:55.000000 smart-rest-client-0.4.2/smart_rest_client/__init__.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)    13434 2021-11-15 22:10:30.000000 smart-rest-client-0.4.2/smart_rest_client/base.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     3992 2021-07-15 19:25:15.000000 smart-rest-client-0.4.2/smart_rest_client/client.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     1656 2021-04-30 21:27:36.000000 smart-rest-client-0.4.2/smart_rest_client/exceptions.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     2266 2021-07-02 12:17:43.000000 smart-rest-client-0.4.2/smart_rest_client/factories.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     4222 2021-05-01 16:22:53.000000 smart-rest-client-0.4.2/smart_rest_client/settings.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     2223 2021-01-08 19:08:53.000000 smart-rest-client-0.4.2/smart_rest_client/status.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     2321 2022-07-18 17:53:56.000000 smart-rest-client-0.4.2/smart_rest_client/utils.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     1132 2021-04-30 19:06:01.000000 smart-rest-client-0.4.2/smart_rest_client/validators.py
--rw-r--r--   0 rafaelhenter   (502) staff       (20)       22 2022-07-18 17:54:34.000000 smart-rest-client-0.4.2/smart_rest_client/version.py
-drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2022-07-18 17:54:34.599276 smart-rest-client-0.4.2/smart_rest_client.egg-info/
--rw-r--r--   0 rafaelhenter   (502) staff       (20)     8316 2022-07-18 17:54:34.000000 smart-rest-client-0.4.2/smart_rest_client.egg-info/PKG-INFO
--rw-r--r--   0 rafaelhenter   (502) staff       (20)      971 2022-07-18 17:54:34.000000 smart-rest-client-0.4.2/smart_rest_client.egg-info/SOURCES.txt
--rw-r--r--   0 rafaelhenter   (502) staff       (20)        1 2022-07-18 17:54:34.000000 smart-rest-client-0.4.2/smart_rest_client.egg-info/dependency_links.txt
--rw-r--r--   0 rafaelhenter   (502) staff       (20)       38 2022-07-18 17:54:34.000000 smart-rest-client-0.4.2/smart_rest_client.egg-info/requires.txt
--rw-r--r--   0 rafaelhenter   (502) staff       (20)       18 2022-07-18 17:54:34.000000 smart-rest-client-0.4.2/smart_rest_client.egg-info/top_level.txt
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.161944 smart-rest-client-0.4.3/
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)      664 2023-06-01 17:53:37.000000 smart-rest-client-0.4.3/CHANGES.rst
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)       89 2020-02-05 23:52:55.000000 smart-rest-client-0.4.3/MANIFEST.in
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     8316 2023-06-01 17:54:03.161691 smart-rest-client-0.4.3/PKG-INFO
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)     5645 2021-05-01 18:04:45.000000 smart-rest-client-0.4.3/README.pt.rst
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)     5951 2021-05-01 17:55:38.000000 smart-rest-client-0.4.3/README.rst
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.148016 smart-rest-client-0.4.3/docs/
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.147730 smart-rest-client-0.4.3/docs/en/
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.153158 smart-rest-client-0.4.3/docs/en/_static/
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)      286 2020-07-23 15:28:04.000000 smart-rest-client-0.4.3/docs/en/_static/file.png
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.153929 smart-rest-client-0.4.3/docs/en/_static/img/
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     8777 2020-07-25 23:07:54.000000 smart-rest-client-0.4.3/docs/en/_static/img/glyphicons-halflings-white.png
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)    12799 2020-07-25 23:07:54.000000 smart-rest-client-0.4.3/docs/en/_static/img/glyphicons-halflings.png
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)       90 2020-07-23 15:28:04.000000 smart-rest-client-0.4.3/docs/en/_static/minus.png
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)       90 2020-07-23 15:28:04.000000 smart-rest-client-0.4.3/docs/en/_static/plus.png
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.148106 smart-rest-client-0.4.3/docs/pt-br/
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.155191 smart-rest-client-0.4.3/docs/pt-br/_static/
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)      286 2020-07-23 15:28:04.000000 smart-rest-client-0.4.3/docs/pt-br/_static/file.png
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.155887 smart-rest-client-0.4.3/docs/pt-br/_static/img/
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     8777 2020-07-25 23:07:54.000000 smart-rest-client-0.4.3/docs/pt-br/_static/img/glyphicons-halflings-white.png
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)    12799 2020-07-25 23:07:54.000000 smart-rest-client-0.4.3/docs/pt-br/_static/img/glyphicons-halflings.png
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)       90 2020-07-23 15:28:04.000000 smart-rest-client-0.4.3/docs/pt-br/_static/minus.png
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)       90 2020-07-23 15:28:04.000000 smart-rest-client-0.4.3/docs/pt-br/_static/plus.png
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)       61 2021-04-30 20:48:56.000000 smart-rest-client-0.4.3/requirements-ci.txt
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)      155 2020-07-25 23:36:06.000000 smart-rest-client-0.4.3/requirements-dev.txt
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)       38 2022-07-18 17:52:53.000000 smart-rest-client-0.4.3/requirements.txt
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)       38 2023-06-01 17:54:03.162037 smart-rest-client-0.4.3/setup.cfg
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)     2312 2021-04-30 20:50:34.000000 smart-rest-client-0.4.3/setup.py
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.160051 smart-rest-client-0.4.3/smart_rest_client/
+-rwxr-xr-x   0 rafaelhenter   (502) staff       (20)      147 2020-02-05 23:52:55.000000 smart-rest-client-0.4.3/smart_rest_client/__init__.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)    13378 2023-06-01 17:53:37.000000 smart-rest-client-0.4.3/smart_rest_client/base.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     3992 2021-07-15 19:25:15.000000 smart-rest-client-0.4.3/smart_rest_client/client.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     1656 2021-04-30 21:27:36.000000 smart-rest-client-0.4.3/smart_rest_client/exceptions.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     2266 2021-07-02 12:17:43.000000 smart-rest-client-0.4.3/smart_rest_client/factories.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     4222 2021-05-01 16:22:53.000000 smart-rest-client-0.4.3/smart_rest_client/settings.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     2223 2021-01-08 19:08:53.000000 smart-rest-client-0.4.3/smart_rest_client/status.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     2321 2022-07-18 17:53:56.000000 smart-rest-client-0.4.3/smart_rest_client/utils.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     1132 2021-04-30 19:06:01.000000 smart-rest-client-0.4.3/smart_rest_client/validators.py
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)       22 2023-06-01 17:54:02.000000 smart-rest-client-0.4.3/smart_rest_client/version.py
+drwxr-xr-x   0 rafaelhenter   (502) staff       (20)        0 2023-06-01 17:54:03.161284 smart-rest-client-0.4.3/smart_rest_client.egg-info/
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)     8316 2023-06-01 17:54:02.000000 smart-rest-client-0.4.3/smart_rest_client.egg-info/PKG-INFO
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)      971 2023-06-01 17:54:02.000000 smart-rest-client-0.4.3/smart_rest_client.egg-info/SOURCES.txt
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)        1 2023-06-01 17:54:02.000000 smart-rest-client-0.4.3/smart_rest_client.egg-info/dependency_links.txt
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)       38 2023-06-01 17:54:02.000000 smart-rest-client-0.4.3/smart_rest_client.egg-info/requires.txt
+-rw-r--r--   0 rafaelhenter   (502) staff       (20)       18 2023-06-01 17:54:02.000000 smart-rest-client-0.4.3/smart_rest_client.egg-info/top_level.txt
```

### Comparing `smart-rest-client-0.4.2/CHANGES.rst` & `smart-rest-client-0.4.3/CHANGES.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.4.3
+-----
+
+- Change encoder default in json to be 'str'
+
 0.4.2
 -----
 
 - Return empty when the value is Nan on json_converter
 
 0.4.1
 -----
```

### Comparing `smart-rest-client-0.4.2/PKG-INFO` & `smart-rest-client-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: smart-rest-client
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python wrapper to perform requests to Rest APIs using objects to request endpoints and their methods
 Home-page: https://github.com/rhenter/smart-rest-client
 Author: Rafael Henter
 Author-email: rafael@henter.com.br
 License: UNKNOWN
 Description: `Para visualizar o README em português <https://github.com/rhenter/smart-rest-client/blob/master/README.pt.rst>`_.
```

### Comparing `smart-rest-client-0.4.2/README.pt.rst` & `smart-rest-client-0.4.3/README.pt.rst`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/README.rst` & `smart-rest-client-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/docs/en/_static/img/glyphicons-halflings-white.png` & `smart-rest-client-0.4.3/docs/en/_static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/docs/en/_static/img/glyphicons-halflings.png` & `smart-rest-client-0.4.3/docs/en/_static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/docs/pt-br/_static/img/glyphicons-halflings-white.png` & `smart-rest-client-0.4.3/docs/pt-br/_static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/docs/pt-br/_static/img/glyphicons-halflings.png` & `smart-rest-client-0.4.3/docs/pt-br/_static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/setup.py` & `smart-rest-client-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/smart_rest_client/base.py` & `smart-rest-client-0.4.3/smart_rest_client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from urllib.parse import urljoin
 
 import requests
 from requests.exceptions import ConnectionError as RequestsConnectionError, ReadTimeout, Timeout
 
 from .exceptions import APIEndpointMissingArgument, APIUnreachableOrOffline
 from .factories import ResponseFactory
-from .utils import json_converter
 from .validators import validate_status_code
 
 
 class RequestsTransport:
     def __init__(self, headers: Any) -> None:
         self.session = requests.Session()
         self.session.headers.update(headers)
@@ -140,15 +139,15 @@
             files: Files to send in the body of the request.
             content_type: Request Content Type. E.g: 'application/json', 'form-data'
 
         Returns:
             dict: Data retrieved for specified endpoint.
         """
         if content_type == 'application/json' or not files:
-            data = json.dumps(data, default=json_converter)
+            data = json.dumps(data, default=str)
         response = self.make_request('POST', endpoint, data=data, files=files, content_type=content_type)
         return self._render_response(response, endpoint)
 
     def update(
             self,
             endpoint: str,
             data: dict = None,
@@ -166,15 +165,15 @@
                      or just a few attributes. Default is False
 
         Returns:
             dict: Data retrieved for specified endpoint.
         """
         method = 'PATCH' if partial else 'PUT'
         if content_type == 'application/json':
-            data = json.dumps(data, default=json_converter)
+            data = json.dumps(data, default=str)
 
         if files:
             response = self.make_request(method, endpoint, data=data, files=files, content_type=content_type)
             return self._render_response(response, endpoint)
 
         response = self.make_request(method, endpoint, data=data, content_type=content_type)
         return self._render_response(response, endpoint)
```

### Comparing `smart-rest-client-0.4.2/smart_rest_client/client.py` & `smart-rest-client-0.4.3/smart_rest_client/client.py`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/smart_rest_client/exceptions.py` & `smart-rest-client-0.4.3/smart_rest_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/smart_rest_client/factories.py` & `smart-rest-client-0.4.3/smart_rest_client/factories.py`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/smart_rest_client/settings.py` & `smart-rest-client-0.4.3/smart_rest_client/settings.py`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/smart_rest_client/status.py` & `smart-rest-client-0.4.3/smart_rest_client/status.py`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/smart_rest_client/utils.py` & `smart-rest-client-0.4.3/smart_rest_client/utils.py`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/smart_rest_client/validators.py` & `smart-rest-client-0.4.3/smart_rest_client/validators.py`

 * *Files identical despite different names*

### Comparing `smart-rest-client-0.4.2/smart_rest_client.egg-info/PKG-INFO` & `smart-rest-client-0.4.3/smart_rest_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: smart-rest-client
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python wrapper to perform requests to Rest APIs using objects to request endpoints and their methods
 Home-page: https://github.com/rhenter/smart-rest-client
 Author: Rafael Henter
 Author-email: rafael@henter.com.br
 License: UNKNOWN
 Description: `Para visualizar o README em português <https://github.com/rhenter/smart-rest-client/blob/master/README.pt.rst>`_.
```

### Comparing `smart-rest-client-0.4.2/smart_rest_client.egg-info/SOURCES.txt` & `smart-rest-client-0.4.3/smart_rest_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

