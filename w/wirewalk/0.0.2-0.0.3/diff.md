# Comparing `tmp/wirewalk-0.0.2.tar.gz` & `tmp/wirewalk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wirewalk-0.0.2.tar", last modified: Wed May 31 22:39:06 2023, max compression
+gzip compressed data, was "wirewalk-0.0.3.tar", last modified: Wed May 31 22:43:37 2023, max compression
```

## Comparing `wirewalk-0.0.2.tar` & `wirewalk-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:39:06.719502 wirewalk-0.0.2/
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 wirewalk-0.0.2/LICENSE
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)      111 2023-04-27 10:12:58.000000 wirewalk-0.0.2/MANIFEST.in
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     2109 2023-05-31 22:39:06.719356 wirewalk-0.0.2/PKG-INFO
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     1294 2023-05-31 22:39:02.000000 wirewalk-0.0.2/README.md
--rw-r--r--   0 tesfaasmara   (501) staff       (20)      870 2023-05-31 22:38:08.000000 wirewalk-0.0.2/settings.ini
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 22:39:06.719541 wirewalk-0.0.2/setup.cfg
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 wirewalk-0.0.2/setup.py
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:39:06.717907 wirewalk-0.0.2/wirewalk/
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       22 2023-05-31 22:39:00.000000 wirewalk-0.0.2/wirewalk/__init__.py
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     2551 2023-05-31 22:39:00.000000 wirewalk-0.0.2/wirewalk/_modidx.py
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     9419 2023-05-31 22:39:00.000000 wirewalk-0.0.2/wirewalk/core.py
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:39:06.719141 wirewalk-0.0.2/wirewalk.egg-info/
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     2109 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/PKG-INFO
--rw-r--r--   0 tesfaasmara   (501) staff       (20)      334 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/SOURCES.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/dependency_links.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/entry_points.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 22:31:34.000000 wirewalk-0.0.2/wirewalk.egg-info/not-zip-safe
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       42 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/requires.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        9 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/top_level.txt
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:43:37.950298 wirewalk-0.0.3/
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 wirewalk-0.0.3/LICENSE
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)      111 2023-04-27 10:12:58.000000 wirewalk-0.0.3/MANIFEST.in
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2472 2023-05-31 22:43:37.950128 wirewalk-0.0.3/PKG-INFO
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     1657 2023-05-31 22:43:20.000000 wirewalk-0.0.3/README.md
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)      870 2023-05-31 22:43:34.000000 wirewalk-0.0.3/settings.ini
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 22:43:37.950342 wirewalk-0.0.3/setup.cfg
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 wirewalk-0.0.3/setup.py
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:43:37.948762 wirewalk-0.0.3/wirewalk/
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       22 2023-05-31 22:43:34.000000 wirewalk-0.0.3/wirewalk/__init__.py
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2551 2023-05-31 22:43:34.000000 wirewalk-0.0.3/wirewalk/_modidx.py
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     9419 2023-05-31 22:43:34.000000 wirewalk-0.0.3/wirewalk/core.py
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:43:37.949881 wirewalk-0.0.3/wirewalk.egg-info/
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2472 2023-05-31 22:43:37.000000 wirewalk-0.0.3/wirewalk.egg-info/PKG-INFO
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)      334 2023-05-31 22:43:37.000000 wirewalk-0.0.3/wirewalk.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 22:43:37.000000 wirewalk-0.0.3/wirewalk.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 22:43:37.000000 wirewalk-0.0.3/wirewalk.egg-info/entry_points.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 22:31:34.000000 wirewalk-0.0.3/wirewalk.egg-info/not-zip-safe
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       42 2023-05-31 22:43:37.000000 wirewalk-0.0.3/wirewalk.egg-info/requires.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)        9 2023-05-31 22:43:37.000000 wirewalk-0.0.3/wirewalk.egg-info/top_level.txt
```

### Comparing `wirewalk-0.0.2/LICENSE` & `wirewalk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.2/PKG-INFO` & `wirewalk-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wirewalk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python3 Implementation of the WireWalk Algorithm
 Home-page: https://github.com/TesfaAsmara/wirewalk
 Author: tesfaasmara
 Author-email: 57428343+TesfaAsmara@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,26 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # wirewalk
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+# References
+
+[Wire Before You Walk. T. Asmara, D. Bhaskar, I. Adelstein, S.
+Krishnaswamy, M. Perlmutter. In proceedings for Asilomar
+2023.](http://tesfaasmara.com/wirewalk.pdf)
+
+# Asilomar 2023 Proceedings
+
+To reproduce the results, please see the instructions in the
+[Asilomar_2023.py](https://github.com/TesfaAsmara/wirewalk/blob/main/Asilomar_2023.py)
+file.
+
 ## Install
 
 ``` sh
 pip install wirewalk
 ```
 
 ### Prerequisites
```

### Comparing `wirewalk-0.0.2/README.md` & `wirewalk-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # wirewalk
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+# References
+
+[Wire Before You Walk. T. Asmara, D. Bhaskar, I. Adelstein, S.
+Krishnaswamy, M. Perlmutter. In proceedings for Asilomar
+2023.](http://tesfaasmara.com/wirewalk.pdf)
+
+# Asilomar 2023 Proceedings
+
+To reproduce the results, please see the instructions in the
+[Asilomar_2023.py](https://github.com/TesfaAsmara/wirewalk/blob/main/Asilomar_2023.py)
+file.
+
 ## Install
 
 ``` sh
 pip install wirewalk
 ```
 
 ### Prerequisites
```

### Comparing `wirewalk-0.0.2/settings.ini` & `wirewalk-0.0.3/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = wirewalk
 lib_name = wirewalk
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = wirewalk
 nbs_path = .
 recursive = False
 tst_flags = notest
```

### Comparing `wirewalk-0.0.2/setup.py` & `wirewalk-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.2/wirewalk/_modidx.py` & `wirewalk-0.0.3/wirewalk/_modidx.py`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.2/wirewalk/core.py` & `wirewalk-0.0.3/wirewalk/core.py`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.2/wirewalk.egg-info/PKG-INFO` & `wirewalk-0.0.3/wirewalk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wirewalk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python3 Implementation of the WireWalk Algorithm
 Home-page: https://github.com/TesfaAsmara/wirewalk
 Author: tesfaasmara
 Author-email: 57428343+TesfaAsmara@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,26 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # wirewalk
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+# References
+
+[Wire Before You Walk. T. Asmara, D. Bhaskar, I. Adelstein, S.
+Krishnaswamy, M. Perlmutter. In proceedings for Asilomar
+2023.](http://tesfaasmara.com/wirewalk.pdf)
+
+# Asilomar 2023 Proceedings
+
+To reproduce the results, please see the instructions in the
+[Asilomar_2023.py](https://github.com/TesfaAsmara/wirewalk/blob/main/Asilomar_2023.py)
+file.
+
 ## Install
 
 ``` sh
 pip install wirewalk
 ```
 
 ### Prerequisites
```

