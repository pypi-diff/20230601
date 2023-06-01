# Comparing `tmp/rudderclient-1.8.0.tar.gz` & `tmp/rudderclient-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.8.0.tar", last modified: Thu Jun  1 11:40:47 2023, max compression
+gzip compressed data, was "rudderclient-1.8.1.tar", last modified: Thu Jun  1 13:13:08 2023, max compression
```

## Comparing `rudderclient-1.8.0.tar` & `rudderclient-1.8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.605796 rudderclient-1.8.0/
--rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-06-01 11:40:15.000000 rudderclient-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-01 11:40:47.605796 rudderclient-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-06-01 11:40:15.000000 rudderclient-1.8.0/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)     1030 2023-06-01 11:40:37.000000 rudderclient-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-06-01 11:40:47.605796 rudderclient-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.596795 rudderclient-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.599795 rudderclient-1.8.0/src/rudderclient/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.601796 rudderclient-1.8.0/src/rudderclient/aws/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/aws/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5006 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/aws/requests.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.603796 rudderclient-1.8.0/src/rudderclient/gcp/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/gcp/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2649 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/gcp/auth.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1969 2023-06-01 11:40:35.000000 rudderclient-1.8.0/src/rudderclient/gcp/http_requests.py
--rw-r--r--   0 runner    (1001) runner    (1001)      869 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3832 2023-06-01 11:40:35.000000 rudderclient-1.8.0/src/rudderclient/gcp/workspace.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.604796 rudderclient-1.8.0/src/rudderclient/request/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/request/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/request/exceptions.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1260 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/request/helpers.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.604796 rudderclient-1.8.0/src/rudderclient/tools/
--rw-r--r--   0 runner    (1001) runner    (1001)     5321 2023-06-01 11:40:15.000000 rudderclient-1.8.0/src/rudderclient/tools/send_account_email.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 11:40:47.600796 rudderclient-1.8.0/src/rudderclient.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      648 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       13 2023-06-01 11:40:47.000000 rudderclient-1.8.0/src/rudderclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 13:13:08.791675 rudderclient-1.8.1/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-06-01 13:12:37.000000 rudderclient-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-01 13:13:08.790675 rudderclient-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-06-01 13:12:37.000000 rudderclient-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     1030 2023-06-01 13:12:56.000000 rudderclient-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-06-01 13:13:08.791675 rudderclient-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 13:13:08.783675 rudderclient-1.8.1/src/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 13:13:08.785675 rudderclient-1.8.1/src/rudderclient/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 13:13:08.787675 rudderclient-1.8.1/src/rudderclient/aws/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/aws/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5006 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/aws/requests.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 13:13:08.789675 rudderclient-1.8.1/src/rudderclient/gcp/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2649 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/gcp/auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1969 2023-06-01 13:12:55.000000 rudderclient-1.8.1/src/rudderclient/gcp/http_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      869 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3832 2023-06-01 13:12:55.000000 rudderclient-1.8.1/src/rudderclient/gcp/workspace.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 13:13:08.790675 rudderclient-1.8.1/src/rudderclient/request/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/request/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/request/exceptions.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1260 2023-06-01 13:12:37.000000 rudderclient-1.8.1/src/rudderclient/request/helpers.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 13:13:08.790675 rudderclient-1.8.1/src/rudderclient/tools/
+-rw-r--r--   0 runner    (1001) runner    (1001)     3816 2023-06-01 13:12:55.000000 rudderclient-1.8.1/src/rudderclient/tools/send_email.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 13:13:08.786675 rudderclient-1.8.1/src/rudderclient.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-01 13:13:08.000000 rudderclient-1.8.1/src/rudderclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      640 2023-06-01 13:13:08.000000 rudderclient-1.8.1/src/rudderclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-06-01 13:13:08.000000 rudderclient-1.8.1/src/rudderclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-06-01 13:13:08.000000 rudderclient-1.8.1/src/rudderclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       13 2023-06-01 13:13:08.000000 rudderclient-1.8.1/src/rudderclient.egg-info/top_level.txt
```

### Comparing `rudderclient-1.8.0/LICENSE` & `rudderclient-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.8.0/PKG-INFO` & `rudderclient-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.8.0
+Version: 1.8.1
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.8.0/pyproject.toml` & `rudderclient-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0.0", "wheel",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudderclient"
-version = "1.8.0"
+version = "1.8.1"
 description = "Shared helpers for rudder application functions code"
 readme = "README.md"
 classifiers = [ "License :: OSI Approved :: MIT License", "Programming Language :: Python", "Programming Language :: Python :: 3.10",]
 keywords = [ "rudder", "client", "helper",]
 dependencies = [ "google-cloud-secret-manager",]
 requires-python = ">=3.10"
 [[project.authors]]
```

### Comparing `rudderclient-1.8.0/src/rudderclient/aws/requests.py` & `rudderclient-1.8.1/src/rudderclient/aws/requests.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.8.0/src/rudderclient/gcp/auth.py` & `rudderclient-1.8.1/src/rudderclient/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.8.0/src/rudderclient/gcp/http_requests.py` & `rudderclient-1.8.1/src/rudderclient/gcp/http_requests.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.8.0/src/rudderclient/gcp/pubsub.py` & `rudderclient-1.8.1/src/rudderclient/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.8.0/src/rudderclient/gcp/workspace.py` & `rudderclient-1.8.1/src/rudderclient/gcp/workspace.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.8.0/src/rudderclient/request/exceptions.py` & `rudderclient-1.8.1/src/rudderclient/request/exceptions.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.8.0/src/rudderclient/request/helpers.py` & `rudderclient-1.8.1/src/rudderclient/request/helpers.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.8.0/src/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.8.1/src/rudderclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.8.0
+Version: 1.8.1
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.8.0/src/rudderclient.egg-info/SOURCES.txt` & `rudderclient-1.8.1/src/rudderclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 src/rudderclient/gcp/auth.py
 src/rudderclient/gcp/http_requests.py
 src/rudderclient/gcp/pubsub.py
 src/rudderclient/gcp/workspace.py
 src/rudderclient/request/__init__.py
 src/rudderclient/request/exceptions.py
 src/rudderclient/request/helpers.py
-src/rudderclient/tools/send_account_email.py
+src/rudderclient/tools/send_email.py
```

