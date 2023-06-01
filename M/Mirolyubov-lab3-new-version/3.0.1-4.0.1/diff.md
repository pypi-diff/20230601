# Comparing `tmp/Mirolyubov_lab3_new_version-3.0.1.tar.gz` & `tmp/Mirolyubov_lab3_new_version-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mirolyubov_lab3_new_version-3.0.1.tar", last modified: Wed May 31 12:54:30 2023, max compression
+gzip compressed data, was "Mirolyubov_lab3_new_version-4.0.1.tar", last modified: Thu Jun  1 09:57:27 2023, max compression
```

## Comparing `Mirolyubov_lab3_new_version-3.0.1.tar` & `Mirolyubov_lab3_new_version-4.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       54 2023-05-30 21:19:09.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/CONSTANTS.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       94 2023-05-30 21:19:09.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/__init__.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      323 2023-05-30 21:19:09.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/factory.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     7825 2023-05-31 12:52:02.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/json_serializer.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     9776 2023-05-31 12:52:02.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/packing.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     7999 2023-05-31 12:52:02.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/xml_serializer.py
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      171 2023-05-31 12:54:30.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      464 2023-05-31 12:54:30.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/SOURCES.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-31 12:54:30.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/dependency_links.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       28 2023-05-31 12:54:30.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/top_level.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      171 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/setup.cfg
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      315 2023-05-31 12:54:18.000000 Mirolyubov_lab3_new_version-3.0.1/setup.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-06-01 09:57:27.681399 Mirolyubov_lab3_new_version-4.0.1/
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-06-01 09:57:27.681399 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       54 2023-05-30 21:19:09.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version/CONSTANTS.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      186 2023-05-31 13:10:29.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version/__init__.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      379 2023-05-31 13:11:08.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version/factory.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     6556 2023-05-31 22:27:26.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version/json_serializer.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)    11653 2023-05-31 22:24:15.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version/packing.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     6600 2023-05-31 22:36:51.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version/xml_serializer.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-06-01 09:57:27.681399 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version.egg-info/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      171 2023-06-01 09:57:27.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version.egg-info/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      464 2023-06-01 09:57:27.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-06-01 09:57:27.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       28 2023-06-01 09:57:27.000000 Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version.egg-info/top_level.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      171 2023-06-01 09:57:27.681399 Mirolyubov_lab3_new_version-4.0.1/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-06-01 09:57:27.681399 Mirolyubov_lab3_new_version-4.0.1/setup.cfg
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      315 2023-06-01 09:57:12.000000 Mirolyubov_lab3_new_version-4.0.1/setup.py
```

### Comparing `Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/packing.py` & `Mirolyubov_lab3_new_version-4.0.1/Mirolyubov_lab3_new_version/packing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,78 @@
 import inspect
-import builtins
 import types
 from Mirolyubov_lab3_new_version.CONSTANTS import PRIMITIVE_TYPES
 from types import FunctionType, BuiltinFunctionType, LambdaType, CodeType, GetSetDescriptorType, MappingProxyType, \
     MethodDescriptorType, WrapperDescriptorType
-
-
-def is_generator(obj):
-    return inspect.isgenerator(obj)
+from types import FunctionType, LambdaType, CodeType, CellType, GeneratorType, ModuleType
 
 
 def is_function(obj):
     return inspect.isfunction(obj) or inspect.ismethod(obj) or isinstance(obj, LambdaType)
 
 
 def is_iterable(obj):
     return getattr(obj, "__iter__", None) is not None
 
 
 def convert(obj):
     if isinstance(obj, PRIMITIVE_TYPES):
         return obj
 
-    elif isinstance(obj, (list, tuple, set, dict)):
+    elif isinstance(obj, (tuple, list, dict, set,frozenset)):
         return obj
 
     elif is_function(obj):
         return pack_function(obj)
 
     elif inspect.iscode(obj):
-        return pack_inner_func(obj)
+        return pack_code(obj)
 
     elif inspect.isclass(obj):
         return pack_class(obj)
 
-    elif is_generator(obj):
-        return pack_generator(obj)
-
     elif is_iterable(obj):
         return pack_iterable(obj)
 
     else:
         return pack_object(obj)
 
 
-def pack_generator(obj, cls=None):
-    result = {"__type__": "generator"}
-    result["__name__"] = obj.__name__
-    lst = []
-
-    for i in obj:
-        lst.append(i)
-    result["__values__"] = lst
-
-    return result
-
-def unpack_generator(obj, cls=None):
-    for i in obj["__values__"]:
-        yield i
-
 def pack_function(obj, cls=None):
     result = {"__type__": "function"}
 
     if inspect.ismethod(obj):
         obj = obj.__func__
 
-    obj.__name__ = obj.__name__.replace('>', '')
-    result["__name__"] = obj.__name__.replace('<', '')
+    result["__name__"] = obj.__name__
 
     globs = get_global_vars(obj, cls)
     result["__globals__"] = pack_iterable(globs)
+    result["__closure__"] = convert(obj.__closure__)
 
     arguments = {}
 
     for (key, value) in inspect.getmembers(obj.__code__):
+        if key == 'co_lines':
+            continue
         if key.startswith("co_"):
-            if key == "co_lines":
-                continue
             if isinstance(value, bytes):
                 value = list(value)
 
             if is_iterable(value) and not isinstance(value, str):
-                converted_vals = []
+                packed_vals = []
 
                 for val in value:
                     if val is not None:
-                        converted_vals.append(convert(val))
+                        packed_vals.append(convert(val))
 
                     else:
-                        converted_vals.append(None)
+                        packed_vals.append(None)
 
-                arguments[key] = converted_vals
+                arguments[key] = packed_vals
 
                 continue
 
             arguments[key] = value
 
     result["__args__"] = arguments
 
@@ -118,15 +96,15 @@
 
             else:
                 globs[global_var] = func.__name__
     return globs
 
 
 def pack_iterable(obj):
-    if isinstance(obj, list) or isinstance(obj, tuple) or isinstance(obj, set):
+    if isinstance(obj, list) or isinstance(obj, tuple) or isinstance(obj, set) or isinstance(obj, bytes):
         packed_iterable = []
 
         for value in obj:
             packed_iterable.append(convert(value))
 
         if isinstance(obj, tuple):
             return tuple(packed_iterable)
@@ -140,17 +118,35 @@
         packed_dict = {}
 
         for key, value in obj.items():
             packed_dict[key] = convert(value)
 
         return packed_dict
 
+    else:
+        result = {"__type__": "iterator"}
+        values = []
+        for i in obj:
+            values.append(convert(i))
+
+        result["__values__"] = values
+
+        return result
+
+
+def pack_code(obj):
+    result = {"__type__": "code"}
 
-def pack_inner_func(obj):   
-    return pack_function(FunctionType(obj, {}))
+    for key, value in inspect.getmembers(obj):
+        if not key.startswith("co"):
+            continue
+
+        result[key] = convert(value)
+
+    return result
 
 
 def pack_class(obj):
     result = {'__type__': 'class', '__name__': obj.__name__}
 
     for attr in inspect.getmembers(obj):
         if attr[0] not in (
@@ -174,89 +170,151 @@
                 result[attr[0]] = convert(attr_value)
 
     result["__bases__"] = [pack_class(base) for base in obj.__bases__ if base != object]
 
     return result
 
 
-def unpack_class(obj):
-    class_bases = tuple(unpack_class(base) for base in obj["__bases__"])
-    class_methods = {}
-
-    for attr, value in obj.items():
-        class_methods[attr] = deconvert(value)
-
-    result = type(obj["__name__"], class_bases, class_methods)
-
-    for key, method in class_methods.items():
-        if inspect.isfunction(method):
-            method.__globals__.update({result.__name__: result})
-
-    return result
-
-
 def pack_object(obj):
     result = {"__type__": "object", "__class__": pack_class(obj.__class__), "attr": {}}
+    if (obj.__class__.__name__ in ["property", "cell"]):
+        for key, value in inspect.getmembers(obj):
+            if not key.startswith("__"):
+                result["attr"][key] = convert(value)
 
-    for key, value in inspect.getmembers(obj):
-        if not key.startswith("__") and not is_function(value):
-            result["attr"][key] = convert(value)
+    else:
+        for key, value in inspect.getmembers(obj):
+            if not key.startswith("__") and not is_function(value):
+                result["attr"][key] = convert(value)
 
     return result
 
 
-def unpack_object(obj):
-    obj_class = deconvert(obj["__class__"])
-    attrs = {}
-
-    for key, value in obj["attr"].items():
-        attrs[key] = deconvert(value)
+def is_function(obj):
+    return inspect.isfunction(obj) or inspect.ismethod(obj) or isinstance(obj, LambdaType)
 
-    result = object.__new__(obj_class)
-    result.__dict__ = attrs
 
-    return result
+def is_iterable(obj):
+    return getattr(obj, "__iter__", None) is not None
 
 
 def deconvert(src):
     if isinstance(src, PRIMITIVE_TYPES):
         return src
 
     elif isinstance(src, dict):
         if "function" in src.values():
             return unpack_function(src)
 
         elif "object" in src.values():
             return unpack_object(src)
 
-        elif "generator" in src.values():
-            return unpack_generator(src)
-
         elif "class" in src.values():
             return unpack_class(src)
 
+        elif "code" in src.values():
+            return unpack_code(src)
+
+        elif "iterator" in src.values():
+            return unpack_iterator(src)
+
         else:
             return unpack_iterable(src)
 
     elif is_iterable(src):
         return unpack_iterable(src)
 
+    elif "module" == src.__class__.__name__:
+        return unpack_module(src)
+
     else:
+
         raise Exception("Unknown type")
 
 
+def unpack_module(obj):
+    return obj
+
+
+def unpack_class(obj):
+    class_bases = tuple(unpack_class(base) for base in obj["__bases__"])
+    class_methods = {}
+
+    for attr, value in obj.items():
+        class_methods[attr] = deconvert(value)
+
+    result = type(obj["__name__"], class_bases, class_methods)
+
+    for key, method in class_methods.items():
+        if inspect.isfunction(method):
+            method.__globals__.update({result.__name__: result})
+
+    return result
+
+
+def unpack_iterator(obj):
+    for i in deconvert(obj["__values__"]):
+        yield i
+
+
+def unpack_code(obj):
+    attrs = {}
+
+    for key, value in obj.items():
+        attrs[key] = deconvert(value)
+
+    result = CodeType(attrs['co_argcount'],
+                      attrs['co_posonlyargcount'],
+                      attrs['co_kwonlyargcount'],
+                      attrs['co_nlocals'],
+                      attrs['co_stacksize'],
+                      attrs['co_flags'],
+                      bytes(attrs['co_code']),
+                      tuple(deconvert(attrs['co_consts'])),
+                      tuple(attrs['co_names']),
+                      tuple(attrs['co_varnames']),
+                      attrs['co_filename'],
+                      attrs['co_name'],
+                      attrs['co_firstlineno'],
+                      bytes(attrs['co_lnotab']),
+                      tuple(attrs['co_freevars']),
+                      tuple(attrs['co_cellvars']))
+
+    return result
+
+
+def unpack_object(obj):
+    obj_class = deconvert(obj["__class__"])
+    attrs = {}
+
+    for key, value in obj["attr"].items():
+        attrs[key] = deconvert(value)
+
+    if "property" in obj_class.__name__:
+        obj_class = property
+        result = property(fget=attrs["fget"], fset=attrs["fset"], fdel=attrs["fdel"])
+    elif "cell" in obj_class.__name__:
+        result = CellType(attrs["cell_contents"])
+    else:
+        result = object.__new__(obj_class)
+        result.__dict__ = attrs
+
+    return result
+
+
 def unpack_function(src):
     arguments = src["__args__"]
     globs = src["__globals__"]
-    globs["__builtins__"] = builtins
+    globs["__builtins__"] = __builtins__
 
     for key in src["__globals__"]:
         if key in arguments["co_names"]:
             try:
                 globs[key] = __import__(src["__globals__"][key])
+
             except:
                 if globs[key] != src["__name__"]:
                     globs[key] = deconvert(src["__globals__"][key])
 
     coded = CodeType(arguments['co_argcount'],
                      arguments['co_posonlyargcount'],
                      arguments['co_kwonlyargcount'],
@@ -270,15 +328,15 @@
                      arguments['co_filename'],
                      arguments['co_name'],
                      arguments['co_firstlineno'],
                      bytes(arguments['co_lnotab']),
                      tuple(arguments['co_freevars']),
                      tuple(arguments['co_cellvars']))
 
-    func_result = FunctionType(coded, globs)
+    func_result = FunctionType(coded, globs, closure=deconvert(src["__closure__"]))
     func_result.__globals__.update({func_result.__name__: func_result})
 
     return func_result
 
 
 def unpack_iterable(obj):
     if isinstance(obj, list) or isinstance(obj, tuple) or isinstance(obj, set):
@@ -369,8 +427,8 @@
 
         for key, val in src.items():
             result[key] = restore_object_from_dict(val)
 
         return result
 
     else:
-        raise Exception("Object type must be dict")
+        raise Exception("Object type must be dict")
```

