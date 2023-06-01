# Comparing `tmp/harmony-py-0.4.7.tar.gz` & `tmp/harmony-py-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony-py-0.4.7.tar", last modified: Mon May  1 15:02:22 2023, max compression
+gzip compressed data, was "harmony-py-0.4.8.tar", last modified: Thu Jun  1 14:56:47 2023, max compression
```

## Comparing `harmony-py-0.4.7.tar` & `harmony-py-0.4.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:22.720744 harmony-py-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-01 15:01:37.000000 harmony-py-0.4.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-01 15:01:37.000000 harmony-py-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 15:01:37.000000 harmony-py-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-01 15:02:22.720744 harmony-py-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-01 15:01:37.000000 harmony-py-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:22.720744 harmony-py-0.4.7/harmony/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 15:02:16.000000 harmony-py-0.4.7/harmony/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-01 15:01:37.000000 harmony-py-0.4.7/harmony/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-01 15:01:37.000000 harmony-py-0.4.7/harmony/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    50839 2023-05-01 15:01:37.000000 harmony-py-0.4.7/harmony/harmony.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 15:01:37.000000 harmony-py-0.4.7/harmony/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:22.720744 harmony-py-0.4.7/harmony_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 15:02:22.724745 harmony-py-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-01 15:01:37.000000 harmony-py-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:22.720744 harmony-py-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    47105 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:47.493812 harmony-py-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-01 14:55:40.000000 harmony-py-0.4.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-01 14:55:40.000000 harmony-py-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 14:55:40.000000 harmony-py-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-01 14:56:47.493812 harmony-py-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-01 14:55:40.000000 harmony-py-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:47.493812 harmony-py-0.4.8/harmony/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-01 14:56:40.000000 harmony-py-0.4.8/harmony/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-01 14:55:40.000000 harmony-py-0.4.8/harmony/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-01 14:55:40.000000 harmony-py-0.4.8/harmony/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51063 2023-06-01 14:55:40.000000 harmony-py-0.4.8/harmony/harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-01 14:55:40.000000 harmony-py-0.4.8/harmony/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:47.493812 harmony-py-0.4.8/harmony_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 14:56:47.493812 harmony-py-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 14:55:40.000000 harmony-py-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:47.493812 harmony-py-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48449 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_util.py
```

### Comparing `harmony-py-0.4.7/CONTRIBUTING.md` & `harmony-py-0.4.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.7/LICENSE` & `harmony-py-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.7/PKG-INFO` & `harmony-py-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: harmony-py
-Version: 0.4.7
+Version: 0.4.8
 Summary: The NASA Harmony Python library
 Home-page: https://github.com/nasa/harmony-py
 Keywords: nasa,harmony,remote-sensing,science,geoscience
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # harmony-py
 
+[![Documentation Status](https://readthedocs.org/projects/harmony-py/badge/?version=latest)](https://harmony-py.readthedocs.io/en/latest/?badge=latest)
+
 Harmony-Py is a Python library for integrating with NASA's [Harmony](https://harmony.earthdata.nasa.gov/) Services.
 
 Harmony-Py provides a Python alternative to directly using [Harmony's RESTful API](https://harmony.earthdata.nasa.gov/docs/api/). It handles NASA [Earthdata Login (EDL)](https://urs.earthdata.nasa.gov/home) authentication and optionally integrates with the [CMR Python Wrapper](https://github.com/nasa/eo-metadata-tools) by accepting collection results as a request parameter. It's convenient for scientists who wish to use Harmony from Jupyter notebooks as well as machine-to-machine communication with larger Python applications.
 
 We welcome feedback on Harmony-Py via [GitHub Issues](https://github.com/nasa/harmony-py/issues)
 
-[![Documentation Status](https://readthedocs.org/projects/harmony-py/badge/?version=latest)](https://harmony-py.readthedocs.io/en/latest/?badge=latest)
-
 # Using Harmony Py
 
 ## Prerequisites
 
 * Python 3.7+
```

### Comparing `harmony-py-0.4.7/README.md` & `harmony-py-0.4.8/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # harmony-py
 
+[![Documentation Status](https://readthedocs.org/projects/harmony-py/badge/?version=latest)](https://harmony-py.readthedocs.io/en/latest/?badge=latest)
+
 Harmony-Py is a Python library for integrating with NASA's [Harmony](https://harmony.earthdata.nasa.gov/) Services.
 
 Harmony-Py provides a Python alternative to directly using [Harmony's RESTful API](https://harmony.earthdata.nasa.gov/docs/api/). It handles NASA [Earthdata Login (EDL)](https://urs.earthdata.nasa.gov/home) authentication and optionally integrates with the [CMR Python Wrapper](https://github.com/nasa/eo-metadata-tools) by accepting collection results as a request parameter. It's convenient for scientists who wish to use Harmony from Jupyter notebooks as well as machine-to-machine communication with larger Python applications.
 
 We welcome feedback on Harmony-Py via [GitHub Issues](https://github.com/nasa/harmony-py/issues)
 
-[![Documentation Status](https://readthedocs.org/projects/harmony-py/badge/?version=latest)](https://harmony-py.readthedocs.io/en/latest/?badge=latest)
-
 # Using Harmony Py
 
 ## Prerequisites
 
 * Python 3.7+
```

### Comparing `harmony-py-0.4.7/harmony/auth.py` & `harmony-py-0.4.8/harmony/auth.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.7/harmony/config.py` & `harmony-py-0.4.8/harmony/config.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.7/harmony/harmony.py` & `harmony-py-0.4.8/harmony/harmony.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """This module defines the main classes used to interact with Harmony.
 
 The classes defined here are also available by importing them from the
 top-level ``harmony`` package, e.g.::
 
     from harmony import Client, Request
 
+
 Overview of the classes:
 
+
     * Collection: A CMR Collection ID
+
     * BBox: A bounding box (lat/lon) used in Requests
+
     * Request: A complete Harmony request with all criteria
+
     * Client: Allows submission of a Harmony Request and getting results
+
 """
+
 from http.client import ResponseNotReady
 import os
 import shutil
 import sys
 from tabnanny import check
 import time
 import platform
@@ -740,15 +747,15 @@
               can't be reached.
         """
         session = self._session()
         response = session.get(self._status_url(job_id))
         if response.ok:
             fields = [
                 'status', 'message', 'progress', 'createdAt', 'updatedAt', 'dataExpiration',
-                'request', 'numInputGranules'
+                'request', 'errors', 'numInputGranules'
             ]
             status_subset = {k: v for k, v in response.json().items() if k in fields}
             created_at_dt = dateutil.parser.parse(status_subset['createdAt'])
             updated_at_dt = dateutil.parser.parse(status_subset['updatedAt'])
 
             status_json = {
                 'status': status_subset['status'],
@@ -764,14 +771,16 @@
             }
             if 'dataExpiration' in status_subset:
                 data_expiration_dt = dateutil.parser.parse(status_subset['dataExpiration'])
                 data_expiration_local = data_expiration_dt.replace(
                     microsecond=0).astimezone().isoformat()
                 status_json['data_expiration'] = data_expiration_dt
                 status_json['data_expiration_local'] = data_expiration_local
+            if 'errors' in status_subset:
+                status_json['errors'] = status_subset['errors']
             return status_json
         else:
             self._handle_error_response(response)
 
     def pause(self, job_id: str):
         """Pause a job.
 
@@ -1004,15 +1013,18 @@
 
         verbose = os.getenv('VERBOSE', 'TRUE')
         if not overwrite and os.path.isfile(filename):
             if verbose and verbose.upper() == 'TRUE':
                 print(filename)
             return filename
         else:
-            with session.get(url, stream=True) as r:
+            headers = {
+                "Accept-Encoding": "identity"
+            }
+            with session.get(url, stream=True, headers=headers) as r:
                 with open(filename, 'wb') as f:
                     shutil.copyfileobj(r.raw, f, length=chunksize)
             if verbose and verbose.upper() == 'TRUE':
                 print(filename)
             return filename
 
     def download(self, url: str, directory: str = '', overwrite: bool = False) -> Future:
```

### Comparing `harmony-py-0.4.7/harmony/util.py` & `harmony-py-0.4.8/harmony/util.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.7/harmony_py.egg-info/PKG-INFO` & `harmony-py-0.4.8/harmony_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: harmony-py
-Version: 0.4.7
+Version: 0.4.8
 Summary: The NASA Harmony Python library
 Home-page: https://github.com/nasa/harmony-py
 Keywords: nasa,harmony,remote-sensing,science,geoscience
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # harmony-py
 
+[![Documentation Status](https://readthedocs.org/projects/harmony-py/badge/?version=latest)](https://harmony-py.readthedocs.io/en/latest/?badge=latest)
+
 Harmony-Py is a Python library for integrating with NASA's [Harmony](https://harmony.earthdata.nasa.gov/) Services.
 
 Harmony-Py provides a Python alternative to directly using [Harmony's RESTful API](https://harmony.earthdata.nasa.gov/docs/api/). It handles NASA [Earthdata Login (EDL)](https://urs.earthdata.nasa.gov/home) authentication and optionally integrates with the [CMR Python Wrapper](https://github.com/nasa/eo-metadata-tools) by accepting collection results as a request parameter. It's convenient for scientists who wish to use Harmony from Jupyter notebooks as well as machine-to-machine communication with larger Python applications.
 
 We welcome feedback on Harmony-Py via [GitHub Issues](https://github.com/nasa/harmony-py/issues)
 
-[![Documentation Status](https://readthedocs.org/projects/harmony-py/badge/?version=latest)](https://harmony-py.readthedocs.io/en/latest/?badge=latest)
-
 # Using Harmony Py
 
 ## Prerequisites
 
 * Python 3.7+
```

### Comparing `harmony-py-0.4.7/setup.py` & `harmony-py-0.4.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
     ],
     keywords='nasa, harmony, remote-sensing, science, geoscience',
     packages=find_packages(exclude=['tests']),
     python_requires='>=3.6, <4',
     install_requires=DEPENDENCIES,
     extras_require={
```

### Comparing `harmony-py-0.4.7/tests/test_auth.py` & `harmony-py-0.4.8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.7/tests/test_client.py` & `harmony-py-0.4.8/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -497,14 +497,44 @@
 
     assert len(responses.calls) == 1
     assert responses.calls[0].request is not None
     assert urllib.parse.unquote(responses.calls[0].request.url) == expected_status_url(job_id)
     assert actual_status == expected_status
 
 @responses.activate
+def test_status_with_errors():
+    collection = Collection(id='C333666999-EOSDIS')
+    job_id = '21469294-d6f7-42cc-89f2-c81990a5d7f4'
+    exp_job = expected_job(collection.id, job_id)
+    exp_job['errors'] = ['some error']
+    expected_status = {
+        'status': exp_job['status'],
+        'message': exp_job['message'],
+        'progress': exp_job['progress'],
+        'created_at': dateutil.parser.parse(exp_job['createdAt']),
+        'updated_at': dateutil.parser.parse(exp_job['updatedAt']),
+        'data_expiration': dateutil.parser.parse(exp_job['dataExpiration']),
+        'created_at_local': dateutil.parser.parse(exp_job['createdAt']).replace(microsecond=0).astimezone().isoformat(),
+        'updated_at_local': dateutil.parser.parse(exp_job['updatedAt']).replace(microsecond=0).astimezone().isoformat(),
+        'data_expiration_local': dateutil.parser.parse(exp_job['dataExpiration']).replace(microsecond=0).astimezone().isoformat(),
+        'request': exp_job['request'],
+        'errors': ['some error'],
+        'num_input_granules': exp_job['numInputGranules']}
+    responses.add(
+        responses.GET,
+        expected_status_url(job_id),
+        status=200,
+        json=exp_job
+    )
+
+    actual_status = Client(should_validate_auth=False).status(job_id)
+
+    assert actual_status == expected_status
+
+@responses.activate
 def test_status_no_key_error_on_missing_expiration():
     collection = Collection(id='C333666999-EOSDIS')
     job_id = '21469294-d6f7-42cc-89f2-c81990a5d7f4'
     exp_job = expected_job(collection.id, job_id)
     del exp_job['dataExpiration']
     expected_status = {
         'status': exp_job['status'],
```

### Comparing `harmony-py-0.4.7/tests/test_config.py` & `harmony-py-0.4.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.7/tests/test_request.py` & `harmony-py-0.4.8/tests/test_request.py`

 * *Files identical despite different names*

