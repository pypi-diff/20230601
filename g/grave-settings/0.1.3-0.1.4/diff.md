# Comparing `tmp/grave-settings-0.1.3.tar.gz` & `tmp/grave-settings-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grave-settings-0.1.3.tar", last modified: Tue May  9 22:28:15 2023, max compression
+gzip compressed data, was "grave-settings-0.1.4.tar", last modified: Thu Jun  1 00:06:23 2023, max compression
```

## Comparing `grave-settings-0.1.3.tar` & `grave-settings-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.385882 grave-settings-0.1.3/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1071 2023-02-15 04:33:38.000000 grave-settings-0.1.3/LICENSE
--rw-r--r--   0 ryan      (1000) ryan      (1000)     5580 2023-05-09 22:28:15.385882 grave-settings-0.1.3/PKG-INFO
--rw-r--r--   0 ryan      (1000) ryan      (1000)     5122 2023-02-15 04:33:38.000000 grave-settings-0.1.3/README.md
--rw-r--r--   0 ryan      (1000) ryan      (1000)      690 2023-05-09 22:28:15.385882 grave-settings-0.1.3/setup.cfg
--rw-r--r--   0 ryan      (1000) ryan      (1000)       67 2023-02-15 04:33:38.000000 grave-settings-0.1.3/setup.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.382548 grave-settings-0.1.3/src/
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.382548 grave-settings-0.1.3/src/grave_settings/
--rw-r--r--   0 ryan      (1000) ryan      (1000)       18 2023-05-09 22:25:55.000000 grave-settings-0.1.3/src/grave_settings/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     5229 2023-05-02 00:14:49.000000 grave-settings-0.1.3/src/grave_settings/abstract.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     6220 2023-05-02 00:57:12.000000 grave-settings-0.1.3/src/grave_settings/base.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)    10636 2023-05-08 21:21:57.000000 grave-settings-0.1.3/src/grave_settings/config_file.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     3715 2023-05-01 23:21:15.000000 grave-settings-0.1.3/src/grave_settings/conversion_manager.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)    13209 2023-05-02 00:14:49.000000 grave-settings-0.1.3/src/grave_settings/default_handlers.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)    24288 2023-05-01 23:21:15.000000 grave-settings-0.1.3/src/grave_settings/formatter.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     6850 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatter_settings.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.385882 grave-settings-0.1.3/src/grave_settings/formatters/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatters/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1328 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatters/bson.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)      668 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatters/json.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1081 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatters/toml.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)      977 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/framestack_context.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     7918 2023-05-02 00:22:48.000000 grave-settings-0.1.3/src/grave_settings/handlers.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1548 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/helper_objects.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)    13217 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/semantics.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     3099 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/utilities.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     3387 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/validation.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.385882 grave-settings-0.1.3/src/grave_settings.egg-info/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     5580 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/PKG-INFO
--rw-r--r--   0 ryan      (1000) ryan      (1000)      883 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/SOURCES.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)        1 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/dependency_links.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)       41 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/requires.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)       15 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/top_level.txt
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 00:06:23.760119 grave-settings-0.1.4/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1071 2023-02-15 04:33:38.000000 grave-settings-0.1.4/LICENSE
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     5716 2023-06-01 00:06:23.760119 grave-settings-0.1.4/PKG-INFO
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     5258 2023-06-01 00:02:00.000000 grave-settings-0.1.4/README.md
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      690 2023-06-01 00:06:23.760119 grave-settings-0.1.4/setup.cfg
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       67 2023-02-15 04:33:38.000000 grave-settings-0.1.4/setup.py
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 00:06:23.756785 grave-settings-0.1.4/src/
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 00:06:23.760119 grave-settings-0.1.4/src/grave_settings/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       18 2023-06-01 00:02:28.000000 grave-settings-0.1.4/src/grave_settings/__init__.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     5173 2023-05-31 23:51:06.000000 grave-settings-0.1.4/src/grave_settings/abstract.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     6220 2023-05-02 00:57:12.000000 grave-settings-0.1.4/src/grave_settings/base.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    10636 2023-05-08 21:21:57.000000 grave-settings-0.1.4/src/grave_settings/config_file.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     3715 2023-05-01 23:21:15.000000 grave-settings-0.1.4/src/grave_settings/conversion_manager.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    13290 2023-05-31 23:54:37.000000 grave-settings-0.1.4/src/grave_settings/default_handlers.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    24288 2023-05-01 23:21:15.000000 grave-settings-0.1.4/src/grave_settings/formatter.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     6850 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/formatter_settings.py
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 00:06:23.760119 grave-settings-0.1.4/src/grave_settings/formatters/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/formatters/__init__.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1328 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/formatters/bson.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      668 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/formatters/json.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1081 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/formatters/toml.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      977 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/framestack_context.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     7918 2023-05-02 00:22:48.000000 grave-settings-0.1.4/src/grave_settings/handlers.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1548 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/helper_objects.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    13217 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/semantics.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     3099 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/utilities.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     3387 2023-02-15 04:33:38.000000 grave-settings-0.1.4/src/grave_settings/validation.py
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 00:06:23.760119 grave-settings-0.1.4/src/grave_settings.egg-info/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     5716 2023-06-01 00:06:23.000000 grave-settings-0.1.4/src/grave_settings.egg-info/PKG-INFO
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      883 2023-06-01 00:06:23.000000 grave-settings-0.1.4/src/grave_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        1 2023-06-01 00:06:23.000000 grave-settings-0.1.4/src/grave_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       41 2023-06-01 00:06:23.000000 grave-settings-0.1.4/src/grave_settings.egg-info/requires.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       15 2023-06-01 00:06:23.000000 grave-settings-0.1.4/src/grave_settings.egg-info/top_level.txt
```

### Comparing `grave-settings-0.1.3/LICENSE` & `grave-settings-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/PKG-INFO` & `grave-settings-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grave-settings
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for automatic serialization of python object hierarchies to storage
 Home-page: https://github.com/ILikesCaviar/GraveSettings
 Author: Ryan McConnell
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
@@ -112,19 +112,21 @@
 This will output:
 
 ```toml
 __class__ = "__main__.MyObject"
 integer = 1
 string = "b"
 
-[color]
-__class__ = "__main__.Color"
-b = 255
-g = 255
-r = 255
+[function]
+__class__ = "types.FunctionType"
+state = "builtins.print"
+
+[type_object]
+__class__ = "builtins.type"
+state = "builtins.int"
 
 [[dates]]
 __class__ = "datetime.date"
 state = [
     2022,
     1,
     1,
@@ -133,14 +135,20 @@
 [[dates]]
 __class__ = "datetime.date"
 state = [
     2023,
     2,
     2,
 ]
+
+[color]
+__class__ = "__main__.Color"
+r = 255
+g = 255
+b = 255
 ```
 
 Now if we take this string and deserialize it with the same (or equivalent) formatter:
 
 ```python
 from grave_settings.formatters.toml import TomlFormatter
 formatter = TomlFormatter()
```

### Comparing `grave-settings-0.1.3/README.md` & `grave-settings-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -99,19 +99,21 @@
 This will output:
 
 ```toml
 __class__ = "__main__.MyObject"
 integer = 1
 string = "b"
 
-[color]
-__class__ = "__main__.Color"
-b = 255
-g = 255
-r = 255
+[function]
+__class__ = "types.FunctionType"
+state = "builtins.print"
+
+[type_object]
+__class__ = "builtins.type"
+state = "builtins.int"
 
 [[dates]]
 __class__ = "datetime.date"
 state = [
     2022,
     1,
     1,
@@ -120,14 +122,20 @@
 [[dates]]
 __class__ = "datetime.date"
 state = [
     2023,
     2,
     2,
 ]
+
+[color]
+__class__ = "__main__.Color"
+r = 255
+g = 255
+b = 255
 ```
 
 Now if we take this string and deserialize it with the same (or equivalent) formatter:
 
 ```python
 from grave_settings.formatters.toml import TomlFormatter
 formatter = TomlFormatter()
```

### Comparing `grave-settings-0.1.3/setup.cfg` & `grave-settings-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/abstract.py` & `grave-settings-0.1.4/src/grave_settings/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         This method is typically called on type objects, so it should remain a class method in sub-classes. This is where
         you can put a reference to :py:class:`~grave_settings.semantics.NotifyFinalizedMethodName` to get a callback
         """
         # context.register_frame_semantic(NotifyFinalizedMethodName('finalize'))
         pass
 
     def to_dict(self, context: FormatterContext, **kwargs) -> dict:
-        zgen = ((i, getattr(self, i)) for i in dir(self))
-        return dict(i for i in zgen if not (callable(i[1]) or i[0].startswith('__')))
+        #zgen = ((i, getattr(self, i)) for i in dir(self))
+        return self.__dict__
 
     def from_dict(self, state_obj: dict, context: FormatterContext, **kwargs):
         for k, v in state_obj.items():
             setattr(self, k, v)
 
     def finalize(self, frame: FormatterContext) -> None:  # This is pretty inefficient. Override it
         for key in dir(self):
```

### Comparing `grave-settings-0.1.3/src/grave_settings/base.py` & `grave-settings-0.1.4/src/grave_settings/base.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/config_file.py` & `grave-settings-0.1.4/src/grave_settings/config_file.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/conversion_manager.py` & `grave-settings-0.1.4/src/grave_settings/conversion_manager.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/default_handlers.py` & `grave-settings-0.1.4/src/grave_settings/default_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from numbers import Rational, Complex
 from pathlib import Path
 from types import NoneType, MethodType
 from datetime import timedelta, datetime, date, timezone, tzinfo
 from enum import Enum
 from typing import Mapping, Union, get_args
-from types import FunctionType
+from types import FunctionType, BuiltinFunctionType
 from functools import partial
 from zoneinfo import ZoneInfo
 
 from observer_hooks import FunctionStub, EventHandler
 from grave_settings.utilities import get_type_hints, format_class_str, load_type, T
 
 from grave_settings.formatter_settings import Temporary, PreservedReference, FormatterContext, NoRef
@@ -43,14 +43,15 @@
             object: self.default_handler,
             Type: self.handle_type,
             NoneType: self.handle_NoneType,
             Iterable: self.handle_Iterable,
             Mapping: self.handle_Mapping,
             FunctionType: self.handle_function_type,
             MethodType: self.handle_method,
+            BuiltinFunctionType: self.handle_function_type,
             PreservedReference: self.handle_PreservedReference,
             Serializable: self.handle_serializable,
             date: self.handle_date,
             datetime: self.handle_datetime,
             timedelta: self.handle_timedelta,
             Enum: self.handle_Enum,
             partial: self.handle_partial,
```

### Comparing `grave-settings-0.1.3/src/grave_settings/formatter.py` & `grave-settings-0.1.4/src/grave_settings/formatter.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/formatter_settings.py` & `grave-settings-0.1.4/src/grave_settings/formatter_settings.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/formatters/bson.py` & `grave-settings-0.1.4/src/grave_settings/formatters/bson.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/formatters/json.py` & `grave-settings-0.1.4/src/grave_settings/formatters/json.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/formatters/toml.py` & `grave-settings-0.1.4/src/grave_settings/formatters/toml.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/framestack_context.py` & `grave-settings-0.1.4/src/grave_settings/framestack_context.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/handlers.py` & `grave-settings-0.1.4/src/grave_settings/handlers.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/helper_objects.py` & `grave-settings-0.1.4/src/grave_settings/helper_objects.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/semantics.py` & `grave-settings-0.1.4/src/grave_settings/semantics.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/utilities.py` & `grave-settings-0.1.4/src/grave_settings/utilities.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings/validation.py` & `grave-settings-0.1.4/src/grave_settings/validation.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.3/src/grave_settings.egg-info/PKG-INFO` & `grave-settings-0.1.4/src/grave_settings.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grave-settings
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for automatic serialization of python object hierarchies to storage
 Home-page: https://github.com/ILikesCaviar/GraveSettings
 Author: Ryan McConnell
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
@@ -112,19 +112,21 @@
 This will output:
 
 ```toml
 __class__ = "__main__.MyObject"
 integer = 1
 string = "b"
 
-[color]
-__class__ = "__main__.Color"
-b = 255
-g = 255
-r = 255
+[function]
+__class__ = "types.FunctionType"
+state = "builtins.print"
+
+[type_object]
+__class__ = "builtins.type"
+state = "builtins.int"
 
 [[dates]]
 __class__ = "datetime.date"
 state = [
     2022,
     1,
     1,
@@ -133,14 +135,20 @@
 [[dates]]
 __class__ = "datetime.date"
 state = [
     2023,
     2,
     2,
 ]
+
+[color]
+__class__ = "__main__.Color"
+r = 255
+g = 255
+b = 255
 ```
 
 Now if we take this string and deserialize it with the same (or equivalent) formatter:
 
 ```python
 from grave_settings.formatters.toml import TomlFormatter
 formatter = TomlFormatter()
```

### Comparing `grave-settings-0.1.3/src/grave_settings.egg-info/SOURCES.txt` & `grave-settings-0.1.4/src/grave_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

