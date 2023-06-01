# Comparing `tmp/autovf-0.0.5.tar.gz` & `tmp/autovf-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autovf-0.0.5.tar", last modified: Thu Jun  1 08:15:17 2023, max compression
+gzip compressed data, was "autovf-0.0.6.tar", last modified: Thu Jun  1 11:24:06 2023, max compression
```

## Comparing `autovf-0.0.5.tar` & `autovf-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 08:15:17.639450 autovf-0.0.5/
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    11356 2023-05-30 14:11:45.000000 autovf-0.0.5/LICENSE
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5821 2023-06-01 08:15:17.639699 autovf-0.0.5/PKG-INFO
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5487 2023-05-30 14:11:45.000000 autovf-0.0.5/README.md
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      386 2023-06-01 08:15:17.642617 autovf-0.0.5/setup.cfg
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1073 2023-05-30 14:34:26.000000 autovf-0.0.5/setup.py
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 08:15:17.512628 autovf-0.0.5/src/
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 08:15:17.587745 autovf-0.0.5/src/autovf/
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)       51 2023-06-01 08:14:28.000000 autovf-0.0.5/src/autovf/__init__.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      319 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/api.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    12318 2023-05-31 16:11:30.000000 autovf-0.0.5/src/autovf/autovf.py
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 08:15:17.638288 autovf-0.0.5/src/autovf/cli/
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      305 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/cli/__init__.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      994 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/cli/autovf.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1300 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/cli/predict.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1658 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/cli/serve.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     4174 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/cli/train.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1297 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/enums.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      225 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/logger.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     2934 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/metrics.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1326 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/params.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     4547 2023-05-30 14:11:45.000000 autovf-0.0.5/src/autovf/predict.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      541 2023-05-31 16:12:48.000000 autovf-0.0.5/src/autovf/schemas.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    15094 2023-05-31 21:08:31.000000 autovf-0.0.5/src/autovf/utils.py
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 08:15:17.598273 autovf-0.0.5/src/autovf.egg-info/
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5821 2023-06-01 08:15:17.000000 autovf-0.0.5/src/autovf.egg-info/PKG-INFO
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      578 2023-06-01 08:15:17.000000 autovf-0.0.5/src/autovf.egg-info/SOURCES.txt
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        1 2023-06-01 08:15:17.000000 autovf-0.0.5/src/autovf.egg-info/dependency_links.txt
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)       50 2023-06-01 08:15:17.000000 autovf-0.0.5/src/autovf.egg-info/entry_points.txt
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      187 2023-06-01 08:15:17.000000 autovf-0.0.5/src/autovf.egg-info/requires.txt
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        7 2023-06-01 08:15:17.000000 autovf-0.0.5/src/autovf.egg-info/top_level.txt
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 11:24:06.593871 autovf-0.0.6/
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    11356 2023-05-30 14:11:45.000000 autovf-0.0.6/LICENSE
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5821 2023-06-01 11:24:06.594205 autovf-0.0.6/PKG-INFO
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5487 2023-05-30 14:11:45.000000 autovf-0.0.6/README.md
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      386 2023-06-01 11:24:06.598591 autovf-0.0.6/setup.cfg
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1073 2023-05-30 14:34:26.000000 autovf-0.0.6/setup.py
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 11:24:06.421598 autovf-0.0.6/src/
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 11:24:06.529573 autovf-0.0.6/src/autovf/
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)       51 2023-06-01 11:21:58.000000 autovf-0.0.6/src/autovf/__init__.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      319 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/api.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    12318 2023-05-31 16:11:30.000000 autovf-0.0.6/src/autovf/autovf.py
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 11:24:06.592265 autovf-0.0.6/src/autovf/cli/
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      305 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/cli/__init__.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      994 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/cli/autovf.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1300 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/cli/predict.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1658 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/cli/serve.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     4174 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/cli/train.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1297 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/enums.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      225 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/logger.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     2934 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/metrics.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1326 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/params.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     4547 2023-05-30 14:11:45.000000 autovf-0.0.6/src/autovf/predict.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      541 2023-05-31 16:12:48.000000 autovf-0.0.6/src/autovf/schemas.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    15094 2023-06-01 11:21:24.000000 autovf-0.0.6/src/autovf/utils.py
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-06-01 11:24:06.550740 autovf-0.0.6/src/autovf.egg-info/
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5821 2023-06-01 11:24:06.000000 autovf-0.0.6/src/autovf.egg-info/PKG-INFO
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      578 2023-06-01 11:24:06.000000 autovf-0.0.6/src/autovf.egg-info/SOURCES.txt
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        1 2023-06-01 11:24:06.000000 autovf-0.0.6/src/autovf.egg-info/dependency_links.txt
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)       50 2023-06-01 11:24:06.000000 autovf-0.0.6/src/autovf.egg-info/entry_points.txt
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      187 2023-06-01 11:24:06.000000 autovf-0.0.6/src/autovf.egg-info/requires.txt
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        7 2023-06-01 11:24:06.000000 autovf-0.0.6/src/autovf.egg-info/top_level.txt
```

### Comparing `autovf-0.0.5/LICENSE` & `autovf-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/PKG-INFO` & `autovf-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autovf
-Version: 0.0.5
+Version: 0.0.6
 Summary: autovf: tuning xgboost with optuna
 Home-page: https://github.com/alicabukel/autovf
 Author: Ali Cabukel
 Author-email: alicabukel@proton.me
 License: Apache 2.0
 Platform: linux
 Platform: unix
```

### Comparing `autovf-0.0.5/README.md` & `autovf-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/setup.py` & `autovf-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/autovf.py` & `autovf-0.0.6/src/autovf/autovf.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/cli/autovf.py` & `autovf-0.0.6/src/autovf/cli/autovf.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/cli/predict.py` & `autovf-0.0.6/src/autovf/cli/predict.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/cli/serve.py` & `autovf-0.0.6/src/autovf/cli/serve.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/cli/train.py` & `autovf-0.0.6/src/autovf/cli/train.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/enums.py` & `autovf-0.0.6/src/autovf/enums.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/metrics.py` & `autovf-0.0.6/src/autovf/metrics.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/params.py` & `autovf-0.0.6/src/autovf/params.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/predict.py` & `autovf-0.0.6/src/autovf/predict.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/schemas.py` & `autovf-0.0.6/src/autovf/schemas.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.5/src/autovf/utils.py` & `autovf-0.0.6/src/autovf/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
         if model_config.project_name is not None and model_config.project_location is not None:
             aiplatform.init(
                 experiment=model_config.output,
                 project=model_config.project_name,
                 location=model_config.project_location,
             )
-            aiplatform.start_run(run=f"study_{int(time.time())}")
+            aiplatform.start_run(run=f"study-{int(time.time())}")
             params = model.get_params()
             param_keys = [
                 "booster",
                 "colsample_bylevel",
                 "colsample_bynode",
                 "colsample_bytree",
                 "gamma",
```

### Comparing `autovf-0.0.5/src/autovf.egg-info/PKG-INFO` & `autovf-0.0.6/src/autovf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autovf
-Version: 0.0.5
+Version: 0.0.6
 Summary: autovf: tuning xgboost with optuna
 Home-page: https://github.com/alicabukel/autovf
 Author: Ali Cabukel
 Author-email: alicabukel@proton.me
 License: Apache 2.0
 Platform: linux
 Platform: unix
```

### Comparing `autovf-0.0.5/src/autovf.egg-info/SOURCES.txt` & `autovf-0.0.6/src/autovf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

