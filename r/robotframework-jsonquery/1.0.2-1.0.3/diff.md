# Comparing `tmp/robotframework_jsonquery-1.0.2.tar.gz` & `tmp/robotframework_jsonquery-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_jsonquery-1.0.2.tar", max compression
+gzip compressed data, was "robotframework_jsonquery-1.0.3.tar", max compression
```

## Comparing `robotframework_jsonquery-1.0.2.tar` & `robotframework_jsonquery-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2474 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/JsonQuery.py
--rw-r--r--   0        0        0       33 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/__init__.py
--rw-r--r--   0        0        0      213 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/errors.py
--rw-r--r--   0        0        0      242 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/module_importer.py
--rw-r--r--   0        0        0      713 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/JsonQuery/queries.py
--rw-r--r--   0        0        0     1063 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/LICENSE
--rw-r--r--   0        0        0     1160 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/README.md
--rw-r--r--   0        0        0      507 2023-06-01 08:37:38.014511 robotframework_jsonquery-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 robotframework_jsonquery-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2474 2023-06-01 09:32:45.963872 robotframework_jsonquery-1.0.3/JsonQuery/JsonQuery.py
+-rw-r--r--   0        0        0       33 2023-06-01 09:32:45.963872 robotframework_jsonquery-1.0.3/JsonQuery/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-01 09:32:45.963872 robotframework_jsonquery-1.0.3/JsonQuery/errors.py
+-rw-r--r--   0        0        0      242 2023-06-01 09:32:45.963872 robotframework_jsonquery-1.0.3/JsonQuery/module_importer.py
+-rw-r--r--   0        0        0      713 2023-06-01 09:32:45.963872 robotframework_jsonquery-1.0.3/JsonQuery/queries.py
+-rw-r--r--   0        0        0     1063 2023-06-01 09:32:45.963872 robotframework_jsonquery-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1155 2023-06-01 09:32:45.963872 robotframework_jsonquery-1.0.3/README.md
+-rw-r--r--   0        0        0      764 2023-06-01 09:32:45.963872 robotframework_jsonquery-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 robotframework_jsonquery-1.0.3/PKG-INFO
```

### Comparing `robotframework_jsonquery-1.0.2/JsonQuery/JsonQuery.py` & `robotframework_jsonquery-1.0.3/JsonQuery/JsonQuery.py`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.2/JsonQuery/queries.py` & `robotframework_jsonquery-1.0.3/JsonQuery/queries.py`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.2/LICENSE` & `robotframework_jsonquery-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.2/README.md` & `robotframework_jsonquery-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 Read and query json file
     ${file}    Read Json File    sample.json
     ${result}   Query Json    ${file}    friends[?id>`1`]    #jmespath syntax
 
 ```
 
 ## Documentation
--   [Keyword Documentation](https://github.com/otemek/robotframework-jsonquery/doc/JsonQuery.html)
+-   [Keyword Documentation](https://otemek.github.io/robotframework-jsonquery/JsonQuery.html)
```

### Comparing `robotframework_jsonquery-1.0.2/PKG-INFO` & `robotframework_jsonquery-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: robotframework-jsonquery
-Version: 1.0.2
+Version: 1.0.3
 Summary: Robot Framework library for parsing json files
+Home-page: https://github.com/otemek/robotframework-jsonquery
 License: MIT
 Author: tom bsc
 Author-email: etombsc@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: Framework :: Robot Framework :: Library
+Classifier: Framework :: Robot Framework :: Tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jmespath (<2)
 Requires-Dist: jsonpath_ng (<2)
 Requires-Dist: robotframework
+Project-URL: Documentation, https://otemek.github.io/robotframework-jsonquery/JsonQuery.html
+Project-URL: Repository, https://github.com/otemek/robotframework-jsonquery
 Description-Content-Type: text/markdown
 
 # robotframework-jsonquery [![tests](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml/badge.svg?branch=master)](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml) [![PyPI version](https://badge.fury.io/py/robotframework-jsonquery.svg)](https://badge.fury.io/py/robotframework-jsonquery)
 Simple wrapper for libraries used to query json files with different query language implementations
 - jsonpath-ng.ext (extended version with e.g. filters)
 - jsonpath-ng
 - jmespath
@@ -42,9 +47,9 @@
 Read and query json file
     ${file}    Read Json File    sample.json
     ${result}   Query Json    ${file}    friends[?id>`1`]    #jmespath syntax
 
 ```
 
 ## Documentation
--   [Keyword Documentation](https://github.com/otemek/robotframework-jsonquery/doc/JsonQuery.html)
+-   [Keyword Documentation](https://otemek.github.io/robotframework-jsonquery/JsonQuery.html)
```

