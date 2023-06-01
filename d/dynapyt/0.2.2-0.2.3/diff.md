# Comparing `tmp/dynapyt-0.2.2.tar.gz` & `tmp/dynapyt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynapyt-0.2.2.tar", last modified: Mon Jan 30 10:02:43 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dynapyt-0.2.2.tar` & `dynapyt-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,39 @@
--rw-r--r--   0        0        0     1096 2023-01-30 10:02:34.081324 dynapyt-0.2.2/LICENSE
--rw-r--r--   0        0        0     5660 2023-01-30 10:02:34.081324 dynapyt-0.2.2/README.md
--rw-r--r--   0        0        0      449 2023-01-30 10:02:34.081324 dynapyt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       36 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/__init__.py
--rw-r--r--   0        0        0      818 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/BaseAnalysis.py
--rw-r--r--   0        0        0      526 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/BranchCoverage.py
--rw-r--r--   0        0        0      866 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/CallGraph.py
--rw-r--r--   0        0        0      538 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/Demo.py
--rw-r--r--   0        0        0      208 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/EventAnalysis.py
--rw-r--r--   0        0        0      718 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/KeyInListAnalysis.py
--rw-r--r--   0        0        0      268 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/LiteralAnalysis.py
--rw-r--r--   0        0        0     1342 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/MLMemoryAnalysis.py
--rw-r--r--   0        0        0      397 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/ManipulateExec.py
--rw-r--r--   0        0        0      734 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/MemoryAccessAnalysis.py
--rw-r--r--   0        0        0      225 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/OnlyAddAnalysis.py
--rw-r--r--   0        0        0      317 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/OperationAnalysis.py
--rw-r--r--   0        0        0     2458 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/SimpleTaintAnalysis.py
--rw-r--r--   0        0        0     4499 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/SimpleTestAnalysis.py
--rw-r--r--   0        0        0    31638 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/TraceAll.py
--rw-r--r--   0        0        0      333 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/UnnecessaryDoubleDictQuery.py
--rw-r--r--   0        0        0        1 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/analyses/__init__.py
--rw-r--r--   0        0        0    47883 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/instrument/CodeInstrumenter.py
--rw-r--r--   0        0        0     1700 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/instrument/IIDs.py
--rw-r--r--   0        0        0        1 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/instrument/__init__.py
--rw-r--r--   0        0        0     3255 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/instrument/instrument.py
--rw-r--r--   0        0        0     1836 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/run_all.py
--rw-r--r--   0        0        0     1829 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/run_analysis.py
--rw-r--r--   0        0        0     1874 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/run_instrumentation.py
--rw-r--r--   0        0        0    16806 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/runtime.py
--rw-r--r--   0        0        0      540 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/utils/AnalysisUtils.py
--rw-r--r--   0        0        0        1 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/utils/__init__.py
--rw-r--r--   0        0        0     3393 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/utils/hierarchy.json
--rw-r--r--   0        0        0     1410 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/utils/hooks.py
--rw-r--r--   0        0        0     2335 2023-01-30 10:02:34.081324 dynapyt-0.2.2/src/dynapyt/utils/nodeLocator.py
--rw-r--r--   0        0        0     5968 1970-01-01 00:00:00.000000 dynapyt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/__init__.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/run_all.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/run_analysis.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/run_instrumentation.py
+-rw-r--r--   0        0        0    17428 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/runtime.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/BaseAnalysis.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/BranchCoverage.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/CallGraph.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/Demo.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/EventAnalysis.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/KeyInListAnalysis.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/LiteralAnalysis.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/MLMemoryAnalysis.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/ManipulateExec.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/MemoryAccessAnalysis.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/OnlyAddAnalysis.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/OperationAnalysis.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/SimpleTaintAnalysis.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/SimpleTestAnalysis.py
+-rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/TraceAll.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/UnnecessaryDoubleDictQuery.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/__init__.py
+-rw-r--r--   0        0        0    47883 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/instrument/CodeInstrumenter.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/instrument/IIDs.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/instrument/__init__.py
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/instrument/instrument.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/AnalysisUtils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/__init__.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/hierarchy.json
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/hooks.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/nodeLocator.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/nativetracer/__init__.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/nativetracer/instrument_tracer.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/nativetracer/trc.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 dynapyt-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dynapyt-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 dynapyt-0.2.3/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 dynapyt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 dynapyt-0.2.3/PKG-INFO
```

### Comparing `dynapyt-0.2.2/LICENSE` & `dynapyt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/README.md` & `dynapyt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/BaseAnalysis.py` & `dynapyt-0.2.3/src/dynapyt/analyses/BaseAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/BranchCoverage.py` & `dynapyt-0.2.3/src/dynapyt/analyses/BranchCoverage.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/Demo.py` & `dynapyt-0.2.3/src/dynapyt/analyses/Demo.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/KeyInListAnalysis.py` & `dynapyt-0.2.3/src/dynapyt/analyses/KeyInListAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/MLMemoryAnalysis.py` & `dynapyt-0.2.3/src/dynapyt/analyses/MLMemoryAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/MemoryAccessAnalysis.py` & `dynapyt-0.2.3/src/dynapyt/analyses/MemoryAccessAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/SimpleTaintAnalysis.py` & `dynapyt-0.2.3/src/dynapyt/analyses/SimpleTaintAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/SimpleTestAnalysis.py` & `dynapyt-0.2.3/src/dynapyt/analyses/SimpleTestAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/analyses/TraceAll.py` & `dynapyt-0.2.3/src/dynapyt/analyses/TraceAll.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,149 +2,149 @@
 from types import TracebackType
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 import libcst as cst
 import libcst.matchers as m
 from .BaseAnalysis import BaseAnalysis
 from ..utils.nodeLocator import get_node_by_location
 
+
 class TraceAll(BaseAnalysis):
-    
     def __init__(self) -> None:
         super().__init__()
         root_logger = logging.getLogger()
         root_logger.setLevel(logging.INFO)
-        handler = logging.FileHandler('output.log', 'w', 'utf-8')
-        handler.setFormatter(logging.Formatter('%(message)s'))
+        handler = logging.FileHandler("output.log", "w", "utf-8")
+        handler.setFormatter(logging.Formatter("%(message)s"))
         root_logger.addHandler(handler)
-    
+
     def log(self, iid: int, *args, **kwargs):
-        res = ''
+        res = ""
         # for arg in args:
         #     if 'danger_of_recursion' in kwargs:
         #         res += ' ' + str(hex(id(arg)))
         #     else:
         #         res += ' ' + str(arg)
-        logging.info(str(iid) + ': ' + res[:80])
+        logging.info(str(iid) + ": " + res[:80])
 
     # Literals
-    
+
     def integer(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for integer literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         val : Any
             The value of the integer literal.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the value of the integer literal.
         """
-        self.log(iid, '    Integer', 'value:', val)
-    
+        self.log(iid, "    Integer", "value:", val)
+
     def _float(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for floating point literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         val : Any
             The value of the floating point literal.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the value of the float literal.
         """
-        self.log(iid, '    Float', 'value:', val)
-    
+        self.log(iid, "    Float", "value:", val)
+
     def imaginary(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for imaginary number literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         val : Any
             The value of the imaginary number literal.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the value of the imaginary number literal.
         """
-        self.log(iid, '    Imaginary', 'value:', val)
-    
+        self.log(iid, "    Imaginary", "value:", val)
+
     def string(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for string literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         val : Any
             The value of the string literal.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the value of the string literal.
         """
-        self.log(iid, '    String', 'value:', val)
-    
+        self.log(iid, "    String", "value:", val)
+
     def boolean(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for boolean literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         val : Any
             The value of the boolean literal.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the value of the boolean literal.
         """
-        self.log(iid, '    Boolean', 'value:', val)
-    
+        self.log(iid, "    Boolean", "value:", val)
+
     def literal(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for all literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         val : Any
             The value of the literal.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the value of the literal.
         """
-        self.log(iid, 'Literal   ', 'value:', val)
-    
+        self.log(iid, "Literal   ", "value:", val)
+
     def dictionary(self, dyn_ast: str, iid: int, items: List[Any], value: Dict) -> Dict:
         """Hook for a dictionary definition.
         E.g. `{'a': 1, 'b': 2}`
         or `{i: i for i in range(10)}`
 
         Parameters
         ----------
@@ -152,43 +152,43 @@
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         items : List[Any]
             The lis of key-value pairs.
         value : Dict
             The dictionary itself.
-        
+
         Returns
         -------
         Dict
             If provided, overwrites the value of the dictionary.
         """
-        self.log(iid, 'Dictionary', 'items:', items)
-    
+        self.log(iid, "Dictionary", "items:", items)
+
     def _list(self, dyn_ast: str, iid: int, value: List) -> List:
         """Hook for a list definition.
         E.g. `[1, 2, 3]`
         or `[i for i in range(10)]`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         value : List
             The list itself.
-        
+
         Returns
         -------
         List
             If provided, overwrites the value of the list.
         """
-        self.log(iid, 'List', value)
-    
+        self.log(iid, "List", value)
+
     def _tuple(self, dyn_ast: str, iid: int, items: List[Any], value: tuple) -> tuple:
         """Hook for a tuple.
         E.g. `(1, 2, 3)`
         or `(i for i in range(10))`
 
         Parameters
         ----------
@@ -196,48 +196,52 @@
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         items : List[Any]
             The lis of items in the tuple.
         value : tuple
             The tuple itself.
-        
+
         Returns
         -------
         tuple
             If provided, overwrites the value of the tuple.
         """
-        self.log(iid, 'Tuple', 'items:', items)
-    
+        self.log(iid, "Tuple", "items:", items)
+
     # Operations
 
-    def operation(self, dyn_ast: str, iid: int, operator: str, operands: List[Any], result: Any) -> Any:
+    def operation(
+        self, dyn_ast: str, iid: int, operator: str, operands: List[Any], result: Any
+    ) -> Any:
         """Hook for any operation.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         operator : str
             The operator of the operation.
         operands : List[Any]
             The operands of the operation.
         result : Any
             The result of the operation.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the result of the operation.
         """
         pass
 
-    def binary_operation(self, dyn_ast: str, iid: int, op: str, left: Any, right: Any, result: Any) -> Any:
+    def binary_operation(
+        self, dyn_ast: str, iid: int, op: str, left: Any, right: Any, result: Any
+    ) -> Any:
         """Hook for any binary operation.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
@@ -246,103 +250,123 @@
             The operator of the operation.
         left : Any
             The left operand of the operation.
         right : Any
             The right operand of the operation.
         result : Any
             The result of the operation.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the result of the operation.
         """
-        self.log(iid, 'Binary Operation', left, op, right, '->', result)
-    
+        self.log(iid, "Binary Operation", left, op, right, "->", result)
+
     def add(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
-    def bit_and(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
+    def bit_and(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
     def bit_or(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
-    def bit_xor(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
+    def bit_xor(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
     def divide(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
-    def floor_divide(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
-    def left_shift(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
-    def right_shift(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
-    def matrix_multiply(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
+    def floor_divide(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
+    def left_shift(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
+    def right_shift(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
+    def matrix_multiply(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
     def modulo(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
-    def multiply(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
+    def multiply(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
     def power(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
-    def subtract(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
+    def subtract(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
     def _and(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
-    
+        self.log(iid, "Binary Operation", left, right, "->", result)
+
     def _or(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Binary Operation', left, right, '->', result)
+        self.log(iid, "Binary Operation", left, right, "->", result)
 
-    def unary_operation(self, dyn_ast: str, iid: int, opr: Any, arg: Any, result: Any) -> Any:
+    def unary_operation(
+        self, dyn_ast: str, iid: int, opr: Any, arg: Any, result: Any
+    ) -> Any:
         """Hook for any unary operation.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         opr : str
             The operator of the operation.
         arg : Any
             The operand of the operation.
         result : Any
             The result of the operation.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the result of the operation.
         """
-        self.log(iid, 'Unary Operation', arg, '->', result)
-    
+        self.log(iid, "Unary Operation", arg, "->", result)
+
     def bit_invert(self, dyn_ast: str, iid: int, arg: Any, result: Any) -> Any:
-        self.log(iid, 'Unary Operation', arg, '->', result)
-    
+        self.log(iid, "Unary Operation", arg, "->", result)
+
     def minus(self, dyn_ast: str, iid: int, arg: Any, result: Any) -> Any:
-        self.log(iid, 'Unary Operation', arg, '->', result)
+        self.log(iid, "Unary Operation", arg, "->", result)
 
     def _not(self, dyn_ast: str, iid: int, arg: Any, result: Any) -> Any:
-        self.log(iid, 'Unary Operation', arg, '->', result)
-    
+        self.log(iid, "Unary Operation", arg, "->", result)
+
     def plus(self, dyn_ast: str, iid: int, arg: Any, result: Any) -> Any:
-        self.log(iid, 'Unary Operation', arg, '->', result)
+        self.log(iid, "Unary Operation", arg, "->", result)
 
-    def comparison(self, dyn_ast: str, iid: int, op: str, left: Any, right: Any, result: Any) -> Any:
+    def comparison(
+        self, dyn_ast: str, iid: int, op: str, left: Any, right: Any, result: Any
+    ) -> Any:
         """Hook for the comparison operation.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
@@ -351,81 +375,92 @@
             The operator of the operation.
         left : Any
             The left operand of the operation.
         right : Any
             The right operand of the operation.
         result : Any
             The result of the operation.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the result of the operation.
         """
-        self.log(iid, 'Comparison', left, op, right, '->', result)
-    
+        self.log(iid, "Comparison", left, op, right, "->", result)
+
     def equal(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
-    
-    def greater_than(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
-    
-    def greater_than_equal(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
-    
-    def _in(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
-    
-    def _is(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
+        self.log(iid, "Comparison", left, right, "->", result)
 
-    def less_than(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
+    def greater_than(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Comparison", left, right, "->", result)
+
+    def greater_than_equal(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Comparison", left, right, "->", result)
 
-    def less_than_equal(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
+    def _in(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
+        self.log(iid, "Comparison", left, right, "->", result)
 
-    def not_equal(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
+    def _is(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
+        self.log(iid, "Comparison", left, right, "->", result)
+
+    def less_than(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Comparison", left, right, "->", result)
+
+    def less_than_equal(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Comparison", left, right, "->", result)
+
+    def not_equal(
+        self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any
+    ) -> Any:
+        self.log(iid, "Comparison", left, right, "->", result)
 
     def is_not(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
+        self.log(iid, "Comparison", left, right, "->", result)
 
     def not_in(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
-        self.log(iid, 'Comparison', left, right, '->', result)
-
+        self.log(iid, "Comparison", left, right, "->", result)
 
     # Memory access
 
     def memory_access(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for any memory access, currently, except some write operations.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         val : Any
             The value accessed.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
         """
-        self.log(iid, 'Accessing')
-    
+        self.log(iid, "Accessing")
+
     def read(self, dyn_ast: str, iid: int, val: Any) -> Any:
-        self.log(iid, ' Reading')
-    
+        self.log(iid, " Reading")
+
     def read_identifier(self, dyn_ast: str, iid: int, val: Any) -> Any:
-        self.log(iid, '    Reading')
+        self.log(iid, "    Reading")
 
-    def write(self, dyn_ast: str, iid: int, old_vals: List[Callable], new_val: Any) -> Any:
+    def write(
+        self, dyn_ast: str, iid: int, old_vals: List[Callable], new_val: Any
+    ) -> Any:
         """Hook for writes.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
@@ -433,42 +468,44 @@
         old_vals : Any
             A list of old values before the write takes effect.
             It's a list to support multiple assignments.
             Each old value is wrapped into a lambda function, so that
             the analysis writer can decide if and when to evaluate it.
         new_val : Any
             The value after the write takes effect.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
         """
-        self.log(iid, '    Writing')
+        self.log(iid, "    Writing")
 
     def delete(self, dyn_ast: str, iid: int, val: Any) -> Optional[bool]:
         """Hook for deletes.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         val : Any
             The value deleted.
-        
+
         Returns
         -------
         Any
             If True cancels the delete.
         """
-        self.log(iid, '    Deleting')
+        self.log(iid, "    Deleting")
 
-    def read_attribute(self, dyn_ast: str, iid: int, base: Any, name: str, val: Any) -> Any:
+    def read_attribute(
+        self, dyn_ast: str, iid: int, base: Any, name: str, val: Any
+    ) -> Any:
         """Hook for reading an object attribute.
         E.g. `obj.attr`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
@@ -476,23 +513,25 @@
             Unique ID of the syntax tree node.
         base : Any
             The object to which the attribute is attached.
         name : str
             The name of the attribute.
         val : Any
             The resulting value.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
         """
-        self.log(iid, 'Attribute', name)
-    
-    def read_subscript(self, dyn_ast: str, iid: int, base: Any, sl: List[Union[int, Tuple]], val: Any) -> Any:
+        self.log(iid, "Attribute", name)
+
+    def read_subscript(
+        self, dyn_ast: str, iid: int, base: Any, sl: List[Union[int, Tuple]], val: Any
+    ) -> Any:
         """Hook for reading a subscript, also known as a slice.
         E.g. `obj[1, 2]`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
@@ -500,25 +539,27 @@
             Unique ID of the syntax tree node.
         base : Any
             The object to which the subscript is attached.
         sl : List[Union[int, Tuple]]
             The subscript.
         val : Any
             The resulting value.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
         """
-        self.log(iid, 'Slice', sl)
+        self.log(iid, "Slice", sl)
 
     # Instrumented function
 
-    def function_enter(self, dyn_ast: str, iid: int, name: str, args: List[Any], is_lambda: bool) -> None:
+    def function_enter(
+        self, dyn_ast: str, iid: int, name: str, args: List[Any], is_lambda: bool
+    ) -> None:
         """Hook for when an instrumented function is entered.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
@@ -531,49 +572,80 @@
             Whether the function is a lambda function.
         """
         tmp = self._get_ast(dyn_ast)
         if tmp is not None:
             ast, iids = tmp
         else:
             return
-        if (not is_lambda) and (get_node_by_location(ast, iids.iid_to_location[iid], m.FunctionDef()).name in ['__str__', '__repr__']):
-            self.log(iid, 'Entered function', danger_of_recursion=True)
-
-    def function_exit(self, dyn_ast: str, iid: int, function_iid: int, name: str, result: Any) -> Any:
+        if (not is_lambda) and (
+            get_node_by_location(ast, iids.iid_to_location[iid], m.FunctionDef()).name
+            in ["__str__", "__repr__"]
+        ):
+            self.log(iid, "Entered function", danger_of_recursion=True)
+
+    def function_exit(
+        self, dyn_ast: str, function_iid: int, name: str, result: Any
+    ) -> Any:
         """Hook for exiting an instrumented function.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
-        iid : int
-            Unique ID of the syntax tree node.
         function_iid: int
             ID unique to the current file, referring to the function
         name: str
             Name of the function called
         result : Any
             The result of the function.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
         """
-        self.log(iid, 'Exiting function')
-    
-    def _return(self, dyn_ast: str, iid: int, value: Any) -> Any:
-        self.log(iid, '   Returning', value)
+        self.log(function_iid, "Exiting function")
+
+    def _return(self, dyn_ast: str, iid: int, function_iid: int, value: Any) -> Any:
+        """Hook for instrumented return statement.
 
-    def _yield(self, dyn_ast: str, iid: int, value: Any) -> Any:
-        self.log(iid, '   Yielding', value)
+        Parameters
+        ----------
+        dyn_ast : str
+            The path to the original code. Can be used to extract the syntax tree.
+        iid: int
+            ID unique to the current file, referring to the return statement
+        function_iid: int
+            ID unique to the current file, referring to the function
+        value : Any
+            The value returned.
+        """
+        self.log(iid, "   Returning", value)
+
+    def _yield(self, dyn_ast: str, iid: int, function_iid: int, value: Any) -> Any:
+        """Hook for instrumented yield statement.
+
+        Parameters
+        ----------
+        dyn_ast : str
+            The path to the original code. Can be used to extract the syntax tree.
+        iid: int
+            ID unique to the current file, referring to the yield statement
+        function_iid: int
+            ID unique to the current file, referring to the function
+        value : Any
+            The value yielded.
+        """
+        self.log(iid, "   Yielding", value)
 
     # Function Call
 
-    def pre_call(self, dyn_ast: str, iid: int, function: Callable, pos_args: Tuple, kw_args: Dict):
+    def pre_call(
+        self, dyn_ast: str, iid: int, function: Callable, pos_args: Tuple, kw_args: Dict
+    ):
         """Hook called before a function call happens.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
@@ -581,17 +653,25 @@
         function : str
             Function which will be called
         pos_args : Tuple
             The positional arguments passed to the function.
         kw_args : Dict
             The keyword arguments passed to the function.
         """
-        self.log(iid, 'Before function call')
-    
-    def post_call(self, dyn_ast: str, iid: int, result: Any, call: Callable, pos_args: Tuple, kw_args: Dict) -> Any:
+        self.log(iid, "Before function call")
+
+    def post_call(
+        self,
+        dyn_ast: str,
+        iid: int,
+        result: Any,
+        call: Callable,
+        pos_args: Tuple,
+        kw_args: Dict,
+    ) -> Any:
         """Hook called after a function call.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
@@ -600,25 +680,27 @@
             The return value of the function.
         call: Callable
             The function which was called
         pos_args : Tuple
             The positional arguments passed to the function.
         kw_args : Dict
             The keyword arguments passed to the function.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
         """
-        self.log(iid, 'After function call')
+        self.log(iid, "After function call")
 
     # Statements
-    
-    def augmented_assignment(self, dyn_ast: str, iid: int, left: Any, op: str, right: Any) -> Any:
+
+    def augmented_assignment(
+        self, dyn_ast: str, iid: int, left: Any, op: str, right: Any
+    ) -> Any:
         """Hook for any augmented assignment.
         E.g. `a += 1`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
@@ -628,156 +710,166 @@
             The left operand.
         op : str
             The operator.
         right : Any
             The right operand.
         val : Any
             The resulting value.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the result.
         """
-        self.log(iid, 'Augmented assignment', left, op, right)
-    
+        self.log(iid, "Augmented assignment", left, op, right)
+
     def add_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def bit_and_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def bit_or_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def bit_xor_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def divide_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def floor_divide_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def left_shift_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
-    def matrix_multiply_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
+    def matrix_multiply_assign(
+        self, dyn_ast: str, iid: int, left: Any, right: Any
+    ) -> Any:
+        self.log(iid, "Augmented assignment", left, right)
+
     def modulo_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def multiply_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def power_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def right_shift_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
-    
+        self.log(iid, "Augmented assignment", left, right)
+
     def subtract_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
-        self.log(iid, 'Augmented assignment', left, right)
+        self.log(iid, "Augmented assignment", left, right)
 
-    def _raise(self, dyn_ast: str, iid: int, exc: Exception, cause: Any) -> Optional[Exception]:
+    def _raise(
+        self, dyn_ast: str, iid: int, exc: Exception, cause: Any
+    ) -> Optional[Exception]:
         """Hook for instrumented raise statement.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         exc : Exception
             The exception raised.
         cause : Any
             The cause of the exception.
-        
+
         Returns
         -------
         Exception
             If provided, changes the exception raised.
         """
-        self.log(iid, 'Exception raised', exc, 'because of', cause)
+        self.log(iid, "Exception raised", exc, "because of", cause)
 
-    def _assert(self, dyn_ast: str, iid: int, condition: bool, message: str) -> Optional[bool]:
+    def _assert(
+        self, dyn_ast: str, iid: int, condition: bool, message: str
+    ) -> Optional[bool]:
         """Hook for assert statement.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         condition : bool
             The condition to assert.
         message : str
             The message to display if the condition is false.
-        
+
         Returns
         -------
         bool
             If provided, changes the condition of assert.
         """
-        self.log(iid, 'Asserting', condition, 'with message', message)
+        self.log(iid, "Asserting", condition, "with message", message)
 
     # Control flow
 
-    def enter_control_flow(self, dyn_ast: str, iid: int, cond_value: bool) -> Optional[bool]:
+    def enter_control_flow(
+        self, dyn_ast: str, iid: int, cond_value: bool
+    ) -> Optional[bool]:
         """Hook called when entering a control flow branch.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         cond_value : bool
             The value of the condition.
-        
+
         Returns
         -------
         bool
             If provided, changes the condition of the control flow.
         """
-        self.log(iid, 'Control-flow enter', 'with condition', cond_value)
-    
+        self.log(iid, "Control-flow enter", "with condition", cond_value)
+
     def exit_control_flow(self, dyn_ast: str, iid: int) -> None:
         """Hook called when exiting a control flow branch.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         """
-        self.log(iid, 'Control-flow exit')
+        self.log(iid, "Control-flow exit")
 
     def enter_if(self, dyn_ast: str, iid: int, cond_value: bool) -> Optional[bool]:
         """Hook called when entering an if conditional.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         cond_value : bool
             Whether the condition is true or false.
-        
+
         Returns
         -------
         Optional[bool]
             If provided, overwrites the condition (which may change the branch outcome).
         """
-        self.log(iid, '   If', cond_value)
+        self.log(iid, "   If", cond_value)
 
-    def enter_for(self, dyn_ast: str, iid: int, next_value: Any, iterable: Iterable) -> Optional[Any]:
+    def enter_for(
+        self, dyn_ast: str, iid: int, next_value: Any, iterable: Iterable
+    ) -> Optional[Any]:
         """Hook for entering a single iteration of a for loop.
 
         In most cases it should be ensured that the provided iterable is not consumed
         as the instrumented program will use it later on in the actual for loop.
 
         Parameters
         ----------
@@ -785,120 +877,122 @@
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         next_value : Any
             The next value of the iterator.
         iterable: Iterable
             Iterable used in the for loop.
-        
+
         Returns
         -------
         Any
             If provided, overwrites the value of the iterator.
         """
-        self.log(iid, '   For', next_value)
+        self.log(iid, "   For", next_value)
 
     def exit_for(self, dyn_ast, iid):
         """Hook for exiting a for loop.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
-        
+
         """
-        self.log(iid, 'For exit')
+        self.log(iid, "For exit")
 
     def enter_while(self, dyn_ast: str, iid: int, cond_value: bool) -> Optional[bool]:
         """Hook for entering the next iteration of a while loop.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         cond_value : bool
             The value of the condition (which may change the branch outcome).
-        
+
         Returns
         -------
         bool
             If provided, overwrites the condition.
         """
-        self.log(iid, '   While', cond_value)
+        self.log(iid, "   While", cond_value)
 
     def _break(self, dyn_ast: str, iid: int) -> Optional[bool]:
         """Hook for break statement.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
-        
+
         Returns
         -------
         bool
             If False, cancels the break.
         """
-        self.log(iid, 'Break')
+        self.log(iid, "Break")
 
     def _continue(self, dyn_ast: str, iid: int) -> Optional[bool]:
         """Hook for continue statement.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
-        
+
         Returns
         -------
         bool
             If False, cancels continue.
         """
-        self.log(iid, 'Continue')
+        self.log(iid, "Continue")
 
     def _try(self, dyn_ast: str, iid: int) -> None:
         """Hook for entering a try block.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         """
-        self.log(iid, 'Entered try')
+        self.log(iid, "Entered try")
 
-    def exception(self, dyn_ast: str, iid: int, exceptions: List[Exception], caught: Exception) -> Optional[Exception]:
+    def exception(
+        self, dyn_ast: str, iid: int, exceptions: List[Exception], caught: Exception
+    ) -> Optional[Exception]:
         """Hook for entering an except block.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
         iid : int
             Unique ID of the syntax tree node.
         exceptions : List[Exception]
             The exceptions to catch.
         caught : Exception
             The exception caught.
-        
+
         Returns
         -------
         Exception
             If provided, overwrites the exception caught.
         """
-        self.log(iid, 'Caught', caught, 'from', exceptions)
+        self.log(iid, "Caught", caught, "from", exceptions)
 
     # Top level
 
     def runtime_event(self, dyn_ast: str, iid: int) -> None:
         """Hook for any runtime event.
 
         Parameters
@@ -916,16 +1010,16 @@
         Parameters
         ----------
         exc : Exception
             The exception raised.
         stack_trace : TracebackType
             The stack trace of the exception.
         """
-        self.log(-1, 'Uncaught exception', exc, stack_trace)
-    
+        self.log(-1, "Uncaught exception", exc, stack_trace)
+
     def begin_execution(self) -> None:
         """Hook for the start of execution."""
-        self.log(-1, 'Execution started')
-    
+        self.log(-1, "Execution started")
+
     def end_execution(self) -> None:
         """Hook for the end of execution."""
-        self.log(-1, 'Execution ended')
+        self.log(-1, "Execution ended")
```

### Comparing `dynapyt-0.2.2/src/dynapyt/instrument/CodeInstrumenter.py` & `dynapyt-0.2.3/src/dynapyt/instrument/CodeInstrumenter.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/instrument/IIDs.py` & `dynapyt-0.2.3/src/dynapyt/instrument/IIDs.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/instrument/instrument.py` & `dynapyt-0.2.3/src/dynapyt/instrument/instrument.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/run_all.py` & `dynapyt-0.2.3/src/dynapyt/run_all.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/run_analysis.py` & `dynapyt-0.2.3/src/dynapyt/run_analysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/run_instrumentation.py` & `dynapyt-0.2.3/src/dynapyt/run_instrumentation.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/runtime.py` & `dynapyt-0.2.3/src/dynapyt/runtime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,95 @@
 from sys import exc_info
 from typing import Callable
 import libcst as cst
 from dynapyt.utils.hooks import snake, get_name
 
 analysis = None
 
+
 def set_analysis(new_analysis):
     global analysis
     analysis = new_analysis
 
+
 def call_if_exists(f, *args):
     func = getattr(analysis, f, lambda *args: None)
     return func(*args)
 
+
 def _dynapyt_parse_to_ast_(code):
     return cst.parse_module(code)
 
+
 def _write_(dyn_ast, iid, right, left):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('memory_access', dyn_ast, iid, right)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("memory_access", dyn_ast, iid, right)
     new_left = left
-    res = call_if_exists('write', dyn_ast, iid, new_left, right)
+    res = call_if_exists("write", dyn_ast, iid, new_left, right)
     if res != None:
         return res
     return right
 
+
 def _aug_assign_(dyn_ast, iid, left, opr, right):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    operator = ['AddAssign', 'BitAndAssign', 'BitOrAssign', 'BitXorAssign', 'DivideAssign',
-            'FloorDivideAssign', 'LeftShiftAssign', 'MatrixMultiplyAssign', 'ModuloAssign',
-            'MultiplyAssign', 'PowerAssign', 'RightShiftAssign', 'SubtractAssign']
-    call_if_exists('operation', dyn_ast, iid, operator[opr][:-6], [left, right], None)
-    call_if_exists('binary_operation', dyn_ast, iid, operator[opr][:-6], left, right, None)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    operator = [
+        "AddAssign",
+        "BitAndAssign",
+        "BitOrAssign",
+        "BitXorAssign",
+        "DivideAssign",
+        "FloorDivideAssign",
+        "LeftShiftAssign",
+        "MatrixMultiplyAssign",
+        "ModuloAssign",
+        "MultiplyAssign",
+        "PowerAssign",
+        "RightShiftAssign",
+        "SubtractAssign",
+    ]
+    call_if_exists("operation", dyn_ast, iid, operator[opr][:-6], [left, right], None)
+    call_if_exists(
+        "binary_operation", dyn_ast, iid, operator[opr][:-6], left, right, None
+    )
     call_if_exists(snake(operator[opr][:-6]), dyn_ast, iid, left, right, None)
-    call_if_exists('memory_access', dyn_ast, iid, right)
-    call_if_exists('write', dyn_ast, iid, [left], right)
-    result_high = call_if_exists('augmented_assignment', dyn_ast, iid, left, operator[opr], right)
-    result_low = call_if_exists(get_name(snake(operator[opr])), dyn_ast, iid, left, right)
+    call_if_exists("memory_access", dyn_ast, iid, right)
+    call_if_exists("write", dyn_ast, iid, [left], right)
+    result_high = call_if_exists(
+        "augmented_assignment", dyn_ast, iid, left, operator[opr], right
+    )
+    result_low = call_if_exists(
+        get_name(snake(operator[opr])), dyn_ast, iid, left, right
+    )
     if result_low != None:
         right = result_low
     elif result_high != None:
         right = result_high
     return right
 
+
 def _binary_op_(dyn_ast, iid, left, opr, right):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    bin_op = ['Add', 'BitAnd', 'BitOr', 'BitXor', 'Divide', 'FloorDivide',
-        'LeftShift', 'MatrixMultiply', 'Modulo', 'Multiply', 'Power',
-        'RightShift', 'Subtract', 'And', 'Or']
+    call_if_exists("runtime_event", dyn_ast, iid)
+    bin_op = [
+        "Add",
+        "BitAnd",
+        "BitOr",
+        "BitXor",
+        "Divide",
+        "FloorDivide",
+        "LeftShift",
+        "MatrixMultiply",
+        "Modulo",
+        "Multiply",
+        "Power",
+        "RightShift",
+        "Subtract",
+        "And",
+        "Or",
+    ]
     if opr < 13:
         try:
             left = left()
             right = right()
         except TypeError:
             raise
     if opr == 0:
@@ -71,15 +109,15 @@
     elif opr == 7:
         result = left @ right
     elif opr == 8:
         result = left % right
     elif opr == 9:
         result = left * right
     elif opr == 10:
-        result = left ** right
+        result = left**right
     elif opr == 11:
         result = left >> right
     elif opr == 12:
         result = left - right
     elif opr == 13:
         try:
             left = left()
@@ -102,47 +140,67 @@
             result = left
         else:
             try:
                 right = right()
             except TypeError:
                 raise
             result = left or right
-    call_if_exists('operation', dyn_ast, iid, bin_op[opr], [left, right], result)
-    result_high = call_if_exists('binary_operation', dyn_ast, iid, bin_op[opr], left, right, result)
-    result_low = call_if_exists(get_name(snake(bin_op[opr])), dyn_ast, iid, left, right, result)
+    call_if_exists("operation", dyn_ast, iid, bin_op[opr], [left, right], result)
+    result_high = call_if_exists(
+        "binary_operation", dyn_ast, iid, bin_op[opr], left, right, result
+    )
+    result_low = call_if_exists(
+        get_name(snake(bin_op[opr])), dyn_ast, iid, left, right, result
+    )
     if result_low != None:
         return result_low
     elif result_high != None:
         return result_high
     return result
 
+
 def _unary_op_(dyn_ast, iid, opr, right):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    un_op = ['BitInvert', 'Minus', 'Not', 'Plus']
+    call_if_exists("runtime_event", dyn_ast, iid)
+    un_op = ["BitInvert", "Minus", "Not", "Plus"]
     if opr == 0:
-        result = ~ right
+        result = ~right
     elif opr == 1:
-        result = - right
+        result = -right
     elif opr == 2:
         result = not right
     elif opr == 3:
-        result = + right
-    call_if_exists('operation', dyn_ast, iid, un_op[opr], [right], result)
-    result_high = call_if_exists('unary_operation', dyn_ast, iid, un_op[opr], right, result)
-    result_low = call_if_exists(get_name(snake(un_op[opr])), dyn_ast, iid, right, result)
+        result = +right
+    call_if_exists("operation", dyn_ast, iid, un_op[opr], [right], result)
+    result_high = call_if_exists(
+        "unary_operation", dyn_ast, iid, un_op[opr], right, result
+    )
+    result_low = call_if_exists(
+        get_name(snake(un_op[opr])), dyn_ast, iid, right, result
+    )
     if result_low != None:
         return result_low
     elif result_high != None:
         return result_high
     return result
 
+
 def _comp_op_(dyn_ast, iid, left, comparisons):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    comp_op = ['Equal', 'GreaterThan', 'GreaterThanEqual', 'In', 'Is', 'LessThan',
-        'LessThanEqual', 'NotEqual', 'IsNot', 'NotIn']
+    call_if_exists("runtime_event", dyn_ast, iid)
+    comp_op = [
+        "Equal",
+        "GreaterThan",
+        "GreaterThanEqual",
+        "In",
+        "Is",
+        "LessThan",
+        "LessThanEqual",
+        "NotEqual",
+        "IsNot",
+        "NotIn",
+    ]
     l = left
     result = True
     for op, r in comparisons:
         if op == 0:
             tmp = l == r
         elif op == 1:
             tmp = l > r
@@ -158,322 +216,371 @@
             tmp = l <= r
         elif op == 7:
             tmp = l != r
         elif op == 8:
             tmp = l is not r
         elif op == 9:
             tmp = l not in r
-        call_if_exists('operation', dyn_ast, iid, comp_op[op], [left, r], tmp)
-        result_high = call_if_exists('comparison', dyn_ast, iid, l, comp_op[op], r, tmp)
-        result_low = call_if_exists(get_name(snake(comp_op[op])), dyn_ast, iid, l, r, tmp)
+        call_if_exists("operation", dyn_ast, iid, comp_op[op], [left, r], tmp)
+        result_high = call_if_exists("comparison", dyn_ast, iid, l, comp_op[op], r, tmp)
+        result_low = call_if_exists(
+            get_name(snake(comp_op[op])), dyn_ast, iid, l, r, tmp
+        )
         if result_low != None:
             tmp = result_low
         elif result_high != None:
             tmp = result_high
         result = result and tmp
         l = r
     return result
 
+
 def _call_(dyn_ast, iid, call, only_post, pos_args, kw_args):
-    call_if_exists('runtime_event', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
     if only_post:
         result = call
-        new_res = call_if_exists('post_call', dyn_ast, iid, result, call, pos_args, kw_args)
+        new_res = call_if_exists(
+            "post_call", dyn_ast, iid, result, call, pos_args, kw_args
+        )
         return new_res if new_res is not None else result
     else:
         tmp = []
         for star, a in pos_args:
-            if star == '':
+            if star == "":
                 tmp.append(a)
-            elif star == '*':
+            elif star == "*":
                 tmp.extend(list(a))
             else:
                 kw_args = dict(kw_args, **a)
         pos_args = tuple(tmp)
-        call_if_exists('pre_call', dyn_ast, iid, call, pos_args, kw_args)
+        call_if_exists("pre_call", dyn_ast, iid, call, pos_args, kw_args)
         result = call(*pos_args, **kw_args)
-        new_res = call_if_exists('post_call', dyn_ast, iid, result, call, pos_args, kw_args)
+        new_res = call_if_exists(
+            "post_call", dyn_ast, iid, result, call, pos_args, kw_args
+        )
         return new_res if new_res is not None else result
 
+
 def _bool_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    res_high = call_if_exists('literal', dyn_ast, iid, val)
-    res_low = call_if_exists('boolean', dyn_ast, iid, val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    res_high = call_if_exists("literal", dyn_ast, iid, val)
+    res_low = call_if_exists("boolean", dyn_ast, iid, val)
     if res_low != None:
         return res_low
     elif res_high != None:
         return res_high
     return val
 
+
 def _int_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    res_high = call_if_exists('literal', dyn_ast, iid, val)
-    res_low = call_if_exists('integer', dyn_ast, iid, val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    res_high = call_if_exists("literal", dyn_ast, iid, val)
+    res_low = call_if_exists("integer", dyn_ast, iid, val)
     if res_low != None:
         return res_low
     elif res_high != None:
         return res_high
     return val
 
+
 def _float_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    res_high = call_if_exists('literal', dyn_ast, iid, val)
-    res_low = call_if_exists('float', dyn_ast, iid, val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    res_high = call_if_exists("literal", dyn_ast, iid, val)
+    res_low = call_if_exists("float", dyn_ast, iid, val)
     if res_low != None:
         return res_low
     elif res_high != None:
         return res_high
     return val
 
+
 def _str_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    res_high = call_if_exists('literal', dyn_ast, iid, val)
-    res_low = call_if_exists('string', dyn_ast, iid, val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    res_high = call_if_exists("literal", dyn_ast, iid, val)
+    res_low = call_if_exists("string", dyn_ast, iid, val)
     if res_low != None:
         return res_low
     elif res_high != None:
         return res_high
     return val
 
+
 def _img_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    res_high = call_if_exists('literal', dyn_ast, iid, val)
-    res_low = call_if_exists('imaginary', dyn_ast, iid, val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    res_high = call_if_exists("literal", dyn_ast, iid, val)
+    res_low = call_if_exists("imaginary", dyn_ast, iid, val)
     if res_low != None:
         return res_low
     elif res_high != None:
         return res_high
     return val
 
+
 def _literal_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    res = call_if_exists('literal', dyn_ast, iid, val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    res = call_if_exists("literal", dyn_ast, iid, val)
     return res if res != None else val
 
+
 def _dict_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
     value = dict()
     for v in val:
         if not isinstance(v, tuple):
             value.update(v)
         else:
             value.update({v[0]: v[1]})
-    call_if_exists('literal', dyn_ast, iid, value)
-    res = call_if_exists('dictionary', dyn_ast, iid, val, value)
+    call_if_exists("literal", dyn_ast, iid, value)
+    res = call_if_exists("dictionary", dyn_ast, iid, val, value)
     return res if res != None else value
 
+
 def _list_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('literal', dyn_ast, iid, val)
-    res = call_if_exists('_list', dyn_ast, iid, val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("literal", dyn_ast, iid, val)
+    res = call_if_exists("_list", dyn_ast, iid, val)
     return res if res != None else val
 
+
 def _tuple_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
     value = tuple(val)
-    call_if_exists('literal', dyn_ast, iid, value)
-    call_if_exists('_tuple', dyn_ast, iid, val, value)
+    call_if_exists("literal", dyn_ast, iid, value)
+    call_if_exists("_tuple", dyn_ast, iid, val, value)
     return value
 
+
 def _delete_(dyn_ast, iid, del_target):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('memory_access', dyn_ast, iid, del_target)
-    cancel = call_if_exists('delete', dyn_ast, iid, del_target)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("memory_access", dyn_ast, iid, del_target)
+    cancel = call_if_exists("delete", dyn_ast, iid, del_target)
     if (cancel is not None) and (cancel == True):
         pass
     else:
         for dt in del_target:
             base, offset, is_sub = dt
             if is_sub:
                 if len(offset) == 1:
                     base.__delitem__(offset[0])
                 else:
                     base.__delitem__(slice(offset))
             else:
                 delattr(base, offset)
 
+
 def _attr_(dyn_ast, iid, base, attr):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    if (attr.startswith('__')) and (not attr.endswith('__')):
-        if type(base).__name__ == 'type':
+    call_if_exists("runtime_event", dyn_ast, iid)
+    if (attr.startswith("__")) and (not attr.endswith("__")):
+        if type(base).__name__ == "type":
             parents = [base]
         else:
             parents = [type(base)]
         found = True
         while len(parents) > 0:
             found = True
             cur_par = parents.pop()
             try:
                 cur_name = cur_par.__name__
-                cur_name = cur_name.lstrip('_')
-                val = getattr(base, '_'+cur_name+attr)
+                cur_name = cur_name.lstrip("_")
+                val = getattr(base, "_" + cur_name + attr)
             except AttributeError:
                 found = False
                 parents.extend(list(cur_par.__bases__))
                 continue
             break
         if not found:
             raise AttributeError()
     else:
         val = getattr(base, attr)
-    call_if_exists('memory_access', dyn_ast, iid, val)
-    call_if_exists('read', dyn_ast, iid, val)
-    result = call_if_exists('read_attribute', dyn_ast, iid, base, attr, val)
+    call_if_exists("memory_access", dyn_ast, iid, val)
+    call_if_exists("read", dyn_ast, iid, val)
+    result = call_if_exists("read_attribute", dyn_ast, iid, base, attr, val)
     return result if result != None else val
 
+
 def _sub_(dyn_ast, iid, base, sl):
-    call_if_exists('runtime_event', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
     if len(sl) == 1:
         val = base[sl[0]]
     else:
         val = base[tuple(sl)]
-    call_if_exists('memory_access', dyn_ast, iid, val)
-    call_if_exists('read', dyn_ast, iid, val)
-    result = call_if_exists('read_subscript', dyn_ast, iid, base, sl, val)
+    call_if_exists("memory_access", dyn_ast, iid, val)
+    call_if_exists("read", dyn_ast, iid, val)
+    result = call_if_exists("read_subscript", dyn_ast, iid, base, sl, val)
     return result if result != None else val
 
+
 def _try_(dyn_ast, iid):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('enter_try', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("enter_try", dyn_ast, iid)
+
 
 def _end_try_(dyn_ast, iid):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('clean_exit_try', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("clean_exit_try", dyn_ast, iid)
+
 
 def _exc_(dyn_ast, iid, exc=None, name=None):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('exception', dyn_ast, iid, exc, name)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("exception", dyn_ast, iid, exc, name)
+
 
 def _raise_(dyn_ast, iid, exc=None, cause=None):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    res = call_if_exists('_raise', dyn_ast, iid, exc, cause)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    res = call_if_exists("_raise", dyn_ast, iid, exc, cause)
     if res is not None:
         exc, cause = res
     if exc == None:
         raise
     else:
         if cause == None:
             raise exc
         else:
             raise exc from cause
 
+
 def _catch_(exception):
     t, v, stack_trace = exc_info()
-    call_if_exists('runtime_event', '', -1)
-    call_if_exists('uncaught_exception', exception, stack_trace)
+    call_if_exists("runtime_event", "", -1)
+    call_if_exists("uncaught_exception", exception, stack_trace)
     raise exception
 
+
 def _read_(dyn_ast, iid, var_arg):
-    call_if_exists('runtime_event', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
     value = var_arg()
-    call_if_exists('memory_access', dyn_ast, iid, value)
-    call_if_exists('read', dyn_ast, iid, value)
-    result = call_if_exists('read_identifier', dyn_ast, iid, value)
+    call_if_exists("memory_access", dyn_ast, iid, value)
+    call_if_exists("read", dyn_ast, iid, value)
+    result = call_if_exists("read_identifier", dyn_ast, iid, value)
     return result if result != None else value
 
+
 def _if_(dyn_ast, iid, val):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result = call_if_exists('_if', dyn_ast, iid, val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result = call_if_exists("_if", dyn_ast, iid, val)
     return result if result != None else val
 
+
 def _func_entry_(dyn_ast, iid, args, name: str, is_lambda=False):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('function_enter', dyn_ast, iid, args, name, is_lambda)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("function_enter", dyn_ast, iid, args, name, is_lambda)
+
 
 def _func_exit_(dyn_ast, iid, name: str):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('function_exit', dyn_ast, iid, name, None)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("function_exit", dyn_ast, iid, name, None)
     return
 
+
 def _return_(dyn_ast, iid, function_iid, function_name, return_val=None):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result_high = call_if_exists('function_exit', dyn_ast, function_iid, function_name, return_val)
-    result_low = call_if_exists('_return', dyn_ast, iid, return_val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result_high = call_if_exists(
+        "function_exit", dyn_ast, function_iid, function_name, return_val
+    )
+    result_low = call_if_exists(
+        "_return", dyn_ast, iid, function_iid, return_val
+    )  # return needs both its own iid and the function iid
     if result_low != None:
         return result_low
     elif result_high != None:
         return result_high
     return return_val
 
+
 def _yield_(dyn_ast, iid, function_iid, function_name, return_val=None):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result_high = call_if_exists('function_exit', dyn_ast, function_iid, function_name, return_val)
-    result_low = call_if_exists('_yield', dyn_ast, iid, return_val)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result_high = call_if_exists(
+        "function_exit", dyn_ast, function_iid, function_name, return_val
+    )
+    result_low = call_if_exists("_yield", dyn_ast, iid, function_iid, return_val)
     if result_low != None:
         return result_low
     elif result_high != None:
         return result_high
     return return_val
 
+
 def _assert_(dyn_ast, iid, test, msg):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result = call_if_exists('_assert', dyn_ast, iid, test, msg)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result = call_if_exists("_assert", dyn_ast, iid, test, msg)
     return result if result is not None else test
 
+
 def _lambda_(dyn_ast, iid, args, expr):
     _func_entry_(dyn_ast, iid, args, "lambda", True)
     res = expr()
     return _return_(dyn_ast, iid, iid, res)
 
+
 def _break_(dyn_ast, iid):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result = call_if_exists('_break', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result = call_if_exists("_break", dyn_ast, iid)
     return result if result != None else True
 
+
 def _continue_(dyn_ast, iid):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result = call_if_exists('_continue', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result = call_if_exists("_continue", dyn_ast, iid)
     return result if result != None else True
 
+
 def _enter_if_(dyn_ast, iid, condition):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result_high = call_if_exists('enter_control_flow', dyn_ast, iid, condition)
-    result_low = call_if_exists('enter_if', dyn_ast, iid, condition)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result_high = call_if_exists("enter_control_flow", dyn_ast, iid, condition)
+    result_low = call_if_exists("enter_if", dyn_ast, iid, condition)
     if result_low is not None:
         return result_low
     elif result_high is not None:
         return result_high
     return condition
 
+
 def _exit_if_(dyn_ast, iid):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('exit_control_flow', dyn_ast, iid)
-    call_if_exists('exit_if', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("exit_control_flow", dyn_ast, iid)
+    call_if_exists("exit_if", dyn_ast, iid)
+
 
 def _enter_while_(dyn_ast, iid, condition):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result_high = call_if_exists('enter_control_flow', dyn_ast, iid, condition)
-    result_low = call_if_exists('enter_while', dyn_ast, iid, condition)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result_high = call_if_exists("enter_control_flow", dyn_ast, iid, condition)
+    result_low = call_if_exists("enter_while", dyn_ast, iid, condition)
     if result_low is not None:
         return result_low
     elif result_high is not None:
         return result_high
     return condition
 
+
 def _exit_while_(dyn_ast, iid):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('exit_control_flow', dyn_ast, iid)
-    call_if_exists('exit_while', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("exit_control_flow", dyn_ast, iid)
+    call_if_exists("exit_while", dyn_ast, iid)
+
 
 def _enter_for_(dyn_ast, iid, next_val, iterable):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    result_high = call_if_exists('enter_control_flow', dyn_ast, iid, not isinstance(next_val, StopIteration))
-    result_low = call_if_exists('enter_for', dyn_ast, iid, next_val, iterable)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    result_high = call_if_exists(
+        "enter_control_flow", dyn_ast, iid, not isinstance(next_val, StopIteration)
+    )
+    result_low = call_if_exists("enter_for", dyn_ast, iid, next_val, iterable)
     if result_low is not None:
         return result_low
     elif result_high is not None:
         if result_high:
             return next_val
         raise StopIteration()
     return next_val
 
+
 def _exit_for_(dyn_ast, iid):
-    call_if_exists('runtime_event', dyn_ast, iid)
-    call_if_exists('exit_control_flow', dyn_ast, iid)
-    call_if_exists('exit_for', dyn_ast, iid)
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("exit_control_flow", dyn_ast, iid)
+    call_if_exists("exit_for", dyn_ast, iid)
+
 
 def _gen_(dyn_ast, iid, iterator):
     if iterator is None:
         return
 
     new_iter = iter(iterator)
     while True:
@@ -482,8 +589,8 @@
             result = _enter_for_(dyn_ast, iid, it, iterator)
             if result is not None:
                 yield result
             else:
                 yield it
         except StopIteration as e:
             _enter_for_(dyn_ast, iid, e, iterator)
-            return
+            return
```

### Comparing `dynapyt-0.2.2/src/dynapyt/utils/AnalysisUtils.py` & `dynapyt-0.2.3/src/dynapyt/utils/AnalysisUtils.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/utils/hierarchy.json` & `dynapyt-0.2.3/src/dynapyt/utils/hierarchy.json`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/utils/hooks.py` & `dynapyt-0.2.3/src/dynapyt/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/src/dynapyt/utils/nodeLocator.py` & `dynapyt-0.2.3/src/dynapyt/utils/nodeLocator.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.2/PKG-INFO` & `dynapyt-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: dynapyt
-Version: 0.2.2
-Summary: DynaPyt
+Version: 0.2.3
+Summary: Dynamic analysis framework for Python
+Project-URL: Bug Tracker, https://github.com/sola-st/DynaPyt/issues
+Project-URL: Homepage, https://github.com/sola-st/DynaPyt
 Author-email: Aryaz Eghbali <aryaz.egh@gmail.com>, Michael Pradel <michael@binaervarianz.de>
-Description-Content-Type: text/markdown
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
-Project-URL: Home, https://github.com/sola-st/dynapyt
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Requires-Dist: libcst
+Description-Content-Type: text/markdown
 
 # DynaPyt: A Dynamic Analysis Framework for Python
 DynaPyt is a dynamic analysis framework designed and developed by [Aryaz Eghbali and Michael Pradel](https://2022.esec-fse.org/details/fse-2022-research-papers/48/DynaPyt-A-Dynamic-Analysis-Framework-for-Python). 
 The framework provides hooks for a variety of runtime events in multiple layers of abstraction.
 Users can create arbitrary dynamic analyses by implementing relevant hooks.
 Beyond observing runtime behavior, DynaPyt also supports manipulation of behavior, e.g., to inject runtime values or modify branching decisions.
 
@@ -171,8 +177,7 @@
   author    = {Aryaz Eghbali and Michael Pradel},
   title     = {Dyna{P}yt: A Dynamic Analysis Framework for {P}ython},
   booktitle = {{ESEC/FSE} '22: 30th {ACM} Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering},
   year      = {2022},
   publisher = {{ACM}},
 }
 ```
-
```

