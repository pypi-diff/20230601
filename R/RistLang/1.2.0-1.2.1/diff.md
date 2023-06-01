# Comparing `tmp/RistLang-1.2.0.tar.gz` & `tmp/RistLang-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RistLang-1.2.0.tar", last modified: Wed May 31 09:40:55 2023, max compression
+gzip compressed data, was "RistLang-1.2.1.tar", last modified: Thu Jun  1 11:41:37 2023, max compression
```

## Comparing `RistLang-1.2.0.tar` & `RistLang-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:55.310464 RistLang-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-31 09:40:33.000000 RistLang-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-31 09:40:55.310464 RistLang-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-31 09:40:33.000000 RistLang-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:55.310464 RistLang-1.2.0/RistLang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:55.310464 RistLang-1.2.0/ristpy/
--rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-05-31 09:40:33.000000 RistLang-1.2.0/ristpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-31 09:40:33.000000 RistLang-1.2.0/ristpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-31 09:40:33.000000 RistLang-1.2.0/ristpy/walkers.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:40:55.310464 RistLang-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-31 09:40:33.000000 RistLang-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:41:37.114766 RistLang-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-01 11:41:19.000000 RistLang-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-01 11:41:37.114766 RistLang-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-01 11:41:19.000000 RistLang-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:41:37.114766 RistLang-1.2.1/RistLang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-01 11:41:37.000000 RistLang-1.2.1/RistLang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-01 11:41:37.000000 RistLang-1.2.1/RistLang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:41:37.000000 RistLang-1.2.1/RistLang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 11:41:37.000000 RistLang-1.2.1/RistLang.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 11:41:37.000000 RistLang-1.2.1/RistLang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 11:41:37.000000 RistLang-1.2.1/RistLang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:41:37.114766 RistLang-1.2.1/ristpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-06-01 11:41:19.000000 RistLang-1.2.1/ristpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-01 11:41:19.000000 RistLang-1.2.1/ristpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-01 11:41:19.000000 RistLang-1.2.1/ristpy/walkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:41:37.114766 RistLang-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-01 11:41:19.000000 RistLang-1.2.1/setup.py
```

### Comparing `RistLang-1.2.0/LICENSE` & `RistLang-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RistLang-1.2.0/PKG-INFO` & `RistLang-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RistLang
-Version: 1.2.0
+Version: 1.2.1
 Summary: A module for compiling RistLang
 Home-page: https://github.com/RistPy/PyRist
 License: MIT
 Project-URL: Issue tracker, https://github.com/RistPy/PyRist/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RistPy
-A programming language made by me ([@Rishiraj0100](https://GitHub.com/Rishiraj0100))
+Just a programming language made to shorten the Python code
 ```
 R  - Rist
 I  - Is
 S  - Short
 T  - Text
 Py - Python
 ```
@@ -161,15 +161,15 @@
 $s    # str
 $y    # try
 $x    # xor
 $d    # dict
 $ei   # elif
 $e    # else
 $l    # list
-$p    # pass
+$pa   # pass
 $t    # type
 $b    # break
 $n    # input
 $p    # print
 $u    # tuple
 $wh   # while
 $yi   # yield
@@ -240,15 +240,16 @@
     ]
   }
 }
 ```
 Here `main` key is required while others are optional
 
 A sample file is given here
-```json{
+```json
+{
   "main": "main.rist",
   "dirs": ["dir_example"],
   "ignore": ["not_to_compile.rist"],
   "snippets": {
     "a": [
       "$p{0}",
       "$p{1}",
```

### Comparing `RistLang-1.2.0/README.md` & `RistLang-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # RistPy
-A programming language made by me ([@Rishiraj0100](https://GitHub.com/Rishiraj0100))
+Just a programming language made to shorten the Python code
 ```
 R  - Rist
 I  - Is
 S  - Short
 T  - Text
 Py - Python
 ```
@@ -143,15 +143,15 @@
 $s    # str
 $y    # try
 $x    # xor
 $d    # dict
 $ei   # elif
 $e    # else
 $l    # list
-$p    # pass
+$pa   # pass
 $t    # type
 $b    # break
 $n    # input
 $p    # print
 $u    # tuple
 $wh   # while
 $yi   # yield
@@ -222,15 +222,16 @@
     ]
   }
 }
 ```
 Here `main` key is required while others are optional
 
 A sample file is given here
-```json{
+```json
+{
   "main": "main.rist",
   "dirs": ["dir_example"],
   "ignore": ["not_to_compile.rist"],
   "snippets": {
     "a": [
       "$p{0}",
       "$p{1}",
```

### Comparing `RistLang-1.2.0/RistLang.egg-info/PKG-INFO` & `RistLang-1.2.1/RistLang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RistLang
-Version: 1.2.0
+Version: 1.2.1
 Summary: A module for compiling RistLang
 Home-page: https://github.com/RistPy/PyRist
 License: MIT
 Project-URL: Issue tracker, https://github.com/RistPy/PyRist/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RistPy
-A programming language made by me ([@Rishiraj0100](https://GitHub.com/Rishiraj0100))
+Just a programming language made to shorten the Python code
 ```
 R  - Rist
 I  - Is
 S  - Short
 T  - Text
 Py - Python
 ```
@@ -161,15 +161,15 @@
 $s    # str
 $y    # try
 $x    # xor
 $d    # dict
 $ei   # elif
 $e    # else
 $l    # list
-$p    # pass
+$pa   # pass
 $t    # type
 $b    # break
 $n    # input
 $p    # print
 $u    # tuple
 $wh   # while
 $yi   # yield
@@ -240,15 +240,16 @@
     ]
   }
 }
 ```
 Here `main` key is required while others are optional
 
 A sample file is given here
-```json{
+```json
+{
   "main": "main.rist",
   "dirs": ["dir_example"],
   "ignore": ["not_to_compile.rist"],
   "snippets": {
     "a": [
       "$p{0}",
       "$p{1}",
```

### Comparing `RistLang-1.2.0/ristpy/__init__.py` & `RistLang-1.2.1/ristpy/__init__.py`

 * *Files identical despite different names*

### Comparing `RistLang-1.2.0/ristpy/__main__.py` & `RistLang-1.2.1/ristpy/__main__.py`

 * *Files identical despite different names*

### Comparing `RistLang-1.2.0/ristpy/walkers.py` & `RistLang-1.2.1/ristpy/walkers.py`

 * *Files identical despite different names*

### Comparing `RistLang-1.2.0/setup.py` & `RistLang-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-version = "1.2.0"
+version = "1.2.1"
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 if version.endswith(('a', 'b', 'rc')):
   # append version identifier based on commit count
   try:
```

