# Comparing `tmp/algoseek-connector-1.0.1.tar.gz` & `tmp/algoseek-connector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/algoseek-connector-1.0.1.tar", last modified: Wed Jun  8 15:04:45 2022, max compression
+gzip compressed data, was "dist/algoseek-connector-1.0.2.tar", last modified: Thu Jun  1 07:28:20 2023, max compression
```

## Comparing `algoseek-connector-1.0.1.tar` & `algoseek-connector-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 taras     (1000) taras     (1000)        0 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/
--rw-rw-r--   0 taras     (1000) taras     (1000)     5890 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/PKG-INFO
--rw-rw-r--   0 taras     (1000) taras     (1000)     3500 2022-06-08 14:50:29.000000 algoseek-connector-1.0.1/README.md
-drwxrwxr-x   0 taras     (1000) taras     (1000)        0 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/algoseek_connector/
--rw-rw-r--   0 taras     (1000) taras     (1000)      430 2022-06-02 09:42:52.000000 algoseek-connector-1.0.1/algoseek_connector/__init__.py
--rw-rw-r--   0 taras     (1000) taras     (1000)      272 2022-06-08 15:03:02.000000 algoseek-connector-1.0.1/algoseek_connector/__version__.py
--rw-rw-r--   0 taras     (1000) taras     (1000)    13607 2022-06-08 14:48:40.000000 algoseek-connector-1.0.1/algoseek_connector/expressions.py
--rw-rw-r--   0 taras     (1000) taras     (1000)     2210 2022-06-07 15:25:44.000000 algoseek-connector-1.0.1/algoseek_connector/functions.py
--rw-rw-r--   0 taras     (1000) taras     (1000)     3316 2022-06-07 09:08:55.000000 algoseek-connector-1.0.1/algoseek_connector/operators.py
--rw-rw-r--   0 taras     (1000) taras     (1000)    13337 2022-06-07 12:54:15.000000 algoseek-connector-1.0.1/algoseek_connector/resources.py
--rw-rw-r--   0 taras     (1000) taras     (1000)     1887 2022-06-06 13:11:15.000000 algoseek-connector-1.0.1/algoseek_connector/sessions.py
-drwxrwxr-x   0 taras     (1000) taras     (1000)        0 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/algoseek_connector.egg-info/
--rw-rw-r--   0 taras     (1000) taras     (1000)     5890 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/algoseek_connector.egg-info/PKG-INFO
--rw-rw-r--   0 taras     (1000) taras     (1000)      494 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/algoseek_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 taras     (1000) taras     (1000)        1 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/algoseek_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 taras     (1000) taras     (1000)        1 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/algoseek_connector.egg-info/not-zip-safe
--rw-rw-r--   0 taras     (1000) taras     (1000)       25 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/algoseek_connector.egg-info/requires.txt
--rw-rw-r--   0 taras     (1000) taras     (1000)       19 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/algoseek_connector.egg-info/top_level.txt
--rw-rw-r--   0 taras     (1000) taras     (1000)       38 2022-06-08 15:04:45.000000 algoseek-connector-1.0.1/setup.cfg
--rw-rw-r--   0 taras     (1000) taras     (1000)     1844 2022-06-08 15:00:04.000000 algoseek-connector-1.0.1/setup.py
+drwxrwxr-x   0 taras     (1000) taras     (1000)        0 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/
+-rw-rw-r--   0 taras     (1000) taras     (1000)     5900 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/PKG-INFO
+-rw-rw-r--   0 taras     (1000) taras     (1000)     3510 2023-06-01 07:08:05.000000 algoseek-connector-1.0.2/README.md
+drwxrwxr-x   0 taras     (1000) taras     (1000)        0 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/algoseek_connector/
+-rw-rw-r--   0 taras     (1000) taras     (1000)      430 2023-06-01 07:07:38.000000 algoseek-connector-1.0.2/algoseek_connector/__init__.py
+-rw-rw-r--   0 taras     (1000) taras     (1000)      272 2023-06-01 07:07:38.000000 algoseek-connector-1.0.2/algoseek_connector/__version__.py
+-rw-rw-r--   0 taras     (1000) taras     (1000)    13539 2023-06-01 07:07:38.000000 algoseek-connector-1.0.2/algoseek_connector/expressions.py
+-rw-rw-r--   0 taras     (1000) taras     (1000)     2123 2023-06-01 07:07:38.000000 algoseek-connector-1.0.2/algoseek_connector/functions.py
+-rw-rw-r--   0 taras     (1000) taras     (1000)     3316 2023-06-01 07:07:38.000000 algoseek-connector-1.0.2/algoseek_connector/operators.py
+-rw-rw-r--   0 taras     (1000) taras     (1000)    13337 2023-06-01 07:07:38.000000 algoseek-connector-1.0.2/algoseek_connector/resources.py
+-rw-rw-r--   0 taras     (1000) taras     (1000)     1887 2023-06-01 07:07:38.000000 algoseek-connector-1.0.2/algoseek_connector/sessions.py
+drwxrwxr-x   0 taras     (1000) taras     (1000)        0 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/algoseek_connector.egg-info/
+-rw-rw-r--   0 taras     (1000) taras     (1000)     5900 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/algoseek_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 taras     (1000) taras     (1000)      494 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/algoseek_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 taras     (1000) taras     (1000)        1 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/algoseek_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 taras     (1000) taras     (1000)        1 2023-06-01 07:10:48.000000 algoseek-connector-1.0.2/algoseek_connector.egg-info/not-zip-safe
+-rw-rw-r--   0 taras     (1000) taras     (1000)       25 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/algoseek_connector.egg-info/requires.txt
+-rw-rw-r--   0 taras     (1000) taras     (1000)       19 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/algoseek_connector.egg-info/top_level.txt
+-rw-rw-r--   0 taras     (1000) taras     (1000)       38 2023-06-01 07:28:20.000000 algoseek-connector-1.0.2/setup.cfg
+-rw-rw-r--   0 taras     (1000) taras     (1000)     1844 2023-06-01 07:24:52.000000 algoseek-connector-1.0.2/setup.py
```

### Comparing `algoseek-connector-1.0.1/PKG-INFO` & `algoseek-connector-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algoseek-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper library for ORM-like SQL builder and executor
 Home-page: UNKNOWN
 Author: Taras Kuzyo
 Author-email: taras@algoseek.com
 License: UNKNOWN
 Description: # algoseek-connector
         
@@ -12,15 +12,15 @@
         The library provides a simple pythonic interface to algoseek datasets with custom data filtering/selection.
         
         ## Installing and Supported Versions
         
         algoseek-connector is available on PyPI:
         
         ```
-        $ python -m pip install requests
+        $ python -m pip install algoseek-connector
         ```
         
         or alternatively
         
         ```
         $ pip install algoseek-connector
         ```
```

### Comparing `algoseek-connector-1.0.1/README.md` & `algoseek-connector-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 The library provides a simple pythonic interface to algoseek datasets with custom data filtering/selection.
 
 ## Installing and Supported Versions
 
 algoseek-connector is available on PyPI:
 
 ```
-$ python -m pip install requests
+$ python -m pip install algoseek-connector
 ```
 
 or alternatively
 
 ```
 $ pip install algoseek-connector
 ```
```

### Comparing `algoseek-connector-1.0.1/algoseek_connector/expressions.py` & `algoseek-connector-1.0.2/algoseek_connector/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import copy
 import datetime
 from typing import List, Any, Union, Iterable, Optional
+from typing import TYPE_CHECKING
 
 from . import operators as op
-from . import functions as fn
+
+if TYPE_CHECKING:
+    from . import functions as fn
 
 
 class BaseExpression(object):
 
     def __init__(
             self,
             body: Any,
@@ -261,24 +264,22 @@
 
     def like(self, other: str) -> 'BooleanExpression':
         return BooleanExpression(op.Like(), self, Literal.wrap_constant(other))
 
     def ilike(self, other: str) -> 'BooleanExpression':
         return BooleanExpression(op.Ilike(), self, Literal.wrap_constant(other))
 
-    # TODO failing test extra parents
     def between(self, beg: Any, end: Any) -> 'BooleanExpression':
         other = Literal.wrap_constant(beg) & Literal.wrap_constant(end)
         return BooleanExpression(op.Between(), self, other)
 
-    def apply(self, func: Union[str, fn.Function], *args) -> 'FuncExpression':
-        if isinstance(func, str):
-            return FuncExpression(fn.Function(func), [self] + list(args))
-        else:
-            return FuncExpression(func, [self] + list(args))
+    def apply(self, func: 'fn.Function', *args) -> 'FuncExpression':
+        # if isinstance(func, str):
+        #     func = Function(func)
+        return func(self, *args)
 
 
 class Expression(BaseExpression):
     def __init__(
             self,
             operation: op.Operation,
             operands: List[BaseExpression],
@@ -376,15 +377,15 @@
         return f"{self.op.symbol}{operand_str}"
 
 
 class FuncExpression(Expression):
 
     def __init__(
             self,
-            function: fn.Function,
+            function: 'fn.Function',
             operand: List[BaseExpression],
             parent: Optional[Any] = None,
             alias_name: str = None,
             cast_dtype: str = None
             ):
         self.fn, self.operand = function, operand
         super().__init__(function, operand, parent, alias_name, cast_dtype)
```

### Comparing `algoseek-connector-1.0.1/algoseek_connector/functions.py` & `algoseek-connector-1.0.2/algoseek_connector/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-from typing import TYPE_CHECKING
-
 from .operators import Operation
-
-if TYPE_CHECKING:
-    from .expressions import BaseExpression, FuncExpression
+from .expressions import BaseExpression, FuncExpression, Literal
 
 
 class Function(Operation):
     """
     """
 
     precedence = 90
 
     def __init__(self, name: str):
         self.name = name
         self.symbol = name
 
     def __call__(self, x: 'BaseExpression', *args, **kwargs) -> 'FuncExpression':
-        # TODO: cannot apply a function to a constant
         # TODO: cannot apply a function to column by its string name
-        # if not isinstance(x, BaseException):
-        #     x = Literal.wrap_constant(x)
-        return x.apply(self, *args)
+        if not isinstance(x, BaseExpression):
+            x = Literal.wrap_constant(x)
+        return FuncExpression(self, [x] + list(args))
 
 
 class AggregateFunction(Function):
     pass
 
 
 distinct = Function('distinct')
```

### Comparing `algoseek-connector-1.0.1/algoseek_connector/operators.py` & `algoseek-connector-1.0.2/algoseek_connector/operators.py`

 * *Files identical despite different names*

### Comparing `algoseek-connector-1.0.1/algoseek_connector/resources.py` & `algoseek-connector-1.0.2/algoseek_connector/resources.py`

 * *Files identical despite different names*

### Comparing `algoseek-connector-1.0.1/algoseek_connector/sessions.py` & `algoseek-connector-1.0.2/algoseek_connector/sessions.py`

 * *Files identical despite different names*

### Comparing `algoseek-connector-1.0.1/algoseek_connector.egg-info/PKG-INFO` & `algoseek-connector-1.0.2/algoseek_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algoseek-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper library for ORM-like SQL builder and executor
 Home-page: UNKNOWN
 Author: Taras Kuzyo
 Author-email: taras@algoseek.com
 License: UNKNOWN
 Description: # algoseek-connector
         
@@ -12,15 +12,15 @@
         The library provides a simple pythonic interface to algoseek datasets with custom data filtering/selection.
         
         ## Installing and Supported Versions
         
         algoseek-connector is available on PyPI:
         
         ```
-        $ python -m pip install requests
+        $ python -m pip install algoseek-connector
         ```
         
         or alternatively
         
         ```
         $ pip install algoseek-connector
         ```
```

### Comparing `algoseek-connector-1.0.1/setup.py` & `algoseek-connector-1.0.2/setup.py`

 * *Files identical despite different names*

