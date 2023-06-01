# Comparing `tmp/eargait-1.8.0.tar.gz` & `tmp/eargait-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eargait-1.8.0.tar", max compression
+gzip compressed data, was "eargait-1.9.0.tar", max compression
```

## Comparing `eargait-1.8.0.tar` & `eargait-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1072 2023-05-22 07:08:27.065757 eargait-1.8.0/LICENSE
--rw-r--r--   0        0        0     5531 2023-05-22 07:08:27.065757 eargait-1.8.0/README.md
--rw-r--r--   0        0        0      154 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/base/__init__.py
--rw-r--r--   0        0        0     5028 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/base/base_eargait.py
--rw-r--r--   0        0        0    13447 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/eargait.py
--rw-r--r--   0        0        0      411 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/event_detection/__init__.py
--rw-r--r--   0        0        0    10101 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/event_detection/base_event_detection.py
--rw-r--r--   0        0        0     4990 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/event_detection/diao_adapted_event_detection.py
--rw-r--r--   0        0        0     8327 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/event_detection/diao_event_detection.py
--rw-r--r--   0        0        0     9077 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/event_detection/jarchi_event_detection.py
--rw-r--r--   0        0        0     9367 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/event_detection/mixed_event_detection.py
--rw-r--r--   0        0        0      307 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/preprocessing/__init__.py
--rw-r--r--   0        0        0     2275 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/preprocessing/load_data_helpers.py
--rw-r--r--   0        0        0     6833 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/preprocessing/rotations.py
--rw-r--r--   0        0        0      204 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/spatial_params/__init__.py
--rw-r--r--   0        0        0      296 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/spatial_params/spatial_params_base.py
--rw-r--r--   0        0        0     1340 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/spatial_params/spatial_params_example_class.py
--rw-r--r--   0        0        0        0 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/utils/__init__.py
--rw-r--r--   0        0        0      609 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/utils/consts.py
--rw-r--r--   0        0        0     1334 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/utils/example_data.py
--rw-r--r--   0        0        0     5535 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/utils/gait_parameters.py
--rw-r--r--   0        0        0     3809 2023-05-22 07:08:27.073757 eargait-1.8.0/eargait/utils/helper_datatype.py
--rw-r--r--   0        0        0    58133 2023-05-22 07:08:27.077757 eargait-1.8.0/eargait/utils/helper_gaitmap.py
--rw-r--r--   0        0        0     2033 2023-05-22 07:08:27.077757 eargait-1.8.0/eargait/utils/helpers.py
--rw-r--r--   0        0        0     2458 2023-05-22 07:08:27.129757 eargait-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 eargait-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 11:27:24.434605 eargait-1.9.0/LICENSE
+-rw-r--r--   0        0        0     5531 2023-05-24 11:27:24.434605 eargait-1.9.0/README.md
+-rw-r--r--   0        0        0      154 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/base/__init__.py
+-rw-r--r--   0        0        0     5028 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/base/base_eargait.py
+-rw-r--r--   0        0        0    13447 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/eargait.py
+-rw-r--r--   0        0        0      411 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/event_detection/__init__.py
+-rw-r--r--   0        0        0    10118 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/event_detection/base_event_detection.py
+-rw-r--r--   0        0        0     4990 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/event_detection/diao_adapted_event_detection.py
+-rw-r--r--   0        0        0     8327 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/event_detection/diao_event_detection.py
+-rw-r--r--   0        0        0     9077 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/event_detection/jarchi_event_detection.py
+-rw-r--r--   0        0        0     9367 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/event_detection/mixed_event_detection.py
+-rw-r--r--   0        0        0      307 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2275 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/preprocessing/load_data_helpers.py
+-rw-r--r--   0        0        0     6833 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/preprocessing/rotations.py
+-rw-r--r--   0        0        0      204 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/spatial_params/__init__.py
+-rw-r--r--   0        0        0      296 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/spatial_params/spatial_params_base.py
+-rw-r--r--   0        0        0     1340 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/spatial_params/spatial_params_example_class.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/utils/__init__.py
+-rw-r--r--   0        0        0      609 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/utils/consts.py
+-rw-r--r--   0        0        0     1334 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/utils/example_data.py
+-rw-r--r--   0        0        0     5535 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/utils/gait_parameters.py
+-rw-r--r--   0        0        0     3809 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/utils/helper_datatype.py
+-rw-r--r--   0        0        0    58133 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/utils/helper_gaitmap.py
+-rw-r--r--   0        0        0     2033 2023-05-24 11:27:24.442605 eargait-1.9.0/eargait/utils/helpers.py
+-rw-r--r--   0        0        0     2458 2023-05-24 11:27:24.506604 eargait-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 eargait-1.9.0/PKG-INFO
```

### Comparing `eargait-1.8.0/LICENSE` & `eargait-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/README.md` & `eargait-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/base/base_eargait.py` & `eargait-1.9.0/eargait/base/base_eargait.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/eargait.py` & `eargait-1.9.0/eargait/eargait.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/event_detection/base_event_detection.py` & `eargait-1.9.0/eargait/event_detection/base_event_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         set_params_from_dict(self, results, result_formatting=True)
         return self
 
     @property
     def event_list_consistent_(self: Self):
         """Consistent based on alternating ipsi- and contralateral steps, non-consistent steps are set to NaN."""
         assert self._has_event_list()
-        dataset_type = is_sensor_data(self.data, frame="body")
+        dataset_type = is_sensor_data(self.data, frame="body", check_gyr=False)
         if dataset_type == "single":
             event_list_consistent_ = self._single_consistent_event_list(self.event_list_)
         else:
             event_list_consistent_: Dict[Hashable, Dict[str, pd.DataFrame]] = {}
             for sensor in get_multi_sensor_names(self.event_list_):
                 event_list_consistent_[sensor] = self._single_consistent_event_list(self.event_list_[sensor])
         return event_list_consistent_
```

### Comparing `eargait-1.8.0/eargait/event_detection/diao_adapted_event_detection.py` & `eargait-1.9.0/eargait/event_detection/diao_adapted_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/event_detection/diao_event_detection.py` & `eargait-1.9.0/eargait/event_detection/diao_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/event_detection/jarchi_event_detection.py` & `eargait-1.9.0/eargait/event_detection/jarchi_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/event_detection/mixed_event_detection.py` & `eargait-1.9.0/eargait/event_detection/mixed_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/preprocessing/load_data_helpers.py` & `eargait-1.9.0/eargait/preprocessing/load_data_helpers.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/preprocessing/rotations.py` & `eargait-1.9.0/eargait/preprocessing/rotations.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/spatial_params/spatial_params_example_class.py` & `eargait-1.9.0/eargait/spatial_params/spatial_params_example_class.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/utils/consts.py` & `eargait-1.9.0/eargait/utils/consts.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/utils/example_data.py` & `eargait-1.9.0/eargait/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/utils/gait_parameters.py` & `eargait-1.9.0/eargait/utils/gait_parameters.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/utils/helper_datatype.py` & `eargait-1.9.0/eargait/utils/helper_datatype.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/utils/helper_gaitmap.py` & `eargait-1.9.0/eargait/utils/helper_gaitmap.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/eargait/utils/helpers.py` & `eargait-1.9.0/eargait/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `eargait-1.8.0/pyproject.toml` & `eargait-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eargait"
-version = "1.8.0"
+version = "1.9.0"
 description = "*Eargait* provides a set of algorithms and functions to process IMU data recorded with ear-worn IMU sensors and to estimate characteristic gait parameters. "
 authors = ["Ann-Kristin Seifer <ann-kristin.seifer@fau.de>",
             "Arne Küderle <arne.kuederle@fau.de>"]
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/eargait"
 repository = "https://github.com/mad-lab-fau/eargait"
```

### Comparing `eargait-1.8.0/PKG-INFO` & `eargait-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eargait
-Version: 1.8.0
+Version: 1.9.0
 Summary: *Eargait* provides a set of algorithms and functions to process IMU data recorded with ear-worn IMU sensors and to estimate characteristic gait parameters. 
 Home-page: https://github.com/mad-lab-fau/eargait
 Author: Ann-Kristin Seifer
 Author-email: ann-kristin.seifer@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

