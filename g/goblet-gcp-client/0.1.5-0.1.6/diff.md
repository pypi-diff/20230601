# Comparing `tmp/goblet_gcp_client-0.1.5.tar.gz` & `tmp/goblet_gcp_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goblet_gcp_client-0.1.5.tar", last modified: Fri May 12 13:03:49 2023, max compression
+gzip compressed data, was "goblet_gcp_client-0.1.6.tar", last modified: Thu Jun  1 14:27:49 2023, max compression
```

## Comparing `goblet_gcp_client-0.1.5.tar` & `goblet_gcp_client-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-12 13:03:49.082708 goblet_gcp_client-0.1.5/
--rw-r--r--   0 austen.novis   (502) staff       (20)    11357 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/LICENSE
--rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-05-12 13:03:49.082533 goblet_gcp_client-0.1.5/PKG-INFO
--rw-r--r--   0 austen.novis   (502) staff       (20)     3984 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/README.md
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-12 13:03:49.081419 goblet_gcp_client-0.1.5/goblet_gcp_client/
--rw-r--r--   0 austen.novis   (502) staff       (20)      200 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/goblet_gcp_client/__init__.py
--rw-r--r--   0 austen.novis   (502) staff       (20)       64 2023-05-12 13:03:39.000000 goblet_gcp_client-0.1.5/goblet_gcp_client/__version__.py
--rw-r--r--   0 austen.novis   (502) staff       (20)     6335 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/goblet_gcp_client/client.py
--rw-r--r--   0 austen.novis   (502) staff       (20)     6149 2023-05-12 13:03:39.000000 goblet_gcp_client-0.1.5/goblet_gcp_client/http_files.py
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-12 13:03:49.082261 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/
--rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/PKG-INFO
--rw-r--r--   0 austen.novis   (502) staff       (20)      353 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/SOURCES.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/dependency_links.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       25 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/requires.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       18 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/top_level.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-05-12 13:03:49.082760 goblet_gcp_client-0.1.5/setup.cfg
--rw-r--r--   0 austen.novis   (502) staff       (20)     3382 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/setup.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-06-01 14:27:49.275831 goblet_gcp_client-0.1.6/
+-rw-r--r--   0 austen.novis   (502) staff       (20)    11357 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.6/LICENSE
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-06-01 14:27:49.275554 goblet_gcp_client-0.1.6/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)     3984 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.6/README.md
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-06-01 14:27:49.274032 goblet_gcp_client-0.1.6/goblet_gcp_client/
+-rw-r--r--   0 austen.novis   (502) staff       (20)      200 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.6/goblet_gcp_client/__init__.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)       64 2023-06-01 14:27:36.000000 goblet_gcp_client-0.1.6/goblet_gcp_client/__version__.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     6385 2023-06-01 14:27:36.000000 goblet_gcp_client-0.1.6/goblet_gcp_client/client.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     6149 2023-05-12 13:03:39.000000 goblet_gcp_client-0.1.6/goblet_gcp_client/http_files.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-06-01 14:27:49.275235 goblet_gcp_client-0.1.6/goblet_gcp_client.egg-info/
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-06-01 14:27:49.000000 goblet_gcp_client-0.1.6/goblet_gcp_client.egg-info/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)      353 2023-06-01 14:27:49.000000 goblet_gcp_client-0.1.6/goblet_gcp_client.egg-info/SOURCES.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-06-01 14:27:49.000000 goblet_gcp_client-0.1.6/goblet_gcp_client.egg-info/dependency_links.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       25 2023-06-01 14:27:49.000000 goblet_gcp_client-0.1.6/goblet_gcp_client.egg-info/requires.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       18 2023-06-01 14:27:49.000000 goblet_gcp_client-0.1.6/goblet_gcp_client.egg-info/top_level.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-06-01 14:27:49.275905 goblet_gcp_client-0.1.6/setup.cfg
+-rw-r--r--   0 austen.novis   (502) staff       (20)     3382 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.6/setup.py
```

### Comparing `goblet_gcp_client-0.1.5/LICENSE` & `goblet_gcp_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.5/PKG-INFO` & `goblet_gcp_client-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goblet_gcp_client
-Version: 0.1.5
+Version: 0.1.6
 Summary: GCP Client and GCP integration testing helpers
 Home-page: https://github.com/goblet/goblet_gcp_client
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `goblet_gcp_client-0.1.5/README.md` & `goblet_gcp_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.5/goblet_gcp_client/client.py` & `goblet_gcp_client-0.1.6/goblet_gcp_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,22 +150,22 @@
             version=self.version,
             credentials=self.credentials,
             calls=calls,
             parent_schema=operation,
         )
         count = 0
         sleep_duration = 4
-        while not done or count > timeout:
+        while not done and count < timeout:
             resp = operation_client.execute("get", parent_key="name")
             done = resp.get("done")
             time.sleep(sleep_duration)
             count += sleep_duration
         if count > timeout:
             log.info("Timeout exceeded in wait_for_operation")
-            return None
+            raise TimeoutError("Timeout exceeded in wait_for_operation")
         return resp
 
     def execute(
         self,
         api,
         calls=None,
         parent_schema=None,
```

### Comparing `goblet_gcp_client-0.1.5/goblet_gcp_client/http_files.py` & `goblet_gcp_client-0.1.6/goblet_gcp_client/http_files.py`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/PKG-INFO` & `goblet_gcp_client-0.1.6/goblet_gcp_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goblet-gcp-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: GCP Client and GCP integration testing helpers
 Home-page: https://github.com/goblet/goblet_gcp_client
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `goblet_gcp_client-0.1.5/setup.py` & `goblet_gcp_client-0.1.6/setup.py`

 * *Files identical despite different names*

