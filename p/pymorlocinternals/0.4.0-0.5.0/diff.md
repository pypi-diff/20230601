# Comparing `tmp/pymorlocinternals-0.4.0.tar.gz` & `tmp/pymorlocinternals-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymorlocinternals-0.4.0.tar", last modified: Sat May 27 04:08:20 2023, max compression
+gzip compressed data, was "pymorlocinternals-0.5.0.tar", last modified: Thu Jun  1 01:05:35 2023, max compression
```

## Comparing `pymorlocinternals-0.4.0.tar` & `pymorlocinternals-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-05-27 04:08:20.233332 pymorlocinternals-0.4.0/
--rw-r--r--   0 z         (1000) z         (1000)      464 2023-05-27 04:08:20.233332 pymorlocinternals-0.4.0/PKG-INFO
--rw-r--r--   0 z         (1000) z         (1000)       34 2022-02-16 21:54:00.000000 pymorlocinternals-0.4.0/README.md
-drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-05-27 04:08:20.229999 pymorlocinternals-0.4.0/pymorlocinternals/
--rw-r--r--   0 z         (1000) z         (1000)       68 2022-02-16 21:54:00.000000 pymorlocinternals-0.4.0/pymorlocinternals/__init__.py
--rw-r--r--   0 z         (1000) z         (1000)     2471 2023-05-27 03:51:47.000000 pymorlocinternals-0.4.0/pymorlocinternals/main.py
--rw-r--r--   0 z         (1000) z         (1000)     1003 2023-03-25 18:12:09.000000 pymorlocinternals-0.4.0/pymorlocinternals/types.py
--rw-r--r--   0 z         (1000) z         (1000)       22 2023-05-27 04:05:31.000000 pymorlocinternals-0.4.0/pymorlocinternals/version.py
-drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-05-27 04:08:20.233332 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/
--rw-r--r--   0 z         (1000) z         (1000)      464 2023-05-27 04:08:20.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/PKG-INFO
--rw-r--r--   0 z         (1000) z         (1000)      334 2023-05-27 04:08:20.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/SOURCES.txt
--rw-r--r--   0 z         (1000) z         (1000)        1 2023-05-27 04:08:20.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/dependency_links.txt
--rw-r--r--   0 z         (1000) z         (1000)        1 2023-05-27 04:08:00.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/not-zip-safe
--rw-r--r--   0 z         (1000) z         (1000)       18 2023-05-27 04:08:20.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/top_level.txt
--rw-r--r--   0 z         (1000) z         (1000)       38 2023-05-27 04:08:20.233332 pymorlocinternals-0.4.0/setup.cfg
--rw-r--r--   0 z         (1000) z         (1000)      770 2023-05-27 03:58:51.000000 pymorlocinternals-0.4.0/setup.py
+drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-06-01 01:05:35.592418 pymorlocinternals-0.5.0/
+-rw-r--r--   0 z         (1000) z         (1000)      464 2023-06-01 01:05:35.592418 pymorlocinternals-0.5.0/PKG-INFO
+-rw-r--r--   0 z         (1000) z         (1000)       34 2022-02-16 21:54:00.000000 pymorlocinternals-0.5.0/README.md
+drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-06-01 01:05:35.589085 pymorlocinternals-0.5.0/pymorlocinternals/
+-rw-r--r--   0 z         (1000) z         (1000)       68 2022-02-16 21:54:00.000000 pymorlocinternals-0.5.0/pymorlocinternals/__init__.py
+-rw-r--r--   0 z         (1000) z         (1000)     2821 2023-05-31 12:39:16.000000 pymorlocinternals-0.5.0/pymorlocinternals/main.py
+-rw-r--r--   0 z         (1000) z         (1000)     1003 2023-03-25 18:12:09.000000 pymorlocinternals-0.5.0/pymorlocinternals/types.py
+-rw-r--r--   0 z         (1000) z         (1000)       22 2023-06-01 01:04:37.000000 pymorlocinternals-0.5.0/pymorlocinternals/version.py
+drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-06-01 01:05:35.592418 pymorlocinternals-0.5.0/pymorlocinternals.egg-info/
+-rw-r--r--   0 z         (1000) z         (1000)      464 2023-06-01 01:05:35.000000 pymorlocinternals-0.5.0/pymorlocinternals.egg-info/PKG-INFO
+-rw-r--r--   0 z         (1000) z         (1000)      334 2023-06-01 01:05:35.000000 pymorlocinternals-0.5.0/pymorlocinternals.egg-info/SOURCES.txt
+-rw-r--r--   0 z         (1000) z         (1000)        1 2023-06-01 01:05:35.000000 pymorlocinternals-0.5.0/pymorlocinternals.egg-info/dependency_links.txt
+-rw-r--r--   0 z         (1000) z         (1000)        1 2023-06-01 01:05:06.000000 pymorlocinternals-0.5.0/pymorlocinternals.egg-info/not-zip-safe
+-rw-r--r--   0 z         (1000) z         (1000)       18 2023-06-01 01:05:35.000000 pymorlocinternals-0.5.0/pymorlocinternals.egg-info/top_level.txt
+-rw-r--r--   0 z         (1000) z         (1000)       38 2023-06-01 01:05:35.592418 pymorlocinternals-0.5.0/setup.cfg
+-rw-r--r--   0 z         (1000) z         (1000)      770 2023-05-27 03:58:51.000000 pymorlocinternals-0.5.0/setup.py
```

### Comparing `pymorlocinternals-0.4.0/pymorlocinternals/main.py` & `pymorlocinternals-0.5.0/pymorlocinternals/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import sys
 
 """
 ("tuple", [("float", None), ("record", OrderedDict(a=("float", None)))])
 """
 
 
 def serialize_list(x, schema):
@@ -93,12 +94,18 @@
     "str"    : lambda x, _: x,
     "bool"   : lambda x, _: x,
     "None"   : None
 }
 
 
 def mlc_deserialize(json_str, schema):
-    x = json.loads(json_str)
+    try:
+        x = json.loads(json_str)
+    except json.JSONDecodeError as e:
+        print(f"Python deserialization error in pymorlocinternals. Failed to deserialized type {type(json_str)} with value: {str(json_str)}", sys.stderr)
+        print(f"Using schema: {str(schema)}", sys.stderr)
+        print(f"JSONDecodeError: {str(e)}", sys.stderr)
+        sys.exit(1)
     if type(schema[0]) == str:
         return dispatch_deserialize[schema[0]](x, schema[1])
     else:
         return schema[0](**deserialize_record(x, schema[1]))
```

### Comparing `pymorlocinternals-0.4.0/pymorlocinternals/types.py` & `pymorlocinternals-0.5.0/pymorlocinternals/types.py`

 * *Files identical despite different names*

### Comparing `pymorlocinternals-0.4.0/setup.py` & `pymorlocinternals-0.5.0/setup.py`

 * *Files identical despite different names*

