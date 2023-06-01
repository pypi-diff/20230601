# Comparing `tmp/JustDeepIt-0.1.29.tar.gz` & `tmp/JustDeepIt-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustDeepIt-0.1.29.tar", last modified: Wed May 31 04:20:12 2023, max compression
+gzip compressed data, was "JustDeepIt-0.1.30.tar", last modified: Thu Jun  1 07:11:18 2023, max compression
```

## Comparing `JustDeepIt-0.1.29.tar` & `JustDeepIt-0.1.30.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.522696 JustDeepIt-0.1.29/JustDeepIt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.522696 JustDeepIt-0.1.29/justdeepit/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.522696 JustDeepIt-0.1.29/justdeepit/models/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/object_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.526696 JustDeepIt-0.1.29/justdeepit/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/detectron2base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.514696 JustDeepIt-0.1.29/justdeepit/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.526696 JustDeepIt-0.1.29/justdeepit/src/font/
--rw-r--r--   0 runner    (1001) docker     (123)   555264 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/src/font/NotoSans-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/src/font/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    56382 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.530696 JustDeepIt-0.1.29/justdeepit/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/appbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/appis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/appod.py
--rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/appsod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/justdeepit/webapp/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/.Rhistory
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/jquery-3.6.0.min.map
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)    58702 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/tree.jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)   174878 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/tree.jquery.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/justdeepit/webapp/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/templates/module.html
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/templates/shutdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.793717 JustDeepIt-0.1.30/JustDeepIt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.793717 JustDeepIt-0.1.30/justdeepit/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.797717 JustDeepIt-0.1.30/justdeepit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/object_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.797717 JustDeepIt-0.1.30/justdeepit/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/detectron2base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.789717 JustDeepIt-0.1.30/justdeepit/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.801717 JustDeepIt-0.1.30/justdeepit/src/font/
+-rw-r--r--   0 runner    (1001) docker     (123)   555264 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    59870 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.805717 JustDeepIt-0.1.30/justdeepit/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/appbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/appis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/appod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/appsod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/justdeepit/webapp/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/.Rhistory
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/jquery-3.6.0.min.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58702 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/tree.jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)   174878 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/tree.jquery.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/justdeepit/webapp/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/templates/module.html
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/templates/shutdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/setup.py
```

### Comparing `JustDeepIt-0.1.29/JustDeepIt.egg-info/PKG-INFO` & `JustDeepIt-0.1.30/JustDeepIt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.1.29
+Version: 0.1.30
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `JustDeepIt-0.1.29/JustDeepIt.egg-info/SOURCES.txt` & `JustDeepIt-0.1.30/JustDeepIt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/LICENSE` & `JustDeepIt-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/PKG-INFO` & `JustDeepIt-0.1.30/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.1.29
+Version: 0.1.30
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `JustDeepIt-0.1.29/README.md` & `JustDeepIt-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/models/instance_segment.py` & `JustDeepIt-0.1.30/justdeepit/models/instance_segment.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/models/object_detect.py` & `JustDeepIt-0.1.30/justdeepit/models/object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/models/salient_object_detect.py` & `JustDeepIt-0.1.30/justdeepit/models/salient_object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/models/utils/detectron2base.py` & `JustDeepIt-0.1.30/justdeepit/models/utils/detectron2base.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/models/utils/mmdetbase.py` & `JustDeepIt-0.1.30/justdeepit/models/utils/mmdetbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/models/utils/u2net.py` & `JustDeepIt-0.1.30/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/models/utils/unet.py` & `JustDeepIt-0.1.30/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/src/font/NotoSans-Medium.ttf` & `JustDeepIt-0.1.30/justdeepit/src/font/NotoSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/src/font/OFL.txt` & `JustDeepIt-0.1.30/justdeepit/src/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/utils.py` & `JustDeepIt-0.1.30/justdeepit/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 import skimage
 import skimage.io
 import skimage.color
 import skimage.measure
 import skimage.draw
 import PIL.Image
 import PIL.ImageOps
+import tempfile
+import pycocotools.coco
+import pycocotools.cocoeval
 
 
 
 class JsonEncoder(json.JSONEncoder):
     """Convert NumPy object to JSON object
     
     Convert NumPy objects to JSON object during writting process.
@@ -1383,9 +1386,124 @@
         
         # save project.vott
             
         # save assets.json
             
 
 
+def __load_json(fpath):
+    with open(fpath) as fh:
+        d = json.load(fh)
+    return d
+
+def __index_common_images(gt_fpath, pred_fpath):
+    # ground truth
+    gt2id = {}
+    d = __load_json(gt_fpath)
+    for im in d['images']:
+        gt2id[os.path.basename(im['file_name'])] = str(im['id'])
+
+    # prediction result
+    pred2id = {}
+    d = __load_json(pred_fpath)
+    for im in d['images']:
+        pred2id[os.path.basename(im['file_name'])] = str(im['id'])
+
+    # common images betweeen groundtruth and prediction reuslt
+    common_images = set(gt2id.keys()) & set(pred2id.keys())
+    im2id = {}
+    for i, common_image in enumerate(sorted(list(common_images))):
+        im2id[common_image] = i + 1
+
+    id2id = {'gt': {}, 'pred': {}}
+    for im_fname, im_id in im2id.items():
+        id2id['gt'][gt2id[im_fname]] = im_id
+        id2id['pred'][pred2id[im_fname]] = im_id
+
+    return id2id
+
+
+def __modify_coco(coco_fpath, id2id):
+    d = __load_json(coco_fpath)
+    d_new = {}
+
+    for coco_key in d.keys():
+        if coco_key == 'images':
+            d_new['images'] = []
+            for x in d['images']:
+                if str(x['id']) in id2id:
+                    x['id'] = id2id[str(x['id'])]
+                    d_new['images'].append(x)
+        elif coco_key == 'annotations':
+            d_new['annotations'] = []
+            for x in d['annotations']:
+                if str(x['image_id']) in id2id:
+                    x['image_id'] = id2id[str(x['image_id'])]
+                    d_new['annotations'].append(x)
+        else:
+            d_new[coco_key] = d[coco_key]
+
+    return d_new
+
+
+
+def __save_json(d, k=None):
+    fd, temp_fpath = tempfile.mkstemp()
+    with open(temp_fpath, 'w') as fh:
+        if k is None:
+            json.dump(d, fh, indent=4)
+        else:
+            json.dump(d[k], fh, indent=4)
+    return temp_fpath
+
+
+
+def coco_eval(gt_fpath, pred_fpath):
+    """Calculate validation scores from inference results
+    
+    This function calculate the validation scores (mAP, mPR) from inference results.
+    This function requires two COCO format files as inputs, one is ground truth and
+    the other is inference result. The image IDs are allowed to be different between
+    two COCO format files, as this function will reindex image IDs according image
+    name between two COCO format files.
+    
+    Args:
+        gt_fpath (str): A path to COCO format file storing the ground truth annotations.
+        pred_fpath (str): A path to COCO format file storing the inference result.
+    
+    Returns:
+        A list contains validation scores.
+    
+    Examples:
+        >>> from justdeepit.utils import coco_eval
+        >>> 
+        >>> scores = coco_eval('gt.coco.json', 'predicted.coco.json')
+        >>> print(scores)
+        
+    """
+
+    id2id = __index_common_images(gt_fpath, pred_fpath)
+    gt_coco_dict = __modify_coco(gt_fpath, id2id['gt'])
+    pred_coco_dict = __modify_coco(pred_fpath, id2id['pred'])
+    gt_coco_fpath = __save_json(gt_coco_dict)
+    pred_coco_fpath = __save_json(pred_coco_dict, 'annotations')
+
+    gt_coco = pycocotools.coco.COCO(gt_coco_fpath)
+    pred_coco = gt_coco.loadRes(pred_coco_fpath)
+    coco_eval = pycocotools.cocoeval.COCOeval(gt_coco, pred_coco, 'bbox')
+    coco_eval.evaluate()
+    coco_eval.accumulate()
+    coco_eval.summarize()
+    
+    os.remove(gt_coco_fpath)
+    os.remove(pred_coco_fpath)
+    
+    return coco_eval.stats
+
+
+
+
+
+
+
```

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/app.py` & `JustDeepIt-0.1.30/justdeepit/webapp/app.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/appbase.py` & `JustDeepIt-0.1.30/justdeepit/webapp/appbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/appis.py` & `JustDeepIt-0.1.30/justdeepit/webapp/appis.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/appod.py` & `JustDeepIt-0.1.30/justdeepit/webapp/appod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/appsod.py` & `JustDeepIt-0.1.30/justdeepit/webapp/appsod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/static/jquery-3.6.0.min.js` & `JustDeepIt-0.1.30/justdeepit/webapp/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/static/jquery-3.6.0.min.map` & `JustDeepIt-0.1.30/justdeepit/webapp/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/static/styles.css` & `JustDeepIt-0.1.30/justdeepit/webapp/static/styles.css`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/static/tree.jquery.js` & `JustDeepIt-0.1.30/justdeepit/webapp/static/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/static/tree.jquery.js.map` & `JustDeepIt-0.1.30/justdeepit/webapp/static/tree.jquery.js.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/static/utils.js` & `JustDeepIt-0.1.30/justdeepit/webapp/static/utils.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/templates/index.html` & `JustDeepIt-0.1.30/justdeepit/webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/templates/module.html` & `JustDeepIt-0.1.30/justdeepit/webapp/templates/module.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/justdeepit/webapp/templates/shutdown.html` & `JustDeepIt-0.1.30/justdeepit/webapp/templates/shutdown.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.29/setup.py` & `JustDeepIt-0.1.30/setup.py`

 * *Files identical despite different names*

