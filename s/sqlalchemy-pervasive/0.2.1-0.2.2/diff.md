# Comparing `tmp/sqlalchemy-pervasive-0.2.1.tar.gz` & `tmp/sqlalchemy-pervasive-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-pervasive-0.2.1.tar", last modified: Wed Mar  3 17:54:33 2021, max compression
+gzip compressed data, was "dist/sqlalchemy-pervasive-0.2.2.tar", last modified: Thu Jun  1 19:27:05 2023, max compression
```

## Comparing `sqlalchemy-pervasive-0.2.1.tar` & `sqlalchemy-pervasive-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-03-03 17:54:33.972707 sqlalchemy-pervasive-0.2.1/
--rw-r--r--   0 lance     (1000) lance     (1000)      417 2021-03-03 17:54:18.000000 sqlalchemy-pervasive-0.2.1/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2015-07-17 20:44:35.000000 sqlalchemy-pervasive-0.2.1/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       28 2015-07-17 20:44:35.000000 sqlalchemy-pervasive-0.2.1/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1679 2021-03-03 17:54:33.972707 sqlalchemy-pervasive-0.2.1/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      164 2015-07-17 20:44:35.000000 sqlalchemy-pervasive-0.2.1/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)      178 2021-03-03 17:54:33.972707 sqlalchemy-pervasive-0.2.1/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     3897 2021-03-03 17:53:34.000000 sqlalchemy-pervasive-0.2.1/setup.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-03-03 17:54:33.968707 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive/
--rw-r--r--   0 lance     (1000) lance     (1000)     1205 2021-03-03 17:47:19.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       22 2021-03-03 17:54:24.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2034 2021-03-03 17:47:10.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive/base.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1259 2021-03-03 17:47:29.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive/pyodbc.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-03-03 17:54:33.968707 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1679 2021-03-03 17:54:33.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      457 2021-03-03 17:54:33.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-03-03 17:54:33.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       89 2021-03-03 17:54:33.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       18 2021-03-03 17:54:33.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       21 2021-03-03 17:54:33.000000 sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive.egg-info/top_level.txt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/
+-rw-r--r--   0 lance     (1000) lance     (1000)       28 2015-07-17 20:44:35.000000 sqlalchemy-pervasive-0.2.2/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1075 2023-05-16 19:32:51.000000 sqlalchemy-pervasive-0.2.2/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1130 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2015-07-17 20:44:35.000000 sqlalchemy-pervasive-0.2.2/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      510 2023-06-01 19:26:37.000000 sqlalchemy-pervasive-0.2.2/CHANGES.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2034 2021-03-03 17:47:10.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive/base.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1259 2021-03-03 17:47:29.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive/pyodbc.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       22 2023-06-01 19:26:41.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1205 2021-03-03 17:47:19.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      164 2015-07-17 20:44:35.000000 sqlalchemy-pervasive-0.2.2/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      457 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       87 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       18 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       21 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      923 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      923 2023-06-01 19:27:05.000000 sqlalchemy-pervasive-0.2.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sqlalchemy-pervasive-0.2.1/COPYING.txt` & `sqlalchemy-pervasive-0.2.2/COPYING.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive/__init__.py` & `sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive/base.py` & `sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-pervasive-0.2.1/sqlalchemy_pervasive/pyodbc.py` & `sqlalchemy-pervasive-0.2.2/sqlalchemy_pervasive/pyodbc.py`

 * *Files identical despite different names*

