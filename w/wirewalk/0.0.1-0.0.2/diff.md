# Comparing `tmp/wirewalk-0.0.1.tar.gz` & `tmp/wirewalk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wirewalk-0.0.1.tar", last modified: Wed May 31 22:31:34 2023, max compression
+gzip compressed data, was "wirewalk-0.0.2.tar", last modified: Wed May 31 22:39:06 2023, max compression
```

## Comparing `wirewalk-0.0.1.tar` & `wirewalk-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:31:34.525724 wirewalk-0.0.1/
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 wirewalk-0.0.1/LICENSE
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)      111 2023-04-27 10:12:58.000000 wirewalk-0.0.1/MANIFEST.in
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     2109 2023-05-31 22:31:34.525568 wirewalk-0.0.1/PKG-INFO
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     1294 2023-05-31 22:31:24.000000 wirewalk-0.0.1/README.md
--rw-r--r--   0 tesfaasmara   (501) staff       (20)      946 2023-05-31 22:14:09.000000 wirewalk-0.0.1/settings.ini
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 22:31:34.525772 wirewalk-0.0.1/setup.cfg
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 wirewalk-0.0.1/setup.py
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:31:34.524401 wirewalk-0.0.1/wirewalk/
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       22 2023-05-31 22:31:27.000000 wirewalk-0.0.1/wirewalk/__init__.py
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     2551 2023-05-31 22:31:27.000000 wirewalk-0.0.1/wirewalk/_modidx.py
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     9419 2023-05-31 22:31:27.000000 wirewalk-0.0.1/wirewalk/core.py
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:31:34.525370 wirewalk-0.0.1/wirewalk.egg-info/
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     2109 2023-05-31 22:31:34.000000 wirewalk-0.0.1/wirewalk.egg-info/PKG-INFO
--rw-r--r--   0 tesfaasmara   (501) staff       (20)      334 2023-05-31 22:31:34.000000 wirewalk-0.0.1/wirewalk.egg-info/SOURCES.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 22:31:34.000000 wirewalk-0.0.1/wirewalk.egg-info/dependency_links.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 22:31:34.000000 wirewalk-0.0.1/wirewalk.egg-info/entry_points.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 22:31:34.000000 wirewalk-0.0.1/wirewalk.egg-info/not-zip-safe
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        7 2023-05-31 22:31:34.000000 wirewalk-0.0.1/wirewalk.egg-info/requires.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        9 2023-05-31 22:31:34.000000 wirewalk-0.0.1/wirewalk.egg-info/top_level.txt
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:39:06.719502 wirewalk-0.0.2/
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 wirewalk-0.0.2/LICENSE
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)      111 2023-04-27 10:12:58.000000 wirewalk-0.0.2/MANIFEST.in
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2109 2023-05-31 22:39:06.719356 wirewalk-0.0.2/PKG-INFO
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     1294 2023-05-31 22:39:02.000000 wirewalk-0.0.2/README.md
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)      870 2023-05-31 22:38:08.000000 wirewalk-0.0.2/settings.ini
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 22:39:06.719541 wirewalk-0.0.2/setup.cfg
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 wirewalk-0.0.2/setup.py
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:39:06.717907 wirewalk-0.0.2/wirewalk/
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       22 2023-05-31 22:39:00.000000 wirewalk-0.0.2/wirewalk/__init__.py
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2551 2023-05-31 22:39:00.000000 wirewalk-0.0.2/wirewalk/_modidx.py
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     9419 2023-05-31 22:39:00.000000 wirewalk-0.0.2/wirewalk/core.py
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 22:39:06.719141 wirewalk-0.0.2/wirewalk.egg-info/
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2109 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/PKG-INFO
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)      334 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/entry_points.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 22:31:34.000000 wirewalk-0.0.2/wirewalk.egg-info/not-zip-safe
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       42 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/requires.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)        9 2023-05-31 22:39:06.000000 wirewalk-0.0.2/wirewalk.egg-info/top_level.txt
```

### Comparing `wirewalk-0.0.1/LICENSE` & `wirewalk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.1/PKG-INFO` & `wirewalk-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wirewalk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python3 Implementation of the WireWalk Algorithm
 Home-page: https://github.com/TesfaAsmara/wirewalk
 Author: tesfaasmara
 Author-email: 57428343+TesfaAsmara@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `wirewalk-0.0.1/README.md` & `wirewalk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.1/setup.py` & `wirewalk-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.1/wirewalk/_modidx.py` & `wirewalk-0.0.2/wirewalk/_modidx.py`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.1/wirewalk/core.py` & `wirewalk-0.0.2/wirewalk/core.py`

 * *Files identical despite different names*

### Comparing `wirewalk-0.0.1/wirewalk.egg-info/PKG-INFO` & `wirewalk-0.0.2/wirewalk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wirewalk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python3 Implementation of the WireWalk Algorithm
 Home-page: https://github.com/TesfaAsmara/wirewalk
 Author: tesfaasmara
 Author-email: 57428343+TesfaAsmara@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

