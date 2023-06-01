# Comparing `tmp/fastchargeapi_cli-1.0.3.tar.gz` & `tmp/fastchargeapi_cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchargeapi_cli-1.0.3.tar", max compression
+gzip compressed data, was "fastchargeapi_cli-1.0.4.tar", max compression
```

## Comparing `fastchargeapi_cli-1.0.3.tar` & `fastchargeapi_cli-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2023-03-17 09:53:33.031435 fastchargeapi_cli-1.0.3/fastchargeapi_cli/__generated__/__init__.py
--rw-r--r--   0        0        0    36816 2023-06-01 08:00:40.037727 fastchargeapi_cli-1.0.3/fastchargeapi_cli/__generated__/gql_operations.py
--rw-r--r--   0        0        0       22 2023-06-01 07:44:44.942823 fastchargeapi_cli-1.0.3/fastchargeapi_cli/__init__.py
--rw-r--r--   0        0        0     3299 2023-06-01 07:11:42.392468 fastchargeapi_cli-1.0.3/fastchargeapi_cli/account.py
--rw-r--r--   0        0        0     8063 2023-05-06 05:16:53.948507 fastchargeapi_cli-1.0.3/fastchargeapi_cli/auth_file.py
--rw-r--r--   0        0        0      884 2023-04-23 16:48:06.408480 fastchargeapi_cli-1.0.3/fastchargeapi_cli/config.py
--rw-r--r--   0        0        0      123 2023-04-23 16:48:08.170800 fastchargeapi_cli-1.0.3/fastchargeapi_cli/context_obj.py
--rw-r--r--   0        0        0     1064 2023-05-07 18:21:01.191960 fastchargeapi_cli-1.0.3/fastchargeapi_cli/exceptions.py
--rw-r--r--   0        0        0     1280 2023-05-07 17:06:26.549181 fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastapi_account.py
--rw-r--r--   0        0        0     1405 2023-05-07 17:06:26.575798 fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastapi_api.py
--rw-r--r--   0        0        0     5140 2023-05-07 18:28:23.129772 fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastapi_subscription.py
--rw-r--r--   0        0        0     4921 2023-05-07 17:06:31.983616 fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_account.py
--rw-r--r--   0        0        0     6932 2023-05-07 20:32:44.869011 fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_api.py
--rw-r--r--   0        0        0     6105 2023-05-30 03:27:23.172124 fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_app.py
--rw-r--r--   0        0        0     7193 2023-05-07 17:06:31.446962 fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_pricing.py
--rw-r--r--   0        0        0      967 2023-05-07 17:06:32.061592 fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_stripe.py
--rw-r--r--   0        0        0     2806 2023-05-07 19:30:33.999971 fastchargeapi_cli-1.0.3/fastchargeapi_cli/graphql_client.py
--rw-r--r--   0        0        0      789 2023-05-07 17:06:31.940160 fastchargeapi_cli-1.0.3/fastchargeapi_cli/groups.py
--rw-r--r--   0        0        0      811 2023-04-23 16:48:40.243041 fastchargeapi_cli-1.0.3/fastchargeapi_cli/http.py
--rw-r--r--   0        0        0     3637 2023-04-23 16:48:41.984143 fastchargeapi_cli-1.0.3/fastchargeapi_cli/local_server.py
--rw-r--r--   0        0        0     3865 2023-06-01 07:59:08.503077 fastchargeapi_cli-1.0.3/fastchargeapi_cli/login.py
--rw-r--r--   0        0        0      718 2023-05-07 17:06:31.932263 fastchargeapi_cli-1.0.3/fastchargeapi_cli/main.py
--rw-r--r--   0        0        0     6023 2023-05-28 22:41:24.242247 fastchargeapi_cli-1.0.3/fastchargeapi_cli/operations.graphql
--rw-r--r--   0        0        0     6594 2023-05-06 01:26:22.394837 fastchargeapi_cli-1.0.3/fastchargeapi_cli/remote_secret.py
--rw-r--r--   0        0        0     2574 2023-05-07 18:42:52.499981 fastchargeapi_cli-1.0.3/fastchargeapi_cli/token.py
--rw-r--r--   0        0        0     1503 2023-06-01 07:46:03.922199 fastchargeapi_cli-1.0.3/fastchargeapi_cli/version.py
--rw-r--r--   0        0        0     1448 2023-06-01 07:45:03.183161 fastchargeapi_cli-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 fastchargeapi_cli-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-17 09:53:33.031435 fastchargeapi_cli-1.0.4/fastchargeapi_cli/__generated__/__init__.py
+-rw-r--r--   0        0        0    36816 2023-06-01 08:04:00.159129 fastchargeapi_cli-1.0.4/fastchargeapi_cli/__generated__/gql_operations.py
+-rw-r--r--   0        0        0       22 2023-06-01 08:03:20.827205 fastchargeapi_cli-1.0.4/fastchargeapi_cli/__init__.py
+-rw-r--r--   0        0        0     3299 2023-06-01 07:11:42.392468 fastchargeapi_cli-1.0.4/fastchargeapi_cli/account.py
+-rw-r--r--   0        0        0     8063 2023-05-06 05:16:53.948507 fastchargeapi_cli-1.0.4/fastchargeapi_cli/auth_file.py
+-rw-r--r--   0        0        0      884 2023-04-23 16:48:06.408480 fastchargeapi_cli-1.0.4/fastchargeapi_cli/config.py
+-rw-r--r--   0        0        0      123 2023-04-23 16:48:08.170800 fastchargeapi_cli-1.0.4/fastchargeapi_cli/context_obj.py
+-rw-r--r--   0        0        0     1064 2023-05-07 18:21:01.191960 fastchargeapi_cli-1.0.4/fastchargeapi_cli/exceptions.py
+-rw-r--r--   0        0        0     1280 2023-05-07 17:06:26.549181 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_account.py
+-rw-r--r--   0        0        0     1405 2023-05-07 17:06:26.575798 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_api.py
+-rw-r--r--   0        0        0     5140 2023-05-07 18:28:23.129772 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_subscription.py
+-rw-r--r--   0        0        0     4921 2023-05-07 17:06:31.983616 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_account.py
+-rw-r--r--   0        0        0     6932 2023-05-07 20:32:44.869011 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_api.py
+-rw-r--r--   0        0        0     6105 2023-05-30 03:27:23.172124 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_app.py
+-rw-r--r--   0        0        0     7193 2023-05-07 17:06:31.446962 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_pricing.py
+-rw-r--r--   0        0        0      967 2023-05-07 17:06:32.061592 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_stripe.py
+-rw-r--r--   0        0        0     2806 2023-05-07 19:30:33.999971 fastchargeapi_cli-1.0.4/fastchargeapi_cli/graphql_client.py
+-rw-r--r--   0        0        0      789 2023-05-07 17:06:31.940160 fastchargeapi_cli-1.0.4/fastchargeapi_cli/groups.py
+-rw-r--r--   0        0        0      811 2023-04-23 16:48:40.243041 fastchargeapi_cli-1.0.4/fastchargeapi_cli/http.py
+-rw-r--r--   0        0        0     3637 2023-04-23 16:48:41.984143 fastchargeapi_cli-1.0.4/fastchargeapi_cli/local_server.py
+-rw-r--r--   0        0        0     3867 2023-06-01 08:02:52.106455 fastchargeapi_cli-1.0.4/fastchargeapi_cli/login.py
+-rw-r--r--   0        0        0      718 2023-05-07 17:06:31.932263 fastchargeapi_cli-1.0.4/fastchargeapi_cli/main.py
+-rw-r--r--   0        0        0     6023 2023-05-28 22:41:24.242247 fastchargeapi_cli-1.0.4/fastchargeapi_cli/operations.graphql
+-rw-r--r--   0        0        0     6594 2023-05-06 01:26:22.394837 fastchargeapi_cli-1.0.4/fastchargeapi_cli/remote_secret.py
+-rw-r--r--   0        0        0     2574 2023-05-07 18:42:52.499981 fastchargeapi_cli-1.0.4/fastchargeapi_cli/token.py
+-rw-r--r--   0        0        0     1503 2023-06-01 07:46:03.922199 fastchargeapi_cli-1.0.4/fastchargeapi_cli/version.py
+-rw-r--r--   0        0        0     1448 2023-06-01 08:03:18.495466 fastchargeapi_cli-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 fastchargeapi_cli-1.0.4/PKG-INFO
```

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/__generated__/gql_operations.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/__generated__/gql_operations.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/account.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/auth_file.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/auth_file.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/config.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/config.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/exceptions.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastapi_account.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastapi_api.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_api.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastapi_subscription.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_subscription.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_account.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_api.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_api.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_app.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_app.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_pricing.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_pricing.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/fastcharge_stripe.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_stripe.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/graphql_client.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/graphql_client.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/groups.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/groups.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/http.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/http.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/local_server.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/local_server.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/login.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 import webbrowser
 from typing import Optional
 from uuid import uuid4
 
 import click
-from blessed import Terminal
+from blessings import Terminal
 from click import echo
 
 from . import config
 from .auth_file import (
     delete_auth_file,
     list_auth_files,
     query_user_pk,
```

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/main.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/main.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/operations.graphql` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/operations.graphql`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/remote_secret.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/remote_secret.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/token.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/token.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/fastchargeapi_cli/version.py` & `fastchargeapi_cli-1.0.4/fastchargeapi_cli/version.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.3/pyproject.toml` & `fastchargeapi_cli-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchargeapi-cli"
-version = "1.0.3"
+version = "1.0.4"
 description = "Official CLI for managing apps and account on FastchargeAPI.com"
 authors = ["FastchargeAPI <fastchargeapi@gmail.com>"]
 license = "GNU v3.0"
 homepage = "https://fastchargeapi.com"
 repository = "https://github.com/FastchargeAPI/fastchargeapi-cli"
 packages = [{include = "fastchargeapi_cli"}]
 include = ["fastchargeapi_cli/__generated__/*"]
```

### Comparing `fastchargeapi_cli-1.0.3/PKG-INFO` & `fastchargeapi_cli-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchargeapi-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Official CLI for managing apps and account on FastchargeAPI.com
 Home-page: https://fastchargeapi.com
 License: GNU v3.0
 Author: FastchargeAPI
 Author-email: fastchargeapi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

