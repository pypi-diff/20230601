# Comparing `tmp/pyjoptional-1.0.5.tar.gz` & `tmp/pyjoptional-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjoptional-1.0.5.tar", last modified: Fri Jan  6 14:33:19 2023, max compression
+gzip compressed data, was "pyjoptional-1.0.6.tar", last modified: Thu Jun  1 16:06:43 2023, max compression
```

## Comparing `pyjoptional-1.0.5.tar` & `pyjoptional-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-01-06 14:33:19.936323 pyjoptional-1.0.5/
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)    35149 2022-12-16 13:18:51.000000 pyjoptional-1.0.5/LICENSE
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2831 2023-01-06 14:33:19.936323 pyjoptional-1.0.5/PKG-INFO
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2101 2022-12-16 13:21:11.000000 pyjoptional-1.0.5/README.md
-drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-01-06 14:33:19.932323 pyjoptional-1.0.5/pyjoptional.egg-info/
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2831 2023-01-06 14:33:19.000000 pyjoptional-1.0.5/pyjoptional.egg-info/PKG-INFO
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)      258 2023-01-06 14:33:19.000000 pyjoptional-1.0.5/pyjoptional.egg-info/SOURCES.txt
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        1 2023-01-06 14:33:19.000000 pyjoptional-1.0.5/pyjoptional.egg-info/dependency_links.txt
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        6 2023-01-06 14:33:19.000000 pyjoptional-1.0.5/pyjoptional.egg-info/requires.txt
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       11 2023-01-06 14:33:19.000000 pyjoptional-1.0.5/pyjoptional.egg-info/top_level.txt
-drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-01-06 14:33:19.936323 pyjoptional-1.0.5/pyoptional/
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2022-12-15 10:28:34.000000 pyjoptional-1.0.5/pyoptional/__init__.py
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     8159 2023-01-05 17:06:35.000000 pyjoptional-1.0.5/pyoptional/pyoptional.py
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       38 2023-01-06 14:33:19.936323 pyjoptional-1.0.5/setup.cfg
--rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     1178 2023-01-05 17:00:49.000000 pyjoptional-1.0.5/setup.py
+drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 16:06:43.745137 pyjoptional-1.0.6/
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)    35149 2022-12-16 13:18:51.000000 pyjoptional-1.0.6/LICENSE
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2831 2023-06-01 16:06:43.745137 pyjoptional-1.0.6/PKG-INFO
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2101 2022-12-16 13:21:11.000000 pyjoptional-1.0.6/README.md
+drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 16:06:43.745137 pyjoptional-1.0.6/pyjoptional.egg-info/
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     2831 2023-06-01 16:06:43.000000 pyjoptional-1.0.6/pyjoptional.egg-info/PKG-INFO
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)      233 2023-06-01 16:06:43.000000 pyjoptional-1.0.6/pyjoptional.egg-info/SOURCES.txt
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        1 2023-06-01 16:06:43.000000 pyjoptional-1.0.6/pyjoptional.egg-info/dependency_links.txt
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        6 2023-06-01 16:06:43.000000 pyjoptional-1.0.6/pyjoptional.egg-info/requires.txt
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       11 2023-06-01 16:06:43.000000 pyjoptional-1.0.6/pyjoptional.egg-info/top_level.txt
+drwxr-xr-x   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2023-06-01 16:06:43.745137 pyjoptional-1.0.6/pyoptional/
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)        0 2022-12-15 10:28:34.000000 pyjoptional-1.0.6/pyoptional/__init__.py
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)       38 2023-06-01 16:06:43.745137 pyjoptional-1.0.6/setup.cfg
+-rw-r--r--   0 cloudstrife9999  (1000) cloudstrife9999  (1000)     1178 2023-06-01 16:05:56.000000 pyjoptional-1.0.6/setup.py
```

### Comparing `pyjoptional-1.0.5/LICENSE` & `pyjoptional-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjoptional-1.0.5/PKG-INFO` & `pyjoptional-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoptional
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python module providing `PyOptional`, a Java-like `Optional` type for Python 3.8+.
 Home-page: https://github.com/cloudstrife9999/pyjoptional
 Author: Emanuele Uliana
 License: GNU3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyjoptional-1.0.5/README.md` & `pyjoptional-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyjoptional-1.0.5/pyjoptional.egg-info/PKG-INFO` & `pyjoptional-1.0.6/pyjoptional.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoptional
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python module providing `PyOptional`, a Java-like `Optional` type for Python 3.8+.
 Home-page: https://github.com/cloudstrife9999/pyjoptional
 Author: Emanuele Uliana
 License: GNU3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyjoptional-1.0.5/setup.py` & `pyjoptional-1.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ]
 dependencies: list = ["wheel"]
 
 # End of metadata
 
 setup(
     name=name,
-    version="1.0.5",
+    version="1.0.6",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cloudstrife9999/pyjoptional",
     author=author,
     license=license,
     packages=find_packages(),
```

