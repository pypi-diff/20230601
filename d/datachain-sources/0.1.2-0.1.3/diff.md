# Comparing `tmp/datachain_sources-0.1.2.tar.gz` & `tmp/datachain_sources-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datachain_sources-0.1.2.tar", max compression
+gzip compressed data, was "datachain_sources-0.1.3.tar", max compression
```

## Comparing `datachain_sources-0.1.2.tar` & `datachain_sources-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2023-06-01 01:26:19.000000 datachain_sources-0.1.2/README.md
--rw-r--r--   0        0        0       32 2023-05-31 11:13:21.000000 datachain_sources-0.1.2/datachain_sources/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-01 00:45:58.000000 datachain_sources-0.1.2/datachain_sources/_utils.py
--rw-r--r--   0        0        0       32 2023-05-31 14:27:33.000000 datachain_sources-0.1.2/datachain_sources/bytes/__init__.py
--rw-r--r--   0        0        0     1322 2023-06-01 00:35:20.000000 datachain_sources-0.1.2/datachain_sources/bytes/_pandas.py
--rw-r--r--   0        0        0      737 2023-06-01 01:29:31.000000 datachain_sources-0.1.2/datachain_sources/file.py
--rw-r--r--   0        0        0       32 2023-06-01 00:28:56.000000 datachain_sources-0.1.2/datachain_sources/files/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-01 01:29:21.000000 datachain_sources-0.1.2/datachain_sources/files/_file.py
--rw-r--r--   0        0        0     1033 2023-06-01 02:25:43.717163 datachain_sources-0.1.2/datachain_sources/files/_ftp.py
--rw-r--r--   0        0        0      843 2023-05-31 11:15:46.000000 datachain_sources-0.1.2/datachain_sources/files/_http.py
--rw-r--r--   0        0        0      624 2023-06-01 01:28:52.000000 datachain_sources-0.1.2/datachain_sources/files/_jsonfile.py
--rw-r--r--   0        0        0      442 2023-03-31 02:13:33.000000 datachain_sources-0.1.2/datachain_sources/files/_local.py
--rw-r--r--   0        0        0     3163 2023-06-01 01:50:46.000000 datachain_sources-0.1.2/datachain_sources/files/_pandas.py
--rw-r--r--   0        0        0     1266 2023-06-01 02:28:24.870909 datachain_sources-0.1.2/datachain_sources/files/_sftp.py
--rw-r--r--   0        0        0     1152 2023-06-01 02:26:17.148560 datachain_sources-0.1.2/datachain_sources/ftp.py
--rw-r--r--   0        0        0     1044 2023-06-01 01:30:03.000000 datachain_sources-0.1.2/datachain_sources/http.py
--rw-r--r--   0        0        0       32 2023-05-31 12:23:56.000000 datachain_sources-0.1.2/datachain_sources/query/__init__.py
--rw-r--r--   0        0        0     3040 2023-06-01 00:36:12.000000 datachain_sources-0.1.2/datachain_sources/query/_pandas.py
--rw-r--r--   0        0        0     1259 2023-06-01 02:26:50.890547 datachain_sources-0.1.2/datachain_sources/sftp.py
--rw-r--r--   0        0        0     1889 2023-06-01 01:53:20.000000 datachain_sources-0.1.2/datachain_sources/sharepoint.py
--rw-r--r--   0        0        0     2393 2023-06-01 01:30:20.000000 datachain_sources-0.1.2/datachain_sources/sql.py
--rw-r--r--   0        0        0     1862 2023-06-01 02:30:56.705388 datachain_sources-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 datachain_sources-0.1.2/setup.py
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 datachain_sources-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-01 01:26:19.000000 datachain_sources-0.1.3/README.md
+-rw-r--r--   0        0        0       32 2023-05-31 11:13:21.000000 datachain_sources-0.1.3/datachain_sources/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-01 00:45:58.000000 datachain_sources-0.1.3/datachain_sources/_utils.py
+-rw-r--r--   0        0        0       32 2023-05-31 14:27:33.000000 datachain_sources-0.1.3/datachain_sources/bytes/__init__.py
+-rw-r--r--   0        0        0     1322 2023-06-01 00:35:20.000000 datachain_sources-0.1.3/datachain_sources/bytes/_pandas.py
+-rw-r--r--   0        0        0      737 2023-06-01 01:29:31.000000 datachain_sources-0.1.3/datachain_sources/file.py
+-rw-r--r--   0        0        0       32 2023-06-01 00:28:56.000000 datachain_sources-0.1.3/datachain_sources/files/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-01 01:29:21.000000 datachain_sources-0.1.3/datachain_sources/files/_file.py
+-rw-r--r--   0        0        0     1033 2023-06-01 02:25:43.717163 datachain_sources-0.1.3/datachain_sources/files/_ftp.py
+-rw-r--r--   0        0        0      843 2023-05-31 11:15:46.000000 datachain_sources-0.1.3/datachain_sources/files/_http.py
+-rw-r--r--   0        0        0      624 2023-06-01 01:28:52.000000 datachain_sources-0.1.3/datachain_sources/files/_jsonfile.py
+-rw-r--r--   0        0        0      442 2023-03-31 02:13:33.000000 datachain_sources-0.1.3/datachain_sources/files/_local.py
+-rw-r--r--   0        0        0     3163 2023-06-01 01:50:46.000000 datachain_sources-0.1.3/datachain_sources/files/_pandas.py
+-rw-r--r--   0        0        0     1266 2023-06-01 02:28:24.870909 datachain_sources-0.1.3/datachain_sources/files/_sftp.py
+-rw-r--r--   0        0        0     1152 2023-06-01 02:26:17.148560 datachain_sources-0.1.3/datachain_sources/ftp.py
+-rw-r--r--   0        0        0     2030 2023-06-01 03:17:38.958840 datachain_sources-0.1.3/datachain_sources/http.py
+-rw-r--r--   0        0        0       32 2023-05-31 12:23:56.000000 datachain_sources-0.1.3/datachain_sources/query/__init__.py
+-rw-r--r--   0        0        0     3040 2023-06-01 00:36:12.000000 datachain_sources-0.1.3/datachain_sources/query/_pandas.py
+-rw-r--r--   0        0        0     1259 2023-06-01 02:26:50.890547 datachain_sources-0.1.3/datachain_sources/sftp.py
+-rw-r--r--   0        0        0     1889 2023-06-01 01:53:20.000000 datachain_sources-0.1.3/datachain_sources/sharepoint.py
+-rw-r--r--   0        0        0     2393 2023-06-01 01:30:20.000000 datachain_sources-0.1.3/datachain_sources/sql.py
+-rw-r--r--   0        0        0     1862 2023-06-01 03:18:23.658249 datachain_sources-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 datachain_sources-0.1.3/setup.py
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 datachain_sources-0.1.3/PKG-INFO
```

### Comparing `datachain_sources-0.1.2/datachain_sources/_utils.py` & `datachain_sources-0.1.3/datachain_sources/_utils.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/bytes/_pandas.py` & `datachain_sources-0.1.3/datachain_sources/bytes/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/file.py` & `datachain_sources-0.1.3/datachain_sources/file.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/files/_file.py` & `datachain_sources-0.1.3/datachain_sources/files/_file.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/files/_ftp.py` & `datachain_sources-0.1.3/datachain_sources/files/_ftp.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/files/_http.py` & `datachain_sources-0.1.3/datachain_sources/files/_http.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/files/_jsonfile.py` & `datachain_sources-0.1.3/datachain_sources/files/_jsonfile.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/files/_pandas.py` & `datachain_sources-0.1.3/datachain_sources/files/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/files/_sftp.py` & `datachain_sources-0.1.3/datachain_sources/files/_sftp.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/ftp.py` & `datachain_sources-0.1.3/datachain_sources/ftp.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/query/_pandas.py` & `datachain_sources-0.1.3/datachain_sources/query/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/sftp.py` & `datachain_sources-0.1.3/datachain_sources/sftp.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/sharepoint.py` & `datachain_sources-0.1.3/datachain_sources/sharepoint.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/datachain_sources/sql.py` & `datachain_sources-0.1.3/datachain_sources/sql.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.2/pyproject.toml` & `datachain_sources-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datachain_sources"
-version = "0.1.2"
+version = "0.1.3"
 description = "Sources for DataChain library."
 authors = ["Rayane AMROUCHE <rayaneamrouche@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 packages = [
     { include = "datachain_sources" },
```

### Comparing `datachain_sources-0.1.2/setup.py` & `datachain_sources-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'snowflake': ['sqlalchemy==1.4.46',
                'snowflake-connector-python>=2.9.0,<3.0.0',
                'snowflake-sqlalchemy>=1.4.4,<2.0.0',
                'cryptography==38.0.4']}
 
 setup_kwargs = {
     'name': 'datachain-sources',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Sources for DataChain library.',
     'long_description': '',
     'author': 'Rayane AMROUCHE',
     'author_email': 'rayaneamrouche@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `datachain_sources-0.1.2/PKG-INFO` & `datachain_sources-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datachain-sources
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sources for DataChain library.
 License: GPL-3.0-or-later
 Author: Rayane AMROUCHE
 Author-email: rayaneamrouche@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

