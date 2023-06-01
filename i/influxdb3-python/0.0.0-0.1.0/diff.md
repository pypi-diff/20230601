# Comparing `tmp/influxdb3-python-0.0.0.tar.gz` & `tmp/influxdb3-python-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.0.0.tar", last modified: Thu Jun  1 10:12:20 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.0.tar", last modified: Thu Jun  1 10:49:49 2023, max compression
```

## Comparing `influxdb3-python-0.0.0.tar` & `influxdb3-python-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-06-01 10:12:20.073664 influxdb3-python-0.0.0/
--rw-r--r--   0 jayclifford   (501) staff       (20)     3504 2023-06-01 10:12:20.073335 influxdb3-python-0.0.0/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     2797 2023-06-01 10:05:12.000000 influxdb3-python-0.0.0/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-06-01 10:12:20.071996 influxdb3-python-0.0.0/influxdb3_python.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     3504 2023-06-01 10:12:20.000000 influxdb3-python-0.0.0/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      247 2023-06-01 10:12:20.000000 influxdb3-python-0.0.0/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-06-01 10:12:20.000000 influxdb3-python-0.0.0/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       24 2023-06-01 10:12:20.000000 influxdb3-python-0.0.0/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-06-01 10:12:20.000000 influxdb3-python-0.0.0/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-06-01 10:12:20.072410 influxdb3-python-0.0.0/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     5060 2023-06-01 09:18:59.000000 influxdb3-python-0.0.0/influxdb_client_3/__init__.py
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-06-01 10:12:20.073761 influxdb3-python-0.0.0/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)     1529 2023-06-01 10:05:12.000000 influxdb3-python-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-01 10:49:38.000000 influxdb3-python-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-01 10:49:38.000000 influxdb3-python-0.1.0/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 10:49:38.000000 influxdb3-python-0.1.0/setup.py
```

### Comparing `influxdb3-python-0.0.0/PKG-INFO` & `influxdb3-python-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.0.0
+Version: 0.1.0
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="python-logo.png" alt="Your Image" width="150px">
+    <img src="https://github.com/InfluxCommunity/influxdb3-python/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python.svg" alt="PyPI version">
     </a>
     <a href="https://pypi.org/project/influxdb3-python/">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.0.0 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.0 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `influxdb3-python-0.0.0/README.md` & `influxdb3-python-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-    <img src="python-logo.png" alt="Your Image" width="150px">
+    <img src="https://github.com/InfluxCommunity/influxdb3-python/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python.svg" alt="PyPI version">
     </a>
     <a href="https://pypi.org/project/influxdb3-python/">
```

### Comparing `influxdb3-python-0.0.0/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.1.0/influxdb3_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.0.0
+Version: 0.1.0
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="python-logo.png" alt="Your Image" width="150px">
+    <img src="https://github.com/InfluxCommunity/influxdb3-python/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python.svg" alt="PyPI version">
     </a>
     <a href="https://pypi.org/project/influxdb3-python/">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.0.0 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.0 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `influxdb3-python-0.0.0/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.0/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.0.0/setup.py` & `influxdb3-python-0.1.0/setup.py`

 * *Files identical despite different names*

