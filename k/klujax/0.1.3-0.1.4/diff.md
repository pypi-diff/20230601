# Comparing `tmp/klujax-0.1.3.tar.gz` & `tmp/klujax-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klujax-0.1.3.tar", last modified: Tue Jan 24 17:13:24 2023, max compression
+gzip compressed data, was "klujax-0.1.4.tar", last modified: Thu Jun  1 17:42:29 2023, max compression
```

## Comparing `klujax-0.1.3.tar` & `klujax-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 17:13:24.195617 klujax-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (122)    24478 2023-01-24 17:12:17.000000 klujax-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-01-24 17:13:24.195617 klujax-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-01-24 17:12:17.000000 klujax-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-01-24 17:12:17.000000 klujax-0.1.3/klujax.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 17:13:24.195617 klujax-0.1.3/klujax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-01-24 17:13:24.000000 klujax-0.1.3/klujax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-01-24 17:13:24.000000 klujax-0.1.3/klujax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-24 17:13:24.000000 klujax-0.1.3/klujax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-01-24 17:13:24.000000 klujax-0.1.3/klujax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-01-24 17:13:24.000000 klujax-0.1.3/klujax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12146 2023-01-24 17:12:17.000000 klujax-0.1.3/klujax.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-01-24 17:12:17.000000 klujax-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-24 17:13:24.195617 klujax-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-01-24 17:12:17.000000 klujax-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 17:42:29.206645 klujax-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    24478 2023-06-01 17:41:20.000000 klujax-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-06-01 17:42:29.206645 klujax-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-06-01 17:41:20.000000 klujax-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-06-01 17:41:20.000000 klujax-0.1.4/klujax.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 17:42:29.206645 klujax-0.1.4/klujax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12146 2023-06-01 17:41:20.000000 klujax-0.1.4/klujax.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-01 17:41:20.000000 klujax-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 17:42:29.206645 klujax-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-06-01 17:41:20.000000 klujax-0.1.4/setup.py
```

### Comparing `klujax-0.1.3/LICENSE` & `klujax-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `klujax-0.1.3/PKG-INFO` & `klujax-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klujax
-Version: 0.1.3
+Version: 0.1.4
 Summary: a KLU solver for JAX
 Home-page: https://github.com/flaport/klujax
 Author: Floris Laporte
 Author-email: floris.laporte@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `klujax-0.1.3/README.md` & `klujax-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `klujax-0.1.3/klujax.cpp` & `klujax-0.1.4/klujax.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// version: 0.1.3
+// version: 0.1.4
 // author: Floris Laporte
 
 #include <iostream>
 #include <vector>
 
 #include <klu.h>
 #include <pybind11/pybind11.h>
```

### Comparing `klujax-0.1.3/klujax.egg-info/PKG-INFO` & `klujax-0.1.4/klujax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klujax
-Version: 0.1.3
+Version: 0.1.4
 Summary: a KLU solver for JAX
 Home-page: https://github.com/flaport/klujax
 Author: Floris Laporte
 Author-email: floris.laporte@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `klujax-0.1.3/klujax.py` & `klujax-0.1.4/klujax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ klujax: a KLU solver for JAX """
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "Floris Laporte"
 __all__ = ["solve", "coo_mul_vec"]
 
 
 # Imports =============================================================================
```

### Comparing `klujax-0.1.3/setup.py` & `klujax-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         "suitesparseconfig",
     ],
     language="c++",
 )
 
 setup(
     name="klujax",
-    version="0.1.3",
+    version="0.1.4",
     author="Floris Laporte",
     author_email="floris.laporte@gmail.com",
     description="a KLU solver for JAX",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/flaport/klujax",
     py_modules=["klujax"],
```

