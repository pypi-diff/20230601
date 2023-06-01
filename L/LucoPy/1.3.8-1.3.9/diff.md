# Comparing `tmp/LucoPy-1.3.8.tar.gz` & `tmp/LucoPy-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LucoPy-1.3.8.tar", last modified: Tue Feb 21 13:14:23 2023, max compression
+gzip compressed data, was "LucoPy-1.3.9.tar", last modified: Thu Mar 16 09:16:20 2023, max compression
```

## Comparing `LucoPy-1.3.8.tar` & `LucoPy-1.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-21 13:14:23.660815 LucoPy-1.3.8/
--rw-r--r--   0 vsts      (1001) docker     (123)     1073 2023-02-21 13:14:07.000000 LucoPy-1.3.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)    18111 2023-02-21 13:14:23.660815 LucoPy-1.3.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    17696 2023-02-21 13:14:07.000000 LucoPy-1.3.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       84 2023-02-21 13:14:07.000000 LucoPy-1.3.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-02-21 13:14:23.660815 LucoPy-1.3.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)       37 2023-02-21 13:14:07.000000 LucoPy-1.3.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-21 13:14:23.648815 LucoPy-1.3.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-21 13:14:23.656815 LucoPy-1.3.8/src/LucoPy/
--rw-r--r--   0 vsts      (1001) docker     (123)     4787 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/ApiCore.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13217 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/LucoApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12833 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/Submissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      176 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/Utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)       51 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      371 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/api_helpers.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-21 13:14:23.656815 LucoPy-1.3.8/src/LucoPy/data_quality/
--rw-r--r--   0 vsts      (1001) docker     (123)       55 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/data_quality/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3415 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/data_quality/data_quality.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-21 13:14:23.660815 LucoPy-1.3.8/src/LucoPy/data_quality/great_expectations/
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/data_quality/great_expectations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7768 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/data_quality/great_expectations/great_expectations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1542 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/data_quality/great_expectations/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)      518 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/data_quality/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)      131 2023-02-21 13:14:07.000000 LucoPy-1.3.8/src/LucoPy/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-21 13:14:23.656815 LucoPy-1.3.8/src/LucoPy.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)    18111 2023-02-21 13:14:23.000000 LucoPy-1.3.8/src/LucoPy.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      665 2023-02-21 13:14:23.000000 LucoPy-1.3.8/src/LucoPy.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-02-21 13:14:23.000000 LucoPy-1.3.8/src/LucoPy.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        9 2023-02-21 13:14:23.000000 LucoPy-1.3.8/src/LucoPy.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        7 2023-02-21 13:14:23.000000 LucoPy-1.3.8/src/LucoPy.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-16 09:16:20.026659 LucoPy-1.3.9/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1073 2023-03-16 09:16:01.000000 LucoPy-1.3.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)    18158 2023-03-16 09:16:20.026659 LucoPy-1.3.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    17743 2023-03-16 09:16:01.000000 LucoPy-1.3.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       84 2023-03-16 09:16:01.000000 LucoPy-1.3.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-03-16 09:16:20.026659 LucoPy-1.3.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)       37 2023-03-16 09:16:01.000000 LucoPy-1.3.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-16 09:16:20.022659 LucoPy-1.3.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-16 09:16:20.022659 LucoPy-1.3.9/src/LucoPy/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4787 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/ApiCore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13217 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/LucoApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12608 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/Submissions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      176 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/Utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       51 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      371 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/api_helpers.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-16 09:16:20.026659 LucoPy-1.3.9/src/LucoPy/data_quality/
+-rw-r--r--   0 vsts      (1001) docker     (123)       55 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/data_quality/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3415 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/data_quality/data_quality.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-16 09:16:20.026659 LucoPy-1.3.9/src/LucoPy/data_quality/great_expectations/
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/data_quality/great_expectations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7768 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/data_quality/great_expectations/great_expectations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1542 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/data_quality/great_expectations/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      518 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/data_quality/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      131 2023-03-16 09:16:01.000000 LucoPy-1.3.9/src/LucoPy/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-16 09:16:20.026659 LucoPy-1.3.9/src/LucoPy.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18158 2023-03-16 09:16:20.000000 LucoPy-1.3.9/src/LucoPy.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      665 2023-03-16 09:16:20.000000 LucoPy-1.3.9/src/LucoPy.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-16 09:16:20.000000 LucoPy-1.3.9/src/LucoPy.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        9 2023-03-16 09:16:20.000000 LucoPy-1.3.9/src/LucoPy.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        7 2023-03-16 09:16:20.000000 LucoPy-1.3.9/src/LucoPy.egg-info/top_level.txt
```

### Comparing `LucoPy-1.3.8/LICENSE` & `LucoPy-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LucoPy-1.3.8/PKG-INFO` & `LucoPy-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LucoPy
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python SDK to support the Luco data observability tool.
 Author: Redkite
 Author-email: luco.support@redkite.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -426,14 +426,16 @@
 check = convert_expectation_to_check(expectation_result,
                                      metadata_mappings=expectation_mapping)
 ```
 
 ---
 
 ## Version History
+LucoPy-1.3.9 : Bug fix: get_quality() method.
+
 LucoPy-1.3.8 : Bug fixes to great_expectations module and export_slot_sequences method.
 
 LucoPy-1.3.7 : DQ module improvements. Define attributes of CheckResult and CollectionResult objects. Add `to_dict()` methods to construct dictionary of required and optional attributes which are not None. New method: LucoApi.export_slot_sequences.
 
 LucoPy-1.3.6 : Refactor `Submission.get_metrics()` to remove breaking change. Added `group_by_stage` kwarg to group metrics.
 
 LucoPy-1.3.5 : DQ module improvements. Add options to auto determine `action` and raise exception.
```

### Comparing `LucoPy-1.3.8/README.md` & `LucoPy-1.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,16 @@
 check = convert_expectation_to_check(expectation_result,
                                      metadata_mappings=expectation_mapping)
 ```
 
 ---
 
 ## Version History
+LucoPy-1.3.9 : Bug fix: get_quality() method.
+
 LucoPy-1.3.8 : Bug fixes to great_expectations module and export_slot_sequences method.
 
 LucoPy-1.3.7 : DQ module improvements. Define attributes of CheckResult and CollectionResult objects. Add `to_dict()` methods to construct dictionary of required and optional attributes which are not None. New method: LucoApi.export_slot_sequences.
 
 LucoPy-1.3.6 : Refactor `Submission.get_metrics()` to remove breaking change. Added `group_by_stage` kwarg to group metrics.
 
 LucoPy-1.3.5 : DQ module improvements. Add options to auto determine `action` and raise exception.
```

### Comparing `LucoPy-1.3.8/setup.cfg` & `LucoPy-1.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = LucoPy
-version = 1.3.8
+version = 1.3.9
 author = Redkite
 author_email = luco.support@redkite.com
 description = Python SDK to support the Luco data observability tool.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers =
```

### Comparing `LucoPy-1.3.8/src/LucoPy/ApiCore.py` & `LucoPy-1.3.9/src/LucoPy/ApiCore.py`

 * *Files identical despite different names*

### Comparing `LucoPy-1.3.8/src/LucoPy/LucoApi.py` & `LucoPy-1.3.9/src/LucoPy/LucoApi.py`

 * *Files identical despite different names*

### Comparing `LucoPy-1.3.8/src/LucoPy/Submissions.py` & `LucoPy-1.3.9/src/LucoPy/Submissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,23 +182,17 @@
         
         Returns:
             quality (dict)
         """
         endpoint = f'/v2/slots/{self.slot_id}/submissions/{self.id}/quality'
 
         r = self.core.get_request(endpoint)
-        r.raise_for_status()
+        collections = r.json()['collections']
 
-        response_json = r.json()
-
-        for i, result in enumerate(response_json['qualityResults']):
-            quality_results = json.loads(result['results'])
-            response_json['qualityResults'][i]['results'] = quality_results
-
-        return response_json
+        return collections
 
     def submit_run_environment(self, stage=None, run_environments=None):
         """
         Submit run environment details
 
         Args:
             stage (string) : Optional
```

### Comparing `LucoPy-1.3.8/src/LucoPy/data_quality/data_quality.py` & `LucoPy-1.3.9/src/LucoPy/data_quality/data_quality.py`

 * *Files identical despite different names*

### Comparing `LucoPy-1.3.8/src/LucoPy/data_quality/great_expectations/great_expectations.py` & `LucoPy-1.3.9/src/LucoPy/data_quality/great_expectations/great_expectations.py`

 * *Files identical despite different names*

### Comparing `LucoPy-1.3.8/src/LucoPy/data_quality/great_expectations/utils.py` & `LucoPy-1.3.9/src/LucoPy/data_quality/great_expectations/utils.py`

 * *Files identical despite different names*

### Comparing `LucoPy-1.3.8/src/LucoPy/data_quality/utils.py` & `LucoPy-1.3.9/src/LucoPy/data_quality/utils.py`

 * *Files identical despite different names*

### Comparing `LucoPy-1.3.8/src/LucoPy.egg-info/PKG-INFO` & `LucoPy-1.3.9/src/LucoPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LucoPy
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python SDK to support the Luco data observability tool.
 Author: Redkite
 Author-email: luco.support@redkite.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -426,14 +426,16 @@
 check = convert_expectation_to_check(expectation_result,
                                      metadata_mappings=expectation_mapping)
 ```
 
 ---
 
 ## Version History
+LucoPy-1.3.9 : Bug fix: get_quality() method.
+
 LucoPy-1.3.8 : Bug fixes to great_expectations module and export_slot_sequences method.
 
 LucoPy-1.3.7 : DQ module improvements. Define attributes of CheckResult and CollectionResult objects. Add `to_dict()` methods to construct dictionary of required and optional attributes which are not None. New method: LucoApi.export_slot_sequences.
 
 LucoPy-1.3.6 : Refactor `Submission.get_metrics()` to remove breaking change. Added `group_by_stage` kwarg to group metrics.
 
 LucoPy-1.3.5 : DQ module improvements. Add options to auto determine `action` and raise exception.
```

### Comparing `LucoPy-1.3.8/src/LucoPy.egg-info/SOURCES.txt` & `LucoPy-1.3.9/src/LucoPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

