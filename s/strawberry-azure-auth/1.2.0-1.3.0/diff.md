# Comparing `tmp/strawberry_azure_auth-1.2.0.tar.gz` & `tmp/strawberry_azure_auth-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_azure_auth-1.2.0.tar", max compression
+gzip compressed data, was "strawberry_azure_auth-1.3.0.tar", max compression
```

## Comparing `strawberry_azure_auth-1.2.0.tar` & `strawberry_azure_auth-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2023-06-01 16:07:40.921981 strawberry_azure_auth-1.2.0/LICENSE
--rw-r--r--   0        0        0     3418 2023-06-01 16:07:40.921981 strawberry_azure_auth-1.2.0/README.md
--rw-r--r--   0        0        0      955 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      167 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/__init__.py
--rw-r--r--   0        0        0      154 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/__init__.py
--rw-r--r--   0        0        0     1318 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/context.py
--rw-r--r--   0        0        0     1851 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/handlers.py
--rw-r--r--   0        0        0     8597 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/schema.py
--rw-r--r--   0        0        0        0 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/django/__init__.py
--rw-r--r--   0        0        0      920 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/django/context.py
--rw-r--r--   0        0        0    10706 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/extension.py
--rw-r--r--   0        0        0     5569 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/openid.py
--rw-r--r--   0        0        0     1164 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/permissions.py
--rw-r--r--   0        0        0      519 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/types.py
--rw-r--r--   0        0        0     1585 2023-06-01 16:07:40.925982 strawberry_azure_auth-1.2.0/strawberry_azure_auth/utils.py
--rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 strawberry_azure_auth-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3418 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/README.md
+-rw-r--r--   0        0        0      955 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/__init__.py
+-rw-r--r--   0        0        0     1318 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/context.py
+-rw-r--r--   0        0        0     3566 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/handlers.py
+-rw-r--r--   0        0        0     8597 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/schema.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/django/__init__.py
+-rw-r--r--   0        0        0      920 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/django/context.py
+-rw-r--r--   0        0        0    10706 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/extension.py
+-rw-r--r--   0        0        0     5569 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/openid.py
+-rw-r--r--   0        0        0     1164 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/permissions.py
+-rw-r--r--   0        0        0      519 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/types.py
+-rw-r--r--   0        0        0     1585 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/utils.py
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 strawberry_azure_auth-1.3.0/PKG-INFO
```

### Comparing `strawberry_azure_auth-1.2.0/LICENSE` & `strawberry_azure_auth-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/README.md` & `strawberry_azure_auth-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/pyproject.toml` & `strawberry_azure_auth-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "strawberry-azure-auth"
-version = "1.2.0"
+version = "1.3.0"
 description = "Azure AD authentication for Strawberry GraphQL"
 authors = ["skarre-r <skarre-r@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/skarre-r/strawberry-azure-auth"
 packages = [{include = "strawberry_azure_auth"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "^0.24.1"
 pyjwt = { version = "^2.7.0", extras = ["crypto"] }
-strawberry-graphql = { version = "^0.177.3", extras = ["channels"] }
+strawberry-graphql = { version = "~0.179.0", extras = ["channels"] }
 strawberry-graphql-django = "^0.9.4"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.270"
 mypy = "^1.3.0"
 black = "^23.3.0"
 pre-commit = "^3.3.1"
```

### Comparing `strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/context.py` & `strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/strawberry_azure_auth/channels/schema.py` & `strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/strawberry_azure_auth/django/context.py` & `strawberry_azure_auth-1.3.0/strawberry_azure_auth/django/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/strawberry_azure_auth/extension.py` & `strawberry_azure_auth-1.3.0/strawberry_azure_auth/extension.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/strawberry_azure_auth/openid.py` & `strawberry_azure_auth-1.3.0/strawberry_azure_auth/openid.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/strawberry_azure_auth/permissions.py` & `strawberry_azure_auth-1.3.0/strawberry_azure_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/strawberry_azure_auth/types.py` & `strawberry_azure_auth-1.3.0/strawberry_azure_auth/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/strawberry_azure_auth/utils.py` & `strawberry_azure_auth-1.3.0/strawberry_azure_auth/utils.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.2.0/PKG-INFO` & `strawberry_azure_auth-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strawberry-azure-auth
-Version: 1.2.0
+Version: 1.3.0
 Summary: Azure AD authentication for Strawberry GraphQL
 Home-page: https://github.com/skarre-r/strawberry-azure-auth
 License: MIT
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
 Requires-Dist: strawberry-graphql-django (>=0.9.4,<0.10.0)
-Requires-Dist: strawberry-graphql[channels] (>=0.177.3,<0.178.0)
+Requires-Dist: strawberry-graphql[channels] (>=0.179.0,<0.180.0)
 Project-URL: Repository, https://github.com/skarre-r/strawberry-azure-auth
 Description-Content-Type: text/markdown
 
 # strawberry-azure-auth
 
 Azure AD authentication for [Strawberry GraphQL](https://github.com/strawberry-graphql/strawberry),
 inspired by [fastapi-azure-auth](https://github.com/Intility/fastapi-azure-auth).
```

