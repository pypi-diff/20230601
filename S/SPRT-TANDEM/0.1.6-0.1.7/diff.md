# Comparing `tmp/SPRT-TANDEM-0.1.6.tar.gz` & `tmp/SPRT-TANDEM-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPRT-TANDEM-0.1.6.tar", last modified: Wed May 31 23:47:55 2023, max compression
+gzip compressed data, was "SPRT-TANDEM-0.1.7.tar", last modified: Thu Jun  1 00:12:04 2023, max compression
```

## Comparing `SPRT-TANDEM-0.1.6.tar` & `SPRT-TANDEM-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.950892 SPRT-TANDEM-0.1.6/
--rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.6/LICENSE
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/PKG-INFO
--rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/README.md
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/PKG-INFO
--rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/SOURCES.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/dependency_links.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       35 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/requires.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/top_level.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 23:47:55.950892 SPRT-TANDEM-0.1.6/setup.cfg
--rw-r--r--   0 afe       (1000) afe       (1000)     1175 2023-05-31 23:47:49.000000 SPRT-TANDEM-0.1.6/setup.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/
--rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/config/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/config/__init__.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/config/config_definition.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/data/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/data/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/models/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/models/__init__.py
--rw-r--r--   0 afe       (1000) afe       (1000)    14098 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/models/losses.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)     1417 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/models/optimizers.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/models/temporal_integrators.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)     2822 2023-05-31 23:37:43.000000 SPRT-TANDEM-0.1.6/tandem/sprt_tandem_main.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/utils/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/__init__.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)     6340 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/checkpoint.py
--rw-r--r--   0 afe       (1000) afe       (1000)    22639 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/data_processing.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/hyperparameter_tuning.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    24962 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/logging.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    20082 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/misc.py
--rw-r--r--   0 afe       (1000) afe       (1000)    49601 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/performance_metrics.py
--rw-r--r--   0 afe       (1000) afe       (1000)    10210 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/training.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/
+-rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.7/LICENSE
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/PKG-INFO
+-rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/README.md
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/SPRT_TANDEM.egg-info/
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-06-01 00:12:04.000000 SPRT-TANDEM-0.1.7/SPRT_TANDEM.egg-info/PKG-INFO
+-rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-06-01 00:12:04.000000 SPRT-TANDEM-0.1.7/SPRT_TANDEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-06-01 00:12:04.000000 SPRT-TANDEM-0.1.7/SPRT_TANDEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       35 2023-06-01 00:12:04.000000 SPRT-TANDEM-0.1.7/SPRT_TANDEM.egg-info/requires.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-06-01 00:12:04.000000 SPRT-TANDEM-0.1.7/SPRT_TANDEM.egg-info/top_level.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/setup.cfg
+-rw-r--r--   0 afe       (1000) afe       (1000)     1175 2023-06-01 00:11:56.000000 SPRT-TANDEM-0.1.7/setup.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/tandem/
+-rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/tandem/config/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/config/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 23:55:31.000000 SPRT-TANDEM-0.1.7/tandem/config/config_definition.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/tandem/data/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/data/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/tandem/models/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/models/__init__.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    14098 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/models/losses.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     1417 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/models/optimizers.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/models/temporal_integrators.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     2822 2023-05-31 23:37:43.000000 SPRT-TANDEM-0.1.7/tandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:12:04.419294 SPRT-TANDEM-0.1.7/tandem/utils/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/utils/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     6340 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/utils/checkpoint.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    22639 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/utils/data_processing.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/utils/hyperparameter_tuning.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    24962 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/utils/logging.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    20082 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/utils/misc.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    49601 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/utils/performance_metrics.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    10210 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.7/tandem/utils/training.py
```

### Comparing `SPRT-TANDEM-0.1.6/LICENSE` & `SPRT-TANDEM-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/PKG-INFO` & `SPRT-TANDEM-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.6
+Version: 0.1.7
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.6/README.md` & `SPRT-TANDEM-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/PKG-INFO` & `SPRT-TANDEM-0.1.7/SPRT_TANDEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.6
+Version: 0.1.7
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/SOURCES.txt` & `SPRT-TANDEM-0.1.7/SPRT_TANDEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/setup.py` & `SPRT-TANDEM-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(
     path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
 ) as f:
     long_description = f.read()
 
 setup(
     name="SPRT-TANDEM",
-    version="0.1.6",
+    version="0.1.7",
     license="MIT",
     description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.",
     author="Akinori F. Ebihara",
     author_email="aebihara@nec.com",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `SPRT-TANDEM-0.1.6/tandem/config/config_definition.py` & `SPRT-TANDEM-0.1.7/tandem/config/config_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 REPRODUCE_TRIAL = False  # 'best', trial index (int) or False
 # Load pretrained weight from .pt file specified below.
 IS_RESUME = False
 SUBPROJECT_TO_RESUME = "_20230330_214519224/ckpt_step3500_target_ausat_confmx0.0011.pt"
 
 # of frequent use
 GPU = 0
-BATCH_SIZE = 150
+BATCH_SIZE = 100
 NUM_TRIALS = 1000
 NUM_EPOCHS = 10
 NUM_ITER = NUM_EPOCHS * NUM_TRAIN // BATCH_SIZE  # e.g., 20 * 25000 // 100 = 5000
 TRAIN_DISPLAY_STEP = 250
 VALIDATION_STEP = 250
 # hyperband, median, percentile, etc... set to 'none' if no pruner is needed.
 PRUNER_NAME = "percentile"
```

### Comparing `SPRT-TANDEM-0.1.6/tandem/models/losses.py` & `SPRT-TANDEM-0.1.7/tandem/models/losses.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/models/optimizers.py` & `SPRT-TANDEM-0.1.7/tandem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/models/temporal_integrators.py` & `SPRT-TANDEM-0.1.7/tandem/models/temporal_integrators.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/sprt_tandem_main.py` & `SPRT-TANDEM-0.1.7/tandem/sprt_tandem_main.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/utils/checkpoint.py` & `SPRT-TANDEM-0.1.7/tandem/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/utils/data_processing.py` & `SPRT-TANDEM-0.1.7/tandem/utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/utils/hyperparameter_tuning.py` & `SPRT-TANDEM-0.1.7/tandem/utils/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/utils/logging.py` & `SPRT-TANDEM-0.1.7/tandem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/utils/misc.py` & `SPRT-TANDEM-0.1.7/tandem/utils/misc.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/utils/performance_metrics.py` & `SPRT-TANDEM-0.1.7/tandem/utils/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.6/tandem/utils/training.py` & `SPRT-TANDEM-0.1.7/tandem/utils/training.py`

 * *Files identical despite different names*

