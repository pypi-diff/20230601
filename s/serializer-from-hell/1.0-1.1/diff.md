# Comparing `tmp/serializer-from-hell-1.0.tar.gz` & `tmp/serializer-from-hell-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer-from-hell-1.0.tar", last modified: Wed May 31 23:31:07 2023, max compression
+gzip compressed data, was "serializer-from-hell-1.1.tar", last modified: Thu Jun  1 00:01:27 2023, max compression
```

## Comparing `serializer-from-hell-1.0.tar` & `serializer-from-hell-1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-05-31 23:31:07.698565 serializer-from-hell-1.0/
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-05-31 23:31:07.698565 serializer-from-hell-1.0/Lab3/
--rw-rw-r--   0 egor      (1000) egor      (1000)      204 2023-05-31 23:24:11.000000 serializer-from-hell-1.0/Lab3/__init__.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-05-31 23:31:07.698565 serializer-from-hell-1.0/Lab3/constants/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2023-05-30 20:22:28.000000 serializer-from-hell-1.0/Lab3/constants/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     1113 2023-05-30 21:52:15.000000 serializer-from-hell-1.0/Lab3/constants/constants.py
--rw-rw-r--   0 egor      (1000) egor      (1000)      377 2023-05-30 20:43:36.000000 serializer-from-hell-1.0/Lab3/constants/formats.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-05-31 23:31:07.698565 serializer-from-hell-1.0/Lab3/funcs/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2023-05-30 20:32:43.000000 serializer-from-hell-1.0/Lab3/funcs/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     6868 2023-05-31 21:02:47.000000 serializer-from-hell-1.0/Lab3/funcs/funcs.py
--rw-rw-r--   0 egor      (1000) egor      (1000)      901 2023-05-31 23:22:50.000000 serializer-from-hell-1.0/Lab3/main.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-05-31 23:31:07.698565 serializer-from-hell-1.0/Lab3/package/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2023-05-30 18:06:25.000000 serializer-from-hell-1.0/Lab3/package/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     2633 2023-05-31 20:16:59.000000 serializer-from-hell-1.0/Lab3/package/basicjsonserializer.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     2778 2023-05-31 20:22:04.000000 serializer-from-hell-1.0/Lab3/package/basicxmlserializer.py
--rw-rw-r--   0 egor      (1000) egor      (1000)      189 2023-05-31 23:31:07.698565 serializer-from-hell-1.0/PKG-INFO
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-05-31 23:31:07.698565 serializer-from-hell-1.0/serializer_from_hell.egg-info/
--rw-rw-r--   0 egor      (1000) egor      (1000)      189 2023-05-31 23:31:07.000000 serializer-from-hell-1.0/serializer_from_hell.egg-info/PKG-INFO
--rw-rw-r--   0 egor      (1000) egor      (1000)      487 2023-05-31 23:31:07.000000 serializer-from-hell-1.0/serializer_from_hell.egg-info/SOURCES.txt
--rw-rw-r--   0 egor      (1000) egor      (1000)        1 2023-05-31 23:31:07.000000 serializer-from-hell-1.0/serializer_from_hell.egg-info/dependency_links.txt
--rw-rw-r--   0 egor      (1000) egor      (1000)        1 2023-05-31 23:31:07.000000 serializer-from-hell-1.0/serializer_from_hell.egg-info/not-zip-safe
--rw-rw-r--   0 egor      (1000) egor      (1000)       44 2023-05-31 23:31:07.000000 serializer-from-hell-1.0/serializer_from_hell.egg-info/top_level.txt
--rw-rw-r--   0 egor      (1000) egor      (1000)       38 2023-05-31 23:31:07.702566 serializer-from-hell-1.0/setup.cfg
--rw-rw-r--   0 egor      (1000) egor      (1000)      263 2023-05-31 23:28:01.000000 serializer-from-hell-1.0/setup.py
+drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-06-01 00:01:27.717231 serializer-from-hell-1.1/
+drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-06-01 00:01:27.717231 serializer-from-hell-1.1/Lab3/
+-rw-rw-r--   0 egor      (1000) egor      (1000)      204 2023-05-31 23:24:11.000000 serializer-from-hell-1.1/Lab3/__init__.py
+drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-06-01 00:01:27.717231 serializer-from-hell-1.1/Lab3/constants/
+-rw-rw-r--   0 egor      (1000) egor      (1000)        0 2023-05-30 20:22:28.000000 serializer-from-hell-1.1/Lab3/constants/__init__.py
+-rw-rw-r--   0 egor      (1000) egor      (1000)     1113 2023-05-30 21:52:15.000000 serializer-from-hell-1.1/Lab3/constants/constants.py
+-rw-rw-r--   0 egor      (1000) egor      (1000)      377 2023-05-30 20:43:36.000000 serializer-from-hell-1.1/Lab3/constants/formats.py
+drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-06-01 00:01:27.717231 serializer-from-hell-1.1/Lab3/funcs/
+-rw-rw-r--   0 egor      (1000) egor      (1000)        0 2023-05-30 20:32:43.000000 serializer-from-hell-1.1/Lab3/funcs/__init__.py
+-rw-rw-r--   0 egor      (1000) egor      (1000)     6873 2023-06-01 00:00:25.000000 serializer-from-hell-1.1/Lab3/funcs/funcs.py
+-rw-rw-r--   0 egor      (1000) egor      (1000)      901 2023-05-31 23:22:50.000000 serializer-from-hell-1.1/Lab3/main.py
+drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-06-01 00:01:27.717231 serializer-from-hell-1.1/Lab3/package/
+-rw-rw-r--   0 egor      (1000) egor      (1000)        0 2023-05-30 18:06:25.000000 serializer-from-hell-1.1/Lab3/package/__init__.py
+-rw-rw-r--   0 egor      (1000) egor      (1000)     2648 2023-06-01 00:00:25.000000 serializer-from-hell-1.1/Lab3/package/basicjsonserializer.py
+-rw-rw-r--   0 egor      (1000) egor      (1000)     2793 2023-06-01 00:00:25.000000 serializer-from-hell-1.1/Lab3/package/basicxmlserializer.py
+-rw-rw-r--   0 egor      (1000) egor      (1000)      189 2023-06-01 00:01:27.717231 serializer-from-hell-1.1/PKG-INFO
+drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2023-06-01 00:01:27.717231 serializer-from-hell-1.1/serializer_from_hell.egg-info/
+-rw-rw-r--   0 egor      (1000) egor      (1000)      189 2023-06-01 00:01:27.000000 serializer-from-hell-1.1/serializer_from_hell.egg-info/PKG-INFO
+-rw-rw-r--   0 egor      (1000) egor      (1000)      487 2023-06-01 00:01:27.000000 serializer-from-hell-1.1/serializer_from_hell.egg-info/SOURCES.txt
+-rw-rw-r--   0 egor      (1000) egor      (1000)        1 2023-06-01 00:01:27.000000 serializer-from-hell-1.1/serializer_from_hell.egg-info/dependency_links.txt
+-rw-rw-r--   0 egor      (1000) egor      (1000)        1 2023-05-31 23:31:07.000000 serializer-from-hell-1.1/serializer_from_hell.egg-info/not-zip-safe
+-rw-rw-r--   0 egor      (1000) egor      (1000)       44 2023-06-01 00:01:27.000000 serializer-from-hell-1.1/serializer_from_hell.egg-info/top_level.txt
+-rw-rw-r--   0 egor      (1000) egor      (1000)       38 2023-06-01 00:01:27.717231 serializer-from-hell-1.1/setup.cfg
+-rw-rw-r--   0 egor      (1000) egor      (1000)      263 2023-06-01 00:01:05.000000 serializer-from-hell-1.1/setup.py
```

### Comparing `serializer-from-hell-1.0/Lab3/constants/constants.py` & `serializer-from-hell-1.1/Lab3/constants/constants.py`

 * *Files identical despite different names*

### Comparing `serializer-from-hell-1.0/Lab3/funcs/funcs.py` & `serializer-from-hell-1.1/Lab3/funcs/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from types import FunctionType, MethodType, CodeType, ModuleType, \
     BuiltinMethodType, BuiltinFunctionType, CellType, GeneratorType
 from typing import Any, Collection, Iterable
 import re
-from constants.constants import IGNORED_FIELDS, IGNORED_FIELD_TYPES, TYPE_MAPPING
+from Lab3.constants.constants import IGNORED_FIELDS, IGNORED_FIELD_TYPES, TYPE_MAPPING
 
 
 def get_key(value, obj: dict) -> int:
     return [key for key in obj if obj[key] == value][0]
 
 
 def to_number(s: str) -> int | float | complex | None:
```

### Comparing `serializer-from-hell-1.0/Lab3/main.py` & `serializer-from-hell-1.1/Lab3/main.py`

 * *Files identical despite different names*

### Comparing `serializer-from-hell-1.0/Lab3/package/basicjsonserializer.py` & `serializer-from-hell-1.1/Lab3/package/basicjsonserializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from constants.formats import JSON, JSON_TYPE
-from constants.constants import BOOL_TYPES, PRIMITIVES, TYPE_MAPPING
-from funcs.funcs import get_key, to_number, get_items, type_from_str, create_object
+from Lab3.constants.formats import JSON, JSON_TYPE
+from Lab3.constants.constants import BOOL_TYPES, PRIMITIVES, TYPE_MAPPING
+from Lab3.funcs.funcs import get_key, to_number, get_items, type_from_str, create_object
 import re
 from typing import Iterator
 
 
 class JSONSerializer:
 
     def dumps(self, obj):
```

### Comparing `serializer-from-hell-1.0/Lab3/package/basicxmlserializer.py` & `serializer-from-hell-1.1/Lab3/package/basicxmlserializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from typing import Iterator
-from constants.constants import PRIMITIVES, TYPE_MAPPING
-from constants.formats import XML, XML_TYPE, XML_ITEM, XML_PRIMITIVE
-from funcs.funcs import get_key, get_items, type_from_str, create_object
+from Lab3.constants.constants import PRIMITIVES, TYPE_MAPPING
+from Lab3.constants.formats import XML, XML_TYPE, XML_ITEM, XML_PRIMITIVE
+from Lab3.funcs.funcs import get_key, get_items, type_from_str, create_object
 
 class XMLSerializer:
 
     def dumps(self, obj) -> str:
         if type(obj) in PRIMITIVES:
             obj_type = get_key(type(obj), TYPE_MAPPING)
             return f'<primitive type="{obj_type}">{obj}</primitive>'
```

