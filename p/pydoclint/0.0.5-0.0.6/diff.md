# Comparing `tmp/pydoclint-0.0.5.tar.gz` & `tmp/pydoclint-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.5.tar", last modified: Wed May 31 10:43:11 2023, max compression
+gzip compressed data, was "pydoclint-0.0.6.tar", last modified: Thu Jun  1 02:59:35 2023, max compression
```

## Comparing `pydoclint-0.0.5.tar` & `pydoclint-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.884906 pydoclint-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-31 10:42:55.000000 pydoclint-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-31 10:43:11.884906 pydoclint-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-31 10:42:55.000000 pydoclint-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.880906 pydoclint-0.0.5/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.884906 pydoclint-0.0.5/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.880906 pydoclint-0.0.5/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-31 10:43:11.884906 pydoclint-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 10:42:55.000000 pydoclint-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.884906 pydoclint-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25662 2023-05-31 10:42:55.000000 pydoclint-0.0.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-31 10:42:55.000000 pydoclint-0.0.5/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.359399 pydoclint-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-01 02:59:22.000000 pydoclint-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-06-01 02:59:35.359399 pydoclint-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-01 02:59:22.000000 pydoclint-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.355399 pydoclint-0.0.6/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.355399 pydoclint-0.0.6/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.355399 pydoclint-0.0.6/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-01 02:59:35.359399 pydoclint-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 02:59:22.000000 pydoclint-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.359399 pydoclint-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25662 2023-06-01 02:59:22.000000 pydoclint-0.0.6/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-01 02:59:22.000000 pydoclint-0.0.6/tests/test_parse_config.py
```

### Comparing `pydoclint-0.0.5/LICENSE` & `pydoclint-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/PKG-INFO` & `pydoclint-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.5
+Version: 0.0.6
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `pydoclint-0.0.5/README.md` & `pydoclint-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/flake8_entry.py` & `pydoclint-0.0.6/pydoclint/flake8_entry.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/main.py` & `pydoclint-0.0.6/pydoclint/main.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/parse_config.py` & `pydoclint-0.0.6/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/utils/annotation.py` & `pydoclint-0.0.6/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/utils/arg.py` & `pydoclint-0.0.6/pydoclint/utils/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/utils/doc.py` & `pydoclint-0.0.6/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/utils/generic.py` & `pydoclint-0.0.6/pydoclint/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.0.6/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/utils/unparser.py` & `pydoclint-0.0.6/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/utils/violation.py` & `pydoclint-0.0.6/pydoclint/utils/violation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 VIOLATION_CODES = types.MappingProxyType({
     1: 'Potential formatting errors in docstring. Error message:',
 
     101: 'Docstring contains fewer arguments than in function signature.',
     102: 'Docstring contains more arguments than in function signature.',
     103: (  # noqa: PAR001
         'Docstring arguments are different from function arguments.'
-        ' (Or could be other formatting issues: https://github.com/jsh9/pydoclint/#notes-on-doc103).'
+        ' (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103).'
     ),
     104: 'Arguments are the same in the docstring and the function signature, but are in a different order.',
     105: 'Argument names match, but type hints do not match',
 
     201: 'does not have a return section in docstring',
     202: 'has a return section in docstring, but there are no return statements or annotations',
```

### Comparing `pydoclint-0.0.5/pydoclint/utils/walk.py` & `pydoclint-0.0.6/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint/visitor.py` & `pydoclint-0.0.6/pydoclint/visitor.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.0.6/pydoclint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.5
+Version: 0.0.6
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `pydoclint-0.0.5/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.0.6/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/setup.cfg` & `pydoclint-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.0.5
+version = 0.0.6
 description = A linter to check arguments in Python docstrings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.0.5/tests/test_main.py` & `pydoclint-0.0.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.5/tests/test_parse_config.py` & `pydoclint-0.0.6/tests/test_parse_config.py`

 * *Files identical despite different names*

