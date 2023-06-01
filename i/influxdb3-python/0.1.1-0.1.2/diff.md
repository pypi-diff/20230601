# Comparing `tmp/influxdb3-python-0.1.1.tar.gz` & `tmp/influxdb3-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.1.tar", last modified: Thu Jun  1 13:26:35 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.2.tar", last modified: Thu Jun  1 13:44:56 2023, max compression
```

## Comparing `influxdb3-python-0.1.1.tar` & `influxdb3-python-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 13:26:35.000000 influxdb3-python-0.1.1/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:35.947650 influxdb3-python-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 13:26:22.000000 influxdb3-python-0.1.1/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.1/LICENSE` & `influxdb3-python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.1/PKG-INFO` & `influxdb3-python-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.1 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.2 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `influxdb3-python-0.1.1/README.md` & `influxdb3-python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.1/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.1.2/influxdb3_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.1 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.2 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `influxdb3-python-0.1.1/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.2/influxdb_client_3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,39 +23,39 @@
 class InfluxDBClient3:
     def __init__(
             self,
             host=None,
             org=None,
             database=None,
             token=None,
-            write_client_options=None,
-            flight_client_options=None,
+            _write_client_options=None,
+            _flight_client_options=None,
             **kwargs):
         """
         This class provides an interface for interacting with an InfluxDB server, simplifying common operations such as writing, querying.
         * host (str, optional): The hostname or IP address of the InfluxDB server. Defaults to None.
         * org (str, optional): The InfluxDB organization name to be used for operations. Defaults to None.
         * database (str, optional): The database to be used for InfluxDB operations. Defaults to None.
         * token (str, optional): The authentication token for accessing the InfluxDB server. Defaults to None.
         * write_options (ANY, optional): Exposes InfuxDB WriteAPI options.
         * **kwargs: Additional arguments to be passed to the InfluxDB Client.
         """
         self._org = org
         self._database = database
-        self.write_client_options = write_client_options if write_client_options is not None else write_client_options(write_options=SYNCHRONOUS)
+        self._write_client_options = _write_client_options if _write_client_options is not None else write_client_options(write_options=SYNCHRONOUS)
         self._client = _InfluxDBClient(
             url=f"https://{host}",
             token=token,
             org=self._org,
             **kwargs)
         
         self._write_api = _WriteApi(
-            self._client, **self.write_client_options)
+            self._client, **self._write_client_options)
 
-        self._flight_client_options = flight_client_options if flight_client_options is not None else {}
+        self._flight_client_options = _flight_client_options if _flight_client_options is not None else {}
         self._flight_client = FlightClient(
             f"grpc+tls://{host}:443",
             **self._flight_client_options)
         
         # create an authorization header
         self._options = FlightCallOptions(
             headers=[(b"authorization", f"Bearer {token}".encode('utf-8'))])
```

### Comparing `influxdb3-python-0.1.1/setup.py` & `influxdb3-python-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.1/tests/test_influxdb_client_3.py` & `influxdb3-python-0.1.2/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

