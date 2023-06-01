# Comparing `tmp/speasy-1.1.1.tar.gz` & `tmp/speasy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speasy-1.1.1.tar", last modified: Thu Apr  6 12:46:52 2023, max compression
+gzip compressed data, was "speasy-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `speasy-1.1.1.tar` & `speasy-1.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1660 2023-04-06 12:46:34.652600 speasy-1.1.1/LICENSE
--rw-r--r--   0        0        0     5850 2023-04-06 12:46:34.652600 speasy-1.1.1/README.rst
--rw-r--r--   0        0        0     1359 2023-04-06 12:46:34.696601 speasy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      920 2023-04-06 12:46:34.696601 speasy-1.1.1/speasy/__init__.py
--rw-r--r--   0        0        0     7468 2023-04-06 12:46:34.696601 speasy-1.1.1/speasy/config/__init__.py
--rw-r--r--   0        0        0     6567 2023-04-06 12:46:34.696601 speasy-1.1.1/speasy/core/__init__.py
--rw-r--r--   0        0        0      533 2023-04-06 12:46:34.696601 speasy-1.1.1/speasy/core/cache/__init__.py
--rw-r--r--   0        0        0     2061 2023-04-06 12:46:34.696601 speasy-1.1.1/speasy/core/cache/_function_cache.py
--rw-r--r--   0        0        0      100 2023-04-06 12:46:34.696601 speasy-1.1.1/speasy/core/cache/_instance.py
--rw-r--r--   0        0        0    14306 2023-04-06 12:46:34.696601 speasy-1.1.1/speasy/core/cache/_providers_caches.py
--rw-r--r--   0        0        0     2386 2023-04-06 12:46:34.696601 speasy-1.1.1/speasy/core/cache/cache.py
--rw-r--r--   0        0        0     1941 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/cache/version.py
--rw-r--r--   0        0        0     2010 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/cdf/__init__.py
--rw-r--r--   0        0        0     8835 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/data_containers.py
--rw-r--r--   0        0        0     4616 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/dataprovider.py
--rw-r--r--   0        0        0     2204 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/datetime_range.py
--rw-r--r--   0        0        0     3586 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/http.py
--rw-r--r--   0        0        0       80 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/index/__init__.py
--rw-r--r--   0        0        0      525 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/index/speasy_index.py
--rw-r--r--   0        0        0     1871 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/inventory/__init__.py
--rw-r--r--   0        0        0     4637 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/inventory/indexes.py
--rw-r--r--   0        0        0     4928 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/proxy/__init__.py
--rw-r--r--   0        0        0       92 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/requests_scheduling/__init__.py
--rw-r--r--   0        0        0    11374 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/requests_scheduling/request_dispatch.py
--rw-r--r--   0        0        0     1089 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/requests_scheduling/split_large_requests.py
--rw-r--r--   0        0        0     3500 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/core/span_utils.py
--rw-r--r--   0        0        0      165 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/inventories/__init__.py
--rw-r--r--   0        0        0     2867 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/plotting/__init__.py
--rw-r--r--   0        0        0     2165 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/plotting/mpl_backend/__init__.py
--rw-r--r--   0        0        0      686 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/products/__init__.py
--rw-r--r--   0        0        0      241 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/products/base_product.py
--rw-r--r--   0        0        0     4582 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/products/catalog.py
--rw-r--r--   0        0        0     1654 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/products/dataset.py
--rw-r--r--   0        0        0     1696 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/products/timetable.py
--rw-r--r--   0        0        0    18641 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/products/variable.py
--rw-r--r--   0        0        0      130 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/__init__.py
--rw-r--r--   0        0        0     1729 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/amda/__init__.py
--rw-r--r--   0        0        0     9131 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/amda/_impl.py
--rw-r--r--   0        0        0       46 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/amda/exceptions.py
--rw-r--r--   0        0        0     6034 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/amda/inventory.py
--rw-r--r--   0        0        0    11428 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/amda/rest_client.py
--rw-r--r--   0        0        0     6833 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/amda/utils.py
--rw-r--r--   0        0        0    22336 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/amda/ws.py
--rw-r--r--   0        0        0     6844 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/cda/__init__.py
--rw-r--r--   0        0        0     2939 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/cda/_inventory_builder/__init__.py
--rw-r--r--   0        0        0     2533 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/cda/_inventory_builder/_cdf_masters_parser.py
--rw-r--r--   0        0        0     3456 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/cda/_inventory_builder/_xml_catalogs_parser.py
--rw-r--r--   0        0        0    10011 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/csa/__init__.py
--rw-r--r--   0        0        0     5777 2023-04-06 12:46:34.700601 speasy-1.1.1/speasy/webservices/ssc/__init__.py
--rw-r--r--   0        0        0     7212 1970-01-01 00:00:00.000000 speasy-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1660 2023-06-01 15:43:40.883456 speasy-1.1.2/LICENSE
+-rw-r--r--   0        0        0     5235 2023-06-01 15:43:40.883456 speasy-1.1.2/README.md
+-rw-r--r--   0        0        0     1358 2023-06-01 15:43:40.931457 speasy-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      920 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/__init__.py
+-rw-r--r--   0        0        0     7468 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/config/__init__.py
+-rw-r--r--   0        0        0     6567 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/__init__.py
+-rw-r--r--   0        0        0      533 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/cache/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/cache/_function_cache.py
+-rw-r--r--   0        0        0      100 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/cache/_instance.py
+-rw-r--r--   0        0        0    14306 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/cache/_providers_caches.py
+-rw-r--r--   0        0        0     2386 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/cache/cache.py
+-rw-r--r--   0        0        0     1941 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/cache/version.py
+-rw-r--r--   0        0        0     2497 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/cdf/__init__.py
+-rw-r--r--   0        0        0     8835 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/data_containers.py
+-rw-r--r--   0        0        0     4616 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/dataprovider.py
+-rw-r--r--   0        0        0     2204 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/datetime_range.py
+-rw-r--r--   0        0        0     3586 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/http.py
+-rw-r--r--   0        0        0       80 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/index/__init__.py
+-rw-r--r--   0        0        0      525 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/index/speasy_index.py
+-rw-r--r--   0        0        0     1871 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/inventory/__init__.py
+-rw-r--r--   0        0        0     4959 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/inventory/indexes.py
+-rw-r--r--   0        0        0     4928 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/proxy/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-01 15:43:40.931457 speasy-1.1.2/speasy/core/requests_scheduling/__init__.py
+-rw-r--r--   0        0        0    11374 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/core/requests_scheduling/request_dispatch.py
+-rw-r--r--   0        0        0     1175 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/core/requests_scheduling/split_large_requests.py
+-rw-r--r--   0        0        0     3500 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/core/span_utils.py
+-rw-r--r--   0        0        0      165 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/inventories/__init__.py
+-rw-r--r--   0        0        0     2867 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/plotting/__init__.py
+-rw-r--r--   0        0        0     2165 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/plotting/mpl_backend/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/products/__init__.py
+-rw-r--r--   0        0        0      241 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/products/base_product.py
+-rw-r--r--   0        0        0     4582 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/products/catalog.py
+-rw-r--r--   0        0        0     1654 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/products/dataset.py
+-rw-r--r--   0        0        0     1696 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/products/timetable.py
+-rw-r--r--   0        0        0    18641 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/products/variable.py
+-rw-r--r--   0        0        0      130 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/amda/__init__.py
+-rw-r--r--   0        0        0     9145 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/amda/_impl.py
+-rw-r--r--   0        0        0       46 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/amda/exceptions.py
+-rw-r--r--   0        0        0     6034 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/amda/inventory.py
+-rw-r--r--   0        0        0    11428 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/amda/rest_client.py
+-rw-r--r--   0        0        0     7678 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/amda/utils.py
+-rw-r--r--   0        0        0    22336 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/amda/ws.py
+-rw-r--r--   0        0        0     7327 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/cda/__init__.py
+-rw-r--r--   0        0        0     2939 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/cda/_inventory_builder/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/cda/_inventory_builder/_cdf_masters_parser.py
+-rw-r--r--   0        0        0     3456 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/cda/_inventory_builder/_xml_catalogs_parser.py
+-rw-r--r--   0        0        0    10015 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/csa/__init__.py
+-rw-r--r--   0        0        0     5741 2023-06-01 15:43:40.935457 speasy-1.1.2/speasy/webservices/ssc/__init__.py
+-rw-r--r--   0        0        0     6600 1970-01-01 00:00:00.000000 speasy-1.1.2/PKG-INFO
```

### Comparing `speasy-1.1.1/LICENSE` & `speasy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/pyproject.toml` & `speasy-1.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core"]
 
 [project]
 name = 'speasy'
-version = "1.1.1"
+version = "1.1.2"
 description = "A simple Python package to deal with main Space Physics WebServices (CDA, CSA, AMDA and SSC)."
 keywords= ["satellite", "plasma-physics", "nasa-data", "amda", "cdpp", "CDF"]
 authors = [
   {name = "Alexis Jeandet", email = "alexis.jeandet@member.fsf.org" }
 ]
 
 maintainers = [
   {name = "Alexis Jeandet", email = "alexis.jeandet@member.fsf.org" }
 ]
 
 requires-python=">=3.7"
 license = {file="LICENSE"}
-readme = "README.rst"
+readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
```

### Comparing `speasy-1.1.1/speasy/__init__.py` & `speasy-1.1.2/speasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
    import speasy as spz
 
 """
 
 __author__ = """Alexis Jeandet"""
 __email__ = 'alexis.jeandet@member.fsf.org'
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 __all__ = ['amda', 'cda', 'ssc', 'csa', 'get_data', 'SpeasyVariable', 'Catalog', 'Event', 'Dataset', 'TimeTable']
 __docformat__ = "numpy"
 
 from speasy.core.inventory.indexes import SpeasyIndex
 from .products import SpeasyVariable, Catalog, Event, Dataset, TimeTable, MaybeAnyProduct
 from typing import List
 from .core.requests_scheduling.request_dispatch import get_data, list_providers, amda, cda, csa, ssc
```

### Comparing `speasy-1.1.1/speasy/config/__init__.py` & `speasy-1.1.2/speasy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/__init__.py` & `speasy-1.1.2/speasy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/cache/__init__.py` & `speasy-1.1.2/speasy/core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/cache/_function_cache.py` & `speasy-1.1.2/speasy/core/cache/_function_cache.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/cache/_providers_caches.py` & `speasy-1.1.2/speasy/core/cache/_providers_caches.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/cache/cache.py` & `speasy-1.1.2/speasy/core/cache/cache.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/cache/version.py` & `speasy-1.1.2/speasy/core/cache/version.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/cdf/__init__.py` & `speasy-1.1.2/speasy/core/cdf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pyistp
+
 from ...products import SpeasyVariable, VariableAxis, VariableTimeAxis, DataContainer
 
 
 def _fix_value_type(value):
     if type(value) in (str, int, float):
         return value
     if type(value) is list:
@@ -22,14 +23,24 @@
         is_time_dependent = True
     else:
         is_time_dependent = False
     return VariableAxis(values=axis.values.copy(), meta=_fix_attributes_types(axis.attributes), name=axis.name,
                         is_time_dependent=is_time_dependent)
 
 
+def _build_labels(variable: pyistp.loader.DataVariable):
+    if len(variable.values.shape) != 2:
+        return variable.labels
+    if type(variable.labels) is list and len(variable.labels) == variable.values.shape[1]:
+        return variable.labels
+    if type(variable.labels) is list and len(variable.labels) == 1:
+        return [f"{variable.labels[0]}[{i}]" for i in range(variable.values.shape[1])]
+    return [f"component_{i}" for i in range(variable.values.shape[1])]
+
+
 def load_variable(variable="", file=None, buffer=None) -> SpeasyVariable or None:
     istp = pyistp.load(file=file, buffer=buffer)
     if istp:
         if variable in istp.data_variables():
             var = istp.data_variable(variable)
         elif variable.replace('-', '_') in istp.data_variables():  # THX CSA/ISTP
             var = istp.data_variable(variable.replace('-', '_'))
@@ -42,9 +53,9 @@
             return SpeasyVariable(
                 axes=[VariableTimeAxis(values=var.axes[0].values.copy(),
                                        meta=_fix_attributes_types(var.axes[0].attributes))] + [
                          _make_axis(axis, time_axis_name) for axis in var.axes[1:]],
                 values=DataContainer(values=var.values.copy(), meta=_fix_attributes_types(var.attributes),
                                      name=var.name,
                                      is_time_dependent=True),
-                columns=var.labels)
+                columns=_build_labels(var))
     return None
```

### Comparing `speasy-1.1.1/speasy/core/data_containers.py` & `speasy-1.1.2/speasy/core/data_containers.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/dataprovider.py` & `speasy-1.1.2/speasy/core/dataprovider.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/datetime_range.py` & `speasy-1.1.2/speasy/core/datetime_range.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/http.py` & `speasy-1.1.2/speasy/core/http.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/index/speasy_index.py` & `speasy-1.1.2/speasy/core/index/speasy_index.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/inventory/__init__.py` & `speasy-1.1.2/speasy/core/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/inventory/indexes.py` & `speasy-1.1.2/speasy/core/inventory/indexes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Optional
 import json
+from typing import Optional
 
 __INDEXES_TYPES__ = {}
 
 
 class SpeasyIndex:
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
@@ -74,32 +74,40 @@
         return f'<ParameterIndex: {self.spz_name()}>'
 
     def __iter__(self):
         return [v for v in self.__dict__.values() if type(v) is ComponentIndex].__iter__()
 
     def __contains__(self, item: str or ComponentIndex):
         if type(item) is ComponentIndex:
-            item = item.name()
-        return item in self.__dict__
+            item = item.spz_uid()
+        for member in self.__dict__.values():
+            if isinstance(member, ComponentIndex):
+                if member.spz_uid() == item:
+                    return True
+        return False
 
 
 class DatasetIndex(SpeasyIndex):
     def __init__(self, name: str, provider: str, uid: str, meta: Optional[dict] = None):
         super().__init__(name, provider, uid, meta)
 
     def __repr__(self):
         return f'<DatasetIndex: {self.spz_name()}>'
 
     def __iter__(self):
         return [v for v in self.__dict__.values() if type(v) is ParameterIndex].__iter__()
 
     def __contains__(self, item: str or ParameterIndex):
         if type(item) is ParameterIndex:
-            item = item.name()
-        return item in self.__dict__
+            item = item.spz_uid()
+        for member in self.__dict__.values():
+            if isinstance(member, ParameterIndex):
+                if member.spz_uid() == item:
+                    return True
+        return False
 
 
 def to_dict(inventory_tree: SpeasyIndex or str):
     if isinstance(inventory_tree, SpeasyIndex):
         return {key: to_dict(value) for key, value in inventory_tree.__dict__.items()}
     elif type(inventory_tree) is not str:
         return str(inventory_tree)
```

### Comparing `speasy-1.1.1/speasy/core/proxy/__init__.py` & `speasy-1.1.2/speasy/core/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/requests_scheduling/request_dispatch.py` & `speasy-1.1.2/speasy/core/requests_scheduling/request_dispatch.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/core/requests_scheduling/split_large_requests.py` & `speasy-1.1.2/speasy/core/requests_scheduling/split_large_requests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from typing import Callable
-from speasy.core.datetime_range import DateTimeRange
 from datetime import timedelta
 from functools import wraps
+from typing import Callable
+
+from speasy.core.datetime_range import DateTimeRange
+from speasy.core.inventory.indexes import ParameterIndex
 from speasy.products.variable import merge as var_merge
 
 
 class SplitLargeRequests(object):
-    def __init__(self, threshold: Callable[[], timedelta]):
+    def __init__(self, threshold: Callable[[ParameterIndex or str], timedelta]):
         self.threshold = threshold
 
     def __call__(self, get_data: Callable):
         @wraps(get_data)
         def wrapped(wrapped_self, product, start_time, stop_time, **kwargs):
             range = DateTimeRange(start_time, stop_time)
             duration = range.duration
-            max_range_per_request = self.threshold()
+            max_range_per_request = self.threshold(product)
             if duration <= max_range_per_request:
                 return get_data(wrapped_self, product=product, start_time=start_time, stop_time=stop_time, **kwargs)
             else:
                 fragments = range.split(max_range_per_request)
                 return var_merge(
                     [get_data(wrapped_self, product=product, start_time=r.start_time, stop_time=r.stop_time, **kwargs)
                      for r in fragments])
```

### Comparing `speasy-1.1.1/speasy/core/span_utils.py` & `speasy-1.1.2/speasy/core/span_utils.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/plotting/__init__.py` & `speasy-1.1.2/speasy/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/plotting/mpl_backend/__init__.py` & `speasy-1.1.2/speasy/plotting/mpl_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/products/__init__.py` & `speasy-1.1.2/speasy/products/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/products/catalog.py` & `speasy-1.1.2/speasy/products/catalog.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/products/dataset.py` & `speasy-1.1.2/speasy/products/dataset.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/products/timetable.py` & `speasy-1.1.2/speasy/products/timetable.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/products/variable.py` & `speasy-1.1.2/speasy/products/variable.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/webservices/amda/__init__.py` & `speasy-1.1.2/speasy/webservices/amda/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/webservices/amda/_impl.py` & `speasy-1.1.2/speasy/webservices/amda/_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from datetime import datetime, timedelta
 from types import SimpleNamespace
 from typing import Dict, Optional
 
+from . import rest_client
+from .exceptions import MissingCredentials
+from .inventory import AmdaXMLParser
+from .rest_client import auth_args
+from .utils import load_catalog, load_csv, load_timetable
 # General modules
 from ...config import amda as amda_cfg
 from ...core.cache import CacheCall
+from ...core.cdf import load_variable as load_cdf
 from ...core.http import urlopen_with_retry
 from ...core.inventory.indexes import SpeasyIndex
-from ...core.cdf import load_variable as load_cdf
 from ...inventories import flat_inventories
 from ...products.variable import SpeasyVariable, merge
-from . import rest_client
-from .exceptions import MissingCredentials
-from .inventory import AmdaXMLParser
-from .rest_client import auth_args
-from .utils import load_catalog, load_csv, load_timetable
 
 log = logging.getLogger(__name__)
 
 
 def credential_are_valid():
     login = amda_cfg.username()
     password = amda_cfg.password()
@@ -102,15 +102,15 @@
         # check status until done
         if url is not None:
             if output_format == "CDF_ISTP":
                 if url is not None:
                     with urlopen_with_retry(url) as remote_cdf:
                         var = load_cdf(buffer=remote_cdf.read(), variable=parameter_id)
             else:
-                var = load_csv(url)
+                var = load_csv(url, parameter_id)
             if len(var):
                 log.debug(
                     f'Loaded var: data shape = {var.values.shape}, data start time = {var.time[0]}, \
                             data stop time = {var.time[-1]}')
             else:
                 log.debug('Loaded var: Empty var')
             return var
```

### Comparing `speasy-1.1.1/speasy/webservices/amda/inventory.py` & `speasy-1.1.2/speasy/webservices/amda/inventory.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/webservices/amda/rest_client.py` & `speasy-1.1.2/speasy/webservices/amda/rest_client.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/webservices/amda/utils.py` & `speasy-1.1.2/speasy/webservices/amda/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """AMDA_Webservice utility functions. This module defines some conversion functions specific to AMDA_Webservice, mainly
 conversion procedures for parsing CSV and VOTable data.
 
 """
 import datetime
 import logging
 import os
+import re
 import tempfile
 from typing import Dict, List
 
 import numpy as np
 import pandas as pds
-
+from speasy.config import amda as amda_cfg
 from speasy.core import epoch_to_datetime64
 from speasy.core.datetime_range import DateTimeRange
 from speasy.core.http import urlopen_with_retry
 from speasy.products.catalog import Catalog, Event
 from speasy.products.timetable import TimeTable
 from speasy.products.variable import (DataContainer, SpeasyVariable,
                                       VariableAxis, VariableTimeAxis)
@@ -42,15 +43,41 @@
         if content_length:
             percent = int((size / content_length) * 100)
             log.debug(f"Download data: {percent}%")
     fd.seek(0)
     return fd
 
 
-def load_csv(filename: str) -> SpeasyVariable:
+_parameters_header_blocks_regex = re.compile(
+    f"(# *PARAMETER_ID : ([^{os.linesep}]+){os.linesep}(# *[A-Z_]+ : [^{os.linesep}]+{os.linesep})+)+")
+
+
+def _parse_header(fd, expected_parameter: str):
+    line = fd.readline().decode()
+    header = ""
+    meta = {}
+    while len(line) and line[0] == '#':
+        header += line
+        if ':' in line:
+            key, value = [v.strip() for v in line[1:].split(':', 1)]
+            if key not in meta:
+                meta[key] = value
+        line = fd.readline().decode()
+    parameters_header_blocks = _parameters_header_blocks_regex.findall(header)
+    for block in parameters_header_blocks:
+        if block[1] == expected_parameter:
+            for line in block[0].split('\n'):
+                if ':' in line:
+                    key, value = [v.strip() for v in line[1:].split(':', 1)]
+                    meta[key] = value
+            break
+    return meta
+
+
+def load_csv(filename: str, expected_parameter: str) -> SpeasyVariable:
     """Load a CSV file
 
     Parameters
     ----------
     filename: str
         CSV filename
 
@@ -64,19 +91,15 @@
     with urlopen_with_retry(filename) as csv:
         with tempfile.TemporaryFile() as fd:
             _copy_data(csv, fd)
             line = fd.readline().decode()
             meta = {}
             y = None
             y_label = None
-            while len(line) > 0 and line[0] == '#':
-                if ':' in line:
-                    key, value = line[1:].split(':', 1)
-                    meta[key.strip()] = value.strip()
-                line = fd.readline().decode()
+            meta = _parse_header(fd, expected_parameter)
             columns = [col.strip()
                        for col in meta.get('DATA_COLUMNS', "").split(', ')[:]]
             meta["UNITS"] = meta.get("PARAMETER_UNITS")
             fd.seek(0)
             data = pds.read_csv(fd, comment='#', delim_whitespace=True,
                                 header=None, names=columns).values.transpose()
             time, data = epoch_to_datetime64(data[0]), data[1:].transpose()
@@ -196,8 +219,9 @@
 
     Returns
     -------
     dict
         parameter arguments in dictionary
     """
     return {'path': f"amda/{product}", 'start_time': f'{start_time.isoformat()}',
-            'stop_time': f'{stop_time.isoformat()}', 'output_format': kwargs.get('output_format', 'ASCII')}
+            'stop_time': f'{stop_time.isoformat()}',
+            'output_format': kwargs.get('output_format', amda_cfg.output_format.get())}
```

### Comparing `speasy-1.1.1/speasy/webservices/amda/ws.py` & `speasy-1.1.2/speasy/webservices/amda/ws.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/webservices/cda/__init__.py` & `speasy-1.1.2/speasy/webservices/cda/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,55 @@
 """CDA_Webservice package for Space Physics WebServices Client."""
 
 __author__ = """Alexis Jeandet"""
 __email__ = 'alexis.jeandet@member.fsf.org'
 __version__ = '0.1.0'
 
 import logging
+import re
 from datetime import datetime, timedelta
 from typing import Dict, Optional, Tuple
 
 from speasy.core import AllowedKwargs, http
-from speasy.core.cache import _cache  # _cache is used for tests (hack...)
 from speasy.core.cache import CACHE_ALLOWED_KWARGS, UnversionedProviderCache
 from speasy.core.cdf import load_variable
 from speasy.core.dataprovider import (GET_DATA_ALLOWED_KWARGS, DataProvider,
                                       ParameterRangeCheck)
 from speasy.core.datetime_range import DateTimeRange
+from speasy.core.http import urlopen_with_retry
 from speasy.core.inventory.indexes import (DatasetIndex, ParameterIndex,
                                            SpeasyIndex)
 from speasy.core.proxy import PROXY_ALLOWED_KWARGS, GetProduct, Proxyfiable
 from speasy.core.requests_scheduling import SplitLargeRequests
-from speasy.core.http import urlopen_with_retry
 from speasy.products.variable import SpeasyVariable
 
 log = logging.getLogger(__name__)
 
+_burst_regex = re.compile("(.*MMS.*FPI.*BRST.*|.*MMS.*SCM.*BRST.*)")
+
+
+def _is_burst_product(product: ParameterIndex or str) -> bool:
+    if isinstance(product, ParameterIndex):
+        product = product.spz_uid()
+    return bool(_burst_regex.match(str(product)))
+
+
+def _large_request_max_duration(product):
+    if _is_burst_product(product):
+        return timedelta(hours=2)
+    else:
+        return timedelta(days=7)
+
+
+def _cache_fragment_size(product):
+    if _is_burst_product(product):
+        return 2
+    else:
+        return 12
+
 
 class CdaWebException(BaseException):
     def __init__(self, text):
         super(CdaWebException, self).__init__(text)
 
 
 def _read_cdf(url: str, variable: str) -> SpeasyVariable:
@@ -143,16 +165,16 @@
             raise CdaWebException(f'Failed to get data with request: {url}, got {resp.status_code} HTTP response')
         else:
             return None
 
     @AllowedKwargs(
         PROXY_ALLOWED_KWARGS + CACHE_ALLOWED_KWARGS + GET_DATA_ALLOWED_KWARGS + ['if_newer_than'])
     @ParameterRangeCheck()
-    @UnversionedProviderCache(prefix="cda", fragment_hours=lambda x: 12, cache_retention=timedelta(days=7))
-    @SplitLargeRequests(threshold=lambda: timedelta(days=7))
+    @UnversionedProviderCache(prefix="cda", fragment_hours=_cache_fragment_size, cache_retention=timedelta(days=7))
+    @SplitLargeRequests(threshold=_large_request_max_duration)
     @Proxyfiable(GetProduct, get_parameter_args)
     def get_data(self, product, start_time: datetime, stop_time: datetime, if_newer_than: datetime or None = None,
                  extra_http_headers: Dict or None = None):
         dataset, variable = self._to_dataset_and_variable(product)
         return self._dl_variable(start_time=start_time, stop_time=stop_time, dataset=dataset,
                                  variable=variable, if_newer_than=if_newer_than, extra_http_headers=extra_http_headers)
```

### Comparing `speasy-1.1.1/speasy/webservices/cda/_inventory_builder/__init__.py` & `speasy-1.1.2/speasy/webservices/cda/_inventory_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/webservices/cda/_inventory_builder/_cdf_masters_parser.py` & `speasy-1.1.2/speasy/webservices/cda/_inventory_builder/_cdf_masters_parser.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/webservices/cda/_inventory_builder/_xml_catalogs_parser.py` & `speasy-1.1.2/speasy/webservices/cda/_inventory_builder/_xml_catalogs_parser.py`

 * *Files identical despite different names*

### Comparing `speasy-1.1.1/speasy/webservices/csa/__init__.py` & `speasy-1.1.2/speasy/webservices/csa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+import logging
+import tarfile
+from datetime import datetime, timedelta
+from io import BytesIO
+from tempfile import TemporaryDirectory
+from typing import Optional, Tuple, Dict
+
 import requests
 from astroquery.utils.tap.core import TapPlus
-from typing import Optional, Tuple, Dict
-from datetime import datetime, timedelta
-from speasy.core.cache import Cacheable, CACHE_ALLOWED_KWARGS  # _cache is used for tests (hack...)
-from speasy.products.variable import SpeasyVariable
+
 from speasy.core import http, AllowedKwargs, fix_name
-from speasy.core.proxy import Proxyfiable, GetProduct, PROXY_ALLOWED_KWARGS
+from speasy.core.cache import Cacheable, CACHE_ALLOWED_KWARGS  # _cache is used for tests (hack...)
 from speasy.core.cdf import load_variable
-from speasy.core.inventory.indexes import ParameterIndex, DatasetIndex, SpeasyIndex, make_inventory_node
 from speasy.core.dataprovider import DataProvider, ParameterRangeCheck, GET_DATA_ALLOWED_KWARGS
-from tempfile import TemporaryDirectory
 from speasy.core.datetime_range import DateTimeRange
+from speasy.core.inventory.indexes import ParameterIndex, DatasetIndex, SpeasyIndex, make_inventory_node
+from speasy.core.proxy import Proxyfiable, GetProduct, PROXY_ALLOWED_KWARGS
 from speasy.core.requests_scheduling import SplitLargeRequests
-import tarfile
-import logging
-from io import BytesIO
+from speasy.products.variable import SpeasyVariable
 
 log = logging.getLogger(__name__)
 
 
 def to_dataset_and_variable(index_or_str: ParameterIndex or str) -> Tuple[str, str]:
     if type(index_or_str) is str:
         parts = index_or_str.split('/')
@@ -219,15 +221,15 @@
         """
         dataset, variable = to_dataset_and_variable(product)
         return self.flat_inventory.datasets[dataset].date_last_update
 
     @AllowedKwargs(PROXY_ALLOWED_KWARGS + CACHE_ALLOWED_KWARGS + GET_DATA_ALLOWED_KWARGS)
     @ParameterRangeCheck()
     @Cacheable(prefix="csa", fragment_hours=lambda x: 12, version=product_last_update)
-    @SplitLargeRequests(threshold=lambda: timedelta(days=7))
+    @SplitLargeRequests(threshold=lambda x: timedelta(days=7))
     @Proxyfiable(GetProduct, get_parameter_args)
     def get_data(self, product, start_time: datetime, stop_time: datetime,
                  extra_http_headers: Dict[str, str] or None = None):
         dataset, variable = to_dataset_and_variable(product)
         return self._dl_variable(start_time=start_time, stop_time=stop_time, dataset=dataset,
                                  variable=variable, extra_http_headers=extra_http_headers)
```

### Comparing `speasy-1.1.1/speasy/webservices/ssc/__init__.py` & `speasy-1.1.2/speasy/webservices/ssc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 """cda package for Space Physics WebServices Client."""
 
 __author__ = """Alexis Jeandet"""
 __email__ = 'alexis.jeandet@member.fsf.org'
 __version__ = '0.1.0'
 
-from typing import Optional, Dict
+import logging
 from datetime import datetime, timedelta
+from typing import Optional, Dict
+
+import numpy as np
+
 from speasy.core.cache import Cacheable, CacheCall, CACHE_ALLOWED_KWARGS
-from speasy.products.variable import SpeasyVariable, VariableTimeAxis, DataContainer
-from ...core import http, AllowedKwargs, deprecation
-from speasy.core.proxy import Proxyfiable, GetProduct, PROXY_ALLOWED_KWARGS
-from speasy.core.inventory.indexes import ParameterIndex, SpeasyIndex
 from speasy.core.dataprovider import DataProvider, ParameterRangeCheck, GET_DATA_ALLOWED_KWARGS
 from speasy.core.datetime_range import DateTimeRange
+from speasy.core.inventory.indexes import ParameterIndex, SpeasyIndex
+from speasy.core.proxy import Proxyfiable, GetProduct, PROXY_ALLOWED_KWARGS
 from speasy.core.requests_scheduling import SplitLargeRequests
-import numpy as np
-from astropy import units
-
-import logging
+from speasy.products.variable import SpeasyVariable, VariableTimeAxis, DataContainer
+from ...core import http, AllowedKwargs
 
 log = logging.getLogger(__name__)
 
 
 def _make_datetime(dt: str) -> np.datetime64:
     '''
         Hack to support python 3.6, once 3.6 support removed then go back to:
@@ -119,15 +119,15 @@
         return var
 
     @AllowedKwargs(
         PROXY_ALLOWED_KWARGS + CACHE_ALLOWED_KWARGS + GET_DATA_ALLOWED_KWARGS + ['coordinate_system',
                                                                                  'debug'])
     @ParameterRangeCheck()
     @Cacheable(prefix="ssc_orbits", fragment_hours=lambda x: 24, version=version, entry_name=_make_cache_entry_name)
-    @SplitLargeRequests(threshold=lambda: timedelta(days=60))
+    @SplitLargeRequests(threshold=lambda x: timedelta(days=60))
     @Proxyfiable(GetProduct, get_parameter_args)
     def _get_orbit(self, product: str, start_time: datetime, stop_time: datetime, coordinate_system: str = 'gse',
                    debug=False, extra_http_headers: Dict or None = None) -> Optional[SpeasyVariable]:
         if stop_time - start_time < timedelta(days=1):
             stop_time += timedelta(days=1)
         url = f"{self.__url}/locations/{product}/{start_time.strftime('%Y%m%dT%H%M%SZ')},{stop_time.strftime('%Y%m%dT%H%M%SZ')}/{coordinate_system.lower()}/"
         if debug:
```

### Comparing `speasy-1.1.1/PKG-INFO` & `speasy-1.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: speasy
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple Python package to deal with main Space Physics WebServices (CDA, CSA, AMDA and SSC).
 Keywords: satellite,plasma-physics,nasa-data,amda,cdpp,CDF
 Author-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Maintainer-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,150 +30,134 @@
 Requires-Dist: tqdm
 Requires-Dist: matplotlib
 Requires-Dist: urllib3>=1.26.0
 Requires-Dist: zstd ; extra == "zstd"
 Project-URL: homepage, https://github.com/SciQLop/speasy
 Provides-Extra: zstd
 
-=======================
-Space Physics made EASY
-=======================
-
-
-.. image:: https://img.shields.io/matrix/speasy:matrix.org
-        :target: https://matrix.to/#/#speasy:matrix.org
-        :alt: Chat on Matrix
-
-.. image:: https://img.shields.io/pypi/v/speasy.svg
-        :target: https://pypi.python.org/pypi/speasy
-
-.. image:: https://github.com/SciQLop/speasy/workflows/Tests/badge.svg
-        :target: https://github.com/SciQLop/speasy/actions?query=workflow%3A%22Tests%22
-
-.. image:: https://readthedocs.org/projects/speasy/badge/?version=latest
-        :target: https://speasy.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-.. image:: https://codecov.io/gh/SciQLop/speasy/coverage.svg?branch=main
-        :target: https://codecov.io/gh/SciQLop/speasy/branch/main
-        :alt: Coverage Status
-
-.. image:: https://img.shields.io/lgtm/alerts/g/SciQLop/speasy.svg?logo=lgtm&logoWidth=18
-        :target: https://lgtm.com/projects/g/SciQLop/speasy/alerts/
-        :alt: Total alerts
-
-.. image:: https://img.shields.io/lgtm/grade/python/g/SciQLop/speasy.svg?logo=lgtm&logoWidth=18
-        :target: https://lgtm.com/projects/g/SciQLop/speasy/context:python
-        :alt: Language grade: Python
-
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4118780.svg
-   :target: https://doi.org/10.5281/zenodo.4118780
-   :alt: Zendoo DOI
-
-.. image:: https://mybinder.org/badge_logo.svg
-    :target: https://mybinder.org/v2/gh/SciQLop/speasy/main?labpath=docs/examples
-    :alt: Discover on MyBinder
-
-.. image:: https://colab.research.google.com/assets/colab-badge.svg
-    :target: https://colab.research.google.com/github/SciQLop/speasy
-    :alt: Discover on Google Colab
-
-.. image:: https://img.shields.io/uptimerobot/ratio/m792771930-24b7f89c03d5090a13462b70
-   :target: http://sciqlop.lpp.polytechnique.fr/cache
-   :alt: Speasy proxy uptime (30 days)
-
-Speasy is an open source Python client for Space Physics web services such as `CDAWEB <https://cdaweb.gsfc.nasa.gov/index.html/>`__
-or `AMDA <http://amda.irap.omp.eu/>`__.
-Most space physics data analysis starts with finding which server provides which dataset then figuring out how to download them.
-This can be difficult specially for students or newcomers, Speasy try to remove all difficulties by providing an unique and
-simple API to access them all.
-Speasy aims to support as much as possible web services and also cover a maximum of features they propose.
-
-Quickstart
-----------
-
-Installing Speasy with pip (`more details here <https://speasy.readthedocs.io/en/stable/installation.html>`_):
-
-.. code-block:: console
-
-    $ python -m pip install speasy
-    # or
-    $ python -m pip install --user speasy
+<h1 align="center">
+<img src="https://raw.githubusercontent.com/SciQLop/speasy/main/logo/logo_speasy.svg" width="300">
+</h1><br>
+
+# Space Physics made EASY
+
+[![Chat on Matrix](https://img.shields.io/matrix/speasy:matrix.org)](https://matrix.to/#/#speasy:matrix.org)
+[![image](https://img.shields.io/pypi/v/speasy.svg)](https://pypi.python.org/pypi/speasy)
+[![image](https://github.com/SciQLop/speasy/workflows/Tests/badge.svg)](https://github.com/SciQLop/speasy/actions?query=workflow%3A%22Tests%22)
+[![Documentation Status](https://readthedocs.org/projects/speasy/badge/?version=latest)](https://speasy.readthedocs.io/en/latest/?badge=latest)
+[![Coverage Status](https://codecov.io/gh/SciQLop/speasy/coverage.svg?branch=main)](https://codecov.io/gh/SciQLop/speasy/branch/main)
+[![CodeQL](https://github.com/SciQLop/speasy/actions/workflows/codeql.yml/badge.svg)](https://github.com/SciQLop/speasy/actions/workflows/codeql.yml)
+[![Zendoo DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4118780.svg)](https://doi.org/10.5281/zenodo.4118780)
+[![Discover on MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SciQLop/speasy/main?labpath=docs/examples)
+[![Discover on Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SciQLop/speasy)
+[![Speasy proxy uptime (30 days)](https://img.shields.io/uptimerobot/ratio/m792771930-24b7f89c03d5090a13462b70)](http://sciqlop.lpp.polytechnique.fr/cache)
+
+Speasy is an open source Python client for Space Physics web services
+such as [CDAWEB](https://cdaweb.gsfc.nasa.gov/index.html/) or
+[AMDA](http://amda.irap.omp.eu/). Most space physics data analysis
+starts with finding which server provides which dataset then figuring
+out how to download them. This can be difficult specially for students
+or newcomers, Speasy try to remove all difficulties by providing an
+unique and simple API to access them all. Speasy aims to support as much
+as possible web services and also cover a maximum of features they
+propose.
+
+## Quickstart
+
+Installing Speasy with pip ([more details
+here](https://speasy.readthedocs.io/en/stable/installation.html)):
+
+``` console
+$ python -m pip install speasy
+# or
+$ python -m pip install --user speasy
+```
 
 Getting data is as simple as:
 
-.. code-block:: python
+``` python
+import speasy as spz
+ace_mag = spz.get_data('amda/imf', "2016-6-2", "2016-6-5")
+```
 
-    import speasy as spz
-    ace_mag = spz.get_data('amda/imf', "2016-6-2", "2016-6-5")
-
-Where amda is the webservice and imf is the product id you will get with this request.
+Where amda is the webservice and imf is the product id you will get with
+this request.
 
 Using the dynamic inventory this can be even simpler:
 
-.. code-block:: python
-
-    import speasy as spz
-    amda_tree = spz.inventory.data_tree.amda
-    ace_mag = spz.get_data(amda_tree.Parameters.ACE.MFI.ace_imf_all.imf, "2016-6-2", "2016-6-5")
-
-Will produce the exact same result than previous example but has the advantage to be easier to manipulate since you can
-discover available data from your favourite Python environment completion such as IPython or notebooks (might not work from IDEs).
-
-This also works with `SSCWEB <https://sscweb.gsfc.nasa.gov/>`__, you can easily download trajectories:
-
-.. code-block:: python
-
-    import speasy as spz
-    sscweb_tree = spz.inventories.data_tree.ssc
-    solo = spz.get_data(sscweb_tree.Trajectories.solarorbiter, "2021-01-01", "2021-02-01")
+``` python
+import speasy as spz
+amda_tree = spz.inventory.data_tree.amda
+ace_mag = spz.get_data(amda_tree.Parameters.ACE.MFI.ace_imf_all.imf, "2016-6-2", "2016-6-5")
+```
+
+Will produce the exact same result than previous example but has the
+advantage to be easier to manipulate since you can discover available
+data from your favourite Python environment completion such as IPython
+or notebooks (might not work from IDEs).
+
+This also works with [SSCWEB](https://sscweb.gsfc.nasa.gov/), you can
+easily download trajectories:
+
+``` python
+import speasy as spz
+sscweb_tree = spz.inventories.data_tree.ssc
+solo = spz.get_data(sscweb_tree.Trajectories.solarorbiter, "2021-01-01", "2021-02-01")
+```
 
 More complex requests like this one are supported:
 
-.. code-block:: python
-
-    import speasy as spz
-    products = [
-        spz.inventories.tree.amda.Parameters.Wind.SWE.wnd_swe_kp.wnd_swe_vth,
-        spz.inventories.tree.amda.Parameters.Wind.SWE.wnd_swe_kp.wnd_swe_pdyn,
-        spz.inventories.tree.amda.Parameters.Wind.SWE.wnd_swe_kp.wnd_swe_n,
-        spz.inventories.tree.cda.Wind.WIND.MFI.WI_H2_MFI.BGSE,
-        spz.inventories.tree.ssc.Trajectories.wind,
-    ]
-    intervals = [["2010-01-02", "2010-01-02T10"], ["2009-08-02", "2009-08-02T10"]]
-    data = spz.get_data(products, intervals)
-
-Documentation
-=============
-
-Check out the documentation and examples at `speasy documentation <https://speasy.readthedocs.io/en/stable/>`_.
-
-Features
---------
-- Simple and intuitive API (spz.get_data to get them all)
-- Pandas DataFrame like interface for variables
-- Quick functions to convert a variable to a Pandas DataFrame
-- Local cache to avoid repeating twice the same request
-- Can take advantage of SciQLop dedicated proxy as a community backed ultra fast cache
-- Full support of `AMDA <http://amda.irap.omp.eu/>`__ API
-- Can retrieve time-series from `AMDA <http://amda.irap.omp.eu/>`__, `CDAWeb <https://cdaweb.gsfc.nasa.gov/>`__, `CSA <https://csa.esac.esa.int/csa-web/>`_, `SSCWeb <https://sscweb.gsfc.nasa.gov/>`__
-
-
-Examples
-========
-See `here <https://speasy.readthedocs.io/en/stable/examples/index.html>`_ for a complete list of examples.
-
-Caveats
-=======
-- installing speasy on both python 3.7 or less and python 3.8 or plus at the same time doesn't work since entries stored in cache by python 3.8+ are not readable by python 3.7-.
-- Speasy is not a plotting package, while it provides basic plot features, it is not meant to produce publication ready figures.
-
-Credits
-========
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+``` python
+import speasy as spz
+products = [
+    spz.inventories.tree.amda.Parameters.Wind.SWE.wnd_swe_kp.wnd_swe_vth,
+    spz.inventories.tree.amda.Parameters.Wind.SWE.wnd_swe_kp.wnd_swe_pdyn,
+    spz.inventories.tree.amda.Parameters.Wind.SWE.wnd_swe_kp.wnd_swe_n,
+    spz.inventories.tree.cda.Wind.WIND.MFI.WI_H2_MFI.BGSE,
+    spz.inventories.tree.ssc.Trajectories.wind,
+]
+intervals = [["2010-01-02", "2010-01-02T10"], ["2009-08-02", "2009-08-02T10"]]
+data = spz.get_data(products, intervals)
+```
+
+### Documentation
+
+Check out the documentation and examples at [speasy
+documentation](https://speasy.readthedocs.io/en/stable/).
+
+## Features
+
+-   Simple and intuitive API (spz.get_data to get them all)
+-   Pandas DataFrame like interface for variables
+-   Quick functions to convert a variable to a Pandas DataFrame
+-   Local cache to avoid repeating twice the same request
+-   Can take advantage of SciQLop dedicated proxy as a community backed
+    ultra fast cache
+-   Full support of [AMDA](http://amda.irap.omp.eu/) API
+-   Can retrieve time-series from [AMDA](http://amda.irap.omp.eu/),
+    [CDAWeb](https://cdaweb.gsfc.nasa.gov/),
+    [CSA](https://csa.esac.esa.int/csa-web/),
+    [SSCWeb](https://sscweb.gsfc.nasa.gov/)
+
+### Examples
+
+See [here](https://speasy.readthedocs.io/en/stable/examples/index.html)
+for a complete list of examples.
+
+### Caveats
+
+-   installing speasy on both python 3.7 or less and python 3.8 or plus
+    at the same time doesn't work since entries stored in cache by
+    python 3.8+ are not readable by python 3.7-.
+-   Speasy is not a plotting package, while it provides basic plot
+    features, it is not meant to produce publication ready figures.
+
+### Credits
+
+This package was created with
+[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
+project template.
 
-The development of speasy is supported by the `CDPP <http://www.cdpp.eu/>`__.
+The development of speasy is supported by the
+[CDPP](http://www.cdpp.eu/).
```

