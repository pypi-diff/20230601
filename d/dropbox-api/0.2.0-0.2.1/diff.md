# Comparing `tmp/dropbox-api-0.2.0.tar.gz` & `tmp/dropbox-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dropbox-api-0.2.0.tar", last modified: Wed May 31 18:20:30 2023, max compression
+gzip compressed data, was "dist/dropbox-api-0.2.1.tar", last modified: Thu Jun  1 03:13:41 2023, max compression
```

## Comparing `dropbox-api-0.2.0.tar` & `dropbox-api-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox/
--rw-r--r--   0 root         (0) root         (0)     1655 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/user.py
--rw-r--r--   0 root         (0) root         (0)     1406 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/shared_link.py
--rw-r--r--   0 root         (0) root         (0)     2888 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/base.py
--rw-r--r--   0 root         (0) root         (0)     6040 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:20:25.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2732 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox/
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/user.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/shared_link.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/base.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/src/dropbox/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 03:13:37.000000 dropbox-api-0.2.1/src/dropbox_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-01 03:13:41.000000 dropbox-api-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-06-01 03:13:35.000000 dropbox-api-0.2.1/README.md
```

### Comparing `dropbox-api-0.2.0/src/dropbox/user.py` & `dropbox-api-0.2.1/src/dropbox/user.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.0/src/dropbox/__init__.py` & `dropbox-api-0.2.1/src/dropbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.0/src/dropbox/shared_link.py` & `dropbox-api-0.2.1/src/dropbox/shared_link.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.0/src/dropbox/base.py` & `dropbox-api-0.2.1/src/dropbox/base.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.0/src/dropbox/file.py` & `dropbox-api-0.2.1/src/dropbox/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,19 @@
                 "Content-Type" : "application/octet-stream",
                 "Dropbox-API-Arg" : json.dumps(params)
             },
             timeout = timeout
         )
         return contents
 
+    def metadata_file(self, path):
+        url = self.base_url + "files/get_metadata"
+        contents = self.post(url, data_j = dict(path = path))
+        return contents
+
     def download_file(self, path):
         url = self.content_url + "files/download"
         params = dict(path = path)
         contents, response = self.post(
             url,
             headers = {
                 "Dropbox-API-Arg" : json.dumps(params)
```

### Comparing `dropbox-api-0.2.0/src/dropbox_api.egg-info/PKG-INFO` & `dropbox-api-0.2.1/src/dropbox_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropbox-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dropbox API Client
 Home-page: http://dropbox-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Dropbox API](http://dropbox-api.hive.pt)
         
@@ -19,14 +19,15 @@
         ## License
         
         Dropbox API is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
         
         ## Build Automation
         
         [![Build Status](https://app.travis-ci.com/hivesolutions/dropbox-api.svg?branch=master)](https://travis-ci.com/github/hivesolutions/dropbox-api)
+        [![Build Status GitHub](https://github.com/hivesolutions/dropbox-api/workflows/Main%20Workflow/badge.svg)](https://github.com/hivesolutions/dropbox-api/actions)
         [![Coverage Status](https://coveralls.io/repos/hivesolutions/dropbox-api/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/dropbox-api?branch=master)
         [![PyPi Status](https://img.shields.io/pypi/v/dropbox-api.svg)](https://pypi.python.org/pypi/dropbox-api)
         [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
         
 Keywords: dropbox api
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dropbox-api-0.2.0/PKG-INFO` & `dropbox-api-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropbox-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dropbox API Client
 Home-page: http://dropbox-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Dropbox API](http://dropbox-api.hive.pt)
         
@@ -19,14 +19,15 @@
         ## License
         
         Dropbox API is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
         
         ## Build Automation
         
         [![Build Status](https://app.travis-ci.com/hivesolutions/dropbox-api.svg?branch=master)](https://travis-ci.com/github/hivesolutions/dropbox-api)
+        [![Build Status GitHub](https://github.com/hivesolutions/dropbox-api/workflows/Main%20Workflow/badge.svg)](https://github.com/hivesolutions/dropbox-api/actions)
         [![Coverage Status](https://coveralls.io/repos/hivesolutions/dropbox-api/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/dropbox-api?branch=master)
         [![PyPi Status](https://img.shields.io/pypi/v/dropbox-api.svg)](https://pypi.python.org/pypi/dropbox-api)
         [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
         
 Keywords: dropbox api
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dropbox-api-0.2.0/setup.py` & `dropbox-api-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "dropbox-api",
-    version = "0.2.0",
+    version = "0.2.1",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Dropbox API Client",
     license = "Apache License, Version 2.0",
     keywords = "dropbox api",
     url = "http://dropbox-api.hive.pt",
     zip_safe = False,
```

### Comparing `dropbox-api-0.2.0/README.md` & `dropbox-api-0.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 ## License
 
 Dropbox API is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
 
 ## Build Automation
 
 [![Build Status](https://app.travis-ci.com/hivesolutions/dropbox-api.svg?branch=master)](https://travis-ci.com/github/hivesolutions/dropbox-api)
+[![Build Status GitHub](https://github.com/hivesolutions/dropbox-api/workflows/Main%20Workflow/badge.svg)](https://github.com/hivesolutions/dropbox-api/actions)
 [![Coverage Status](https://coveralls.io/repos/hivesolutions/dropbox-api/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/dropbox-api?branch=master)
 [![PyPi Status](https://img.shields.io/pypi/v/dropbox-api.svg)](https://pypi.python.org/pypi/dropbox-api)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
```

