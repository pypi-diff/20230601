# Comparing `tmp/pyjoptional-1.0.8.tar.gz` & `tmp/pyjoptional-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjoptional-1.0.8.tar", last modified: Thu Jun  1 17:01:47 2023, max compression
+gzip compressed data, was "pyjoptional-1.0.9.tar", last modified: Thu Jun  1 17:03:43 2023, max compression
```

## Comparing `pyjoptional-1.0.8.tar` & `pyjoptional-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 17:01:47.482836 pyjoptional-1.0.8/
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)    35149 2022-12-16 13:18:51.000000 pyjoptional-1.0.8/LICENSE
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       34 2023-06-01 16:45:57.000000 pyjoptional-1.0.8/MANIFEST.in
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2832 2023-06-01 17:01:47.482836 pyjoptional-1.0.8/PKG-INFO
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2101 2022-12-16 13:21:11.000000 pyjoptional-1.0.8/README.md
-drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 17:01:47.482836 pyjoptional-1.0.8/pyjoptional.egg-info/
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2832 2023-06-01 17:01:47.000000 pyjoptional-1.0.8/pyjoptional.egg-info/PKG-INFO
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)      296 2023-06-01 17:01:47.000000 pyjoptional-1.0.8/pyjoptional.egg-info/SOURCES.txt
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        1 2023-06-01 17:01:47.000000 pyjoptional-1.0.8/pyjoptional.egg-info/dependency_links.txt
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        6 2023-06-01 17:01:47.000000 pyjoptional-1.0.8/pyjoptional.egg-info/requires.txt
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       11 2023-06-01 17:01:47.000000 pyjoptional-1.0.8/pyjoptional.egg-info/top_level.txt
-drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 17:01:47.482836 pyjoptional-1.0.8/pyoptional/
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2022-12-15 10:28:34.000000 pyjoptional-1.0.8/pyoptional/__init__.py
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     8363 2023-06-01 16:57:30.000000 pyjoptional-1.0.8/pyoptional/pyoptional.py
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     5456 2023-06-01 16:30:12.000000 pyjoptional-1.0.8/pyoptional/pyoptional.pyi
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       38 2023-06-01 17:01:47.482836 pyjoptional-1.0.8/setup.cfg
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     1189 2023-06-01 17:00:20.000000 pyjoptional-1.0.8/setup.py
+drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 17:03:43.216745 pyjoptional-1.0.9/
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)    35149 2022-12-16 13:18:51.000000 pyjoptional-1.0.9/LICENSE
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       34 2023-06-01 16:45:57.000000 pyjoptional-1.0.9/MANIFEST.in
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2832 2023-06-01 17:03:43.216745 pyjoptional-1.0.9/PKG-INFO
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2101 2022-12-16 13:21:11.000000 pyjoptional-1.0.9/README.md
+drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 17:03:43.216745 pyjoptional-1.0.9/pyjoptional.egg-info/
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2832 2023-06-01 17:03:43.000000 pyjoptional-1.0.9/pyjoptional.egg-info/PKG-INFO
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)      296 2023-06-01 17:03:43.000000 pyjoptional-1.0.9/pyjoptional.egg-info/SOURCES.txt
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        1 2023-06-01 17:03:43.000000 pyjoptional-1.0.9/pyjoptional.egg-info/dependency_links.txt
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        6 2023-06-01 17:03:43.000000 pyjoptional-1.0.9/pyjoptional.egg-info/requires.txt
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       11 2023-06-01 17:03:43.000000 pyjoptional-1.0.9/pyjoptional.egg-info/top_level.txt
+drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 17:03:43.216745 pyjoptional-1.0.9/pyoptional/
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2022-12-15 10:28:34.000000 pyjoptional-1.0.9/pyoptional/__init__.py
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     8363 2023-06-01 16:57:30.000000 pyjoptional-1.0.9/pyoptional/pyoptional.py
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     5466 2023-06-01 17:02:13.000000 pyjoptional-1.0.9/pyoptional/pyoptional.pyi
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       38 2023-06-01 17:03:43.216745 pyjoptional-1.0.9/setup.cfg
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     1189 2023-06-01 17:02:29.000000 pyjoptional-1.0.9/setup.py
```

### Comparing `pyjoptional-1.0.8/LICENSE` & `pyjoptional-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjoptional-1.0.8/PKG-INFO` & `pyjoptional-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoptional
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python module providing `PyOptional`, a Java-like `Optional` type for Python 3.8+.
 Home-page: https://github.com/cloudstrife9999/pyjoptional
 Author: Emanuele Uliana
 License: GNU3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyjoptional-1.0.8/README.md` & `pyjoptional-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyjoptional-1.0.8/pyjoptional.egg-info/PKG-INFO` & `pyjoptional-1.0.9/pyjoptional.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoptional
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python module providing `PyOptional`, a Java-like `Optional` type for Python 3.8+.
 Home-page: https://github.com/cloudstrife9999/pyjoptional
 Author: Emanuele Uliana
 License: GNU3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyjoptional-1.0.8/pyoptional/pyoptional.py` & `pyjoptional-1.0.9/pyoptional/pyoptional.py`

 * *Files identical despite different names*

### Comparing `pyjoptional-1.0.8/pyoptional/pyoptional.pyi` & `pyjoptional-1.0.9/pyoptional/pyoptional.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     def if_present(self, fn: Callable[[T], Any]) -> None:
         '''
         If a value is present, performs the given action (i.e., applies `fn`) with the value, otherwise does nothing.
         '''
         ...
 
-    def if_present_or_else(self, fn: Callable[[T], Any], empty_fn: Callable) -> None:
+    def if_present_or_else(self, fn: Callable[[T], Any], empty_fn: Callable[[], None]) -> None:
         '''
         If a value is present, calls `fn` with the value as argument, otherwise calls `empty_fn` with no arguments.
         '''
         ...
 
     def filter(self, fn: Callable[[T], bool]) -> PyOptional[T]:
         '''
```

### Comparing `pyjoptional-1.0.8/setup.py` & `pyjoptional-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ]
 dependencies: list[str] = ["wheel"]
 
 # End of metadata
 
 setup(
     name=name,
-    version="1.0.8",
+    version="1.0.9",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cloudstrife9999/pyjoptional",
     author=author,
     license=license,
     packages=find_packages(),
```

