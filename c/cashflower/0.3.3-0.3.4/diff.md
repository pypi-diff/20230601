# Comparing `tmp/cashflower-0.3.3.tar.gz` & `tmp/cashflower-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.3.3.tar", last modified: Thu May  4 17:45:15 2023, max compression
+gzip compressed data, was "cashflower-0.3.4.tar", last modified: Thu Jun  1 15:50:57 2023, max compression
```

## Comparing `cashflower-0.3.3.tar` & `cashflower-0.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-04 17:45:01.000000 cashflower-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 17:45:01.000000 cashflower-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-04 17:45:15.076512 cashflower-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-04 17:45:01.000000 cashflower-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29050 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/cashflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/model_tpl/model.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:45:15.076512 cashflower-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 17:45:02.000000 cashflower-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-04 17:45:02.000000 cashflower-0.3.3/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-04 17:45:02.000000 cashflower-0.3.3/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-04 17:45:02.000000 cashflower-0.3.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-01 15:50:45.000000 cashflower-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 15:50:45.000000 cashflower-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-01 15:50:57.547887 cashflower-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-01 15:50:45.000000 cashflower-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/cashflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/model_tpl/model.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:50:57.547887 cashflower-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-01 15:50:45.000000 cashflower-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-06-01 15:50:45.000000 cashflower-0.3.4/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-01 15:50:45.000000 cashflower-0.3.4/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-01 15:50:45.000000 cashflower-0.3.4/tests/test_utils.py
```

### Comparing `cashflower-0.3.3/LICENSE` & `cashflower-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.3.3/PKG-INFO` & `cashflower-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.3.3
+Version: 0.3.4
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.3.3/README.md` & `cashflower-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cashflower-0.3.3/cashflower/cashflow.py` & `cashflower-0.3.4/cashflower/cashflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import copy
-import datetime
 import functools
 import inspect
 import numpy as np
-import os
 import time
 import pandas as pd
 import sys
 
 
 from .utils import *
 
@@ -41,14 +39,74 @@
     text = "\r[{}] {:.0f}% {}".format(
         "#" * block + "-" * (bar_length - block), round(progress * 100, 0),
         status)
     sys.stdout.write(text)
     sys.stdout.flush()
 
 
+def get_col_dict(model_point_sets, variables, constants, settings):
+    """
+    | main | ModelVariable = ["a", "b"]
+    |      | Constant      = ["c"]
+    | fund | ModelVariable = ["d"]
+    |      | Constant      = []
+    """
+    col_dict = {}
+    for model_point_set in model_point_sets:
+        col_dict[model_point_set.name] = {}
+        col_dict[model_point_set.name]["ModelVariable"] = []
+        col_dict[model_point_set.name]["Constant"] = []
+
+    # A subset of output columns has been chosen
+    if len(settings["OUTPUT_COLUMNS"]) > 0:
+        variables = [variable for variable in variables if variable.name in settings["OUTPUT_COLUMNS"]]
+        constants = [constant for constant in constants if constant.name in settings["OUTPUT_COLUMNS"]]
+
+    for variable in variables:
+        col_dict[variable.model_point_set.name]["ModelVariable"].append(variable.name)
+
+    # Aggregate output does not contain Constants (because they don't add up)
+    if not settings["AGGREGATE"]:
+        for constant in constants:
+            col_dict[constant.model_point_set.name]["Constant"].append(constant.name)
+
+    return col_dict
+
+
+def col_dict_to_model_point_output(col_dict, settings, records):
+    """
+    | main | ModelVariable = matrix(n1 x m1)
+    |      | Constant      = matrix(n2 x m2)
+    | fund | ModelVariable = matrix(n3 x m3)
+    |      | Constant      = matrix(n4 x m4)
+    m_x = num_components (may be zero)
+    n_x = t_output_max (* num_records if individual output)
+    """
+    model_point_output = copy.deepcopy(col_dict)
+
+    for model_point_set_name in col_dict.keys():
+        num_records = 1 if settings["AGGREGATE"] else records[model_point_set_name]
+        n = (settings["T_OUTPUT_MAX"]+1) * num_records
+
+        m = len(col_dict[model_point_set_name]["ModelVariable"])
+        model_point_output[model_point_set_name]["ModelVariable"] = np.zeros((n, m), dtype=np.float64)
+
+        m = len(col_dict[model_point_set_name]["Constant"])
+        model_point_output[model_point_set_name]["Constant"] = np.zeros((n, m), dtype=np.object_)
+    return model_point_output
+
+
+def flatten_col_dict(col_dict):
+    lst = []
+    for key1 in col_dict.keys():
+        for key2 in col_dict[key1]:
+            lst.append(col_dict[key1][key2])
+    return [item for sublist in lst for item in sublist]
+
+
 class CashflowModelError(Exception):
     pass
 
 
 class Runplan:
     """Runplan of the cash flow model.
 
@@ -279,15 +337,19 @@
         if t < 0 or t > self.settings["T_CALCULATION_MAX"]:
             return 0
 
         # User might call lower order variable from higher order variable and specify record (r)
         if r is not None:
             return self.result[r, t]
 
-        return self.result[self.model_point_set.model_point_record_num, t]
+        value = self.result[self.model_point_set.model_point_record_num, t]
+        if np.isnan(value):
+            return self.formula(t)
+        else:
+            return self.result[self.model_point_set.model_point_record_num, t]
 
     @property
     def formula(self):
         """Formula used to calculate result. """
         return self._formula
 
     @formula.setter
@@ -317,15 +379,14 @@
         """Clear formula's cache. """
         if self.mp_dep:
             self.formula.cache_clear()
 
     def calculate(self):
         """Calculate result for all records of the model point."""
         t_calculation_max = self.settings["T_CALCULATION_MAX"]
-        self.result = np.empty((self.model_point_set.model_point_size, t_calculation_max + 1), dtype=float)
 
         for r in range(self.model_point_set.model_point_size):
             self.clear()
             self.model_point_set.model_point_record_num = r
 
             # Formula returns an array
             if self.calc_array:
@@ -341,26 +402,33 @@
                     for t in range(t_calculation_max+1):
                         self.result[r, t] = self.formula(t)
                 # recursive backward
                 else:
                     for t in range(t_calculation_max, -1, -1):
                         self.result[r, t] = self.formula(t)
 
+    def calculate_t(self, t):
+        for r in range(self.model_point_set.model_point_size):
+            self.clear()
+            self.model_point_set.model_point_record_num = r
+            self.result[r, t] = self.formula(t)
+        return self.result[:, t]
+
     def initialize(self, main=None):
         if self.assigned_formula is None:
             msg = f"\nThe '{self.name}' variable has no formula. Please check the 'model.py' script."
             raise CashflowModelError(msg)
 
         if self.model_point_set is None:
             self.model_point_set = main
 
         self.formula = self.assigned_formula
-
-    def in_output(self, output_columns):
-        return output_columns == [] or self.name in output_columns
+        self.result = np.empty((self.model_point_set.model_point_size, self.settings["T_CALCULATION_MAX"] + 1),
+                               dtype=float)
+        self.result[:] = np.nan
 
 
 class Constant:
     """Constant of a cash flow model.
     Constant can return either number or string and is t-independent.
 
     Attributes
@@ -436,27 +504,27 @@
         """Calculate constant's value for all records in the model point."""
         self.result = [None] * self.model_point_set.model_point_size
         for r in range(self.model_point_set.model_point_size):
             self.clear()
             self.model_point_set.model_point_record_num = r
             self.result[r] = self.formula()
 
+    def calculate_t(self, t):
+        return self.calculate()
+
     def initialize(self, main=None):
         if self.assigned_formula is None:
             msg = f"\nThe '{self.name}' parameter has no formula. Please check the 'model.py' script."
             raise CashflowModelError(msg)
 
         if self.model_point_set is None:
             self.model_point_set = main
 
         self.formula = self.assigned_formula
 
-    def in_output(self, output_columns):
-        return output_columns == [] or self.name in output_columns
-
 
 class Model:
     """Actuarial cash flow model.
     Model combines model variables, constants and model point sets.
     Model components (constants and variables) are ordered into a calculation queue.
 
     Attributes
@@ -486,34 +554,22 @@
         self.settings = settings
         self.components = variables + constants
         self.queue = []
         self.empty_output = None
         self.output = None
         self.cpu_count = cpu_count
 
-    def get_component_by_name(self, name):
-        """Get a model component object by its name."""
-        for component in self.components:
-            if component.name == name:
-                return component
-
-    def get_model_point_set_by_name(self, name):
-        """Get a model point set object by its name."""
-        for model_point_set in self.model_point_sets:
-            if model_point_set.name == name:
-                return model_point_set
-
     def set_children(self):
         """Set children of the model components. """
         component_names = [component.name for component in self.components]
         for component in self.components:
             formula_source = inspect.getsource(component.formula)
             cleaned_formula_source = clean_formula_source(formula_source)
             child_names = list_called_funcs(cleaned_formula_source, component_names)
-            component.children = [self.get_component_by_name(n) for n in child_names if n != component.name]
+            component.children = [get_object_by_name(self.components, n) for n in child_names if n != component.name]
 
     def set_grandchildren(self):
         """Set grandchildren of model components. """
         for component in self.components:
             component.grandchildren = list(component.children)
             i = 0
             while i < len(component.grandchildren):
@@ -526,209 +582,195 @@
         for component in self.components:
             if removed_component in component.grandchildren:
                 component.grandchildren.remove(removed_component)
 
     def set_queue(self):
         """Set an ordrer in which model components should be evaluated."""
         queue = []
+        log = None
 
-        # User has chosen components, so there is no need to calculate all of them
+        # User has chosen components, so limit them
         if len(self.settings["OUTPUT_COLUMNS"]) > 0:
             components = []
             for component_name in self.settings["OUTPUT_COLUMNS"]:
-                component = self.get_component_by_name(component_name)
+                component = get_object_by_name(self.components, component_name)
+                if component is None:
+                    log = f"'{component_name}' is not one of the model components and will be ignored."
+                    continue
                 components = unique_append(components, component)
                 components = unique_extend(components, component.grandchildren)
             components = sorted(components)
         else:
             components = sorted(self.components)
 
+        # Create a queue based on number of grandchildren
         while components:
             component = components[0]
 
             if len(component.grandchildren) != 0:
                 cycle = get_cycle(component, rest=components)
-                msg = f"Cycle of model components detected. Please review:\n {cycle_to_str(cycle)}"
-                raise CashflowModelError(msg)
-
-            queue.append(component)
-            self.remove_from_grandchildren(component)
-            components.remove(component)
+                # msg = f"Cycle of model components detected. Please review:\n {cycle_to_str(cycle)}"
+                # raise CashflowModelError(msg)
+                queue.append(cycle)
+                for item in cycle:
+                    self.remove_from_grandchildren(item)
+                    components.remove(item)
+            else:
+                queue.append(component)
+                self.remove_from_grandchildren(component)
+                components.remove(component)
             components = sorted(components)
         self.queue = queue
-
-    def set_empty_output(self):
-        """Create empty output to be populated with results. """
-        empty_output = dict()
-        aggregate = self.settings["AGGREGATE"]
-        output_columns = self.settings["OUTPUT_COLUMNS"]
-
-        # Each model_point_set has a separate output file
-        for modelpointset in self.model_point_sets:
-            empty_output[modelpointset.name] = pd.DataFrame()
-            empty_output[modelpointset.name]["t"] = None
-            # Individual output contains record numbers
-            if not aggregate:
-                empty_output[modelpointset.name]["r"] = None
-
-        # Aggregated output contains only variables
-        # Individual output contains all components (variables and constants)
-        if aggregate:
-            output_variables = [v for v in self.variables if v.in_output(output_columns)]
-            for output_variable in output_variables:
-                empty_output[output_variable.model_point_set.name][output_variable.name] = None
-        else:
-            output_components = [c for c in self.components if c.in_output(output_columns)]
-            for output_component in output_components:
-                empty_output[output_component.model_point_set.name][output_component.name] = None
-
-        self.empty_output = empty_output
+        return log
 
     def initialize(self):
-        self.set_empty_output()
         self.set_children()
         self.set_grandchildren()
-        self.set_queue()
+        log = self.set_queue()
+        return log
 
-    def calculate_single_model_point(self, row, pb_max, main, one_core=None):
+    def calculate_model_point(self, row, pb_max, main, col_dict, one_core=None):
         """Calculate results for a model point currently indicated in the model point set."""
         model_point_id = main.model_point_set_data.index[row]
+        records = {}
         for model_point_set in self.model_point_sets:
             model_point_set.id = model_point_id
+            records[model_point_set.name] = model_point_set.model_point_data.shape[0]
 
-        model_point_output = copy.deepcopy(self.empty_output)
-        aggregate = self.settings["AGGREGATE"]
-        t_calculation_max = self.settings["T_CALCULATION_MAX"]
-        t_output_max = min(self.settings["T_OUTPUT_MAX"], t_calculation_max)
-        output_columns = self.settings["OUTPUT_COLUMNS"]
+        model_point_output = col_dict_to_model_point_output(col_dict, self.settings, records)
+        col_components = flatten_col_dict(col_dict)
 
+        # Calculate results
         for c in self.queue:
-            start = time.time()
-            try:
-                c.calculate()
-            except:
-                raise CashflowModelError(f"Unable to evaluate '{c.name}'.")
+            # Single model component
+            if type(c) is not list:
+                start = time.time()
+                try:
+                    c.calculate()
+                except:
+                    raise CashflowModelError(f"Unable to evaluate '{c.name}'.")
+                c.runtime += time.time() - start
+            # It's a cycle
             else:
-                # User can choose output columns
-                if c.in_output(output_columns):
-                    # Variables are always in the output (individual and aggregate)
-                    if isinstance(c, ModelVariable):
-                        if aggregate:
-                            model_point_output[c.model_point_set.name][c.name] = sum(c.result[:, :t_output_max + 1])
-                        else:
-                            model_point_output[c.model_point_set.name][c.name] = c.result[:, :t_output_max + 1].flatten()
-                    # Constants are added only to individual output
-                    if isinstance(c, Constant) and not aggregate:
-                        model_point_output[c.model_point_set.name][c.name] = np.repeat(c.result, t_output_max + 1)
-            c.runtime += time.time() - start
-
-        # Add time and record number to the individual output
-        if not aggregate:
-            for model_point_set in self.model_point_sets:
-                model_point_output[model_point_set.name]["t"] = np.tile(np.arange(t_output_max + 1), model_point_set.model_point_size)
-                model_point_output[model_point_set.name]["r"] = np.repeat(np.arange(1, model_point_set.model_point_size + 1), t_output_max + 1)
+                for t in range(self.settings["T_CALCULATION_MAX"] + 1):
+                    for item in c:
+                        try:
+                            x = item.calculate_t(t)
+                        except:
+                            raise CashflowModelError(f"Unable to evaluate '{item.name}'.")
+
+        # Add results to model_point_output
+        for c in flatten(self.queue):
+            if c.name in col_components:
+                if isinstance(c, ModelVariable):
+                    index = col_dict[c.model_point_set.name]["ModelVariable"].index(c.name)
+                    if self.settings["AGGREGATE"]:
+                        result = sum(c.result[:, :self.settings["T_OUTPUT_MAX"] + 1])
+                    else:
+                        result = (c.result[:, :self.settings["T_OUTPUT_MAX"] + 1]).flatten()
+                    model_point_output[c.model_point_set.name]["ModelVariable"][:, index] = result
+                if isinstance(c, Constant):
+                    index = col_dict[c.model_point_set.name]["Constant"].index(c.name)
+                    result = np.repeat(c.result, self.settings["T_OUTPUT_MAX"] + 1)
+                    result = result.astype(np.object_, copy=False)
+                    model_point_output[c.model_point_set.name]["Constant"][:, index] = result
 
         if one_core:
             updt(pb_max, row + 1)
 
         return model_point_output
 
-    def calculate(self, range_start=None, range_end=None):
+    def calculate_model(self, range_start=None, range_end=None):
         """Calculate results for all model points."""
-        # Configuration
-        model_output = copy.deepcopy(self.empty_output)
-        aggregate = self.settings["AGGREGATE"]
-        t_output_max = min(self.settings["T_OUTPUT_MAX"], self.settings["T_CALCULATION_MAX"])
-        main = self.get_model_point_set_by_name("main")
+        main = get_object_by_name(self.model_point_sets, "main")
         one_core = range_start == 0 or range_start is None
 
-        # Calculate formulas
-        n_pols = len(main)
-        pb_max = n_pols if range_end is None else range_end
-        calculate = functools.partial(self.calculate_single_model_point, pb_max=pb_max, main=main, one_core=one_core)
+        # Calculate model points
+        num_mp = len(main)
+        pb_max = num_mp if range_end is None else range_end
+        col_dict = get_col_dict(self.model_point_sets, self.variables, self.constants, self.settings)
+        p = functools.partial(self.calculate_model_point, pb_max=pb_max, main=main, col_dict=col_dict, one_core=one_core)
         if range_start is None:
-            model_point_outputs = [*map(calculate, range(n_pols))]
+            model_point_outputs = [*map(p, range(num_mp))]
         else:
-            model_point_outputs = [*map(calculate, range(range_start, range_end))]
+            model_point_outputs = [*map(p, range(range_start, range_end))]
 
-        # Merge results from single model points
+        # Merge results from model points
         if one_core:
             print_log("Preparing results")
 
-        for model_point_set in self.model_point_sets:
-            if aggregate:
-                model_output[model_point_set.name] = sum(model_point_output[model_point_set.name] for model_point_output in model_point_outputs)
-                if not self.settings["MULTIPROCESSING"]:
-                    model_output[model_point_set.name]["t"] = np.arange(t_output_max + 1)
+        model_output = {}
+        for key in col_dict.keys():
+            if self.settings["AGGREGATE"]:
+                columns = col_dict[key]["ModelVariable"]
+                if len(columns) > 0:
+                    data = sum(mpo[key]["ModelVariable"] for mpo in model_point_outputs)
+                    model_output[key] = pd.DataFrame(data, columns=col_dict[key]["ModelVariable"])
             else:
-                model_output[model_point_set.name] = pd.concat(model_point_output[model_point_set.name] for model_point_output in model_point_outputs)
+                columns = col_dict[key]["Constant"] + col_dict[key]["ModelVariable"]
+                if len(columns) > 0:
+                    data1 = np.concatenate([mpo[key]["Constant"] for mpo in model_point_outputs], axis=0)
+                    data2 = np.concatenate([mpo[key]["ModelVariable"] for mpo in model_point_outputs], axis=0)
+                    data = np.concatenate([data1, data2], axis=1)
+                    model_output[key] = pd.DataFrame(data, columns=columns)
+
+                    # Add records
+                    main = get_object_by_name(self.model_point_sets, "main")
+                    main_ids = main.model_point_set_data[self.settings["ID_COLUMN"]].tolist()
+                    if range_start is not None:
+                        main_ids = main_ids[range_start:range_end]
+
+                    model_point_set = get_object_by_name(self.model_point_sets, key)
+                    ids = model_point_set.model_point_set_data[self.settings["ID_COLUMN"]]
+                    ids = [_id for _id in ids if _id in main_ids]
+
+                    records = lst_to_records(ids)
+                    model_output[key].insert(0, "r", np.repeat(records, self.settings["T_OUTPUT_MAX"]+1))
 
         self.output = model_output
         return model_output
 
     def run(self, part=None):
         """Orchestrate all steps of the cash flow model run."""
         one_core = part == 0 or part is None
 
         if one_core:
             print_log(f"Start run for model '{self.name}'")
 
         # Prepare the order of variables for the calculation
-        self.initialize()
+        log = self.initialize()
+        if log is not None and one_core:
+            print_log(log)
 
         # Inform on the number of model points
-        main = self.get_model_point_set_by_name("main")
+        main = get_object_by_name(self.model_point_sets, "main")
         if one_core:
             print_log(f"Total number of model points: {main.model_point_set_data.shape[0]}")
         if part == 0:
-            # Runtime is not saved when multiprocessing
-            if self.settings["SAVE_RUNTIME"]:
-                print_log(f"The SAVE_RUNTIME setting is not applicable for multiprocessing.\n"
-                          f"{' '*10} Set the MULTIPROCESSING setting to 'False' to save the runtime.")
-            if main.model_point_set_data.shape[0] > self.cpu_count:
+            if len(main) > self.cpu_count:
                 print_log(f"Multiprocessing on {self.cpu_count} cores")
                 print_log(f"Calculation of ca. {len(main) // self.cpu_count} model points per core")
                 print_log("The progressbar for the calculations on the 1st core:")
 
-        # In multiprocessing mode, the subset of policies is calculated
+        # Calculate all or subset of model points
         if self.settings["MULTIPROCESSING"]:
             main_ranges = split_to_ranges(len(main), self.cpu_count)
 
             # Number of model points is lower than the number of cpus, only calculate on the 1st core
             if part >= len(main_ranges):
                 return None
 
             main_range = main_ranges[part]
-            self.calculate(range_start=main_range[0], range_end=main_range[1])
-        # Otherwise, all policies are calculated
+            model_output = self.calculate_model(range_start=main_range[0], range_end=main_range[1])
         else:
-            self.calculate()
-
-        return self.output
+            model_output = self.calculate_model()
 
-    def save(self):
-        """Only for single core (no multiprocessing)"""
-        timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
-
-        if not os.path.exists("output"):
-            os.makedirs("output")
-
-        # Save output to csv
-        if self.settings["SAVE_OUTPUT"]:
-            print_log("Saving output:")
-            for model_point_set in self.model_point_sets:
-                filepath = f"output/{timestamp}_{model_point_set.name}.csv"
-                model_point_set_output = self.output.get(model_point_set.name)
-                column_names = [col for col in model_point_set_output.columns.values.tolist() if col not in ["t", "r"]]
-                if len(column_names) > 0:
-                    print(f"{' ' * 10} {filepath}")
-                    model_point_set_output.to_csv(filepath, index=False)
-
-        # Save runtime
+        # Get runtime
+        runtime = None
         if self.settings["SAVE_RUNTIME"]:
-            data = [(c.name, c.runtime) for c in self.components]
-            runtime = pd.DataFrame(data, columns=["component", "runtime"])
-            runtime.to_csv(f"output/{timestamp}_runtime.csv", index=False)
-            print(f"{' '*10} output/{timestamp}_runtime.csv")
+            runtime = pd.DataFrame({
+                "component": [c.name for c in self.components],
+                "runtime": [c.runtime for c in self.components]
+            })
+
+        return model_output, runtime
 
-        print_log("Finished")
-        return timestamp
```

### Comparing `cashflower-0.3.3/cashflower/start.py` & `cashflower-0.3.4/cashflower/start.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import datetime
 import functools
 import importlib
 import inspect
 import multiprocessing
-import numpy as np
 import os
 import pandas as pd
 import shutil
 
 from .cashflow import CashflowModelError, ModelVariable, ModelPointSet, Model, Constant, Runplan
-from .utils import replace_in_file, print_log
+from .utils import print_log, replace_in_file
 
 
 def create_model(model):
     """Create a folder structure for a model.
 
     Copies the whole content of the model_tpl folder and changes templates to scripts.
 
@@ -51,17 +50,25 @@
         "T_CALCULATION_MAX": 1200,
         "T_OUTPUT_MAX": 1200,
     }
 
     if settings is None:
         return initial_settings
 
+    # Update with the user settings
     for key, value in settings.items():
         initial_settings[key] = value
 
+    # Maximal output t can't exceed maximal calculation t
+    if initial_settings["T_CALCULATION_MAX"] < initial_settings["T_OUTPUT_MAX"]:
+        initial_settings["T_OUTPUT_MAX"] = initial_settings["T_CALCULATION_MAX"]
+        msg = "The T_CALCULATION_MAX setting is greater than the T_OUTPUT_MAX setting. " \
+              "T_OUTPUT_MAX has been set to T_CALCULATION_MAX."
+        print_log(msg)
+
     return initial_settings
 
 
 def get_runplan(input_members):
     """Get runplan object from input.py script."""
     runplan = None
     for name, item in input_members:
@@ -139,78 +146,110 @@
     # User can provide runplan version in CLI command
     if runplan is not None and len(argv) > 1:
         runplan.version = argv[1]
 
     return runplan, model_point_sets, variables, constants
 
 
+def dict_to_csv(_dict, timestamp):
+    if not os.path.exists("output"):
+        os.makedirs("output")
+
+    for key in _dict:
+        filepath = f"output/{timestamp}_{key}.csv"
+        data = _dict.get(key)
+        data.to_csv(filepath, index=False)
+        print(f"{' ' * 10} {filepath}")
+
+    return None
+
+
+def df_to_csv(df, timestamp):
+    df.to_csv(f"output/{timestamp}_runtime.csv", index=False)
+    print(f"{' ' * 10} output/{timestamp}_runtime.csv")
+    return None
+
+
 def start_single_core(model_name, settings, argv):
-    """Create, run and save results of a cash flow model."""
-    settings = load_settings(settings)
+    """Create and run a cash flow model."""
     runplan, model_point_sets, variables, constants = prepare_model_input(model_name, settings, argv)
 
-    # Run model on single core and save results
+    # Run model on single core
     model = Model(model_name, variables, constants, model_point_sets, settings)
-    output = model.run()
-    model.save()
-    return output
+    model_output, runtime = model.run()
+    return model_output, runtime
 
 
-def execute_multiprocessing(part, model_name, settings, cpu_count, argv):
+def start_multiprocessing(part, cpu_count, model_name, settings, argv):
     """Run subset of the model points using multiprocessing."""
     runplan, model_point_sets, variables, constants = prepare_model_input(model_name, settings, argv)
 
     # Run model on multiple cores
     model = Model(model_name, variables, constants, model_point_sets, settings, cpu_count)
+
     output = model.run(part)
-    return output
+    if output is None:
+        part_model_output, part_runtime = None, None
+    else:
+        part_model_output, part_runtime = output
+    return part_model_output, part_runtime
 
 
-def merge_and_save_multiprocessing(part_outputs, settings):
+def merge_part_model_outputs(part_model_outputs, settings):
     """Merge outputs from multiprocessing and save to files."""
-    t_output_max = min(settings["T_OUTPUT_MAX"], settings["T_CALCULATION_MAX"])
-
     # Nones are returned, when number of policies < number of cpus
-    part_outputs = [part_output for part_output in part_outputs if part_output is not None]
+    part_model_outputs = [pmo for pmo in part_model_outputs if pmo is not None]
+    first = part_model_outputs[0]
 
     # Merge outputs into one
-    model_point_set_names = part_outputs[0].keys()
     model_output = {}
-    for model_point_set_name in model_point_set_names:
+    for key in first.keys():
         if settings["AGGREGATE"]:
-            model_output[model_point_set_name] = sum(part_output[model_point_set_name] for part_output in part_outputs)
-            model_output[model_point_set_name]["t"] = np.arange(t_output_max + 1)
+            model_output[key] = sum(pmo[key] for pmo in part_model_outputs)
         else:
-            model_output[model_point_set_name] = pd.concat(part_output[model_point_set_name] for part_output in part_outputs)
+            model_output[key] = pd.concat(pmo[key] for pmo in part_model_outputs)
+    return model_output
 
-    if not os.path.exists("output"):
-        os.makedirs("output")
 
-    # Save output to csv
-    if settings["SAVE_OUTPUT"]:
-        print_log("Saving output:")
-        timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-        for model_point_set_name in model_point_set_names:
-            filepath = f"output/{timestamp}_{model_point_set_name}.csv"
-
-            column_names = [col for col in model_output[model_point_set_name].columns.values.tolist() if col not in ["t", "r"]]
-            if len(column_names) > 0:
-                print(f"{' ' * 10} {filepath}")
-                model_output[model_point_set_name].to_csv(filepath, index=False)
-
-    print_log("Finished")
-    return model_output
+def merge_part_runtimes(part_runtimes):
+    total_runtimes = sum([pr["runtime"] for pr in part_runtimes])
+    first = part_runtimes[0]
+    runtimes = pd.DataFrame({
+        "component": first["component"],
+        "runtime": total_runtimes
+    })
+    return runtimes
 
 
 def start(model_name, settings, argv):
+    timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
     settings = load_settings(settings)
 
-    if settings.get("MULTIPROCESSING"):
+    if settings["MULTIPROCESSING"]:
         cpu_count = multiprocessing.cpu_count()
-        p = functools.partial(execute_multiprocessing, model_name=model_name, settings=settings, cpu_count=cpu_count, argv=argv)
+        p = functools.partial(start_multiprocessing, cpu_count=cpu_count, model_name=model_name, settings=settings,
+                              argv=argv)
         with multiprocessing.Pool(cpu_count) as pool:
-            part_outputs = pool.map(p, range(cpu_count))
-        output = merge_and_save_multiprocessing(part_outputs, settings)
+            parts = pool.map(p, range(cpu_count))
+        part_model_outputs = [p[0] for p in parts]
+        output = merge_part_model_outputs(part_model_outputs, settings)
+        if settings["SAVE_RUNTIME"]:
+            part_runtimes = [p[1] for p in parts]
+            runtime = merge_part_runtimes(part_runtimes)
     else:
-        output = start_single_core(model_name, settings, argv)
+        output, runtime = start_single_core(model_name, settings, argv)
+
+    # Add time column
+    for key in output.keys():
+        values = [*range(settings["T_OUTPUT_MAX"]+1)] * int(output[key].shape[0] / (settings["T_OUTPUT_MAX"]+1))
+        output[key].insert(0, "t", values)
+
+    if settings["SAVE_OUTPUT"]:
+        print_log("Saving results:")
+        dict_to_csv(output, timestamp)
+
+    if settings["SAVE_RUNTIME"]:
+        print_log("Saving runtime:")
+        df_to_csv(runtime, timestamp)
 
+    print_log("Finished")
     return output
```

### Comparing `cashflower-0.3.3/cashflower/utils.py` & `cashflower-0.3.4/cashflower/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -180,7 +180,41 @@
     return cycle
 
 
 def cycle_to_str(cycle):
     cycle_names = [c.name for c in cycle]
     cycle_str = " --> ".join(cycle_names) + " --> " + cycle[0].name
     return cycle_str
+
+
+def get_object_by_name(objects, name):
+    for _object in objects:
+        if _object.name == name:
+            return _object
+    return None
+
+
+def lst_to_records(lst):
+    """['a', 'b', 'b', 'c', 'd', 'd', 'd', 'd', 'b'] ---> [1, 1, 2, 1, 1, 2, 3, 4, 1]"""
+    prev = None
+    output = []
+    for i, curr in enumerate(lst):
+        if i == 0:
+            output.append(1)
+        else:
+            if curr == prev:
+                output.append(output[i-1]+1)
+            else:
+                output.append(1)
+        prev = curr
+    return output
+
+
+def flatten(lst):
+    flat_list = []
+    for element in lst:
+        if type(element) is list:
+            for item in element:
+                flat_list.append(item)
+        else:
+            flat_list.append(element)
+    return flat_list
```

### Comparing `cashflower-0.3.3/cashflower.egg-info/PKG-INFO` & `cashflower-0.3.4/cashflower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.3.3
+Version: 0.3.4
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.3.3/setup.py` & `cashflower-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.3.3",
+    version="0.3.4",
 )
```

### Comparing `cashflower-0.3.3/tests/test_cashflow.py` & `cashflower-0.3.4/tests/test_cashflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
 
 from pandas.testing import assert_frame_equal
 from unittest import TestCase
 
 from cashflower.start import *
 from cashflower.cashflow import *
+from cashflower.utils import get_object_by_name
 
 
 class TestAssign(TestCase):
     def test_assign(self):
         my_var = ModelVariable()
         assert my_var.assigned_formula is None
 
@@ -21,14 +22,59 @@
 
 class TestUpdt(TestCase):
     def test_updt(self):
         assert updt(100, 20) is None
         assert updt(100, 110) is None
 
 
+class TestGetColDict(TestCase):
+    def test_get_col_dict(self):
+        settings = load_settings()
+        main = ModelPointSet(data=pd.DataFrame({"id": [1]}), name="main")
+        premium = ModelVariable(name="premium", model_point_set=main)
+        col_dict = get_col_dict(model_point_sets=[main], variables=[premium], constants=[], settings=settings)
+        output_dict = {
+            "main": {
+                "ModelVariable": ["premium"],
+                "Constant": []
+            }
+        }
+        assert col_dict == output_dict
+
+    def test_get_col_dict_with_column_subset(self):
+        settings = load_settings()
+        settings["OUTPUT_COLUMNS"] = ["b"]
+        main = ModelPointSet(data=pd.DataFrame({"id": [1]}), name="main")
+        a = ModelVariable(name="a", model_point_set=main)
+        b = ModelVariable(name="b", model_point_set=main)
+        col_dict = get_col_dict(model_point_sets=[main], variables=[a, b], constants=[], settings=settings)
+        output_dict = {
+            "main": {
+                "ModelVariable": ["b"],
+                "Constant": []
+            }
+        }
+        assert col_dict == output_dict
+
+    def test_get_col_dict_with_constant(self):
+        settings = load_settings()
+        settings["AGGREGATE"] = False
+        main = ModelPointSet(data=pd.DataFrame({"id": [1]}), name="main")
+        a = ModelVariable(name="a", model_point_set=main)
+        b = Constant(name="b", model_point_set=main)
+        col_dict = get_col_dict(model_point_sets=[main], variables=[a], constants=[b], settings=settings)
+        output_dict = {
+            "main": {
+                "ModelVariable": ["a"],
+                "Constant": ["b"]
+            }
+        }
+        assert col_dict == output_dict
+
+
 class TestRunplan(TestCase):
     def test_runplan(self):
         runplan = Runplan(data=pd.DataFrame({
             "version": [1, 2],
             "value": [57, 89]
         }))
         assert runplan.version == "1"
@@ -101,34 +147,35 @@
 
 
 class TestModelVariable(TestCase):
     def test_model_variable(self):
         premium = ModelVariable()
 
         @assign(premium)
-        def mv_formula(t):
+        def _mv(t):
             pass
 
-        assert premium.assigned_formula == mv_formula
+        assert premium.assigned_formula == _mv
 
         premium.name = "premium"
         assert repr(premium) == "ModelVariable: premium"
 
     def test_model_variable_is_lower_when_fewer_grandchildren(self):
         mv = ModelVariable()
         other_mv = ModelVariable()
         mv.grandchildren = [1, 2, 3]
         other_mv.grandchildren = [1, 3]
         assert mv > other_mv
 
     def test_model_variable_gets_called(self):
+        settings = load_settings()
         policy = ModelPointSet(
             data=pd.DataFrame({"id": [1]}),
             name="policy",
-            settings=load_settings()
+            settings=settings
         )
         policy.initialize()
 
         mv = ModelVariable(name="mv", model_point_set=policy, settings=load_settings())
 
         @assign(mv)
         def mv_formula(t):
@@ -207,15 +254,24 @@
 
         mv.initialize(policy)
         assert mv.model_point_set == policy
 
 
 class TestConstant(TestCase):
     def test_constant(self):
-        Constant()
+        premium = Constant()
+
+        @assign(premium)
+        def _c():
+            pass
+
+        assert premium.assigned_formula == _c
+
+        premium.name = "premium"
+        assert repr(premium) == "Constant: premium"
 
     def test_constant_is_lower_when_fewer_grandchildren(self):
         p1 = Constant()
         p2 = Constant()
 
         p1.grandchildren = [1, 2, 3]
         p2.grandchildren = [4, 5]
@@ -233,14 +289,17 @@
         @assign(p)
         def mv_formula():
             return 10
 
         p.initialize()
         p.calculate()
         assert p() == 10
+        assert p(0) == 10
+        with pytest.raises(CashflowModelError):
+            p(1)
 
     def test_constant_raises_error_when_formula_has_parameters(self):
         p = Constant()
 
         @assign(p)
         def mv_formula(x):
             return x
@@ -256,26 +315,30 @@
 
 
 class TestModel(TestCase):
     def test_get_component_by_name(self):
         m = ModelVariable(name="my-variable")
         p = Constant(name="my-parameter")
         model = Model(None, [m], [p], None, None)
-        assert model.get_component_by_name("my-variable") == m
-        assert model.get_component_by_name("my-parameter") == p
+        assert get_object_by_name(model.components, "my-variable") == m
+        assert get_object_by_name(model.components, "my-parameter") == p
 
     def test_get_model_point_set_by_name(self):
         mps = ModelPointSet(data=None, name="my-model-point-set")
         model = Model(None, [], [], [mps], None)
-        assert model.get_model_point_set_by_name("my-model-point-set") == mps
+        assert get_object_by_name(model.model_point_sets, "my-model-point-set") == mps
 
     def test_set_children(self):
-        a = ModelVariable(name="a")
-        b = ModelVariable(name="b")
-        c = Constant(name="c")
+        settings = load_settings()
+        main = ModelPointSet(data=pd.DataFrame({"id": [1]}), name="main", settings=settings)
+        main.initialize()
+
+        a = ModelVariable(name="a", model_point_set=main, settings=settings)
+        b = ModelVariable(name="b", model_point_set=main, settings=settings)
+        c = Constant(name="c", model_point_set=main)
 
         @assign(a)
         def a_formula(t):
             return b(t) + c() + t
 
         @assign(b)
         def b_formula(t):
@@ -339,114 +402,118 @@
         c.grandchildren = []
 
         settings = load_settings()
         model = Model(None, [a, b, c], [], None, settings)
         model.set_queue()
         assert model.queue == [c, b, a]
 
-    def test_set_empty_output(self):
-        policy = ModelPointSet(data=pd.DataFrame({"id": [1, 2, 3]}), name="policy")
-        fund = ModelPointSet(data=pd.DataFrame({"id": [1, 2, 2, 3]}), name="fund")
-
-        a = ModelVariable(name="a", model_point_set=policy)
-        b = Constant(name="b", model_point_set=policy)
-        c = ModelVariable(name="c", model_point_set=fund)
-
-        # Aggregate output
-        settings = load_settings()
-        model = Model(None, [a, c], [b], [policy, fund], settings)
-        model.set_empty_output()
-
-        empty_output = {"policy": pd.DataFrame(columns=["t", "a"]), "fund": pd.DataFrame(columns=["t", "c"])}
-        assert_frame_equal(model.empty_output["policy"], empty_output["policy"])
-        assert_frame_equal(model.empty_output["fund"], empty_output["fund"])
+    def test_queue_with_columns_subset(self):
+        settings = load_settings()
 
-        # Individual output
-        settings["AGGREGATE"] = False
-        model = Model(None, [a, c], [b], [policy, fund], settings)
-        model.set_empty_output()
+        a = ModelVariable(name="a")
+        b = ModelVariable(name="b")
+        c = ModelVariable(name="c")
 
-        empty_output = {
-            "policy": pd.DataFrame(columns=["t", "r", "a", "b"]),
-            "fund": pd.DataFrame(columns=["t", "r", "c"])
-        }
-        assert_frame_equal(model.empty_output["policy"], empty_output["policy"])
-        assert_frame_equal(model.empty_output["fund"], empty_output["fund"])
+        a.grandchildren = [c]
+        b.grandchildren = [c]
+        c.grandchildren = []
 
-    def test_calculate_single_model_point(self):
+        settings["OUTPUT_COLUMNS"] = ["a", "c"]
+        model = Model(None, [a, b, c], [], None, settings)
+        model.set_queue()
+        assert model.queue == [c, a]
+
+    def test_queue_with_columns_subset_and_unnecessary_col(self):
         settings = load_settings()
-        main = ModelPointSet(data=pd.DataFrame({"id": [1]}), name="main")
+
+        a = ModelVariable(name="a")
+        b = ModelVariable(name="b")
+        c = ModelVariable(name="c")
+
+        a.grandchildren = [c]
+        b.grandchildren = [c]
+        c.grandchildren = []
+
+        settings["OUTPUT_COLUMNS"] = ["a", "z", "c"]
+        model = Model(None, [a, b, c], [], None, settings)
+        model.set_queue()
+
+        assert model.queue == [c, a]
+
+    def test_calculate_model_point(self):
+        settings = load_settings()
+        main = ModelPointSet(data=pd.DataFrame({"id": [1]}), name="main", settings=settings)
+        main.initialize()
 
         premium = ModelVariable(name="premium", model_point_set=main, settings=settings)
 
         @assign(premium)
         def mv_formula(t):
             return 1
 
         premium.initialize()
 
         model = Model(None, [premium], [], [main], settings)
         model.initialize()
-        model_point_output = model.calculate_single_model_point(0, 1, main)
-        test_output = pd.DataFrame({
-            "premium": [1.0] * (settings.get("T_OUTPUT_MAX") + 1)
-        })
-        assert_frame_equal(model_point_output["main"][["premium"]], test_output)
+        col_dict = get_col_dict(model.model_point_sets, model.variables, model.constants, model.settings)
+        model_point_output = model.calculate_model_point(0, 1, main, col_dict)
+        left = model_point_output["main"]["ModelVariable"][:, 0]
+        right = np.array([1.0] * (settings.get("T_OUTPUT_MAX") + 1))
+        assert all(left == right)
 
     def test_calculate(self):
         settings = load_settings()
-        main = ModelPointSet(data=pd.DataFrame({"id": [1, 2]}), name="main")
+        main = ModelPointSet(data=pd.DataFrame({"id": [1, 2]}), name="main", settings=settings)
+        main.initialize()
 
-        premium = ModelVariable(name="a", model_point_set=main, settings=settings)
+        premium = ModelVariable(name="premium", model_point_set=main, settings=settings)
 
         @assign(premium)
-        def premium_formula(t):
+        def _premium(t):
             return t + 100
 
         premium.initialize()
 
         # Aggregated output
         model = Model(None, [premium], [], [main], settings)
         model.initialize()
 
-        model_output = model.calculate()
+        model_output = model.calculate_model()
         test_output = pd.DataFrame({
-            "t": list(range(1201)),
-            "a": [2 * (i + 100) for i in range(1201)]
+            "premium": [2 * (i + 100) for i in range(1201)]
         })
 
         assert_frame_equal(model_output["main"], test_output, check_dtype=False)
 
         # Individual output
         settings["AGGREGATE"] = False
         model = Model(None, [premium], [], [main], settings)
         model.initialize()
 
-        model_output = model.calculate()
+        model_output = model.calculate_model()
         test_output = pd.DataFrame({
-            "t": list(range(1201)) * 2,
             "r": [1 for _ in range(1201 * 2)],
-            "a": [(i + 100) for i in range(1201)] * 2
+            "premium": [(i + 100) for i in range(1201)] * 2
         })
 
         assert_frame_equal(model_output["main"].reset_index(drop=True), test_output.reset_index(drop=True), check_dtype=False)
 
     def test_run(self):
         settings = load_settings()
-        main = ModelPointSet(data=pd.DataFrame({"id": [1, 2]}), name="main")
+        main = ModelPointSet(data=pd.DataFrame({"id": [1, 2]}), name="main", settings=settings)
+        main.initialize()
 
-        premium = ModelVariable(name="a", model_point_set=main, settings=settings)
+        premium = ModelVariable(name="premium", model_point_set=main, settings=settings)
 
         @assign(premium)
-        def premium_formula(t):
+        def _premium(t):
             return t + 100
 
         premium.initialize()
 
-        test_output = pd.DataFrame({
-            "t": list(range(1201)),
-            "a": [2 * (i + 100) for i in range(1201)]
-        })
+        test_output = pd.DataFrame({"premium": [2 * (i + 100) for i in range(1201)]})
 
         model = Model(None, [premium], [], [main], settings)
-        model_output = model.run()
+        model.initialize()
+
+        model_output, _ = model.run()
         assert_frame_equal(model_output["main"], test_output, check_dtype=False)
```

### Comparing `cashflower-0.3.3/tests/test_start.py` & `cashflower-0.3.4/tests/test_start.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             "AGGREGATE": True,
             "MULTIPROCESSING": False,
             "OUTPUT_COLUMNS": ["a", "b", "c"],
             "ID_COLUMN": "polnumber",
             "SAVE_OUTPUT": True,
             "SAVE_RUNTIME": False,
             "T_CALCULATION_MAX": 100,
-            "T_OUTPUT_MAX": 1200,
+            "T_OUTPUT_MAX": 100,
         }
 
 
 class TestGetRunplan(TestCase):
     def test_get_runplan(self):
         runplan = Runplan()
         input_members = [("foo", "foo"), ("runplan", runplan), ("bar", "bar")]
@@ -139,14 +139,18 @@
         shutil.rmtree("output")
         test_output = pd.DataFrame({
             "t": range(settings["T_CALCULATION_MAX"]+1),
             "projection_year": [0] + [x for x in range(1, 101) for _ in range(12)],
         })
         assert_frame_equal(model_output["main"], test_output, check_dtype=False)
 
+    def test_simple_model_runs_multiprocessing(self):
+        model_name = "my_test_model"
+        settings = load_settings()
+
         # Multiprocessing
         settings["MULTIPROCESSING"] = True
         create_model(model_name)
         model_output = start(model_name, settings, [])
         shutil.rmtree(model_name)
         shutil.rmtree("output")
         test_output = pd.DataFrame({
```

### Comparing `cashflower-0.3.3/tests/test_utils.py` & `cashflower-0.3.4/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -127,7 +127,34 @@
         a = Object(name="a")
         b = Object(name="b")
 
         cycle = [b, a]
         result = cycle_to_str(cycle)
         assert result == "b --> a --> b"
 
+
+class TestGetObjectByName(TestCase):
+    def test_get_object_by_name(self):
+        class Object:
+            def __init__(self, name):
+                self.name = name
+
+        a = Object(name="a")
+        b = Object(name="b")
+        objects = [a, b]
+
+        assert get_object_by_name(objects, "a") == a
+        assert get_object_by_name(objects, "c") is None
+
+
+class TestLstToRecords(TestCase):
+    def test_lst_to_records(self):
+        left = ['a', 'b', 'b', 'c', 'd', 'd', 'd', 'd', 'b']
+        right = [1, 1, 2, 1, 1, 2, 3, 4, 1]
+        assert lst_to_records(left) == right
+
+
+class TestFlatten(TestCase):
+    def test_flatten(self):
+        lst = [1, [2, 3, 4], 5]
+        flat_lst = [1, 2, 3, 4, 5]
+        assert flatten(lst) == flat_lst
```

