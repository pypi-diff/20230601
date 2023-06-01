# Comparing `tmp/sqlsynthgen-0.1.0.tar.gz` & `tmp/sqlsynthgen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsynthgen-0.1.0.tar", max compression
+gzip compressed data, was "sqlsynthgen-0.2.0.tar", max compression
```

## Comparing `sqlsynthgen-0.1.0.tar` & `sqlsynthgen-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1082 2023-04-15 12:58:52.957433 sqlsynthgen-0.1.0/LICENSE
--rw-r--r--   0        0        0      247 2023-04-25 13:14:57.094359 sqlsynthgen-0.1.0/README.md
--rw-r--r--   0        0        0     1170 2023-06-01 07:08:13.086110 sqlsynthgen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-15 12:58:52.958860 sqlsynthgen-0.1.0/sqlsynthgen/__init__.py
--rw-r--r--   0        0        0      637 2023-05-22 10:39:40.766223 sqlsynthgen-0.1.0/sqlsynthgen/base.py
--rw-r--r--   0        0        0     5411 2023-05-26 17:25:44.683072 sqlsynthgen-0.1.0/sqlsynthgen/create.py
--rw-r--r--   0        0        0     2946 2023-06-01 06:59:02.912570 sqlsynthgen-0.1.0/sqlsynthgen/json_schemas/config_schema.json
--rw-r--r--   0        0        0     7012 2023-06-01 06:59:02.912832 sqlsynthgen-0.1.0/sqlsynthgen/main.py
--rw-r--r--   0        0        0    14869 2023-05-22 10:39:40.766611 sqlsynthgen-0.1.0/sqlsynthgen/make.py
--rw-r--r--   0        0        0     3107 2023-05-22 10:39:40.766877 sqlsynthgen-0.1.0/sqlsynthgen/providers.py
--rw-r--r--   0        0        0     4632 2023-05-26 17:25:44.683720 sqlsynthgen-0.1.0/sqlsynthgen/settings.py
--rw-r--r--   0        0        0     5086 2023-05-22 13:29:50.224369 sqlsynthgen-0.1.0/sqlsynthgen/settings.py_
--rw-r--r--   0        0        0     2122 2023-05-26 17:25:44.684057 sqlsynthgen-0.1.0/sqlsynthgen/templates/ssg.py.j2
--rw-r--r--   0        0        0     2149 2023-05-15 16:15:28.771627 sqlsynthgen-0.1.0/sqlsynthgen/utils.py
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 sqlsynthgen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-01 16:18:08.329813 sqlsynthgen-0.2.0/LICENSE
+-rw-r--r--   0        0        0      247 2023-06-01 16:18:08.329813 sqlsynthgen-0.2.0/README.md
+-rw-r--r--   0        0        0     1170 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/__init__.py
+-rw-r--r--   0        0        0      637 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/base.py
+-rw-r--r--   0        0        0     5411 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/create.py
+-rw-r--r--   0        0        0     2946 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/json_schemas/config_schema.json
+-rw-r--r--   0        0        0     7012 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/main.py
+-rw-r--r--   0        0        0    14869 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/make.py
+-rw-r--r--   0        0        0     3107 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/providers.py
+-rw-r--r--   0        0        0     4632 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/settings.py
+-rw-r--r--   0        0        0     2122 2023-06-01 16:18:08.337813 sqlsynthgen-0.2.0/sqlsynthgen/templates/ssg.py.j2
+-rw-r--r--   0        0        0     2149 2023-06-01 16:18:08.337813 sqlsynthgen-0.2.0/sqlsynthgen/utils.py
+-rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 sqlsynthgen-0.2.0/PKG-INFO
```

### Comparing `sqlsynthgen-0.1.0/LICENSE` & `sqlsynthgen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/pyproject.toml` & `sqlsynthgen-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlsynthgen"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Iain <25081046+Iain-S@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
```

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/base.py` & `sqlsynthgen-0.2.0/sqlsynthgen/base.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/create.py` & `sqlsynthgen-0.2.0/sqlsynthgen/create.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/json_schemas/config_schema.json` & `sqlsynthgen-0.2.0/sqlsynthgen/json_schemas/config_schema.json`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/main.py` & `sqlsynthgen-0.2.0/sqlsynthgen/main.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/make.py` & `sqlsynthgen-0.2.0/sqlsynthgen/make.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/providers.py` & `sqlsynthgen-0.2.0/sqlsynthgen/providers.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/settings.py` & `sqlsynthgen-0.2.0/sqlsynthgen/settings.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/templates/ssg.py.j2` & `sqlsynthgen-0.2.0/sqlsynthgen/templates/ssg.py.j2`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/sqlsynthgen/utils.py` & `sqlsynthgen-0.2.0/sqlsynthgen/utils.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.1.0/PKG-INFO` & `sqlsynthgen-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsynthgen
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Iain
 Author-email: 25081046+Iain-S@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

