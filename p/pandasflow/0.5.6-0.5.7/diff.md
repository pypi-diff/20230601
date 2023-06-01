# Comparing `tmp/pandasflow-0.5.6.tar.gz` & `tmp/pandasflow-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.5.6.tar", last modified: Thu Jun  1 08:29:39 2023, max compression
+gzip compressed data, was "pandasflow-0.5.7.tar", last modified: Thu Jun  1 08:35:15 2023, max compression
```

## Comparing `pandasflow-0.5.6.tar` & `pandasflow-0.5.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.417497 pandasflow-0.5.6/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.6/LICENCE
--rw-rw-rw-   0        0        0      869 2023-06-01 08:29:39.417497 pandasflow-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.5.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.403535 pandasflow-0.5.6/pandasflow/
--rw-rw-rw-   0        0        0      391 2023-06-01 08:29:36.000000 pandasflow-0.5.6/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.406526 pandasflow-0.5.6/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.6/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.6/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.5.6/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.6/pandasflow/get_psql.py
--rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.5.6/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.410516 pandasflow-0.5.6/pandasflow/metrics/
--rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.6/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      797 2023-06-01 08:27:10.000000 pandasflow-0.5.6/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.6/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.5.6/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.6/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.6/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.6/pandasflow/metrics/roc.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.410516 pandasflow-0.5.6/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.6/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.5.6/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.410516 pandasflow-0.5.6/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.6/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.412510 pandasflow-0.5.6/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.6/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.5.6/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.5.6/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.405529 pandasflow-0.5.6/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      869 2023-06-01 08:29:39.000000 pandasflow-0.5.6/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      958 2023-06-01 08:29:39.000000 pandasflow-0.5.6/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:29:39.000000 pandasflow-0.5.6/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-01 08:29:39.000000 pandasflow-0.5.6/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-01 08:29:39.000000 pandasflow-0.5.6/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 08:29:39.418495 pandasflow-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:29:39.417497 pandasflow-0.5.6/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.6/test/__init__.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.6/test/best_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.6/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.5.6/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.6/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.6/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.6/test/roc_test.py
--rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.5.6/test/split_tt_test.py
--rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.5.6/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.414077 pandasflow-0.5.7/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.7/LICENCE
+-rw-rw-rw-   0        0        0      869 2023-06-01 08:35:15.414077 pandasflow-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.5.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.397489 pandasflow-0.5.7/pandasflow/
+-rw-rw-rw-   0        0        0      391 2023-06-01 08:35:10.000000 pandasflow-0.5.7/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.401479 pandasflow-0.5.7/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.7/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.7/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.5.7/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.7/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.5.7/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.405148 pandasflow-0.5.7/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.7/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      797 2023-06-01 08:27:10.000000 pandasflow-0.5.7/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.7/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.5.7/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.7/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.7/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.7/pandasflow/metrics/roc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.405148 pandasflow-0.5.7/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.7/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.5.7/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.406149 pandasflow-0.5.7/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.7/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.407146 pandasflow-0.5.7/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.7/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.5.7/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.5.7/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.399484 pandasflow-0.5.7/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      869 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:35:15.414077 pandasflow-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.413473 pandasflow-0.5.7/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.7/test/__init__.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.7/test/best_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.7/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.5.7/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.7/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.7/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.7/test/roc_test.py
+-rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.5.7/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.5.7/test/split_tvt_test.py
```

### Comparing `pandasflow-0.5.6/LICENCE` & `pandasflow-0.5.7/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/PKG-INFO` & `pandasflow-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.6
+Version: 0.5.7
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.6/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.5.7/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow/metrics/best_f1.py` & `pandasflow-0.5.7/pandasflow/metrics/best_f1.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow/metrics/conf_mat.py` & `pandasflow-0.5.7/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow/metrics/lloss_up.py` & `pandasflow-0.5.7/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow/metrics/precision_recall.py` & `pandasflow-0.5.7/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow/metrics/roc.py` & `pandasflow-0.5.7/pandasflow/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow/reset_mi.py` & `pandasflow-0.5.7/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow/split/train_test.py` & `pandasflow-0.5.7/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow/split/train_valid_test.py` & `pandasflow-0.5.7/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.5.7/pandasflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.6
+Version: 0.5.7
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.6/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.5.7/pandasflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/setup.py` & `pandasflow-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/test/best_f1_test.py` & `pandasflow-0.5.7/test/best_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/test/conf_mat_test.py` & `pandasflow-0.5.7/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/test/lloss_up_test.py` & `pandasflow-0.5.7/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/test/precision_recall_test.py` & `pandasflow-0.5.7/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/test/roc_test.py` & `pandasflow-0.5.7/test/roc_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.6/test/split_tvt_test.py` & `pandasflow-0.5.7/test/split_tvt_test.py`

 * *Files identical despite different names*

