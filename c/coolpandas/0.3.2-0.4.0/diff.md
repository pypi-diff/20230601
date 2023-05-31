# Comparing `tmp/coolpandas-0.3.2.tar.gz` & `tmp/coolpandas-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpandas-0.3.2.tar", last modified: Tue May 23 18:40:42 2023, max compression
+gzip compressed data, was "coolpandas-0.4.0.tar", last modified: Wed May 31 23:26:25 2023, max compression
```

## Comparing `coolpandas-0.3.2.tar` & `coolpandas-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.396992 coolpandas-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 18:40:31.000000 coolpandas-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-23 18:40:42.396992 coolpandas-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-23 18:40:31.000000 coolpandas-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.388992 coolpandas-0.3.2/coolpandas/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas/connect/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/connect/redshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/features_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/geo_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/random_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/evaluate/confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/distplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/geoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/mapplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.396992 coolpandas-0.3.2/coolpandas/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.396992 coolpandas-0.3.2/coolpandas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-23 18:40:31.000000 coolpandas-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:40:42.396992 coolpandas-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 23:26:16.000000 coolpandas-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-31 23:26:25.188072 coolpandas-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-31 23:26:16.000000 coolpandas-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.180071 coolpandas-0.4.0/coolpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.184071 coolpandas-0.4.0/coolpandas/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/connect/redshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.184071 coolpandas-0.4.0/coolpandas/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/features_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/geo_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.184071 coolpandas-0.4.0/coolpandas/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/evaluate/confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/coolpandas/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/distplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/geoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/mapplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/coolpandas/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/stats/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/stats/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/coolpandas/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/coolpandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.184071 coolpandas-0.4.0/coolpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-31 23:26:16.000000 coolpandas-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:26:25.188072 coolpandas-0.4.0/setup.cfg
```

### Comparing `coolpandas-0.3.2/LICENSE` & `coolpandas-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/PKG-INFO` & `coolpandas-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.3.2/README.md` & `coolpandas-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/connect/redshift.py` & `coolpandas-0.4.0/coolpandas/connect/redshift.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/__init__.py` & `coolpandas-0.4.0/coolpandas/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/correlation.py` & `coolpandas-0.4.0/coolpandas/eda/correlation.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/distribution.py` & `coolpandas-0.4.0/coolpandas/eda/distribution.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/duplicates.py` & `coolpandas-0.4.0/coolpandas/eda/duplicates.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/features_type.py` & `coolpandas-0.4.0/coolpandas/eda/features_type.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/geo_distance.py` & `coolpandas-0.4.0/coolpandas/eda/geo_distance.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/missing_values.py` & `coolpandas-0.4.0/coolpandas/eda/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/shape.py` & `coolpandas-0.4.0/coolpandas/eda/shape.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/summary.py` & `coolpandas-0.4.0/coolpandas/eda/summary.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/eda/value_counts.py` & `coolpandas-0.4.0/coolpandas/eda/value_counts.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/evaluate/confusion_matrix.py` & `coolpandas-0.4.0/coolpandas/evaluate/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/plot/barplot.py` & `coolpandas-0.4.0/coolpandas/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/plot/boxplot.py` & `coolpandas-0.4.0/coolpandas/plot/lineplot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-"""Box plot module."""
+"""Lineplot module."""
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 
 from .style import custom_template, format_title
 
 
-def boxplot(
+def lineplot(
     data_frame: pd.DataFrame,
     x_axis: str,
     y_axis: str,
     title: str,
     subtitle: str | None = None,
     **kwargs,
 ) -> go.Figure:
-    """Create a box plot.
+    """Create a bar plot.
 
     Args:
         data_frame (pd.DataFrame): DataFrame to plot.
         x_axis (str): Column to use as x axis.
         y_axis (str): Column to use as y axis.
         title (str): Title of the plot.
         subtitle (str, optional): Subtitle of the plot. Defaults to None.
-        **kwargs: Keyword arguments to pass to plotly.express.box.
+        **kwargs: Keyword arguments to pass to plotly.express.bar.
 
     Returns:
-        go.Figure: Box plot figure.
+        go.Figure: Bar plot figure.
     """
-    if "color" not in kwargs:
-        kwargs["color"] = x_axis
-    fig = px.box(
+    fig = px.line(
         data_frame,
         x=x_axis,
         y=y_axis,
-        notched=True,
         title=format_title(title, subtitle=subtitle),
         template=custom_template,
         width=800,
         height=400,
         **kwargs,
     )
-    if kwargs.get("color") == x_axis:
-        fig.layout.update(showlegend=False)
     return fig
```

### Comparing `coolpandas-0.3.2/coolpandas/plot/distplot.py` & `coolpandas-0.4.0/coolpandas/plot/distplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/plot/geoplot.py` & `coolpandas-0.4.0/coolpandas/plot/geoplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/plot/lineplot.py` & `coolpandas-0.4.0/coolpandas/plot/mapplot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-"""Lineplot module."""
+"""Correlation map function."""
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 
 from .style import custom_template, format_title
 
 
-def lineplot(
-    data_frame: pd.DataFrame,
-    x_axis: str,
-    y_axis: str,
+def mapplot(
+    matrix: pd.DataFrame,
     title: str,
     subtitle: str | None = None,
+    width: int = 1000,
+    height: int = 1000,
     **kwargs,
 ) -> go.Figure:
-    """Create a bar plot.
+    """Create a correlation map.
 
     Args:
-        data_frame (pd.DataFrame): DataFrame to plot.
-        x_axis (str): Column to use as x axis.
-        y_axis (str): Column to use as y axis.
+        matrix (pd.DataFrame): Correlation matrix to plot.
         title (str): Title of the plot.
         subtitle (str, optional): Subtitle of the plot. Defaults to None.
-        **kwargs: Keyword arguments to pass to plotly.express.bar.
+        width (int, optional): Width of the plot. Defaults to 1000.
+        height (int, optional): Height of the plot. Defaults to 1000.
+        **kwargs: Keyword arguments to pass to plotly.express.imshow.
 
     Returns:
-        go.Figure: Bar plot figure.
+        go.Figure: Correlation map figure.
     """
-    fig = px.line(
-        data_frame,
-        x=x_axis,
-        y=y_axis,
+    fig = px.imshow(
+        matrix,
+        text_auto=True,
+        zmin=-1,
+        zmax=1,
         title=format_title(title, subtitle=subtitle),
         template=custom_template,
-        width=800,
-        height=400,
+        width=width,
+        height=height,
         **kwargs,
     )
     return fig
```

### Comparing `coolpandas-0.3.2/coolpandas/plot/style.py` & `coolpandas-0.4.0/coolpandas/plot/style.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/transform/bin.py` & `coolpandas-0.4.0/coolpandas/transform/bin.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/transform/missing_values.py` & `coolpandas-0.4.0/coolpandas/transform/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas/transform/outliers.py` & `coolpandas-0.4.0/coolpandas/transform/outliers.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.2/coolpandas.egg-info/PKG-INFO` & `coolpandas-0.4.0/coolpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.3.2/coolpandas.egg-info/SOURCES.txt` & `coolpandas-0.4.0/coolpandas.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 coolpandas/plot/barplot.py
 coolpandas/plot/boxplot.py
 coolpandas/plot/distplot.py
 coolpandas/plot/geoplot.py
 coolpandas/plot/lineplot.py
 coolpandas/plot/mapplot.py
 coolpandas/plot/style.py
+coolpandas/stats/__init__.py
+coolpandas/stats/effect.py
+coolpandas/stats/ttest.py
 coolpandas/transform/__init__.py
 coolpandas/transform/bin.py
 coolpandas/transform/epoch.py
 coolpandas/transform/missing_values.py
 coolpandas/transform/outliers.py
 coolpandas/utils/__init__.py
 coolpandas/utils/random_state.py
```

### Comparing `coolpandas-0.3.2/pyproject.toml` & `coolpandas-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coolpandas"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   { name="Avel Docquin", email="adocquin@outlook.com" },
   ]
 description = "A Python package for Exploratory Data Analysis."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
   "pandas ~= 1.5.1",
   "scipy ~= 1.9.3",
   "scikit-learn ~= 1.1.3",
   "plotly ~= 5.11.0",
   "nbformat ~= 5.7.0",
   "ipython ~= 8.6.0",
   "openrouteservice ~= 2.3.3",
+  "redshift-connector ~= 2.0.910",
+  "statsmodels ~= 0.14.0",
+  "jinja2 ~= 3.1.2",
   "pytest-cov ~= 4.0.0",
   "black ~= 22.10.0",
   "pylint ~= 2.15.5",
   "isort ~= 5.10.1",
   "pre-commit ~= 2.20.0"
 ]
 classifiers = [
@@ -44,14 +47,15 @@
 [tool.setuptools]
 packages = [
   "coolpandas",
   "coolpandas.connect",
   "coolpandas.eda",
   "coolpandas.evaluate",
   "coolpandas.plot",
+  "coolpandas.stats",
   "coolpandas.transform",
   "coolpandas.utils",
   ]
 
 [tool.isort]
 profile = "black"
```

