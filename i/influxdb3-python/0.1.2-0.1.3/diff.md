# Comparing `tmp/influxdb3-python-0.1.2.tar.gz` & `tmp/influxdb3-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.2.tar", last modified: Thu Jun  1 13:44:56 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.3.tar", last modified: Thu Jun  1 17:55:27 2023, max compression
```

## Comparing `influxdb3-python-0.1.2.tar` & `influxdb3-python-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 13:44:56.000000 influxdb3-python-0.1.2/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:44:56.539277 influxdb3-python-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 13:44:42.000000 influxdb3-python-0.1.2/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.2/LICENSE` & `influxdb3-python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.2/PKG-INFO` & `influxdb3-python-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -50,15 +50,15 @@
 - `influxdb-client`
 
 ## Installation
 
 You can install the dependencies using `pip`:
 
 ```bash
-pip install influxdb3-client
+pip install influxdb3-python
 ```
 
 # Usage
 ## Importing the Module
 ```python
 from influxdb_client_3 import InfluxDBClient3, Point
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.2 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.3 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -12,15 +12,15 @@
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
 # InfluxDB 3.0 Python Client ## Introduction `influxdb_client_3` is a Python
 module that provides a simple and convenient way to interact with InfluxDB 3.0.
 This module supports both writing data to InfluxDB and querying data using the
 Flight client, which allows you to execute SQL and InfluxQL queries on InfluxDB
 3.0. ## Dependencies - `pyarrow` - `influxdb-client` ## Installation You can
-install the dependencies using `pip`: ```bash pip install influxdb3-client ```
+install the dependencies using `pip`: ```bash pip install influxdb3-python ```
 # Usage ## Importing the Module ```python from influxdb_client_3 import
 InfluxDBClient3, Point ``` ## Initialization If you are using InfluxDB Cloud,
 then you should note that: 1. You will need to supply your org id, this is not
 necessary for InfluxDB Dedicated. 2. Use a bucketname for the database
 argument. ```python client = InfluxDBClient3(token="your-token", host="your-
 host", org="your-org", database="your-database") ``` ## Writing Data You can
 write data using the Point class, or supplying line protocol. ### Using Points
```

### Comparing `influxdb3-python-0.1.2/README.md` & `influxdb3-python-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 - `influxdb-client`
 
 ## Installation
 
 You can install the dependencies using `pip`:
 
 ```bash
-pip install influxdb3-client
+pip install influxdb3-python
 ```
 
 # Usage
 ## Importing the Module
 ```python
 from influxdb_client_3 import InfluxDBClient3, Point
 ```
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
 # InfluxDB 3.0 Python Client ## Introduction `influxdb_client_3` is a Python
 module that provides a simple and convenient way to interact with InfluxDB 3.0.
 This module supports both writing data to InfluxDB and querying data using the
 Flight client, which allows you to execute SQL and InfluxQL queries on InfluxDB
 3.0. ## Dependencies - `pyarrow` - `influxdb-client` ## Installation You can
-install the dependencies using `pip`: ```bash pip install influxdb3-client ```
+install the dependencies using `pip`: ```bash pip install influxdb3-python ```
 # Usage ## Importing the Module ```python from influxdb_client_3 import
 InfluxDBClient3, Point ``` ## Initialization If you are using InfluxDB Cloud,
 then you should note that: 1. You will need to supply your org id, this is not
 necessary for InfluxDB Dedicated. 2. Use a bucketname for the database
 argument. ```python client = InfluxDBClient3(token="your-token", host="your-
 host", org="your-org", database="your-database") ``` ## Writing Data You can
 write data using the Point class, or supplying line protocol. ### Using Points
```

### Comparing `influxdb3-python-0.1.2/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.1.3/influxdb3_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -50,15 +50,15 @@
 - `influxdb-client`
 
 ## Installation
 
 You can install the dependencies using `pip`:
 
 ```bash
-pip install influxdb3-client
+pip install influxdb3-python
 ```
 
 # Usage
 ## Importing the Module
 ```python
 from influxdb_client_3 import InfluxDBClient3, Point
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.2 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.3 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -12,15 +12,15 @@
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
 # InfluxDB 3.0 Python Client ## Introduction `influxdb_client_3` is a Python
 module that provides a simple and convenient way to interact with InfluxDB 3.0.
 This module supports both writing data to InfluxDB and querying data using the
 Flight client, which allows you to execute SQL and InfluxQL queries on InfluxDB
 3.0. ## Dependencies - `pyarrow` - `influxdb-client` ## Installation You can
-install the dependencies using `pip`: ```bash pip install influxdb3-client ```
+install the dependencies using `pip`: ```bash pip install influxdb3-python ```
 # Usage ## Importing the Module ```python from influxdb_client_3 import
 InfluxDBClient3, Point ``` ## Initialization If you are using InfluxDB Cloud,
 then you should note that: 1. You will need to supply your org id, this is not
 necessary for InfluxDB Dedicated. 2. Use a bucketname for the database
 argument. ```python client = InfluxDBClient3(token="your-token", host="your-
 host", org="your-org", database="your-database") ``` ## Writing Data You can
 write data using the Point class, or supplying line protocol. ### Using Points
```

### Comparing `influxdb3-python-0.1.2/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.3/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.2/setup.py` & `influxdb3-python-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.2/tests/test_influxdb_client_3.py` & `influxdb3-python-0.1.3/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

