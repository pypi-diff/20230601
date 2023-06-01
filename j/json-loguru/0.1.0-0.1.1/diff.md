# Comparing `tmp/json_loguru-0.1.0.tar.gz` & `tmp/json_loguru-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_loguru-0.1.0.tar", max compression
+gzip compressed data, was "json_loguru-0.1.1.tar", max compression
```

## Comparing `json_loguru-0.1.0.tar` & `json_loguru-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-01 02:53:56.772930 json_loguru-0.1.0/README.md
--rw-r--r--   0        0        0     1482 2023-06-01 03:19:07.679229 json_loguru-0.1.0/loguru_json/__init__.py
--rw-r--r--   0        0        0     5798 2023-06-01 03:21:15.248846 json_loguru-0.1.0/loguru_json/format.py
--rw-r--r--   0        0        0     1486 2023-06-01 02:54:59.734267 json_loguru-0.1.0/loguru_json/json_encoder/__init__.py
--rw-r--r--   0        0        0     2221 2023-06-01 03:21:24.612669 json_loguru-0.1.0/loguru_json/monkey.py
--rw-r--r--   0        0        0      642 2023-06-01 03:20:14.441990 json_loguru-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 json_loguru-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-01 02:53:56.772930 json_loguru-0.1.1/README.md
+-rw-r--r--   0        0        0     1504 2023-06-01 03:44:21.605611 json_loguru-0.1.1/loguru_json/__init__.py
+-rw-r--r--   0        0        0     5798 2023-06-01 03:21:15.248846 json_loguru-0.1.1/loguru_json/format.py
+-rw-r--r--   0        0        0     1486 2023-06-01 02:54:59.734267 json_loguru-0.1.1/loguru_json/json_encoder/__init__.py
+-rw-r--r--   0        0        0     2221 2023-06-01 03:21:24.612669 json_loguru-0.1.1/loguru_json/monkey.py
+-rw-r--r--   0        0        0      642 2023-06-01 03:44:38.350229 json_loguru-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 json_loguru-0.1.1/PKG-INFO
```

### Comparing `json_loguru-0.1.0/loguru_json/__init__.py` & `json_loguru-0.1.1/loguru_json/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 
 from loguru import logger, _defaults
 
+from . import monkey
 from .format import escape_format, escape_colorized, JSONFormatterBuilder
 
 logger.remove()
 
 
 def _lower_level(level):
     return f"\"{level.name.lower()}\""
```

### Comparing `json_loguru-0.1.0/loguru_json/format.py` & `json_loguru-0.1.1/loguru_json/format.py`

 * *Files identical despite different names*

### Comparing `json_loguru-0.1.0/loguru_json/json_encoder/__init__.py` & `json_loguru-0.1.1/loguru_json/json_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `json_loguru-0.1.0/loguru_json/monkey.py` & `json_loguru-0.1.1/loguru_json/monkey.py`

 * *Files identical despite different names*

### Comparing `json_loguru-0.1.0/pyproject.toml` & `json_loguru-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json-loguru"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["jeff <jeff.jiang.cd.cn@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "loguru_json" }]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `json_loguru-0.1.0/PKG-INFO` & `json_loguru-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-loguru
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: jeff
 Author-email: jeff.jiang.cd.cn@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

