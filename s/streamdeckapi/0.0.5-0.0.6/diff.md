# Comparing `tmp/streamdeckapi-0.0.5.tar.gz` & `tmp/streamdeckapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeckapi-0.0.5.tar", last modified: Thu Jun  1 13:55:30 2023, max compression
+gzip compressed data, was "streamdeckapi-0.0.6.tar", last modified: Thu Jun  1 14:18:04 2023, max compression
```

## Comparing `streamdeckapi-0.0.5.tar` & `streamdeckapi-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/streamdeckapi/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/streamdeckapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:04.444562 streamdeckapi-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 14:18:04.444562 streamdeckapi-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 14:17:51.000000 streamdeckapi-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:18:04.444562 streamdeckapi-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-01 14:17:51.000000 streamdeckapi-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:04.444562 streamdeckapi-0.0.6/streamdeckapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 14:17:51.000000 streamdeckapi-0.0.6/streamdeckapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-01 14:17:51.000000 streamdeckapi-0.0.6/streamdeckapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 14:17:51.000000 streamdeckapi-0.0.6/streamdeckapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-01 14:17:51.000000 streamdeckapi-0.0.6/streamdeckapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 14:17:51.000000 streamdeckapi-0.0.6/streamdeckapi/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-01 14:17:51.000000 streamdeckapi-0.0.6/streamdeckapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:04.444562 streamdeckapi-0.0.6/streamdeckapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 14:18:04.000000 streamdeckapi-0.0.6/streamdeckapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-01 14:18:04.000000 streamdeckapi-0.0.6/streamdeckapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:18:04.000000 streamdeckapi-0.0.6/streamdeckapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 14:18:04.000000 streamdeckapi-0.0.6/streamdeckapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 14:18:04.000000 streamdeckapi-0.0.6/streamdeckapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 14:18:04.000000 streamdeckapi-0.0.6/streamdeckapi.egg-info/top_level.txt
```

### Comparing `streamdeckapi-0.0.5/PKG-INFO` & `streamdeckapi-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `streamdeckapi-0.0.5/README.md` & `streamdeckapi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.5/setup.py` & `streamdeckapi-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "Stream Deck API Library"
 
 # Setting up
 setup(
     name="streamdeckapi",
     version=VERSION,
     author="Patrick762",
```

### Comparing `streamdeckapi-0.0.5/streamdeckapi/api.py` & `streamdeckapi-0.0.6/streamdeckapi/api.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.5/streamdeckapi/server.py` & `streamdeckapi-0.0.6/streamdeckapi/server.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.5/streamdeckapi/tools.py` & `streamdeckapi-0.0.6/streamdeckapi/tools.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.5/streamdeckapi/types.py` & `streamdeckapi-0.0.6/streamdeckapi/types.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.5/streamdeckapi.egg-info/PKG-INFO` & `streamdeckapi-0.0.6/streamdeckapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

