# Comparing `tmp/config_patterns-1.0.1.tar.gz` & `tmp/config_patterns-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_patterns-1.0.1.tar", last modified: Wed May 17 15:54:57 2023, max compression
+gzip compressed data, was "config_patterns-1.0.2.tar", last modified: Thu Jun  1 15:08:01 2023, max compression
```

## Comparing `config_patterns-1.0.1.tar` & `config_patterns-1.0.2.tar`

### file list

```diff
@@ -1,51 +1,65 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.189868 config_patterns-1.0.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 01:08:10.000000 config_patterns-1.0.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-12 01:08:10.000000 config_patterns-1.0.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-12 01:08:10.000000 config_patterns-1.0.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4016 2023-05-17 15:54:57.189713 config_patterns-1.0.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2892 2023-05-12 01:08:10.000000 config_patterns-1.0.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.184085 config_patterns-1.0.1/config_patterns/
--rw-r--r--   0 sanhehu    (501) staff       (20)      303 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-17 15:54:41.000000 config_patterns-1.0.1/config_patterns/_version.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.185615 config_patterns-1.0.1/config_patterns/aws/
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/aws/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5169 2023-05-12 16:38:32.000000 config_patterns-1.0.1/config_patterns/aws/s3.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2792 2023-05-12 16:35:47.000000 config_patterns-1.0.1/config_patterns/aws/ssm.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.185883 config_patterns-1.0.1/config_patterns/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-05-17 07:06:41.000000 config_patterns-1.0.1/config_patterns/jsonutils.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      182 2023-05-12 03:09:13.000000 config_patterns-1.0.1/config_patterns/logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      724 2023-05-12 03:09:31.000000 config_patterns-1.0.1/config_patterns/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.186513 config_patterns-1.0.1/config_patterns/patterns/
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/patterns/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4585 2023-05-17 07:06:29.000000 config_patterns-1.0.1/config_patterns/patterns/hierarchy.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3213 2023-05-17 07:29:04.000000 config_patterns-1.0.1/config_patterns/patterns/merge_key_value.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.187104 config_patterns-1.0.1/config_patterns/patterns/multi_env_json/
--rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-05-17 14:16:39.000000 config_patterns-1.0.1/config_patterns/patterns/multi_env_json/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    23831 2023-05-17 15:47:41.000000 config_patterns-1.0.1/config_patterns/patterns/multi_env_json/impl.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.187943 config_patterns-1.0.1/config_patterns/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      149 2023-05-12 03:10:02.000000 config_patterns-1.0.1/config_patterns/tests/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1216 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.189082 config_patterns-1.0.1/config_patterns/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-17 15:41:42.000000 config_patterns-1.0.1/config_patterns/vendor/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 15:37:26.000000 config_patterns-1.0.1/config_patterns/vendor/nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    44420 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/vendor/strutils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.184805 config_patterns-1.0.1/config_patterns.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4016 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1137 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      438 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2912 2023-05-17 15:41:07.000000 config_patterns-1.0.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)       73 2023-05-12 18:03:12.000000 config_patterns-1.0.1/requirements-aws.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-12 01:08:10.000000 config_patterns-1.0.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-12 01:08:10.000000 config_patterns-1.0.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-12 16:53:20.000000 config_patterns-1.0.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       65 2023-05-12 01:08:10.000000 config_patterns-1.0.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-17 15:54:57.189912 config_patterns-1.0.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7961 2023-05-12 01:08:10.000000 config_patterns-1.0.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.189411 config_patterns-1.0.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      258 2023-05-12 01:08:10.000000 config_patterns-1.0.1/tests/test_import.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.442141 config_patterns-1.0.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 01:08:10.000000 config_patterns-1.0.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-12 01:08:10.000000 config_patterns-1.0.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-12 01:08:10.000000 config_patterns-1.0.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5322 2023-06-01 15:08:01.441982 config_patterns-1.0.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4169 2023-06-01 14:23:44.000000 config_patterns-1.0.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.434432 config_patterns-1.0.2/config_patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      361 2023-06-01 14:22:10.000000 config_patterns-1.0.2/config_patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-17 15:55:27.000000 config_patterns-1.0.2/config_patterns/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      252 2023-06-01 05:06:26.000000 config_patterns-1.0.2/config_patterns/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.435962 config_patterns-1.0.2/config_patterns/aws/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-1.0.2/config_patterns/aws/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      337 2023-06-01 05:05:25.000000 config_patterns-1.0.2/config_patterns/aws/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16647 2023-06-01 13:51:58.000000 config_patterns-1.0.2/config_patterns/aws/s3.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2792 2023-05-12 16:35:47.000000 config_patterns-1.0.2/config_patterns/aws/ssm.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-05-12 01:08:10.000000 config_patterns-1.0.2/config_patterns/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.436180 config_patterns-1.0.2/config_patterns/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-12 01:08:10.000000 config_patterns-1.0.2/config_patterns/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      378 2023-06-01 13:46:33.000000 config_patterns-1.0.2/config_patterns/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-05-17 07:06:41.000000 config_patterns-1.0.2/config_patterns/jsonutils.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      181 2023-05-30 16:57:44.000000 config_patterns-1.0.2/config_patterns/logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      724 2023-05-12 03:09:31.000000 config_patterns-1.0.2/config_patterns/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.436317 config_patterns-1.0.2/config_patterns/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-01 04:56:48.000000 config_patterns-1.0.2/config_patterns/patterns/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.436928 config_patterns-1.0.2/config_patterns/patterns/hierarchy/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       24 2023-06-01 05:00:26.000000 config_patterns-1.0.2/config_patterns/patterns/hierarchy/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      109 2023-06-01 04:59:14.000000 config_patterns-1.0.2/config_patterns/patterns/hierarchy/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4585 2023-05-17 07:06:29.000000 config_patterns-1.0.2/config_patterns/patterns/hierarchy/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.437687 config_patterns-1.0.2/config_patterns/patterns/merge_key_value/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       24 2023-06-01 05:00:23.000000 config_patterns-1.0.2/config_patterns/patterns/merge_key_value/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       68 2023-06-01 05:01:05.000000 config_patterns-1.0.2/config_patterns/patterns/merge_key_value/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3213 2023-05-17 07:29:04.000000 config_patterns-1.0.2/config_patterns/patterns/merge_key_value/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.438448 config_patterns-1.0.2/config_patterns/patterns/multi_env_json/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       24 2023-05-30 16:57:14.000000 config_patterns-1.0.2/config_patterns/patterns/multi_env_json/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-05-30 16:57:10.000000 config_patterns-1.0.2/config_patterns/patterns/multi_env_json/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    24950 2023-06-01 13:47:26.000000 config_patterns-1.0.2/config_patterns/patterns/multi_env_json/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.439467 config_patterns-1.0.2/config_patterns/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-12 01:08:10.000000 config_patterns-1.0.2/config_patterns/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      149 2023-05-12 03:10:02.000000 config_patterns-1.0.2/config_patterns/tests/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      460 2023-05-30 18:53:22.000000 config_patterns-1.0.2/config_patterns/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-05-30 13:44:03.000000 config_patterns-1.0.2/config_patterns/tests/mock.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      277 2023-06-01 04:44:23.000000 config_patterns-1.0.2/config_patterns/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.441170 config_patterns-1.0.2/config_patterns/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-12 01:08:10.000000 config_patterns-1.0.2/config_patterns/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-17 15:41:42.000000 config_patterns-1.0.2/config_patterns/vendor/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-30 15:18:56.000000 config_patterns-1.0.2/config_patterns/vendor/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-30 18:52:02.000000 config_patterns-1.0.2/config_patterns/vendor/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    44420 2023-05-12 01:08:10.000000 config_patterns-1.0.2/config_patterns/vendor/strutils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.435179 config_patterns-1.0.2/config_patterns.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5322 2023-06-01 15:08:01.000000 config_patterns-1.0.2/config_patterns.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1574 2023-06-01 15:08:01.000000 config_patterns-1.0.2/config_patterns.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-01 15:08:01.000000 config_patterns-1.0.2/config_patterns.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      483 2023-06-01 15:08:01.000000 config_patterns-1.0.2/config_patterns.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-06-01 15:08:01.000000 config_patterns-1.0.2/config_patterns.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3498 2023-06-01 14:37:51.000000 config_patterns-1.0.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-05-30 14:36:35.000000 config_patterns-1.0.2/requirements-aws.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-12 01:08:10.000000 config_patterns-1.0.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-12 01:08:10.000000 config_patterns-1.0.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-12 16:53:20.000000 config_patterns-1.0.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       65 2023-05-12 01:08:10.000000 config_patterns-1.0.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-01 15:08:01.442199 config_patterns-1.0.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7506 2023-05-30 14:37:27.000000 config_patterns-1.0.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-01 15:08:01.441690 config_patterns-1.0.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      659 2023-06-01 05:07:29.000000 config_patterns-1.0.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      258 2023-05-12 01:08:10.000000 config_patterns-1.0.2/tests/test_import.py
```

### Comparing `config_patterns-1.0.1/LICENSE.txt` & `config_patterns-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/PKG-INFO` & `config_patterns-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: config_patterns
-Version: 1.0.1
-Summary: Implement common config management patterns.
+Version: 1.0.2
+Summary: Brings config management best practices for production-ready application.
 Home-page: https://github.com/MacHu-GWU/config_patterns-project
-Download-URL: https://pypi.python.org/pypi/config_patterns/1.0.1#downloads
+Download-URL: https://pypi.python.org/pypi/config_patterns/1.0.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -47,14 +47,17 @@
 
 .. image:: https://img.shields.io/pypi/l/config_patterns.svg
     :target: https://pypi.python.org/pypi/config_patterns
 
 .. image:: https://img.shields.io/pypi/pyversions/config_patterns.svg
     :target: https://pypi.python.org/pypi/config_patterns
 
+.. image:: https://img.shields.io/pypi/dm/config_patterns.svg
+    :target: https://pypi.python.org/pypi/config_patterns
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/config_patterns-project
 
 ------
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
     :target: https://config_patterns.readthedocs.io/index.html
@@ -79,18 +82,21 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/config_patterns#files
 
 
 Welcome to ``config_patterns`` Documentation
 ==============================================================================
-``config_patterns`` is a Python library that simplify your config management for production-ready application.
-
-1. `Multi Environment Json <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/multi_env_json/example.ipynb>`_: allows you to manage configs for multi-environment deployment application, use AWS Parameter Store or AWS S3 as the backend.
+``config_patterns`` is a Python library that brings config management best practices for production-ready application.
 
+1. `Hierarchy Json Pattern for Config Management <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/separate_and_merge_non_sesitive_and_sensitive_data_example.ipynb>`_: allows you to define a hierarchy structure of your config data model, and inherit global config values if a specific config value is not defined.
+2. `Separate and Merge Non-Sensitive Data and Secret Data <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/hierarchy_json_example.ipynb>`_: allows you to manage non-sensitive config data and sensitive config data separately and merge them together.
+3. `Multi Environment Json <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/multi_env_json/example.ipynb>`_: allows you to manage configs for multi-environment deployment application.
+4. `Multi Environment Config Management - SSM Backend <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/multi_env_json/multi_environment_config_with_ssm_backend.ipynb>`_: a production ready solution using AWS Parameter Store as the backend for multi-environment config management.
+5. `Multi Environment Config Management - S3 Backend <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/multi_env_json/multi_environment_config_with_s3_backend.ipynb>`_: a production ready solution using AWS S3 as the backend for multi-environment config management.
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``config_patterns`` is released on PyPI, so all you need is:
```

### Comparing `config_patterns-1.0.1/config_patterns/aws/ssm.py` & `config_patterns-1.0.2/config_patterns/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/config_patterns/jsonutils.py` & `config_patterns-1.0.2/config_patterns/jsonutils.py`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/config_patterns/paths.py` & `config_patterns-1.0.2/config_patterns/paths.py`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/config_patterns/patterns/hierarchy.py` & `config_patterns-1.0.2/config_patterns/patterns/hierarchy/impl.py`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/config_patterns/patterns/merge_key_value.py` & `config_patterns-1.0.2/config_patterns/patterns/merge_key_value/impl.py`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/config_patterns/patterns/multi_env_json/impl.py` & `config_patterns-1.0.2/config_patterns/patterns/multi_env_json/impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 import copy
-import enum
 import string
 import dataclasses
 from pathlib import Path
 
 # import optional dependencies
 try:
     import boto3
     import boto_session_manager
 except ImportError:  # pragma: no cover
     pass
 
 try:
     import pysecret
     import aws_console_url
+    from s3pathlib import S3Path
 
     from ...aws.ssm import deploy_parameter, delete_parameter
-    from ...aws.s3 import deploy_config, delete_config, S3Object
+    from ...aws.s3 import (
+        get_bucket_version_status,
+        read_config,
+        deploy_config,
+        delete_config,
+        S3Object,
+    )
 except ImportError:  # pragma: no cover
     pass
 
+from ... import exc
 from ...logger import logger
 from ...jsonutils import json_loads
 from ...compat import cached_property
+from ...utils import sha256_of_config_data
 from ...vendor.strutils import slugify
 from ...vendor.better_enum import BetterStrEnum
-from ..hierarchy import apply_shared_value
-from ..merge_key_value import merge_key_value
+from ..hierarchy.api import apply_shared_value
+from ..merge_key_value.api import merge_key_value
 
 
 def validate_project_name(project_name: str):
     if project_name[0] not in string.ascii_lowercase:
         raise ValueError("first letter of project_name has to be a-z!")
     if project_name[-1] not in (string.ascii_lowercase + string.digits):
         raise ValueError("last letter of project_name has to be a-z, 0-9!")
@@ -215,18 +223,24 @@
         tags: T.Optional[T.Dict[str, str]] = None,
         verbose: bool = True,
     ):
         """
         Deploy config to AWS SSM Parameter Store.
         """
         if tags is None:
-            tags = dict(
-                ProjectName=self.project_name,
-                EnvName=self.env_name,
-            )
+            tags = {}
+
+        tags.update(
+            {
+                "config_pattern:project_name": self.project_name,
+                "config_pattern:env_name": self.env_name,
+                "config_pattern:config_sha256": sha256_of_config_data(self.parameter_data)
+            }
+        )
+
         with logger.disabled(
             disable=not verbose,
         ):
             self.deployment = deploy_parameter(
                 bsm=bsm,
                 parameter_name=self.parameter_name,
                 parameter_data=self.parameter_data,
@@ -234,32 +248,38 @@
                 tags=tags,
             )
             return self.deployment
 
     def deploy_to_s3(
         self,
         bsm: "boto_session_manager.BotoSesManager",
-        s3dir_config: str,
+        s3folder_config: str,
         tags: T.Optional[T.Dict[str, str]] = None,
         verbose: bool = True,
     ):
         """
         Deploy config to AWS S3.
         """
         if tags is None:
-            tags = dict(
-                ProjectName=self.project_name,
-                EnvName=self.env_name,
-            )
+            tags = {}
+
+        tags.update(
+            {
+                "config_pattern:project_name": self.project_name,
+                "config_pattern:env_name": self.env_name,
+            }
+        )
+
         with logger.disabled(
             disable=not verbose,
         ):
             self.deployment = deploy_config(
                 bsm=bsm,
-                s3path_config=f"{s3dir_config}{self.parameter_name_for_arn}.json",
+                s3folder_config=S3Path(s3folder_config).to_dir().uri,
+                parameter_name=self.parameter_name_for_arn,
                 config_data=self.parameter_data,
                 tags=tags,
             )
             return self.deployment
 
     def delete_from_ssm_parameter(
         self,
@@ -277,27 +297,29 @@
                 parameter_name=self.parameter_name,
             )
             return self.deletion
 
     def delete_from_s3(
         self,
         bsm: "boto_session_manager.BotoSesManager",
-        s3dir_config: str,
+        s3folder_config: str,
+        include_history: bool = False,
         verbose: bool = True,
     ):
         """
         Delete config from AWS S3.
         """
         with logger.disabled(
             disable=not verbose,
         ):
-            s3_uri = f"{s3dir_config}{self.parameter_name_for_arn}.json"
             self.deletion = delete_config(
                 bsm=bsm,
-                s3path_config=s3_uri,
+                s3folder_config=S3Path(s3folder_config).to_dir().uri,
+                parameter_name=self.parameter_name_for_arn,
+                include_history=include_history,
             )
             return self.deletion
 
 
 @dataclasses.dataclass
 class BaseConfig:
     """
@@ -332,14 +354,16 @@
 
     data: dict = dataclasses.field()
     secret_data: dict = dataclasses.field()
 
     Env: T.Type[BaseEnv] = dataclasses.field()
     EnvEnum: T.Type[BaseEnvEnum] = dataclasses.field()
 
+    version: str = dataclasses.field()
+
     _applied_data: dict = dataclasses.field(init=False)
     _applied_secret_data: dict = dataclasses.field(init=False)
     _merged: dict = dataclasses.field(init=False)
 
     def _validate(self):
         """
         Validate input arguments.
@@ -454,80 +478,85 @@
         env_class: T.Type[BaseEnv],
         env_enum_class: T.Type[BaseEnvEnum],
         path_config: T.Optional[str] = None,
         path_secret_config: T.Optional[str] = None,
         bsm: T.Optional["boto_session_manager.BotoSesManager"] = None,
         parameter_name: T.Optional[str] = None,
         parameter_with_encryption: T.Optional[bool] = None,
-        s3path_config: T.Optional[str] = None,
+        s3folder_config: T.Optional[str] = None,
     ):
         """
         Create and initialize the config object from configuration store.
         Currently, it supports:
 
         1. read from local config files.
-        2. read from AWS Parameter Store.
+        2. read from AWS Parameter Store. You have to specify
         3. read from AWS S3.
 
         :param env_class: the per environment config dataclass object.
         :param env_enum_class: the environment enumeration class.
         :param path_config: local file path to the non-sensitive config file.
         :param path_secret_config: local file path to the sensitive config file.
         :param parameter_name: the AWS Parameter name.
         :param parameter_with_encryption: is AWS Parameter turned on encryption?
-        :param s3path_config: the s3 uri to the config file.
+        :param s3folder_config: the s3 folder uri where you store the config file.
         :return:
         """
         if (path_config is not None) and (path_secret_config is not None):
             data = json_loads(Path(path_config).read_text())
             secret_data = json_loads(Path(path_secret_config).read_text())
             return cls(
                 data=data,
                 secret_data=secret_data,
                 Env=env_class,
                 EnvEnum=env_enum_class,
+                version="local",
             )
         elif (parameter_name is not None) and (
             parameter_with_encryption is not None
         ):  # pragma: no cover
             parameter = pysecret.Parameter.load(
                 ssm_client=bsm.ssm_client,
                 name=parameter_name,
                 with_decryption=parameter_with_encryption,
             )
+            if parameter is None:
+                raise exc.ParameterNotExists(f"SSM Parameter {parameter_name!r} not exist!")
             parameter_data = parameter.json_dict
             return cls(
                 data=parameter_data["data"],
                 secret_data=parameter_data["secret_data"],
                 Env=env_class,
                 EnvEnum=env_enum_class,
+                version=str(parameter.Version),
             )
-        elif s3path_config is not None:  # pragma: no cover
-            parts = s3path_config.split("/", 3)
-            bucket = parts[2]
-            key = parts[3]
-            config_data = json_loads(
-                bsm.s3_client.get_object(Bucket=bucket, Key=key)["Body"]
-                .read()
-                .decode("utf-8")
+        elif (parameter_name is not None) and (
+            s3folder_config is not None
+        ):  # pragma: no cover
+            config_data, config_version = read_config(
+                bsm=bsm,
+                s3folder_config=s3folder_config,
+                parameter_name=parameter_name,
             )
             return cls(
                 data=config_data["data"],
                 secret_data=config_data["secret_data"],
                 Env=env_class,
                 EnvEnum=env_enum_class,
+                version=config_version,
             )
         else:
             raise ValueError(
                 "The arguments has to meet one of these criteria:\n"
                 "1. set both ``path_config`` and ``path_secret_config`` to indicate that "
                 "you want to read config from local config json file.\n"
                 "2. set both ``parameter_name`` and ``parameter_with_encryption`` "
                 "to indicate that you want to read from AWS Parameter Store.\n"
-                "3. set ``s3path_config`` similar to s3://my-bucket/my-project/dev.json "
+                "3. set both ``parameter_name`` similar to 'my-project-dev' "
+                "and ``s3folder_config`` similar to s3://my-bucket/my-project/ "
                 "to indicate that you want to read from AWS S3.\n"
             )
 
     def prepare_deploy(self) -> T.List[ConfigDeployment]:
         """
         split the consolidated config into per environment config.
 
@@ -583,15 +612,15 @@
 
         return deployment_list
 
     def deploy(
         self,
         bsm: "boto_session_manager.BotoSesManager",
         parameter_with_encryption: T.Optional[bool] = None,
-        s3dir_config: T.Optional[str] = None,
+        s3folder_config: T.Optional[str] = None,
         tags: T.Optional[T.Dict[str, str]] = None,
         verbose: bool = True,
     ) -> T.List[ConfigDeployment]:
         """
         Deploy the project config of all environments to configuration store.
         Currently, it supports:
 
@@ -600,15 +629,15 @@
 
         Note:
 
             this function should ONLY run from the project admin's trusted laptop.
 
         :param bsm:
         :param parameter_with_encryption:
-        :param s3dir_config:
+        :param s3folder_config:
         :param tags:
         :param verbose:
 
         :return: a list of :class:`ConfigDeployment`.
         """
         if parameter_with_encryption is not None:
             # validate arguments
@@ -622,51 +651,53 @@
                 deployment.deploy_to_ssm_parameter(
                     bsm=bsm,
                     parameter_with_encryption=parameter_with_encryption,
                     tags=tags,
                     verbose=verbose,
                 )
             return deployment_list
-        elif s3dir_config is not None:
+        elif s3folder_config is not None:
             deployment_list = self.prepare_deploy()
             for deployment in deployment_list:
                 deployment.deploy_to_s3(
                     bsm=bsm,
-                    s3dir_config=s3dir_config,
+                    s3folder_config=s3folder_config,
                     tags=tags,
                     verbose=verbose,
                 )
             return deployment_list
         else:
             raise ValueError(
                 "The arguments has to meet one of these criteria:\n"
                 "1. set ``parameter_with_encryption`` to True or False to indicate that "
                 "you want to deploy to AWS Parameter Store.\n"
-                "2. set ``s3dir_config`` similar to s3://my-bucket/my-project/ "
+                "2. set ``s3folder_config`` similar to s3://my-bucket/my-project/ "
                 "to indicate that you want to deploy to S3."
             )
 
     def delete(
         self,
         bsm: "boto_session_manager.BotoSesManager",
         use_parameter_store: T.Optional[bool] = None,
-        s3dir_config: T.Optional[str] = None,
+        s3folder_config: T.Optional[str] = None,
+        include_history: bool = False,
         verbose: bool = True,
     ):
         """
         Delete the all project config of all environments from configuration store.
 
         Currently, it supports:
 
         1. delete from AWS Parameter Store
         2. delete from AWS S3
 
         :param bsm:
         :param use_parameter_store:
-        :param s3dir_config:
+        :param s3folder_config:
+        :param include_history:
         :param verbose:
 
         :return: a list of :class:`ConfigDeployment`.
 
         Note:
 
             this function should ONLY run from the project admin's trusted laptop.
@@ -675,24 +706,25 @@
             deployment_list = self.prepare_deploy()
             for deployment in deployment_list:
                 deployment.delete_from_ssm_parameter(
                     bsm=bsm,
                     verbose=verbose,
                 )
             return deployment_list
-        elif (bsm is not None) and (s3dir_config is not None):
+        elif (bsm is not None) and (s3folder_config is not None):
             deployment_list = self.prepare_deploy()
             for deployment in deployment_list:
                 deployment.delete_from_s3(
                     bsm=bsm,
-                    s3dir_config=s3dir_config,
+                    s3folder_config=s3folder_config,
+                    include_history=include_history,
                     verbose=verbose,
                 )
             return deployment_list
         else:
             raise ValueError(
                 "The arguments has to meet one of these criteria:\n"
                 "1. set ``use_parameter_store`` to True to indicate that "
                 "you want to delete config from AWS Parameter Store.\n"
-                "2. set ``s3dir_config`` similar to s3://my-bucket/my-project/ "
+                "2. set ``s3folder_config`` similar to s3://my-bucket/my-project/ "
                 "to indicate that you want to delete config file from S3."
             )
```

### Comparing `config_patterns-1.0.1/config_patterns/vendor/better_enum.py` & `config_patterns-1.0.2/config_patterns/vendor/better_enum.py`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/config_patterns/vendor/nest_logger.py` & `config_patterns-1.0.2/config_patterns/vendor/nest_logger.py`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/config_patterns/vendor/strutils.py` & `config_patterns-1.0.2/config_patterns/vendor/strutils.py`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/config_patterns.egg-info/PKG-INFO` & `config_patterns-1.0.2/config_patterns.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: config-patterns
-Version: 1.0.1
-Summary: Implement common config management patterns.
+Version: 1.0.2
+Summary: Brings config management best practices for production-ready application.
 Home-page: https://github.com/MacHu-GWU/config_patterns-project
-Download-URL: https://pypi.python.org/pypi/config_patterns/1.0.1#downloads
+Download-URL: https://pypi.python.org/pypi/config_patterns/1.0.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -47,14 +47,17 @@
 
 .. image:: https://img.shields.io/pypi/l/config_patterns.svg
     :target: https://pypi.python.org/pypi/config_patterns
 
 .. image:: https://img.shields.io/pypi/pyversions/config_patterns.svg
     :target: https://pypi.python.org/pypi/config_patterns
 
+.. image:: https://img.shields.io/pypi/dm/config_patterns.svg
+    :target: https://pypi.python.org/pypi/config_patterns
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/config_patterns-project
 
 ------
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
     :target: https://config_patterns.readthedocs.io/index.html
@@ -79,18 +82,21 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/config_patterns#files
 
 
 Welcome to ``config_patterns`` Documentation
 ==============================================================================
-``config_patterns`` is a Python library that simplify your config management for production-ready application.
-
-1. `Multi Environment Json <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/multi_env_json/example.ipynb>`_: allows you to manage configs for multi-environment deployment application, use AWS Parameter Store or AWS S3 as the backend.
+``config_patterns`` is a Python library that brings config management best practices for production-ready application.
 
+1. `Hierarchy Json Pattern for Config Management <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/separate_and_merge_non_sesitive_and_sensitive_data_example.ipynb>`_: allows you to define a hierarchy structure of your config data model, and inherit global config values if a specific config value is not defined.
+2. `Separate and Merge Non-Sensitive Data and Secret Data <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/hierarchy_json_example.ipynb>`_: allows you to manage non-sensitive config data and sensitive config data separately and merge them together.
+3. `Multi Environment Json <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/multi_env_json/example.ipynb>`_: allows you to manage configs for multi-environment deployment application.
+4. `Multi Environment Config Management - SSM Backend <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/multi_env_json/multi_environment_config_with_ssm_backend.ipynb>`_: a production ready solution using AWS Parameter Store as the backend for multi-environment config management.
+5. `Multi Environment Config Management - S3 Backend <https://github.com/MacHu-GWU/config_patterns-project/blob/main/example/multi_env_json/multi_environment_config_with_s3_backend.ipynb>`_: a production ready solution using AWS S3 as the backend for multi-environment config management.
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``config_patterns`` is released on PyPI, so all you need is:
```

### Comparing `config_patterns-1.0.1/config_patterns.egg-info/SOURCES.txt` & `config_patterns-1.0.2/config_patterns.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,33 +7,45 @@
 requirements-dev.txt
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 config_patterns/__init__.py
 config_patterns/_version.py
+config_patterns/api.py
 config_patterns/compat.py
+config_patterns/exc.py
 config_patterns/jsonutils.py
 config_patterns/logger.py
 config_patterns/paths.py
+config_patterns/utils.py
 config_patterns.egg-info/PKG-INFO
 config_patterns.egg-info/SOURCES.txt
 config_patterns.egg-info/dependency_links.txt
 config_patterns.egg-info/requires.txt
 config_patterns.egg-info/top_level.txt
 config_patterns/aws/__init__.py
+config_patterns/aws/api.py
 config_patterns/aws/s3.py
 config_patterns/aws/ssm.py
 config_patterns/docs/__init__.py
 config_patterns/patterns/__init__.py
-config_patterns/patterns/hierarchy.py
-config_patterns/patterns/merge_key_value.py
+config_patterns/patterns/hierarchy/__init__.py
+config_patterns/patterns/hierarchy/api.py
+config_patterns/patterns/hierarchy/impl.py
+config_patterns/patterns/merge_key_value/__init__.py
+config_patterns/patterns/merge_key_value/api.py
+config_patterns/patterns/merge_key_value/impl.py
 config_patterns/patterns/multi_env_json/__init__.py
+config_patterns/patterns/multi_env_json/api.py
 config_patterns/patterns/multi_env_json/impl.py
 config_patterns/tests/__init__.py
 config_patterns/tests/boto_ses.py
 config_patterns/tests/helper.py
+config_patterns/tests/mock.py
 config_patterns/vendor/__init__.py
 config_patterns/vendor/better_enum.py
 config_patterns/vendor/nest_logger.py
+config_patterns/vendor/pytest_cov_helper.py
 config_patterns/vendor/strutils.py
+tests/test_api.py
 tests/test_import.py
```

### Comparing `config_patterns-1.0.1/release-history.rst` & `config_patterns-1.0.2/release-history.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,42 @@
 .. _release_history:
 
 Release and Version History
 ==============================================================================
 
 
-Backlog (TODO)
+1.1.1 (TODO)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
+- prepare for the first API stable release.
+
+**Minor Improvements**
+
+**Bugfixes**
+
+**Miscellaneous**
+
+
+1.0.2 (2023-06-01)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add support to use version enabled S3 bucket as the backend.
+- now keep all historical versions of the config files in version not enabled S3 bucket.
+- add code_sha256 to the S3 object metadata for integrity check.
+- add ``api`` module to expose stable APIs to public.
+
 **Minor Improvements**
 
+- rewrite the documents. Now the documents are more clear and easy to understand.
+
 **Bugfixes**
 
+
 **Miscellaneous**
 
 
 1.0.1 (2023-05-17)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Breaking Changes**
```

### Comparing `config_patterns-1.0.1/requirements-doc.txt` & `config_patterns-1.0.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `config_patterns-1.0.1/setup.py` & `config_patterns-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,33 +149,18 @@
         REQUIRES = read_requirements_file("requirements.txt")
     except:
         print("'requirements.txt' not found!")
         REQUIRES = list()
 
     EXTRA_REQUIRE = dict()
 
-    try:
-        EXTRA_REQUIRE["dev"] = read_requirements_file("requirements-dev.txt")
-    except:
-        print("'requirements-dev.txt' not found!")
-
-    try:
-        EXTRA_REQUIRE["test"] = read_requirements_file("requirements-test.txt")
-    except:
-        print("'requirements-test.txt' not found!")
-
-    try:
-        EXTRA_REQUIRE["doc"] = read_requirements_file("requirements-doc.txt")
-    except:
-        print("'requirements-doc.txt' not found!")
-
-    try:
-        EXTRA_REQUIRE["aws"] = read_requirements_file("requirements-aws.txt")
-    except:
-        print("'requirements-aws.txt' not found!")
+    EXTRA_REQUIRE["dev"] = read_requirements_file("requirements-dev.txt")
+    EXTRA_REQUIRE["test"] = read_requirements_file("requirements-test.txt")
+    EXTRA_REQUIRE["doc"] = read_requirements_file("requirements-doc.txt")
+    EXTRA_REQUIRE["aws"] = read_requirements_file("requirements-aws.txt")
 
     setup(
         name=PKG_NAME,
         description=SHORT_DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         version=VERSION,
         author=AUTHOR,
@@ -238,17 +223,14 @@
         "Operating System :: Unix",
     
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 2 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ]
 """
```

