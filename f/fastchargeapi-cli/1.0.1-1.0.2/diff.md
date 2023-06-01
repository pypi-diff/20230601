# Comparing `tmp/fastchargeapi_cli-1.0.1.tar.gz` & `tmp/fastchargeapi_cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchargeapi_cli-1.0.1.tar", max compression
+gzip compressed data, was "fastchargeapi_cli-1.0.2.tar", max compression
```

## Comparing `fastchargeapi_cli-1.0.1.tar` & `fastchargeapi_cli-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2023-03-17 09:53:33.031435 fastchargeapi_cli-1.0.1/fastchargeapi_cli/__generated__/__init__.py
--rw-r--r--   0        0        0    36816 2023-06-01 07:14:08.995350 fastchargeapi_cli-1.0.1/fastchargeapi_cli/__generated__/gql_operations.py
--rw-r--r--   0        0        0     3299 2023-06-01 07:11:42.392468 fastchargeapi_cli-1.0.1/fastchargeapi_cli/account.py
--rw-r--r--   0        0        0     8063 2023-05-06 05:16:53.948507 fastchargeapi_cli-1.0.1/fastchargeapi_cli/auth_file.py
--rw-r--r--   0        0        0      884 2023-04-23 16:48:06.408480 fastchargeapi_cli-1.0.1/fastchargeapi_cli/config.py
--rw-r--r--   0        0        0      123 2023-04-23 16:48:08.170800 fastchargeapi_cli-1.0.1/fastchargeapi_cli/context_obj.py
--rw-r--r--   0        0        0     1064 2023-05-07 18:21:01.191960 fastchargeapi_cli-1.0.1/fastchargeapi_cli/exceptions.py
--rw-r--r--   0        0        0     1280 2023-05-07 17:06:26.549181 fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastapi_account.py
--rw-r--r--   0        0        0     1405 2023-05-07 17:06:26.575798 fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastapi_api.py
--rw-r--r--   0        0        0     5140 2023-05-07 18:28:23.129772 fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastapi_subscription.py
--rw-r--r--   0        0        0     4921 2023-05-07 17:06:31.983616 fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_account.py
--rw-r--r--   0        0        0     6932 2023-05-07 20:32:44.869011 fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_api.py
--rw-r--r--   0        0        0     6105 2023-05-30 03:27:23.172124 fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_app.py
--rw-r--r--   0        0        0     7193 2023-05-07 17:06:31.446962 fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_pricing.py
--rw-r--r--   0        0        0      967 2023-05-07 17:06:32.061592 fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_stripe.py
--rw-r--r--   0        0        0     2806 2023-05-07 19:30:33.999971 fastchargeapi_cli-1.0.1/fastchargeapi_cli/graphql_client.py
--rw-r--r--   0        0        0      789 2023-05-07 17:06:31.940160 fastchargeapi_cli-1.0.1/fastchargeapi_cli/groups.py
--rw-r--r--   0        0        0      811 2023-04-23 16:48:40.243041 fastchargeapi_cli-1.0.1/fastchargeapi_cli/http.py
--rw-r--r--   0        0        0     3637 2023-04-23 16:48:41.984143 fastchargeapi_cli-1.0.1/fastchargeapi_cli/local_server.py
--rw-r--r--   0        0        0     3729 2023-05-07 17:06:31.595872 fastchargeapi_cli-1.0.1/fastchargeapi_cli/login.py
--rw-r--r--   0        0        0      718 2023-05-07 17:06:31.932263 fastchargeapi_cli-1.0.1/fastchargeapi_cli/main.py
--rw-r--r--   0        0        0     6023 2023-05-28 22:41:24.242247 fastchargeapi_cli-1.0.1/fastchargeapi_cli/operations.graphql
--rw-r--r--   0        0        0     6594 2023-05-06 01:26:22.394837 fastchargeapi_cli-1.0.1/fastchargeapi_cli/remote_secret.py
--rw-r--r--   0        0        0     2574 2023-05-07 18:42:52.499981 fastchargeapi_cli-1.0.1/fastchargeapi_cli/token.py
--rw-r--r--   0        0        0     1666 2023-04-23 16:48:52.111227 fastchargeapi_cli-1.0.1/fastchargeapi_cli/version.py
--rw-r--r--   0        0        0     1295 2023-06-01 07:14:03.781964 fastchargeapi_cli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 fastchargeapi_cli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-17 09:53:33.031435 fastchargeapi_cli-1.0.2/fastchargeapi_cli/__generated__/__init__.py
+-rw-r--r--   0        0        0    36816 2023-06-01 07:16:17.995843 fastchargeapi_cli-1.0.2/fastchargeapi_cli/__generated__/gql_operations.py
+-rw-r--r--   0        0        0     3299 2023-06-01 07:11:42.392468 fastchargeapi_cli-1.0.2/fastchargeapi_cli/account.py
+-rw-r--r--   0        0        0     8063 2023-05-06 05:16:53.948507 fastchargeapi_cli-1.0.2/fastchargeapi_cli/auth_file.py
+-rw-r--r--   0        0        0      884 2023-04-23 16:48:06.408480 fastchargeapi_cli-1.0.2/fastchargeapi_cli/config.py
+-rw-r--r--   0        0        0      123 2023-04-23 16:48:08.170800 fastchargeapi_cli-1.0.2/fastchargeapi_cli/context_obj.py
+-rw-r--r--   0        0        0     1064 2023-05-07 18:21:01.191960 fastchargeapi_cli-1.0.2/fastchargeapi_cli/exceptions.py
+-rw-r--r--   0        0        0     1280 2023-05-07 17:06:26.549181 fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastapi_account.py
+-rw-r--r--   0        0        0     1405 2023-05-07 17:06:26.575798 fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastapi_api.py
+-rw-r--r--   0        0        0     5140 2023-05-07 18:28:23.129772 fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastapi_subscription.py
+-rw-r--r--   0        0        0     4921 2023-05-07 17:06:31.983616 fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_account.py
+-rw-r--r--   0        0        0     6932 2023-05-07 20:32:44.869011 fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_api.py
+-rw-r--r--   0        0        0     6105 2023-05-30 03:27:23.172124 fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_app.py
+-rw-r--r--   0        0        0     7193 2023-05-07 17:06:31.446962 fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_pricing.py
+-rw-r--r--   0        0        0      967 2023-05-07 17:06:32.061592 fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_stripe.py
+-rw-r--r--   0        0        0     2806 2023-05-07 19:30:33.999971 fastchargeapi_cli-1.0.2/fastchargeapi_cli/graphql_client.py
+-rw-r--r--   0        0        0      789 2023-05-07 17:06:31.940160 fastchargeapi_cli-1.0.2/fastchargeapi_cli/groups.py
+-rw-r--r--   0        0        0      811 2023-04-23 16:48:40.243041 fastchargeapi_cli-1.0.2/fastchargeapi_cli/http.py
+-rw-r--r--   0        0        0     3637 2023-04-23 16:48:41.984143 fastchargeapi_cli-1.0.2/fastchargeapi_cli/local_server.py
+-rw-r--r--   0        0        0     3729 2023-05-07 17:06:31.595872 fastchargeapi_cli-1.0.2/fastchargeapi_cli/login.py
+-rw-r--r--   0        0        0      718 2023-05-07 17:06:31.932263 fastchargeapi_cli-1.0.2/fastchargeapi_cli/main.py
+-rw-r--r--   0        0        0     6023 2023-05-28 22:41:24.242247 fastchargeapi_cli-1.0.2/fastchargeapi_cli/operations.graphql
+-rw-r--r--   0        0        0     6594 2023-05-06 01:26:22.394837 fastchargeapi_cli-1.0.2/fastchargeapi_cli/remote_secret.py
+-rw-r--r--   0        0        0     2574 2023-05-07 18:42:52.499981 fastchargeapi_cli-1.0.2/fastchargeapi_cli/token.py
+-rw-r--r--   0        0        0     1666 2023-04-23 16:48:52.111227 fastchargeapi_cli-1.0.2/fastchargeapi_cli/version.py
+-rw-r--r--   0        0        0     1316 2023-06-01 07:16:11.526043 fastchargeapi_cli-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 fastchargeapi_cli-1.0.2/PKG-INFO
```

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/__generated__/gql_operations.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/__generated__/gql_operations.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/account.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/auth_file.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/auth_file.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/config.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/config.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/exceptions.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastapi_account.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastapi_account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastapi_api.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastapi_api.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastapi_subscription.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastapi_subscription.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_account.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_api.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_api.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_app.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_app.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_pricing.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_pricing.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/fastcharge_stripe.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/fastcharge_stripe.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/graphql_client.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/graphql_client.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/groups.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/groups.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/http.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/http.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/local_server.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/local_server.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/login.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/login.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/main.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/main.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/operations.graphql` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/operations.graphql`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/remote_secret.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/remote_secret.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/token.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/token.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/fastchargeapi_cli/version.py` & `fastchargeapi_cli-1.0.2/fastchargeapi_cli/version.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.1/pyproject.toml` & `fastchargeapi_cli-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchargeapi-cli"
-version = "1.0.1"
+version = "1.0.2"
 description = "Official CLI for managing apps and account on FastchargeAPI.com"
 authors = ["FastchargeAPI <fastchargeapi@gmail.com>"]
 license = "GNU v3.0"
 homepage = "https://fastchargeapi.com"
 repository = "https://github.com/FastchargeAPI/fastchargeapi-cli"
 packages = [{include = "fastchargeapi_cli"}]
 include = ["fastchargeapi_cli/__generated__/*"]
@@ -19,14 +19,15 @@
 sgqlc = "^16.1"
 emoji = "^2.2.0"
 aws-requests-auth = "^0.4.3"
 flask-cors = "^3.0.10"
 python-jose = {extras = ["cryptography"], version = "^3.3.0"}
 tomli = "^2.0.1"
 pyjwt = {extras = ["crypto"], version = "^2.6.0"}
+pydantic = "^1.10.8"
 
 [tool.poetry.scripts]
 fastcharge = 'fastchargeapi_cli.main:fastcharge'
 fastapi = 'fastchargeapi_cli.main:fastapi'
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
```

### Comparing `fastchargeapi_cli-1.0.1/PKG-INFO` & `fastchargeapi_cli-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchargeapi-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: Official CLI for managing apps and account on FastchargeAPI.com
 Home-page: https://fastchargeapi.com
 License: GNU v3.0
 Author: FastchargeAPI
 Author-email: fastchargeapi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -16,12 +16,13 @@
 Requires-Dist: blessings (>=1.7,<2.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: emoji (>=2.2.0,<3.0.0)
 Requires-Dist: flask-cors (>=3.0.10,<4.0.0)
 Requires-Dist: gql[all] (>=3.4.0,<4.0.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyjwt[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/FastchargeAPI/fastchargeapi-cli
```

