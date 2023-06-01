# Comparing `tmp/gravitas-0.1.5.tar.gz` & `tmp/gravitas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.1.5.tar", last modified: Wed May 31 05:21:09 2023, max compression
+gzip compressed data, was "gravitas-0.1.7.tar", last modified: Thu Jun  1 16:33:24 2023, max compression
```

## Comparing `gravitas-0.1.5.tar` & `gravitas-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:21:09.759637 gravitas-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 05:21:09.759637 gravitas-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 05:20:58.000000 gravitas-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:21:09.755638 gravitas-0.1.5/gravitas/
--rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/EGM96.c
--rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/GRGM360.c
--rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/MRO120F.c
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/gravlib.c
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/libgrav.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:21:09.759637 gravitas-0.1.5/gravitas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-31 05:20:58.000000 gravitas-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 05:21:09.759637 gravitas-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 05:20:58.000000 gravitas-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:33:24.499450 gravitas-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-01 16:33:24.499450 gravitas-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-01 16:33:14.000000 gravitas-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:33:24.495449 gravitas-0.1.7/gravitas/
+-rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/EGM96.c
+-rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/GRGM360.c
+-rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/MRO120F.c
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/gravlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/libgrav.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:33:24.495449 gravitas-0.1.7/gravitas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 16:33:14.000000 gravitas-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:33:24.499450 gravitas-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-01 16:33:14.000000 gravitas-0.1.7/setup.py
```

### Comparing `gravitas-0.1.5/PKG-INFO` & `gravitas-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.1.5
+Version: 0.1.7
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 License: GPL-2
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `gravitas-0.1.5/README.md` & `gravitas-0.1.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Setup
 
 `pip install gravitas`
 
 # Example Usage
 
 ```python
+import gravitas
 import numpy as np
 
 r_ecef = np.array([[7000.0, 0.0, 0.0], [0.0, 7000.0, 0.0]]) 
 # Define an [nx3] numpy array in Earth-Centered, Earth-Fixed (ECEF) coordinates [km]
 g_vector = gravitas.acceleration(r_ecef, max_order=360, use_model="EGM96") 
 # Query the acceneration at these positions using a maximum degree/order of 360 and the EGM96 Earth gravity model
 >>> [[-8.14574564e-03 -2.19120213e-08  3.01312643e-08]
```

### Comparing `gravitas-0.1.5/gravitas/EGM96.c` & `gravitas-0.1.7/gravitas/EGM96.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.5/gravitas/GRGM360.c` & `gravitas-0.1.7/gravitas/GRGM360.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.5/gravitas/MRO120F.c` & `gravitas-0.1.7/gravitas/MRO120F.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.5/gravitas/gravlib.c` & `gravitas-0.1.7/gravitas/gravlib.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.5/gravitas/lib.py` & `gravitas-0.1.7/gravitas/lib.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.5/gravitas/libgrav.h` & `gravitas-0.1.7/gravitas/libgrav.h`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.5/gravitas.egg-info/PKG-INFO` & `gravitas-0.1.7/gravitas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.1.5
+Version: 0.1.7
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 License: GPL-2
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `gravitas-0.1.5/setup.py` & `gravitas-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import numpy as np
 
 _SOURCES = [os.path.join('gravitas', x) for x in os.listdir('gravitas') if '.c' == x[-2:]]
 _INCDIR = ['gravitas', np.get_include()]
 
 class CustomBuildExt(build_ext):
     def build_extensions(self):
-        # for ext in self.extensions:
-        #     if self.compiler.compiler_type == 'msvc':
-        #         ext.extra_compile_args.append('/std:c90')
         super().build_extensions()
 
 # _LIB_DIR
 setup(
     name='gravitas',
-    version='0.1.5',
+    version='0.1.7',
     packages=find_packages(),
     license='GPL-2',
     long_description="""High-fidelity gravity fields for satellite propagation""",
     long_description_content_type='text/markdown',
     author="Liam Robinson",
     author_email="robin502@purdue.edu",
     install_requires=['numpy'],
     package_data={'gravitas': ['libgrav.h']},
     classifiers=[
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
     ],
```

