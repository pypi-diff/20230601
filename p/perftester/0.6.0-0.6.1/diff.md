# Comparing `tmp/perftester-0.6.0.tar.gz` & `tmp/perftester-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perftester-0.6.0.tar", last modified: Thu Jun  1 09:21:21 2023, max compression
+gzip compressed data, was "perftester-0.6.1.tar", last modified: Thu Jun  1 10:10:51 2023, max compression
```

## Comparing `perftester-0.6.0.tar` & `perftester-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 09:21:21.137649 perftester-0.6.0/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-01 09:21:21.135744 perftester-0.6.0/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28074 2023-06-01 09:16:42.000000 perftester-0.6.0/README.md
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 09:21:21.094188 perftester-0.6.0/perftester/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      284 2023-06-01 07:37:48.000000 perftester-0.6.0/perftester/__init__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     5119 2022-06-22 16:29:34.000000 perftester-0.6.0/perftester/__main__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    33256 2023-06-01 09:21:14.000000 perftester-0.6.0/perftester/perftester.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1657 2022-09-02 13:30:35.000000 perftester-0.6.0/perftester/tmp.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      820 2022-09-02 07:16:38.000000 perftester-0.6.0/perftester/tmp_working.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    15670 2022-09-13 11:31:09.000000 perftester-0.6.0/perftester/understand.py
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 09:21:21.132740 perftester-0.6.0/perftester.egg-info/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-01 09:21:21.000000 perftester-0.6.0/perftester.egg-info/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      364 2023-06-01 09:21:21.000000 perftester-0.6.0/perftester.egg-info/SOURCES.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-01 09:21:21.000000 perftester-0.6.0/perftester.egg-info/dependency_links.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       57 2023-06-01 09:21:21.000000 perftester-0.6.0/perftester.egg-info/entry_points.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       61 2023-06-01 09:21:21.000000 perftester-0.6.0/perftester.egg-info/requires.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       11 2023-06-01 09:21:21.000000 perftester-0.6.0/perftester.egg-info/top_level.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-01 09:21:21.138260 perftester-0.6.0/setup.cfg
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      903 2023-06-01 09:12:21.000000 perftester-0.6.0/setup.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 10:10:51.140047 perftester-0.6.1/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-01 10:10:51.139047 perftester-0.6.1/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28074 2023-06-01 10:09:00.000000 perftester-0.6.1/README.md
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 10:10:51.099044 perftester-0.6.1/perftester/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      284 2023-06-01 10:09:00.000000 perftester-0.6.1/perftester/__init__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     5119 2022-06-22 16:29:34.000000 perftester-0.6.1/perftester/__main__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    33369 2023-06-01 10:09:15.000000 perftester-0.6.1/perftester/perftester.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1657 2022-09-02 13:30:35.000000 perftester-0.6.1/perftester/tmp.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      820 2022-09-02 07:16:38.000000 perftester-0.6.1/perftester/tmp_working.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    15670 2023-06-01 10:09:00.000000 perftester-0.6.1/perftester/understand.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 10:10:51.135045 perftester-0.6.1/perftester.egg-info/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      364 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       57 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/entry_points.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       61 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/requires.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       11 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/top_level.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-01 10:10:51.140503 perftester-0.6.1/setup.cfg
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      903 2023-06-01 10:09:41.000000 perftester-0.6.1/setup.py
```

### Comparing `perftester-0.6.0/PKG-INFO` & `perftester-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perftester
-Version: 0.6.0
+Version: 0.6.1
 Summary: Lightweight performance testing in Python
 Home-page: https://github.com/nyggus/perftester
 Author: Nyggus
 Author-email: nyggus@gmail.com
 License: UNKNOWN
 Description: # `perftester`: Lightweight performance testing of Python functions
```

### Comparing `perftester-0.6.0/README.md` & `perftester-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `perftester-0.6.0/perftester/__main__.py` & `perftester-0.6.1/perftester/__main__.py`

 * *Files identical despite different names*

### Comparing `perftester-0.6.0/perftester/perftester.py` & `perftester-0.6.1/perftester/perftester.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 """
 import builtins
 import copy
 import os
 import rounder
 import sys
 import timeit
+import warnings
 
 from collections import namedtuple
 from collections.abc import Callable
 from easycheck import (
     check_argument,
     check_if,
     check_if_not,
@@ -869,18 +870,21 @@
     MEMLOGS, also available from any module.
     
     Memory is collected using pympler.asizeof.asizeof(), and reported in
     bytes. So, the function measures the size of all current gc objects,
     including module, global and stack frame objects, minus the size
     of `MEMLOGS`.
     """
-    MEMLOGS.append(MemLog( # type: ignore
-            ID,
-            (asizeof(all=True) - asizeof(MEMLOGS))) # type: ignore
-        )
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        MEMLOGS.append(MemLog( # type: ignore
+                ID,
+                (asizeof(all=True) - asizeof(MEMLOGS))) # type: ignore
+            )
+
 
 
 def MEMTRACE(func, ID_before=None, ID_after=None):
     """Decorator to log memory before and after running a function."""
     @wraps(func)
     def inner(*args, **kwargs):
         before = ID_before if ID_before else f"Before {func.__name__}()"
```

### Comparing `perftester-0.6.0/perftester/tmp.py` & `perftester-0.6.1/perftester/tmp.py`

 * *Files identical despite different names*

### Comparing `perftester-0.6.0/perftester/tmp_working.py` & `perftester-0.6.1/perftester/tmp_working.py`

 * *Files identical despite different names*

### Comparing `perftester-0.6.0/perftester/understand.py` & `perftester-0.6.1/perftester/understand.py`

 * *Files identical despite different names*

### Comparing `perftester-0.6.0/perftester.egg-info/PKG-INFO` & `perftester-0.6.1/perftester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perftester
-Version: 0.6.0
+Version: 0.6.1
 Summary: Lightweight performance testing in Python
 Home-page: https://github.com/nyggus/perftester
 Author: Nyggus
 Author-email: nyggus@gmail.com
 License: UNKNOWN
 Description: # `perftester`: Lightweight performance testing of Python functions
```

### Comparing `perftester-0.6.0/setup.py` & `perftester-0.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 extras_requirements = {
     "dev": ["wheel", "black"],
 }
 
 setuptools.setup(
     name="perftester",
-    version="0.6.0",
+    version="0.6.1",
     author="Nyggus",
     author_email="nyggus@gmail.com",
     description="Lightweight performance testing in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyggus/perftester",
     packages=setuptools.find_packages(),
```

