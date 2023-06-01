# Comparing `tmp/streamdeckapi-0.0.4.tar.gz` & `tmp/streamdeckapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeckapi-0.0.4.tar", last modified: Thu Jun  1 13:34:52 2023, max compression
+gzip compressed data, was "streamdeckapi-0.0.5.tar", last modified: Thu Jun  1 13:55:30 2023, max compression
```

## Comparing `streamdeckapi-0.0.4.tar` & `streamdeckapi-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/streamdeckapi/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/streamdeckapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/streamdeckapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-01 13:55:21.000000 streamdeckapi-0.0.5/streamdeckapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:55:30.831295 streamdeckapi-0.0.5/streamdeckapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 13:55:30.000000 streamdeckapi-0.0.5/streamdeckapi.egg-info/top_level.txt
```

### Comparing `streamdeckapi-0.0.4/PKG-INFO` & `streamdeckapi-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `streamdeckapi-0.0.4/README.md` & `streamdeckapi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.4/setup.py` & `streamdeckapi-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "Stream Deck API Library"
 
 # Setting up
 setup(
     name="streamdeckapi",
     version=VERSION,
     author="Patrick762",
     author_email="<pip-stream-deck-api@hosting-rt.de>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/Patrick762/streamdeckapi",
     packages=find_packages(),
     install_requires=[
-        "requests==2.28.2",
+        "requests",
         "websockets==11.0.2",
-        "aiohttp==3.8.4",
+        "aiohttp>=3.8",
         "human-readable-ids==0.1.3",
         "jsonpickle==3.0.1",
         "streamdeck==0.9.3",
         "pillow>=9.4.0,<10.0.0",
         "cairosvg==2.7.0",
         "ssdpy==0.4.1",
     ],
```

### Comparing `streamdeckapi-0.0.4/streamdeckapi/api.py` & `streamdeckapi-0.0.5/streamdeckapi/api.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.4/streamdeckapi/server.py` & `streamdeckapi-0.0.5/streamdeckapi/server.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.4/streamdeckapi/tools.py` & `streamdeckapi-0.0.5/streamdeckapi/tools.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.4/streamdeckapi/types.py` & `streamdeckapi-0.0.5/streamdeckapi/types.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.4/streamdeckapi.egg-info/PKG-INFO` & `streamdeckapi-0.0.5/streamdeckapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

