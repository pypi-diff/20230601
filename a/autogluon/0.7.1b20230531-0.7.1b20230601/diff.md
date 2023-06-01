# Comparing `tmp/autogluon-0.7.1b20230531.tar.gz` & `tmp/autogluon-0.7.1b20230601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.7.1b20230531.tar", last modified: Wed May 31 09:04:34 2023, max compression
+gzip compressed data, was "autogluon-0.7.1b20230601.tar", last modified: Thu Jun  1 09:04:16 2023, max compression
```

## Comparing `autogluon-0.7.1b20230531.tar` & `autogluon-0.7.1b20230601.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:34.331694 autogluon-0.7.1b20230531/
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-31 09:04:34.331694 autogluon-0.7.1b20230531/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:04:34.331694 autogluon-0.7.1b20230531/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-31 09:03:45.000000 autogluon-0.7.1b20230531/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:34.327694 autogluon-0.7.1b20230531/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:34.327694 autogluon-0.7.1b20230531/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:34.331694 autogluon-0.7.1b20230531/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:03:45.000000 autogluon-0.7.1b20230531/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:34.331694 autogluon-0.7.1b20230531/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-31 09:04:34.000000 autogluon-0.7.1b20230531/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 09:04:34.000000 autogluon-0.7.1b20230531/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:04:34.000000 autogluon-0.7.1b20230531/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:04:34.000000 autogluon-0.7.1b20230531/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-31 09:04:34.000000 autogluon-0.7.1b20230531/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:04:34.000000 autogluon-0.7.1b20230531/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:04:34.000000 autogluon-0.7.1b20230531/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:16.021633 autogluon-0.7.1b20230601/
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-06-01 09:04:16.021633 autogluon-0.7.1b20230601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:04:16.021633 autogluon-0.7.1b20230601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-01 09:03:27.000000 autogluon-0.7.1b20230601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:16.021633 autogluon-0.7.1b20230601/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:16.021633 autogluon-0.7.1b20230601/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:16.021633 autogluon-0.7.1b20230601/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:03:27.000000 autogluon-0.7.1b20230601/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:16.021633 autogluon-0.7.1b20230601/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-06-01 09:04:15.000000 autogluon-0.7.1b20230601/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-01 09:04:15.000000 autogluon-0.7.1b20230601/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:04:15.000000 autogluon-0.7.1b20230601/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:04:15.000000 autogluon-0.7.1b20230601/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-01 09:04:15.000000 autogluon-0.7.1b20230601/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:04:15.000000 autogluon-0.7.1b20230601/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:04:15.000000 autogluon-0.7.1b20230601/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.7.1b20230531/PKG-INFO` & `autogluon-0.7.1b20230601/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230531
+Version: 0.7.1b20230601
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.7.1b20230531/setup.py` & `autogluon-0.7.1b20230601/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.7.1b20230531/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.7.1b20230601/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230531
+Version: 0.7.1b20230601
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

