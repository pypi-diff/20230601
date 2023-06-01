# Comparing `tmp/hcai-nova-server-nightly-0.1.7.dev202305310956.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.7.dev202305311442.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.7.dev202305310956.tar", last modified: Wed May 31 09:56:52 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.7.dev202305311442.tar", last modified: Wed May 31 14:42:46 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956.tar` & `hcai-nova-server-nightly-0.1.7.dev202305311442.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:52.052613 hcai-nova-server-nightly-0.1.7.dev202305310956/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-31 09:56:52.052613 hcai-nova-server-nightly-0.1.7.dev202305310956/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:52.048613 hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-31 09:56:51.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-31 09:56:52.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 09:56:51.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-31 09:56:51.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-31 09:56:51.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-31 09:56:51.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:52.052613 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:52.052613 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9863 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:52.052613 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:52.052613 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    13770 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 09:56:52.052613 hcai-nova-server-nightly-0.1.7.dev202305310956/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-05-31 09:56:39.000000 hcai-nova-server-nightly-0.1.7.dev202305310956/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:46.595945 hcai-nova-server-nightly-0.1.7.dev202305311442/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-31 14:42:46.595945 hcai-nova-server-nightly-0.1.7.dev202305311442/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:46.595945 hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-31 14:42:46.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-31 14:42:46.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 14:42:46.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-31 14:42:46.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-31 14:42:46.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-31 14:42:46.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:46.595945 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:46.595945 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9863 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:46.595945 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:46.595945 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 14:42:46.595945 hcai-nova-server-nightly-0.1.7.dev202305311442/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-05-31 14:42:35.000000 hcai-nova-server-nightly-0.1.7.dev202305311442/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/PKG-INFO` & `hcai-nova-server-nightly-0.1.7.dev202305311442/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.7.dev202305310956
+Version: 0.1.7.dev202305311442
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.7.dev202305310956
+Version: 0.1.7.dev202305311442
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.7.dev202305311442/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/app.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/app.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/predict.py`

 * *Files 13% similar despite different names*

```diff
@@ -130,27 +130,25 @@
         annos = predictor.to_anno(data)
         logger.info("...done")
 
         logger.info("Saving predictions to database...")
 
         # TODO: Refactor to not use request form in upload
         request_form_copy = copy.copy(request_form)
-        request_form_copy['scheme'] = 'activelistening'
-
         assert len(ss_ds_iter.sessions) == 1
         request_form_copy['sessions'] = ss_ds_iter.sessions[0]
-        request_form_copy['roles'] = ss_ds_iter.roles[0]
 
         for anno in annos:
             db_utils.write_annotation_to_db(request_form_copy, anno, logger)
         logger.info("...done")
 
     logger.info("Prediction completed!")
     status_utils.update_status(key, status_utils.JobStatus.FINISHED)
 
+'''Keep for later reference to implement polygons'''
     # model_script.ds_iter = ds_iter
     # model_script.request_form["sessions"] = session
     # model_script.request_form["roles"] = role
     #
     # logger.info("Execute preprocessing.")
     # model_script.preprocess()
     # logger.info("Preprocessing done.")
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305310956/setup.py` & `hcai-nova-server-nightly-0.1.7.dev202305311442/setup.py`

 * *Files identical despite different names*

