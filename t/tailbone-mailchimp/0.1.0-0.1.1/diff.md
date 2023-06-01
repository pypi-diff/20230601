# Comparing `tmp/tailbone-mailchimp-0.1.0.tar.gz` & `tmp/tailbone-mailchimp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tailbone-mailchimp-0.1.0.tar", last modified: Tue Nov  9 17:54:36 2021, max compression
+gzip compressed data, was "dist/tailbone-mailchimp-0.1.1.tar", last modified: Thu Jun  1 19:28:22 2023, max compression
```

## Comparing `tailbone-mailchimp-0.1.0.tar` & `tailbone-mailchimp-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/
--rw-r--r--   0 lance     (1000) lance     (1000)      340 2021-11-09 17:54:18.000000 tailbone-mailchimp-0.1.0/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 tailbone-mailchimp-0.1.0/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       97 2021-11-08 19:21:33.000000 tailbone-mailchimp-0.1.0/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1116 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      349 2021-11-08 17:08:11.000000 tailbone-mailchimp-0.1.0/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     3648 2021-11-08 17:10:37.000000 tailbone-mailchimp-0.1.0/setup.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp/
--rw-r--r--   0 lance     (1000) lance     (1000)     1013 2021-11-08 17:11:01.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2021-11-08 17:11:06.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp/views/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-07-04 16:53:35.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp/views/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp/views/mailchimp/
--rw-r--r--   0 lance     (1000) lance     (1000)     1047 2021-11-08 17:12:53.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp/views/mailchimp/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2993 2021-11-08 19:25:13.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp/views/mailchimp/lists.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1116 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      496 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)       35 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       19 2021-11-09 17:54:36.000000 tailbone-mailchimp-0.1.0/tailbone_mailchimp.egg-info/top_level.txt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/
+-rw-r--r--   0 lance     (1000) lance     (1000)       97 2021-11-08 19:21:33.000000 tailbone-mailchimp-0.1.1/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)      974 2023-05-16 19:30:04.000000 tailbone-mailchimp-0.1.1/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      856 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 tailbone-mailchimp-0.1.1/COPYING.txt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)      506 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       35 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       19 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1116 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      349 2021-11-08 17:08:11.000000 tailbone-mailchimp-0.1.1/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp/views/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp/views/mailchimp/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2993 2021-11-08 19:25:13.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp/views/mailchimp/lists.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1047 2021-11-08 17:12:53.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp/views/mailchimp/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-07-04 16:53:35.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp/views/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-06-01 19:28:05.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1013 2021-11-08 17:11:01.000000 tailbone-mailchimp-0.1.1/tailbone_mailchimp/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      425 2023-06-01 19:28:01.000000 tailbone-mailchimp-0.1.1/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)     1116 2023-06-01 19:28:22.000000 tailbone-mailchimp-0.1.1/PKG-INFO
```

### Comparing `tailbone-mailchimp-0.1.0/COPYING.txt` & `tailbone-mailchimp-0.1.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `tailbone-mailchimp-0.1.0/PKG-INFO` & `tailbone-mailchimp-0.1.1/tailbone_mailchimp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailbone-mailchimp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tailbone integration for MailChimp
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tailbone-mailchimp-0.1.0/tailbone_mailchimp/__init__.py` & `tailbone-mailchimp-0.1.1/tailbone_mailchimp/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-mailchimp-0.1.0/tailbone_mailchimp/views/mailchimp/__init__.py` & `tailbone-mailchimp-0.1.1/tailbone_mailchimp/views/mailchimp/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-mailchimp-0.1.0/tailbone_mailchimp/views/mailchimp/lists.py` & `tailbone-mailchimp-0.1.1/tailbone_mailchimp/views/mailchimp/lists.py`

 * *Files identical despite different names*

### Comparing `tailbone-mailchimp-0.1.0/tailbone_mailchimp.egg-info/PKG-INFO` & `tailbone-mailchimp-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailbone-mailchimp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tailbone integration for MailChimp
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

