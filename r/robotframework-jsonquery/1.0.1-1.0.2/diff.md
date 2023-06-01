# Comparing `tmp/robotframework_jsonquery-1.0.1.tar.gz` & `tmp/robotframework_jsonquery-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_jsonquery-1.0.1.tar", max compression
+gzip compressed data, was "robotframework_jsonquery-1.0.2.tar", max compression
```

## Comparing `robotframework_jsonquery-1.0.1.tar` & `robotframework_jsonquery-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1665 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/JsonQuery.py
--rw-r--r--   0        0        0       33 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/__init__.py
--rw-r--r--   0        0        0      213 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/errors.py
--rw-r--r--   0        0        0      242 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/module_importer.py
--rw-r--r--   0        0        0      713 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/queries.py
--rw-r--r--   0        0        0     1063 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/LICENSE
--rw-r--r--   0        0        0      895 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/README.md
--rw-r--r--   0        0        0      507 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 robotframework_jsonquery-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2474 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/JsonQuery.py
+-rw-r--r--   0        0        0       33 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/errors.py
+-rw-r--r--   0        0        0      242 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/module_importer.py
+-rw-r--r--   0        0        0      713 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/queries.py
+-rw-r--r--   0        0        0     1063 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1160 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/README.md
+-rw-r--r--   0        0        0      507 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 robotframework_jsonquery-1.0.2/PKG-INFO
```

### Comparing `robotframework_jsonquery-1.0.1/JsonQuery/queries.py` & `robotframework_jsonquery-1.0.2/JsonQuery/queries.py`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.1/LICENSE` & `robotframework_jsonquery-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.1/README.md` & `robotframework_jsonquery-1.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-# robotframework-jsonquery [![tests](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml/badge.svg?branch=master)](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml)
+# robotframework-jsonquery [![tests](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml/badge.svg?branch=master)](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml) [![PyPI version](https://badge.fury.io/py/robotframework-jsonquery.svg)](https://badge.fury.io/py/robotframework-jsonquery)
 Simple wrapper for libraries used to query json files with different query language implementations
 - jsonpath-ng.ext (extended version with e.g. filters)
 - jsonpath-ng
 - jmespath
 
 Example:
 ```Robot Framework
 *** Settings ***
 Library    JsonQuery    jsonpath-ng.ext
 
 *** Test Cases ***
 Read and query json file
     ${file}    Read Json File    sample.json
-    Query Json    ${file}    friends[?(@.id>1)]    #jsonpath-ng.ext syntax
+    ${result}   Query Json    ${file}    friends[?(@.id>1)]    #jsonpath-ng.ext syntax
 
 ```
 
 ```Robot Framework
 *** Settings ***
 Library    JsonQuery    jmespath
 
 *** Test Cases ***
 Read and query json file
     ${file}    Read Json File    sample.json
-    Query Json    ${file}    friends[?id>`1`]    #jmespath syntax
+    ${result}   Query Json    ${file}    friends[?id>`1`]    #jmespath syntax
 
 ```
+
+## Documentation
+-   [Keyword Documentation](https://github.com/otemek/robotframework-jsonquery/doc/JsonQuery.html)
```

### Comparing `robotframework_jsonquery-1.0.1/PKG-INFO` & `robotframework_jsonquery-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-jsonquery
-Version: 1.0.1
+Version: 1.0.2
 Summary: Robot Framework library for parsing json files
 License: MIT
 Author: tom bsc
 Author-email: etombsc@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,36 +12,39 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jmespath (<2)
 Requires-Dist: jsonpath_ng (<2)
 Requires-Dist: robotframework
 Description-Content-Type: text/markdown
 
-# robotframework-jsonquery [![tests](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml/badge.svg?branch=master)](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml)
+# robotframework-jsonquery [![tests](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml/badge.svg?branch=master)](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml) [![PyPI version](https://badge.fury.io/py/robotframework-jsonquery.svg)](https://badge.fury.io/py/robotframework-jsonquery)
 Simple wrapper for libraries used to query json files with different query language implementations
 - jsonpath-ng.ext (extended version with e.g. filters)
 - jsonpath-ng
 - jmespath
 
 Example:
 ```Robot Framework
 *** Settings ***
 Library    JsonQuery    jsonpath-ng.ext
 
 *** Test Cases ***
 Read and query json file
     ${file}    Read Json File    sample.json
-    Query Json    ${file}    friends[?(@.id>1)]    #jsonpath-ng.ext syntax
+    ${result}   Query Json    ${file}    friends[?(@.id>1)]    #jsonpath-ng.ext syntax
 
 ```
 
 ```Robot Framework
 *** Settings ***
 Library    JsonQuery    jmespath
 
 *** Test Cases ***
 Read and query json file
     ${file}    Read Json File    sample.json
-    Query Json    ${file}    friends[?id>`1`]    #jmespath syntax
+    ${result}   Query Json    ${file}    friends[?id>`1`]    #jmespath syntax
 
 ```
 
+## Documentation
+-   [Keyword Documentation](https://github.com/otemek/robotframework-jsonquery/doc/JsonQuery.html)
+
```

