# Comparing `tmp/context_python-0.2.0.tar.gz` & `tmp/context_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "context_python-0.2.0.tar", max compression
+gzip compressed data, was "context_python-0.2.1.tar", max compression
```

## Comparing `context_python-0.2.0.tar` & `context_python-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2023-06-01 15:29:28.188846 context_python-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2748 2023-06-01 15:52:50.567602 context_python-0.2.0/README.md
--rw-r--r--   0        0        0       43 2023-06-01 14:40:09.995595 context_python-0.2.0/getcontext/__init__.py
--rw-r--r--   0        0        0      709 2023-06-01 14:36:11.780194 context_python-0.2.0/getcontext/generated/__init__.py
--rw-r--r--   0        0        0     3290 2023-06-01 14:36:11.780203 context_python-0.2.0/getcontext/generated/_client.py
--rw-r--r--   0        0        0     2643 2023-06-01 14:36:11.780222 context_python-0.2.0/getcontext/generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780394 context_python-0.2.0/getcontext/generated/_patch.py
--rw-r--r--   0        0        0    78836 2023-06-01 14:36:11.780239 context_python-0.2.0/getcontext/generated/_serialization.py
--rw-r--r--   0        0        0      709 2023-06-01 14:36:11.780251 context_python-0.2.0/getcontext/generated/aio/__init__.py
--rw-r--r--   0        0        0     3426 2023-06-01 14:36:11.780275 context_python-0.2.0/getcontext/generated/aio/_client.py
--rw-r--r--   0        0        0     2685 2023-06-01 14:36:11.780268 context_python-0.2.0/getcontext/generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780179 context_python-0.2.0/getcontext/generated/aio/_patch.py
--rw-r--r--   0        0        0      665 2023-06-01 14:36:11.780283 context_python-0.2.0/getcontext/generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     6598 2023-06-01 14:36:11.780301 context_python-0.2.0/getcontext/generated/aio/operations/_operations.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780424 context_python-0.2.0/getcontext/generated/aio/operations/_patch.py
--rw-r--r--   0        0        0      973 2023-06-01 14:36:11.780337 context_python-0.2.0/getcontext/generated/models/__init__.py
--rw-r--r--   0        0        0      794 2023-06-01 14:36:11.780328 context_python-0.2.0/getcontext/generated/models/_enums.py
--rw-r--r--   0        0        0     4130 2023-06-01 14:36:11.780320 context_python-0.2.0/getcontext/generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780310 context_python-0.2.0/getcontext/generated/models/_patch.py
--rw-r--r--   0        0        0      665 2023-06-01 14:36:11.780259 context_python-0.2.0/getcontext/generated/operations/__init__.py
--rw-r--r--   0        0        0     7263 2023-06-01 14:36:11.780290 context_python-0.2.0/getcontext/generated/operations/_operations.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780357 context_python-0.2.0/getcontext/generated/operations/_patch.py
--rw-r--r--   0        0        0       26 2023-06-01 14:36:10.592708 context_python-0.2.0/getcontext/generated/py.typed
--rw-r--r--   0        0        0      449 2023-06-01 15:50:20.326267 context_python-0.2.0/getcontext/token.py
--rw-r--r--   0        0        0      481 2023-06-01 15:58:45.482788 context_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 context_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-01 15:29:28.188846 context_python-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     2899 2023-06-01 16:09:16.093724 context_python-0.2.1/README.md
+-rw-r--r--   0        0        0       43 2023-06-01 14:40:09.995595 context_python-0.2.1/getcontext/__init__.py
+-rw-r--r--   0        0        0      709 2023-06-01 14:36:11.780194 context_python-0.2.1/getcontext/generated/__init__.py
+-rw-r--r--   0        0        0     3290 2023-06-01 14:36:11.780203 context_python-0.2.1/getcontext/generated/_client.py
+-rw-r--r--   0        0        0     2643 2023-06-01 14:36:11.780222 context_python-0.2.1/getcontext/generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780394 context_python-0.2.1/getcontext/generated/_patch.py
+-rw-r--r--   0        0        0    78836 2023-06-01 14:36:11.780239 context_python-0.2.1/getcontext/generated/_serialization.py
+-rw-r--r--   0        0        0      709 2023-06-01 14:36:11.780251 context_python-0.2.1/getcontext/generated/aio/__init__.py
+-rw-r--r--   0        0        0     3426 2023-06-01 14:36:11.780275 context_python-0.2.1/getcontext/generated/aio/_client.py
+-rw-r--r--   0        0        0     2685 2023-06-01 14:36:11.780268 context_python-0.2.1/getcontext/generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780179 context_python-0.2.1/getcontext/generated/aio/_patch.py
+-rw-r--r--   0        0        0      665 2023-06-01 14:36:11.780283 context_python-0.2.1/getcontext/generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0     6598 2023-06-01 14:36:11.780301 context_python-0.2.1/getcontext/generated/aio/operations/_operations.py
+-rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780424 context_python-0.2.1/getcontext/generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0      973 2023-06-01 14:36:11.780337 context_python-0.2.1/getcontext/generated/models/__init__.py
+-rw-r--r--   0        0        0      794 2023-06-01 14:36:11.780328 context_python-0.2.1/getcontext/generated/models/_enums.py
+-rw-r--r--   0        0        0     4130 2023-06-01 14:36:11.780320 context_python-0.2.1/getcontext/generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780310 context_python-0.2.1/getcontext/generated/models/_patch.py
+-rw-r--r--   0        0        0      665 2023-06-01 14:36:11.780259 context_python-0.2.1/getcontext/generated/operations/__init__.py
+-rw-r--r--   0        0        0     7263 2023-06-01 14:36:11.780290 context_python-0.2.1/getcontext/generated/operations/_operations.py
+-rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780357 context_python-0.2.1/getcontext/generated/operations/_patch.py
+-rw-r--r--   0        0        0       26 2023-06-01 14:36:10.592708 context_python-0.2.1/getcontext/generated/py.typed
+-rw-r--r--   0        0        0      449 2023-06-01 15:50:20.326267 context_python-0.2.1/getcontext/token.py
+-rw-r--r--   0        0        0      481 2023-06-01 16:11:17.537642 context_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 context_python-0.2.1/PKG-INFO
```

### Comparing `context_python-0.2.0/LICENSE.md` & `context_python-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/README.md` & `context_python-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Context Python Library
 
+[![PyPI version](https://badge.fury.io/py/context-python.svg)](https://badge.fury.io/py/context-python)
+
 The Context Python library provides a convenient way to interface with the Context APIs. We include pre-defined classes and operations to interact with API resources.
 
 ## Installation
 
+```
+pip install --upgrade context-python
+```
+
 ## Usage
 
 The library needs to be configured with your Context API key, which is available in the [Context Settings Dashboard](https://go.getcontext.ai/settings).
 
 ### Synchronous Example
 
 ```python
```

### Comparing `context_python-0.2.0/getcontext/generated/__init__.py` & `context_python-0.2.1/getcontext/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/_client.py` & `context_python-0.2.1/getcontext/generated/_client.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/_configuration.py` & `context_python-0.2.1/getcontext/generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/_patch.py` & `context_python-0.2.1/getcontext/generated/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/_serialization.py` & `context_python-0.2.1/getcontext/generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/aio/__init__.py` & `context_python-0.2.1/getcontext/generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/aio/_client.py` & `context_python-0.2.1/getcontext/generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/aio/_configuration.py` & `context_python-0.2.1/getcontext/generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/aio/_patch.py` & `context_python-0.2.1/getcontext/generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/aio/operations/__init__.py` & `context_python-0.2.1/getcontext/generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/aio/operations/_operations.py` & `context_python-0.2.1/getcontext/generated/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/aio/operations/_patch.py` & `context_python-0.2.1/getcontext/generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/models/__init__.py` & `context_python-0.2.1/getcontext/generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/models/_enums.py` & `context_python-0.2.1/getcontext/generated/models/_enums.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/models/_models.py` & `context_python-0.2.1/getcontext/generated/models/_models.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/models/_patch.py` & `context_python-0.2.1/getcontext/generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/operations/__init__.py` & `context_python-0.2.1/getcontext/generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/operations/_operations.py` & `context_python-0.2.1/getcontext/generated/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/getcontext/generated/operations/_patch.py` & `context_python-0.2.1/getcontext/generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.0/PKG-INFO` & `context_python-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for the Context API
 License: LICENSE.md
 Keywords: context,api,sdk
 Author: Alex Gamble
 Author-email: alex@woolly.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -15,18 +15,24 @@
 Requires-Dist: azure-core (>=1.26.4,<2.0.0)
 Requires-Dist: azure-mgmt-core (>=1.4.0,<2.0.0)
 Requires-Dist: msrest (>=0.7.1,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Context Python Library
 
+[![PyPI version](https://badge.fury.io/py/context-python.svg)](https://badge.fury.io/py/context-python)
+
 The Context Python library provides a convenient way to interface with the Context APIs. We include pre-defined classes and operations to interact with API resources.
 
 ## Installation
 
+```
+pip install --upgrade context-python
+```
+
 ## Usage
 
 The library needs to be configured with your Context API key, which is available in the [Context Settings Dashboard](https://go.getcontext.ai/settings).
 
 ### Synchronous Example
 
 ```python
```

