# Comparing `tmp/dapr-ext-fastapi-dev-1.9.0rc1.dev1601.tar.gz` & `tmp/dapr-ext-fastapi-dev-1.9.0rc1.dev1607.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-fastapi-dev-1.9.0rc1.dev1601.tar", last modified: Wed May 31 15:44:24 2023, max compression
+gzip compressed data, was "dist/dapr-ext-fastapi-dev-1.9.0rc1.dev1607.tar", last modified: Wed May 31 22:52:20 2023, max compression
```

## Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601.tar` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-31 15:43:49.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-31 15:43:49.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-31 15:43:49.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-31 15:43:49.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-31 15:43:49.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 15:43:49.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr_ext_fastapi_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr_ext_fastapi_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr_ext_fastapi_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr_ext_fastapi_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr_ext_fastapi_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr_ext_fastapi_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-31 15:44:24.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-31 15:43:49.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-31 22:51:50.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-31 22:51:50.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-31 22:51:50.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-31 22:51:50.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-31 22:51:50.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 22:51:50.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr_ext_fastapi_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr_ext_fastapi_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr_ext_fastapi_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr_ext_fastapi_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr_ext_fastapi_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr_ext_fastapi_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-31 22:52:20.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-31 22:51:50.000000 dapr-ext-fastapi-dev-1.9.0rc1.dev1607/setup.py
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/LICENSE` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/PKG-INFO` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-fastapi-dev
-Version: 1.9.0rc1.dev1601
+Version: 1.9.0rc1.dev1607
 Summary: The developmental release for Dapr FastAPI extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/__init__.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/actor.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/actor.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/app.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr/ext/fastapi/version.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr/ext/fastapi/version.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/dapr_ext_fastapi_dev.egg-info/PKG-INFO` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/dapr_ext_fastapi_dev.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-fastapi-dev
-Version: 1.9.0rc1.dev1601
+Version: 1.9.0rc1.dev1607
 Summary: The developmental release for Dapr FastAPI extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/setup.cfg` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-dev-1.9.0rc1.dev1601/setup.py` & `dapr-ext-fastapi-dev-1.9.0rc1.dev1607/setup.py`

 * *Files identical despite different names*

