# Comparing `tmp/celoMine-0.0.3.tar.gz` & `tmp/celoMine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\celoMine-0.0.3.tar", last modified: Wed May 31 20:55:52 2023, max compression
+gzip compressed data, was "dist\celoMine-0.0.4.tar", last modified: Thu Jun  1 09:39:03 2023, max compression
```

## Comparing `celoMine-0.0.3.tar` & `celoMine-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 20:55:52.483464 celoMine-0.0.3/
--rw-rw-rw-   0        0        0    35820 2023-05-31 18:08:15.000000 celoMine-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2925 2023-05-31 20:55:52.481485 celoMine-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2362 2023-05-31 18:08:15.000000 celoMine-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 20:55:52.445461 celoMine-0.0.3/celoMine/
--rw-rw-rw-   0        0        0     5377 2023-05-31 18:08:15.000000 celoMine-0.0.3/celoMine/PredictivePR.py
--rw-rw-rw-   0        0        0       98 2023-05-31 18:08:15.000000 celoMine-0.0.3/celoMine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:55:52.476465 celoMine-0.0.3/celoMine.egg-info/
--rw-rw-rw-   0        0        0     2925 2023-05-31 20:55:52.000000 celoMine-0.0.3/celoMine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-31 20:55:52.000000 celoMine-0.0.3/celoMine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 20:55:52.000000 celoMine-0.0.3/celoMine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-31 20:55:52.000000 celoMine-0.0.3/celoMine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 20:55:52.000000 celoMine-0.0.3/celoMine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 20:55:52.484465 celoMine-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-05-31 20:55:18.000000 celoMine-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:39:03.978544 celoMine-0.0.4/
+-rw-rw-rw-   0        0        0    35820 2023-05-31 18:08:15.000000 celoMine-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2925 2023-06-01 09:39:03.978544 celoMine-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2362 2023-05-31 18:08:15.000000 celoMine-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 09:39:03.962551 celoMine-0.0.4/celoMine/
+-rw-rw-rw-   0        0        0     5377 2023-05-31 18:08:15.000000 celoMine-0.0.4/celoMine/PredictivePR.py
+-rw-rw-rw-   0        0        0       98 2023-05-31 18:08:15.000000 celoMine-0.0.4/celoMine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:39:03.978544 celoMine-0.0.4/celoMine.egg-info/
+-rw-rw-rw-   0        0        0     2925 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:39:03.978544 celoMine-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-06-01 09:32:48.000000 celoMine-0.0.4/setup.py
```

### Comparing `celoMine-0.0.3/LICENSE` & `celoMine-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.3/PKG-INFO` & `celoMine-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celoMine
-Version: 0.0.3
+Version: 0.0.4
 Summary: Predictive machine learning for Celonis
 Author: Jean BERTIN
 Author-email: <jeanbertin.ensam@gmail.com>
 Keywords: python,celonis,process mining
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `celoMine-0.0.3/README.md` & `celoMine-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.3/celoMine/PredictivePR.py` & `celoMine-0.0.4/celoMine/PredictivePR.py`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.3/celoMine.egg-info/PKG-INFO` & `celoMine-0.0.4/celoMine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celoMine
-Version: 0.0.3
+Version: 0.0.4
 Summary: Predictive machine learning for Celonis
 Author: Jean BERTIN
 Author-email: <jeanbertin.ensam@gmail.com>
 Keywords: python,celonis,process mining
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `celoMine-0.0.3/setup.py` & `celoMine-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Predictive machine learning for Celonis'
 LONG_DESCRIPTION = 'Enrich Celonis process mining analyses using predictive machine learning and visualisation tools'
 
 # Setting up
 setup(
     name="celoMine",
     version=VERSION,
     author="Jean BERTIN",
     author_email="<jeanbertin.ensam@gmail.com>",
     description=DESCRIPTION,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    install_requires=['pandas', 'numpy' ,'sklearn','matplotlib'],
+    install_requires=['pandas', 'numpy' ,'scikit-learn','matplotlib'],
     keywords=['python', 'celonis', 'process mining'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

