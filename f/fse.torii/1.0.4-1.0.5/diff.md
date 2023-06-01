# Comparing `tmp/fse.torii-1.0.4.tar.gz` & `tmp/fse.torii-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse.torii-1.0.4.tar", last modified: Thu Jun  1 17:35:16 2023, max compression
+gzip compressed data, was "dist/fse.torii-1.0.5.tar", last modified: Thu Jun  1 17:42:01 2023, max compression
```

## Comparing `fse.torii-1.0.4.tar` & `fse.torii-1.0.5.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:35:16.217367 fse.torii-1.0.4/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      196 2023-06-01 17:35:16.218367 fse.torii-1.0.4/PKG-INFO
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      371 2023-06-01 17:34:16.783369 fse.torii-1.0.4/setup.py
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:35:16.202367 fse.torii-1.0.4/torii/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      152 2023-06-01 17:23:07.541388 fse.torii-1.0.4/torii/__init__.py
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:35:16.207367 fse.torii-1.0.4/torii/data/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      483 2022-03-31 12:08:35.209393 fse.torii-1.0.4/torii/data/__init__.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3291 2022-03-31 12:08:35.212393 fse.torii-1.0.4/torii/data/application.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3600 2023-06-01 16:20:57.784497 fse.torii-1.0.4/torii/data/business_object.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2602 2022-03-31 12:08:35.215393 fse.torii-1.0.4/torii/data/cluster.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2204 2022-03-31 12:08:35.217393 fse.torii-1.0.4/torii/data/picom.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      227 2022-03-31 12:08:35.219393 fse.torii-1.0.4/torii/data/record.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    10680 2023-04-03 15:45:31.915559 fse.torii-1.0.4/torii/data/struct.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    12716 2022-03-31 12:08:35.223393 fse.torii-1.0.4/torii/data/task.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3906 2023-04-03 15:45:31.917559 fse.torii-1.0.4/torii/data/torii_object.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      209 2022-03-31 12:08:38.854393 fse.torii-1.0.4/torii/exception.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      497 2022-03-31 12:08:38.868393 fse.torii-1.0.4/torii/generate_doc.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      401 2022-03-31 12:08:38.869393 fse.torii-1.0.4/torii/generate_pythonApi_doc.py
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:35:16.217367 fse.torii-1.0.4/torii/services/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      943 2022-03-31 12:08:38.900393 fse.torii-1.0.4/torii/services/__init__.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3894 2022-03-31 12:08:38.901393 fse.torii-1.0.4/torii/services/addon_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3374 2022-03-31 12:08:38.903393 fse.torii-1.0.4/torii/services/ai_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    24318 2022-03-31 12:08:38.905393 fse.torii-1.0.4/torii/services/application_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      403 2023-04-03 15:45:31.921559 fse.torii-1.0.4/torii/services/bo_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     1874 2023-04-03 15:45:31.923559 fse.torii-1.0.4/torii/services/bs_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     4785 2022-03-31 12:08:38.909393 fse.torii-1.0.4/torii/services/file_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      904 2022-03-31 12:08:38.911393 fse.torii-1.0.4/torii/services/graph_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      476 2022-03-31 12:08:38.913393 fse.torii-1.0.4/torii/services/organisation_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      333 2022-03-31 12:08:38.914393 fse.torii-1.0.4/torii/services/picom_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2890 2022-03-31 12:08:38.916393 fse.torii-1.0.4/torii/services/profile_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     6265 2023-04-03 15:45:31.929559 fse.torii-1.0.4/torii/services/service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3589 2023-06-01 16:20:57.785497 fse.torii-1.0.4/torii/services/session_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    11633 2022-03-31 12:08:38.922393 fse.torii-1.0.4/torii/services/task_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    16406 2023-04-03 15:45:31.933559 fse.torii-1.0.4/torii/services/torii_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    17521 2023-04-03 15:45:31.935559 fse.torii-1.0.4/torii/torii_main.py
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:42:00.000000 fse.torii-1.0.5/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      144 2023-06-01 17:42:00.000000 fse.torii-1.0.5/PKG-INFO
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:42:00.000000 fse.torii-1.0.5/fse.torii.egg-info/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      144 2023-06-01 17:41:59.000000 fse.torii-1.0.5/fse.torii.egg-info/PKG-INFO
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      967 2023-06-01 17:42:00.000000 fse.torii-1.0.5/fse.torii.egg-info/SOURCES.txt
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)        1 2023-06-01 17:41:59.000000 fse.torii-1.0.5/fse.torii.egg-info/dependency_links.txt
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)       55 2023-06-01 17:42:00.000000 fse.torii-1.0.5/fse.torii.egg-info/requires.txt
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)        6 2023-06-01 17:42:00.000000 fse.torii-1.0.5/fse.torii.egg-info/top_level.txt
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)       38 2023-06-01 17:42:00.000000 fse.torii-1.0.5/setup.cfg
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      371 2023-06-01 17:40:56.000000 fse.torii-1.0.5/setup.py
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:42:00.000000 fse.torii-1.0.5/torii/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      135 2023-06-01 17:39:13.000000 fse.torii-1.0.5/torii/__init__.py
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:42:00.000000 fse.torii-1.0.5/torii/data/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      483 2022-03-31 12:08:35.000000 fse.torii-1.0.5/torii/data/__init__.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3291 2022-03-31 12:08:35.000000 fse.torii-1.0.5/torii/data/application.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3600 2023-06-01 16:20:57.000000 fse.torii-1.0.5/torii/data/business_object.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2602 2022-03-31 12:08:35.000000 fse.torii-1.0.5/torii/data/cluster.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2204 2022-03-31 12:08:35.000000 fse.torii-1.0.5/torii/data/picom.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      227 2022-03-31 12:08:35.000000 fse.torii-1.0.5/torii/data/record.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    10680 2023-04-03 15:45:31.000000 fse.torii-1.0.5/torii/data/struct.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    12716 2022-03-31 12:08:35.000000 fse.torii-1.0.5/torii/data/task.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3906 2023-04-03 15:45:31.000000 fse.torii-1.0.5/torii/data/torii_object.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      209 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/exception.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      497 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/generate_doc.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      401 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/generate_pythonApi_doc.py
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:42:00.000000 fse.torii-1.0.5/torii/services/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      943 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/__init__.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3894 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/addon_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3374 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/ai_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    24318 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/application_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      403 2023-04-03 15:45:31.000000 fse.torii-1.0.5/torii/services/bo_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     1874 2023-04-03 15:45:31.000000 fse.torii-1.0.5/torii/services/bs_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     4785 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/file_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      904 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/graph_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      476 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/organisation_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      333 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/picom_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2890 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/profile_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     6265 2023-04-03 15:45:31.000000 fse.torii-1.0.5/torii/services/service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3589 2023-06-01 16:20:57.000000 fse.torii-1.0.5/torii/services/session_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    11633 2022-03-31 12:08:38.000000 fse.torii-1.0.5/torii/services/task_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    16406 2023-04-03 15:45:31.000000 fse.torii-1.0.5/torii/services/torii_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    17521 2023-04-03 15:45:31.000000 fse.torii-1.0.5/torii/torii_main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `fse.torii-1.0.4/torii/data/application.py` & `fse.torii-1.0.5/torii/data/application.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/data/business_object.py` & `fse.torii-1.0.5/torii/data/business_object.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/data/cluster.py` & `fse.torii-1.0.5/torii/data/cluster.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/data/picom.py` & `fse.torii-1.0.5/torii/data/picom.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/data/struct.py` & `fse.torii-1.0.5/torii/data/struct.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/data/task.py` & `fse.torii-1.0.5/torii/data/task.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/data/torii_object.py` & `fse.torii-1.0.5/torii/data/torii_object.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/__init__.py` & `fse.torii-1.0.5/torii/services/__init__.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/addon_service.py` & `fse.torii-1.0.5/torii/services/addon_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/ai_service.py` & `fse.torii-1.0.5/torii/services/ai_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/application_service.py` & `fse.torii-1.0.5/torii/services/application_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/bs_service.py` & `fse.torii-1.0.5/torii/services/bs_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/file_service.py` & `fse.torii-1.0.5/torii/services/file_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/graph_service.py` & `fse.torii-1.0.5/torii/services/graph_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/profile_service.py` & `fse.torii-1.0.5/torii/services/profile_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/service.py` & `fse.torii-1.0.5/torii/services/service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/session_service.py` & `fse.torii-1.0.5/torii/services/session_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/task_service.py` & `fse.torii-1.0.5/torii/services/task_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/services/torii_service.py` & `fse.torii-1.0.5/torii/services/torii_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.4/torii/torii_main.py` & `fse.torii-1.0.5/torii/torii_main.py`

 * *Files identical despite different names*

