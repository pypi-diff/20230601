# Comparing `tmp/fse.torii-1.0.2.tar.gz` & `tmp/fse.torii-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fse.torii-1.0.2.tar", last modified: Thu Jun  1 16:47:03 2023, max compression
+gzip compressed data, was "dist/fse.torii-1.0.3.tar", last modified: Thu Jun  1 17:07:38 2023, max compression
```

## Comparing `fse.torii-1.0.2.tar` & `fse.torii-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 16:47:02.000000 fse.torii-1.0.2/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      144 2023-06-01 16:47:02.000000 fse.torii-1.0.2/PKG-INFO
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 16:47:02.000000 fse.torii-1.0.2/fse.torii.egg-info/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      144 2023-06-01 16:47:01.000000 fse.torii-1.0.2/fse.torii.egg-info/PKG-INFO
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      967 2023-06-01 16:47:02.000000 fse.torii-1.0.2/fse.torii.egg-info/SOURCES.txt
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)        1 2023-06-01 16:47:01.000000 fse.torii-1.0.2/fse.torii.egg-info/dependency_links.txt
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)       55 2023-06-01 16:47:02.000000 fse.torii-1.0.2/fse.torii.egg-info/requires.txt
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)        6 2023-06-01 16:47:02.000000 fse.torii-1.0.2/fse.torii.egg-info/top_level.txt
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)       38 2023-06-01 16:47:02.000000 fse.torii-1.0.2/setup.cfg
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      351 2023-06-01 16:30:24.000000 fse.torii-1.0.2/setup.py
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 16:47:02.000000 fse.torii-1.0.2/torii/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      176 2022-03-31 12:08:35.000000 fse.torii-1.0.2/torii/__init__.py
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 16:47:02.000000 fse.torii-1.0.2/torii/data/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      483 2022-03-31 12:08:35.000000 fse.torii-1.0.2/torii/data/__init__.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3291 2022-03-31 12:08:35.000000 fse.torii-1.0.2/torii/data/application.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3600 2023-06-01 16:20:57.000000 fse.torii-1.0.2/torii/data/business_object.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2602 2022-03-31 12:08:35.000000 fse.torii-1.0.2/torii/data/cluster.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2204 2022-03-31 12:08:35.000000 fse.torii-1.0.2/torii/data/picom.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      227 2022-03-31 12:08:35.000000 fse.torii-1.0.2/torii/data/record.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    10680 2023-04-03 15:45:31.000000 fse.torii-1.0.2/torii/data/struct.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    12716 2022-03-31 12:08:35.000000 fse.torii-1.0.2/torii/data/task.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3906 2023-04-03 15:45:31.000000 fse.torii-1.0.2/torii/data/torii_object.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      209 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/exception.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      497 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/generate_doc.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      401 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/generate_pythonApi_doc.py
-drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 16:47:02.000000 fse.torii-1.0.2/torii/services/
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      943 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/__init__.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3894 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/addon_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3374 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/ai_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    24318 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/application_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      403 2023-04-03 15:45:31.000000 fse.torii-1.0.2/torii/services/bo_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     1874 2023-04-03 15:45:31.000000 fse.torii-1.0.2/torii/services/bs_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     4785 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/file_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      904 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/graph_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      476 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/organisation_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)      333 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/picom_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2890 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/profile_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     6265 2023-04-03 15:45:31.000000 fse.torii-1.0.2/torii/services/service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3589 2023-06-01 16:20:57.000000 fse.torii-1.0.2/torii/services/session_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    11633 2022-03-31 12:08:38.000000 fse.torii-1.0.2/torii/services/task_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    16406 2023-04-03 15:45:31.000000 fse.torii-1.0.2/torii/services/torii_service.py
--rw-rw----   0 sylvain  (1000013) rnd      (1000001)    17521 2023-04-03 15:45:31.000000 fse.torii-1.0.2/torii/torii_main.py
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:07:37.000000 fse.torii-1.0.3/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      144 2023-06-01 17:07:37.000000 fse.torii-1.0.3/PKG-INFO
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:07:37.000000 fse.torii-1.0.3/fse.torii.egg-info/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      144 2023-06-01 17:07:37.000000 fse.torii-1.0.3/fse.torii.egg-info/PKG-INFO
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      967 2023-06-01 17:07:37.000000 fse.torii-1.0.3/fse.torii.egg-info/SOURCES.txt
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)        1 2023-06-01 17:07:37.000000 fse.torii-1.0.3/fse.torii.egg-info/dependency_links.txt
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)       55 2023-06-01 17:07:37.000000 fse.torii-1.0.3/fse.torii.egg-info/requires.txt
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)        6 2023-06-01 17:07:37.000000 fse.torii-1.0.3/fse.torii.egg-info/top_level.txt
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)       38 2023-06-01 17:07:37.000000 fse.torii-1.0.3/setup.cfg
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      371 2023-06-01 17:07:21.000000 fse.torii-1.0.3/setup.py
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:07:37.000000 fse.torii-1.0.3/torii/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      176 2022-03-31 12:08:35.000000 fse.torii-1.0.3/torii/__init__.py
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:07:37.000000 fse.torii-1.0.3/torii/data/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      483 2022-03-31 12:08:35.000000 fse.torii-1.0.3/torii/data/__init__.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3291 2022-03-31 12:08:35.000000 fse.torii-1.0.3/torii/data/application.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3600 2023-06-01 16:20:57.000000 fse.torii-1.0.3/torii/data/business_object.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2602 2022-03-31 12:08:35.000000 fse.torii-1.0.3/torii/data/cluster.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2204 2022-03-31 12:08:35.000000 fse.torii-1.0.3/torii/data/picom.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      227 2022-03-31 12:08:35.000000 fse.torii-1.0.3/torii/data/record.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    10680 2023-04-03 15:45:31.000000 fse.torii-1.0.3/torii/data/struct.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    12716 2022-03-31 12:08:35.000000 fse.torii-1.0.3/torii/data/task.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3906 2023-04-03 15:45:31.000000 fse.torii-1.0.3/torii/data/torii_object.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      209 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/exception.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      497 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/generate_doc.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      401 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/generate_pythonApi_doc.py
+drwxrwx---   0 sylvain  (1000013) rnd      (1000001)        0 2023-06-01 17:07:37.000000 fse.torii-1.0.3/torii/services/
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      943 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/__init__.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3894 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/addon_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3374 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/ai_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    24318 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/application_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      403 2023-04-03 15:45:31.000000 fse.torii-1.0.3/torii/services/bo_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     1874 2023-04-03 15:45:31.000000 fse.torii-1.0.3/torii/services/bs_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     4785 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/file_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      904 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/graph_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      476 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/organisation_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)      333 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/picom_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     2890 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/profile_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     6265 2023-04-03 15:45:31.000000 fse.torii-1.0.3/torii/services/service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)     3589 2023-06-01 16:20:57.000000 fse.torii-1.0.3/torii/services/session_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    11633 2022-03-31 12:08:38.000000 fse.torii-1.0.3/torii/services/task_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    16406 2023-04-03 15:45:31.000000 fse.torii-1.0.3/torii/services/torii_service.py
+-rw-rw----   0 sylvain  (1000013) rnd      (1000001)    17521 2023-04-03 15:45:31.000000 fse.torii-1.0.3/torii/torii_main.py
```

### Comparing `fse.torii-1.0.2/fse.torii.egg-info/SOURCES.txt` & `fse.torii-1.0.3/fse.torii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/data/application.py` & `fse.torii-1.0.3/torii/data/application.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/data/business_object.py` & `fse.torii-1.0.3/torii/data/business_object.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/data/cluster.py` & `fse.torii-1.0.3/torii/data/cluster.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/data/picom.py` & `fse.torii-1.0.3/torii/data/picom.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/data/struct.py` & `fse.torii-1.0.3/torii/data/struct.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/data/task.py` & `fse.torii-1.0.3/torii/data/task.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/data/torii_object.py` & `fse.torii-1.0.3/torii/data/torii_object.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/__init__.py` & `fse.torii-1.0.3/torii/services/__init__.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/addon_service.py` & `fse.torii-1.0.3/torii/services/addon_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/ai_service.py` & `fse.torii-1.0.3/torii/services/ai_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/application_service.py` & `fse.torii-1.0.3/torii/services/application_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/bs_service.py` & `fse.torii-1.0.3/torii/services/bs_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/file_service.py` & `fse.torii-1.0.3/torii/services/file_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/graph_service.py` & `fse.torii-1.0.3/torii/services/graph_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/profile_service.py` & `fse.torii-1.0.3/torii/services/profile_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/service.py` & `fse.torii-1.0.3/torii/services/service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/session_service.py` & `fse.torii-1.0.3/torii/services/session_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/task_service.py` & `fse.torii-1.0.3/torii/services/task_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/services/torii_service.py` & `fse.torii-1.0.3/torii/services/torii_service.py`

 * *Files identical despite different names*

### Comparing `fse.torii-1.0.2/torii/torii_main.py` & `fse.torii-1.0.3/torii/torii_main.py`

 * *Files identical despite different names*

