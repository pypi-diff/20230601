# Comparing `tmp/rattail-quickbooks-0.1.2.tar.gz` & `tmp/rattail-quickbooks-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lance/src/rattail-quickbooks/dist/tmpg20xe3c3/rattail-quickbooks-0.1.2.tar", last modified: Thu May 11 19:22:45 2023, max compression
+gzip compressed data, was "/home/lance/src/rattail-quickbooks/dist/tmpk6xfj3jr/rattail-quickbooks-0.1.3.tar", last modified: Thu Jun  1 19:29:40 2023, max compression
```

## Comparing `rattail-quickbooks-0.1.2.tar` & `rattail-quickbooks-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/
--rw-r--r--   0 lance     (1000) lance     (1000)      135 2022-12-22 02:35:45.000000 rattail-quickbooks-0.1.2/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     3542 2022-12-08 21:06:07.000000 rattail-quickbooks-0.1.2/setup.py
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/setup.cfg
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/alembic/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)     1686 2022-12-22 01:18:01.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/alembic/versions/6a6791ac0961_add_invoice_shipping_supplies.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14774 2022-12-20 23:52:46.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/alembic/versions/72134a69c576_initial_integration_tables.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     2315 2022-12-09 23:37:22.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/org.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1979 2022-12-20 22:36:04.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2412 2022-12-08 23:02:30.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/vendors.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11857 2023-05-05 06:51:14.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/invoices.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1255 2022-12-20 22:36:12.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2022-12-08 21:01:36.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-11 19:22:10.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)     2384 2022-12-21 01:41:56.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)      993 2022-12-09 23:35:30.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2066 2022-12-21 11:55:26.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/importing/versions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1010 2022-12-08 21:01:36.000000 rattail-quickbooks-0.1.2/rattail_quickbooks/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)      348 2022-12-08 21:01:36.000000 rattail-quickbooks-0.1.2/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      828 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       19 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1087 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/rattail_quickbooks.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      537 2023-05-11 19:22:06.000000 rattail-quickbooks-0.1.2/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)     1087 2023-05-11 19:22:45.000000 rattail-quickbooks-0.1.2/PKG-INFO
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/
+-rw-r--r--   0 lance     (1000) lance     (1000)      135 2022-12-22 02:35:45.000000 rattail-quickbooks-0.1.3/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1014 2023-05-16 19:36:36.000000 rattail-quickbooks-0.1.3/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      790 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/setup.cfg
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/alembic/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1686 2022-12-22 01:18:01.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/alembic/versions/6a6791ac0961_add_invoice_shipping_supplies.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14774 2022-12-20 23:52:46.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/alembic/versions/72134a69c576_initial_integration_tables.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2315 2022-12-09 23:37:22.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/org.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1979 2022-12-20 22:36:04.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2412 2022-12-08 23:02:30.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/vendors.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11857 2023-05-05 06:51:14.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/invoices.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1255 2022-12-20 22:36:12.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2022-12-08 21:01:36.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-06-01 19:29:19.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2384 2022-12-21 01:41:56.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      993 2022-12-09 23:35:30.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2066 2022-12-21 11:55:26.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/importing/versions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1010 2022-12-08 21:01:36.000000 rattail-quickbooks-0.1.3/rattail_quickbooks/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      348 2022-12-08 21:01:36.000000 rattail-quickbooks-0.1.3/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      838 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       19 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1087 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/rattail_quickbooks.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      622 2023-06-01 19:29:16.000000 rattail-quickbooks-0.1.3/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)     1087 2023-06-01 19:29:40.000000 rattail-quickbooks-0.1.3/PKG-INFO
```

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/db/alembic/versions/6a6791ac0961_add_invoice_shipping_supplies.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/db/alembic/versions/6a6791ac0961_add_invoice_shipping_supplies.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/db/alembic/versions/72134a69c576_initial_integration_tables.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/db/alembic/versions/72134a69c576_initial_integration_tables.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/org.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/org.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/stores.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/stores.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/vendors.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/vendors.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/invoices.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/invoices.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/db/model/__init__.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/importing/model.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/importing/model.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/importing/__init__.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/importing/versions.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/importing/versions.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks/__init__.py` & `rattail-quickbooks-0.1.3/rattail_quickbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks.egg-info/SOURCES.txt` & `rattail-quickbooks-0.1.3/rattail_quickbooks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGELOG.md
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 rattail_quickbooks/__init__.py
 rattail_quickbooks/_version.py
 rattail_quickbooks.egg-info/PKG-INFO
 rattail_quickbooks.egg-info/SOURCES.txt
 rattail_quickbooks.egg-info/dependency_links.txt
 rattail_quickbooks.egg-info/requires.txt
```

### Comparing `rattail-quickbooks-0.1.2/rattail_quickbooks.egg-info/PKG-INFO` & `rattail-quickbooks-0.1.3/rattail_quickbooks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-quickbooks
-Version: 0.1.2
+Version: 0.1.3
 Summary: Rattail integration package for Quickbooks
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rattail-quickbooks-0.1.2/CHANGELOG.md` & `rattail-quickbooks-0.1.3/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
 # Changelog
 All notable changes to rattail-quickbooks will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.1.3] - 2023-06-01
+### Changed
+- Replace `setup.py` contents with `setup.cfg`.
+
 ## [0.1.2] - 2023-05-11
 ### Changed
 - Avoid deprecated import for `OrderedDict`.
 
 ## [0.1.1] - 2022-12-21
 ### Changed
 - Include alembic version scripts in built dist.
```

### Comparing `rattail-quickbooks-0.1.2/PKG-INFO` & `rattail-quickbooks-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-quickbooks
-Version: 0.1.2
+Version: 0.1.3
 Summary: Rattail integration package for Quickbooks
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

