# Comparing `tmp/rhubarb_py-1.8.1.tar.gz` & `tmp/rhubarb_py-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhubarb_py-1.8.1.tar", max compression
+gzip compressed data, was "rhubarb_py-1.8.3.tar", max compression
```

## Comparing `rhubarb_py-1.8.1.tar` & `rhubarb_py-1.8.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1079 2023-06-01 14:43:36.441851 rhubarb_py-1.8.1/LICENSE
--rw-r--r--   0        0        0     7269 2023-06-01 14:43:36.441851 rhubarb_py-1.8.1/README.md
--rw-r--r--   0        0        0     3651 2023-06-01 17:52:40.284156 rhubarb_py-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      570 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/__init__.py
--rw-r--r--   0        0        0    16069 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/_core.py
--rw-r--r--   0        0        0     3131 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/backends/base.py
--rw-r--r--   0        0        0       40 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/backends/exceptions.py
--rw-r--r--   0        0        0     7555 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/backends/kafka.py
--rw-r--r--   0        0        0     2483 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/backends/memory.py
--rw-r--r--   0        0        0     3094 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/backends/postgres.py
--rw-r--r--   0        0        0     4360 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/backends/rabbitmq.py
--rw-r--r--   0        0        0    13779 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/backends/redis.py
--rw-r--r--   0        0        0      210 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/event.py
--rw-r--r--   0        0        0        0 2023-06-01 14:43:36.445851 rhubarb_py-1.8.1/rhubarb/py.typed
--rw-r--r--   0        0        0     8517 1970-01-01 00:00:00.000000 rhubarb_py-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-01 18:37:38.783184 rhubarb_py-1.8.3/LICENSE
+-rw-r--r--   0        0        0     7269 2023-06-01 18:37:38.783184 rhubarb_py-1.8.3/README.md
+-rw-r--r--   0        0        0     3651 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0      570 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/__init__.py
+-rw-r--r--   0        0        0    16069 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/_core.py
+-rw-r--r--   0        0        0     3131 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/base.py
+-rw-r--r--   0        0        0       40 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/exceptions.py
+-rw-r--r--   0        0        0     7555 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/kafka.py
+-rw-r--r--   0        0        0     2483 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/memory.py
+-rw-r--r--   0        0        0     3094 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/postgres.py
+-rw-r--r--   0        0        0     4360 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/rabbitmq.py
+-rw-r--r--   0        0        0    13779 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/backends/redis.py
+-rw-r--r--   0        0        0      210 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/event.py
+-rw-r--r--   0        0        0        0 2023-06-01 18:37:38.787184 rhubarb_py-1.8.3/rhubarb/py.typed
+-rw-r--r--   0        0        0     8517 1970-01-01 00:00:00.000000 rhubarb_py-1.8.3/PKG-INFO
```

### Comparing `rhubarb_py-1.8.1/LICENSE` & `rhubarb_py-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/README.md` & `rhubarb_py-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/pyproject.toml` & `rhubarb_py-1.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rhubarb-py"
 packages = [{ include = "rhubarb" }]
-version = "1.8.1"
+version = "1.8.3"
 description = "Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API"
 readme = "README.md"
 authors = ["mopeyjellyfish <dev@davidhall.tech>"]
 license = "MIT"
 repository = "https://github.com/mopeyjellyfish/rhubarb"
 homepage = "https://github.com/mopeyjellyfish/rhubarb"
```

### Comparing `rhubarb_py-1.8.1/rhubarb/__init__.py` & `rhubarb_py-1.8.3/rhubarb/__init__.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/rhubarb/_core.py` & `rhubarb_py-1.8.3/rhubarb/_core.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/rhubarb/backends/base.py` & `rhubarb_py-1.8.3/rhubarb/backends/base.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/rhubarb/backends/kafka.py` & `rhubarb_py-1.8.3/rhubarb/backends/kafka.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/rhubarb/backends/memory.py` & `rhubarb_py-1.8.3/rhubarb/backends/memory.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/rhubarb/backends/postgres.py` & `rhubarb_py-1.8.3/rhubarb/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/rhubarb/backends/rabbitmq.py` & `rhubarb_py-1.8.3/rhubarb/backends/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/rhubarb/backends/redis.py` & `rhubarb_py-1.8.3/rhubarb/backends/redis.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.1/PKG-INFO` & `rhubarb_py-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhubarb-py
-Version: 1.8.1
+Version: 1.8.3
 Summary: Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API
 Home-page: https://github.com/mopeyjellyfish/rhubarb
 License: MIT
 Author: mopeyjellyfish
 Author-email: dev@davidhall.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

