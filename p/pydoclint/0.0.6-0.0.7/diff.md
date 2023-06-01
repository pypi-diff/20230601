# Comparing `tmp/pydoclint-0.0.6.tar.gz` & `tmp/pydoclint-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.6.tar", last modified: Thu Jun  1 02:59:35 2023, max compression
+gzip compressed data, was "pydoclint-0.0.7.tar", last modified: Thu Jun  1 10:42:17 2023, max compression
```

## Comparing `pydoclint-0.0.6.tar` & `pydoclint-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.359399 pydoclint-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-01 02:59:22.000000 pydoclint-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-06-01 02:59:35.359399 pydoclint-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-01 02:59:22.000000 pydoclint-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.355399 pydoclint-0.0.6/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.355399 pydoclint-0.0.6/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.355399 pydoclint-0.0.6/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 02:59:35.000000 pydoclint-0.0.6/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-01 02:59:22.000000 pydoclint-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-01 02:59:35.359399 pydoclint-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 02:59:22.000000 pydoclint-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:59:35.359399 pydoclint-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25662 2023-06-01 02:59:22.000000 pydoclint-0.0.6/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-01 02:59:22.000000 pydoclint-0.0.6/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-01 10:42:07.000000 pydoclint-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-01 10:42:17.178283 pydoclint-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-06-01 10:42:07.000000 pydoclint-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-01 10:42:17.178283 pydoclint-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 10:42:07.000000 pydoclint-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-06-01 10:42:07.000000 pydoclint-0.0.7/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-01 10:42:07.000000 pydoclint-0.0.7/tests/test_parse_config.py
```

### Comparing `pydoclint-0.0.6/LICENSE` & `pydoclint-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/PKG-INFO` & `pydoclint-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.6
+Version: 0.0.7
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -139,15 +139,15 @@
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
 | Code     | Explanation                                                                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
-| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint/#notes-on-doc103) |
+| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
 | `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
 | `DOC105` | Argument names match, but type hints do not match                                                                                                    |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
```

### Comparing `pydoclint-0.0.6/README.md` & `pydoclint-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
 | Code     | Explanation                                                                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
-| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint/#notes-on-doc103) |
+| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
 | `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
 | `DOC105` | Argument names match, but type hints do not match                                                                                                    |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
```

### Comparing `pydoclint-0.0.6/pydoclint/flake8_entry.py` & `pydoclint-0.0.7/pydoclint/flake8_entry.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/main.py` & `pydoclint-0.0.7/pydoclint/main.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/parse_config.py` & `pydoclint-0.0.7/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/utils/annotation.py` & `pydoclint-0.0.7/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/utils/arg.py` & `pydoclint-0.0.7/pydoclint/utils/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/utils/doc.py` & `pydoclint-0.0.7/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/utils/generic.py` & `pydoclint-0.0.7/pydoclint/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.0.7/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/utils/unparser.py` & `pydoclint-0.0.7/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/utils/violation.py` & `pydoclint-0.0.7/pydoclint/utils/violation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/utils/walk.py` & `pydoclint-0.0.7/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint/visitor.py` & `pydoclint-0.0.7/pydoclint/visitor.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.0.7/pydoclint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.6
+Version: 0.0.7
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -139,15 +139,15 @@
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
 | Code     | Explanation                                                                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
-| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint/#notes-on-doc103) |
+| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
 | `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
 | `DOC105` | Argument names match, but type hints do not match                                                                                                    |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
```

### Comparing `pydoclint-0.0.6/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.0.7/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.6/setup.cfg` & `pydoclint-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.0.6
+version = 0.0.7
 description = A linter to check arguments in Python docstrings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.0.6/tests/test_main.py` & `pydoclint-0.0.7/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,154 +12,154 @@
 
 
 expectedViolations_True_True = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
     'the docstring: [arg2: float | int | None].',
     'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC104: Method `MyClass.func4`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
     'match ',
     'DOC104: Method `MyClass.func6`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
     'match ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolations_False_True = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
     'the docstring: [arg2: float | int | None].',
     'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC104: Method `MyClass.func4`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC104: Method `MyClass.func6`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolations_True_False = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
     'the docstring: [arg2: float | int | None].',
     'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
     'match ',
     'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
     'match ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolations_False_False = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
     'the docstring: [arg2: float | int | None].',
     'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolationsLookup: Dict[str, List[str]] = {
     'true_true': expectedViolations_True_True,
     'true_false': expectedViolations_True_False,
     'false_true': expectedViolations_False_True,
@@ -236,15 +236,15 @@
         'docstring ',
         'DOC201: Method `MyClass.func1_6` does not have a return section in '
         'docstring ',
         'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
         'function signature. ',
         'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
         'function arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
         'the docstring: [arg2: float, arg3: str]. Arguments in the docstring but not '
         'in the function signature: [arg1: int].',
         'DOC201: Function `func52` does not have a return section in docstring ',
         'DOC202: Method `MyClass.func6` has a return section in docstring, but there '
         'are no return statements or annotations ',
     ]
 
@@ -263,40 +263,40 @@
 
 
 expected_True = [
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
     'the function signature: [var1: int, var2: str].',
     'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
 expected_False = [
     'DOC101: Function `func1`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func1`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func1` does not have a return section in docstring ',
     'DOC101: Function `func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func2`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func2` does not have a return section in docstring ',
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
     'the function signature: [var1: int, var2: str].',
     'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
 
 @pytest.mark.parametrize(
@@ -337,15 +337,15 @@
         'because __init__() cannot return anything ',
         'DOC105: Method `C.__init__`: Argument names match, but type hints do not '
         'match ',
         'DOC302: Class `C`: The class docstring does not need a "Returns" section, '
         'because __init__() cannot return anything ',
         'DOC103: Method `D.__init__`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
         'docstring: [arg1: int, arg2: float]. Arguments in the docstring but not in '
         'the function signature: [var1: list, var2: dict].',
         'DOC302: Class `D`: The class docstring does not need a "Returns" section, '
         'because __init__() cannot return anything ',
     ]
     assert list(map(str, violations)) == expected
 
@@ -435,33 +435,33 @@
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/star_args/cases.py',
         style=style,
     )
     expected = [
         'DOC103: Function `func2`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
         'docstring: [**kwargs: ]. Arguments in the docstring but not in the function '
         'signature: [kwargs: ].',
         'DOC103: Function `func4`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
         'docstring: [*args: ]. Arguments in the docstring but not in the function '
         'signature: [args: ].',
         'DOC101: Function `func6`: Docstring contains fewer arguments than in '
         'function signature. ',
         'DOC103: Function `func6`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
         'docstring: [**kwargs: , *args: ].',
         'DOC101: Function `func7`: Docstring contains fewer arguments than in '
         'function signature. ',
         'DOC103: Function `func7`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint/#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
         'docstring: [**kwargs: , *args: , arg1: float, arg2: str]. Arguments in the '
         'docstring but not in the function signature: [arg1: int, arg2: dict].',
     ]
     assert list(map(str, violations)) == expected
 
 
 def testParsingErrors_google() -> None:
```

### Comparing `pydoclint-0.0.6/tests/test_parse_config.py` & `pydoclint-0.0.7/tests/test_parse_config.py`

 * *Files identical despite different names*

