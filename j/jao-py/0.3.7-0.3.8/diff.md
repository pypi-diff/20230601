# Comparing `tmp/jao-py-0.3.7.tar.gz` & `tmp/jao-py-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jao-py-0.3.7.tar", last modified: Sat May 27 20:19:50 2023, max compression
+gzip compressed data, was "jao-py-0.3.8.tar", last modified: Thu Jun  1 07:53:46 2023, max compression
```

## Comparing `jao-py-0.3.7.tar` & `jao-py-0.3.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-27 20:19:41.000000 jao-py-0.3.7/LICENSE.MD
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-27 20:19:50.689649 jao-py-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-27 20:19:41.000000 jao-py-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/jao/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/jao/CWE/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/jao/beta/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/beta/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/webservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/jao_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-27 20:19:50.693649 jao-py-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-27 20:19:41.000000 jao-py-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.144340 jao-py-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 07:53:35.000000 jao-py-0.3.8/LICENSE.MD
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-01 07:53:46.144340 jao-py-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-01 07:53:35.000000 jao-py-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.140340 jao-py-0.3.8/jao/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.144340 jao-py-0.3.8/jao/CWE/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.144340 jao-py-0.3.8/jao/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/beta/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.144340 jao-py-0.3.8/jao_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 07:53:46.144340 jao-py-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-01 07:53:35.000000 jao-py-0.3.8/setup.py
```

### Comparing `jao-py-0.3.7/LICENSE.MD` & `jao-py-0.3.8/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.7/PKG-INFO` & `jao-py-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.3.7
+Version: 0.3.8
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jao-py-0.3.7/README.md` & `jao-py-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.7/jao/CWE/jao.py` & `jao-py-0.3.8/jao/CWE/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.7/jao/CWE/parsers.py` & `jao-py-0.3.8/jao/CWE/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.7/jao/beta/jao.py` & `jao-py-0.3.8/jao/beta/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.7/jao/jao.py` & `jao-py-0.3.8/jao/jao.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import itertools
 from .exceptions import NoMatchingDataError
 from .parsers import parse_final_domain, parse_base_output
 from typing import List, Dict
 from .util import to_snake_case
 
 __title__ = "jao-py"
-__version__ = "0.3.7"
+__version__ = "0.3.8"
 __author__ = "Frank Boerman"
 __license__ = "MIT"
 
 
 class JaoPublicationToolClient:
     BASEURL = "https://publicationtool.jao.eu/core/api/core/"
     BASEURL2 = "https://publicationtool.jao.eu/core/api/data/"
@@ -116,14 +116,16 @@
         data = []
         for mtu in pd.date_range(day, day + pd.Timedelta(days=1), freq='1h'):
             r = self.s.get(self.BASEURL + 'shadowPrices/index', params={
                 'date': mtu.isoformat()
             })
             r.raise_for_status()
             data += r.json()['data']
+        if len(data) == 0:
+            raise NoMatchingDataError
 
         return data
 
     def query_validations(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> List[Dict]:
         return self._query_base_fromto(d_from, d_to, 'validationReductions')
 
     def query_maxbex(self, day: pd.Timestamp) -> List[Dict]:
```

### Comparing `jao-py-0.3.7/jao/parsers.py` & `jao-py-0.3.8/jao/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.7/jao/webservice.py` & `jao-py-0.3.8/jao/webservice.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.7/jao_py.egg-info/PKG-INFO` & `jao-py-0.3.8/jao_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.3.7
+Version: 0.3.8
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jao-py-0.3.7/setup.py` & `jao-py-0.3.8/setup.py`

 * *Files identical despite different names*

