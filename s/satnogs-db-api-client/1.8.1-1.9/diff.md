# Comparing `tmp/satnogs-db-api-client-1.8.1.tar.gz` & `tmp/satnogs-db-api-client-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/satnogs-db-api-client-1.8.1.tar", last modified: Wed Sep  9 10:05:30 2020, max compression
+gzip compressed data, was "dist/satnogs-db-api-client-1.9.tar", last modified: Sat Sep 12 22:04:54 2020, max compression
```

## Comparing `satnogs-db-api-client-1.8.1.tar` & `satnogs-db-api-client-1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/
--rw-rw-rw-   0 root         (0) root         (0)       61 2020-09-09 09:53:34.000000 satnogs-db-api-client-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      870 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      360 2020-09-09 09:53:34.000000 satnogs-db-api-client-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogs_db_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      870 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogs_db_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      860 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogs_db_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogs_db_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogs_db_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogs_db_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/
--rw-r--r--   0 root         (0) root         (0)     1074 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/api/
--rw-r--r--   0 root         (0) root         (0)      145 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91182 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/api/default_api.py
--rw-r--r--   0 root         (0) root         (0)    27333 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/api_client.py
--rw-r--r--   0 root         (0) root         (0)    15876 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5119 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/models/
--rw-r--r--   0 root         (0) root         (0)      492 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5223 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/models/inline_response200.py
--rw-r--r--   0 root         (0) root         (0)     5243 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/models/inline_response2001.py
--rw-r--r--   0 root         (0) root         (0)    12737 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/test/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2212 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/test/test_default_api.py
--rw-r--r--   0 root         (0) root         (0)     1581 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/test/test_inline_response200.py
--rw-r--r--   0 root         (0) root         (0)     1592 2020-09-09 09:54:58.000000 satnogs-db-api-client-1.8.1/satnogsdbapiclient/test/test_inline_response2001.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2020-09-09 10:05:30.000000 satnogs-db-api-client-1.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      136 2020-09-09 09:53:34.000000 satnogs-db-api-client-1.8.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    68573 2020-09-09 09:53:34.000000 satnogs-db-api-client-1.8.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2020-09-12 21:53:19.000000 satnogs-db-api-client-1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      868 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      360 2020-09-12 21:53:19.000000 satnogs-db-api-client-1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogs_db_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      868 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogs_db_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      860 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogs_db_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogs_db_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogs_db_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogs_db_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/
+-rw-r--r--   0 root         (0) root         (0)     1074 2020-09-12 21:54:40.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      495 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/api/
+-rw-r--r--   0 root         (0) root         (0)      145 2020-09-12 21:54:40.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91182 2020-09-12 21:54:39.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/api/default_api.py
+-rw-r--r--   0 root         (0) root         (0)    27333 2020-09-12 21:54:40.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    15876 2020-09-12 21:54:40.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2020-09-12 21:54:40.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/models/
+-rw-r--r--   0 root         (0) root         (0)      492 2020-09-12 21:54:40.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5223 2020-09-12 21:54:39.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/models/inline_response200.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2020-09-12 21:54:39.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/models/inline_response2001.py
+-rw-r--r--   0 root         (0) root         (0)    12737 2020-09-12 21:54:40.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-09-12 21:54:40.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2020-09-12 21:54:39.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/test/test_default_api.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2020-09-12 21:54:39.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/test/test_inline_response200.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2020-09-12 21:54:39.000000 satnogs-db-api-client-1.9/satnogsdbapiclient/test/test_inline_response2001.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2020-09-12 22:04:54.000000 satnogs-db-api-client-1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      136 2020-09-12 21:53:19.000000 satnogs-db-api-client-1.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    68573 2020-09-12 21:53:19.000000 satnogs-db-api-client-1.9/versioneer.py
```

### Comparing `satnogs-db-api-client-1.8.1/PKG-INFO` & `satnogs-db-api-client-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: satnogs-db-api-client
-Version: 1.8.1
+Version: 1.9
 Summary: SatNOGS DB API Client
 Home-page: https://gitlab.com/librespacefoundation/satnogs/satnogs-db
 Author: SatNOGS project
 Author-email: dev@satnogs.org
 License: AGPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `satnogs-db-api-client-1.8.1/satnogs_db_api_client.egg-info/PKG-INFO` & `satnogs-db-api-client-1.9/satnogs_db_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: satnogs-db-api-client
-Version: 1.8.1
+Version: 1.9
 Summary: SatNOGS DB API Client
 Home-page: https://gitlab.com/librespacefoundation/satnogs/satnogs-db
 Author: SatNOGS project
 Author-email: dev@satnogs.org
 License: AGPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `satnogs-db-api-client-1.8.1/satnogs_db_api_client.egg-info/SOURCES.txt` & `satnogs-db-api-client-1.9/satnogs_db_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/__init__.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/api/default_api.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/api/default_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/api_client.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/api_client.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/configuration.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/configuration.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/exceptions.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/models/inline_response200.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/models/inline_response2001.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/rest.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/rest.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/test/test_default_api.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/test/test_inline_response200.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/satnogsdbapiclient/test/test_inline_response2001.py` & `satnogs-db-api-client-1.9/satnogsdbapiclient/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/setup.cfg` & `satnogs-db-api-client-1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `satnogs-db-api-client-1.8.1/versioneer.py` & `satnogs-db-api-client-1.9/versioneer.py`

 * *Files identical despite different names*

