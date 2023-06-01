# Comparing `tmp/datachain_sources-0.1.1.tar.gz` & `tmp/datachain_sources-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datachain_sources-0.1.1.tar", max compression
+gzip compressed data, was "datachain_sources-0.1.2.tar", max compression
```

## Comparing `datachain_sources-0.1.1.tar` & `datachain_sources-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2023-06-01 01:26:19.859742 datachain_sources-0.1.1/README.md
--rw-r--r--   0        0        0       32 2023-05-31 11:13:21.461420 datachain_sources-0.1.1/datachain_sources/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-01 00:45:58.852159 datachain_sources-0.1.1/datachain_sources/_utils.py
--rw-r--r--   0        0        0       32 2023-05-31 14:27:33.860480 datachain_sources-0.1.1/datachain_sources/bytes/__init__.py
--rw-r--r--   0        0        0     1322 2023-06-01 00:35:20.042249 datachain_sources-0.1.1/datachain_sources/bytes/_pandas.py
--rw-r--r--   0        0        0      737 2023-06-01 01:29:31.192827 datachain_sources-0.1.1/datachain_sources/file.py
--rw-r--r--   0        0        0       32 2023-06-01 00:28:56.862995 datachain_sources-0.1.1/datachain_sources/files/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-01 01:29:21.878284 datachain_sources-0.1.1/datachain_sources/files/_file.py
--rw-r--r--   0        0        0      972 2023-03-31 02:14:16.000000 datachain_sources-0.1.1/datachain_sources/files/_ftp.py
--rw-r--r--   0        0        0      843 2023-05-31 11:15:46.822209 datachain_sources-0.1.1/datachain_sources/files/_http.py
--rw-r--r--   0        0        0      624 2023-06-01 01:28:52.178966 datachain_sources-0.1.1/datachain_sources/files/_jsonfile.py
--rw-r--r--   0        0        0      442 2023-03-31 02:13:33.000000 datachain_sources-0.1.1/datachain_sources/files/_local.py
--rw-r--r--   0        0        0     3163 2023-06-01 01:50:46.715579 datachain_sources-0.1.1/datachain_sources/files/_pandas.py
--rw-r--r--   0        0        0     1205 2023-03-31 02:14:23.000000 datachain_sources-0.1.1/datachain_sources/files/_sftp.py
--rw-r--r--   0        0        0     1100 2023-06-01 01:29:46.912109 datachain_sources-0.1.1/datachain_sources/ftp.py
--rw-r--r--   0        0        0     1044 2023-06-01 01:30:03.611089 datachain_sources-0.1.1/datachain_sources/http.py
--rw-r--r--   0        0        0       32 2023-05-31 12:23:56.344417 datachain_sources-0.1.1/datachain_sources/query/__init__.py
--rw-r--r--   0        0        0     3040 2023-06-01 00:36:12.838156 datachain_sources-0.1.1/datachain_sources/query/_pandas.py
--rw-r--r--   0        0        0     1187 2023-06-01 01:30:07.584911 datachain_sources-0.1.1/datachain_sources/sftp.py
--rw-r--r--   0        0        0     1889 2023-06-01 01:53:20.493358 datachain_sources-0.1.1/datachain_sources/sharepoint.py
--rw-r--r--   0        0        0     2393 2023-06-01 01:30:20.225491 datachain_sources-0.1.1/datachain_sources/sql.py
--rw-r--r--   0        0        0     1862 2023-06-01 01:51:59.967014 datachain_sources-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 datachain_sources-0.1.1/setup.py
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 datachain_sources-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-01 01:26:19.000000 datachain_sources-0.1.2/README.md
+-rw-r--r--   0        0        0       32 2023-05-31 11:13:21.000000 datachain_sources-0.1.2/datachain_sources/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-01 00:45:58.000000 datachain_sources-0.1.2/datachain_sources/_utils.py
+-rw-r--r--   0        0        0       32 2023-05-31 14:27:33.000000 datachain_sources-0.1.2/datachain_sources/bytes/__init__.py
+-rw-r--r--   0        0        0     1322 2023-06-01 00:35:20.000000 datachain_sources-0.1.2/datachain_sources/bytes/_pandas.py
+-rw-r--r--   0        0        0      737 2023-06-01 01:29:31.000000 datachain_sources-0.1.2/datachain_sources/file.py
+-rw-r--r--   0        0        0       32 2023-06-01 00:28:56.000000 datachain_sources-0.1.2/datachain_sources/files/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-01 01:29:21.000000 datachain_sources-0.1.2/datachain_sources/files/_file.py
+-rw-r--r--   0        0        0     1033 2023-06-01 02:25:43.717163 datachain_sources-0.1.2/datachain_sources/files/_ftp.py
+-rw-r--r--   0        0        0      843 2023-05-31 11:15:46.000000 datachain_sources-0.1.2/datachain_sources/files/_http.py
+-rw-r--r--   0        0        0      624 2023-06-01 01:28:52.000000 datachain_sources-0.1.2/datachain_sources/files/_jsonfile.py
+-rw-r--r--   0        0        0      442 2023-03-31 02:13:33.000000 datachain_sources-0.1.2/datachain_sources/files/_local.py
+-rw-r--r--   0        0        0     3163 2023-06-01 01:50:46.000000 datachain_sources-0.1.2/datachain_sources/files/_pandas.py
+-rw-r--r--   0        0        0     1266 2023-06-01 02:28:24.870909 datachain_sources-0.1.2/datachain_sources/files/_sftp.py
+-rw-r--r--   0        0        0     1152 2023-06-01 02:26:17.148560 datachain_sources-0.1.2/datachain_sources/ftp.py
+-rw-r--r--   0        0        0     1044 2023-06-01 01:30:03.000000 datachain_sources-0.1.2/datachain_sources/http.py
+-rw-r--r--   0        0        0       32 2023-05-31 12:23:56.000000 datachain_sources-0.1.2/datachain_sources/query/__init__.py
+-rw-r--r--   0        0        0     3040 2023-06-01 00:36:12.000000 datachain_sources-0.1.2/datachain_sources/query/_pandas.py
+-rw-r--r--   0        0        0     1259 2023-06-01 02:26:50.890547 datachain_sources-0.1.2/datachain_sources/sftp.py
+-rw-r--r--   0        0        0     1889 2023-06-01 01:53:20.000000 datachain_sources-0.1.2/datachain_sources/sharepoint.py
+-rw-r--r--   0        0        0     2393 2023-06-01 01:30:20.000000 datachain_sources-0.1.2/datachain_sources/sql.py
+-rw-r--r--   0        0        0     1862 2023-06-01 02:30:56.705388 datachain_sources-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 datachain_sources-0.1.2/setup.py
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 datachain_sources-0.1.2/PKG-INFO
```

### Comparing `datachain_sources-0.1.1/datachain_sources/_utils.py` & `datachain_sources-0.1.2/datachain_sources/_utils.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/bytes/_pandas.py` & `datachain_sources-0.1.2/datachain_sources/bytes/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/file.py` & `datachain_sources-0.1.2/datachain_sources/file.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/files/_file.py` & `datachain_sources-0.1.2/datachain_sources/files/_file.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/files/_ftp.py` & `datachain_sources-0.1.2/datachain_sources/files/_ftp.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 Ftp source.
 """
 
 import io
 import ftplib
 
+from urllib.parse import unquote
+
 
 def ftp_to_file(ftp_url: str) -> bytes:
     """Retrieves bytes from an FTP path.
 
     Args:
         ftp_url (str): The URL of the FTP server.
 
@@ -23,13 +25,13 @@
     parts = ftp_url.split("/")
     username_password = parts[2].split("@")[0]
     username, password = username_password.split(":")
     server = parts[2].split("@")[1]
     path = "/" + "/".join(parts[3:])
 
     # Connect to the FTP server and retrieve the file
-    with ftplib.FTP(server) as ftp:
-        ftp.login(user=username, passwd=password)
+    with ftplib.FTP(unquote(server)) as ftp:
+        ftp.login(user=unquote(username), passwd=unquote(password))
         with ftp.retrbinary(f"RETR {path}", callback=None) as file:
             data_bytes = file.read()
             data = io.BytesIO(data_bytes)
             return data
```

### Comparing `datachain_sources-0.1.1/datachain_sources/files/_http.py` & `datachain_sources-0.1.2/datachain_sources/files/_http.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/files/_jsonfile.py` & `datachain_sources-0.1.2/datachain_sources/files/_jsonfile.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/files/_pandas.py` & `datachain_sources-0.1.2/datachain_sources/files/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/files/_sftp.py` & `datachain_sources-0.1.2/datachain_sources/files/_sftp.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 FTP source.
 """
 
 import io
 import paramiko
 
+from urllib.parse import unquote
+
 
 def sftp_to_file(sftp_url: str) -> io.BytesIO:
     """Retrieves bytes from an SFTP path.
 
     Args:
         sftp_url (str): The URL of the SFTP server.
 
@@ -25,14 +27,14 @@
     username, password = username_password.split(":")
     server_port = parts[2].split("@")[1]
     server = server_port.split(":")[0]
     port = int(server_port.split(":")[1]) if ":" in server_port else 22
     path = "/" + "/".join(parts[3:])
 
     # Connect to the SFTP server and retrieve the file
-    with paramiko.Transport((server, port)) as transport:
-        transport.connect(username=username, password=password)
+    with paramiko.Transport((unquote(server), port)) as transport:
+        transport.connect(username=unquote(username), password=unquote(password))
         with paramiko.SFTPClient.from_transport(transport) as sftp:
             with sftp.open(path, "rb") as file:
                 data_bytes = file.read()
                 data = io.BytesIO(data_bytes)
                 return data
```

### Comparing `datachain_sources-0.1.1/datachain_sources/ftp.py` & `datachain_sources-0.1.2/datachain_sources/ftp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """@Author: Rayane AMROUCHE
 
 Ftp source.
 """
 
 from typing import Any, Optional
+from urllib.parse import quote
 
 from datachain import DataSource
 
 from datachain_sources.files._pandas import read_pandas
 from datachain_sources._utils import login
 
 
@@ -16,15 +17,15 @@
     server: str,
     username: Optional[str] = None,
     password: Optional[str] = None,
     username_env: str = "",
     password_env: str = "",
 ):  # pylint: disable=too-many-arguments
     username, password = login(username, password, username_env, password_env)
-    ftp_path = f"ftp://{username}:{password}@{server}/{path}"
+    ftp_path = f"ftp://{quote(username)}:{quote(password)}@{quote(server)}/{path}"
     return read_pandas(ftp_path)
 
 
 class TabularSource(DataSource):  # pylint: disable=too-few-public-methods
     """Pandas implementation of DataSource being able to read dataframes from an ftp
     server"""
```

### Comparing `datachain_sources-0.1.1/datachain_sources/http.py` & `datachain_sources-0.1.2/datachain_sources/http.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/query/_pandas.py` & `datachain_sources-0.1.2/datachain_sources/query/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/sftp.py` & `datachain_sources-0.1.2/datachain_sources/sftp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """@Author: Rayane AMROUCHE
 
 Sftp source.
 """
 
 from typing import Any, Optional
+from urllib.parse import quote
 
 from datachain import DataSource
 
 
 from datachain_sources.files._pandas import read_pandas
 from datachain_sources._utils import login
 
@@ -18,17 +19,18 @@
     port: int = None,
     username: Optional[str] = None,
     password: Optional[str] = None,
     username_env: str = "",
     password_env: str = "",
 ):  # pylint: disable=too-many-arguments
     username, password = login(username, password, username_env, password_env)
+    server = quote(server)
     if port:
         server += ":" + str(port)
-    sftp_path = f"sftp://{username}:{password}@{server}/{path}"
+    sftp_path = f"sftp://{quote(username)}:{quote(password)}@{server}/{path}"
     return read_pandas(sftp_path)
 
 
 class TabularSource(DataSource):  # pylint: disable=too-few-public-methods
     """Pandas implementation of DataSource being able to read dataframes"""
 
     def __init__(self, **kwds: Any) -> None:
```

### Comparing `datachain_sources-0.1.1/datachain_sources/sharepoint.py` & `datachain_sources-0.1.2/datachain_sources/sharepoint.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/datachain_sources/sql.py` & `datachain_sources-0.1.2/datachain_sources/sql.py`

 * *Files identical despite different names*

### Comparing `datachain_sources-0.1.1/pyproject.toml` & `datachain_sources-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datachain_sources"
-version = "0.1.1"
+version = "0.1.2"
 description = "Sources for DataChain library."
 authors = ["Rayane AMROUCHE <rayaneamrouche@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 packages = [
     { include = "datachain_sources" },
```

### Comparing `datachain_sources-0.1.1/setup.py` & `datachain_sources-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'snowflake': ['sqlalchemy==1.4.46',
                'snowflake-connector-python>=2.9.0,<3.0.0',
                'snowflake-sqlalchemy>=1.4.4,<2.0.0',
                'cryptography==38.0.4']}
 
 setup_kwargs = {
     'name': 'datachain-sources',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Sources for DataChain library.',
     'long_description': '',
     'author': 'Rayane AMROUCHE',
     'author_email': 'rayaneamrouche@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `datachain_sources-0.1.1/PKG-INFO` & `datachain_sources-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datachain-sources
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sources for DataChain library.
 License: GPL-3.0-or-later
 Author: Rayane AMROUCHE
 Author-email: rayaneamrouche@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

