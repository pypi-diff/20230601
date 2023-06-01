# Comparing `tmp/pyprobables-0.5.7.tar.gz` & `tmp/pyprobables-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprobables-0.5.7.tar", last modified: Wed Apr 26 01:58:17 2023, max compression
+gzip compressed data, was "pyprobables-0.5.8.tar", last modified: Thu Jun  1 18:24:36 2023, max compression
```

## Comparing `pyprobables-0.5.7.tar` & `pyprobables-0.5.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.247358 pyprobables-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 01:58:00.000000 pyprobables-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-26 01:58:17.243358 pyprobables-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-26 01:58:00.000000 pyprobables-0.5.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/probables/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/probables/blooms/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/blooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27728 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/blooms/bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/blooms/countingbloom.py
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/blooms/expandingbloom.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/probables/countminsketch/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/countminsketch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/countminsketch/countminsketch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/probables/cuckoo/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/cuckoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/cuckoo/countingcuckoo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/cuckoo/cuckoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/pyprobables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-26 01:58:17.000000 pyprobables-0.5.7/pyprobables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-26 01:58:17.000000 pyprobables-0.5.7/pyprobables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 01:58:17.000000 pyprobables-0.5.7/pyprobables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 01:58:17.000000 pyprobables-0.5.7/pyprobables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 01:58:00.000000 pyprobables-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 01:58:17.247358 pyprobables-0.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3954 2023-04-26 01:58:00.000000 pyprobables-0.5.7/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:36.983450 pyprobables-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 18:24:07.000000 pyprobables-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-06-01 18:24:36.983450 pyprobables-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-01 18:24:07.000000 pyprobables-0.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:36.979450 pyprobables-0.5.8/probables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:36.979450 pyprobables-0.5.8/probables/blooms/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/blooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27728 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/blooms/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/blooms/countingbloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/blooms/expandingbloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:36.979450 pyprobables-0.5.8/probables/countminsketch/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/countminsketch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/countminsketch/countminsketch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:36.983450 pyprobables-0.5.8/probables/cuckoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/cuckoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/cuckoo/countingcuckoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/cuckoo/cuckoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-01 18:24:07.000000 pyprobables-0.5.8/probables/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:36.983450 pyprobables-0.5.8/pyprobables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-06-01 18:24:36.000000 pyprobables-0.5.8/pyprobables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-01 18:24:36.000000 pyprobables-0.5.8/pyprobables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:24:36.000000 pyprobables-0.5.8/pyprobables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 18:24:36.000000 pyprobables-0.5.8/pyprobables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-01 18:24:07.000000 pyprobables-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:24:36.983450 pyprobables-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:36.983450 pyprobables-0.5.8/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3954 2023-06-01 18:24:07.000000 pyprobables-0.5.8/tests/test_utilities.py
```

### Comparing `pyprobables-0.5.7/LICENSE` & `pyprobables-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/PKG-INFO` & `pyprobables-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprobables
-Version: 0.5.7
+Version: 0.5.8
 Summary: Probabilistic data structures in python
 Author-email: Tyler Barrus <barrust@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/barrust/pyprobables
 Project-URL: Bug-tracker, https://github.com/barrust/pyprobables/issues
 Project-URL: Documentation, https://pyprobables.readthedocs.io/
 Keywords: python,probabilistic,data-structure,bloom,filter,count-min,sketch,bloom-filter,count-min-sketch,cuckoo-filter
@@ -43,15 +43,15 @@
 .. image:: https://codecov.io/gh/barrust/pyprobables/branch/master/graph/badge.svg?token=OdETiNgz9k
     :target: https://codecov.io/gh/barrust/pyprobables
     :alt: Test Coverage
 .. image:: https://readthedocs.org/projects/pyprobables/badge/?version=latest
     :target: http://pyprobables.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/pyprobables.svg
-    :target: https://badge.fury.io/py/pyprobables
+    :target: https://pypi.org/project/pyprobables/
     :alt: Pypi Release
 .. image:: https://pepy.tech/badge/pyprobables
     :target: https://pepy.tech/project/pyprobables
     :alt: Downloads
 
 **pyprobables** is a pure-python library for probabilistic data structures.
 The goal is to provide the developer with a pure-python implementation of
```

### Comparing `pyprobables-0.5.7/README.rst` & `pyprobables-0.5.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 .. image:: https://codecov.io/gh/barrust/pyprobables/branch/master/graph/badge.svg?token=OdETiNgz9k
     :target: https://codecov.io/gh/barrust/pyprobables
     :alt: Test Coverage
 .. image:: https://readthedocs.org/projects/pyprobables/badge/?version=latest
     :target: http://pyprobables.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/pyprobables.svg
-    :target: https://badge.fury.io/py/pyprobables
+    :target: https://pypi.org/project/pyprobables/
     :alt: Pypi Release
 .. image:: https://pepy.tech/badge/pyprobables
     :target: https://pepy.tech/project/pyprobables
     :alt: Downloads
 
 **pyprobables** is a pure-python library for probabilistic data structures.
 The goal is to provide the developer with a pure-python implementation of
```

### Comparing `pyprobables-0.5.7/probables/__init__.py` & `pyprobables-0.5.8/probables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     RotatingBloomFilterError,
 )
 
 __author__ = "Tyler Barrus"
 __maintainer__ = "Tyler Barrus"
 __email__ = "barrust@gmail.com"
 __license__ = "MIT"
-__version__ = "0.5.7"
+__version__ = "0.5.8"
 __credits__ = []  # type: ignore
 __url__ = "https://github.com/barrust/pyprobables"
 __bugtrack_url__ = "https://github.com/barrust/pyprobables/issues"
 
 __all__ = [
     "BloomFilter",
     "BloomFilterOnDisk",
```

### Comparing `pyprobables-0.5.7/probables/blooms/bloom.py` & `pyprobables-0.5.8/probables/blooms/bloom.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/probables/blooms/countingbloom.py` & `pyprobables-0.5.8/probables/blooms/countingbloom.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/probables/blooms/expandingbloom.py` & `pyprobables-0.5.8/probables/blooms/expandingbloom.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/probables/countminsketch/countminsketch.py` & `pyprobables-0.5.8/probables/countminsketch/countminsketch.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/probables/cuckoo/countingcuckoo.py` & `pyprobables-0.5.8/probables/cuckoo/countingcuckoo.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/probables/cuckoo/cuckoo.py` & `pyprobables-0.5.8/probables/cuckoo/cuckoo.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/probables/exceptions.py` & `pyprobables-0.5.8/probables/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/probables/hashes.py` & `pyprobables-0.5.8/probables/hashes.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/probables/utilities.py` & `pyprobables-0.5.8/probables/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """Simplified mmap.mmap class"""
 
     __slots__ = ("__p", "__f", "__m", "_closed")
 
     def __init__(self, path: Union[Path, str]):
         self.__p = Path(path)
         self.__f = self.path.open("rb")
-        self.__m = mmap.mmap(self.__f.fileno(), 0, prot=mmap.PROT_READ)
+        self.__m = mmap.mmap(self.__f.fileno(), 0, access=mmap.ACCESS_READ)
         self._closed = False
 
     def __enter__(self) -> mmap.mmap:
         return self.__m
 
     def __exit__(self, *args, **kwargs) -> None:
         if self.__m and not self.map.closed:
```

### Comparing `pyprobables-0.5.7/pyprobables.egg-info/PKG-INFO` & `pyprobables-0.5.8/pyprobables.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprobables
-Version: 0.5.7
+Version: 0.5.8
 Summary: Probabilistic data structures in python
 Author-email: Tyler Barrus <barrust@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/barrust/pyprobables
 Project-URL: Bug-tracker, https://github.com/barrust/pyprobables/issues
 Project-URL: Documentation, https://pyprobables.readthedocs.io/
 Keywords: python,probabilistic,data-structure,bloom,filter,count-min,sketch,bloom-filter,count-min-sketch,cuckoo-filter
@@ -43,15 +43,15 @@
 .. image:: https://codecov.io/gh/barrust/pyprobables/branch/master/graph/badge.svg?token=OdETiNgz9k
     :target: https://codecov.io/gh/barrust/pyprobables
     :alt: Test Coverage
 .. image:: https://readthedocs.org/projects/pyprobables/badge/?version=latest
     :target: http://pyprobables.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/pyprobables.svg
-    :target: https://badge.fury.io/py/pyprobables
+    :target: https://pypi.org/project/pyprobables/
     :alt: Pypi Release
 .. image:: https://pepy.tech/badge/pyprobables
     :target: https://pepy.tech/project/pyprobables
     :alt: Downloads
 
 **pyprobables** is a pure-python library for probabilistic data structures.
 The goal is to provide the developer with a pure-python implementation of
```

### Comparing `pyprobables-0.5.7/pyprobables.egg-info/SOURCES.txt` & `pyprobables-0.5.8/pyprobables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/pyproject.toml` & `pyprobables-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.7/tests/test_utilities.py` & `pyprobables-0.5.8/tests/test_utilities.py`

 * *Files identical despite different names*

