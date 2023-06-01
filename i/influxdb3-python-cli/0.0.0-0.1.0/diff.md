# Comparing `tmp/influxdb3-python-cli-0.0.0.tar.gz` & `tmp/influxdb3-python-cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-cli-0.0.0.tar", last modified: Thu Jun  1 11:15:29 2023, max compression
+gzip compressed data, was "influxdb3-python-cli-0.1.0.tar", last modified: Thu Jun  1 11:19:31 2023, max compression
```

## Comparing `influxdb3-python-cli-0.0.0.tar` & `influxdb3-python-cli-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-06-01 11:15:29.190622 influxdb3-python-cli-0.0.0/
--rw-r--r--   0 jayclifford   (501) staff       (20)    11357 2023-06-01 09:21:47.000000 influxdb3-python-cli-0.0.0/LICENSE
--rw-r--r--   0 jayclifford   (501) staff       (20)     5348 2023-06-01 11:15:29.190291 influxdb3-python-cli-0.0.0/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     4605 2023-06-01 11:11:54.000000 influxdb3-python-cli-0.0.0/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-06-01 11:15:29.189044 influxdb3-python-cli-0.0.0/influxdb3_python_cli.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     5348 2023-06-01 11:15:29.000000 influxdb3-python-cli-0.0.0/influxdb3_python_cli.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      341 2023-06-01 11:15:29.000000 influxdb3-python-cli-0.0.0/influxdb3_python_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-06-01 11:15:29.000000 influxdb3-python-cli-0.0.0/influxdb3_python_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       54 2023-06-01 11:15:29.000000 influxdb3-python-cli-0.0.0/influxdb3_python_cli.egg-info/entry_points.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       65 2023-06-01 11:15:29.000000 influxdb3-python-cli-0.0.0/influxdb3_python_cli.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       13 2023-06-01 11:15:29.000000 influxdb3-python-cli-0.0.0/influxdb3_python_cli.egg-info/top_level.txt
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-06-01 11:15:29.189774 influxdb3-python-cli-0.0.0/influxdb_cli/
--rw-r--r--   0 jayclifford   (501) staff       (20)        0 2023-06-01 09:23:04.000000 influxdb3-python-cli-0.0.0/influxdb_cli/__init__.py
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     7638 2023-06-01 09:23:04.000000 influxdb3-python-cli-0.0.0/influxdb_cli/influx3.py
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-06-01 11:15:29.190753 influxdb3-python-cli-0.0.0/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)     1747 2023-06-01 09:25:31.000000 influxdb3-python-cli-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7638 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/influxdb_cli/influx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/setup.py
```

### Comparing `influxdb3-python-cli-0.0.0/LICENSE` & `influxdb3-python-cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.0.0/PKG-INFO` & `influxdb3-python-cli-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.0.0
+Version: 0.1.0
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
     <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python-cli.svg" alt="PyPI version">
     </a>
-    <a href="https://pypi.org/project/your-python-package/">
+    <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/dm/influxdb3-python-cli.svg" alt="PyPI downloads">
     </a>
     <a href="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/pylint.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
     </a>
         <a href="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/python-publish.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.0.0 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.1.0 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `influxdb3-python-cli-0.0.0/README.md` & `influxdb3-python-cli-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python-cli.svg" alt="PyPI version">
     </a>
-    <a href="https://pypi.org/project/your-python-package/">
+    <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/dm/influxdb3-python-cli.svg" alt="PyPI downloads">
     </a>
     <a href="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/pylint.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
     </a>
         <a href="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/python-publish.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
```

### Comparing `influxdb3-python-cli-0.0.0/influxdb3_python_cli.egg-info/PKG-INFO` & `influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.0.0
+Version: 0.1.0
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
     <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python-cli.svg" alt="PyPI version">
     </a>
-    <a href="https://pypi.org/project/your-python-package/">
+    <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/dm/influxdb3-python-cli.svg" alt="PyPI downloads">
     </a>
     <a href="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/pylint.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
     </a>
         <a href="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/python-publish.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.0.0 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.1.0 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `influxdb3-python-cli-0.0.0/influxdb_cli/influx3.py` & `influxdb3-python-cli-0.1.0/influxdb_cli/influx3.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.0.0/setup.py` & `influxdb3-python-cli-0.1.0/setup.py`

 * *Files identical despite different names*

