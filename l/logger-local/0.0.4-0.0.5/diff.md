# Comparing `tmp/logger-local-0.0.4.tar.gz` & `tmp/logger-local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-local-0.0.4.tar", last modified: Wed May 24 02:22:57 2023, max compression
+gzip compressed data, was "logger-local-0.0.5.tar", last modified: Thu Jun  1 06:38:34 2023, max compression
```

## Comparing `logger-local-0.0.4.tar` & `logger-local-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:22:57.467477 logger-local-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 02:22:44.000000 logger-local-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 02:22:57.467477 logger-local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 02:22:44.000000 logger-local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:22:57.467477 logger-local-0.0.4/logger_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 02:22:57.000000 logger-local-0.0.4/logger_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-24 02:22:57.000000 logger-local-0.0.4/logger_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:22:57.000000 logger-local-0.0.4/logger_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 02:22:57.000000 logger-local-0.0.4/logger_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:22:57.467477 logger-local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 02:22:44.000000 logger-local-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:22:57.467477 logger-local-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-24 02:22:44.000000 logger-local-0.0.4/src/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-24 02:22:44.000000 logger-local-0.0.4/src/LoggerServiceSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 02:22:44.000000 logger-local-0.0.4/src/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-24 02:22:44.000000 logger-local-0.0.4/src/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:22:44.000000 logger-local-0.0.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:22:57.467477 logger-local-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-24 02:22:44.000000 logger-local-0.0.4/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:34.261656 logger-local-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 06:38:24.000000 logger-local-0.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:34.257656 logger-local-0.0.5/LoggerLocalPythonPackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/LoggerServiceSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-01 06:38:34.261656 logger-local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-01 06:38:24.000000 logger-local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:34.257656 logger-local-0.0.5/logger_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-01 06:38:34.000000 logger-local-0.0.5/logger_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-01 06:38:34.000000 logger-local-0.0.5/logger_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 06:38:34.000000 logger-local-0.0.5/logger_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 06:38:34.000000 logger-local-0.0.5/logger_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 06:38:34.261656 logger-local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 06:38:24.000000 logger-local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:34.257656 logger-local-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-01 06:38:24.000000 logger-local-0.0.5/tests/test_writer.py
```

### Comparing `logger-local-0.0.4/LICENSE` & `logger-local-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.4/PKG-INFO` & `logger-local-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.4/logger_local.egg-info/PKG-INFO` & `logger-local-0.0.5/logger_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.4/setup.py` & `logger-local-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='logger-local',
-    version='0.0.4',
+    version='0.0.5',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Logger Python Local",
     long_description="This is a package for sharing common Logger function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles-zone/logger-local-python-package",
     packages=setuptools.find_packages(),
```

### Comparing `logger-local-0.0.4/src/LoggerService.py` & `logger-local-0.0.5/LoggerLocalPythonPackage/LoggerService.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.MessageSeverity import MessageSeverity
-from src.Writer import Writer
+from LoggerLocalPythonPackage.MessageSeverity import MessageSeverity
+from LoggerLocalPythonPackage.Writer import Writer
 
 
 class LoggerService:
 
     def __init__(self):
         self._writer = Writer()
```

### Comparing `logger-local-0.0.4/src/Writer.py` & `logger-local-0.0.5/LoggerLocalPythonPackage/Writer.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.4/tests/test_writer.py` & `logger-local-0.0.5/tests/test_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pymysql
 import os
-from src.MessageSeverity import MessageSeverity
-from src.LoggerServiceSingleton import locallgr
+from LoggerLocalPythonPackage.MessageSeverity import MessageSeverity
+from LoggerLocalPythonPackage.LoggerServiceSingleton import locallgr
 
 ID = 5000001
 # ID = 1
 
 def get_connection() -> pymysql.connections.Connection:
     return pymysql.connect(
         user=os.getenv('RDS_USERNAME'),
```

