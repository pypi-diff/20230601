# Comparing `tmp/permacache-3.6.2.tar.gz` & `tmp/permacache-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permacache-3.6.2.tar", last modified: Tue Dec  6 23:50:16 2022, max compression
+gzip compressed data, was "permacache-3.7.0.tar", last modified: Thu Jun  1 19:55:31 2023, max compression
```

## Comparing `permacache-3.6.2.tar` & `permacache-3.7.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2022-12-06 23:50:16.302215 permacache-3.6.2/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3051 2022-12-06 23:50:16.302215 permacache-3.6.2/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2105 2021-12-16 05:53:32.000000 permacache-3.6.2/README.md
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2022-12-06 23:50:16.302215 permacache-3.6.2/permacache/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      179 2022-09-20 00:37:01.000000 permacache-3.6.2/permacache/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2987 2022-04-08 03:07:04.000000 permacache-3.6.2/permacache/cache.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1183 2022-01-29 00:35:40.000000 permacache-3.6.2/permacache/dict_function.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3875 2022-04-08 03:07:04.000000 permacache-3.6.2/permacache/hash.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3988 2022-12-06 23:50:14.000000 permacache-3.6.2/permacache/locked_shelf.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1065 2021-03-14 06:24:57.000000 permacache-3.6.2/permacache/main.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      584 2022-09-20 00:37:01.000000 permacache-3.6.2/permacache/swap_unpickler.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      853 2022-01-29 00:38:11.000000 permacache-3.6.2/permacache/utils.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2022-12-06 23:50:16.302215 permacache-3.6.2/permacache.egg-info/
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3051 2022-12-06 23:50:16.000000 permacache-3.6.2/permacache.egg-info/PKG-INFO
--rw-r--r--   0 kavi      (1000) kavi      (1000)      419 2022-12-06 23:50:16.000000 permacache-3.6.2/permacache.egg-info/SOURCES.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)        1 2022-12-06 23:50:16.000000 permacache-3.6.2/permacache.egg-info/dependency_links.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       53 2022-12-06 23:50:16.000000 permacache-3.6.2/permacache.egg-info/entry_points.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       32 2022-12-06 23:50:16.000000 permacache-3.6.2/permacache.egg-info/requires.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       11 2022-12-06 23:50:16.000000 permacache-3.6.2/permacache.egg-info/top_level.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       79 2022-12-06 23:50:16.302215 permacache-3.6.2/setup.cfg
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      838 2022-12-06 23:50:14.000000 permacache-3.6.2/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-01 19:55:31.802679 permacache-3.7.0/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3051 2023-06-01 19:55:31.802679 permacache-3.7.0/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2105 2021-12-16 05:53:32.000000 permacache-3.7.0/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-01 19:55:31.802679 permacache-3.7.0/permacache/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      247 2023-06-01 19:53:46.000000 permacache-3.7.0/permacache/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3381 2023-06-01 19:53:46.000000 permacache-3.7.0/permacache/cache.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      871 2023-06-01 19:53:46.000000 permacache-3.7.0/permacache/cache_miss_error.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1183 2022-01-29 00:35:40.000000 permacache-3.7.0/permacache/dict_function.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3875 2022-04-08 03:07:04.000000 permacache-3.7.0/permacache/hash.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3988 2022-12-06 23:50:14.000000 permacache-3.7.0/permacache/locked_shelf.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     1065 2021-03-14 06:24:57.000000 permacache-3.7.0/permacache/main.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      584 2022-09-20 00:37:01.000000 permacache-3.7.0/permacache/swap_unpickler.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      853 2022-01-29 00:38:11.000000 permacache-3.7.0/permacache/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-01 19:55:31.802679 permacache-3.7.0/permacache.egg-info/
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     3051 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/PKG-INFO
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      450 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/SOURCES.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)        1 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/dependency_links.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       53 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/entry_points.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       32 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/requires.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       11 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/top_level.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       79 2023-06-01 19:55:31.802679 permacache-3.7.0/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      838 2023-06-01 19:53:46.000000 permacache-3.7.0/setup.py
```

### Comparing `permacache-3.6.2/PKG-INFO` & `permacache-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permacache
-Version: 3.6.2
+Version: 3.7.0
 Summary: Permanant cache.
 Home-page: https://github.com/kavigupta/permacache
 Author: Kavi Gupta
 Author-email: permacache@kavigupta.org
 License: UNKNOWN
 Description: 
         # Permacache
```

### Comparing `permacache-3.6.2/README.md` & `permacache-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `permacache-3.6.2/permacache/cache.py` & `permacache-3.7.0/permacache/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 import os
 
 import shutil
 
 from appdirs import user_cache_dir
 
-
+from .cache_miss_error import CacheMissError, error_on_miss, error_on_miss_global
 from .locked_shelf import LockedShelf
 from .hash import stringify
 from .dict_function import dict_function, parallel_output
 from .utils import bind_arguments
 
 CACHE = user_cache_dir("permacache")
 
 
 class CachedFunction:
     def __init__(self, function, key_function, path, *, parallel, **kwargs):
         self.function = function
         self.key_function = key_function
         self.parallel = parallel
         self.shelf = LockedShelf(path, **kwargs)
+        self._error_on_miss = False
+
+    def _run_underlying(self, *args, **kwargs):
+        if self._error_on_miss or error_on_miss_global.error_on_miss:
+            raise CacheMissError
+        return self.function(*args, **kwargs)
+
+    def error_on_miss(self):
+        return error_on_miss(self)
 
     def __call__(self, *args, **kwargs):
         key = self.key_function(args, kwargs, parallel=self.parallel)
         if isinstance(key, parallel_output):
             return self.call_parallel(key.values, args, kwargs)
 
         key = stringify(key)
 
         with self.shelf as db:
             if key in db:
                 return db[key]
-        value = self.function(*args, **kwargs)
+        value = self._run_underlying(*args, **kwargs)
         with self.shelf as db:
             # TODO maybe check if key is now in db
             db[key] = value
         return value
 
     def cache_contains(self, *args, **kwargs):
         key = self.key_function(args, kwargs, parallel=self.parallel)
@@ -61,15 +70,15 @@
             arguments = bind_arguments(self.function, args, kwargs)
             arguments = arguments.copy()
             for k in self.parallel:
                 arg = arguments[k]
                 arg = [arg[i] for i in indices]
                 arguments[k] = arg
 
-            values_for_indices = self.function(**arguments)
+            values_for_indices = self._run_underlying(**arguments)
         with self.shelf as db:
             for k, v in zip(keys_for_indices, values_for_indices):
                 db[k] = v
             return [db[k] for k in keys]
 
 
 def permacache(path, key_function=dict(), *, parallel=(), **kwargs):
```

### Comparing `permacache-3.6.2/permacache/dict_function.py` & `permacache-3.7.0/permacache/dict_function.py`

 * *Files identical despite different names*

### Comparing `permacache-3.6.2/permacache/hash.py` & `permacache-3.7.0/permacache/hash.py`

 * *Files identical despite different names*

### Comparing `permacache-3.6.2/permacache/locked_shelf.py` & `permacache-3.7.0/permacache/locked_shelf.py`

 * *Files identical despite different names*

### Comparing `permacache-3.6.2/permacache/main.py` & `permacache-3.7.0/permacache/main.py`

 * *Files identical despite different names*

### Comparing `permacache-3.6.2/permacache/swap_unpickler.py` & `permacache-3.7.0/permacache/swap_unpickler.py`

 * *Files identical despite different names*

### Comparing `permacache-3.6.2/permacache/utils.py` & `permacache-3.7.0/permacache/utils.py`

 * *Files identical despite different names*

### Comparing `permacache-3.6.2/permacache.egg-info/PKG-INFO` & `permacache-3.7.0/permacache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permacache
-Version: 3.6.2
+Version: 3.7.0
 Summary: Permanant cache.
 Home-page: https://github.com/kavigupta/permacache
 Author: Kavi Gupta
 Author-email: permacache@kavigupta.org
 License: UNKNOWN
 Description: 
         # Permacache
```

### Comparing `permacache-3.6.2/setup.py` & `permacache-3.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="permacache",
-    version="3.6.2",
+    version="3.7.0",
     author="Kavi Gupta",
     author_email="permacache@kavigupta.org",
     description="Permanant cache.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/permacache",
     packages=setuptools.find_packages(),
```

