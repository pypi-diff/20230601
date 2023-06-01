# Comparing `tmp/mcda-0.5.0.tar.gz` & `tmp/mcda-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcda-0.5.0.tar", last modified: Wed Apr 19 15:55:27 2023, max compression
+gzip compressed data, was "mcda-0.5.1.tar", last modified: Thu Jun  1 16:07:38 2023, max compression
```

## Comparing `mcda-0.5.0.tar` & `mcda-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.378942 mcda-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-04-19 15:55:14.000000 mcda-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-19 15:55:14.000000 mcda-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3012 2023-04-19 15:55:27.378942 mcda-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2118 2023-04-19 15:55:14.000000 mcda-0.5.0/README.PYPI.md
--rw-rw-rw-   0 root         (0) root         (0)     2502 2023-04-19 15:55:14.000000 mcda-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.367941 mcda-0.5.0/mcda/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.374941 mcda-0.5.0/mcda/core/
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/aliases.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/categories.py
--rw-rw-rw-   0 root         (0) root         (0)     6345 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/criteria_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    15169 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    21163 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/matrices.py
--rw-rw-rw-   0 root         (0) root         (0)     8123 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/performance_table.py
--rw-rw-rw-   0 root         (0) root         (0)    20025 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/relations.py
--rw-rw-rw-   0 root         (0) root         (0)    20692 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/scales.py
--rw-rw-rw-   0 root         (0) root         (0)    21193 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/set_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    13700 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.374941 mcda-0.5.0/mcda/dea/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/dea/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.375941 mcda-0.5.0/mcda/mavt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/mavt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17750 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/mavt/aggregators.py
--rw-rw-rw-   0 root         (0) root         (0)    24133 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/mavt/uta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.377941 mcda-0.5.0/mcda/outranking/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/outranking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36397 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/outranking/electre.py
--rw-rw-rw-   0 root         (0) root         (0)    25895 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/outranking/promethee.py
--rw-rw-rw-   0 root         (0) root         (0)    40811 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/outranking/srmp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.378942 mcda-0.5.0/mcda/plot/
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41564 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/plot/plot.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.369941 mcda-0.5.0/mcda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3012 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      787 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-19 15:55:14.000000 mcda-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 15:55:27.378942 mcda-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1451 2023-04-19 15:55:14.000000 mcda-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:07:38.096783 mcda-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-01 16:07:28.000000 mcda-0.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-01 16:07:28.000000 mcda-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-06-01 16:07:38.096783 mcda-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-06-01 16:07:28.000000 mcda-0.5.1/README.PYPI.md
+-rw-rw-rw-   0 root         (0) root         (0)     2502 2023-06-01 16:07:28.000000 mcda-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:07:38.090783 mcda-0.5.1/mcda/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:07:38.093783 mcda-0.5.1/mcda/core/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/aliases.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)     6345 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/criteria_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15169 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    10282 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)     9919 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/performance_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    20125 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    20692 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/scales.py
+-rw-rw-rw-   0 root         (0) root         (0)    21193 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/set_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12267 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/core/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:07:38.094783 mcda-0.5.1/mcda/dea/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/dea/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:07:38.094783 mcda-0.5.1/mcda/mavt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/mavt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17750 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/mavt/aggregators.py
+-rw-rw-rw-   0 root         (0) root         (0)    24133 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/mavt/uta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:07:38.095783 mcda-0.5.1/mcda/outranking/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/outranking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36123 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/outranking/electre.py
+-rw-rw-rw-   0 root         (0) root         (0)    24851 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/outranking/promethee.py
+-rw-rw-rw-   0 root         (0) root         (0)    40875 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/outranking/srmp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:07:38.095783 mcda-0.5.1/mcda/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41564 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/plot/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-01 16:07:28.000000 mcda-0.5.1/mcda/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:07:38.091783 mcda-0.5.1/mcda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-06-01 16:07:38.000000 mcda-0.5.1/mcda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 16:07:38.000000 mcda-0.5.1/mcda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:07:38.000000 mcda-0.5.1/mcda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:07:37.000000 mcda-0.5.1/mcda.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-01 16:07:38.000000 mcda-0.5.1/mcda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-01 16:07:38.000000 mcda-0.5.1/mcda.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-01 16:07:28.000000 mcda-0.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 16:07:38.096783 mcda-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2023-06-01 16:07:28.000000 mcda-0.5.1/setup.py
```

### Comparing `mcda-0.5.0/LICENSE` & `mcda-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/PKG-INFO` & `mcda-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mcda
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package for Multi Criteria Decision Analysis
 Author: Nicolas Duminy
 Author-email: nicolas.duminy@imt-atlantique.fr
 Project-URL: Source, https://gitlab.com/decide.imt-atlantique/pymcda
 Project-URL: Documentation, https://py-mcda.readthedocs.io
 Project-URL: Tracker, https://gitlab.com/decide.imt-atlantique/pymcda/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
 
 
 # Package description
```

### Comparing `mcda-0.5.0/README.PYPI.md` & `mcda-0.5.1/README.PYPI.md`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/README.md` & `mcda-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda/core/categories.py` & `mcda-0.5.1/mcda/core/categories.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,32 +48,27 @@
         :param upmost:
             if ``True`` add a category profile with first profile as its lower
             bound (and no upper bound)
         :raises ValueError: if any profile doesn't dominate its predecessor
         :return:
             list of bounded category profiles in ascending domination order
         """
+        values = list(profiles.alternatives_values.values())
         try:
             res = [
                 cls(p1, p2)
                 for p1, p2 in zip(
-                    profiles.alternatives_values.at[:-1],
-                    profiles.alternatives_values.at[1:],
+                    values[:-1],
+                    values[1:],
                 )
             ]
             if upmost:
-                res = [cls(upper=profiles.alternatives_values.at[0])] + res
+                res = [cls(upper=values[0])] + res
             if lowest:
-                res += [
-                    cls(
-                        lower=profiles.alternatives_values.at[
-                            len(profiles.alternatives) - 1
-                        ]
-                    )
-                ]
+                res += [cls(lower=values[-1])]
             return res
         except ValueError:
             raise ValueError("any profile must dominate its predecessor")
 
 
 class CentralCategoryProfile:
     """This class represents a category defined by a central profile.
```

### Comparing `mcda-0.5.0/mcda/core/criteria_functions.py` & `mcda-0.5.1/mcda/core/criteria_functions.py`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda/core/functions.py` & `mcda-0.5.1/mcda/core/functions.py`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda/core/interfaces.py` & `mcda-0.5.1/mcda/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda/core/performance_table.py` & `mcda-0.5.1/mcda/core/performance_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,68 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Union, cast
 
-from pandas import DataFrame, Series
+from pandas import DataFrame, Series, concat
 from pandas.api.types import is_numeric_dtype  # type: ignore
 
 import mcda.core.criteria_functions
 
 from .aliases import Function
 from .matrices import Matrix
 from .scales import QuantitativeScale, Scale
-from .values import Container, ScaleValues
+from .values import ScaleValues
 
 
 class PerformanceTable(Matrix):
     """This class is used to represent performance tables.
 
     :param data: performance table in an array-like or dict structure
     :param scales: criteria scales (scales are inferred from data if not set)
     :param alternatives:
     :param criteria:
+    :raise KeyError:
+        * if some alternatives are duplicated
+        * if some criteria are duplicated
+        * if `scales` keys and `data` columns mismatch
 
-    :attr df: dataframe containing the performances
+    :attr data: dataframe containing the performances
     :attr scales: criteria scales
 
     .. note::
         when applying pandas methods to modify the performance table, do it
-        this way: `table.df = table.df.method()` (for a method called `method`)
+        this way: `table.data = table.data.method()` (for a method called
+        `method`)
 
         Also you may want to modify the criteria scales depending on such
         modifications.
     """
 
     def __init__(
         self,
         data,
         scales: Dict[Any, Scale] = None,
         alternatives: List[Any] = None,
         criteria: List[Any] = None,
     ):
         df = DataFrame(data, index=alternatives, columns=criteria)
+        if df.index.has_duplicates:
+            raise KeyError(
+                "some alternatives are duplicated: "
+                f"{df.index[df.index.duplicated()].tolist()}"
+            )
+        if df.columns.has_duplicates:
+            raise KeyError(
+                "some criteria are duplicated: "
+                f"{df.columns[df.columns.duplicated()].tolist()}"
+            )
         super().__init__(df)
         self.scales = self.bounds if scales is None else scales
+        if set(self.criteria) != set(self.scales.keys()):
+            raise KeyError("data and scales must have the same criteria")
 
     def __eq__(self, other) -> bool:
         """Check equality of performance tables.
 
         Equality is defines as having the same set of scales, and having the
         same dataframe.
 
@@ -65,32 +82,27 @@
 
     @property
     def alternatives(self) -> List[Any]:
         """Return performance table alternatives"""
         return self.data.index.tolist()
 
     @property
-    def alternatives_values(self) -> Container[ScaleValues]:
+    def alternatives_values(self) -> Dict[Any, ScaleValues]:
         """Iterator on the table alternatives values"""
-        return Container[ScaleValues](
-            dict(
-                (a, ScaleValues(self.data.loc[a], self.scales))
-                for a in self.alternatives
-            )
-        )
+        return {
+            a: ScaleValues(self.data.loc[a], self.scales)
+            for a in self.alternatives
+        }
 
     @property
-    def criteria_values(self) -> Container[ScaleValues]:
+    def criteria_values(self) -> Dict[Any, ScaleValues]:
         """Iterator on the table criteria values"""
-        return Container[ScaleValues](
-            dict(
-                (c, ScaleValues(self.data[c], self.scales[c]))
-                for c in self.criteria
-            )
-        )
+        return {
+            c: ScaleValues(self.data[c], self.scales[c]) for c in self.criteria
+        }
 
     @property
     def is_numeric(self) -> bool:
         """Check whether performance table is numeric.
 
         :return:
         :rtype: bool
@@ -119,15 +131,15 @@
 
         This is the list of alternatives that are not strongly dominated by
         another one.
 
         :return:
         """
         res = set(self.alternatives)
-        for avalues in self.alternatives_values:
+        for avalues in self.alternatives_values.values():
             dominated = set()
             for b in res:
                 if avalues.name == b:
                     continue
                 if avalues.dominate_strongly(self.alternatives_values[b]):
                     dominated.add(b)
             res -= dominated
@@ -258,7 +270,41 @@
             self.alternatives if alternatives is None else alternatives
         )
         criteria = self.criteria if criteria is None else criteria
         return self.__class__(
             self.data.loc[alternatives, criteria],
             {criterion: self.scales[criterion] for criterion in criteria},
         )
+
+    @classmethod
+    def concat(
+        cls,
+        performance_tables: List[PerformanceTable],
+        scales: Dict[Any, Scale] = None,
+        axis: int = 0,
+    ) -> PerformanceTable:
+        """Concatenate multiple performance tables.
+
+        :param performance_tables:
+        :param scales:
+            scales used in concatenated result (taken from `performance_tables`
+            scales if not set, with first occurence taken in case of duplicates
+            )
+        :param axis:
+            axis along which to concatenate
+            (0: add alternatives, 1: add criteria)
+        :return: concatenated performance table
+
+        .. warning::
+            `performance_tables` objects are concatenated as is, no
+            transformation of scales is applied.
+        """
+        scales = {} if scales is None else scales
+        dataframes: List[DataFrame] = []
+        for t in performance_tables:
+            dataframes.append(t.data)
+            for c, s in t.scales.items():
+                scales.setdefault(c, s)
+        # Must use int type for `axis` for python 3.7 compatibility
+        # But it breaks mypy
+        df = concat(dataframes, axis=axis)  # type: ignore
+        return cls(df, scales=scales)
```

### Comparing `mcda-0.5.0/mcda/core/relations.py` & `mcda-0.5.1/mcda/core/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,16 +559,20 @@
 
     The outranking matrix is represented internally by a
     :class:`pandas.DataFrame` with vertices as the indexes and columns.
 
     :param data: adjacency matrix in an array-like or dict-structure
     :param vertices:
 
-    :raise ValueError: if non-binary values are in the matrix
-    :raise ValueError: if columns and rows have different sets of labels
+    :raise ValueError:
+        * if non-binary values are in the matrix
+        * if columns and rows have different sets of labels
+    :raise KeyError:
+        * if some indexes are duplicated
+        * if some columns are duplicated
     """
 
     @property
     def preference_structure(self) -> PreferenceStructure:
         """Return corresponding preference structure."""
         relations: List[Relation] = list()
         for ii, i in enumerate(self.vertices):
```

### Comparing `mcda-0.5.0/mcda/core/scales.py` & `mcda-0.5.1/mcda/core/scales.py`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda/core/set_functions.py` & `mcda-0.5.1/mcda/core/set_functions.py`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda/core/values.py` & `mcda-0.5.1/mcda/core/values.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import ItemsView, KeysView, ValuesView
-from typing import Any, Dict, Generic, Iterator, List, TypeVar, cast
+from typing import Any, Dict, Iterator, List, cast
 
 from pandas import Series
 from pandas.api.types import is_numeric_dtype  # type: ignore
 
 from .relations import (
     IndifferenceRelation,
     IPreferenceStructure,
@@ -31,20 +30,26 @@
 class Values:
     """This class is a wrapper around :class:`pandas.Series`.
 
     It is intended to be used for all classes across the package that uses
     a Series as their internal data representation.
 
     :param data: series containing the data
+    :raise KeyError: if some labels are duplicated
 
     :attr data: internal representation of data
     """
 
     def __init__(self, data: Series):
         self.data = Series(data)
+        if self.data.index.has_duplicates:
+            raise KeyError(
+                "some labels are duplicated: "
+                f"{self.data.index[self.data.index.duplicated()].tolist()}"
+            )
 
     def __eq__(self, other: Any) -> bool:
         """Check if both values have the same data
 
         :return:
 
         .. note:: values order does not matter
@@ -108,15 +113,17 @@
     multiple :class:`mcda.core.Scale`.
 
     :param data: series containing the data
     :param scales:
         data scale(s) (one per value or one shared, will be inferred from data
         if absent using :meth:`ScaleValues.bounds`)
     :param preference_direction: (ignored is `scales` supplied)
-    :raise KeyError: if `scales` keys and `data` indexes mismatch
+    :raise KeyError:
+        * if some labels are duplicated
+        * if `scales` keys and `data` indexes mismatch
 
     :attr data: internal representation of data
     :attr scales: scales of the data (one per value)
     """
 
     def __init__(
         self,
@@ -293,14 +300,17 @@
     """This class describes a ranking as a :class:`ScaleValues`.
 
     It is intended as a shorthand to create rankings.
 
     :param data:
     :param preference_direction:
     :raise ValueError: if `data` contains non-numeric values
+    :raise KeyError:
+        * if some labels are duplicated
+        * if `scales` keys and `data` indexes mismatch
 
     :attr data: internal representation of data
     :attr scales:
         scales of the data (one per value, all equals to the same
         :class:`mcda.core.scales.QuantitativeScale` with bounds inferred from
         data)
     """
@@ -369,90 +379,7 @@
         :return:
         """
         return cls._from_preference_structure(data.preference_structure)
 
     def copy(self) -> "Ranking":
         """Return a copy of the object"""
         return Ranking(self.data.copy(), self.preference_direction)
-
-
-T = TypeVar("T")
-
-
-class Container(Generic[T]):
-    """This generic class is a container accessible and traversable as a dict
-    or a list.
-
-    :param values:
-    """
-
-    def __init__(self, values: Dict[Any, T]):
-        self._values = values
-
-    def __contains__(self, key: Any) -> bool:
-        """Check if `key` is in container.
-
-        :param key:
-        :return: ``true`` if `key` in container, ``False`` otherwise
-        """
-        return key in self._values
-
-    def __len__(self) -> int:
-        """Return length of container.
-
-        :return:
-        """
-        return len(self._values)
-
-    def __getitem__(self, key: Any) -> T:
-        """Get value by key.
-
-        :param key:
-        :return: value if found
-        """
-        return self._values[key]
-
-    def __iter__(self) -> Iterator[T]:
-        """Return a list-like iterator on the container values.
-
-        :return:
-        :yield: a contained value
-        """
-        return iter(self._values.values())
-
-    @property
-    def at(self) -> List[T]:
-        """Return container as a list.
-
-        :return:
-        """
-        return list(self)
-
-    def keys(self) -> KeysView[Any]:
-        """Return container keys.
-
-        :return:
-        :yield: key
-        """
-        return self._values.keys()
-
-    def values(self) -> ValuesView[T]:
-        """Return container values.
-
-        :return:
-        :yield: value
-        """
-        return self._values.values()
-
-    def items(self) -> ItemsView[Any, T]:
-        """Return container items as (key, value) pairs.
-
-        :return:
-        """
-        return self._values.items()
-
-    def to_dict(self) -> Dict[Any, T]:
-        """Return a copy of internal container dictionary.
-
-        :return:
-        """
-        return self._values.copy()
```

### Comparing `mcda-0.5.0/mcda/mavt/aggregators.py` & `mcda-0.5.1/mcda/mavt/aggregators.py`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda/mavt/uta.py` & `mcda-0.5.1/mcda/mavt/uta.py`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda/outranking/electre.py` & `mcda-0.5.1/mcda/outranking/electre.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Generic, List, Set, Tuple, TypeVar, cast
 
 from pandas import DataFrame, Series
 
 from ..core.categories import BoundedCategoryProfile
 from ..core.interfaces import Assignator, Ranker, Selector
-from ..core.matrices import AdjacencyMatrix, ProfileAlternativeMatrix
+from ..core.matrices import AdjacencyMatrix
 from ..core.performance_table import PerformanceTable
 from ..core.relations import (
     IncomparableRelation,
     IndifferenceRelation,
     OutrankingMatrix,
     PreferenceRelation,
     Relation,
@@ -68,15 +68,15 @@
     @abstractmethod
     def exploit(
         self, outranking_structure: T, **kwargs
     ) -> Any:  # pragma: nocover
         pass
 
 
-class BaseElectre1(ABC):
+class _BaseElectre1(ABC):
     """This class implements common methods for Electre I and II.
 
     :param criteria_weights:
     """
 
     def __init__(self, criteria_weights: Dict[Any, float]):
         self.criteria_weights = criteria_weights
@@ -195,15 +195,15 @@
                 index=performance_table.alternatives,
                 columns=performance_table.alternatives,
             )
             / max(performance_table.data.apply(lambda x: max(x) - min(x)))
         )
 
 
-class Electre1(BaseElectre1, IElectre[OutrankingMatrix], Selector):
+class Electre1(_BaseElectre1, IElectre[OutrankingMatrix], Selector):
     """This class implements the Electre I algorithm.
 
     :param criteria_weights:
     :param c_hat: concordance threshold
     :param d_hat: discordance threshold
     """
 
@@ -308,15 +308,15 @@
         matrix = self.construct(performance_table)
         return self.exploit(
             matrix, cycle_reduction=cycle_reduction, transitivity=transitivity
         )
 
 
 class Electre2(
-    BaseElectre1, IElectre[Tuple[OutrankingMatrix, OutrankingMatrix]], Ranker
+    _BaseElectre1, IElectre[Tuple[OutrankingMatrix, OutrankingMatrix]], Ranker
 ):
     """This class implements the Electre II algorithm.
 
     :param criteria_weights:
     :param c_hat: concordance thresholds (min, max)
     :param d_hat: discordance threshold (min, max)
     """
@@ -452,15 +452,15 @@
 
         :param performance_table:
         :return: result outranking matrix
         """
         return self.exploit(self.construct(performance_table))
 
 
-class BaseElectre3(ABC):
+class _BaseElectre3(ABC):
     """This class implements basic Electre III methods shared to other classes.
 
     :param criteria_weights:
     :param preference_thresholds:
     :param indifference_thresholds:
     :param veto_thresholds:
     """
@@ -716,15 +716,15 @@
                 ]
                 for i in performance_table.alternatives
             ],
             vertices=performance_table.alternatives,
         )
 
 
-class Electre3(BaseElectre3, IElectre[AdjacencyMatrix], Ranker):
+class Electre3(_BaseElectre3, IElectre[AdjacencyMatrix], Ranker):
     """This class implements the Electre III algorithm.
 
     :param criteria_weights:
     :param preference_thresholds:
     :param indifference_thresholds:
     :param veto_thresholds:
     :param alpha:  preset up values of distillation coefficients
@@ -857,15 +857,15 @@
 
         :param performance_table:
         :return: final outranking matrix
         """
         return self.exploit(self.construct(performance_table))
 
 
-class ElectreTri(BaseElectre3, IElectre[ProfileAlternativeMatrix], Assignator):
+class ElectreTri(_BaseElectre3, IElectre[AdjacencyMatrix], Assignator):
     """This class implements the Electre-Tri B algorithm.
 
     :param criteria_weights:
     :param profiles: profiles in ascending dominance order
     :param preference_thresholds:
     :param indifference_thresholds:
     :param veto_thresholds:
@@ -913,73 +913,66 @@
             zip(
                 categories,
                 BoundedCategoryProfile.profiles_partition(self.profiles),
             )
         )
         self.lambda_ = lambda_
 
-    def credibility(
+    def construct(
         self, performance_table: PerformanceTable
-    ) -> ProfileAlternativeMatrix:
-        """Return credibility matrix.
+    ) -> AdjacencyMatrix:
+        """Construct alternatives and profiles credibility matrix.
 
         Returned credibility matrix concatenates `performance_table`
         and :attr:`profiles` (in that order).
 
         :param performance_table:
         :return:
-
-        .. note::
-            uses :meth:`Electre3.construct` implementation
+        :raise IndexError: if profiles and alternatives share some labels
         """
-        # Concatenate performance table and category profile
-        # Replace indexes so no chance of same id category profile alternative
-        altered_performance_table = PerformanceTable(
-            performance_table.data.values.tolist()
-            + self.profiles.data[performance_table.criteria].values.tolist(),
-            criteria=performance_table.criteria,
-        )
-        matrix = BaseElectre3.credibility(self, altered_performance_table)
-        return ProfileAlternativeMatrix(
-            matrix.data.values,
-            alternatives=performance_table.alternatives,
-            profiles=self.profiles.alternatives,
+        common_labels = set(performance_table.alternatives).intersection(
+            set(self.profiles.alternatives)
         )
+        if len(common_labels) != 0:
+            raise IndexError(
+                "profiles and alternatives must have different labels. "
+                f"Common labels: {common_labels}"
+            )
 
-    def construct(
-        self, performance_table: PerformanceTable
-    ) -> ProfileAlternativeMatrix:
-        """Construct outranking structure which is the credibility matrix.
+        # Transform profiles to performance table scales
+        _profiles = self.profiles.transform(performance_table.scales)
 
-        :param performance_table:
-        :return: credibility matrix
-        """
-        return self.credibility(performance_table)
+        # Concatenate performance table and category profiles
+        altered_performance_table = PerformanceTable.concat(
+            [performance_table, _profiles], axis=0
+        )
+
+        return self.credibility(altered_performance_table)
 
     def _pairwise_outrank(
         self,
-        credibility_mat: ProfileAlternativeMatrix,
-        label1: Tuple[Any, Any],
-        label2: Tuple[Any, Any],
+        credibility_mat: AdjacencyMatrix,
+        label1: Any,
+        label2: Any,
     ) -> bool:
         """Check whether first label outranks second.
 
         :param credibility_mat:
         :param label1:
         :param label2:
         :return: ``True`` if `label1` outranks `label2`, ``False`` otherwise
         """
         aSb = cast(float, credibility_mat.data.at[label1, label2])
         return aSb >= self.lambda_
 
     def _pairwise_relation(
         self,
-        credibility_mat: ProfileAlternativeMatrix,
-        label1: Tuple[Any, Any],
-        label2: Tuple[Any, Any],
+        credibility_mat: AdjacencyMatrix,
+        label1: Any,
+        label2: Any,
     ) -> Relation:
         """Compute relation between two actions based on credibility matrix.
 
         :param credibility_mat:
             credibility matrix of concatenated performance table / profiles
         :param label1:
         :param label2:
@@ -992,87 +985,93 @@
         elif aSb >= self.lambda_ > bSa:
             return PreferenceRelation(label1, label2)
         elif aSb < self.lambda_ <= bSa:
             return PreferenceRelation(label2, label1)
         return IncomparableRelation(label1, label2)
 
     def _exploit_pessimistic(
-        self, outranking_structure: ProfileAlternativeMatrix
+        self, outranking_structure: AdjacencyMatrix
     ) -> Dict[Any, Set]:
         """Compute the exploitation procedure pessimistically.
 
         :param outranking_structure: credibility matrix
         :return: categories
         """
-        rest = set(outranking_structure.alternatives)
+        rest = set(outranking_structure.vertices) - set(
+            self.profiles.alternatives
+        )
         categories = list(self.category_profiles.keys())
         classes: Dict[Any, Set] = {category: set() for category in categories}
         for cat, cat_profile in reversed(
             list(self.category_profiles.items())[1:]
         ):
             assigned = set()
             for a in rest:
                 if self._pairwise_outrank(
                     outranking_structure,
-                    outranking_structure.alternative_index(a),
-                    outranking_structure.profile_index(
-                        cast(ScaleValues, cat_profile.lower).name
-                    ),
+                    a,
+                    cast(ScaleValues, cat_profile.lower).name,
                 ):
                     classes[cat].add(a)
                     assigned.add(a)
             rest -= assigned
         classes[categories[0]] = rest
         return classes
 
     def _exploit_optimistic(
-        self, outranking_structure: ProfileAlternativeMatrix
+        self, outranking_structure: AdjacencyMatrix
     ) -> Dict[Any, Set]:
         """Compute the exploitation procedure optimistically.
 
         :param outranking_structure: credibility matrix
         :return: categories
         """
-        rest = set(outranking_structure.alternatives)
+        rest = set(outranking_structure.vertices) - set(
+            self.profiles.alternatives
+        )
         categories = list(self.category_profiles.keys())
         classes: Dict[Any, Set] = {}
         for cat, cat_profile in list(self.category_profiles.items())[:-1]:
             assigned = set()
             profile = cast(ScaleValues, cat_profile.upper).name
             for a in rest:
                 pref = PreferenceRelation(
-                    outranking_structure.profile_index(profile),
-                    outranking_structure.alternative_index(a),
+                    profile,
+                    a,
                 )
                 if (
                     self._pairwise_relation(
                         outranking_structure,
-                        outranking_structure.profile_index(profile),
-                        outranking_structure.alternative_index(a),
+                        profile,
+                        a,
                     )
                     == pref
                 ):
                     assigned.add(a)
             classes[cat] = assigned
             rest -= assigned
         classes[categories[-1]] = rest
         return classes
 
     def exploit(
         self,
-        outranking_structure: ProfileAlternativeMatrix,
+        outranking_structure: AdjacencyMatrix,
         pessimistic: bool = False,
         **kwargs,
     ) -> Dict[Any, Set]:
         """Compute the exploitation procedure (either optimistically or
         pessimistically).
 
         :param outranking_structure: credibility matrix
         :param pessimistic: if ``True`` performs procedure pessimistically
-        :return: categories
+        :return: categories in ascending domination order
+
+        .. note::
+            the category profiles defining the categories are the ones from
+            :attr:`category_profiles`
         """
         return (
             self._exploit_pessimistic(outranking_structure)
             if pessimistic
             else self._exploit_optimistic(outranking_structure)
         )
 
@@ -1081,17 +1080,19 @@
         performance_table: PerformanceTable,
         pessimistic: bool = False,
         **kwargs,
     ) -> Dict[Any, Set]:
         """Compute the exploitation procedure (either optimistically or
         pessimistically).
 
-        In the output ranking, class -1 means incomparable class
-
         :param performance_table:
         :param pessimistic:
-        :return: categories
+        :return: categories in ascending domination order
+
+        .. note::
+            the category profiles defining the categories are the ones from
+            :attr:`category_profiles`
         """
         return self.exploit(
             self.construct(performance_table=performance_table),
             pessimistic=pessimistic,
         )
```

### Comparing `mcda-0.5.0/mcda/outranking/promethee.py` & `mcda-0.5.1/mcda/outranking/promethee.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Any, Dict, List, cast
 
 import matplotlib.pyplot as plt
 from pandas import DataFrame, Series
 from sklearn.decomposition import PCA
 
 from ..core.interfaces import Ranker
-from ..core.matrices import AdjacencyMatrix, ProfileAlternativeMatrix
+from ..core.matrices import AdjacencyMatrix
 from ..core.performance_table import PerformanceTable
 from ..core.relations import (
     IncomparableRelation,
     IndifferenceRelation,
     PreferenceRelation,
     PreferenceStructure,
     Relation,
@@ -215,65 +215,37 @@
             alternative_values1.transform(scales).data
             - alternative_values2.transform(scales).data
         )
         return Series(
             {c: self.preference_functions[c](v) for c, v in diffs.items()}
         )
 
-    def _partial_preferences(
+    def partial_preferences(
         self,
         performance_table: PerformanceTable,
-    ) -> DataFrame:
+    ) -> AdjacencyMatrix:
         """Compute partial preferences for each alternatives' pair.
 
         :param performance_table:
-        :return: matrix of pairwise partial preferences
+        :return: matrix of partial preferences
         """
-        return DataFrame(
+        return AdjacencyMatrix(
             [
                 [
                     self._pairwise_partial_preference(
                         performance_table.alternatives_values[ai],
                         performance_table.alternatives_values[aj],
                     )
                     for aj in performance_table.alternatives
                 ]
                 for ai in performance_table.alternatives
             ],
-            index=performance_table.alternatives,
-            columns=performance_table.alternatives,
+            vertices=performance_table.alternatives,
         )
 
-    def partial_preferences(
-        self,
-        performance_table: PerformanceTable,
-        profiles: PerformanceTable = None,
-    ) -> AdjacencyMatrix:
-        """Compute partial preferences for each
-        alternative/profile or alternative/alternative pair.
-
-        :param performance_table:
-        :param profiles:
-        :return: matrix of partial preferences
-        """
-        if profiles:
-            updated_table = PerformanceTable(
-                performance_table.data.values.tolist()
-                + profiles.data.values.tolist(),
-                criteria=performance_table.criteria,
-                scales=performance_table.scales,
-            )
-            prefs = self._partial_preferences(updated_table)
-            return ProfileAlternativeMatrix(
-                prefs.values.tolist(),
-                alternatives=performance_table.alternatives,
-                profiles=profiles.alternatives,
-            )
-        return AdjacencyMatrix(self._partial_preferences(performance_table))
-
 
 class GeneralizedCriteriaAggregator(ABC):
     """This abstract class defines the methods implemented by aggregators of
     generalized criteria.
     """
 
     @abstractmethod
@@ -463,49 +435,59 @@
 
         :param preferences:
         :return: computed flows
         """
         pass
 
 
-def positive_flows(preferences: AdjacencyMatrix) -> Series:
+def positive_flows(
+    preferences: AdjacencyMatrix, profiles: List = None
+) -> Series:
     """Compute positive flows.
 
     :param preferences:
+    :param profiles:
     :return: computed positive flows
 
     .. note::
-        this function accept both alternative/alternative and
-        alternative/profile preferences
+        if `profiles` is not ``None``, it will returns alternatives
+        vs profiles positive flows
     """
-    if isinstance(preferences, ProfileAlternativeMatrix):
-        data = preferences.submatrix(
-            preferences.ALTERNATIVES, preferences.PROFILES
-        ).data
-    else:
+    if profiles is None:
         data = preferences.data
+    else:
+        alternatives = sorted(
+            set(preferences.vertices) - set(profiles),
+            key=lambda a: preferences.vertices.index(a),
+        )
+        data = preferences.data.loc[alternatives, profiles]
     return data.sum(axis=1)
 
 
-def negative_flows(preferences: AdjacencyMatrix) -> Series:
+def negative_flows(
+    preferences: AdjacencyMatrix, profiles: List = None
+) -> Series:
     """Compute negative flows.
 
     :param preferences:
+    :param profiles:
     :return: computed negative flows
 
     .. note::
-        this function accept both alternative/alternative and
-        alternative/profile preferences
+        if `profiles` is not ``None``, it will returns profiles
+        vs alternatives negative flows
     """
-    if isinstance(preferences, ProfileAlternativeMatrix):
-        data = preferences.submatrix(
-            preferences.PROFILES, preferences.ALTERNATIVES
-        ).data
-    else:
+    if profiles is None:
         data = preferences.data
+    else:
+        alternatives = sorted(
+            set(preferences.vertices) - set(profiles),
+            key=lambda a: preferences.vertices.index(a),
+        )
+        data = preferences.data.loc[profiles, alternatives]
     return data.sum(axis=0)
 
 
 class OutrankingFlows(Flows):
     """This class defines a basic outranking flows computer able to return
     either positive or negative flows.
     """
@@ -518,36 +500,30 @@
     ) -> Series:
         """Compute outranking flows.
 
         :param preferences:
         :param negative:
             if ``True``, returns the negative flows, positive ones otherwise
         :return: outranking flows
-
-        .. note::
-            this method accept both alternative/alternative and
-            alternative/profile preferences
         """
         return (
             negative_flows(preferences)
             if negative
             else positive_flows(preferences)
         )
 
 
 class NetOutrankingFlows(Flows):
+    """This class defines a net outranking flows computer."""
+
     def flows(self, preferences: AdjacencyMatrix, **kwargs) -> Series:
         """Compute net outranking flows.
 
         :param preferences:
         :return: net outranking flows
-
-        .. note::
-            this method accept both alternative/alternative and
-            alternative/profile preferences
         """
         return positive_flows(preferences) - negative_flows(preferences)
 
 
 """
 class NetFlowAggregatorType(Enum):
     MAX = np.nanmax
```

### Comparing `mcda-0.5.0/mcda/outranking/srmp.py` & `mcda-0.5.1/mcda/outranking/srmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,23 +75,24 @@
         self, performance_table: PerformanceTable
     ) -> OutrankingMatrix:
         """Construct the outranking matrix.
 
         :param performance_table:
         :return:
         """
+        _profile = self.profile.transform(performance_table.scales)
         functions = CriteriaFunctions(
             {
                 criterion: (
                     cast(
                         Function,
                         lambda x, c=criterion: self.criteria_weights[c]
                         if is_better_or_equal(
                             x,
-                            self.profile.data[c],
+                            _profile.data[c],
                             cast(
                                 QuantitativeScale, performance_table.scales[c]
                             ),
                         )
                         else 0,
                     )
                 )  # https://bugs.python.org/issue13652
```

### Comparing `mcda-0.5.0/mcda/plot/plot.py` & `mcda-0.5.1/mcda/plot/plot.py`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/mcda.egg-info/PKG-INFO` & `mcda-0.5.1/mcda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mcda
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package for Multi Criteria Decision Analysis
 Author: Nicolas Duminy
 Author-email: nicolas.duminy@imt-atlantique.fr
 Project-URL: Source, https://gitlab.com/decide.imt-atlantique/pymcda
 Project-URL: Documentation, https://py-mcda.readthedocs.io
 Project-URL: Tracker, https://gitlab.com/decide.imt-atlantique/pymcda/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
 
 
 # Package description
```

### Comparing `mcda-0.5.0/mcda.egg-info/SOURCES.txt` & `mcda-0.5.1/mcda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcda-0.5.0/setup.py` & `mcda-0.5.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
 setup(
     name="mcda",
-    version="0.5.0",
+    version="0.5.1",
     author="Nicolas Duminy",
     author_email="nicolas.duminy@imt-atlantique.fr",
     description="Package for Multi Criteria Decision Analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "Source": "https://gitlab.com/decide.imt-atlantique/pymcda",
@@ -37,10 +37,10 @@
         "matplotlib",
         "pulp",
         "graphviz",
         "scikit-learn",
         "pandas",
         "Deprecated",
     ),
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     zip_safe=False,
 )
```

