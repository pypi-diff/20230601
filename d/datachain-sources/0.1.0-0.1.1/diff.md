# Comparing `tmp/datachain_sources-0.1.0.tar.gz` & `tmp/datachain_sources-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datachain_sources-0.1.0.tar", max compression
+gzip compressed data, was "datachain_sources-0.1.1.tar", max compression
```

## Comparing `datachain_sources-0.1.0.tar` & `datachain_sources-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2023-06-01 01:26:19.859742 datachain_sources-0.1.0/README.md
--rw-r--r--   0        0        0       32 2023-05-31 11:13:21.461420 datachain_sources-0.1.0/datachain_sources/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-01 00:45:58.852159 datachain_sources-0.1.0/datachain_sources/_utils.py
--rw-r--r--   0        0        0       32 2023-05-31 14:27:33.860480 datachain_sources-0.1.0/datachain_sources/bytes/__init__.py
--rw-r--r--   0        0        0     1322 2023-06-01 00:35:20.042249 datachain_sources-0.1.0/datachain_sources/bytes/_pandas.py
--rw-r--r--   0        0        0      737 2023-06-01 01:29:31.192827 datachain_sources-0.1.0/datachain_sources/file.py
--rw-r--r--   0        0        0       32 2023-06-01 00:28:56.862995 datachain_sources-0.1.0/datachain_sources/files/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-01 01:29:21.878284 datachain_sources-0.1.0/datachain_sources/files/_file.py
--rw-r--r--   0        0        0      972 2023-03-31 02:14:16.000000 datachain_sources-0.1.0/datachain_sources/files/_ftp.py
--rw-r--r--   0        0        0      843 2023-05-31 11:15:46.822209 datachain_sources-0.1.0/datachain_sources/files/_http.py
--rw-r--r--   0        0        0      624 2023-06-01 01:28:52.178966 datachain_sources-0.1.0/datachain_sources/files/_jsonfile.py
--rw-r--r--   0        0        0      442 2023-03-31 02:13:33.000000 datachain_sources-0.1.0/datachain_sources/files/_local.py
--rw-r--r--   0        0        0     3097 2023-06-01 01:29:00.648918 datachain_sources-0.1.0/datachain_sources/files/_pandas.py
--rw-r--r--   0        0        0     1205 2023-03-31 02:14:23.000000 datachain_sources-0.1.0/datachain_sources/files/_sftp.py
--rw-r--r--   0        0        0     1100 2023-06-01 01:29:46.912109 datachain_sources-0.1.0/datachain_sources/ftp.py
--rw-r--r--   0        0        0     1044 2023-06-01 01:30:03.611089 datachain_sources-0.1.0/datachain_sources/http.py
--rw-r--r--   0        0        0       32 2023-05-31 12:23:56.344417 datachain_sources-0.1.0/datachain_sources/query/__init__.py
--rw-r--r--   0        0        0     3040 2023-06-01 00:36:12.838156 datachain_sources-0.1.0/datachain_sources/query/_pandas.py
--rw-r--r--   0        0        0     1187 2023-06-01 01:30:07.584911 datachain_sources-0.1.0/datachain_sources/sftp.py
--rw-r--r--   0        0        0     1866 2023-06-01 01:30:13.897738 datachain_sources-0.1.0/datachain_sources/sharepoint.py
--rw-r--r--   0        0        0     2393 2023-06-01 01:30:20.225491 datachain_sources-0.1.0/datachain_sources/sql.py
--rw-r--r--   0        0        0     1862 2023-06-01 01:37:55.407775 datachain_sources-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 datachain_sources-0.1.0/setup.py
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 datachain_sources-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-01 01:26:19.859742 datachain_sources-0.1.1/README.md
+-rw-r--r--   0        0        0       32 2023-05-31 11:13:21.461420 datachain_sources-0.1.1/datachain_sources/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-01 00:45:58.852159 datachain_sources-0.1.1/datachain_sources/_utils.py
+-rw-r--r--   0        0        0       32 2023-05-31 14:27:33.860480 datachain_sources-0.1.1/datachain_sources/bytes/__init__.py
+-rw-r--r--   0        0        0     1322 2023-06-01 00:35:20.042249 datachain_sources-0.1.1/datachain_sources/bytes/_pandas.py
+-rw-r--r--   0        0        0      737 2023-06-01 01:29:31.192827 datachain_sources-0.1.1/datachain_sources/file.py
+-rw-r--r--   0        0        0       32 2023-06-01 00:28:56.862995 datachain_sources-0.1.1/datachain_sources/files/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-01 01:29:21.878284 datachain_sources-0.1.1/datachain_sources/files/_file.py
+-rw-r--r--   0        0        0      972 2023-03-31 02:14:16.000000 datachain_sources-0.1.1/datachain_sources/files/_ftp.py
+-rw-r--r--   0        0        0      843 2023-05-31 11:15:46.822209 datachain_sources-0.1.1/datachain_sources/files/_http.py
+-rw-r--r--   0        0        0      624 2023-06-01 01:28:52.178966 datachain_sources-0.1.1/datachain_sources/files/_jsonfile.py
+-rw-r--r--   0        0        0      442 2023-03-31 02:13:33.000000 datachain_sources-0.1.1/datachain_sources/files/_local.py
+-rw-r--r--   0        0        0     3163 2023-06-01 01:50:46.715579 datachain_sources-0.1.1/datachain_sources/files/_pandas.py
+-rw-r--r--   0        0        0     1205 2023-03-31 02:14:23.000000 datachain_sources-0.1.1/datachain_sources/files/_sftp.py
+-rw-r--r--   0        0        0     1100 2023-06-01 01:29:46.912109 datachain_sources-0.1.1/datachain_sources/ftp.py
+-rw-r--r--   0        0        0     1044 2023-06-01 01:30:03.611089 datachain_sources-0.1.1/datachain_sources/http.py
+-rw-r--r--   0        0        0       32 2023-05-31 12:23:56.344417 datachain_sources-0.1.1/datachain_sources/query/__init__.py
+-rw-r--r--   0        0        0     3040 2023-06-01 00:36:12.838156 datachain_sources-0.1.1/datachain_sources/query/_pandas.py
+-rw-r--r--   0        0        0     1187 2023-06-01 01:30:07.584911 datachain_sources-0.1.1/datachain_sources/sftp.py
+-rw-r--r--   0        0        0     1889 2023-06-01 01:53:20.493358 datachain_sources-0.1.1/datachain_sources/sharepoint.py
+-rw-r--r--   0        0        0     2393 2023-06-01 01:30:20.225491 datachain_sources-0.1.1/datachain_sources/sql.py
+-rw-r--r--   0        0        0     1862 2023-06-01 01:51:59.967014 datachain_sources-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 datachain_sources-0.1.1/setup.py
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 datachain_sources-0.1.1/PKG-INFO
```

### Comparing `datachain_sources-0.1.0/datachain_sources/_utils.py` & `datachain_sources-0.1.1/datachain_sources/_utils.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/bytes/_pandas.py` & `datachain_sources-0.1.1/datachain_sources/bytes/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/file.py` & `datachain_sources-0.1.1/datachain_sources/file.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/files/_file.py` & `datachain_sources-0.1.1/datachain_sources/files/_file.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/files/_ftp.py` & `datachain_sources-0.1.1/datachain_sources/files/_ftp.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/files/_http.py` & `datachain_sources-0.1.1/datachain_sources/files/_http.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/files/_jsonfile.py` & `datachain_sources-0.1.1/datachain_sources/files/_jsonfile.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/files/_pandas.py` & `datachain_sources-0.1.1/datachain_sources/files/_pandas.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         path (str): The path to the input file.
         **kwds (Any): Keyword arguments to pass to the reading method.
 
     Returns:
         pandas.DataFrame: The DataFrame created from the file.
     """
 
+    file_extension = path.split(".")[-1].lower()
+
     read_file_params = {}
     for param in kwds.items():
         if param in [
             "params",
             "data",
             "headers",
             "cookies",
@@ -37,15 +39,15 @@
             "verify",
             "cert",
             "json",
         ]:
             read_file_params[param] = kwds[param]
             del kwds[param]
 
-    return read_bytes(get_file(path, **read_file_params), **kwds)
+    return read_bytes(get_file(path, **read_file_params), file_extension, **kwds)
 
 
 def write_pandas(data: Any, path: str, **kwds: Any) -> None:
     """Save a pandas DataFrame to the specified file format.
 
     Parameters:
         data (pandas.DataFrame): The DataFrame to save.
```

### Comparing `datachain_sources-0.1.0/datachain_sources/files/_sftp.py` & `datachain_sources-0.1.1/datachain_sources/files/_sftp.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/ftp.py` & `datachain_sources-0.1.1/datachain_sources/ftp.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/http.py` & `datachain_sources-0.1.1/datachain_sources/http.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/query/_pandas.py` & `datachain_sources-0.1.1/datachain_sources/query/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/sftp.py` & `datachain_sources-0.1.1/datachain_sources/sftp.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/datachain_sources/sharepoint.py` & `datachain_sources-0.1.1/datachain_sources/sharepoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         authcookie=authcookie,
     )
     if not isinstance(site, _Site365):
         return None
     folder = site.Folder("/".join(path_split[5:-1]))
     file = folder.get_file(path_split[-1])
 
-    data = read_pandas(file, path_split[-1], **kwds)
+    data = read_pandas(file, path_split[-1].split(".")[-1].lower(), **kwds)
     return data
 
 
 class TabularSource(DataSource):  # pylint: disable=too-few-public-methods
     """Pandas implementation of DataSource being able to read dataframes"""
 
     def __init__(self, **kwds: Any) -> None:
```

### Comparing `datachain_sources-0.1.0/datachain_sources/sql.py` & `datachain_sources-0.1.1/datachain_sources/sql.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.0/pyproject.toml` & `datachain_sources-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datachain_sources"
-version = "0.1.0"
+version = "0.1.1"
 description = "Sources for DataChain library."
 authors = ["Rayane AMROUCHE <rayaneamrouche@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 packages = [
     { include = "datachain_sources" },
```

### Comparing `datachain_sources-0.1.0/setup.py` & `datachain_sources-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'snowflake': ['sqlalchemy==1.4.46',
                'snowflake-connector-python>=2.9.0,<3.0.0',
                'snowflake-sqlalchemy>=1.4.4,<2.0.0',
                'cryptography==38.0.4']}
 
 setup_kwargs = {
     'name': 'datachain-sources',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Sources for DataChain library.',
     'long_description': '',
     'author': 'Rayane AMROUCHE',
     'author_email': 'rayaneamrouche@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `datachain_sources-0.1.0/PKG-INFO` & `datachain_sources-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datachain-sources
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sources for DataChain library.
 License: GPL-3.0-or-later
 Author: Rayane AMROUCHE
 Author-email: rayaneamrouche@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

