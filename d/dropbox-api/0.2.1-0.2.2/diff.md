# Comparing `tmp/dropbox-api-0.2.1.tar.gz` & `tmp/dropbox-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dropbox-api-0.2.1.tar", last modified: Thu Jun  1 03:13:41 2023, max compression
+gzip compressed data, was "dist/dropbox-api-0.2.2.tar", last modified: Thu Jun  1 10:18:09 2023, max compression
```

## Comparing `dropbox-api-0.2.1.tar` & `dropbox-api-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox/
--rw-r--r--   0 root         (0) root         (0)     1655 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/user.py
--rw-r--r--   0 root         (0) root         (0)     1406 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/shared_link.py
--rw-r--r--   0 root         (0) root         (0)     2888 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/base.py
--rw-r--r--   0 root         (0) root         (0)     6218 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      371 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 03:13:37.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2732 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     1250 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-06-01 10:18:03.000000 dropbox-api-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/src/dropbox/
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-06-01 10:18:03.000000 dropbox-api-0.2.2/src/dropbox/base.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-06-01 10:18:03.000000 dropbox-api-0.2.2/src/dropbox/user.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-06-01 10:18:03.000000 dropbox-api-0.2.2/src/dropbox/shared_link.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-06-01 10:18:03.000000 dropbox-api-0.2.2/src/dropbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-06-01 10:18:03.000000 dropbox-api-0.2.2/src/dropbox/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/src/dropbox_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/src/dropbox_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 10:18:05.000000 dropbox-api-0.2.2/src/dropbox_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/src/dropbox_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/src/dropbox_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/src/dropbox_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/src/dropbox_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-06-01 10:18:03.000000 dropbox-api-0.2.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-01 10:18:09.000000 dropbox-api-0.2.2/setup.cfg
```

### Comparing `dropbox-api-0.2.1/src/dropbox/user.py` & `dropbox-api-0.2.2/src/dropbox/user.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.1/src/dropbox/__init__.py` & `dropbox-api-0.2.2/src/dropbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.1/src/dropbox/shared_link.py` & `dropbox-api-0.2.2/src/dropbox/shared_link.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 class SharedLinkAPI(object):
 
+    def list_shared_links(self, path):
+        url = self.base_url + "sharing/list_shared_links"
+        contents = self.post(url, data_j = dict(path = path))
+        return contents
+
     def create_shared_link(self, path, settings = dict()):
         url = self.base_url + "sharing/create_shared_link_with_settings"
         contents = self.post(
             url,
             data_j = dict(
                 path = path,
                 settings = settings
```

### Comparing `dropbox-api-0.2.1/src/dropbox/base.py` & `dropbox-api-0.2.2/src/dropbox/base.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.1/src/dropbox/file.py` & `dropbox-api-0.2.2/src/dropbox/file.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.1/src/dropbox_api.egg-info/PKG-INFO` & `dropbox-api-0.2.2/src/dropbox_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropbox-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: Dropbox API Client
 Home-page: http://dropbox-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Dropbox API](http://dropbox-api.hive.pt)
```

### Comparing `dropbox-api-0.2.1/PKG-INFO` & `dropbox-api-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropbox-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: Dropbox API Client
 Home-page: http://dropbox-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Dropbox API](http://dropbox-api.hive.pt)
```

### Comparing `dropbox-api-0.2.1/setup.py` & `dropbox-api-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "dropbox-api",
-    version = "0.2.1",
+    version = "0.2.2",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Dropbox API Client",
     license = "Apache License, Version 2.0",
     keywords = "dropbox api",
     url = "http://dropbox-api.hive.pt",
     zip_safe = False,
```

### Comparing `dropbox-api-0.2.1/README.md` & `dropbox-api-0.2.2/README.md`

 * *Files identical despite different names*

