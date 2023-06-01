# Comparing `tmp/streamdeckapi-0.0.3.tar.gz` & `tmp/streamdeckapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeckapi-0.0.3.tar", last modified: Wed May 24 17:02:51 2023, max compression
+gzip compressed data, was "streamdeckapi-0.0.4.tar", last modified: Thu Jun  1 13:34:52 2023, max compression
```

## Comparing `streamdeckapi-0.0.3.tar` & `streamdeckapi-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:02:51.712803 streamdeckapi-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-24 17:02:51.712803 streamdeckapi-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-24 17:02:38.000000 streamdeckapi-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:02:51.712803 streamdeckapi-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-24 17:02:38.000000 streamdeckapi-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:02:51.712803 streamdeckapi-0.0.3/streamdeckapi/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 17:02:38.000000 streamdeckapi-0.0.3/streamdeckapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-05-24 17:02:38.000000 streamdeckapi-0.0.3/streamdeckapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 17:02:38.000000 streamdeckapi-0.0.3/streamdeckapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-05-24 17:02:38.000000 streamdeckapi-0.0.3/streamdeckapi/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-24 17:02:38.000000 streamdeckapi-0.0.3/streamdeckapi/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-24 17:02:38.000000 streamdeckapi-0.0.3/streamdeckapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:02:51.712803 streamdeckapi-0.0.3/streamdeckapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-24 17:02:51.000000 streamdeckapi-0.0.3/streamdeckapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 17:02:51.000000 streamdeckapi-0.0.3/streamdeckapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:02:51.000000 streamdeckapi-0.0.3/streamdeckapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-24 17:02:51.000000 streamdeckapi-0.0.3/streamdeckapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 17:02:51.000000 streamdeckapi-0.0.3/streamdeckapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 17:02:51.000000 streamdeckapi-0.0.3/streamdeckapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/streamdeckapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-01 13:34:41.000000 streamdeckapi-0.0.4/streamdeckapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:52.485369 streamdeckapi-0.0.4/streamdeckapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 13:34:52.000000 streamdeckapi-0.0.4/streamdeckapi.egg-info/top_level.txt
```

### Comparing `streamdeckapi-0.0.3/PKG-INFO` & `streamdeckapi-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `streamdeckapi-0.0.3/README.md` & `streamdeckapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.3/setup.py` & `streamdeckapi-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "Stream Deck API Library"
 
 # Setting up
 setup(
     name="streamdeckapi",
     version=VERSION,
     author="Patrick762",
```

### Comparing `streamdeckapi-0.0.3/streamdeckapi/api.py` & `streamdeckapi-0.0.4/streamdeckapi/api.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.3/streamdeckapi/server.py` & `streamdeckapi-0.0.4/streamdeckapi/server.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.3/streamdeckapi/tools.py` & `streamdeckapi-0.0.4/streamdeckapi/tools.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.3/streamdeckapi/types.py` & `streamdeckapi-0.0.4/streamdeckapi/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,19 +75,20 @@
         self.position = SDButtonPosition(obj["position"])
 
 
 class SDInfo(dict):
     """Stream Deck Info Type."""
 
     application: SDApplication
-    devices: list[SDDevice] = []
-    buttons: dict[str, SDButton] = {}
 
     def __init__(self, obj: dict) -> None:
         """Init Stream Deck Info object."""
+        self.devices: list[SDDevice] = []
+        self.buttons: dict[str, SDButton] = {}
+
         dict.__init__(self, obj)
         self.application = SDApplication(obj["application"])
         for device in obj["devices"]:
             self.devices.append(SDDevice(device))
         for _id in obj["buttons"]:
             self.buttons.update({_id: SDButton(obj["buttons"][_id])})
```

### Comparing `streamdeckapi-0.0.3/streamdeckapi.egg-info/PKG-INFO` & `streamdeckapi-0.0.4/streamdeckapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

