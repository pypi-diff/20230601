# Comparing `tmp/Timeseries-Preprocess-0.1.2.tar.gz` & `tmp/Timeseries-Preprocess-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Timeseries-Preprocess-0.1.2.tar", last modified: Thu Jun  1 02:04:49 2023, max compression
+gzip compressed data, was "Timeseries-Preprocess-0.1.3.tar", last modified: Thu Jun  1 02:29:30 2023, max compression
```

## Comparing `Timeseries-Preprocess-0.1.2.tar` & `Timeseries-Preprocess-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:04:49.862782 Timeseries-Preprocess-0.1.2/
--rw-r--r--   0 ruiwan     (501) staff       (20)      653 2023-06-01 02:04:49.862604 Timeseries-Preprocess-0.1.2/PKG-INFO
--rw-r--r--   0 ruiwan     (501) staff       (20)      279 2023-05-11 03:28:23.000000 Timeseries-Preprocess-0.1.2/README.md
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:04:49.853244 Timeseries-Preprocess-0.1.2/Timeseries_Preprocess.egg-info/
--rw-r--r--   0 ruiwan     (501) staff       (20)      653 2023-06-01 02:04:49.000000 Timeseries-Preprocess-0.1.2/Timeseries_Preprocess.egg-info/PKG-INFO
--rw-r--r--   0 ruiwan     (501) staff       (20)     1895 2023-06-01 02:04:49.000000 Timeseries-Preprocess-0.1.2/Timeseries_Preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 ruiwan     (501) staff       (20)        1 2023-06-01 02:04:49.000000 Timeseries-Preprocess-0.1.2/Timeseries_Preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 ruiwan     (501) staff       (20)       47 2023-06-01 02:04:49.000000 Timeseries-Preprocess-0.1.2/Timeseries_Preprocess.egg-info/requires.txt
--rw-r--r--   0 ruiwan     (501) staff       (20)       22 2023-06-01 02:04:49.000000 Timeseries-Preprocess-0.1.2/Timeseries_Preprocess.egg-info/top_level.txt
--rw-r--r--   0 ruiwan     (501) staff       (20)       38 2023-06-01 02:04:49.863000 Timeseries-Preprocess-0.1.2/setup.cfg
--rw-r--r--   0 ruiwan     (501) staff       (20)     1153 2023-06-01 02:04:46.000000 Timeseries-Preprocess-0.1.2/setup.py
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:04:49.853849 Timeseries-Preprocess-0.1.2/timeseries_preprocess/
--rw-r--r--   0 ruiwan     (501) staff       (20)      350 2023-05-12 02:31:04.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/__init__.py
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:04:49.856563 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/
--rw-r--r--   0 ruiwan     (501) staff       (20)      502 2023-05-03 03:30:17.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/__init__.py
--rw-r--r--   0 ruiwan     (501) staff       (20)     1130 2023-05-07 07:45:13.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/adaptive_denoise.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      712 2023-05-07 07:45:18.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/ceemdan_denoise.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      294 2023-05-03 09:10:09.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/denoise_object.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      697 2023-05-07 07:45:29.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/eemd_denoise.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      692 2023-05-07 07:45:33.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/emd_denoise.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      625 2023-05-03 09:09:59.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/fourier_denoise.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      571 2023-05-07 07:45:50.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/moving_avg_denoise.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      576 2023-05-07 07:45:55.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/moving_median_denoise.py
--rw-r--r--   0 ruiwan     (501) staff       (20)     1125 2023-05-07 07:46:04.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/ssa_denoise.py
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:04:49.859786 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/
--rw-r--r--   0 ruiwan     (501) staff       (20)     1006 2023-05-03 08:52:55.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/__init__.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      411 2023-05-03 09:09:42.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/backward_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      484 2023-05-07 14:01:20.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/fixed_value_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      410 2023-05-03 09:09:35.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/forward_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      297 2023-05-03 09:09:31.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/imputation_object.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      408 2023-05-03 09:09:29.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/interpolate_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      677 2023-05-07 07:46:22.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/knn_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      451 2023-05-03 09:09:22.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/mean_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      455 2023-05-03 09:09:15.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/median_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      718 2023-05-03 09:09:10.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/missing_forest_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      451 2023-05-03 09:09:02.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/mode_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      615 2023-05-07 07:46:39.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/moving_avg_imputation.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      788 2023-05-07 13:19:56.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/weighted_moving_avg_imputation.py
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:04:49.861340 Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/
--rw-r--r--   0 ruiwan     (501) staff       (20)      264 2023-05-03 03:33:33.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/__init__.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      866 2023-05-08 07:52:35.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/dbscan_outlier.py
--rw-r--r--   0 ruiwan     (501) staff       (20)     1547 2023-05-08 07:52:40.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/gesd_outlier.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      768 2023-05-08 07:52:29.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/iqr_outlier.py
--rw-r--r--   0 ruiwan     (501) staff       (20)     1272 2023-05-08 07:52:45.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/kmeans_outlier.py
--rw-r--r--   0 ruiwan     (501) staff       (20)      320 2023-05-08 02:35:16.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/outlier_object.py
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:04:49.861743 Timeseries-Preprocess-0.1.2/timeseries_preprocess/tests/
--rw-r--r--   0 ruiwan     (501) staff       (20)        0 2023-05-07 13:01:02.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/tests/__init__.py
--rw-r--r--   0 ruiwan     (501) staff       (20)     5056 2023-05-12 03:54:39.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/timeseries_preprocess_framework.py
-drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:04:49.861865 Timeseries-Preprocess-0.1.2/timeseries_preprocess/utils/
--rw-r--r--   0 ruiwan     (501) staff       (20)     4126 2023-05-11 12:42:59.000000 Timeseries-Preprocess-0.1.2/timeseries_preprocess/utils/__init__.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:29:30.818613 Timeseries-Preprocess-0.1.3/
+-rw-r--r--   0 ruiwan     (501) staff       (20)      653 2023-06-01 02:29:30.818409 Timeseries-Preprocess-0.1.3/PKG-INFO
+-rw-r--r--   0 ruiwan     (501) staff       (20)      279 2023-05-11 03:28:23.000000 Timeseries-Preprocess-0.1.3/README.md
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:29:30.804631 Timeseries-Preprocess-0.1.3/Timeseries_Preprocess.egg-info/
+-rw-r--r--   0 ruiwan     (501) staff       (20)      653 2023-06-01 02:29:30.000000 Timeseries-Preprocess-0.1.3/Timeseries_Preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 ruiwan     (501) staff       (20)     1895 2023-06-01 02:29:30.000000 Timeseries-Preprocess-0.1.3/Timeseries_Preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 ruiwan     (501) staff       (20)        1 2023-06-01 02:29:30.000000 Timeseries-Preprocess-0.1.3/Timeseries_Preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 ruiwan     (501) staff       (20)       47 2023-06-01 02:29:30.000000 Timeseries-Preprocess-0.1.3/Timeseries_Preprocess.egg-info/requires.txt
+-rw-r--r--   0 ruiwan     (501) staff       (20)       22 2023-06-01 02:29:30.000000 Timeseries-Preprocess-0.1.3/Timeseries_Preprocess.egg-info/top_level.txt
+-rw-r--r--   0 ruiwan     (501) staff       (20)       38 2023-06-01 02:29:30.818691 Timeseries-Preprocess-0.1.3/setup.cfg
+-rw-r--r--   0 ruiwan     (501) staff       (20)     1153 2023-06-01 02:29:26.000000 Timeseries-Preprocess-0.1.3/setup.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:29:30.805084 Timeseries-Preprocess-0.1.3/timeseries_preprocess/
+-rw-r--r--   0 ruiwan     (501) staff       (20)      350 2023-05-12 02:31:04.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/__init__.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:29:30.810446 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/
+-rw-r--r--   0 ruiwan     (501) staff       (20)      502 2023-05-03 03:30:17.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/__init__.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)     1130 2023-05-07 07:45:13.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/adaptive_denoise.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      712 2023-05-07 07:45:18.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/ceemdan_denoise.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      294 2023-05-03 09:10:09.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/denoise_object.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      697 2023-05-07 07:45:29.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/eemd_denoise.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      692 2023-05-07 07:45:33.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/emd_denoise.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      625 2023-05-03 09:09:59.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/fourier_denoise.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      571 2023-05-07 07:45:50.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/moving_avg_denoise.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      576 2023-05-07 07:45:55.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/moving_median_denoise.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)     1125 2023-05-07 07:46:04.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/ssa_denoise.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:29:30.815811 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/
+-rw-r--r--   0 ruiwan     (501) staff       (20)     1006 2023-05-03 08:52:55.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/__init__.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      411 2023-05-03 09:09:42.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/backward_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      484 2023-05-07 14:01:20.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/fixed_value_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      410 2023-05-03 09:09:35.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/forward_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      297 2023-05-03 09:09:31.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/imputation_object.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      408 2023-05-03 09:09:29.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/interpolate_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      700 2023-06-01 02:28:59.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/knn_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      451 2023-05-03 09:09:22.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/mean_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      455 2023-05-03 09:09:15.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/median_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      718 2023-05-03 09:09:10.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/missing_forest_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      451 2023-05-03 09:09:02.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/mode_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      615 2023-05-07 07:46:39.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/moving_avg_imputation.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      788 2023-05-07 13:19:56.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/weighted_moving_avg_imputation.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:29:30.817535 Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/
+-rw-r--r--   0 ruiwan     (501) staff       (20)      264 2023-05-03 03:33:33.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/__init__.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      866 2023-05-08 07:52:35.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/dbscan_outlier.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)     1547 2023-05-08 07:52:40.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/gesd_outlier.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      768 2023-05-08 07:52:29.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/iqr_outlier.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)     1272 2023-05-08 07:52:45.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/kmeans_outlier.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)      320 2023-05-08 02:35:16.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/outlier_object.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:29:30.817829 Timeseries-Preprocess-0.1.3/timeseries_preprocess/tests/
+-rw-r--r--   0 ruiwan     (501) staff       (20)        0 2023-05-07 13:01:02.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/tests/__init__.py
+-rw-r--r--   0 ruiwan     (501) staff       (20)     5056 2023-05-12 03:54:39.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/timeseries_preprocess_framework.py
+drwxr-xr-x   0 ruiwan     (501) staff       (20)        0 2023-06-01 02:29:30.817955 Timeseries-Preprocess-0.1.3/timeseries_preprocess/utils/
+-rw-r--r--   0 ruiwan     (501) staff       (20)     4126 2023-05-11 12:42:59.000000 Timeseries-Preprocess-0.1.3/timeseries_preprocess/utils/__init__.py
```

### Comparing `Timeseries-Preprocess-0.1.2/PKG-INFO` & `Timeseries-Preprocess-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Timeseries-Preprocess
-Version: 0.1.2
+Version: 0.1.3
 Summary: toolkit for time series preprocessing
 Home-page: https://github.com/Kiko-RWan/Timeseries-Preprocess
 Author: Rui Wan
 Author-email: rwan972000@gamil.com
 License: MIT
 Description: # Timeseries-Preprocess
         ## Deploy Web App
```

### Comparing `Timeseries-Preprocess-0.1.2/Timeseries_Preprocess.egg-info/PKG-INFO` & `Timeseries-Preprocess-0.1.3/Timeseries_Preprocess.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Timeseries-Preprocess
-Version: 0.1.2
+Version: 0.1.3
 Summary: toolkit for time series preprocessing
 Home-page: https://github.com/Kiko-RWan/Timeseries-Preprocess
 Author: Rui Wan
 Author-email: rwan972000@gamil.com
 License: MIT
 Description: # Timeseries-Preprocess
         ## Deploy Web App
```

### Comparing `Timeseries-Preprocess-0.1.2/Timeseries_Preprocess.egg-info/SOURCES.txt` & `Timeseries-Preprocess-0.1.3/Timeseries_Preprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/setup.py` & `Timeseries-Preprocess-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         from pip.download import PipSession
         from pip.req import parse_requirements
 
 requirements = parse_requirements(os.path.join(os.path.dirname(__file__), 'requirements.txt'), session=PipSession())
 
 setup(
     name='Timeseries-Preprocess',
-    version='0.1.2',
+    version='0.1.3',
     description='toolkit for time series preprocessing',
     author='Rui Wan',
     author_email='rwan972000@gamil.com',
     url='https://github.com/Kiko-RWan/Timeseries-Preprocess',
     packages=find_packages(),
     license='MIT',
     long_description_content_type="text/markdown",
```

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/adaptive_denoise.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/adaptive_denoise.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/ceemdan_denoise.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/ceemdan_denoise.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/eemd_denoise.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/eemd_denoise.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/emd_denoise.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/emd_denoise.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/fourier_denoise.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/fourier_denoise.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/moving_avg_denoise.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/moving_avg_denoise.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/moving_median_denoise.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/moving_median_denoise.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/denoise/ssa_denoise.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/denoise/ssa_denoise.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/__init__.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/__init__.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/knn_imputation.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/knn_imputation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from .imputation_object import ImputationObject
 
 import pandas as pd
-from sklearn.impute import KNNImputer
+# from sklearn.impute import KNNImputer
 
 
 class KnnImputation(ImputationObject):
     _required_args = ["k"]
     
     def __init__(
         self, data: pd.DataFrame, target_col, inplace=False, analysis=False, **kwargs
     ):
         self._required_args = ["k"]
         super().__init__(data, target_col, inplace, analysis, **kwargs)
         self._run_once = True
 
     def real_run(self, target_col):
-        imputer = KNNImputer(n_neighbors=self.k)
+        # imputer = KNNImputer(n_neighbors=self.k)
 
-        knn_data = self.data.copy(deep=True)
-        knn_data = imputer.fit_transform(knn_data)
+        # knn_data = self.data.copy(deep=True)
+        # knn_data = imputer.fit_transform(knn_data)
 
-        self.data.iloc[:, target_col] = knn_data[:, target_col]
+        # self.data.iloc[:, target_col] = knn_data[:, target_col]
+        pass
```

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/missing_forest_imputation.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/missing_forest_imputation.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/moving_avg_imputation.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/moving_avg_imputation.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/imputation/weighted_moving_avg_imputation.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/imputation/weighted_moving_avg_imputation.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/dbscan_outlier.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/dbscan_outlier.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/gesd_outlier.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/gesd_outlier.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/iqr_outlier.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/iqr_outlier.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/outlier/kmeans_outlier.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/outlier/kmeans_outlier.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/timeseries_preprocess_framework.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/timeseries_preprocess_framework.py`

 * *Files identical despite different names*

### Comparing `Timeseries-Preprocess-0.1.2/timeseries_preprocess/utils/__init__.py` & `Timeseries-Preprocess-0.1.3/timeseries_preprocess/utils/__init__.py`

 * *Files identical despite different names*

