# Comparing `tmp/metayaml-ng-1.0.tar.gz` & `tmp/metayaml-ng-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metayaml-ng-1.0.tar", last modified: Wed Apr 26 17:37:37 2023, max compression
+gzip compressed data, was "metayaml-ng-1.1.tar", last modified: Thu Jun  1 14:41:52 2023, max compression
```

## Comparing `metayaml-ng-1.0.tar` & `metayaml-ng-1.1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:37:37.763980 metayaml-ng-1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:37:37.755979 metayaml-ng-1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:37:37.763980 metayaml-ng-1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-26 17:37:25.000000 metayaml-ng-1.0/.github/workflows/ci-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-26 17:37:37.763980 metayaml-ng-1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7910 2023-04-26 17:37:25.000000 metayaml-ng-1.0/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-04-26 17:37:25.000000 metayaml-ng-1.0/bitbucket-pipelines.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:37:37.763980 metayaml-ng-1.0/metayaml/
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-04-26 17:37:25.000000 metayaml-ng-1.0/metayaml/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-04-26 17:37:25.000000 metayaml-ng-1.0/metayaml/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2430 2023-04-26 17:37:25.000000 metayaml-ng-1.0/metayaml/jinja_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12179 2023-04-26 17:37:25.000000 metayaml-ng-1.0/metayaml/metayaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:37:37.763980 metayaml-ng-1.0/metayaml_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-26 17:37:37.000000 metayaml-ng-1.0/metayaml_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 17:37:37.000000 metayaml-ng-1.0/metayaml_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:37:37.000000 metayaml-ng-1.0/metayaml_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 17:37:37.000000 metayaml-ng-1.0/metayaml_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 17:37:37.000000 metayaml-ng-1.0/metayaml_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 17:37:25.000000 metayaml-ng-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 17:37:25.000000 metayaml-ng-1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 17:37:37.763980 metayaml-ng-1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:37:37.763980 metayaml-ng-1.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4575 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:37:37.763980 metayaml-ng-1.0/tests/test_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/cp.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/dict_update.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/f1.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/f2.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/f3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/inherit.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/inherit_deepcp.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/inherit_subst.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/test.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/test_list.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/test_multi.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/test_order.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/undef.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tests/test_files/undef2.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-26 17:37:25.000000 metayaml-ng-1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.185858 metayaml-ng-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.173858 metayaml-ng-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.177857 metayaml-ng-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-01 14:41:42.000000 metayaml-ng-1.1/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-01 14:41:42.000000 metayaml-ng-1.1/.github/workflows/sync.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-06-01 14:41:42.000000 metayaml-ng-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-01 14:41:52.185858 metayaml-ng-1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7910 2023-06-01 14:41:42.000000 metayaml-ng-1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.177857 metayaml-ng-1.1/metayaml/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-01 14:41:42.000000 metayaml-ng-1.1/metayaml/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-06-01 14:41:42.000000 metayaml-ng-1.1/metayaml/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2402 2023-06-01 14:41:42.000000 metayaml-ng-1.1/metayaml/jinja_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12482 2023-06-01 14:41:42.000000 metayaml-ng-1.1/metayaml/metayaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.181858 metayaml-ng-1.1/metayaml_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 14:41:52.000000 metayaml-ng-1.1/metayaml_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 14:41:42.000000 metayaml-ng-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 14:41:42.000000 metayaml-ng-1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-01 14:41:52.185858 metayaml-ng-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.181858 metayaml-ng-1.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5031 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:52.185858 metayaml-ng-1.1/tests/test_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/cp.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/dict_update.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/f1.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/f2.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/f3.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/foo_data.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/inherit.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/inherit_deepcp.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/inherit_subst.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      133 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/list_eval.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/test.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/test_multi.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/test_order.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/undef.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tests/test_files/undef2.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-06-01 14:41:42.000000 metayaml-ng-1.1/tox.ini
```

### Comparing `metayaml-ng-1.0/.github/workflows/ci-cd.yml` & `metayaml-ng-1.1/.github/workflows/ci-cd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 name: CI
 
 on:
   push:
-    branches: ["main"]
+    branches: ["master"]
   pull_request:
-    branches: ["main"]
+    branches: ["master"]
   release:
     types: [created]
     branches:
-      - 'main'
+      - 'master'
   workflow_dispatch:
 
 env:
   FORCE_COLOR: "1"  # Make tools pretty.
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_PYTHON_VERSION_WARNING: "1"
   PYTHON_LATEST: "3.11"
```

### Comparing `metayaml-ng-1.0/PKG-INFO` & `metayaml-ng-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metayaml-ng
-Version: 1.0
+Version: 1.1
 Summary: Enhancements of yaml format to support include and python expression
 Download-URL: https://pypi.org/project/metayaml-ng/
 Author: Anton Tagunov
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metayaml-ng-1.0/README.rst` & `metayaml-ng-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.0/metayaml/exception.py` & `metayaml-ng-1.1/metayaml/exception.py`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.0/metayaml/jinja_eval.py` & `metayaml-ng-1.1/metayaml/jinja_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import jinja2
+from jinja2.compiler import CodeGenerator as _CodeGenerator, Frame
 from jinja2 import nodes
-from jinja2.compiler import CodeGenerator as _CodeGenerator
-from jinja2.compiler import Frame
-
 from metayaml.exception import MetaYamlExceptionPath
 
 
 class CodeGenerator(_CodeGenerator):
     def _output_child_pre(self, node: nodes.Expr, frame: Frame, finalize) -> None:
         """Output extra source code before visiting a child of an
         ``Output`` node.
```

### Comparing `metayaml-ng-1.0/metayaml/metayaml.py` & `metayaml-ng-1.1/metayaml/metayaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
+import yaml
 import datetime
 import typing as tp
+from copy import deepcopy
 from collections import defaultdict
 from collections.abc import Iterable, MutableMapping
 from copy import deepcopy
 from glob import glob
-
-import yaml
-
-from metayaml.exception import FileNotFound, MetaYamlException, MetaYamlExceptionPath
+from collections.abc import MutableMapping, Iterable
+from metayaml.exception import MetaYamlException, FileNotFound, MetaYamlExceptionPath
 
 Path = tp.Tuple
 
 
 def _path(path: Path, key: tp.Union[str, int], index=False):
     if not index:
         key = str(key)
@@ -236,16 +236,16 @@
                     added_values = source[self.EXTEND_MARKER]
                     if not isinstance(added_values, list):
                         raise MetaYamlExceptionPath(
                             f"expected list, but have got {type(added_values)}",
                             path + (self.EXTEND_MARKER,),
                             added_values,
                         )
-                    added_values = self.eval_value(
-                        added_values, path, global_data, True
+                    added_values, _ = self.eval_expression(
+                        added_values, global_data, path, True
                     )
                     dest.extend(added_values)
                     return dest
                 else:
                     raise MetaYamlExceptionPath(
                         f"dict can't be merged to {type(dest)}", path, source
                     )
@@ -275,51 +275,56 @@
 
         brackets = self.eager_brackets if eager else self.lazy_brackets
         if brackets[0] not in val:
             return val
 
         return jinja_eval_value(self, val, path, global_data, eager, brackets)
 
-    def process_lazy(self, data, global_data, path: Path) -> tp.Tuple[tp.Any, bool]:
+    def eval_expression(
+        self, data, global_data, path: Path, eager: bool
+    ) -> tp.Tuple[tp.Any, bool]:
         # the first item in result is evaluated value
         # the second item is true when value was substituted
         if isinstance(data, (float, int, bool)):
             return data, False
 
         if isinstance(data, str):
-            evaluated_value = self.eval_value(data, path, global_data, False)
+            evaluated_value = self.eval_value(data, path, global_data, eager)
             return evaluated_value, evaluated_value != data
 
         substituted = False
         if isinstance(data, dict):
             for key, value in list(data.items()):
                 evaluated_key = self.eval_value(
                     key, _path(path, key), global_data, False
                 )
-                evaluated_value, changed = self.process_lazy(
-                    value, global_data, _path(path, key)
+                evaluated_value, changed = self.eval_expression(
+                    value, global_data, _path(path, key), eager=eager
                 )
                 substituted |= changed
                 if key != evaluated_key:
                     data.pop(key)
                     substituted = True
                 data[evaluated_key] = evaluated_value
             return data, substituted
 
         if isinstance(data, list):
             for index, value in enumerate(data):
-                evaluated_value, changed = self.process_lazy(
-                    value, global_data, _path(path, index, index=True)
+                evaluated_value, changed = self.eval_expression(
+                    value, global_data, _path(path, index, index=True), eager
                 )
                 if changed:
-                    data[index] = changed
+                    data[index] = evaluated_value
                     substituted = True
             return data, substituted
         return data, False
 
+    def process_lazy(self, data, global_data, path: Path) -> tp.Tuple[tp.Any, bool]:
+        return self.eval_expression(data, global_data, path, False)
+
 
 def read(
     yaml_file,
     defaults=None,
     extend_key_word="extend",
     ignore_errors=False,
     ignore_not_existed_files=False,
```

### Comparing `metayaml-ng-1.0/metayaml_ng.egg-info/PKG-INFO` & `metayaml-ng-1.1/metayaml_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metayaml-ng
-Version: 1.0
+Version: 1.1
 Summary: Enhancements of yaml format to support include and python expression
 Download-URL: https://pypi.org/project/metayaml-ng/
 Author: Anton Tagunov
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metayaml-ng-1.0/metayaml_ng.egg-info/SOURCES.txt` & `metayaml-ng-1.1/metayaml_ng.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+.gitignore
 README.rst
-bitbucket-pipelines.yml
 pyproject.toml
 requirements-dev.txt
 setup.cfg
 tox.ini
 .github/workflows/ci-cd.yml
+.github/workflows/sync.yml
 metayaml/__init__.py
 metayaml/exception.py
 metayaml/jinja_eval.py
 metayaml/metayaml.py
 metayaml_ng.egg-info/PKG-INFO
 metayaml_ng.egg-info/SOURCES.txt
 metayaml_ng.egg-info/dependency_links.txt
@@ -17,16 +18,17 @@
 tests/__init__.py
 tests/test.py
 tests/test_files/cp.yaml
 tests/test_files/dict_update.yaml
 tests/test_files/f1.yaml
 tests/test_files/f2.yaml
 tests/test_files/f3.yaml
+tests/test_files/foo_data.yaml
 tests/test_files/inherit.yaml
 tests/test_files/inherit_deepcp.yaml
 tests/test_files/inherit_subst.yaml
+tests/test_files/list_eval.yaml
 tests/test_files/test.yaml
-tests/test_files/test_list.yaml
 tests/test_files/test_multi.yaml
 tests/test_files/test_order.yaml
 tests/test_files/undef.yaml
 tests/test_files/undef2.yaml
```

### Comparing `metayaml-ng-1.0/setup.cfg` & `metayaml-ng-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `metayaml-ng-1.0/tests/test.py` & `metayaml-ng-1.1/tests/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,10 +115,26 @@
             'b': {'a': 2, 'aa': 1, 'b': 2, 'bb': 6},
             'bar': 6,
             'foo': {'a': 2, 'b': 2}
         }
 
         self.assertEqual(d, expected)
 
+    def test_list_extend(self):
+        d = read(self._file_name("list_eval.yaml"))
+        expected = {
+            "foo1": "bar1",
+            "foo2": "bar2",
+            "hour": 3600,
+            "zz": 60 * 60 * 5,
+            "data": [
+                {"a2": "2bar2"},
+                {"a": "1bar1"},
+                {"b": "yy"},
+                {"c": 60 * 60 * 5},
+                "dbar1"
+            ]
+        }
+        self.assertEqual(d, expected)
 
 if __name__ == '__main__':
     main()
```

