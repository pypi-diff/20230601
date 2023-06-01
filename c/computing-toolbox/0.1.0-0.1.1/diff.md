# Comparing `tmp/computing-toolbox-0.1.0.tar.gz` & `tmp/computing-toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.1.0.tar", last modified: Thu Jun  1 03:58:49 2023, max compression
+gzip compressed data, was "computing-toolbox-0.1.1.tar", last modified: Thu Jun  1 09:19:24 2023, max compression
```

## Comparing `computing-toolbox-0.1.0.tar` & `computing-toolbox-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.716709 computing-toolbox-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 03:58:49.716709 computing-toolbox-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:58:49.716709 computing-toolbox-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.712708 computing-toolbox-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.712708 computing-toolbox-0.1.0/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.712708 computing-toolbox-0.1.0/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.716709 computing-toolbox-0.1.0/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.712708 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:24.937215 computing-toolbox-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 09:19:24.937215 computing-toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:19:24.937215 computing-toolbox-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:24.933215 computing-toolbox-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:24.933215 computing-toolbox-0.1.1/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:24.937215 computing-toolbox-0.1.1/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:24.937215 computing-toolbox-0.1.1/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-01 09:19:14.000000 computing-toolbox-0.1.1/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:19:24.937215 computing-toolbox-0.1.1/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 09:19:24.000000 computing-toolbox-0.1.1/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 09:19:24.000000 computing-toolbox-0.1.1/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:19:24.000000 computing-toolbox-0.1.1/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-01 09:19:24.000000 computing-toolbox-0.1.1/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 09:19:24.000000 computing-toolbox-0.1.1/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.1.0/LICENSE` & `computing-toolbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/PKG-INFO` & `computing-toolbox-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.1.0/README.md` & `computing-toolbox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/pyproject.toml` & `computing-toolbox-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "computing-toolbox"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Pedro Mayorga", email="ppmayorga80@gmail.com" },
 ]
 description = "Computing Toolbox for daily computations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.1.1/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.1.1/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.1.1/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.1.1/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.1.1/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.1.1/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.1.1/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.1.1/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.1.0/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.1.1/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

