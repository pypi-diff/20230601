# Comparing `tmp/influxdb3-python-0.1.0.tar.gz` & `tmp/influxdb3-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.0.tar", last modified: Thu Jun  1 10:49:49 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.1.tar", last modified: Thu Jun  1 13:26:35 2023, max compression
```

## Comparing `influxdb3-python-0.1.0.tar` & `influxdb3-python-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-01 10:49:38.000000 influxdb3-python-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 10:49:49.000000 influxdb3-python-0.1.0/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-01 10:49:38.000000 influxdb3-python-0.1.0/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 10:49:49.936418 influxdb3-python-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 10:49:38.000000 influxdb3-python-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.0/PKG-INFO` & `influxdb3-python-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <p align="center">
     <img src="https://github.com/InfluxCommunity/influxdb3-python/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python/">
@@ -29,15 +30,15 @@
     </a>
     <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
     </a>
         <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
     </a>
-    <a href="https://app.slack.com/huddle/influxcommunity/">
+    <a href="https://influxcommunity.slack.com">
         <img src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social" alt="Community Slack">
     </a>
 </p>
 
 # InfluxDB 3.0 Python Client
 ## Introduction
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.0 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.1 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
-Content-Type: text/markdown
+Content-Type: text/markdown License-File: LICENSE
                                  [Your Image]
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
 # InfluxDB 3.0 Python Client ## Introduction `influxdb_client_3` is a Python
 module that provides a simple and convenient way to interact with InfluxDB 3.0.
 This module supports both writing data to InfluxDB and querying data using the
 Flight client, which allows you to execute SQL and InfluxQL queries on InfluxDB
```

### Comparing `influxdb3-python-0.1.0/README.md` & `influxdb3-python-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     </a>
     <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
     </a>
         <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
     </a>
-    <a href="https://app.slack.com/huddle/influxcommunity/">
+    <a href="https://influxcommunity.slack.com">
         <img src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social" alt="Community Slack">
     </a>
 </p>
 
 # InfluxDB 3.0 Python Client
 ## Introduction
```

### Comparing `influxdb3-python-0.1.0/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.1.1/influxdb3_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <p align="center">
     <img src="https://github.com/InfluxCommunity/influxdb3-python/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python/">
@@ -29,15 +30,15 @@
     </a>
     <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
     </a>
         <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml">
         <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
     </a>
-    <a href="https://app.slack.com/huddle/influxcommunity/">
+    <a href="https://influxcommunity.slack.com">
         <img src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social" alt="Community Slack">
     </a>
 </p>
 
 # InfluxDB 3.0 Python Client
 ## Introduction
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.0 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.1 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
-Content-Type: text/markdown
+Content-Type: text/markdown License-File: LICENSE
                                  [Your Image]
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
 # InfluxDB 3.0 Python Client ## Introduction `influxdb_client_3` is a Python
 module that provides a simple and convenient way to interact with InfluxDB 3.0.
 This module supports both writing data to InfluxDB and querying data using the
 Flight client, which allows you to execute SQL and InfluxQL queries on InfluxDB
```

### Comparing `influxdb3-python-0.1.0/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.1/influxdb_client_3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,148 @@
 # influxdb_client_3/__init__.py
 
 from pyarrow import csv
 from pyarrow.flight import FlightClient, Ticket, FlightCallOptions
 from influxdb_client import InfluxDBClient as _InfluxDBClient
-from influxdb_client import WriteOptions as _WriteOptions
+from influxdb_client import WriteOptions as WriteOptions
 from influxdb_client.client.write_api import WriteApi as _WriteApi
-from influxdb_client.client.write_api import SYNCHRONOUS, ASYNCHRONOUS
-from influxdb_client.client.write_api import PointSettings
+from influxdb_client.client.write_api import SYNCHRONOUS, ASYNCHRONOUS, PointSettings
 from influxdb_client.domain.write_precision import WritePrecision
+from influxdb_client.client.exceptions import InfluxDBError
 from influxdb_client import Point
 import json
 
-def write_options(**kwargs):
-   return  _WriteOptions(**kwargs)
-
-def flight_client_options(**kwargs):
-    return kwargs  # You can replace this with a specific data structure if needed
-
 
+def write_client_options(**kwargs):
+    return kwargs
 
 
+def flight_client_options(**kwargs):
+    return kwargs  # You can replace this with a specific data structure if needed
 
 
 class InfluxDBClient3:
-    def __init__(self, host=None, org=None, database=None, token=None, write_options=None, flight_client_options=None ,**kwargs):
+    def __init__(
+            self,
+            host=None,
+            org=None,
+            database=None,
+            token=None,
+            write_client_options=None,
+            flight_client_options=None,
+            **kwargs):
         """
         This class provides an interface for interacting with an InfluxDB server, simplifying common operations such as writing, querying.
         * host (str, optional): The hostname or IP address of the InfluxDB server. Defaults to None.
         * org (str, optional): The InfluxDB organization name to be used for operations. Defaults to None.
         * database (str, optional): The database to be used for InfluxDB operations. Defaults to None.
         * token (str, optional): The authentication token for accessing the InfluxDB server. Defaults to None.
-        * write_options (enum, optional): Specifies the write mode (synchronous or asynchronous) to use when writing data points to InfluxDB. Defaults to SYNCHRONOUS.
+        * write_options (ANY, optional): Exposes InfuxDB WriteAPI options.
         * **kwargs: Additional arguments to be passed to the InfluxDB Client.
         """
         self._org = org
         self._database = database
-        self.write_options = write_options if write_options is not None else SYNCHRONOUS
-        self._client = _InfluxDBClient(url=f"https://{host}", token=token, org=self._org, **kwargs )
-        self._write_api = _WriteApi(self._client, write_options=self.write_options )
+        self.write_client_options = write_client_options if write_client_options is not None else write_client_options(write_options=SYNCHRONOUS)
+        self._client = _InfluxDBClient(
+            url=f"https://{host}",
+            token=token,
+            org=self._org,
+            **kwargs)
+        
+        self._write_api = _WriteApi(
+            self._client, **self.write_client_options)
 
         self._flight_client_options = flight_client_options if flight_client_options is not None else {}
-        self._flight_client = FlightClient(f"grpc+tls://{host}:443", **self._flight_client_options)
+        self._flight_client = FlightClient(
+            f"grpc+tls://{host}:443",
+            **self._flight_client_options)
+        
         # create an authorization header
-        self._options = FlightCallOptions(headers=[(b"authorization",f"Bearer {token}".encode('utf-8'))])
+        self._options = FlightCallOptions(
+            headers=[(b"authorization", f"Bearer {token}".encode('utf-8'))])
 
     def write(self, record=None, **kwargs):
         """
         Write data to InfluxDB.
 
         :type database: str
         :param record: The data point(s) to write.
         :type record: Point or list of Point objects
         :param kwargs: Additional arguments to pass to the write API.
         """
         try:
-            self._write_api.write(bucket=self._database, record=record, **kwargs)
+            self._write_api.write(
+                bucket=self._database, record=record, **kwargs)
         except Exception as e:
             print(e)
-    
-    def write_csv(self, csv_file, measurement_name=None, tag_columns = [],timestamp_column = 'time',  **kwargs):
+
+    def write_csv(
+            self,
+            csv_file,
+            measurement_name=None,
+            tag_columns=[],
+            timestamp_column='time',
+            **kwargs):
         """
         Write data from a CSV file to InfluxDB.
 
         :param csv_file: The CSV file to write.
         :type csv_file: str
         :param kwargs: Additional arguments to pass to the write API.
         """
         try:
             atable = csv.read_csv(csv_file, **kwargs)
-     
+
             df = atable.to_pandas()
-            self._write_api.write(bucket=self._database, record=df, 
-                                  data_frame_measurement_name=measurement_name, 
+            self._write_api.write(bucket=self._database, record=df,
+                                  data_frame_measurement_name=measurement_name,
                                   data_frame_tag_columns=tag_columns,
-                                  data_frame_timestamp_column = timestamp_column )
+                                  data_frame_timestamp_column=timestamp_column)
         except Exception as e:
             print(e)
-    
-
-
 
     def query(self, query, language="sql"):
         # create a flight client pointing to the InfluxDB
         # create a ticket
         ticket_data = {
-        "database": self._database,
-        "sql_query": query,
-        "query_type": language}
-        
+            "database": self._database,
+            "sql_query": query,
+            "query_type": language}
+
         ticket_bytes = json.dumps(ticket_data)
         ticket = Ticket(ticket_bytes)
-        
+
         # execute the query and return all the data
         flight_reader = self._flight_client.do_get(ticket, self._options)
 
         # use read_all() to get all of the data as an Arrow table
         # there are other functions to iterate through rows or read only parts of the data
         # which is useful if you have huge data sets
         return flight_reader.read_all()
 
-
     def close(self):
         # Clean up resources here.
         # Call close method of _write_api and _flight_client, if they exist.
         if hasattr(self._write_api, 'close'):
             self._write_api.close()
         if hasattr(self._flight_client, 'close'):
             self._flight_client.close()
         if hasattr(self._client, 'close'):
             self._client.close()
-    
+
     def __enter__(self):
         return self
-    
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
-__all__ = ["InfluxDBClient3", "Point", "PointSettings", "SYNCHRONOUS", "ASYNCHRONOUS", "write_options", "WritePrecision", "flight_client_options"]
+
+__all__ = [
+    "InfluxDBClient3",
+    "Point",
+    "PointSettings",
+    "SYNCHRONOUS",
+    "ASYNCHRONOUS",
+    "write_client_options",
+    "WritePrecision",
+    "flight_client_options",
+    "WriteOptions"]
```

### Comparing `influxdb3-python-0.1.0/setup.py` & `influxdb3-python-0.1.1/setup.py`

 * *Files identical despite different names*

