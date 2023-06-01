# Comparing `tmp/libhxl-5.0.tar.gz` & `tmp/libhxl-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libhxl-5.0.tar", last modified: Thu May 18 15:26:11 2023, max compression
+gzip compressed data, was "libhxl-5.0.1.tar", last modified: Thu Jun  1 16:04:10 2023, max compression
```

## Comparing `libhxl-5.0.tar` & `libhxl-5.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-18 15:26:11.104760 libhxl-5.0/
--rw-rw-r--   0 david     (1001) david     (1001)     1210 2022-10-28 23:20:29.000000 libhxl-5.0/LICENSE.md
--rw-rw-r--   0 david     (1001) david     (1001)       28 2022-10-28 23:20:29.000000 libhxl-5.0/MANIFEST.in
--rw-rw-r--   0 david     (1001) david     (1001)     6393 2023-05-18 15:26:11.104760 libhxl-5.0/PKG-INFO
--rw-rw-r--   0 david     (1001) david     (1001)     6000 2022-10-28 23:20:29.000000 libhxl-5.0/README.md
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-18 15:26:11.100760 libhxl-5.0/hxl/
--rw-rw-r--   0 david     (1001) david     (1001)     3639 2023-05-18 15:24:53.000000 libhxl-5.0/hxl/__init__.py
--rw-rw-r--   0 david     (1001) david     (1001)     6595 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/converters.py
--rw-rw-r--   0 david     (1001) david     (1001)    13116 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/datatypes.py
--rw-rw-r--   0 david     (1001) david     (1001)   105695 2023-03-10 15:48:58.000000 libhxl-5.0/hxl/filters.py
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-18 15:26:11.104760 libhxl-5.0/hxl/formulas/
--rw-rw-r--   0 david     (1001) david     (1001)        0 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/formulas/__init__.py
--rw-rw-r--   0 david     (1001) david     (1001)      703 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/formulas/eval.py
--rw-rw-r--   0 david     (1001) david     (1001)    12797 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/formulas/functions.py
--rw-rw-r--   0 david     (1001) david     (1001)     1010 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/formulas/lexer.py
--rw-rw-r--   0 david     (1001) david     (1001)     1820 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/formulas/parser.py
--rw-rw-r--   0 david     (1001) david     (1001)     3919 2022-10-28 23:20:50.000000 libhxl-5.0/hxl/formulas/parsetab.py
--rw-rw-r--   0 david     (1001) david     (1001)     5788 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/geo.py
--rw-rw-r--   0 david     (1001) david     (1001)     1983 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/hxl-default-schema.json
--rw-rw-r--   0 david     (1001) david     (1001)    67144 2023-05-18 15:23:18.000000 libhxl-5.0/hxl/input.py
--rw-rw-r--   0 david     (1001) david     (1001)    51976 2023-03-10 15:35:47.000000 libhxl-5.0/hxl/model.py
--rw-rw-r--   0 david     (1001) david     (1001)    79626 2023-05-18 15:23:18.000000 libhxl-5.0/hxl/scripts.py
--rw-rw-r--   0 david     (1001) david     (1001)      605 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/util.py
--rw-rw-r--   0 david     (1001) david     (1001)    62582 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/validation.py
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-18 15:26:11.104760 libhxl-5.0/libhxl.egg-info/
--rw-rw-r--   0 david     (1001) david     (1001)     6393 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1001) david     (1001)      541 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1001) david     (1001)        1 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1001) david     (1001)      663 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1001) david     (1001)      153 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/requires.txt
--rw-rw-r--   0 david     (1001) david     (1001)        4 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/top_level.txt
--rw-rw-r--   0 david     (1001) david     (1001)       38 2023-05-18 15:26:11.104760 libhxl-5.0/setup.cfg
--rwxrwxr-x   0 david     (1001) david     (1001)     2134 2023-05-18 15:24:53.000000 libhxl-5.0/setup.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:04:10.749013 libhxl-5.0.1/
+-rw-rw-r--   0 david     (1001) david     (1001)     1210 2022-10-28 23:20:29.000000 libhxl-5.0.1/LICENSE.md
+-rw-rw-r--   0 david     (1001) david     (1001)       28 2022-10-28 23:20:29.000000 libhxl-5.0.1/MANIFEST.in
+-rw-rw-r--   0 david     (1001) david     (1001)     6634 2023-06-01 16:04:10.749013 libhxl-5.0.1/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)     6000 2022-10-28 23:20:29.000000 libhxl-5.0.1/README.md
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:04:10.749013 libhxl-5.0.1/hxl/
+-rw-rw-r--   0 david     (1001) david     (1001)     3641 2023-06-01 16:03:34.000000 libhxl-5.0.1/hxl/__init__.py
+-rw-rw-r--   0 david     (1001) david     (1001)     6595 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/converters.py
+-rw-rw-r--   0 david     (1001) david     (1001)    13116 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/datatypes.py
+-rw-rw-r--   0 david     (1001) david     (1001)   105695 2023-03-10 15:48:58.000000 libhxl-5.0.1/hxl/filters.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:04:10.749013 libhxl-5.0.1/hxl/formulas/
+-rw-rw-r--   0 david     (1001) david     (1001)        0 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/formulas/__init__.py
+-rw-rw-r--   0 david     (1001) david     (1001)      703 2022-11-25 16:01:58.000000 libhxl-5.0.1/hxl/formulas/eval.py
+-rw-rw-r--   0 david     (1001) david     (1001)    12791 2023-06-01 16:03:34.000000 libhxl-5.0.1/hxl/formulas/functions.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1010 2022-11-25 16:01:58.000000 libhxl-5.0.1/hxl/formulas/lexer.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1820 2022-11-25 16:01:58.000000 libhxl-5.0.1/hxl/formulas/parser.py
+-rw-rw-r--   0 david     (1001) david     (1001)     3919 2022-10-28 23:20:50.000000 libhxl-5.0.1/hxl/formulas/parsetab.py
+-rw-rw-r--   0 david     (1001) david     (1001)     5788 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/geo.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1983 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/hxl-default-schema.json
+-rw-rw-r--   0 david     (1001) david     (1001)    67060 2023-06-01 16:03:34.000000 libhxl-5.0.1/hxl/input.py
+-rw-rw-r--   0 david     (1001) david     (1001)    51976 2023-03-10 15:35:47.000000 libhxl-5.0.1/hxl/model.py
+-rw-rw-r--   0 david     (1001) david     (1001)    79626 2023-05-18 15:23:18.000000 libhxl-5.0.1/hxl/scripts.py
+-rw-rw-r--   0 david     (1001) david     (1001)      605 2022-11-25 16:01:58.000000 libhxl-5.0.1/hxl/util.py
+-rw-rw-r--   0 david     (1001) david     (1001)    62582 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/validation.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:04:10.749013 libhxl-5.0.1/libhxl.egg-info/
+-rw-rw-r--   0 david     (1001) david     (1001)     6634 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)      541 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1001) david     (1001)        1 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1001) david     (1001)      663 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1001) david     (1001)      118 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/requires.txt
+-rw-rw-r--   0 david     (1001) david     (1001)        4 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1001) david     (1001)       38 2023-06-01 16:04:10.749013 libhxl-5.0.1/setup.cfg
+-rwxrwxr-x   0 david     (1001) david     (1001)     2355 2023-06-01 16:03:34.000000 libhxl-5.0.1/setup.py
```

### Comparing `libhxl-5.0/LICENSE.md` & `libhxl-5.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/PKG-INFO` & `libhxl-5.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: libhxl
-Version: 5.0
+Version: 5.0.1
 Summary: Python support library for the Humanitarian Exchange Language (HXL). See http://hxlstandard.org and https://github.com/HXLStandard/libhxl-python
 Home-page: http://hxlproject.org
 Author: David Megginson
 Author-email: megginson@un.org
 License: UNKNOWN
+Project-URL: Documentation, https://hxlstandard.github.io/libhxl-python/index.html
+Project-URL: GitHub, https://github.com/HXLStandard/libhxl-python/
+Project-URL: Changelog, https://github.com/HXLStandard/libhxl-python/blob/prod/CHANGELOG
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 libhxl-python
 =============
```

### Comparing `libhxl-5.0/README.md` & `libhxl-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/__init__.py` & `libhxl-5.0.1/hxl/__init__.py`

 * *Files identical despite different names*

```diff
@@ -77,15 +77,15 @@
 """
 
 import sys
 
 if sys.version_info < (3,):
     raise RuntimeError("libhxl requires Python 3 or higher")
 
-__version__="5.0"
+__version__="5.0.1"
 """Module version number
 see https://www.python.org/dev/peps/pep-0396/
 """
 
 # Flatten out common items for easier access
 
 class HXLException(Exception):
```

### Comparing `libhxl-5.0/hxl/converters.py` & `libhxl-5.0.1/hxl/converters.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/datatypes.py` & `libhxl-5.0.1/hxl/datatypes.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/filters.py` & `libhxl-5.0.1/hxl/filters.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/formulas/eval.py` & `libhxl-5.0.1/hxl/formulas/eval.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/formulas/functions.py` & `libhxl-5.0.1/hxl/formulas/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,10 +372,10 @@
     Otherwise, return zero and log a warning.
     """
     if not arg:
         return 0
     try:
         return hxl.datatypes.normalise_number(arg)
     except (ValueError, TypeError):
-        logup('Cannot convert to a number for calculated field', {"arg": arg}, level='warning')
-        logger.warning("Cannot convert %s to a number for calculated field", arg)
+        logup('Cannot convert to a number for calculated field', {"arg": arg}, level='info')
+        logger.info("Cannot convert %s to a number for calculated field", arg)
         return 0
```

### Comparing `libhxl-5.0/hxl/formulas/lexer.py` & `libhxl-5.0.1/hxl/formulas/lexer.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/formulas/parser.py` & `libhxl-5.0.1/hxl/formulas/parser.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/formulas/parsetab.py` & `libhxl-5.0.1/hxl/formulas/parsetab.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/geo.py` & `libhxl-5.0.1/hxl/geo.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/hxl-default-schema.json` & `libhxl-5.0.1/hxl/hxl-default-schema.json`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/input.py` & `libhxl-5.0.1/hxl/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import hxl, hxl.filters
 
 from hxl.util import logup
 
 import abc, collections, csv, datetime, dateutil.parser, hashlib, \
     io, io_wrapper, json, jsonpath_ng.ext, logging, \
-    os.path, re, requests, requests_cache, shutil, six, sys, \
+    os.path, re, requests, shutil, six, sys, \
     tempfile, time, urllib.parse, xlrd3 as xlrd, zipfile
 
 logger = logging.getLogger(__name__)
 
 __all__ = (
     "data",
     "tagger",
@@ -1875,22 +1875,21 @@
 
     info_url = response.json().get("url")
 
     # 3. Look up the data record for the export to get the download URL
 
     fail_counter = 0
     while True:
-        with requests_cache.disabled():
-            logup("Getting info for Kobo export", {"url": info_url})
-            response = requests.get(
-                info_url,
-                verify=input_options.verify_ssl,
-                headers=http_headers
-            )
-            logup("Response for Kobo info", {"url": info_url, "status": response.status_code})
+        logup("Getting info for Kobo export", {"url": info_url})
+        response = requests.get(
+            info_url,
+            verify=input_options.verify_ssl,
+            headers=http_headers
+        )
+        logup("Response for Kobo info", {"url": info_url, "status": response.status_code})
 
         # check for errors
         if (response.status_code == 403): # CKAN sends "403 Forbidden" for a private file
             raise HXLAuthorizationException("Access not authorized", url=info_url)
         else:
             response.raise_for_status()
```

### Comparing `libhxl-5.0/hxl/model.py` & `libhxl-5.0.1/hxl/model.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/scripts.py` & `libhxl-5.0.1/hxl/scripts.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/util.py` & `libhxl-5.0.1/hxl/util.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/hxl/validation.py` & `libhxl-5.0.1/hxl/validation.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/libhxl.egg-info/PKG-INFO` & `libhxl-5.0.1/libhxl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: libhxl
-Version: 5.0
+Version: 5.0.1
 Summary: Python support library for the Humanitarian Exchange Language (HXL). See http://hxlstandard.org and https://github.com/HXLStandard/libhxl-python
 Home-page: http://hxlproject.org
 Author: David Megginson
 Author-email: megginson@un.org
 License: UNKNOWN
+Project-URL: Documentation, https://hxlstandard.github.io/libhxl-python/index.html
+Project-URL: GitHub, https://github.com/HXLStandard/libhxl-python/
+Project-URL: Changelog, https://github.com/HXLStandard/libhxl-python/blob/prod/CHANGELOG
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 libhxl-python
 =============
```

### Comparing `libhxl-5.0/libhxl.egg-info/SOURCES.txt` & `libhxl-5.0.1/libhxl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/libhxl.egg-info/entry_points.txt` & `libhxl-5.0.1/libhxl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `libhxl-5.0/setup.py` & `libhxl-5.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,32 +7,36 @@
     raise RuntimeError("libhxl requires Python 3 or higher")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='libhxl',
-    version="5.0",
+    version="5.0.1",
     description='Python support library for the Humanitarian Exchange Language (HXL). See http://hxlstandard.org and https://github.com/HXLStandard/libhxl-python',
     long_description=long_description,
     long_description_content_type="text/markdown",
+    project_urls={
+        'Documentation': 'https://hxlstandard.github.io/libhxl-python/index.html',
+        'GitHub': 'https://github.com/HXLStandard/libhxl-python/',
+        'Changelog': 'https://github.com/HXLStandard/libhxl-python/blob/prod/CHANGELOG',
+    },
     author='David Megginson',
     author_email='megginson@un.org',
     url='http://hxlproject.org',
     install_requires=[
-        'urllib3>=1.21.1,<1.27', # version required by requests
         'jsonpath_ng',
         'ply',
         'pytest',
         'python-dateutil',
         'python-io-wrapper>=0.2',
-        'requests>=2.27',
-        'requests_cache',
+        'requests',
         'structlog',
         'unidecode',
+        'urllib3', # version required by requests
         'wheel',
         'xlrd3>=1.1.0',
     ],
     packages=['hxl', 'hxl.formulas'],
     package_data={'hxl': ['*.json']},
     include_package_data=True,
     test_suite='tests',
```

