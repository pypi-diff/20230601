# Comparing `tmp/SPRT-TANDEM-0.1.8.tar.gz` & `tmp/SPRT-TANDEM-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPRT-TANDEM-0.1.8.tar", last modified: Thu Jun  1 00:19:47 2023, max compression
+gzip compressed data, was "SPRT-TANDEM-0.1.9.tar", last modified: Thu Jun  1 03:02:45 2023, max compression
```

## Comparing `SPRT-TANDEM-0.1.8.tar` & `SPRT-TANDEM-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/
--rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.8/LICENSE
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/PKG-INFO
--rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/README.md
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/SPRT_TANDEM.egg-info/
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-06-01 00:19:47.000000 SPRT-TANDEM-0.1.8/SPRT_TANDEM.egg-info/PKG-INFO
--rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-06-01 00:19:47.000000 SPRT-TANDEM-0.1.8/SPRT_TANDEM.egg-info/SOURCES.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-06-01 00:19:47.000000 SPRT-TANDEM-0.1.8/SPRT_TANDEM.egg-info/dependency_links.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       35 2023-06-01 00:19:47.000000 SPRT-TANDEM-0.1.8/SPRT_TANDEM.egg-info/requires.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-06-01 00:19:47.000000 SPRT-TANDEM-0.1.8/SPRT_TANDEM.egg-info/top_level.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/setup.cfg
--rw-r--r--   0 afe       (1000) afe       (1000)     1150 2023-06-01 00:19:26.000000 SPRT-TANDEM-0.1.8/setup.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/tandem/
--rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/tandem/config/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/config/__init__.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 23:55:31.000000 SPRT-TANDEM-0.1.8/tandem/config/config_definition.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/tandem/data/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/data/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/tandem/models/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/models/__init__.py
--rw-r--r--   0 afe       (1000) afe       (1000)    14098 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/models/losses.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)     1417 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/models/optimizers.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/models/temporal_integrators.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)     2822 2023-05-31 23:37:43.000000 SPRT-TANDEM-0.1.8/tandem/sprt_tandem_main.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 00:19:47.110714 SPRT-TANDEM-0.1.8/tandem/utils/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/utils/__init__.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)     6340 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/utils/checkpoint.py
--rw-r--r--   0 afe       (1000) afe       (1000)    22639 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/utils/data_processing.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/utils/hyperparameter_tuning.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    24962 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/utils/logging.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    20082 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/utils/misc.py
--rw-r--r--   0 afe       (1000) afe       (1000)    49601 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/utils/performance_metrics.py
--rw-r--r--   0 afe       (1000) afe       (1000)    10210 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.8/tandem/utils/training.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/
+-rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.9/LICENSE
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/PKG-INFO
+-rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/README.md
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/SPRT_TANDEM.egg-info/
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-06-01 03:02:45.000000 SPRT-TANDEM-0.1.9/SPRT_TANDEM.egg-info/PKG-INFO
+-rw-rw-r--   0 afe       (1000) afe       (1000)      743 2023-06-01 03:02:45.000000 SPRT-TANDEM-0.1.9/SPRT_TANDEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-06-01 03:02:45.000000 SPRT-TANDEM-0.1.9/SPRT_TANDEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       35 2023-06-01 03:02:45.000000 SPRT-TANDEM-0.1.9/SPRT_TANDEM.egg-info/requires.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-06-01 03:02:45.000000 SPRT-TANDEM-0.1.9/SPRT_TANDEM.egg-info/top_level.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/setup.cfg
+-rw-r--r--   0 afe       (1000) afe       (1000)     1167 2023-06-01 03:02:31.000000 SPRT-TANDEM-0.1.9/setup.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/tandem/
+-rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/tandem/config/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/config/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 23:55:31.000000 SPRT-TANDEM-0.1.9/tandem/config/config_definition.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/tandem/data/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/data/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/tandem/data/train_10000/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/data/train_10000/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/tandem/data/val_100/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/data/val_100/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/tandem/models/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/models/__init__.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    14098 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/models/losses.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     1417 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/models/optimizers.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/models/temporal_integrators.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     2822 2023-05-31 23:37:43.000000 SPRT-TANDEM-0.1.9/tandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-06-01 03:02:45.339186 SPRT-TANDEM-0.1.9/tandem/utils/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/utils/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     6340 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/utils/checkpoint.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    22639 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/utils/data_processing.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/utils/hyperparameter_tuning.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    24962 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/utils/logging.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    20082 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/utils/misc.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    49601 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/utils/performance_metrics.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    10210 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.9/tandem/utils/training.py
```

### Comparing `SPRT-TANDEM-0.1.8/LICENSE` & `SPRT-TANDEM-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/PKG-INFO` & `SPRT-TANDEM-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.8
+Version: 0.1.9
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.8/README.md` & `SPRT-TANDEM-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/SPRT_TANDEM.egg-info/PKG-INFO` & `SPRT-TANDEM-0.1.9/SPRT_TANDEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.8
+Version: 0.1.9
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.8/SPRT_TANDEM.egg-info/SOURCES.txt` & `SPRT-TANDEM-0.1.9/SPRT_TANDEM.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 SPRT_TANDEM.egg-info/requires.txt
 SPRT_TANDEM.egg-info/top_level.txt
 tandem/__init__.py
 tandem/sprt_tandem_main.py
 tandem/config/__init__.py
 tandem/config/config_definition.py
 tandem/data/__init__.py
+tandem/data/train_10000/__init__.py
+tandem/data/val_100/__init__.py
 tandem/models/__init__.py
 tandem/models/losses.py
 tandem/models/optimizers.py
 tandem/models/temporal_integrators.py
 tandem/utils/__init__.py
 tandem/utils/checkpoint.py
 tandem/utils/data_processing.py
```

### Comparing `SPRT-TANDEM-0.1.8/setup.py` & `SPRT-TANDEM-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 with open(
     path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
 ) as f:
     long_description = f.read()
 
 setup(
     name="SPRT-TANDEM",
-    version="0.1.8",
+    version="0.1.9",
     license="MIT",
     description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.",
     author="Akinori F. Ebihara",
     author_email="aebihara@nec.com",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     package_data={
-        "data": ["train_10000/*.mdb"],
+        "data": ["train_10000/*.mdb", "val_100/*.mdb"],
     },
     url="https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch",
     keywords=[
         "Sequential Probability Ratio Test",
         "likelihood ratio",
         "density ratio estimation",
         "early classification",
```

### Comparing `SPRT-TANDEM-0.1.8/tandem/config/config_definition.py` & `SPRT-TANDEM-0.1.9/tandem/config/config_definition.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/models/losses.py` & `SPRT-TANDEM-0.1.9/tandem/models/losses.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/models/optimizers.py` & `SPRT-TANDEM-0.1.9/tandem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/models/temporal_integrators.py` & `SPRT-TANDEM-0.1.9/tandem/models/temporal_integrators.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/sprt_tandem_main.py` & `SPRT-TANDEM-0.1.9/tandem/sprt_tandem_main.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/utils/checkpoint.py` & `SPRT-TANDEM-0.1.9/tandem/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/utils/data_processing.py` & `SPRT-TANDEM-0.1.9/tandem/utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/utils/hyperparameter_tuning.py` & `SPRT-TANDEM-0.1.9/tandem/utils/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/utils/logging.py` & `SPRT-TANDEM-0.1.9/tandem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/utils/misc.py` & `SPRT-TANDEM-0.1.9/tandem/utils/misc.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/utils/performance_metrics.py` & `SPRT-TANDEM-0.1.9/tandem/utils/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.8/tandem/utils/training.py` & `SPRT-TANDEM-0.1.9/tandem/utils/training.py`

 * *Files identical despite different names*

