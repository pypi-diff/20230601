# Comparing `tmp/celoMine-0.0.6.tar.gz` & `tmp/celoMine-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\celoMine-0.0.6.tar", last modified: Thu Jun  1 14:22:50 2023, max compression
+gzip compressed data, was "dist\celoMine-0.0.7.tar", last modified: Thu Jun  1 14:40:18 2023, max compression
```

## Comparing `celoMine-0.0.6.tar` & `celoMine-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:22:50.198871 celoMine-0.0.6/
--rw-rw-rw-   0        0        0    35820 2023-05-31 18:08:15.000000 celoMine-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3721 2023-06-01 14:22:50.198871 celoMine-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2023-06-01 14:17:10.000000 celoMine-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 14:22:50.151951 celoMine-0.0.6/celoMine/
--rw-rw-rw-   0        0        0     5377 2023-05-31 18:08:15.000000 celoMine-0.0.6/celoMine/PredictivePR.py
--rw-rw-rw-   0        0        0       98 2023-05-31 18:08:15.000000 celoMine-0.0.6/celoMine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:22:50.183235 celoMine-0.0.6/celoMine.egg-info/
--rw-rw-rw-   0        0        0     3721 2023-06-01 14:22:49.000000 celoMine-0.0.6/celoMine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-01 14:22:50.000000 celoMine-0.0.6/celoMine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:22:49.000000 celoMine-0.0.6/celoMine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-01 14:22:49.000000 celoMine-0.0.6/celoMine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 14:22:49.000000 celoMine-0.0.6/celoMine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 14:22:50.198871 celoMine-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1090 2023-06-01 14:20:39.000000 celoMine-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:40:18.029615 celoMine-0.0.7/
+-rw-rw-rw-   0        0        0    35820 2023-05-31 18:08:15.000000 celoMine-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3721 2023-06-01 14:40:18.029615 celoMine-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3079 2023-06-01 14:17:10.000000 celoMine-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 14:40:17.998356 celoMine-0.0.7/celoMine/
+-rw-rw-rw-   0        0        0     5377 2023-05-31 18:08:15.000000 celoMine-0.0.7/celoMine/PredictivePR.py
+-rw-rw-rw-   0        0        0      110 2023-06-01 14:39:08.000000 celoMine-0.0.7/celoMine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:40:18.013984 celoMine-0.0.7/celoMine.egg-info/
+-rw-rw-rw-   0        0        0     3721 2023-06-01 14:40:17.000000 celoMine-0.0.7/celoMine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-01 14:40:17.000000 celoMine-0.0.7/celoMine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 14:40:17.000000 celoMine-0.0.7/celoMine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-01 14:40:17.000000 celoMine-0.0.7/celoMine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 14:40:17.000000 celoMine-0.0.7/celoMine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 14:40:18.029615 celoMine-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-06-01 14:39:21.000000 celoMine-0.0.7/setup.py
```

### Comparing `celoMine-0.0.6/LICENSE` & `celoMine-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.6/PKG-INFO` & `celoMine-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celoMine
-Version: 0.0.6
+Version: 0.0.7
 Summary: Predictive machine learning for Celonis
 Home-page: https://github.com/JeanBertinR/celoMine
 Author: Jean BERTIN
 Author-email: <jeanbertin.ensam@gmail.com>
 License: GPL-v3
 Keywords: celonis,process mining,machine learning
 Classifier: Development Status :: 1 - Planning
```

### Comparing `celoMine-0.0.6/README.md` & `celoMine-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.6/celoMine/PredictivePR.py` & `celoMine-0.0.7/celoMine/PredictivePR.py`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.6/celoMine.egg-info/PKG-INFO` & `celoMine-0.0.7/celoMine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celoMine
-Version: 0.0.6
+Version: 0.0.7
 Summary: Predictive machine learning for Celonis
 Home-page: https://github.com/JeanBertinR/celoMine
 Author: Jean BERTIN
 Author-email: <jeanbertin.ensam@gmail.com>
 License: GPL-v3
 Keywords: celonis,process mining,machine learning
 Classifier: Development Status :: 1 - Planning
```

### Comparing `celoMine-0.0.6/setup.py` & `celoMine-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Predictive machine learning for Celonis'
 LONG_DESCRIPTION = 'Enrich Celonis process mining analyses using predictive machine learning and visualisation tools'
 
 # Setting up
 setup(
     name="celoMine",
     version=VERSION,
```

