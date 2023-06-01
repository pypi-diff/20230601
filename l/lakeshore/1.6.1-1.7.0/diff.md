# Comparing `tmp/lakeshore-1.6.1.tar.gz` & `tmp/lakeshore-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakeshore-1.6.1.tar", last modified: Fri Apr 21 15:42:02 2023, max compression
+gzip compressed data, was "lakeshore-1.7.0.tar", last modified: Thu Jun  1 19:16:31 2023, max compression
```

## Comparing `lakeshore-1.6.1.tar` & `lakeshore-1.7.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:42:02.980605 lakeshore-1.6.1/
--rw-rw-rw-   0        0        0     4167 2023-04-21 15:41:25.000000 lakeshore-1.6.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1106 2023-04-21 15:41:25.000000 lakeshore-1.6.1/LICENSE
--rw-rw-rw-   0        0        0       48 2023-04-21 15:41:25.000000 lakeshore-1.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4958 2023-04-21 15:42:02.980605 lakeshore-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     4525 2023-04-21 15:41:25.000000 lakeshore-1.6.1/README.md
--rw-rw-rw-   0        0        0        5 2023-04-21 15:41:25.000000 lakeshore-1.6.1/VERSION
-drwxrwxrwx   0        0        0        0 2023-04-21 15:42:02.964980 lakeshore-1.6.1/lakeshore/
--rw-rw-rw-   0        0        0     1384 2023-04-21 15:41:25.000000 lakeshore-1.6.1/lakeshore/__init__.py
--rw-rw-rw-   0        0        0    63668 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/fast_hall_controller.py
--rw-rw-rw-   0        0        0    10942 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/generic_instrument.py
--rw-rw-rw-   0        0        0     1065 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_121.py
--rw-rw-rw-   0        0        0    17159 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_155.py
--rw-rw-rw-   0        0        0    54949 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_224.py
--rw-rw-rw-   0        0        0    18745 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_240.py
--rw-rw-rw-   0        0        0    30747 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_335.py
--rw-rw-rw-   0        0        0    31409 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_336.py
--rw-rw-rw-   0        0        0     1069 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_350.py
--rw-rw-rw-   0        0        0    72172 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_372.py
--rw-rw-rw-   0        0        0     1025 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_425.py
--rw-rw-rw-   0        0        0     1071 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_643.py
--rw-rw-rw-   0        0        0     1057 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_648.py
--rw-rw-rw-   0        0        0     1120 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/requires_firmware_version.py
--rw-rw-rw-   0        0        0     1404 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_base_module.py
--rw-rw-rw-   0        0        0    38123 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_measure_module.py
--rw-rw-rw-   0        0        0     3608 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_settings_profiles.py
--rw-rw-rw-   0        0        0    48487 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_source_module.py
--rw-rw-rw-   0        0        0    22443 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_system.py
--rw-rw-rw-   0        0        0     4941 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_system_enums.py
--rw-rw-rw-   0        0        0    60182 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/temperature_controllers.py
--rw-rw-rw-   0        0        0    29728 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/teslameter.py
--rw-rw-rw-   0        0        0    15782 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/xip_instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:42:02.980605 lakeshore-1.6.1/lakeshore.egg-info/
--rw-rw-rw-   0        0        0     4958 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      873 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 15:42:02.980605 lakeshore-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-04-21 15:41:25.000000 lakeshore-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:16:31.514281 lakeshore-1.7.0/
+-rw-rw-rw-   0        0        0     4350 2023-06-01 19:15:43.000000 lakeshore-1.7.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1106 2023-06-01 19:15:43.000000 lakeshore-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0       48 2023-06-01 19:15:43.000000 lakeshore-1.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4958 2023-06-01 19:16:31.514281 lakeshore-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4525 2023-06-01 19:15:43.000000 lakeshore-1.7.0/README.md
+-rw-rw-rw-   0        0        0        5 2023-06-01 19:15:43.000000 lakeshore-1.7.0/VERSION
+drwxrwxrwx   0        0        0        0 2023-06-01 19:16:31.514281 lakeshore-1.7.0/lakeshore/
+-rw-rw-rw-   0        0        0     1384 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/__init__.py
+-rw-rw-rw-   0        0        0    63499 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/fast_hall_controller.py
+-rw-rw-rw-   0        0        0    12933 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/generic_instrument.py
+-rw-rw-rw-   0        0        0     1599 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_121.py
+-rw-rw-rw-   0        0        0    16931 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_155.py
+-rw-rw-rw-   0        0        0    53128 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_224.py
+-rw-rw-rw-   0        0        0    18804 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_240.py
+-rw-rw-rw-   0        0        0    29897 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_335.py
+-rw-rw-rw-   0        0        0    30394 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_336.py
+-rw-rw-rw-   0        0        0     1071 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_350.py
+-rw-rw-rw-   0        0        0    71162 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_372.py
+-rw-rw-rw-   0        0        0     1027 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_425.py
+-rw-rw-rw-   0        0        0     1073 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_643.py
+-rw-rw-rw-   0        0        0     1059 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/model_648.py
+-rw-rw-rw-   0        0        0     1114 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/requires_firmware_version.py
+-rw-rw-rw-   0        0        0     1406 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/ssm_base_module.py
+-rw-rw-rw-   0        0        0    38608 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/ssm_measure_module.py
+-rw-rw-rw-   0        0        0     3832 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/ssm_settings_profiles.py
+-rw-rw-rw-   0        0        0    48535 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/ssm_source_module.py
+-rw-rw-rw-   0        0        0    22671 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/ssm_system.py
+-rw-rw-rw-   0        0        0     4965 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/ssm_system_enums.py
+-rw-rw-rw-   0        0        0    59168 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/temperature_controllers.py
+-rw-rw-rw-   0        0        0    29875 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/teslameter.py
+-rw-rw-rw-   0        0        0    16196 2023-06-01 19:15:44.000000 lakeshore-1.7.0/lakeshore/xip_instrument.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:16:31.514281 lakeshore-1.7.0/lakeshore.egg-info/
+-rw-rw-rw-   0        0        0     4958 2023-06-01 19:16:31.000000 lakeshore-1.7.0/lakeshore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2023-06-01 19:16:31.000000 lakeshore-1.7.0/lakeshore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:16:31.000000 lakeshore-1.7.0/lakeshore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-06-01 19:16:31.000000 lakeshore-1.7.0/lakeshore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 19:16:31.000000 lakeshore-1.7.0/lakeshore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:16:31.514281 lakeshore-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-06-01 19:15:43.000000 lakeshore-1.7.0/setup.py
```

### Comparing `lakeshore-1.6.1/CHANGELOG.md` & `lakeshore-1.7.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Change Log
 ==========
 
+Release 1.7.0
+-------------
+Added:
+- Alternative instrument connection support (Ex. GPIB)
+- Frequency sweep support for M81
+
+Fixed:
+- Inconsistencies in documentation style
+
 Release 1.6.1
 -------------
 Added:
 - Added explicit requirement for packaging package
 
 Fixed:
 - Catch error on wakepy import that breaks in some scenarios
```

### Comparing `lakeshore-1.6.1/LICENSE` & `lakeshore-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.1/PKG-INFO` & `lakeshore-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeshore
-Version: 1.6.1
+Version: 1.7.0
 Summary: A package to connect to and interact with Lake Shore instruments.
 Home-page: https://github.com/lakeshorecryotronics/python-driver
 Maintainer: Lake Shore Cryotronics, Inc.
 Maintainer-email: service@lakeshore.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lakeshore-1.6.1/README.md` & `lakeshore-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.1/lakeshore/__init__.py` & `lakeshore-1.7.0/lakeshore/__init__.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.1/lakeshore/fast_hall_controller.py` & `lakeshore-1.7.0/lakeshore/fast_hall_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Implements functionality unique to the Lake Shore M91 Fast Hall"""
+"""Implements functionality unique to the Lake Shore M91 Fast Hall."""
 
 import json
 from .xip_instrument import XIPInstrument, RegisterBase, StatusByteRegister, StandardEventRegister
 
 
 class FastHallOperationRegister(RegisterBase):
-    """Class object representing the operation status register"""
+    """Class object representing the operation status register."""
 
     bit_names = [
         "",
         "",
         "",
         "",
         "measuring_Done"
@@ -29,15 +29,15 @@
         self.waiting_for_trigger = waiting_for_trigger
         self.field_control_ramping = field_control_ramping
         self.field_measurement_enabled = field_measurement_enabled
         self.transient = transient
 
 
 class FastHallQuestionableRegister(RegisterBase):
-    """Class object representing the questionable status register"""
+    """Class object representing the questionable status register."""
 
     bit_names = [
         "source_in_compliance_or_at_current_limit",
         "negative_resistivity",
         "",
         "",
         "",
@@ -90,193 +90,159 @@
                  measurement_range='AUTO',
                  min_r_squared=0.9999,
                  blanking_time=2e-3):
         """The constructor for ContackCheckManualParameters class.
 
             Args:
                 excitation_type (str):
-                    * The excitation type used for the measurement. Options are:
-                    * "CURRENT"
-                    * "VOLTAGE"
-
+                    The excitation type used for the measurement. Options are: "CURRENT" and "VOLTAGE".
                 excitation_start_value (float):
-                    The starting excitation value For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A
-
+                    The starting excitation value For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A.
                 excitation_end_value (float):
-                    The ending excitation value For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A
-
+                    The ending excitation value For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A.
                 excitation_range (float or str):
-                    * Excitation range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V: voltage excitation
-                        - amps in the range of -100e-3 to 100e-3 A: current excitation
-
+                    Excitation range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 measurement_range (float or str):
-                    * Measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - amps in the range of 0 to 100e-3A: voltage excitation
-                        - volts in the range of 0 to 10.0V: current excitation
-
+                    Measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either amps in the range of 0 to 100e-3A for voltage excitation, or
+                    volts in the range of 0 to 10.0V for current excitation.
                 compliance_limit (float):
-                    For voltage excitation, specify the current limit 100e-9 to 100e-3 A For current excitation,
-                    specify the voltage compliance 1.00 to 10.0 V
-
+                    For voltage excitation, specify the current limit 100e-9 to 100e-3 A. For current excitation,
+                    specify the voltage compliance 1.00 to 10.0 V.
                 number_of_points (int):
-                    The number of points to measure between the excitation start and end. 0 - 100
-
+                    The number of points to measure between the excitation start and end. 0 - 100.
                 min_r_squared (float):
                     The minimum R^2 desired. Default is 0.9999.
-
                 blanking_time (float or str):
-                    * The time in seconds to wait for hardware to settle before gathering readings. Range of time is
-                      0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
-                    * "DEF" (Default) = 2 ms
-                    * "MIN" = 0.5 ms
-                    * "MAX" = 300 s
-                    * floating point number of seconds
+                    The time in seconds to wait for hardware to settle before gathering readings. Range of time is
+                    0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
+                    "DEF" (Default) = 2 ms,
+                    "MIN" = 0.5 ms,
+                    "MAX" = 300 s, or a
+                    floating point number of seconds.
         """
         self.excitation_type = excitation_type
         self.excitation_start_value = excitation_start_value
         self.excitation_end_value = excitation_end_value
         self.excitation_range = excitation_range
         self.measurement_range = measurement_range
         self.compliance_limit = compliance_limit
         self.number_of_points = number_of_points
         self.min_r_squared = min_r_squared
         self.blanking_time = blanking_time
 
 
 class ContactCheckOptimizedParameters:
-    """Class object representing parameters used for optimized Contact Check run methods"""
+    """Class object representing parameters used for optimized Contact Check run methods."""
     def __init__(self,
                  max_current=100e-3,
                  max_voltage=10,
                  number_of_points=11,
                  min_r_squared=0.9999):
         """The constructor for ContactCheckOptimizedParameters class.
 
             Args:
                 max_current(float or str):
-                    * A 'not to exceed' output current value for the auto algorithm to use. Options are:
-                    * "MIN" = 1 uA
-                    * "MAX" = 100 mA
-                    * "DEF" (Default) = 100 mA
-                    * floating point number of amps
-
+                    A 'not to exceed' output current value for the auto algorithm to use. Options are:
+                    "MIN" = 1 uA,
+                    "MAX" = 100 mA,
+                    "DEF" (Default) = 100 mA, or
+                    floating point number of amps.
                 max_voltage(float or str):
-                    * A 'not to exceed' output voltage value for the auto algorithm to use. Options are:
-                    * "MIN" = 1 V
-                    * "MAX" = 10 V
-                    * "DEF" (Default) = 10 V
-                    * floating point number of volts
-
+                    A 'not to exceed' output voltage value for the auto algorithm to use. Options are:
+                    "MIN" = 1 V,
+                    "MAX" = 10 V,
+                    "DEF" (Default) = 10 V, or
+                    floating point number of volts.
                 number_of_points(int or str):
-                    * The number of points to measure between the excitation start and end. Options are:
-                    * "MIN" = 2
-                    * "MAX" = 100
-                    * "DEF" (Default) = 11
-                    * integer number of points
-
+                    The number of points to measure between the excitation start and end. Options are:
+                    "MIN" = 2,
+                    "MAX" = 100,
+                    "DEF" (Default) = 11, or
+                    an integer number of points.
                 min_r_squared(float):
                     The minimum R^2 desired. Default is 0.9999.
         """
         self.max_current = max_current
         self.max_voltage = max_voltage
         self.number_of_points = number_of_points
         self.min_r_squared = min_r_squared
 
 
 class FastHallManualParameters:
-    """Class object representing parameters used for running manual FastHall measurements"""
+    """Class object representing parameters used for running manual FastHall measurements."""
     def __init__(self,
                  excitation_type,
                  excitation_value,
                  user_defined_field,
                  compliance_limit,
                  excitation_range='AUTO',
                  excitation_measurement_range='AUTO',
                  measurement_range='AUTO',
                  max_samples=100,
                  resistivity='"NaN"',
                  blanking_time=2e-3,
                  averaging_samples=60,
                  sample_thickness=0,
                  min_hall_voltage_snr=30):
-        """The constructor for FastHallManualParameters class
+        """The constructor for FastHallManualParameters class.
 
             Args:
                 excitation_type (str):
-                    * The excitation type used for the measurement. Options are:
-                    * "CURRENT"
-                    * "VOLTAGE"
-
+                    The excitation type used for the measurement. Options are: "CURRENT" or "VOLTAGE".
                 excitation_value(float):
-                    For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A
-
+                    For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A.
                 excitation_range (float or str):
-                    * Excitation range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V for voltage excitation,
-                        - amps in the range of -100e-3 to 100e-3 A for current excitation
-
+                    Excitation range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 excitation_measurement_range (float or str):
-                    * Excitation measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V: voltage excitation
-                        - amps in the range of -100e-3 to 100e-3 A: current excitation
-
+                    Excitation measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 measurement_range (float or str):
-                    * Measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - amps in the range of 0 to 100e-3A: voltage excitation
-                        - volts in the range of 0 to 10.0V: current excitation
-
+                    Measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either amps in the range of 0 to 100e-3A for voltage excitation, or
+                    volts in the range of 0 to 10.0V for current excitation.
                 compliance_limit (float):
-                    For voltage excitation, specify the current limit 100e-9 to 100e-3 A For current excitation,
-                    specify the voltage compliance 1.00 to 10.0 V
-
+                    For voltage excitation, specify the current limit 100e-9 to 100e-3. A For current excitation,
+                    specify the voltage compliance 1.00 to 10.0 V.
                 user_defined_field (float):
                     The field, in units of Tesla, the sample is being subjected to. Used for calculations.
-
                 max_samples(int):
                     When minimumSnr is omitted or Infinity ('INF'), the total number of samples to average 1 - 1000 When
-                    minimumSnr is specified, the maximum number of samples to average 10 - 1000. Default is 100
-
+                    minimumSnr is specified, the maximum number of samples to average 10 - 1000. Default is 100.
                 resistivity (float):
                     The resistivity of the sample in units of Ohm*Meters (bulk) of Ohms Per Square (sheet). Used for
                     calculations. Measure this value using the RESistivity SCPI subsystem. Defaults to 'Nan' (not a
-                    number) which will propagate through calculated values
-
-
+                    number) which will propagate through calculated values.
                 blanking_time (float or str):
-                    * The time in seconds to wait for hardware to settle before gathering readings. Range of time is
-                      0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
-                    * "DEF" (Default) = 2 ms
-                    * "MIN" = 0.5 ms
-                    * "MAX" = 300 s
-                    * floating point number in seconds
-
+                    The time in seconds to wait for hardware to settle before gathering readings. Range of time is
+                    0.5 ms - 300 s with a resolution of 0.1 ms. Options are: "DEF" (Default) = 2 ms,
+                    "MIN" = 0.5 ms,
+                    "MAX" = 300 s, or
+                    a floating point number in seconds.
                 averaging_samples (int):
                     The number of voltage compensation samples to average. Only applied for excitation type voltage.
                     1 - 120. Default is 60.
-
                 sample_thickness (float):
-                    Thickness of the sample in meters. 0 to 10E-3 m Default is 0 m
-
+                    Thickness of the sample in meters. 0 to 10E-3 m Default is 0 m.
                 min_hall_voltage_snr (float or str):
-                    * The desired signal to noise ratio of the measurement calculated using average hall voltage / error
-                      of mean 1 - 1000. Options are:
-                    * "INF" (Infinity)
-                    * "DEF" (Default) = 30
-                    * floating point number to represent the ratio
+                    The desired signal-to-noise ratio of the measurement calculated using average hall voltage / error
+                    of mean 1 - 1000. Options are:
+                    "INF" (Infinity),
+                    "DEF" (Default) = 30, or
+                    a floating point number to represent the ratio.
         """
         self.excitation_type = excitation_type
         self.excitation_value = excitation_value
         self.excitation_range = excitation_range
         self.excitation_measurement_range = excitation_measurement_range
         self.measurement_range = measurement_range
         self.compliance_limit = compliance_limit
@@ -286,61 +252,54 @@
         self.blanking_time = blanking_time
         self.averaging_samples = averaging_samples
         self.sample_thickness = sample_thickness
         self.min_hall_voltage_snr = min_hall_voltage_snr
 
 
 class FastHallLinkParameters:
-    """Class object representing parameters used for running FastHall Link measurements"""
+    """Class object representing parameters used for running FastHall Link measurements."""
     def __init__(self,
                  user_defined_field,
                  measurement_range='AUTO',
                  max_samples=100,
                  min_hall_voltage_snr=30,
                  averaging_samples=60,
                  sample_thickness='DEF'):
-        """The constructor for FastHallLinkParameters class
+        """The constructor for FastHallLinkParameters class.
 
             Args:
                 user_defined_field (float):
                     The field, in units of Tesla, the sample is being subjected to. Used for calculations.
-
                 measurement_range (float or str):
                     For voltage excitation, specify the current measurement range 0 to 100e-3 A For current
-                    excitation, specify the voltage measurement range 0 to 10.0 V. Defaults to 'AUTO'
-
+                    excitation, specify the voltage measurement range 0 to 10.0 V. Defaults to 'AUTO'.
                 max_samples(int):
-                    When minimumSnr is omitted or Infinity ('INF'), the total number of samples to average 1 - 1000
-                    When minimumSnr is specified, the maximum number of samples to average 10 - 1000 Defaults to 100
-
+                    When minimumSnr is omitted or Infinity ('INF'), the total number of samples to average 1 - 1000.
+                    When minimumSnr is specified, the maximum number of samples to average 10 - 1000 Defaults to 100.
                 min_hall_voltage_snr (float or str):
-                    * The desired signal to noise ratio of the measurement calculated using average hall voltage / error
-                      of mean 1 - 1000. Options are:
-                    * "INF" (Infinity)
-                    * "DEF" (Default) = 30
-                    * floating point number to represent the ratio
-
+                    The desired signal-to-noise ratio of the measurement calculated using average hall voltage / error
+                    of mean 1 - 1000. Options are: "INF" (Infinity), "DEF" (Default) = 30, or a floating point number
+                    to represent the ratio.
                 averaging_samples (int):
                     The number of voltage compensation samples to average. Only applied for excitation type voltage.
-                    1 - 120. Defaults to 60
-
+                    1 - 120. Defaults to 60.
                 sample_thickness (float):
                     Thickness of the sample in meters. 0 to 10E-3 m Default is the last run resistivity measurement's
                     sample thickness.
         """
         self.user_defined_field = user_defined_field
         self.measurement_range = measurement_range
         self.max_samples = max_samples
         self.min_hall_voltage_snr = min_hall_voltage_snr
         self.averaging_samples = averaging_samples
         self.sample_thickness = sample_thickness
 
 
 class FourWireParameters:
-    """Class object representing parameters used for running Four Wire measurements"""
+    """Class object representing parameters used for running Four Wire measurements."""
     def __init__(self,
                  contact_point1,
                  contact_point2,
                  contact_point3,
                  contact_point4,
                  excitation_type,
                  excitation_value,
@@ -353,80 +312,62 @@
                  min_snr=30,
                  excitation_reversal=True):
         """The constructor for FourWireParameter class.
 
             Args:
                 contact_point1 (int):
                     Excitation +. Valid contact points are: 1, 2, 3, 4, 5, or 6. Cannot be the same as Contact Point 2.
-
                 contact_point2 (int):
                     Excitation - Valid contact points are: 1, 2, 3, 4, 5, or 6. Cannot be the same as Contact Point 1.
-
                 contact_point3 (int):
                     Voltage Measure/Sense +. Valid contact points are: 1, 2, 3, 4, 5, or 6. Cannot be the same as
                     Contact Point 4.
-
                 contact_point4 (int):
                     Voltage Measure/Sense -. Valid contact points are: 1, 2, 3, 4, 5, or 6. Cannot be the same as
                     Contact Point 3.
-
                 excitation_type (str):
-                    * The excitation type used for the measurement. Options are:
-                    * "CURRENT"
-                    * "VOLTAGE"
-
+                    The excitation type used for the measurement. Options: "CURRENT" or "VOLTAGE".
                 excitation_value(float):
-                    For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A
-
+                    For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A.
                 excitation_range (float or str):
-                    * Excitation range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V for voltage excitation,
-                        - amps in the range of -100e-3 to 100e-3 A for current excitation
-
+                    Excitation range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 measurement_range (float or str):
-                    * Measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - amps in the range of 0 to 100e-3A: voltage excitation
-                        - volts in the range of 0 to 10.0V: current excitation
-
+                    Measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either amps in the range of 0 to 100e-3A for voltage excitation, or
+                    volts in the range of 0 to 10.0V for current excitation.
                 excitation_measurement_range (float or str):
-                    * Excitation measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V: voltage excitation
-                        - amps in the range of -100e-3 to 100e-3 A: current excitation
-
+                    Excitation measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 compliance_limit (float):
                     For voltage excitation, specify the current limit 100e-9 to 100e-3 A For current excitation,
-                    specify the voltage compliance 1.00 to 10.0 V
-
+                    specify the voltage compliance 1.00 to 10.0 V.
                 blanking_time (float or str):
-                    * The time in seconds to wait for hardware to settle before gathering readings. Range of time is
-                      0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
-                    * "DEF" (Default)= 2 ms
-                    * "MIN" = 0.5 ms
-                    * "MAX" = 300 s
-                    * floating point number in seconds
-
+                    The time in seconds to wait for hardware to settle before gathering readings. Range of time is
+                    0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
+                    "DEF" (Default)= 2 ms,
+                    "MIN" = 0.5 ms.
+                    "MAX" = 300 s, or
+                    a floating point number in seconds.
                 max_samples(int):
                     When minimumSnr is omitted or Infinity, the total number of samples to average 1 - 1000 When
-                    minimumSnr is specified, the maximum number of samples to average 10 - 1000. Default is 100
-
+                    minimumSnr is specified, the maximum number of samples to average 10 - 1000. Default is 100.
                 min_snr (float or str):
-                    * The desired signal to noise ratio of the measurement resistance, calculated using measurement
-                      average / error of mean 1 - 1000. Options are:
-                    * "INF" (Infinity)
-                    * "DEF" (Default)= 30
-                    * floating point number to represent the ratio
-
+                    The desired signal-to-noise ratio of the measurement resistance, calculated using measurement
+                    average / error of mean 1 - 1000. Options are:
+                    "INF" (Infinity),
+                    "DEF" (Default)= 30, or
+                    a floating point number to represent the ratio.
                 excitation_reversal (bool):
-                    True = Reverse the excitation to generate the resistance. False = no excitation reversal
+                    True = Reverse the excitation to generate the resistance. False = no excitation reversal.
         """
         self.contact_point1 = contact_point1
         self.contact_point2 = contact_point2
         self.contact_point3 = contact_point3
         self.contact_point4 = contact_point4
         self.excitation_type = excitation_type
         self.excitation_value = excitation_value
@@ -437,15 +378,15 @@
         self.blanking_time = blanking_time
         self.max_samples = max_samples
         self.min_snr = min_snr
         self.excitation_reversal = str(int(excitation_reversal))
 
 
 class DCHallParameters:
-    """Class object representing parameters used for running DC Hall measurements"""
+    """Class object representing parameters used for running DC Hall measurements."""
     def __init__(self,
                  excitation_type,
                  excitation_value,
                  compliance_limit,
                  averaging_samples,
                  user_defined_field,
                  excitation_range='AUTO',
@@ -455,70 +396,54 @@
                  resistivity='"NaN"',
                  blanking_time=2e-3,
                  sample_thickness=0):
         """The constructor for DCHallParameters.
 
             Args:
                 excitation_type (str):
-                    * The excitation type used for the measurement. Options are:
-                    * "CURRENT"
-                    * "VOLTAGE"
-
+                    The excitation type used for the measurement. Options: "CURRENT", or "VOLTAGE".
                 excitation_value(float):
-                    For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A
-
+                    For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A.
                 excitation_range (float or str):
-                    * Excitation range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V for voltage excitation,
-                        - amps in the range of -100e-3 to 100e-3 A for current excitation
-
+                    Excitation range based on the excitation type. Options are:
+                    "AUTO" for sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 excitation_measurement_range (float or str):
-                    * Excitation measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V: voltage excitation
-                        - amps in the range of -100e-3 to 100e-3 A: current excitation
-
+                    Excitation measurement range based on the excitation type. Options are:
+                    "AUTO" for sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 measurement_range (float or str):
-                    * Measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - amps in the range of 0 to 100e-3A: voltage excitation
-                        - volts in the range of 0 to 10.0V: current excitation
-
+                    Measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either amps in the range of 0 to 100e-3A for voltage excitation, or
+                    volts in the range of 0 to 10.0V for current excitation.
                 compliance_limit (float):
                     For voltage excitation, specify the current limit 100e-9 to 100e-3 A For current excitation,
-                    specify the voltage compliance 1.00 to 10.0 V
-
+                    specify the voltage compliance 1.00 to 10.0 V.
                 averaging_samples(int):
-                    The number of samples to average 1-1000
-
+                    The number of samples to average 1-1000.
                 user_defined_field(float):
                     The field, in units of Tesla, the sample is being subjected to. Used for calculations.
-
                 with_field_reversal (bool):
-                    Specifies whether or not to apply reversal field. Default is true
-
+                    Specifies whether to apply reversal field. Default is true
                 resistivity(float):
                     The resistivity of the sample in units of Ohm*Meters (bulk) of Ohms Per Square (sheet). Used for
                     calculations. Measure this value using the RESistivity SCPI subsystem. Defaults to 'NaN' (not a
                     number) which will propagate through calculated values.
-
                 blanking_time (float or str):
-                    * The time in seconds to wait for hardware to settle before gathering readings. Range of time is
-                      0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
-                    * "DEF" (Default) = 2 ms
-                    * "MIN" = 0.5 ms
-                    * "MAX" = 300 s
-                    * floating point number in seconds
-
+                    The time in seconds to wait for hardware to settle before gathering readings. Range of time is
+                    0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
+                    "DEF" (Default) = 2 ms,
+                    "MIN" = 0.5 ms,
+                    "MAX" = 300 s, or
+                    floating point number in seconds.
                 sample_thickness (float):
-                    Thickness of the sample in meters. 0 to 10e-3 m. Default is 0m
+                    Thickness of the sample in meters. 0 to 10e-3 m. Default is 0m.
             """
 
         self.excitation_type = excitation_type
         self.excitation_value = excitation_value
         self.excitation_range = excitation_range
         self.excitation_measurement_range = excitation_measurement_range
         self.measurement_range = measurement_range
@@ -528,15 +453,15 @@
         self.with_field_reversal = str(int(with_field_reversal))
         self.resistivity = resistivity
         self.blanking_time = blanking_time
         self.sample_thickness = sample_thickness
 
 
 class ResistivityManualParameters:
-    """Class object representing parameters used for running manual Resistivity measurements"""
+    """Class object representing parameters used for running manual Resistivity measurements."""
     def __init__(self,
                  excitation_type,
                  excitation_value,
                  compliance_limit,
                  excitation_range='AUTO',
                  excitation_measurement_range='AUTO',
                  measurement_range='AUTO',
@@ -545,78 +470,61 @@
                  sample_thickness=0,
                  min_snr=30,
                  **kwargs):
         """The constructor for ResistivityManualParameters class.
 
             Args:
                 excitation_type (str):
-                    * The excitation type used for the measurement. Options are:
-                    * "CURRENT"
-                    * "VOLTAGE"
-
+                    The excitation type used for the measurement. Options are: "CURRENT" or "VOLTAGE".
                 excitation_value(float):
-                    For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A
-
+                    For voltage -10.0 to 10.0 V For current -100e-3 to 100e-3 A.
                 excitation_range (float or str):
-                    * Excitation range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V for voltage excitation,
-                        - amps in the range of -100e-3 to 100e-3 A for current excitation
-
+                    Excitation range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 excitation_measurement_range (float or str):
-                    * Excitation measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - volts in the range of 0 to 10.0V: voltage excitation
-                        - amps in the range of -100e-3 to 100e-3 A: current excitation
-
+                    Excitation measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    floating point number of either volts in the range of 0 to 10.0V for voltage excitation, or
+                    amps in the range of -100e-3 to 100e-3 A for current excitation.
                 measurement_range (float or str):
-                    * Measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - amps in the range of 0 to 100e-3A: voltage excitation
-                        - volts in the range of 0 to 10.0V: current excitation
-
+                    Measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either amps in the range of 0 to 100e-3A for voltage excitation, or
+                    volts in the range of 0 to 10.0V for current excitation.
                 compliance_limit (float):
                     For voltage excitation, specify the current limit 100e-9 to 100e-3 A For current excitation,
-                    specify the voltage compliance 1.00 to 10.0 V
-
+                    specify the voltage compliance 1.00 to 10.0 V.
                 max_samples(int):
                     When minimumSnr is omitted or Infinity ('INF'), the total number of samples to average 1 - 1000 When
-                    minimumSnr is specified, the maximum number of samples to average 10 - 1000. Default is 100
-
+                    minimumSnr is specified, the maximum number of samples to average 10 - 1000. Default is 100.
                 blanking_time (float or str):
-                    * The time in seconds to wait for hardware to settle before gathering readings. Range of time is
-                      0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
-                    * "DEF" (Default) = 2 ms
-                    * "MIN" = 0.5 ms
-                    * "MAX" = 300 s
-                    * floating point number in seconds
-
+                    The time in seconds to wait for hardware to settle before gathering readings. Range of time is
+                    0.5 ms - 300 s with a resolution of 0.1 ms. Options are:
+                    "DEF" (Default) = 2 ms,
+                    "MIN" = 0.5 ms,
+                    "MAX" = 300 s, or
+                    a floating point number in seconds.
                 averaging_samples (int):
                     The number of voltage compensation samples to average. Only applied for excitation type voltage.
-                    1 - 120. Default is 60
-
+                    1 - 120. Default is 60.
                 sample_thickness (float):
-                    Thickness of the sample in meters. 0 to 10E-3 m. Default is 0 m
-
+                    Thickness of the sample in meters. 0 to 10E-3 m. Default is 0 m.
                 min_snr (float or str):
-                    * The desired signal to noise ratio of the measurement calculated using average resistivity / error
-                      of mean 1 - 1000. Options are:
-                    * "INF" (Infinity)
-                    * "DEF" (Default) = 30
-                    * floating point number to represent the ratio
-
+                    The desired signal-to-noise ratio of the measurement calculated using average resistivity / error
+                    of mean 1 - 1000. Options are:
+                    "INF" (Infinity),
+                    "DEF" (Default) = 30, or
+                    a floating point number to represent the ratio.
             Kwargs:
                 width(float):
-                    The width of the sample in meters. Greater than 0
-
+                    The width of the sample in meters. Greater than 0.
                 separation(float):
-                    The distance between the sample's arms in meters. Greater than 0
+                    The distance between the sample's arms in meters. Greater than 0.
             """
 
         self.excitation_type = excitation_type
         self.excitation_value = excitation_value
         self.excitation_range = excitation_range
         self.excitation_measurement_range = excitation_measurement_range
         self.measurement_range = measurement_range
@@ -626,53 +534,49 @@
         self.max_samples = max_samples
         self.blanking_time = blanking_time
         self.sample_thickness = sample_thickness
         self.min_snr = min_snr
 
 
 class ResistivityLinkParameters:
-    """Class object representing parameters used for running manual Resistivity measurements"""
+    """Class object representing parameters used for running manual Resistivity measurements."""
     def __init__(self,
                  measurement_range='AUTO',
                  sample_thickness=0,
                  min_snr=30,
                  max_samples=100):
         """The constructor for ResistivityLinkParameters class.
 
             Args:
                 measurement_range (float or str):
-                    * Measurement range based on the excitation type. Options are:
-                    * "AUTO": sets the range to the best fit range for a given excitation value
-                    * floating point number of
-                        - amps in the range of 0 to 100e-3A: voltage excitation
-                        - volts in the range of 0 to 10.0V: current excitation
-
+                    Measurement range based on the excitation type. Options are:
+                    "AUTO" which sets the range to the best fit range for a given excitation value, or
+                    a floating point number of either amps in the range of 0 to 100e-3 A for voltage excitation, or
+                    volts in the range of 0 to 10.0V for current excitation.
                 sample_thickness (float):
-                    Thickness of the sample in meters. 0 to 10E-3 m. Default is 0 m
-
+                    Thickness of the sample in meters. 0 to 10E-3 m. Default is 0 m.
                 min_snr (float or str):
-                    * The desired signal to noise ratio of the measurement calculated using average resistivity / error
-                      of mean 1 - 1000. Options are:
-                    * "INF" (Infinity)
-                    * "DEF" (Default)= 30
-                    * floating point number to represent the ratio
-
+                    The desired signal-to-noise ratio of the measurement calculated using average resistivity / error
+                    of mean 1 - 1000. Options are:
+                    "INF" (Infinity),
+                    "DEF" (Default)= 30, or
+                    a floating point number to represent the ratio.
                 max_samples(int):
                     When minimumSnr is omitted or Infinity ('INF'), the total number of samples to average 1 - 1000 When
-                    minimumSnr is specified, the maximum number of samples to average 10 - 1000 Default is 100
+                    minimumSnr is specified, the maximum number of samples to average 10 - 1000 Default is 100.
         """
 
         self.measurement_range = measurement_range
         self.sample_thickness = sample_thickness
         self.min_snr = min_snr
         self.max_samples = max_samples
 
 
 class FastHall(XIPInstrument):
-    """A class object representing a Lake Shore M91 Fast Hall controller"""
+    """A class object representing a Lake Shore M91 Fast Hall controller."""
 
     vid_pid = [(0x1FB9, 0x0705)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=921600,
@@ -692,35 +596,35 @@
 
     # Status Methods
     def get_contact_check_running_status(self):
         """Indicates if the contact check measurement is running."""
         return bool(int(self.query("CCHECK:RUNNING?")))
 
     def get_fasthall_running_status(self):
-        """Indicates if the FastHall measurement is running"""
+        """Indicates if the FastHall measurement is running."""
         return bool(int(self.query("FASTHALL:RUNNING?")))
 
     def get_four_wire_running_status(self):
-        """Indicates if the four wire measurement is running"""
+        """Indicates if the four wire measurement is running."""
         return bool(int(self.query("FWIRE:RUNNING?")))
 
     def get_resistivity_running_status(self):
-        """Indicates if the resistivity measurement is running"""
+        """Indicates if the resistivity measurement is running."""
         return bool(int(self.query("RESISTIVITY:RUNNING?")))
 
     def get_dc_hall_running_status(self):
-        """Indicates if the DC Hall measurement is running"""
+        """Indicates if the DC Hall measurement is running."""
         return bool(int(self.query("HALL:DC:RUNNING?")))
 
     def get_dc_hall_waiting_status(self):
         """Indicates if the DC hall measurement is running."""
         return bool(int(self.query("HALL:DC:WAITING?")))
 
     def continue_dc_hall(self):
-        """Continues the DC hall measurement if it's in a waiting state """
+        """Continues the DC hall measurement if it's in a waiting state."""
         self.command("HALL:DC:CONTINUE")
 
     def start_contact_check_vdp_optimized(self, settings):
         """Automatically determines excitation value and ranges. Then runs contact check on all 4 pairs.
 
             Args:
                 settings(ContactCheckOptimizedParameters):
@@ -787,36 +691,41 @@
                          f"{str(settings.blanking_time)}," +
                          f"{str(settings.averaging_samples)}," +
                          f"{str(settings.sample_thickness)}," +
                          f"{str(settings.min_hall_voltage_snr)}")
         self.command(command_string)
 
     def start_fasthall_link_vdp(self, settings):
-        """Performs a FastHall (measurement that uses the last run contact check measurement's excitation type,
-        compliance limit, blanking time, excitation range, and the largest absolute value of the start and end
-        excitation values along with the last run resistivity measurement's resistivity average and sample thickness.
+        """Starts a FastHall measurement with provided link parameters.
+
+            Performs a FastHall measurement that uses the last run contact check measurement's excitation type,
+            compliance limit, blanking time, excitation range, and the largest absolute value of the start and end
+            excitation values along with the last run resistivity measurement's resistivity average and sample
+            thickness.
 
             Args:
-                settings (FastHallLinkParameters)
+                settings (FastHallLinkParameters):
         """
         command_string = ("FASTHALL:START:LINK " +
                          f"{str(settings.user_defined_field)}," +
                          f"{str(settings.measurement_range)}," +
                          f"{str(settings.max_samples)}," +
                          f"{str(settings.min_hall_voltage_snr)}," +
                          f"{str(settings.averaging_samples)}," +
                          f"{str(settings.sample_thickness)}")
         self.command(command_string)
 
     def start_four_wire(self, settings):
-        """Performs a Four wire measurement. Excitation is sourced from Contact Point 1 to Contact Point 2. Voltage is
-        measured/sensed between contact point 3 and contact point 4.
+        """Performs a Four wire measurement.
+
+            Excitation is sourced from Contact Point 1 to Contact Point 2. Voltage is measured/sensed between contact
+            point 3 and contact point 4.
 
             Args:
-                settings(FourWireParameters)
+                settings(FourWireParameters):
         """
         command_string = ("FWIRE:START " +
                          f"{str(settings.contact_point1)}," +
                          f"{str(settings.contact_point2)}," +
                          f"{str(settings.contact_point3)}," +
                          f"{str(settings.contact_point4)}," +
                          f"{str(settings.excitation_type)}," +
@@ -832,15 +741,15 @@
         self.command(command_string)
 
     def start_dc_hall_vdp(self, settings):
 
         """Performs a DC hall measurement for a Hall Bar sample.
 
             Args:
-                settings(DCHallParameters)
+                settings(DCHallParameters):
 
         """
         command_string = ("HALL:DC:START " +
                          f"{str(settings.excitation_type)}," +
                          f"{str(settings.excitation_value)}," +
                          f"{str(settings.excitation_range)}," +
                          f"{str(settings.excitation_measurement_range)}," +
@@ -854,15 +763,15 @@
                          f"{str(settings.sample_thickness)}")
         self.command(command_string)
 
     def start_dc_hall_hbar(self, settings):
         """Performs a DC hall measurement for a Hall Bar sample.
 
             Args:
-                settings(DCHallParameters)
+                settings(DCHallParameters):
         """
         command_string = ("HALL:HBAR:DC:START " +
                          f"{str(settings.excitation_type)}," +
                          f"{str(settings.excitation_value)}," +
                          f"{str(settings.excitation_range)}," +
                          f"{str(settings.excitation_measurement_range)}," +
                          f"{str(settings.measurement_range)}," +
@@ -875,15 +784,15 @@
                          f"{str(settings.sample_thickness)}")
         self.command(command_string)
 
     def start_resistivity_vdp(self, settings):
         """Performs a resistivity measurement on a Van der Pauw sample.
 
             Args:
-                settings(ResistivityManualParameters)
+                settings(ResistivityManualParameters):
         """
         command_string = ("RESISTIVITY:START " +
                          f"{str(settings.excitation_type)}," +
                          f"{str(settings.excitation_value)}," +
                          f"{str(settings.excitation_range)}," +
                          f"{str(settings.excitation_measurement_range)}," +
                          f"{str(settings.measurement_range)}," +
@@ -891,33 +800,35 @@
                          f"{str(settings.max_samples)}," +
                          f"{str(settings.blanking_time)}," +
                          f"{str(settings.sample_thickness)}," +
                          f"{str(settings.min_snr)}")
         self.command(command_string)
 
     def start_resistivity_link_vdp(self, settings):
-        """Performs a resistivity measurement that uses the last run contact check measurement's excitation type,
-        compliance limit, blanking time, excitation range, and the largest absolute value of the start and end
-        excitation values.
+        """Performs a resistivity measurement with provided link settings.
+
+            Performs a resistivity measurement that uses the last run contact check measurement's excitation type,
+            compliance limit, blanking time, excitation range, and the largest absolute value of the start and end
+            excitation values.
 
             Args:
-                settings(ResistivityLinkParameters)
+                settings(ResistivityLinkParameters):
         """
         command_string = ("RESISTIVITY:START:LINK " +
                          f"{str(settings.measurement_range)}," +
                          f"{str(settings.sample_thickness)}," +
                          f"{str(settings.min_snr)}," +
                          f"{str(settings.max_samples)}")
         self.command(command_string)
 
     def start_resistivity_hbar(self, settings):
         """Performs a resistivity measurement on a hall bar sample.
 
             Args:
-                settings(ResistivityManualParameters)
+                settings(ResistivityManualParameters):
 
         """
         command_string = ("RESISTIVITY:HBAR:START " +
                          f"{str(settings.excitation_type)}," +
                          f"{str(settings.excitation_value)}," +
                          f"{str(settings.excitation_range)}," +
                          f"{str(settings.excitation_measurement_range)}," +
@@ -928,15 +839,15 @@
                          f"{str(settings.max_samples)}," +
                          f"{str(settings.blanking_time)}," +
                          f"{str(settings.sample_thickness)}," +
                          f"{str(settings.min_snr)}")
         self.command(command_string)
 
     def get_contact_check_setup_results(self):
-        """Returns an object representing the setup results of the last run Contact Check measurement"""
+        """Returns an object representing the setup results of the last run Contact Check measurement."""
 
         # Parse the JSON query string into a dictionary with only the setup results
         json_results = self.query('CCHECK:RESULT:JSON? 0')
         setup_results = json.loads(json_results).get('Setup')
 
         # Generate a  Contact Check settings object using the setup result values as the initialization parameters
         settings = ContactCheckManualParameters(excitation_type=setup_results.get('ExcitationType'),
@@ -947,29 +858,29 @@
                                                 compliance_limit=setup_results.get('ComplianceLimit'),
                                                 number_of_points=setup_results.get('NumberOfPoints'),
                                                 min_r_squared=setup_results.get('MinimumRSquared'),
                                                 blanking_time=setup_results.get('BlankingTimeInSeconds'))
         return settings
 
     def get_contact_check_measurement_results(self):
-        """Returns a dictionary representing the results of the last run Contact Check measurement"""
+        """Returns a dictionary representing the results of the last run Contact Check measurement."""
 
         # Parse the JSON query string into a dictionary
         json_results = self.query('CCHECK:RESULT:JSON? 0')
         measurement_results = json.loads(json_results)
 
         # Remove the setup data from the results dictionary
         measurement_results.pop('Setup')
         measurement_results.pop('OptimizationSetup')
         measurement_results.pop('OptimizationDiagnostics')
 
         return measurement_results
 
     def get_fasthall_setup_results(self):
-        """Returns an object representing the setup results of the last run FastHall measurement"""
+        """Returns an object representing the setup results of the last run FastHall measurement."""
 
         # Parse the JSON query string into a dictionary with only the setup results
         json_results = self.query('FASTHALL:RESULT:JSON? 0')
         setup_results = json.loads(json_results).get('Setup')
 
         # Generate a FastHall settings object using the setup result values as the initialization parameters
         settings = FastHallManualParameters(excitation_type=setup_results.get('ExcitationType'),
@@ -986,27 +897,27 @@
                                             averaging_samples=setup_results.get('NumberOfVoltageCompensationSamplesTo\
                                             Average'),
                                             sample_thickness=setup_results.get('SampleThicknessInMeters'),
                                             min_hall_voltage_snr=setup_results.get('HallVoltageSnr'))
         return settings
 
     def get_fasthall_measurement_results(self):
-        """Returns a dictionary representing the results of the last run FastHall measurement"""
+        """Returns a dictionary representing the results of the last run FastHall measurement."""
 
         # Parse the JSON query string into a dictionary
         json_results = self.query('FASTHALL:RESULT:JSON? 0')
         measurement_results = json.loads(json_results)
 
         # Remove the setup data from the results dictionary
         measurement_results.pop('Setup')
 
         return measurement_results
 
     def get_four_wire_setup_results(self):
-        """Returns an object representing the setup results of the last run Four Wire measurement"""
+        """Returns an object representing the setup results of the last run Four Wire measurement."""
 
         # Parse the JSON query string into a dictionary with only the setup results
         json_results = self.query('FWIRE:RESULT:JSON? 0')
         setup_results = json.loads(json_results).get('Setup')
 
         # Generate a Four Wire settings object using the setup result values as the initialization parameters
         settings = FourWireParameters(contact_point1=setup_results.get('ContactPairExcitation').get('Point1'),
@@ -1022,27 +933,27 @@
                                       blanking_time=setup_results.get('BlankingTimeInSeconds'),
                                       max_samples=setup_results.get('MaximumNumberOfSamples'),
                                       min_snr=setup_results.get('MinimumResistanceSnr'),
                                       excitation_reversal=setup_results.get('UseExcitationReversal'))
         return settings
 
     def get_four_wire_measurement_results(self):
-        """Returns a dictionary representing the results of the last run Four Wire measurement"""
+        """Returns a dictionary representing the results of the last run Four Wire measurement."""
 
         # Parse the JSON query string into a dictionary
         json_results = self.query('FWIRE:RESULT:JSON? 0')
         measurement_results = json.loads(json_results)
 
         # Remove the setup data from the results dictionary
         measurement_results.pop('Setup')
 
         return measurement_results
 
     def get_dc_hall_setup_results(self):
-        """Returns a dictionary representing the setup results of the last run Hall measurement"""
+        """Returns a dictionary representing the setup results of the last run Hall measurement."""
 
         # Parse the JSON query string into a dictionary with only the setup results
         json_results = self.query('HALL:DC:RESULT:JSON? 0')
         setup_results = json.loads(json_results).get('Setup')
 
         # Generate a DC Hall settings object using the setup result values as the initialization parameters
         settings = DCHallParameters(excitation_type=setup_results.get('ExcitationType'),
@@ -1056,27 +967,27 @@
                                     with_field_reversal=setup_results.get('WithFieldReversal'),
                                     resistivity=setup_results.get('Resistivity'),
                                     blanking_time=setup_results.get('BlankingTimeInSeconds'),
                                     sample_thickness=setup_results.get('SampleThicknessInMeters'))
         return settings
 
     def get_dc_hall_measurement_results(self):
-        """Returns a dictionary representing the results of the last run Hall measurement"""
+        """Returns a dictionary representing the results of the last run Hall measurement."""
 
         # Parse the JSON query string into a dictionary
         json_results = self.query('HALL:DC:RESULT:JSON? 0')
         measurement_results = json.loads(json_results)
 
         # Remove the setup data from the results dictionary
         measurement_results.pop('Setup')
 
         return measurement_results
 
     def get_resistivity_setup_results(self):
-        """Returns an object representing the setup results of the last run Resistivity measurement"""
+        """Returns an object representing the setup results of the last run Resistivity measurement."""
 
         # Parse the JSON query string into a dictionary with only the setup results
         json_results = self.query('RESISTIVITY:RESULT:JSON? 0')
         setup_results = json.loads(json_results).get('Setup')
 
         # Generate a Resistivity settings object using the setup result values as the initialization parameters
         settings = ResistivityManualParameters(setup_results.get('ExcitationType'),
@@ -1091,30 +1002,30 @@
                                                max_samples=setup_results.get('MaxNumberOfSamples'),
                                                blanking_time=setup_results.get('BlankingTimeInSeconds'),
                                                sample_thickness=setup_results.get('SampleThicknessInMeters'),
                                                min_snr=setup_results.get('MinimumSnr'))
         return settings
 
     def get_resistivity_measurement_results(self):
-        """Returns a dictionary representing the results of the last run Resistivity measurement"""
+        """Returns a dictionary representing the results of the last run Resistivity measurement."""
 
         # Parse the JSON query string into a dictionary
         json_results = self.query('RESISTIVITY:RESULT:JSON? 0')
         measurement_results = json.loads(json_results)
 
         # Remove the setup data from the results dictionary
         measurement_results.pop('Setup')
 
         return measurement_results
 
     def run_complete_contact_check_optimized(self, settings):
         """Performs a contact check measurement and then returns the corresponding measurement results.
 
             Args:
-                settings(ContactCheckOptimizedParameters)
+                settings(ContactCheckOptimizedParameters):
 
             Returns:
                 The measurement results as a dictionary.
         """
 
         # Run an optimized contact check
         self.start_contact_check_vdp_optimized(settings)
@@ -1127,23 +1038,22 @@
         results = self.get_contact_check_measurement_results()
         return results
 
     def run_complete_contact_check_manual(self, settings, sample_type):
         """Performs a manual contact check measurement and then returns the corresponding measurement results.
 
             Args:
-                settings(ContactCheckManualParameters)
-
-                sample_type(str):
-                    * Indicates sample type. Options are:
-                    * "VDP" (Van der Pauw sample)
-                    * "HBAR" (Hall Bar sample)
+                settings (ContactCheckManualParameters):
+                    Object with settings for FastHall link setup.
+                sample_type (str):
+                    Indicates sample type. Options: "VDP" (Van der Pauw sample), or "HBAR" (Hall Bar sample).
 
             Returns:
                 The measurement results as a dictionary.
+
         """
 
         # Run specific measurement based on sample type
         if sample_type == "VDP":
             self.start_contact_check_vdp(settings)
         elif sample_type == "HBAR":
             self.start_contact_check_hbar(settings)
@@ -1156,15 +1066,16 @@
         results = self.get_contact_check_measurement_results()
         return results
 
     def run_complete_fasthall_link(self, settings):
         """Performs a FastHall Link measurement and then returns the corresponding measurement results.
 
             Args:
-                settings(FastHallLinkParameters)
+                settings(FastHallLinkParameters):
+                    Object with settings for FastHall link setup.
 
             Returns:
                 The measurement results as a dictionary.
         """
 
         # Run FastHall Link measurement
         self.start_fasthall_link_vdp(settings)
@@ -1177,16 +1088,16 @@
         results = self.get_fasthall_measurement_results()
         return results
 
     def run_complete_fasthall_manual(self, settings):
         """Performs a manual FastHall measurement and then returns the corresponding measurement results.
 
             Args:
-                settings(FastHallManualParameters)
-
+                settings(FastHallManualParameters):
+                    Object with settings for FastHall link setup.
             Returns:
                 The measurement results as a dictionary.
         """
 
         # Run manual FastHall measurement
         self.start_fasthall_vdp(settings)
 
@@ -1198,15 +1109,15 @@
         results = self.get_fasthall_measurement_results()
         return results
 
     def run_complete_four_wire(self, settings):
         """Performs a Four Wire measurement and then returns the corresponding measurement results.
 
             Args:
-                settings(FourWireParameters)
+                settings(FourWireParameters):
 
             Returns:
                 The measurement results as a dictionary.
         """
 
         # Run Four Wire measurement
         self.start_four_wire(settings)
@@ -1219,20 +1130,18 @@
         results = self.get_four_wire_measurement_results()
         return results
 
     def run_complete_dc_hall(self, settings, sample_type):
         """Performs a DC Hall measurement and then returns the corresponding measurement results.
 
             Args:
-                settings(DCHallParameters)
-
+                settings(DCHallParameters):
+                    Object with settings for FastHall link setup.
                 sample_type(str):
-                    * Indicates sample type. Options are:
-                    * "VDP" (Van der Pauw sample)
-                    * "HBAR" (Hall Bar sample)
+                    Indicates sample type. Options: "VDP" (Van der Pauw sample), or"HBAR" (Hall Bar sample).
 
             Returns:
                 The measurement results as a dictionary.
         """
 
         # Run specific measurement based on sample type
         if sample_type == "VDP":
@@ -1249,15 +1158,15 @@
         results = self.get_dc_hall_measurement_results()
         return results
 
     def run_complete_resistivity_link(self, settings):
         """Performs a resistivity link measurement and then returns the corresponding measurement results.
 
             Args:
-                settings(ResistivityLinkParameters)
+                settings(ResistivityLinkParameters):
 
             Returns:
                 The measurement results as a dictionary.
         """
 
         # Run a resistivity link measurement
         self.start_resistivity_link_vdp(settings)
@@ -1270,20 +1179,18 @@
         results = self.get_resistivity_measurement_results()
         return results
 
     def run_complete_resistivity_manual(self, settings, sample_type):
         """Performs a manual resistivity measurement and then returns the corresponding measurement results.
 
             Args:
-                settings(ResistivityManualParameters)
-
+                settings(ResistivityManualParameters):
+                    Object with settings for manual resistivity setup.
                 sample_type(str):
-                    * Indicates sample type. Options are:
-                    * "VDP" (Van der Pauw sample)
-                    * "HBAR" (Hall Bar sample)
+                    Indicates sample type. Options are: "VDP" (Van der Pauw sample), or "HBAR" (Hall Bar sample).
 
             Returns:
                 The measurement results as a dictionary.
         """
 
         # Run specific measurement based on sample type
         if sample_type == "VDP":
@@ -1296,30 +1203,30 @@
             pass
 
         # Collect and return results
         results = self.get_resistivity_measurement_results()
         return results
 
     def reset_contact_check_measurement(self):
-        """Resets the measurement to a not run state, canceling any running measurement"""
+        """Resets the measurement to a not run state, canceling any running measurement."""
         self.command("CCHECK:RESET")
 
     def reset_fasthall_measurement(self):
-        """Resets the measurement to a not run state, canceling any running measurement"""
+        """Resets the measurement to a not run state, canceling any running measurement."""
         self.command("FASTHALL:RESET")
 
     def reset_four_wire_measurement(self):
 
-        """Resets the measurement to a not run state, canceling any running measurement"""
+        """Resets the measurement to a not run state, canceling any running measurement."""
         self.command("FWIRE:RESET")
 
     def reset_dc_hall_measurement(self):
-        """Resets the measurement to a not run state, canceling any running measurement"""
+        """Resets the measurement to a not run state, canceling any running measurement."""
         self.command("HALL:DC:RESET")
 
     def reset_resistivity_measurement(self):
-        """Resets the measurement to a not run state, canceling any running measurement"""
+        """Resets the measurement to a not run state, canceling any running measurement."""
         self.command("RESISTIVITY:RESET")
 
 
 # Create an alias using the product name
 M91 = FastHall
```

### Comparing `lakeshore-1.6.1/lakeshore/generic_instrument.py` & `lakeshore-1.7.0/lakeshore/generic_instrument.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""This module implements a parent class that contains basic functionality for communicating with Lake Shore instruments."""
+"""This module implements a parent class that contains basic functionality for communicating with
+Lake Shore instruments.
+"""
 import logging
 import select
 import socket
 from threading import Lock
 from time import sleep
 
 import serial
@@ -10,78 +12,100 @@
 
 
 class InstrumentException(Exception):
     """Names a new type of exception specific to general instrument connectivity."""
 
 
 class RegisterBase:
-    """Base class of the status register classes"""
+    """Base class of the status register classes."""
 
     bit_names = []
 
     def __str__(self):
         return str(vars(self))
 
     def to_integer(self):
-        """Translates the register object to an integer representation value"""
+        """Translates the register object to an integer representation value."""
 
         integer_representation = 0
 
         # Add up the boolean values of a list of named instrument states
         # while being careful to account for unnamed entries in the register bit names list
         for count, bit_name in enumerate(self.bit_names):
 
             if bit_name:
                 integer_representation += int(getattr(self, bit_name)) << count
 
         return integer_representation
 
     @classmethod
     def from_integer(cls, integer_representation):
-        """Creates the register object from an integer representation value"""
+        """Creates the register object from an integer representation value."""
 
         # Create a dictionary to temporarily store the bit states
         bit_states = {}
 
         # Assign the boolean value of each bit in the integer to the corresponding status register bit name
         for count, bit_name in enumerate(cls.bit_names):
             if bit_name:
                 mask = 0b1 << count
                 bit_states[bit_name] = bool(int(integer_representation) & mask)
 
         return cls(**bit_states)
 
 
+def _is_valid_user_connection(connection):
+    """Verifies connection can be used and has write and query methods."""
+    try:
+        return callable(connection.write) and callable(connection.query)
+    except AttributeError:
+        return 0
+
+
 class GenericInstrument:
-    """Parent class that implements functionality to connect to generic instruments"""
+    """Parent class that implements functionality to connect to generic instruments."""
 
     vid_pid = []
     logger = logging.getLogger(__name__)
 
     def __init__(self, serial_number, com_port, baud_rate, data_bits, stop_bits, parity, flow_control,
                  handshaking, timeout, ip_address, tcp_port, connection=None):
         # Initialize values common to all instruments
         self.device_serial = None
         self.device_tcp = None
         self.dut_lock = Lock()
         self.serial_number = None
         self.option_card_serial = None
+        self.user_connection = None
 
-        # Raise an error if serial and TCP parameters are passed. Otherwise connect to the instrument using one of them.
-        if ip_address is not None:
-            if com_port is not None:
-                raise ValueError("Two different connection methods provided.")
+        # Raise an error if multiple connection methods are passed. Otherwise, connect to instrument.
+        if ip_address and com_port:
+            raise ValueError("Too many connections. Cannot have IP and serial connection at the same time.")
+        if ip_address and connection:
+            raise ValueError("Too many connections. Cannot have IP and user connection at the same time.")
+        if com_port and connection:
+            raise ValueError("Too many connections. Cannot have serial and user connection at the same time.")
 
+        # TCP via IP
+        if ip_address:
             self.connect_tcp(ip_address, tcp_port, timeout)
-        else:
-            if connection is None:
-                self.connect_usb(serial_number, com_port, baud_rate, data_bits, stop_bits, parity,
-                                 timeout, handshaking, flow_control)
-            else:
+        # User provided connection
+        elif connection:
+            # Test connection
+            if hasattr(connection, "FAKE_CONNECTION"):
                 self.device_serial = connection
+            # Check validity of provided connection with duck-typing
+            elif _is_valid_user_connection(connection):
+                self.user_connection = connection
+            else:
+                raise ValueError("Invalid connection. Connection must have callable write and query methods.")
+        # USB connection (default)
+        else:
+            self.connect_usb(serial_number, com_port, baud_rate, data_bits, stop_bits, parity,
+                             timeout, handshaking, flow_control)
 
         # Query the instrument identification information and store it in variables
         try:
             idn_response = self._get_identity()
             self.firmware_version = idn_response[3]
             serial_string = idn_response[2].split("/")
             self.serial_number = serial_string[0]
@@ -106,62 +130,74 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.__del__()
 
+    def write(self, command_string):
+        """Alias of command. Send a command to the instrument.
+
+            Args:
+                command_string (str):
+                    A serial command.
+        """
+        self.command(command_string)
     def command(self, command_string):
-        """Send a command to the instrument
+        """Send a command to the instrument.
 
             Args:
                 command_string (str):
-                    A serial command
+                    A serial command.
         """
 
         # Query the instrument over serial. If serial is not configured, use TCP.
         with self.dut_lock:
             # Send command to the instrument over serial. If serial is not configured, send it over TCP.
             if self.device_serial is not None:
                 self._usb_command(command_string)
             elif self.device_tcp is not None:
                 self._tcp_command(command_string)
+            elif self.user_connection is not None:
+                self._user_connection_command(command_string)
             else:
                 raise InstrumentException("No connections configured")
 
             self.logger.info('Sent command to %s: %s', self.serial_number, command_string)
 
     def query(self, query_string):
-        """Send a query to the instrument and return the response
+        """Send a query to the instrument and return the response.
 
             Args:
                 query_string (str):
-                    A serial query ending in a question mark
+                    A serial query ending in a question mark.
 
             Returns:
                The instrument query response as a string.
 
         """
 
         # Query the instrument over serial. If serial is not configured, use TCP.
         with self.dut_lock:
             if self.device_serial is not None:
                 response = self._usb_query(query_string)
             elif self.device_tcp is not None:
                 response = self._tcp_query(query_string)
+            elif self.user_connection is not None:
+                response = self._user_connection_query(query_string)
             else:
                 raise InstrumentException("No connections configured")
 
             self.logger.info('Sent query to %s: %s', self.serial_number, query_string)
             self.logger.info('Received response from %s: %s', self.serial_number, response)
 
         return response
 
     def connect_tcp(self, ip_address, tcp_port, timeout):
-        """Establishes a TCP connection with the instrument on the specified IP address"""
+        """Establishes a TCP connection with the instrument on the specified IP address."""
 
         self.device_tcp = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.device_tcp.settimeout(timeout)
         self.device_tcp.connect((ip_address, tcp_port))
 
         # Send the instrument a line break, wait 100ms, and clear the input buffer so that
         # any leftover communications from a prior session don't gum up the works.
@@ -171,22 +207,22 @@
             read_objects, _, _ = select.select([self.device_tcp], [], [], 0.0)
             if not read_objects:
                 break
             for read_object in read_objects:
                 read_object.recv(1)
 
     def disconnect_tcp(self):
-        """Disconnect the TCP connection"""
+        """Disconnect the TCP connection."""
 
         self.device_tcp.close()
         self.device_tcp = None
 
     def connect_usb(self, serial_number=None, com_port=None, baud_rate=None, data_bits=None,
                     stop_bits=None, parity=None, timeout=None, handshaking=None, flow_control=None):
-        """Establish a serial USB connection"""
+        """Establish a serial USB connection."""
 
         # Scan the ports for devices matching the VID and PID combos of the instrument
         for port in comports():
             if (port.vid, port.pid) in self.vid_pid:
                 # If the com port argument is passed, check for a match
                 if port.device == com_port or com_port is None:
                     # If the serial number argument is passed, check for a match
@@ -212,26 +248,26 @@
             if com_port is None and serial_number is None:
                 raise InstrumentException("No serial connections found")
 
             raise InstrumentException(
                 "No serial connections found with a matching COM port and/or matching serial number")
 
     def disconnect_usb(self):
-        """Disconnect the USB connection"""
+        """Disconnect the USB connection."""
 
         self.device_serial.close()
         self.device_serial = None
 
     def _tcp_command(self, command):
-        """Send a command over the TCP connection"""
+        """Send a command over the TCP connection."""
 
         self.device_tcp.send(command.encode('utf-8') + b'\n')
 
     def _tcp_query(self, query):
-        """Query over the TCP connection"""
+        """Query over the TCP connection."""
 
         self._tcp_command(query)
 
         total_response = ""
 
         # Continuously receive data from the buffer until a line break
         while True:
@@ -246,25 +282,40 @@
             total_response += response
 
             # Return the response once it ends with a line break
             if total_response.endswith("\r\n"):
                 return total_response.rstrip()
 
     def _usb_command(self, command):
-        """Send a command over the serial USB connection"""
+        """Send a command over the serial USB connection."""
 
         self.device_serial.write(command.encode('ascii') + b'\n')
 
     def _usb_query(self, query):
-        """Query over the serial USB connection"""
+        """Query over the serial USB connection."""
 
         self._usb_command(query)
         response = self.device_serial.read_until(b'\r\n').decode('ascii')
 
         # If nothing is returned, raise a timeout error.
         if not response:
             raise InstrumentException("Communication timed out")
 
         return response.rstrip()
 
+    def _user_connection_command(self, command):
+        """Send a command over the user provided connection."""
+
+        self.user_connection.write(command)
+
+    def _user_connection_query(self, query):
+        """Query over the user provided connection."""
+
+        response = self.user_connection.query(query)
+
+        if not response:
+            raise InstrumentException("Communication timed out")
+
+        return response
+
     def _get_identity(self):
         return self.query('*IDN?').split(',')
```

### Comparing `lakeshore-1.6.1/lakeshore/model_121.py` & `lakeshore-1.7.0/lakeshore/model_425.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Implements functionality unique to the Lake Shore Model 121 programmable DC current source"""
+"""Implements functionality unique to the Lake Shore Model 425 Gaussmeter."""
 import serial
 
 from .generic_instrument import GenericInstrument
 
 
-class Model121(GenericInstrument):
-    """A class object representing the Lake Shore Model 121 programmable DC current source"""
+class Model425(GenericInstrument):
+    """A class object representing the Lake Shore Model 425 Gaussmeter."""
 
-    vid_pid = [(0x1FB9, 0x0100)]
+    vid_pid = [(0x1FB9, 0x0401)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=57600,
                  data_bits=7,
                  stop_bits=1,
```

### Comparing `lakeshore-1.6.1/lakeshore/model_155.py` & `lakeshore-1.7.0/lakeshore/model_155.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Implements functionality unique to the Lake Shore 155 Precision Source"""
+"""Implements functionality unique to the Lake Shore 155 Precision Source."""
 
 from time import sleep
 import itertools
 
 from .xip_instrument import XIPInstrument, RegisterBase, StatusByteRegister, StandardEventRegister
 
 
 class PrecisionSourceOperationRegister(RegisterBase):
-    """Class object representing the operation status register"""
+    """Class object representing the operation status register."""
 
     bit_names = [
         "",
         "",
         "",
         "",
         "",
@@ -33,15 +33,15 @@
         self.waiting_for_trigger_event = waiting_for_trigger_event
         self.waiting_for_arm_event = waiting_for_arm_event
         self.trigger_model_is_idle = trigger_model_is_idle
         self.interlock_is_open = interlock_is_open
 
 
 class PrecisionSourceQuestionableRegister(RegisterBase):
-    """Class object representing the questionable status register"""
+    """Class object representing the questionable status register."""
 
     bit_names = [
         "voltage_source_in_current_limit",
         "current_source_in_voltage_compliance",
         "",
         "",
         "",
@@ -60,15 +60,15 @@
         self.voltage_source_in_current_limit = voltage_source_in_current_limit
         self.current_source_in_voltage_compliance = current_source_in_voltage_compliance
         self.calibration_error = calibration_error
         self.inter_processor_communication_error = inter_processor_communication_error
 
 
 class PrecisionSource(XIPInstrument):
-    """A class object representing a Lake Shore 155 precision I/V source"""
+    """A class object representing a Lake Shore 155 precision I/V source."""
 
     vid_pid = [(0x1FB9, 0x0103)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=115200,
@@ -88,28 +88,25 @@
     def sweep_voltage(self,
                       dwell_time,
                       offset_values=None,
                       amplitude_values=None,
                       frequency_values=None):
         """Sweep source output voltage parameters based on list arguments.
 
-        Args:
-            dwell_time (float):
-                The length of time in seconds to wait at each parameter combination.
-                Note that the update rate will be limited by the SCPI communication response time.
-                The response time is usually on the order of 10-30 milliseconds.
-
-            offset_values (list):
-                DC offset values in volts to sweep over
-
-            amplitude_values (list):
-                Peak to peak values in volts to sweep over
-
-            frequency_values (list):
-                Frequency values in Hertz to sweep over
+            Args:
+                dwell_time (float):
+                    The length of time in seconds to wait at each parameter combination.
+                    Note that the update rate will be limited by the SCPI communication response time.
+                    The response time is usually on the order of 10-30 milliseconds.
+                offset_values (list):
+                    DC offset values in volts to sweep over.
+                amplitude_values (list):
+                    Peak to peak values in volts to sweep over.
+                frequency_values (list):
+                    Frequency values in Hertz to sweep over.
 
         """
 
         # Change the output mode to source voltage instead of current.
         self.command("SOURCE:FUNCTION:MODE VOLTAGE")
 
         # Configure the instrument to output a sine wave
@@ -153,23 +150,20 @@
         """Sweep the source output current parameters based on list arguments
 
             Args:
                 dwell_time (float):
                     The length of time in seconds to wait at each parameter combination.
                     Note that the update rate will be limited by the SCPI communication response time.
                     The response time is usually on the order of 10-30 milliseconds.
-
                 offset_values (list):
-                    DC offset values in volts to sweep over
-
+                    DC offset values in volts to sweep over.
                 amplitude_values (list):
-                    Peak to peak values in volts to sweep over
-
+                    Peak to peak values in volts to sweep over.
                 frequency_values (list):
-                    Frequency values in Hertz to sweep over
+                    Frequency values in Hertz to sweep over.
 
         """
 
         # Change the output mode to source current instead of voltage
         self.command("SOURCE:FUNCTION:MODE CURRENT")
 
         # Configure the instrument to output a sine wave
@@ -227,34 +221,30 @@
             self.disable_output()
 
     def route_terminals(self, output_connections_location="REAR"):
         """Configures whether the source output is routed through the front or rear connections.
 
             Args:
                 output_connections_location (str):
-                    * Valid options are:
-                    * "REAR" (Output is routed out the rear connections)
-                    * "FRONT" (Output is routed out the front connections)
+                    Valid options are: "REAR" (Output is routed out the rear connections), and
+                    "FRONT" (Output is routed out the front connections).
 
         """
         self.command("ROUTE:TERMINALS " + output_connections_location)
 
     def output_sine_current(self, amplitude, frequency, offset=0.0, phase=0.0):
         """Configures and enables the source output to be a sine wave current source.
 
             Args:
                 amplitude (float):
                     The peak current amplitude value in amps.
-
                 frequency (float):
                     The source frequency value in hertz.
-
                 offset (float):
                     The DC offset current in amps.
-
                 phase (float):
                     Shifts the phase of the output relative to the reference out. Must be between -180 and 180 degrees.
 
         """
 
         # Change the output mode to source current instead of voltage
         self.command("SOURCE:FUNCTION:MODE CURRENT")
@@ -279,21 +269,18 @@
 
     def output_sine_voltage(self, amplitude, frequency, offset=0.0, phase=0.0):
         """Configures and enables the source output to be a sine wave voltage source.
 
             Args:
                 amplitude (float):
                     The peak voltage amplitude value in volts.
-
                 frequency (float):
                     The source frequency value in hertz.
-
                 offset (float):
                     The DC offset voltage in volts.
-
                 phase (float):
                     Shifts the phase of the output relative to the reference out. Must be between -180 and 180 degrees.
 
         """
 
         # Change the output mode to source voltage instead of current
         self.command("SOURCE:FUNCTION:MODE VOLTAGE")
@@ -387,46 +374,35 @@
         self.command("SOURCE:CURRENT:RANGE:AUTO OFF")
 
     def set_current_range(self, current_range="100E-3"):
         """Manually sets the current range when autorange is disabled.
 
             Args:
                 current_range (str):
-                    * The range in amps. Valid ranges are:
-                    * "100E-3"
-                    * "10E-3"
-                    * "1E-3"
-                    * "100E-6"
-                    * "10E-6"
-                    * "1E-6"
+                    The range in amps. Valid ranges are: "100E-3", "10E-3", "1E-3", "100E-6", "10E-6", and "1E-6".
 
         """
         self.command("SOURCE:CURRENT:RANGE " + current_range)
 
     def set_voltage_range(self, voltage_range="10"):
         """Manually sets the voltage range when autorange is disabled.
 
             Args:
                 voltage_range (str):
-                    * The range in volts. Valid ranges are:
-                    * "100"
-                    * "10"
-                    * "1"
-                    * "0.1"
-                    * "0.01"
+                    The range in volts. Valid ranges are: "100", "10", "1", "0.1", and "0.01".
 
         """
         self.command("SOURCE:VOLTAGE:RANGE " + voltage_range)
 
     def set_current_limit(self, current_limit):
         """Sets the highest settable current output value when in current mode.
 
             Args:
                 current_limit (float):
-                    The maximum settable current in amps. Must be between 0 and 100 milliamps.
+                    The maximum settable current in amps. Must be between 0 and 100 milli-amps.
 
         """
         self.command("SOURCE:CURRENT:LIMIT " + str(current_limit))
 
     def set_voltage_limit(self, voltage_limit):
         """Sets the highest settable voltage output value when in voltage mode.
```

### Comparing `lakeshore-1.6.1/lakeshore/model_224.py` & `lakeshore-1.7.0/lakeshore/model_224.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-"""Implements functionality unique to the Lake Shore Model 224 temperature monitor"""
+"""Implements functionality unique to the Lake Shore Model 224 temperature monitor."""
 
 from enum import IntEnum
 import serial
 from .generic_instrument import GenericInstrument, InstrumentException, RegisterBase
 from .temperature_controllers import StandardEventRegister
 
 
 class Model224AlarmParameters:
-    """Class used to disable or configure an alarm in conjunction with the set/get_alarm_parameters() method"""
+    """Class used to disable or configure an alarm in conjunction with the set/get_alarm_parameters() method."""
 
     def __init__(self, high_value, low_value, deadband, latch_enable, audible=None, visible=None):
-        """Constructor for Model224AlarmParameters class
+        """Constructor for Model224AlarmParameters class.
 
             Args:
                 high_value (float):
-                    Sets the value the source is checked against to activate the
-                    high alarm
+                    Sets the value the source is checked against to activate the high alarm.
                 low_value (float):
                     Sets the value the source is checked against to activate low alarm.
                 deadband (float):
-                    Sets the value that the source must change outside of an alarm
+                    Sets the value that the source must change outside an alarm
                     condition to deactivate an unlatched alarm.
                 latch_enable (bool):
-                    Specifies a latched alarm (False = off, True = on)
+                    Specifies a latched alarm (False = off, True = on).
                 audible (bool):
                     Specifies if the internal speaker will beep when an alarm condition
-                    occurs (False = off, True = on)
-                    Optional parameter.
+                    occurs (False = off, True = on). Optional parameter.
                 visible (bool):
                     Specifies if the Alarm LED on the instrument front panel will blink
-                    when an alarm condition occurs (False = off, True = on)
-                    Optional parameter.
+                    when an alarm condition occurs (False = off, True = on). Optional parameter.
+
         """
         self.high_value = high_value
         self.low_value = low_value
         self.deadband = deadband
         self.latch_enable = latch_enable
         self.audible = audible
         self.visible = visible
@@ -94,38 +92,39 @@
                  sensor_range=None,
                  autorange_enabled=False,
                  compensation=False):
         """Constructor for the Model224InputSensorSettings class.
 
             Args:
                 sensor_type (Model224InputSensorType or int):
-                    * Specifies what type of sensor is being used at the input.
+                    Specifies what type of sensor is being used at the input.
                 preferred_units (Model224InputSensorUnits or int):
-                    * Specifies the preferred units used for sensor readings and alarm setpoints when displayed.
+                    Specifies the preferred units used for sensor readings and alarm set-points when displayed.
                 sensor_range (IntEnum):
-                    * Specifies the range of the sensor.
-                    * Optional if auto range is enabled
+                    Specifies the range of the sensor.
+                    Optional if auto range is enabled.
                 autorange_enabled (bool):
-                    * Defines if autorange is enabled.
-                    * Not applicable for diode sensors
-                    * Defaults to false
+                    Defines if autorange is enabled.
+                    Not applicable for diode sensors.
+                    Defaults to false. Optional parameter.
                 compensation (bool):
-                    * Defines if thermal input compensation is on or off.
-                    * Not applicable for diode sensors
-                    * Defaults to false
+                    Defines if thermal input compensation is on or off.
+                    Not applicable for diode sensors.
+                    Defaults to false. Optional parameter.
+
         """
         self.sensor_type = sensor_type
         self.sensor_range = sensor_range
         self.preferred_units = preferred_units
         self.autorange_enabled = autorange_enabled
         self.compensation = compensation
 
 
 class Model224InterfaceMode(IntEnum):
-    """Enumeration for the mode of the remote interface"""
+    """Enumeration for the mode of the remote interface."""
     LOCAL = 0
     REMOTE = 1
     REMOTE_LOCAL_LOCK = 2
 
 
 class Model224RemoteInterface(IntEnum):
     """Enumeration for the remote interface being used to communicate with the instrument."""
@@ -197,62 +196,60 @@
     """Enumeration of the configured mode of a relay."""
     RELAY_OFF = 0
     RELAY_ON = 1
     ALARMS = 2
 
 
 class Model224CurveFormat(IntEnum):
-    """Enumerations specify formats for temperature sensor curves"""
+    """Enumerations specify formats for temperature sensor curves."""
     MILLIVOLT_PER_KELVIN = 1
     VOLTS_PER_KELVIN = 2
     OHMS_PER_KELVIN = 3
     LOG_OHMS_PER_KELVIN = 4
 
 
 class Model224CurveTemperatureCoefficients(IntEnum):
-    """Enumerations specify positive/negative temperature sensor curve coefficients"""
+    """Enumerations specify positive/negative temperature sensor curve coefficients."""
     NEGATIVE = 1
     POSITIVE = 2
 
 
 class Model224DiodeExcitationCurrent(IntEnum):
     """Enum type representing the different excitation currents available for a diode sensor."""
     TEN_MICRO_AMPS = 0
     ONE_MILLI_AMP = 1
 
 
 class Model224SoftCalSensorTypes(IntEnum):
-    """Enum type representing the standard curves used to generate a SoftCal curve. The 3 standard curves each
-    represent a different type of sensor that can be calibrated with a SoftCal curve."""
+    """Enum type representing the standard curves used to generate a SoftCal curve.
+
+        The 3 standard curves each represent a different type of sensor that can be calibrated with a SoftCal curve.
+    """
     DT_400 = 1
     PT_100 = 6
     PT_1000 = 7
 
 
 class Model224CurveHeader:
-    """A class that configures the user curve header and corresponding parameters"""
+    """A class that configures the user curve header and corresponding parameters."""
 
     def __init__(self, curve_name, serial_number, curve_data_format, temperature_limit, coefficient):
-        """Constructor for Model224CurveHeader class
+        """Constructor for Model224CurveHeader class.
 
             Args:
                 curve_name (str):
-                    Specifies curve name (limit of 15 characters)
-
+                    Specifies curve name (limit of 15 characters).
                 serial_number (str):
-                    Specifies curve serial number (limit of 10 characters)
-
+                    Specifies curve serial number (limit of 10 characters).
                 curve_data_format (Model224CurveFormat):
-                    Specifies the curve data format
-
+                    Specifies the curve data format.
                 temperature_limit (float):
-                    * Specifies the curve temperature limit in Kelvin
-
+                    Specifies the curve temperature limit in Kelvin.
                 coefficient (Model224CurveTemperatureCoefficients):
-                    * Specifies the curve temperature coefficient
+                    Specifies the curve temperature coefficient.
 
         """
 
         self.curve_name = curve_name
         self.serial_number = serial_number
         self.curve_data_format = curve_data_format
         self.temperature_limit = temperature_limit
@@ -305,16 +302,19 @@
         self.message_available = message_available
         self.event_summary = event_summary
         self.master_summary_status = master_summary_status
         self.operation_summary = operation_summary
 
 
 class Model224ReadingStatusRegister(RegisterBase):
-    """Class object representing the reading status of an input. While not a literal register, the return of an int
-    representation of multiple booleans makes it conveninet to represent this functionality as a register."""
+    """Class object representing the reading status of an input.
+
+        While not a literal register, the return of an int representation of multiple booleans makes it convenient to
+        represent this functionality as a register.
+    """
     bit_names = [
         "invalid_reading",
         "",
         "",
         "",
         "temperature_under_range",
         "temperature_over_range",
@@ -332,15 +332,15 @@
         self.temperature_under_range = temperature_under_range
         self.temperature_over_range = temperature_over_range
         self.sensor_units_zero = sensor_units_zero
         self.sensor_units_over_range = sensor_units_over_range
 
 
 class Model224(GenericInstrument):
-    """A class object representing the Lake Shore Model 224 temperature monitor"""
+    """A class object representing the Lake Shore Model 224 temperature monitor."""
 
     vid_pid = [(0x1FB9, 0x0204)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=57600,
@@ -365,44 +365,43 @@
             raise InstrumentException('Query Error')
         if event_register.command_error:
             raise InstrumentException('Command Error: Invalid Command or Query')
         if event_register.execution_error:
             raise InstrumentException('Execution Error: Instrument not able to execute command or query.')
 
     def command(self, *commands, check_errors=True):
-        """Send a SCPI command or multiple commands to the instrument
+        """Sends an SCPI command or multiple commands to the instrument.
 
             Args:
                 commands (str):
-                    * A serial command
-
-            Kwargs:
+                    A serial command.
                 check_errors (bool):
-                    * Chooses whether to check for and raise errors after sending a command. True by default.
+                    Chooses whether to check for and raise errors after sending a command. True by default. kwarg.
+                    Optional Parameter
 
         """
 
         # Group all commands and queries a single string with SCPI delimiters.
         command_string = ";:".join(commands)
 
         if check_errors:
             self.query(command_string)
         else:
             command_string += ";*OPC?"
             self.query(command_string, check_errors=False)
 
     def query(self, *queries, check_errors=True):
-        """Send a query to the instrument and return the response
+        """Send a query to the instrument and return the response.
 
             Args:
                 queries (str):
-                    * A serial query ending in a question mark
+                    A serial query ending in a question mark.
 
-            Return:
-               * The instrument query response as a string.
+            Returns:
+                The instrument query response as a string.
 
         """
 
         # Group all commands and queries a single string with SCPI delimiters.
         query_string = ";:".join(queries)
 
         # Append the query with an additional error buffer query.
@@ -417,176 +416,172 @@
             self._error_check(error_code)
             response = ';'.join(response_list)
 
         return response
 
     def get_standard_event_enable_mask(self):
         """Returns the names of the standard event enable register bits and their values.
-        These values determine which bits propagate to the standard event register"""
+
+            These values determine which bits propagate to the standard event register.
+        """
 
         response = self.query("*ESE?")
         status_register = Model224StandardEventRegister.from_integer(response)
         return status_register
 
     def set_standard_event_enable_mask(self, register_mask):
         """Configures values of the standard event enable register bits.
-        These values determine which bits propagate to the standard event register
+
+            These values determine which bits propagate to the standard event register.
 
             Args:
                 register_mask (Model224StandardEventRegister):
-                    An StandardEventRegister class object with all bits set to a value
+                    An StandardEventRegister class object with all bits set to a value.
 
         """
 
         integer_representation = register_mask.to_integer()
         self.command("*ESE " + str(integer_representation))
 
     def clear_interface_command(self):
-        """Clears the bits in the Status Byte Register, Standard Event Status Register, and Operation Event Register,
-        and terminates all pending operations. Clears the interface, but not the controller."""
+        """Clears the bits of the interface and terminates all pending operations.
+
+            Clears the bits in the Status Byte Register, Standard Event Status Register, and Operation Event Register,
+            and terminates all pending operations. Clears the interface, but not the controller.
+        """
 
         self.command("*CLS")
 
     def reset_instrument(self):
-        """Sets controller parameters to power-up settings"""
+        """Sets controller parameters to power-up settings."""
 
         self.command("*RST")
 
     def set_service_request(self, register_mask):
-        """Manually enable/disable the mask of the corresponding status flag bit in the status
-        byte register
+        """Manually enable/disable the mask of the corresponding status-flag bit in the status byte register.
 
             Args:
                 register_mask (Model224ServiceRequestRegister):
-                    A Model224ServiceRequestRegister class object with all bits configured
+                    A Model224ServiceRequestRegister class object with all bits configured.
         """
 
         integer_representation = register_mask.to_integer()
         self.command("*SRE " + str(integer_representation))
 
     def get_service_request(self):
-        """Returns the status byte register bits and their values as a class instance"""
+        """Returns the status byte register bits and their values as a class instance."""
 
         response = self.query("*SRE?")
         status_register = Model224ServiceRequestRegister.from_integer(response)
         return status_register
 
     def get_status_byte(self):
-        """Returns the status flag bits as a class instance without resetting the register"""
+        """Returns the status flag bits as a class instance without resetting the register."""
 
         response = self.query("*STB?")
         status_flag = Model224StatusByteRegister.from_integer(response)
         return status_flag
 
     def get_self_test(self):
-        """Instrument self test result completed at power up
+        """Instrument self test result completed at power up.
 
-            Return:
+            Returns:
                 test_errors (bool):
-                    * True = errors found
-                    * False = no errors found
+                    True means errors found, and False means no errors found.
         """
 
         test_errors = bool(int(self.query("*TST?")))
         return test_errors
 
     def set_wait_to_continue(self):
         """Causes the IEEE-488 interface to hold off until all pending operations have been completed.
-        This has the same function as the set_operation_complete() method, except that it does not set the
-        Operation Complete event bit in the Event Status Register"""
+
+            This has the same function as the set_operation_complete() method, except that it does not set the
+            Operation Complete event bit in the Event Status Register.
+        """
 
         self.command("*WAI")
 
     def set_to_factory_defaults(self):
         """Sets all the settings and configurations to their factory default values."""
         self.command("DFLT 99")
 
     def get_reading_status(self, input_channel):
         """Returns the reading status of any input status flags that may be set.
 
             Args:
                 input_channel (str):
-                    * The input to check for reading status flags.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                    The input to check for reading status flags.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
             Returns:
                 (dict):
-                    {invalid_reading: bool, temperature_under_range: bool, temperature_over_range: bool,
-                    sensor_units_zero: bool, sensor_units_over_range: bool}
+                    {"invalid_reading": bool, "temperature_under_range": bool, "temperature_over_range": bool,
+                    "sensor_units_zero": bool, "sensor_units_over_range": bool}
         """
         flag_code = int(self.query(f"RDGST? {input_channel}"))
         reading_status = Model224ReadingStatusRegister.from_integer(flag_code)
         return reading_status
 
     def get_kelvin_reading(self, input_channel):
-        """Returns the temperature value in kelvin of either channel
+        """Returns the temperature value in kelvin of either channel.
 
             Args:
                 input_channel:
-                    * Selects the channel to retrieve measurement.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                    Selects the channel to retrieve measurement.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
             Returns:
                 (float):
-                    The reading of the sensor in kelvin
+                    The reading of the sensor in kelvin.
 
 
         """
 
         return float(self.query(f"KRDG? {input_channel}"))
 
     def get_sensor_reading(self, input_channel):
         """Returns the sensor reading in the sensor's units.
 
             Args:
                 input_channel:
-                    * Selects the channel to retrieve measurement.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                    Selects the channel to retrieve measurement.
+                    Options are: Options are: A, B, C(1 - 5), D(1 - 5).
 
             Returns:
                 reading (float):
-                    * The raw sensor reading in the units of the connected sensor
+                    The raw sensor reading in the units of the connected sensor.
 
         """
 
         return float(self.query(f"SRDG? {input_channel}"))
 
     def get_celsius_reading(self, input_channel):
         """Returns the given input's temperature reading in degrees Celsius.
 
             Args:
-                input_channel (str)
+                input_channel (str):
                     Selects input to retrieve measurement from.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
             Returns:
                 (float):
-                    Temperature readings in degrees Celsius
+                    Temperature readings in degrees Celsius.
         """
         return float(self.query(f"CRDG? {input_channel}"))
 
     def get_all_inputs_celsius_reading(self):
         """Returns the temperature reading in degrees Celsius of all the inputs.
 
             Returns:
                 (dict):
-                    {input_a_reading: float, input_b_reading: float, input_c1_reading: float, input_c2_reading: float,
-                    input_c3_reading: float, input_c4_reading: float, input_c5_reading: float, input_d1_reading: float,
-                    input_d2_reading: float, input_d3_reading: float, input_d4_reading: float, input_d5_reading: float}
+                    {"input_a_reading": float, "input_b_reading": float, "input_c1_reading": float,
+                    "input_c2_reading": float, "input_c3_reading": float, "input_c4_reading": float,
+                    "input_c5_reading": float, "input_d1_reading": float, "input_d2_reading": float,
+                    "input_d3_reading": float, "input_d4_reading": float, "input_d5_reading": float}
         """
         reading = self.query("CRDG? 0")
         separated_readings = reading.split(",")
         return {'input_a_reading': float(separated_readings[0]),
                 'input_b_reading': float(separated_readings[1]),
                 'input_c1_reading': float(separated_readings[2]),
                 'input_c2_reading': float(separated_readings[3]),
@@ -596,23 +591,23 @@
                 'input_d1_reading': float(separated_readings[7]),
                 'input_d2_reading': float(separated_readings[8]),
                 'input_d3_reading': float(separated_readings[9]),
                 'input_d4_reading': float(separated_readings[10]),
                 'input_d5_reading': float(separated_readings[11])}
 
     def set_input_diode_excitation_current(self, input_channel, diode_current):
-        """Sets the excitation current of a diode sensor. Input must be configured for a diode sensor for command
-        to work. Current defaults to 10uA.
+        """Sets the excitation current of a diode sensor.
+
+            Input must be configured for a diode sensor for command to work. Current defaults to 10uA.
 
             Args:
                 input_channel (str):
-                    * The input to configure the diode excitation current for.
-
+                    The input to configure the diode excitation current for.
                 diode_current (Model224DiodeExcitationCurrent):
-                    * The excitation current for the diode sensor.
+                    The excitation current for the diode sensor.
 
         """
         self.command(f"DIOCUR {input_channel},{diode_current}")
 
     def get_input_diode_excitation_current(self, input_channel):
         """Returns the diode excitation current for the given diode sensor.
 
@@ -625,243 +620,232 @@
                     A member of the Model224DiodeExcitationCurrent enum class.
 
         """
         diode_current_int = int(self.query(f"DIOCUR? {input_channel}"))
         return Model224DiodeExcitationCurrent(diode_current_int)
 
     def set_sensor_name(self, channel, sensor_name):
-        """Sets a given name to a sensor on the specified channel
+        """Sets a given name to a sensor on the specified channel.
 
             Args:
                 channel (str):
-                    * Specifies which the sensor to name is on.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                    Specifies which the sensor to name is on.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
                 sensor_name(str):
-                    * Name user wants to give to the sensor on the specified channel
+                    Name user wants to give to the sensor on the specified channel.
 
         """
 
         self.command(f"INNAME {channel},\"{sensor_name}\"")
 
     def get_sensor_name(self, channel):
-        """Returns the name of the sensor on the specified channel
+        """Returns the name of the sensor on the specified channel.
 
             Args:
                 channel (str):
-                    * Specifies which input sensor to retrieve name of.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                    Specifies which input sensor to retrieve name of.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
             Returns:
-                name (str)
-                    * Name associated with the sensor
+                name (str):
+                    Name associated with the sensor.
 
         """
 
         return self.query(f"INNAME? {channel}")
 
     def set_display_contrast(self, contrast_level):
-        """Sets the contrast level for the front panel display
+        """Sets the contrast level for the front panel display.
 
             Args:
                 contrast_level (int):
-                    * Display contrast for the front panel LCD screen
-                    * Options are:
-                        * 1 - 32
+                    Display contrast for the front panel LCD screen. Options are:
+                    1 - 32.
 
         """
 
         self.command(f"BRIGT {contrast_level}")
 
     def get_display_contrast(self):
-        """Returns the contrast level of front panel display
+        """Returns the contrast level of front panel display.
 
-            Return:
+            Returns:
                 (int):
-                    * Contrast level of the front panel LCD screen
+                    Contrast level of the front panel LCD screen.
 
         """
 
         return int(self.query("BRIGT?"))
 
     def set_ieee_488(self, address):
-        """Specifies the IEEE address
+        """Specifies the IEEE address.
 
             Args:
                 address (int):
-                    * 1-30 (0 and 31 reserved)
+                    1-30 (0 and 31 reserved).
         """
         self.command(f"IEEE {address}")
 
     def get_ieee_488(self):
-        """Returns the IEEE address set
+        """Returns the IEEE address set.
 
-            Return:
+            Returns:
                 address (int):
-                    * 1-30 (0 and 31 reserved)
+                    1-30 (0 and 31 reserved).
 
         """
         return int(self.query("IEEE?"))
 
     def set_led_state(self, state):
         """Sets the front panel LEDs to on or off.
 
             Args:
-                state (bool)
-                    * Sets the LEDs to functional or nonfunctional. Options are:
-                    * False for off or True for on
+                state (bool):
+                    Sets the LEDs to functional or nonfunctional. Options are:
+                    False for off, True for on.
 
         """
         self.command(f"LEDS {str(int(state))}")
 
     def get_led_state(self):
-        """Returns whether or not front panel LEDs are enabled.
+        """Returns whether front panel LEDs are enabled.
 
             Returns:
-                state (bool)
-                    * Specifies whether front panel LEDs are functional. Returns:
-                    * False if disabled, True enabled.
+                state (bool):
+                    Specifies whether front panel LEDs are functional. Returns:
+                    False if disabled, True enabled.
 
         """
         return bool(int(self.query("LEDS?")))
 
     def set_keypad_lock(self, state, code):
         """Locks or unlocks front panel keypad (except for alarms and disabling heaters).
 
             Args:
-                state (bool)
-                    * Sets the keypad to locked or unlocked. Options are:
-                    * False for unlocked or True for locked
-
-                code (int)
-                    * Specifies 3 digit lock-out code. Options are:
-                    * 000 - 999
+                state (bool):
+                    Sets the keypad to locked or unlocked. Options are:
+                    False for unlocked or True for locked.
+                code (int):
+                    Specifies 3 digit lock-out code. Options are:
+                    000 - 999.
 
         """
         self.command(f"LOCK {str(int(state))},{str(code)}")
 
     def get_keypad_lock(self):
         """Returns the state of the keypad lock and the lock-out code.
 
-            Return:
+            Returns:
                 (dict):
-                    * [state: bool, code: int]
+                    {"state": bool, "code": int}
 
         """
         output_string = self.query("LOCK?")
         separated_response = output_string.split(",")
         return {'state': bool(int(separated_response[0])),
                 'code': int(separated_response[1])}
 
     def get_min_max_data(self, input_channel):
-        """Returns the minimum and maximum data from an input
+        """Returns the minimum and maximum data from an input.
 
             Args:
                 input_channel (str):
-                    Specifies which input to query
-            Return:
+                    Specifies which input to query.
+
+            Returns:
                 min_max_data (dict):
-                    * [minimum: float, maximum: float]
+                    {"minimum": float, "maximum": float}
 
         """
         min_max_data = self.query("MDAT? " + str(input_channel)).split(",")
         min_max_dictionary = {"minimum": float(min_max_data[0]),
                               "maximum": float(min_max_data[1])}
         return min_max_dictionary
 
     def reset_min_max_data(self):
-        """Resets the minimum and maximum input data"""
+        """Resets the minimum and maximum input data."""
         self.command("MNMXRST")
 
     def set_input_curve(self, input_channel, curve_number):
-        """Specifies the curve an input uses for temperature conversion
+        """Specifies the curve an input uses for temperature conversion.
 
             Args:
                 input_channel (str):
-                    Specifies which input to configure
-
+                    Specifies which input to configure.
                 curve_number (int):
-                    * 0 = none, 1-20 = standard curves, 21-59 = user curves
+                    0 = none, 1-20 = standard curves, 21-59 = user curves.
 
         """
         self.command(f"INCRV {str(input_channel)},{str(curve_number)}")
         # Check that the user mapped an input to a curve (not just set the input to no curve)
         if curve_number != 0:
             # Query the curve mapped to input_channel, if the query returns zero,
             # an invalid curve was selected for the specified input
             set_curve = self.get_input_curve(input_channel)
             if set_curve == 0:
                 raise InstrumentException("The specified curve type does not match the configured input type")
 
     def get_input_curve(self, input_channel):
-        """Returns the curve number being used for a given input
+        """Returns the curve number being used for a given input.
 
             Args:
                 input_channel (str):
-                    Specifies which input to query
+                    Specifies which input to query.
 
-            Return:
+            Returns:
                 curve_number (int):
-                    * 0-59
+                    0-59.
 
         """
         return int(self.query(f"INCRV? {str(input_channel)}"))
 
     def set_website_login(self, username, password):
         """Sets the username and password to connect instrument to website.
 
             Args:
-                username (str)
-                    * Username to set for login.
-                    * Must be less than or equal to 15 characters.
-                    * Method automatically puts quotation marks around string, so they are not needed in the
-                      string literal passed into the method.
-
-                password (str)
-                    * password to set for login.
-                    * Must be less than or equal to 15 characters.
-                    * Method automatically puts quotation marks around string, so they are not needed in the
-                      string literal passed into the method.
+                username (str):
+                    Username to set for login.
+                    Must be less than or equal to 15 characters.
+                    Method automatically puts quotation marks around string, so they are not needed in the
+                    string literal passed into the method.
+                password (str):
+                    Password to set for login.
+                    Must be less than or equal to 15 characters.
+                    Method automatically puts quotation marks around string, so they are not needed in the
+                    string literal passed into the method.
 
         """
         self.command("WEBLOG \"" + username + "\",\"" + password + "\"")
 
     def get_website_login(self):
         """Returns the set username and password for web login for the instrument.
 
             Returns:
                 (dict):
-                    {username: str, password: str}
+                    {"username": str, "password": str}
         """
         username_password = self.query("WEBLOG?")
         separated_string = username_password.split(",")
         # Remove padded whitespace and quotations in the returned username and password
         username = separated_string[0].strip(' "')
         password = separated_string[1].strip(' "')
         return {"username": username,
                 "password": password}
 
     def set_alarm_parameters(self, input_channel, alarm_enable, alarm_settings=None):
-        """Configures the alarm parameters for an input
+        """Configures the alarm parameters for an input.
 
             Args:
                 input_channel (str):
-                    Specifies which input to configure
+                    Specifies which input to configure.
                 alarm_enable (bool):
                     Specifies whether to turn on the alarm for the input, or turn the alarm off.
                 alarm_settings (Model224AlarmParameters):
-                    See Model224AlarmParameters class. Optional if alarm_enable is set to False
+                    See Model224AlarmParameters class. Optional if alarm_enable is set to False.
 
         """
 
         if alarm_enable:
             if alarm_settings.audible is None:
                 audible = 0
             else:
@@ -873,200 +857,177 @@
             self.command(f"ALARM {input_channel.upper()},{int(alarm_enable)},{alarm_settings.high_value}," +
                         f"{alarm_settings.low_value},{alarm_settings.deadband},{int(alarm_settings.latch_enable)}," +
                         f"{audible},{visible}")
         else:
             self.command("ALARM " + str(input_channel.upper()) + "," + str(int(alarm_enable)) + ",0,0,0,0,0,0")
 
     def get_alarm_parameters(self, input_channel):
-        """Returns the present state of all alarm parameters
+        """Returns the present state of all alarm parameters.
 
             Args:
                 input_channel (str):
-                    Specifies which input to configure
+                    Specifies which input to configure.
 
-            Return:
+            Returns:
                 (dict):
-                    {alarm_enable: bool, alarm_settings: Model224AlarmParameters}
+                    {"alarm_enable": bool, "alarm_settings": Model224AlarmParameters}.
 
         """
         parameters = self.query("ALARM? " + str(input_channel)).split(",")
         alarm_enable = bool(int(parameters[0]))
         alarm_settings = Model224AlarmParameters(float(parameters[1]), float(parameters[2]),
                                                  float(parameters[3]), bool(int((parameters[4]))),
                                                  audible=bool(int(parameters[5])), visible=bool(int(parameters[6])))
         return {'alarm_enable': alarm_enable,
                 'alarm_settings': alarm_settings}
 
     def get_alarm_status(self, input_channel):
-        """Returns the high state and low state of the alarm for the specified channel
+        """Returns the high state and low state of the alarm for the specified channel.
 
             Args:
-                input_channel (str)
-                    * Specifies which input channel to read from.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                input_channel (str):
+                    Specifies which input channel to read from.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
             Returns:
                 (dict):
-                    {high_state: bool, low_state: bool}
-                        * high_state (bool)
-                            * True if high state is on, False if high state is off
-
-                        * low_state (bool)
-                            * True if low state is on, False if low state is off
+                    {"high_state": bool, "low_state": bool}
 
         """
         response = self.query("ALARMST? " + str(input_channel))
         separated_response = response.split(",")
         return {"high_state": bool(int(separated_response[0])),
                 "low_state": bool(int(separated_response[1]))}
 
     def reset_alarm_status(self):
         """Clears the high and low status of all alarms."""
         self.command("ALMRST")
 
     def set_curve_header(self, curve_number, curve_header):
-        """Configures the user curve header
+        """Configures the user curve header.
 
             Args:
                 curve_number (int):
-                    * Specifies which curve to configure.
-                    * Options are:
-                        * 21 - 59
-
+                    Specifies which curve to configure.
+                    Options are: 21 - 59.
                 curve_header (Model224CurveHeader):
-                    * A Model224CurveHeader class object containing the desired curve information
+                    A Model224CurveHeader class object containing the desired curve information.
 
         """
         command_string = (f"CRVHDR {curve_number},{curve_header.curve_name},{curve_header.serial_number}," +
                         f"{curve_header.curve_data_format},{curve_header.temperature_limit},{curve_header.coefficient}")
 
         self.command(command_string)
 
     def get_curve_header(self, curve):
-        """Returns parameters set on a particular user curve header
+        """Returns parameters set on a particular user curve header.
 
             Args:
                 curve (int):
-                    * Specifies a curve to retrieve
-                    * Options are:
-                        * 21 - 59
+                    Specifies a curve to retrieve.
+                    Options are: 21 - 59.
 
             Returns:
                 header (Model224CurveHeader):
-                    * A Model224CurveHeader class object containing the desired curve information
+                    A Model224CurveHeader class object containing the desired curve information.
 
         """
         response = self.query(f"CRVHDR? {curve}")
         curve_header = response.split(",")
         header = Model224CurveHeader(str(curve_header[0]),
                                      str(curve_header[1]),
                                      Model224CurveFormat(int(curve_header[2])),
                                      float(curve_header[3]),
                                      Model224CurveTemperatureCoefficients(int(curve_header[4])))
 
         return header
 
     def set_curve_data_point(self, curve, index, sensor_units, temperature):
-        """Configures a user curve point
+        """Configures a user curve point.
 
             Args:
                 curve (int or str):
-                    * Specifies which curve to configure
-
+                    Specifies which curve to configure.
                 index (int):
-                    * Specifies the points index in the curve
-
+                    Specifies the points index in the curve.
                 sensor_units (float):
-                    * Specifies sensor units for this point to 6 digits
-
+                    Specifies sensor units for this point to 6 digits.
                 temperature (float):
-                    * Specifies the corresponding temperature in Kelvin for this point to 6 digits
+                    Specifies the corresponding temperature in Kelvin for this point to 6 digits.
 
         """
         self.command(f"CRVPT {curve},{index},{sensor_units},{temperature}")
 
     def get_curve_data_point(self, curve, index):
-        """Returns a standard or user curve data point
+        """Returns a standard or user curve data point.
 
             Args:
                 curve (int):
-                    * Specifies which curve to query
-
+                    Specifies which curve to query.
                 index (int):
-                    * Specifies the points index in the curve
+                    Specifies the points index in the curve.
 
-            Return:
-                curve_point (tuple)
-                    * (sensor_units: float, temp_value: float))
+            Returns:
+                curve_point (tuple):
+                    (sensor_units: float, temp_value: float)).
 
         """
         curve_point = self.query(f"CRVPT? {curve},{index}").split(",")
         return float(curve_point[0]), float(curve_point[1])
 
     def delete_curve(self, curve):
-        """Deletes the user curve
+        """Deletes the user curve.
 
             Args:
                 curve (int):
-                    * Specifies a user curve to delete
+                    Specifies a user curve to delete.
 
         """
         self.command(f"CRVDEL {curve}")
 
     def generate_and_apply_soft_cal_curve(self, source_curve, curve_number, serial_number, calibration_point_1,
                                           calibration_point_2=(0, 0), calibration_point_3=(0, 0)):
-        """Creates a SoftCal curve from 1-3 temperature/sensor points and a standard curve. Inputs generated curve
-        into the given curve number.
+        """Creates a SoftCal curve from 1-3 temperature/sensor points and a standard curve.
+
+            Inputs generated curve into the given curve number.
 
             Args:
                 source_curve (Model224SoftCalSensorTypes):
-                    * The standard curve to use to generate the SoftCal curve from along with calibration points.
-
+                    The standard curve to use to generate the SoftCal curve from along with calibration points.
                 curve_number (int):
-                    * The curve number to save the generated curve to.
-                    * Options are:
-                        * 21 - 59
-
+                    The curve number to save the generated curve to.
+                    Options are: 21 - 59.
                 serial_number (str):
-                    * Serial number of the user curve.
-                    * Maximum of 10 characters
-
+                    Serial number of the user curve.
+                    Maximum of 10 characters.
                 calibration_point_1 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-
+                    Tuple of two floats in the form (temperature_value, sensor_value).
                 calibration_point_2 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
-
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
                 calibration_point_3 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional parameter.
 
         """
         command_string = (f"SCAL {source_curve},{curve_number},{serial_number}," +
                             f"{calibration_point_1[0]},{calibration_point_1[1]}," +
                             f"{calibration_point_2[0]},{calibration_point_2[1]}," +
                             f"{calibration_point_3[0]},{calibration_point_3[1]}")
         self.command(command_string)
 
     def get_curve(self, curve):
-        """Returns a list of all the data points in a particular curve
+        """Returns a list of all the data points in a particular curve.
 
             Args:
                 curve (int):
-                    * Specifies which curve to set
+                    Specifies which curve to set.
 
             Return:
                 data_points (list):
-                    * A list containing every point in the curve represented as a tuple
-                        * (sensor_units: float, temp_value: float)
+                    A list containing every point in the curve represented as a tuple
+                    (sensor_units: float, temp_value: float).
 
         """
 
         data_points = []
         true_point_index = 0
         for i in range(0, 200):
             point = self.get_curve_data_point(curve, i + 1)
@@ -1076,154 +1037,131 @@
 
         # Remove all extraneous points
         data_points = data_points[:true_point_index + 1]
 
         return data_points
 
     def set_curve(self, curve, data_points):
-        """Method to define a user curve using a list of data points
+        """Method to define a user curve using a list of data points.
 
             Args:
                 curve (int):
-                    * Specifies which curve to set
-
+                    Specifies which curve to set.
                 data_points (list):
-                    * A list containing every point in the curve represented as a tuple
-                        * (sensor_units: float, temp_value: float)
+                    A list containing every point in the curve represented as a tuple
+                        (sensor_units: float, temp_value: float).
 
         """
 
         self.delete_curve(curve)
 
         for index, point in data_points:
             self.set_curve_data_point(curve, index + 1, point[0], point[1])
 
     def get_relay_status(self, relay_channel):
         """Returns whether the specified relay is On or Off.
 
             Args:
-                relay_channel (int)
-                    * The relay channel to query.
-                    * Options are:
-                        * 1 or 2
+                relay_channel (int):
+                    The relay channel to query.
+                    Options are: 1 or 2.
 
             Returns:
                 (bool):
-                    * True if relay is on, False if relay is off.
+                    True if relay is on, False if relay is off.
         """
         return bool(int(self.query(f"RELAYST? {str(relay_channel)}")))
 
     def set_filter(self, input_channel, filter_enabled, number_of_points=8, filter_reset_threshold=10):
-        """Enables or disables a filter for the readings of the specified input channel. Filter is a running
-        average that smooths input readings exponentially.
+        """Enables or disables a filter for the readings of the specified input channel.
+
+            Filter is a running average that smooths input readings exponentially.
 
             Args:
                 input_channel (str):
-                    * The input to set or disable a filter for.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
-
+                    The input to set or disable a filter for.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
                 filter_enabled (bool):
-                    * Enables or disables a filter for the input channel.
-                    * True for enabled, False for disabled.
-
+                    Enables or disables a filter for the input channel.
+                    True for enabled, False for disabled.
                 number_of_points (int):
-                    * Specifies the number of points used for the filter.
-                    * Inputting a larger number of points will slow down the instrument's response to changes in
-                        temperature.
-                    * Options are:
-                        * 2 - 64
-                    * Optional if disabling the filter function.
-
+                    Specifies the number of points used for the filter.
+                    Inputting a larger number of points will slow down the instrument's response to changes in
+                    temperature.
+                    Options are: 2 - 64
+                    Optional if disabling the filter function.
                 filter_reset_threshold (int):
-                    * Specifies the limit for restarting the filter, represented by a percent of the full scale reading.
-                        If raw reading differs from filtered value by more than this threshold, filter averaging resets.
-                    * Options are:
-                        * 1% - 10%
-                    * Optional if disabling the filter function.
+                    Specifies the limit for restarting the filter, represented by a percent of the full scale reading.
+                    If raw reading differs from filtered value by more than this threshold, filter averaging resets.
+                    Options are: 1% - 10%.
+                    Optional if disabling the filter function.
 
         """
         self.command("FILTER " + str(input_channel) + "," + str(int(filter_enabled)) + "," + str(number_of_points) +
                      "," + str(filter_reset_threshold))
 
     def get_filter(self, input_channel):
         """Retrieves information about the filter set on the specified input channel.
 
             Args:
                 input_channel (str):
-                    * The input to query for filter information.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                    The input to query for filter information.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
             Returns:
                 (dict):
-                    {filter_enabled: bool, number_of_points: int, filter_reset_threshold: int}
+                    {"filter_enabled": bool, "number_of_points": int, "filter_reset_threshold": int}
 
         """
         filter_information = self.query(f"FILTER? {str(input_channel)}")
         separated_information = filter_information.split(",")
         return {'filter_enabled': bool(int(separated_information[0])),
                 'number_of_points': int(separated_information[1]),
                 'filter_reset_threshold': int(separated_information[2])}
 
     def configure_input(self, input_channel, settings):
         """Configures a sensor for measurement input readings.
 
             Args:
                 input_channel (str):
-                    The input to configure the input for. Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                    The input to configure the input for.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
                 settings (Model224InputSensorSettings):
                     Object of the Model224InputSensorSettings containing information for sensor setup.
 
         """
         command_string = (f"INTYPE {input_channel},{settings.sensor_type},{int(settings.autorange_enabled)}," +
                         f"{settings.sensor_range},{int(settings.compensation)},{settings.preferred_units}")
         self.command(command_string)
 
     def disable_input(self, input_channel):
         """Disables the selected input channel.
 
             Args:
                 input_channel (str):
-                    The input to disable. Options are:
-                        * A
-                        * B
-                        * C (1 - 5)
-                        * D (1 - 5)
+                    The input to disable.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
         """
         # Fill all parameters with 0 to disable
         self.command(f"INTYPE {str(input_channel)},0,0,0,0,0")
 
     def get_input_configuration(self, input_channel):
         """Returns the configuration settings of the sensor at the specified input channel.
 
             Args:
-                input_channel (str)
-                    The input to query. Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
+                input_channel (str):
+                    The input to query.
+                    Options are: A, B, C(1 - 5), D(1 - 5).
 
             Returns:
                 (Model224InputSensorSettings):
                     Object of type Model224InputSensorSettings containing information about the sensor at the given
-                    input_channel
+                    input_channel.
 
         """
         settings_string = self.query(f"INTYPE? {str(input_channel)}")
         separated_settings = settings_string.split(",")
         # Convert sensor_range depending on sensor type
         sensor_type = int(separated_settings[0])
         if sensor_type == 1:
@@ -1244,26 +1182,26 @@
 
     def select_remote_interface(self, remote_interface):
         """Selects the remote interface to use for communications.
 
             Args:
                 remote_interface (Model224RemoteInterface):
                     Object of enum type Model224RemoteInterface, representing the type of interface used for
-                    communications
+                    communications.
 
         """
         self.command(f"INTSEL {remote_interface}")
 
     def get_remote_interface(self):
         """Returns the remote interface being used for communications.
 
             Returns:
                 (Model224RemoteInterface):
                     Object of enum type Model224RemoteInterface representing the interface being used for
-                    communications
+                    communications.
 
         """
         interface_number = int(self.query("INTSEL?"))
         return Model224RemoteInterface(interface_number)
 
     def select_interface_mode(self, interface_mode):
         """Selects the mode for the remote interface being used.
@@ -1287,68 +1225,64 @@
         return Model224InterfaceMode(mode_number)
 
     def set_display_field_settings(self, field, input_channel, display_units):
         """Configures a display field in custom display mode.
 
             Args:
                 field (int):
-                    * Specifies which display field to configure.
-                    * Options are:
-                        * 1 - 8
-
-                input_channel (Model224InputChannel)
-                    * Defines which input to display.
-
-                display_units (Model224DisplayFieldUnits)
-                    * Defines which units to display reading in.
+                    Specifies which display field to configure.
+                    Options are: 1 - 8.
+                input_channel (Model224InputChannel):
+                    Defines which input to display.
+                display_units (Model224DisplayFieldUnits):
+                    Defines which units to display reading in.
 
         """
         self.command(f"DISPFLD {field},{input_channel},{display_units}")
 
     def get_display_field_settings(self, field):
         """Returns the settings of a single display field in custom display mode.
 
             Args:
                 field (int):
-                    * Specifies the display field to query.
-                    * Options are:
-                        * 1 - 8
+                    Specifies the display field to query.
+                    Options are: 1 - 8.
 
             Returns:
                 (dict):
-                    {input_channel: Model224InputChannel, display_units: Model224DisplayFieldUnits}
+                    {"input_channel": Model224InputChannel, "display_units": Model224DisplayFieldUnits}
 
         """
         display_field_settings = self.query("DISPFLD? " + str(field))
         separated_settings = display_field_settings.split(",")
         return {'input_channel': Model224InputChannel(int(separated_settings[0])),
                 'display_units': Model224DisplayFieldUnits(int(separated_settings[1]))}
 
     def configure_display(self, display_mode, number_of_fields=0):
         """Configures the display of the instrument.
 
             Args:
                 display_mode (Model224DisplayMode):
-                    * Defines what mode to set the display in.
-                    * Mode either defines which input to display, or sets up a custom display using display fields.
-
+                    Defines what mode to set the display in.
+                    Mode either defines which input to display, or sets up a custom display using display fields.
                 number_of_fields (Model224NumberOfFields):
-                    * Defines the number of display locations to display.
-                    * Only valid if mode is set to CUSTOM
+                    Defines the number of display locations to display.
+                    Only valid if mode is set to CUSTOM.
 
         """
         self.command(f"DISPLAY {display_mode},{number_of_fields}")
 
     def get_display_configuration(self):
-        """Returns the mode of the display. If display mode is Custom, this method also returns the number of
-        display fields in the custom display.
+        """Returns the mode of the display.
+
+            If display mode is Custom, this method also returns the number of display fields in the custom display.
 
             Returns:
                 (dict):
-                    {display_mode: Model224DisplayMode, number_of_fields: Model224NumberOfFields}
+                    {"display_mode": Model224DisplayMode, "number_of_fields": Model224NumberOfFields}.
 
         """
         display_settings_string = self.query("DISPLAY?")
         separated_settings = display_settings_string.split(",")
         display_mode = int(separated_settings[0])
         if display_mode != 4:
             return_dictionary = {'display_mode': Model224DisplayMode(display_mode),
@@ -1360,93 +1294,77 @@
         return return_dictionary
 
     def turn_relay_on(self, relay_number):
         """Turns the specified relay on.
 
             Args:
                 relay_number (int):
-                    * The relay to turn on.
-                    * Options are:
-                        * 1 or 2
+                    The relay to turn on. Options are: 1 or 2.
 
         """
         self.command(f"RELAY {relay_number},1,0,0")
 
     def turn_relay_off(self, relay_number):
         """Turns the specified relay off.
 
             Args:
                 relay_number (int):
-                    * The relay to turn off.
-                    * Options are:
-                        * 1 or 2
+                    The relay to turn off. Options are: 1 or 2.
 
         """
         self.command(f"RELAY {relay_number},0,0,0")
 
     def set_relay_alarms(self, relay_number, activating_input_channel, alarm_relay_trigger_type):
         """Sets a relay to turn on and off automatically based on the state of the alarm of the specified input channel.
 
             Args:
                 relay_number (int):
-                    * The relay to configure.
-                    * Options are:
-                        * 1 or 2
-
+                    The relay to configure. Options are: 1 or 2.
                 activating_input_channel (str):
-                    * Specifies which input alarm activates the relay when the relay is in alarm mode
-                    * Only applies if ALARM mode is chosen.
-                    * Options are:
-                        * A
-                        * B
-                        * C(1 - 5)
-                        * D(1 - 5)
-
+                    Specifies which input alarm activates the relay when the relay is in alarm mode.
+                    Only applies if ALARM mode is chosen. Options are: A, B, C(1 - 5), D(1 - 5).
                 alarm_relay_trigger_type (Model224RelayControlAlarm):
-                    * Specifies the type of alarm that triggers the relay
-                    * Only applies if ALARM mode is chosen.
+                    Specifies the type of alarm that triggers the relay.
+                    Only applies if ALARM mode is chosen.
 
         """
         self.command(f"RELAY {relay_number},2,{activating_input_channel},{alarm_relay_trigger_type}")
 
     def get_relay_alarm_control_parameters(self, relay_number):
-        """Returns the relay alarm configuration for either of the two configurable relays. Relay must be
-        configured for alarm mode to retrieve parameters.
+        """Returns the relay alarm configuration for either of the two configurable relays.
+
+            Relay must be configured for alarm mode to retrieve parameters.
 
             Args:
-                relay_number (int)
-                    * Specifies which relay to query
-                    * Options are:
-                        * 1 or 2
+                relay_number (int):
+                    Specifies which relay to query. Options are: 1 or 2.
 
             Return:
                 (dict):
-                    {activating_input_channel: str, alarm_relay_trigger_type: Model224RelayControlAlarm}
+                    {"activating_input_channel": str, "alarm_relay_trigger_type": Model224RelayControlAlarm}.
 
         """
 
         relay_config = self.query(f"RELAY? {relay_number}").split(",")
         activating_input_channel = relay_config[1]
         alarm_relay_trigger_type = Model224RelayControlAlarm(int(relay_config[2]))
         return {'activating_input_channel': activating_input_channel,
                 'alarm_relay_trigger_type': alarm_relay_trigger_type}
 
     def get_relay_control_mode(self, relay_number):
         """Returns the configured mode of the specified relay.
 
             Args:
                 relay_number (int):
-                    * Specifies which relay to query
-                    * Options are:
-                        * 1 or 2
+                    Specifies which relay to query. Options are: 1 or 2.
 
             Returns:
                 (Model224RelayControlMode):
-                    * The configured mode of the relay, represented as an object of the enum type
-                        Model224RelayControlMode
+                    The configured mode of the relay, represented as an object of the enum type
+                    Model224RelayControlMode.
 
         """
         relay_settings = self.query("RELAY? " + str(relay_number))
         split_relay_settings = relay_settings.split(",")
         return Model224RelayControlMode(int(split_relay_settings[0]))
 
     def _get_identity(self):
```

### Comparing `lakeshore-1.6.1/lakeshore/model_240.py` & `lakeshore-1.7.0/lakeshore/model_240.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,93 +1,89 @@
 # -*- coding: utf-8 -*-
-"""Implements functionality unique to the Lake Shore Model 240 channel modules"""
+"""Implements functionality unique to the Lake Shore Model 240 channel modules."""
 from enum import IntEnum
 import serial
 
 from .generic_instrument import GenericInstrument
 
 
 class Model240Units(IntEnum):
-    """Enumerations that specify temperature units"""
+    """Enumerations that specify temperature units."""
     KELVIN = 1
     CELSIUS = 2
     SENSOR = 3
     FAHRENHEIT = 4
 
 
 class Model240CurveFormat(IntEnum):
-    """Enumerations that specify temperature sensor curve format units"""
+    """Enumerations that specify temperature sensor curve format units."""
     VOLTS_PER_KELVIN = 2
     OHMS_PER_KELVIN = 3
     LOG_OHMS_PER_KELVIN = 4
 
 
 class Model240Coefficients(IntEnum):
-    """Enumerations that specify a positive or negative coefficient"""
+    """Enumerations that specify a positive or negative coefficient."""
     NEGATIVE = 1
     POSITIVE = 2
 
 
 class Model240SensorTypes(IntEnum):
-    """Enumerations specify types of temperature sensors"""
+    """Enumerations specify types of temperature sensors."""
     DIODE = 1
     PLATINUM_RTD = 2
     NTC_RTD = 3
 
 
 class Model240BrightnessLevel(IntEnum):
-    """Enumerations for the screen brightness levels"""
+    """Enumerations for the screen brightness levels."""
     OFF = 0
     LOW = 25
     MED_LOW = 50
     MED_HIGH = 75
     HIGH = 100
 
 
 class Model240TemperatureCoefficient(IntEnum):
-    """Enumerations specify positive/negative temperature sensor curve coefficients"""
+    """Enumerations specify positive/negative temperature sensor curve coefficients."""
     NEGATIVE = 1
     POSITIVE = 2
 
 
 class Model240InputRange(IntEnum):
-    """Enumerations to specify the input range when autorange is off"""
+    """Enumerations to specify the input range when auto-range is off."""
     RANGE_DIODE = 0
     RANGE_PTRTD_1_KIL_OHMS = 0
     RANGE_NTCRTD_10_OHMS = 0
     RANGE_NTCRTD_30_OHMS = 1
     RANGE_NTCRTD_100_OHMS = 2
     RANGE_NTCRTD_1_KIL_OHMS = 4
     RANGE_NTCRTD_3_KIL_OHMS = 5
     RANGE_NTCRTD_10_KIL_OHMS = 6
     RANGE_NTCRTD_30_KIL_OHMS = 7
     RANGE_NTCRTD_100_KIL_OHMS = 8
 
 
 class Model240CurveHeader:
-    """A class that configures the user curve header and corresponding parameters"""
+    """A class that configures the user curve header and corresponding parameters."""
 
     def __init__(self, curve_name, serial_number, curve_data_format, temperature_limit, coefficient):
-        """Constructor for CurveHeader class
+        """Constructor for CurveHeader class.
 
             Args:
                 curve_name (str):
-                    * Specifies curve name (limit of 15 characters)
-
+                    Specifies curve name (limit of 15 characters).
                 serial_number (str):
-                    * Specifies curve serial number (limit of 10 characters)
-
+                    Specifies curve serial number (limit of 10 characters).
                 curve_data_format (Model240CurveFormat):
-                    * Specifies the curve data format
-
+                    Specifies the curve data format.
                 temperature_limit (float):
-                    * Specifies the curve temperature limit in Kelvin
-
+                    Specifies the curve temperature limit in Kelvin.
                 coefficient (Model240TemperatureCoefficient):
-                    * Specifies the curve temperature coefficient
+                    Specifies the curve temperature coefficient.
 
         """
 
         self.curve_name = curve_name
         self.serial_number = serial_number
         self.curve_data_format = curve_data_format
         self.temperature_limit = temperature_limit
@@ -97,37 +93,30 @@
 class Model240InputParameter:
     """Class used to retrieve and set an input channel's parameters and initial settings."""
 
     def __init__(self, sensor, auto_range_enable, current_reversal_enable, units, input_enable, input_range=None):
         """The constructor for InputParameter class.
 
             Args:
-
                 sensor (Model240SensorTypes):
-                    * Specifies the type of sensor configured at the input
-                    * Member of the Model240SensorTypes IntEnum class
-
+                    Specifies the type of sensor configured at the input.
+                    Member of the Model240SensorTypes IntEnum class.
                 auto_range_enable (bool):
-                    Specifies if autoranging is enabled
-
+                    Specifies if auto-ranging is enabled.
                 current_reversal_enable (bool):
-                    * Specifies channel current reversal
-                    * Current reversal is used to remove thermal EMF errors on resistive sensors.
-                    * Always False if channel is a diode
-                    * False = OFF, True = ON
-
+                    Specifies channel current reversal.
+                    Current reversal is used to remove thermal EMF errors on resistive sensors.
+                    Always False if channel is a diode (False = OFF, True = ON).
                 units (Model240Units):
-                    * Member of the Model240Units IntEnum class
-                    * Specifies the preferred units parameter.
-
+                    Member of the Model240Units IntEnum class.
+                    Specifies the preferred units parameter.
                 input_enable (bool):
-                    Specifies whether the channel is disabled or enabled
-
+                    Specifies whether the channel is disabled or enabled.
                 input_range (Model240InputRange):
-                    Specifies channel range when autorange is off
+                    Specifies channel range when auto-range is off.
 
         """
 
         self.sensor_type = sensor
         self.temperature_unit = units
         self.auto_range_enable = auto_range_enable
         self.current_reversal_enable = current_reversal_enable
@@ -139,28 +128,27 @@
     """Class used to configure and retrieve data for given PROFIBUS slot."""
 
     def __init__(self, channel, temp_unit):
         """The constructor for Model240ProfiSlot class.
 
             Args:
                 channel (int):
-                    Specifies which slot to configure (1-8)
-
+                    Specifies which slot to configure (1-8).
                 temp_unit (Model240Units):
-                    * Member of Model240Units IntEnum class
-                    * Specifies the units to use for the data in this slot
+                    Member of Model240Units IntEnum class.
+                    Specifies the units to use for the data in this slot.
 
         """
 
         self.slot_channel = channel
         self.slot_units = temp_unit
 
 
 class Model240(GenericInstrument):
-    """A class object representing the Lake Shore Model 240 channel modules"""
+    """A class object representing the Lake Shore Model 240 channel modules."""
 
     vid_pid = [(0x1FB9, 0x0205)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  timeout=2.0,
@@ -170,243 +158,234 @@
                                    False, timeout, None, None, **kwargs)
 
     def get_identification(self):
         """Returns instrument's identification parameters.
 
             Returns:
                 id (list):
-                    List defining instrument's manufacturer, model, instrument serial, firmware version
+                    List defining instrument's manufacturer, model, instrument serial, firmware version.
 
         """
         id_parameter = self.query("*IDN?").split(",")
         id_list = {'manufacturer': id_parameter[0],
                    'model': id_parameter[1],
                    'serial number': id_parameter[2],
                    'firmware version': id_parameter[3]}
 
         return id_list
 
     def set_brightness(self, brightness_level):
-        """Sets the brightness for the front panel display
+        """Sets the brightness for the front panel display.
 
             Args:
                 brightness_level (Model240BrightnessLevel):
-                    * Display brightness in percent
+                    Display brightness in percent.
 
         """
         self.command(f"BRIGT {brightness_level}")
 
     def get_brightness(self):
-        """Returns the brightness level of front panel display
+        """Returns the brightness level of front panel display.
 
             Return:
                 brightness_level (Model240BrightnessLevel):
-                    * Display brightness in percent
+                    Display brightness in percent.
 
         """
         brightness_level = Model240BrightnessLevel(int(self.query("BRIGT?")))
         return brightness_level
 
     def get_celsius_reading(self, channel):
         """Returns the temperature value in Celsius of channel selected.
 
             Args:
                 channel (int):
-                    Specifies channel (1-8)
+                    Specifies channel (1-8).
 
         """
         return self.query(f"CRDG? {channel}")
 
     def set_factory_defaults(self):
-        """Sets all configuration values to factory defaults and resets the instrument"""
+        """Sets all configuration values to factory defaults and resets the instrument."""
         self.command("DFLT 99")
 
     def get_kelvin_reading(self, channel):
         """Returns the temperature value in Kelvin of channel selected.
 
             Args:
                 channel (int):
-                    Specifies channel (1-8)
+                    Specifies channel (1-8).
 
         """
         return float(self.query(f"KRDG? {channel}"))
 
     def get_fahrenheit_reading(self, channel):
-        """Returns the temperature value in Farenheit of channel selected
+        """Returns the temperature value in Farenheit of channel selected.
 
             Args:
                 channel (int):
-                    Specifies channel (1-8)
+                    Specifies channel (1-8).
 
         """
         return self.query(f"FRDG? {channel}")
 
     def get_sensor_reading(self, input_channel):
         """Returns the sensor reading in the sensor's units.
 
             Returns:
                 reading (float):
-                    * The raw sensor reading in the units of the connected sensor
+                    The raw sensor reading in the units of the connected sensor.
 
         """
         return float(self.query(f"SRDG? {input_channel}"))
 
     def delete_curve(self, curve):
-        """Deletes the user curve
+        """Deletes the user curve.
 
             Args:
                 curve (int):
-                    * Specifies a user curve to delete
+                    Specifies a user curve to delete.
 
         """
         self.command(f"CRVDEL {curve}")
 
     def set_curve_header(self, input_channel, curve_header):
-        """Configures the user curve header
+        """Configures the user curve header.
 
             Args:
                 input_channel (int):
-                    * Specifies which input_channel curve to configure
-                    * 1 - 8
-
+                    Specifies which input_channel curve to configure (1 - 8).
                 curve_header (CurveHeader):
-                    * A CurveHeader class object containing the desired curve information
+                    A CurveHeader class object containing the desired curve information.
 
         """
         command_string = (f"CRVHDR {input_channel},{curve_header.curve_name},{curve_header.serial_number}," +
                             f"{curve_header.curve_data_format},{curve_header.temperature_limit},{curve_header.coefficient}")
         self.command(command_string)
 
     def get_curve_header(self, curve):
-        """Returns parameters set on a particular user curve header
+        """Returns parameters set on a particular user curve header.
 
             Args:
                 curve:
-                    * Specifies a curve to retrieve
+                    Specifies a curve to retrieve.
 
             Returns:
                 header (CurveHeader):
-                    * A CurveHeader class object containing the desired curve information
+                    A CurveHeader class object containing the desired curve information.
 
         """
         response = self.query(f"CRVHDR? {curve}")
         curve_header = response.split(",")
         header = Model240CurveHeader(str(curve_header[0]),
                                      str(curve_header[1]),
                                      Model240CurveFormat(int(curve_header[2])),
                                      float(curve_header[3]),
                                      Model240TemperatureCoefficient(int(curve_header[4])))
         return header
 
     def set_curve_data_point(self, channel, index, units, temp):
-        """Configures a user curve point
+        """Configures a user curve point.
 
             Args:
                 channel (int):
-                    Specifies which channel curve to configure (1-8)
-
+                    Specifies which channel curve to configure (1-8).
                 index (int):
-                    Specifies the points index in the curve (1-200)
-
+                    Specifies the points index in the curve (1-200).
                 units (float):
-                    Specifies sensor units for this point to 6 digits
-
+                    Specifies sensor units for this point to 6 digits.
                 temp (float):
-                    Specifies the corresponding temperature in Kelvin for this point to 6 digits
+                    Specifies the corresponding temperature in Kelvin for this point to 6 digits.
 
         """
         self.command(f"CRVPT {channel},{index},{units},{temp}")
 
     def get_curve_data_point(self, channel, index):
-        """Returns a standard or user curve data point
+        """Returns a standard or user curve data point.
 
             Args:
                 channel (int):
-                    Specifies channel (1-8)
-
+                    Specifies channel (1-8).
                 index (int):
-                    Specifies the points index in the curve (1–200)
+                    Specifies the points index in the curve (1–200).
 
         """
         return self.query(f"CRVPT? {channel},{index}")
 
     def set_filter(self, channel, length):
-        """Sets the channel filter parameter
+        """Sets the channel filter parameter.
 
             Args:
                 channel (int):
-                    Specifies which channel to configure (1-8)
-
+                    Specifies which channel to configure (1-8).
                 length (int):
-                    Specifies the number of 1 ms points to average for each update (1-100)
+                    Specifies the number of 1 ms points to average for each update (1-100).
 
         """
         self.command(f"FILTER {channel},{length}")
 
     def get_filter(self, channel):
-        """Returns the filter parameter
+        """Returns the filter parameter.
 
             Args:
                 channel (int):
-                    Specifies channel (1-8)
+                    Specifies channel (1-8).
 
         """
         return self.query(f"FILTER? {channel}")
 
     def set_sensor_name(self, channel, name):
         """Names the sensor channel in specified channel.
 
             Args:
                 channel (int):
-                    Specifies which channel to configure (1-8)
-
+                    Specifies which channel to configure (1-8).
                 name (str):
-                    Specifies the name to associate with the sensor channel
+                    Specifies the name to associate with the sensor channel.
 
         """
         self.command(f"INNAME {channel},{name}")
 
     def get_sensor_name(self, channel):
         """Returns the sensor channel's name.
 
             Args:
                 channel (int):
-                    Specifies channel (1-8)
+                    Specifies channel (1-8).
 
         """
         return str(self.query(f"INNAME? {channel}"))
 
     def set_input_parameter(self, channel, input_parameter):
         """Sets channel type parameters.
 
             Args:
                 channel (int):
-                    Specifies which channel to configure (1-8)
-
+                    Specifies which channel to configure (1-8).
                 input_parameter (InputParameter):
-                    See InputParameter class
+                    See InputParameter class.
 
         """
         if input_parameter.auto_range_enable is None:
             input_range = 0
         else:
             input_range = input_parameter.input_range
 
         command_string = (f"INTYPE {channel},{input_parameter.sensor_type.value},{int(input_parameter.auto_range_enable)}," +
                             f"{input_range},{int(input_parameter.current_reversal_enable)},{input_parameter.temperature_unit.value}," +
                             f"{int(input_parameter.input_enable)}")
 
         self.command(command_string)
 
     def get_input_parameter(self, channel):
-        """Returns channel type parameter details
+        """Returns channel type parameter details.
 
             Args:
                 channel (int):
-                    Specifies channel (1-8)
+                    Specifies channel (1-8).
 
         """
         response = self.query(f"INTYPE? {channel}")
         data = response.split(",")
         input_parameter = Model240InputParameter(Model240SensorTypes(int(data[0])),
                                                  bool(data[1]),
                                                  bool(data[3]),
@@ -416,117 +395,121 @@
         return input_parameter
 
     def set_modname(self, name):
         """Names module.
 
             Args:
                 name (str):
-                    Specifies the name or description to help identify the module
+                    Specifies the name or description to help identify the module.
 
         """
         self.command(f"MODNAME {name}")
 
     def get_modname(self):
-        """Returns module name
+        """Returns module name.
 
             Returns:
                 modname (str):
-                    Specifies name of module
+                    Specifies name of module.
 
         """
         return self.query("MODNAME?")
 
     def set_profibus_slot_count(self, count):
-        """Configures the number of PROFIBUS slots for the instrument to present to the bus as a modular station
+        """Configures the number of PROFIBUS slots for the instrument to present to the bus as a modular station.
 
             Args:
                 count (int):
-                    Specifies the number of PROFIBUS slots (1-8)
+                    Specifies the number of PROFIBUS slots (1-8).
 
         """
         self.command(f"PROFINUM {count}")
 
     def get_profibus_slot_count(self):
-        """Returns the number of PROFIBUS slots for the instrument present to the bus as a modular station
+        """Returns the number of PROFIBUS slots for the instrument present to the bus as a modular station.
 
             Returns:
                 slot_count (str):
-                    Specifies PROFIBUS slot count
+                    Specifies PROFIBUS slot count.
 
         """
         return self.query("PROFINUM?")
 
     def set_profibus_address(self, address):
-        """Configures the PROFIBUS address for the module. An address of 126 indicates that it is not configured and it
-        then can be set by a PROFIBUS master.
+        """Configures the PROFIBUS address for the module.
+
+            An address of 126 indicates that it is not configured, and it then can be set by a PROFIBUS master.
 
             Args:
                 address (str):
-                    Specifies the PROFIBUS address (1-126)
+                    Specifies the PROFIBUS address (1-126).
 
         """
         self.command(f"ADDR {address}")
 
     def get_profibus_address(self):
         """Returns the PROFIBUS address for the module.
 
             Returns:
                 address (str):
-                    Specifies PROFIBUS address of module
+                    Specifies PROFIBUS address of module.
 
         """
         return int(self.query("ADDR?"))
 
     def set_profibus_slot_configuration(self, slot, profislot_config):
-        """Configures what data to present on the given PROFIBUS slot. Note that the correct
-            number of slots must be configured with the PROFINUM command, or the slot may be ignored.
+        """Configures what data to present on the given PROFIBUS slot.
+
+            Note that the correct number of slots must be configured with the PROFINUM command, or the slot may be
+            ignored.
 
             Args:
                 slot (int):
-                    Specifies the slot to be configured
-
+                    Specifies the slot to be configured.
                 profislot_config (Model240ProfiSlot):
-                    A Model240ProfiSlot class object containing the desired PROFIBUS slot configuration information
+                    A Model240ProfiSlot class object containing the desired PROFIBUS slot configuration information.
 
         """
         self.command(f"PROFISLOT {slot},{profislot_config.slot_channel},{profislot_config.slot_units}")
 
     def get_profibus_slot_configuration(self, slot_num):
         """Returns the slot configuration of the slot number.
 
             Returns:
                 slot_config (Model240ProfiSlot):
-                    See Model240ProfiSlot class
+                    See Model240ProfiSlot class.
 
         """
         response = self.query(f"PROFISLOT? {slot_num}").split(",")
         slot_configuration = Model240ProfiSlot(int(response[0]), Model240Units(int(response[1])))
         return slot_configuration
 
     def get_profibus_connection_status(self):
         """Returns the connection status of PROFIBUS.
 
             Returns:
                 status (str):
-                    Specifies connection status of PROFIBUS
+                    Specifies connection status of PROFIBUS.
 
         """
         return self.query("PROFISTAT?")
 
     def get_channel_reading_status(self, channel):
-        """The integer returned represents the sum of the bit weighting of the channel status flag
-            bits. A “000” response indicates a valid reading is present.
+        """Returns the current status indicator of the specified channel
+
+            The integer returned represents the sum of the bit weighting of the channel status flag bits. A “000”
+            response indicates a valid reading is present.
 
             Args:
                 channel (int):
-                    Specifies which channel to query (1-8)
+                    Specifies which channel to query (1-8).
 
             Returns:
                 bit_status (dict):
-                    Dictionary containing the current status indicator
+                    Dictionary containing the current status indicator.
 
         """
         bit_status = {}
         bit_names = ["invalid reading",
                      "",
                      "",
                      "",
@@ -541,19 +524,19 @@
         for count, bit_name in enumerate(bit_names):
             mask = 0b1 << count
             bit_status[bit_name] = bool(mask & status_indicator)
 
         return bit_status
 
     def get_sensor_units_channel_reading(self, channel):
-        """Returns the sensor units value of channel being queried
+        """Returns the sensor units value of channel being queried.
 
             Args:
                 channel (int):
-                    Specifies which channel to query (1-8)
+                    Specifies which channel to query (1-8).
 
         """
         return self.query(f"SRDG? {channel}")
 
 
 __all__ = ['Model240', 'Model240Units', 'Model240CurveFormat', 'Model240Coefficients', 'Model240SensorTypes',
            'Model240BrightnessLevel', 'Model240TemperatureCoefficient', 'Model240InputRange', 'Model240CurveHeader',
```

### Comparing `lakeshore-1.6.1/lakeshore/model_335.py` & `lakeshore-1.7.0/lakeshore/model_335.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Implements functionality unique to the Lake Shore Model 335 cryogenic temperature controller"""
+"""Implements functionality unique to the Lake Shore Model 335 cryogenic temperature controller."""
 from enum import IntEnum
 
 from .temperature_controllers import TemperatureController, InstrumentException
 from .temperature_controllers import RelayControlMode, RelayControlAlarm, InterfaceMode, HeaterError, \
     CurveFormat, CurveTemperatureCoefficient, BrightnessLevel, AutotuneMode, HeaterResistance, Polarity, \
     DiodeCurrent, HeaterOutputUnits, InputSensorUnits, ControlTypes, StandardEventRegister, OperationEvent, RegisterBase
 
@@ -22,224 +22,203 @@
 Model335ControlTypes = ControlTypes
 
 Model335StandardEventRegister = StandardEventRegister
 Model335OperationEvent = OperationEvent
 
 
 class Model335InputSensor(IntEnum):
-    """Enumeration when "NONE" is an option for sensor input"""
+    """Enumeration when "NONE" is an option for sensor input."""
     NONE = 0
     CHANNEL_A = 1
     CHANNEL_B = 2
 
 
 class Model335MonitorOutUnits(IntEnum):
-    """Units associated with a sensor channel"""
+    """Units associated with a sensor channel."""
     KELVIN = 1
     CELSIUS = 2
     SENSOR = 3
 
 
 class Model335InputSensorType(IntEnum):
-    """Sensor type enumeration"""
+    """Sensor type enumeration."""
     DISABLED = 0
     DIODE = 1
     PLATINUM_RTD = 2
     NTC_RTD = 3
     THERMOCOUPLE = 4
 
 
 class Model335DiodeRange(IntEnum):
-    """Diode voltage range enumeration"""
+    """Diode voltage range enumeration."""
     TWO_POINT_FIVE_VOLTS = 0
     TEN_VOLTS = 1
 
 
 class Model335RTDRange(IntEnum):
-    """RTD resistance range enumeration"""
+    """RTD resistance range enumeration."""
     TEN_OHM = 0
     THIRTY_OHM = 1
     HUNDRED_OHM = 2
     THREE_HUNDRED_OHM = 3
     ONE_THOUSAND_OHM = 4
     THREE_THOUSAND_OHM = 5
     TEN_THOUSAND_OHM = 6
     THIRTY_THOUSAND_OHM = 7
     ONE_HUNDRED_THOUSAND_OHM = 8
 
 
 class Model335ThermocoupleRange(IntEnum):
-    """Thermocouple range enumeration"""
+    """Thermocouple range enumeration."""
     FIFTY_MILLIVOLT = 0
 
 
 class Model335InputSensorSettings:
-    """Class object used in the get/set_input_sensor methods"""
+    """Class object used in the get/set_input_sensor methods."""
 
     def __init__(self, sensor_type, autorange_enable, compensation, units, input_range=None):
-        """Constructor for the InputSensor class
+        """Constructor for the InputSensor class.
 
             Args:
                 sensor_type (Model335InputSensorType):
-                    * Specifies input sensor type
-
+                    Specifies input sensor type.
                 autorange_enable (bool):
-                    * Specifies autoranging
-                    * False = off and True = on
-
+                    Specifies autoranging (False = off, True = on).
                 compensation (bool):
-                    * Specifies input compensation
-                    * False = off and True = on
-
+                    Specifies input compensation. (False = off, True = on).
                 units (Model335InputSensorUnits):
-                    * Specifies the preferred units parameter for sensor readings and for the control setpoint
-
+                    Specifies the preferred units parameter for sensor readings and for the control set-point.
                 input_range (IntEnum)
-                    * Specifies input range if autorange_enable is false
-                    * See IntEnum classes:
-                        * Model335DiodeRange
-                        * Model335RTDRange
-                        * Model335ThermocoupleRange
+                    Specifies input range if autorange_enable is false.
+                    See IntEnum classes: Model335DiodeRange, Model335RTDRange, and Model335ThermocoupleRange.
 
         """
 
         self.sensor_type = sensor_type
         self.autorange_enable = autorange_enable
         self.compensation = compensation
         self.units = units
         self.input_range = input_range
 
 
 class Model335HeaterOutType(IntEnum):
-    """Heater output 2 enumeration"""
+    """Heater output 2 enumeration."""
     CURRENT = 0
     VOLTAGE = 1
 
 
 class Model335HeaterOutputDisplay(IntEnum):
-    """Heater output display units enumeration"""
+    """Heater output display units enumeration."""
     CURRENT = 1
     POWER = 2
 
 
 class Model335HeaterOutputMode(IntEnum):
-    """Control loop enumeration"""
+    """Control loop enumeration."""
     OFF = 0
     CLOSED_LOOP = 1
     ZONE = 2
     OPEN_LOOP = 3
     MONITOR_OUT = 4
     WARMUP_SUPPLY = 5
 
 
 class Model335WarmupControl(IntEnum):
-    """Heater output 2 voltage mode warmup enumerations"""
+    """Heater output 2 voltage mode warmup enumerations."""
     AUTO_OFF = 0
     CONTINUOUS = 1
 
 
 class Model335HeaterRange(IntEnum):
-    """Control loop heater range enumeration"""
+    """Control loop heater range enumeration."""
     OFF = 0
     LOW = 1
     MEDIUM = 2
     HIGH = 3
 
 
 class Model335ControlLoopZoneSettings:
-    """Control loop configuration for a particular heater output and zone"""
+    """Control loop configuration for a particular heater output and zone."""
 
     def __init__(self, upper_bound, proportional, integral, derivative, manual_output_value,
                  heater_range, channel, ramp_rate):
-        """Constructor
+        """Constructor.
 
             Args:
                 upper_bound (float):
-                    * Specifies the upper Setpoint boundary of this zone in kelvin
-
+                    Specifies the upper set-point boundary of this zone in kelvin.
                 proportional (float):
-                    * Specifies the proportional gain for this zone
-                    * 0.1 to 1000
-
+                    Specifies the proportional gain for this zone (0.1 to 1000).
                 integral (float):
-                    * Specifies the integral gain for this zone
-                    * 0.1 to 1000
-
+                    Specifies the integral gain for this zone (0.1 to 1000).
                 derivative (float):
-                    * Specifies the derivative gain for this zone
-                    * 0 to 200 %
-
+                    Specifies the derivative gain for this zone (0 to 200 %).
                 manual_output_value (float):
-                    * Specifies the manual output for this zone
-                    * 0 to 100 %
-
+                    Specifies the manual output for this zone (0 to 100 %).
                 heater_range (Model335HeaterRange):
-                    * Specifies the heater range for this zone
-                    * See Model335HeaterRange IntEnum class
-
+                    Specifies the heater range for this zone.
+                    See Model335HeaterRange IntEnum class.
                 channel (Model335InputSensor):
-                    * See Model335InputSensor IntEnum class
-
+                    See Model335InputSensor IntEnum class.
                 ramp_rate (float):
-                    * Specifies the ramp rate for this zone
-                    * 0 - 100 K/min
+                    Specifies the ramp rate for this zone (0 - 100 K/min).
 
         """
 
         self.upper_bound = upper_bound
         self.proportional = proportional
         self.integral = integral
         self.derivative = derivative
         self.manual_output_value = manual_output_value
         self.heater_range = heater_range
         self.channel = channel
         self.ramp_rate = ramp_rate
 
 
 class Model335DisplaySetup(IntEnum):
-    """Panel display setup enumeration"""
+    """Panel display setup enumeration."""
     INPUT_A = 0
     INPUT_A_MAX_MIN = 1
     TWO_INPUT_A = 2
     INPUT_B = 3
     INPUT_B_MAX_MIN = 4
     TWO_INPUT_B = 5
     CUSTOM = 6
     TWO_LOOP = 7
 
 
 class Model335HeaterVoltageRange(IntEnum):
-    """Voltage mode heater enumerations"""
+    """Voltage mode heater enumerations."""
     VOLTAGE_OFF = 0
     VOLTAGE_ON = 1
 
 
 class Model335DisplayInputChannel(IntEnum):
-    """Panel display information enumeration"""
+    """Panel display information enumeration."""
     NONE = 0
     INPUT_A = 1
     INPUT_B = 2
     SETPOINT_1 = 3
     SETPOINT_2 = 4
     OUTPUT_1 = 5
     OUTPUT_2 = 6
 
 
 class Model335DisplayFieldUnits(IntEnum):
-    """Panel display units enumeration"""
+    """Panel display units enumeration."""
     KELVIN = 1
     CELSIUS = 2
     SENSOR_UNITS = 3
     MINIMUM_DATA = 4
     MAXIMUM_DATA = 5
     SENSOR_NAME = 6
 
 
 class Model335StatusByteRegister(RegisterBase):
-    """Class object representing the status byte register LSB to MSB"""
+    """Class object representing the status byte register LSB to MSB."""
 
     bit_names = [
         "",
         "",
         "",
         "",
         "message_available_summary_bit",
@@ -256,15 +235,15 @@
         self.message_available_summary_bit = message_available_summary_bit
         self.event_status_summary_bit = event_status_summary_bit
         self.service_request = service_request
         self.operation_summary_bit = operation_summary_bit
 
 
 class Model335ServiceRequestEnable(RegisterBase):
-    """Class object representing the service request enable register LSB to MSB"""
+    """Class object representing the service request enable register LSB to MSB."""
 
     bit_names = [
         "",
         "",
         "",
         "",
         "message_available_summary_bit",
@@ -279,15 +258,15 @@
                  operation_summary_bit):
         self.message_available_summary_bit = message_available_summary_bit
         self.event_status_summary_bit = event_status_summary_bit
         self.operation_summary_bit = operation_summary_bit
 
 
 class Model335InputReadingStatus(RegisterBase):
-    """Class object representing the input status flag bits"""
+    """Class object representing the input status flag bits."""
 
     bit_names = [
         "invalid_reading",
         "",
         "",
         "",
         "temp_underrange",
@@ -301,15 +280,15 @@
         self.temp_underrange = temp_underrange
         self.temp_overrange = temp_overrange
         self.sensor_units_zero = sensor_units_zero
         self.sensor_units_overrange = sensor_units_overrange
 
 
 class Model335(TemperatureController):
-    """A class object representing the Lake Shore Model 335 cryogenic temperature controller"""
+    """A class object representing the Lake Shore Model 335 cryogenic temperature controller."""
 
     # Initiate enum types for temperature controllers
     _input_channel_enum = Model335DisplayInputChannel
     _display_units_enum = Model335DisplayFieldUnits
 
     # Initiate instrument specific registers
     _status_byte_register = Model335StatusByteRegister
@@ -353,141 +332,128 @@
 
     def set_monitor_output_heater(self, channel, high_value, low_value, units=Model335MonitorOutUnits.KELVIN,
                                   polarity=Model335Polarity.UNIPOLAR):
         """Configures output 2. Use the set_heater_output_mode command to set the output mode to Monitor Out.
 
             Args:
                 channel (Model335InputSensor):
-                    * Specifies which sensor input to monitor
-
+                    Specifies which sensor input to monitor.
                 high_value (float):
-                    * Represents the data at which the Monitor Out reaches +100% output
-                    * Entered in the units designated by the <units> argument
-
+                    Represents the data at which the Monitor Out reaches +100% output.
+                    Entered in the units designated by the <units> argument.
                 low_value (float):
-                    * Represents the data at which the analog output reaches -100% output if bipolar,
-                    * or 0% outputif unipolar. Entered in the units designated by the <units> argument
-
+                    Represents the data at which the analog output reaches -100% output if bipolar,
+                    or 0% output if unipolar. Entered in the units designated by the <units> argument.
                 units (Model335MonitorOutUnits):
-                    * Specifies the units on which to base the output voltage
-
+                    Specifies the units on which to base the output voltage.
                 polarity (Model335Polarity):
-                    * Specifies output voltage is unipolar or bipolar
+                    Specifies output voltage is unipolar or bipolar.
 
         """
         self.command(f"ANALOG 2,{channel},{units},{high_value},{low_value},{polarity}")
 
     def get_monitor_output_heater(self):
         """Used to obtain all monitor out parameters for output 2.
 
-            Return:
+            Returns:
                 (dict):
-                    * See set_monitor_output_heater method arguments
-                    * Keys:
-                        * "channel": Model335InputSensor
-                        * "units": Model335MonitorOutUnits
-                        * "high_value": float
-                        * "low_value": float
-                        * "polarity": Model335Polarity
+                    {"channel": Model335InputSensor,
+                    "units": Model335MonitorOutUnits,
+                    "high_value": float,
+                    "low_value": float,
+                    "polarity": Model335Polarity}
+
+                    See set_monitor_output_heater method arguments
 
         """
         parameters = self.query("ANALOG? 2").split(",")
         return {"channel": Model335InputSensor(int(parameters[0])),
                 "units": Model335MonitorOutUnits(int(parameters[1])),
                 "high_value": float(parameters[2]),
                 "low_value": float(parameters[3]),
                 "polarity": Model335Polarity(int(parameters[4]))}
 
     def get_celsius_reading(self, channel):
-        """Returns the temperature value in celsius of either channel.
+        """Returns the temperature value in Celsius of either channel.
 
             Args:
                 channel (str):
-                    * Selects the sensor input to query
-                    * "A" or "B"
+                    Selects the sensor input to query ("A" or "B"),
 
         """
         return float(self.query(f"CRDG? {channel}"))
 
     def set_display_setup(self, mode):
-        """Sets the display mode
+        """Sets the display mode.
 
             Args:
                 mode (Model335DisplaySetup):
-                    * Specifies the front panel display mode
-                    * See Model335DisplaySetup IntEnum class
+                    Specifies the front panel display mode.
+                    See Model335DisplaySetup IntEnum class.
 
         """
         self.command(f"DISPLAY {mode}")
 
     def get_display_setup(self):
-        """Returns the display mode
+        """Returns the display mode.
 
             Return:
                 (Model335DisplaySetup):
-                    * Specifies the front panel display mode
-                    * See Model335DisplaySetup IntEnum class
+                    Specifies the front panel display mode.
+                    See Model335DisplaySetup IntEnum class.
 
         """
         return Model335DisplaySetup(int(self.query("DISPLAY?")))
 
     def set_heater_setup_one(self, heater_resistance, max_current, output_display_mode):
         """Method to configure heater output one.
 
             Args:
                 heater_resistance (Model335HeaterResistance):
-                    * See Model335HeaterResistance IntEnum class
-
+                    See Model335HeaterResistance IntEnum class.
                 max_current (float):
-                    * Specifies the maximum current for the heater
-
+                    Specifies the maximum current for the heater.
                 output_display_mode (Model335HeaterOutputDisplay):
-                    * Specifies how the heater output is displayed
-                    * See Model335HeaterOutType IntEnum class
+                    Specifies how the heater output is displayed.
+                    See Model335HeaterOutType IntEnum class.
 
         """
         self.command(f"HTRSET 1,0,{heater_resistance},0,{max_current},{output_display_mode}")
 
     def set_heater_setup_two(self, output_type, heater_resistance, max_current, display_mode):
         """Method to configure the heater output 2.
 
             Args:
                 output_type (Model335HeaterOutType):
-                    * Specifies wheter the heater output is in constant current or voltage mode
-                    * See Model335HeaterOutType IntEnum class
-
+                    Specifies whether the heater output is in constant current or voltage mode.
+                    See Model335HeaterOutType IntEnum class.
                 heater_resistance (Model335HeaterResistance):
-                    * See Model335HeaterResistance IntEnum class
-
+                    See Model335HeaterResistance IntEnum class.
                 max_current (float):
-                    * Specifies the maximum current for the heater
-
+                    Specifies the maximum current for the heater.
                 display_mode (Model335HeaterOutType):
-                    * Specifies how the heater output is displayed
-                    * Required only if output_type is set to CURRENT
-                    * See Model335HeaterOutType IntEnum class
+                    Specifies how the heater output is displayed.
+                    Required only if output_type is set to CURRENT.
+                    See Model335HeaterOutType IntEnum class.
 
         """
         self.command(f"HTRSET 2,{output_type},{heater_resistance},0,{max_current},{display_mode}")
 
     def get_heater_setup(self, heater_output):
         """Returns the heater configuration status.
 
             Args:
-                heater_output (int)
-                    * Selects which heater output to query
+                heater_output (int):
+                    Selects which heater output to query:
 
             Return:
                 (dict):
-                    * See set_heater_setup_one/set_heater_setup_two method arguments
-                    * Keys:
-                        * "output_type": Model335HeaterOutType
-                        * "heater_resistance": Model335HeaterResistance
-                        * "max_current": float
-                        * "output_display_mode": Model335HeaterOutputDisplay
+                    See set_heater_setup_one/set_heater_setup_two method arguments.
+                    {"output_type": Model335HeaterOutType, "heater_resistance": Model335HeaterResistance,
+                    "max_current": float, "output_display_mode": Model335HeaterOutputDisplay}
 
         """
         heater_setup = self.query(f"HTRSET? {heater_output}").split(",")
         if int(heater_setup[2]) == 0:
             max_current = float(heater_setup[3])
         else:
             preset_currents = ["USER", 0.707, 1.0, 1.141, 1.732]
@@ -500,19 +466,17 @@
                 "output_display_mode": Model335HeaterOutputDisplay(int(heater_setup[4]))}
 
     def set_input_sensor(self, channel, sensor_parameters):
         """Sets the sensor type and associated parameters.
 
             Args:
                 channel (str):
-                    * Specifies input to configure
-                    * "A" or "B"
-
+                    Specifies input to configure ("A" or "B").
                 sensor_parameters (Model335InputSensorSettings):
-                    * See Model335InputSensorSettings class
+                    See Model335InputSensorSettings class.
 
         """
         autorange_enable = bool(int(sensor_parameters.autorange_enable))
         if autorange_enable:
             input_range = 0
         else:
             input_range = sensor_parameters.input_range
@@ -523,20 +487,19 @@
         self.command(command_string)
 
     def get_input_sensor(self, channel):
         """Returns the sensor type and associated parameters.
 
             Args:
                 channel (str):
-                    * Specifies sensor input to configure
-                    * "A" or "B"
+                    Specifies sensor input to configure ("A" or "B").
 
             Return:
                 (Model335InputSensorSettings):
-                    * See Model335InputSensor IntEnum class
+                    See Model335InputSensor IntEnum class.
 
         """
         sensor_configuration = self.query(f"INTYPE? {channel}").split(",")
         input_sensor_type = Model335InputSensorType(int(sensor_configuration[0]))
 
         sensor_range = None
         if bool(int(sensor_configuration[1])):
@@ -566,103 +529,95 @@
         return [float(self.query("KRDG? A")), float(self.query("KRDG? B"))]
 
     def set_heater_output_mode(self, output, mode, channel, powerup_enable=False):
         """Configures the heater output mode.
 
             Args:
                 output (int):
-                    * Specifies which output to configure (1 or 2)
-
+                    Specifies which output to configure (1 or 2).
                 mode (Model335HeaterOutputMode):
-                    * Member of Model335HeaterOutputMode IntEnum class
-                    * Specifies the control mode
-
-                channel (Model335InputSensor)
-                    * Specifies which input to use for control
-
-                powerup_enable (bool)
-                    * Specifies whether the output remains on (True)
-                    * or shuts off after power cycle (False)
+                    Member of Model335HeaterOutputMode IntEnum class.
+                    Specifies the control mode.
+                channel (Model335InputSensor):
+                    Specifies which input to use for control.
+                powerup_enable (bool):
+                    Specifies whether the output remains on (True)
+                    or shuts off after power cycle (False).
 
         """
         command_string = f"OUTMODE {output},{mode},{channel},{int(powerup_enable)}"
         self.command(command_string)
 
     def get_heater_output_mode(self, output):
         """Returns the heater output mode for a given output and whether powerup is enabled.
 
             Args:
                 output (int):
-                    * Specifies which output to query (1 or 2)
+                    Specifies which output to query (1 or 2).
 
             Return:
                 (dict):
-                    * Keys:
-                        * "mode": Model335HeaterOutputMode
-                        * "channel": Model335InputSensor
-                        * "powerup_enable": bool
+                {"mode": Model335HeaterOutputMode, "channel": Model335InputSensor, "powerup_enable": bool}
 
         """
         outmode = self.query(f"OUTMODE? {output}").split(",")
 
         return {"mode": Model335HeaterOutputMode(int(outmode[0])),
                 "channel": Model335InputSensor(int(outmode[1])),
                 "powerup_enable": bool(int(outmode[2]))}
 
     def set_output_two_polarity(self, output_polarity):
-        """Sets polarity of output 2 to either unipolar or bipolar, only applicable when
-        output 2 is in voltage mode.
+        """Sets polarity of output 2 to either unipolar or bipolar.
+
+            Only applicable when output 2 is in voltage mode.
 
             Args:
-                output_polarity (Model335Polarity)
-                    * Specifies whether output voltage is UNIPOLAR or BIPOLAR
+                output_polarity (Model335Polarity):
+                    Specifies whether output voltage is UNIPOLAR or BIPOLAR.
 
         """
         self.command(f"POLARITY 2,{output_polarity}")
 
     def get_output_2_polarity(self):
-        """Returns the polarity of output 2
+        """Returns the polarity of output 2.
 
             Return:
-                (Model335Polarity)
-                    * Specifies whether output is UNIPOLAR or BIPOLAR
+                (Model335Polarity):
+                    Specifies whether output is UNIPOLAR or BIPOLAR.
 
         """
         return Model335Polarity(int(self.query("POLARITY?")))
 
     def set_heater_range(self, output, heater_range):
-        """Sets the heater range for a particular output. The range setting has no effect if an output is in
-        the off mode, and does not apply to an output in Monitor Out mode. An output in Monitor Out mode is always on.
+        """Sets the heater range for a particular output.
+
+            The range setting has no effect if an output is in the off mode, and does not apply to an output in Monitor
+            Out mode. An output in Monitor Out mode is always on.
 
             Args:
                 output (int):
-                    * Specifies which output to configure (1 or 2)
-
+                    Specifies which output to configure (1 or 2).
                 heater_range (IntEnum):
-                    * For Outputs 1 and 2 in Current mode:
-                        * Model335HeaterRange IntEnum member
-                    * For Output 2 in Voltage mode:
-                        * Model335HeaterVoltageRange IntEnum member
+                    For Outputs 1 and 2 in Current mode: Model335HeaterRange IntEnum member.
+                    For Output 2 in Voltage mode: Model335HeaterVoltageRange IntEnum member.
 
         """
         self.command(f"RANGE {output},{heater_range}")
 
     def get_heater_range(self, output):
         """Returns the heater range for a particular output.
 
             Args:
                 output (int):
-                    * Specifies which output to configure (1 or 2)
+                    Specifies which output to configure (1 or 2).
 
             Return:
                 heater_range (IntEnum):
-                    * For Outputs 1 and 2 in Current mode:
-                        * Model335HeaterRange IntEnum member
-                    * For Output 2 in Voltage mode:
-                        * Model335HeaterVoltageRange IntEnum member
+                    For Outputs 1 and 2 in Current mode: Model335HeaterRange IntEnum member.
+                    For Output 2 in Voltage mode: Model335HeaterVoltageRange IntEnum member.
 
         """
         heater_range = int(self.query(f"RANGE? {output}"))
         if output == 2:
             # Check if output 2 is in voltage mode
             output_2_heater_setup = self.query("HTRSET? 2").split(",")
             output_2_voltage_enable = bool(int(output_2_heater_setup[0]))
@@ -671,45 +626,44 @@
             else:
                 heater_range = Model335HeaterRange(heater_range)
         else:
             heater_range = Model335HeaterRange(heater_range)
         return heater_range
 
     def all_heaters_off(self):
-        """Recreates the front panel safety feature of shutting off all heaters"""
+        """Recreates the front panel safety feature of shutting off all heaters."""
 
         self.command("RANGE 1,0")
         self.command("RANGE 2,0")
 
     def get_input_reading_status(self, channel):
         """Returns the state of the input status flag bits.
 
             Args:
                 channel (str):
-                    * Specifies which channel to query
-                    * "A" or "B"
+                    Specifies which channel to query ("A" or "B").
 
             Return:
                 (InputReadingStatus):
-                    * Boolean representation of each bit of the input status flag register
+                    Boolean representation of each bit of the input status flag register.
         """
         response = int(self.query(f"RDGST? {channel}"))
         return Model335InputReadingStatus.from_integer(response)
 
     def set_warmup_supply(self, control, percentage):
-        """Warmup mode applies only to Output 2 in Voltage mode. The Output Type parameter
-        must be configured using the set_heater_setup() method, and the Output mode and Control
-        Input parameters must be configured using the set_monitor_out_parameters() method.
+        """Warmup mode applies only to Output 2 in Voltage mode.
+
+            The Output Type parameter must be configured using the set_heater_setup() method, and the Output mode and
+            Control Input parameters must be configured using the set_monitor_out_parameters() method.
 
             Args:
                 control (Model335WarmupControl):
-                    * Specifies the type of control used
-
+                    Specifies the type of control used.
                 percentage (float):
-                    * Specifies the percentage of full scale (10 V) Monitor Out voltage to apply
+                    Specifies the percentage of full scale (10 V) Monitor Out voltage to apply.
 
         """
         # Check if output 2 is in voltage mode
         output_2_heater_setup = self.query("HTRSET? 2").split(",")
         output_2_voltage_enable = bool(int(output_2_heater_setup[0]))
         if not output_2_voltage_enable:
             raise InstrumentException("Output 2 is not configured in voltage mode")
@@ -718,59 +672,50 @@
         self.command(command_string)
 
     def get_warmup_supply(self):
         """Returns the output 2 warmup supply configuration.
 
             Return:
                 (dict):
-                    * Keys:
-                        * "control": Model335WarmupControl
-                        * "percentage": float
+                    {"control": Model335WarmupControl, "percentage": float}
 
         """
         warmup_supply = self.query("WARMUP? 2").split(",")
         return {"control": Model335WarmupControl(int(warmup_supply[0])),
                 "percentage": float(warmup_supply[1])}
 
     def set_control_loop_zone_table(self, output, zone, control_loop_zone):
         """Configures the output zone parameters.
 
             Args:
                 output (int):
-                    * Specifies which heater output to configure
-                    * 1 or 2
-
+                    Specifies which heater output to configure (1 or 2).
                 zone (int):
-                    * Specifies which zone in the table to configure
-                    * 1 to 10
-
+                    Specifies which zone in the table to configure (1 to 10).
                 control_loop_zone (ControlLoopZone):
-                    * See ControlLoopZone class
+                    See ControlLoopZone class.
 
         """
         command_string = (f"ZONE {output},{zone},{control_loop_zone.upper_bound},{control_loop_zone.proportional}," +
                             f"{control_loop_zone.integral},{control_loop_zone.derivative},{control_loop_zone.manual_output_value}," +
                             f"{control_loop_zone.heater_range},{control_loop_zone.channel},{control_loop_zone.ramp_rate}")
         self.command(command_string)
 
     def get_control_loop_zone_table(self, output, zone):
         """Returns a list of zone control parameters for a selected output and zone.
 
             Args:
                 output (int):
-                    * Specifies which heater output to query
-                    * 1 or 2
-
+                    Specifies which heater output to query (1 or 2).
                 zone (int):
-                    * Specifies which zone in the table to query
-                    * 1 to 10
+                    Specifies which zone in the table to query (1 to 10).
 
             Return:
                 (Model335ControlLoopZone):
-                    * See Model335ControlLoopZone class
+                    See Model335ControlLoopZone class.
 
         """
         zone_parameters = self.query(f"ZONE? {output},{zone}").split(",")
         control_loop_zone_parameters = Model335ControlLoopZoneSettings(float(zone_parameters[0]),
                                                                        float(zone_parameters[1]),
                                                                        float(zone_parameters[2]),
                                                                        float(zone_parameters[3]),
```

### Comparing `lakeshore-1.6.1/lakeshore/model_336.py` & `lakeshore-1.7.0/lakeshore/model_336.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Implements functionality unique to the Lake Shore Model 336 cryogenic temperature controller"""
+"""Implements functionality unique to the Lake Shore Model 336 cryogenic temperature controller."""
 from enum import IntEnum
 
 from .generic_instrument import RegisterBase
 from .temperature_controllers import TemperatureController, InstrumentException
 from .temperature_controllers import RelayControlMode, RelayControlAlarm, InterfaceMode, HeaterError, \
     CurveFormat, CurveTemperatureCoefficient, AutotuneMode, HeaterResistance, Polarity, DiodeCurrent, \
     HeaterOutputUnits, InputSensorUnits, ControlTypes, StandardEventRegister, OperationEvent, \
@@ -28,44 +28,45 @@
 Model336DisplayFields = DisplayFields
 Model336DisplayFieldsSize = DisplayFieldsSize
 Model336StandardEventRegister = StandardEventRegister
 Model336OperationEvent = OperationEvent
 
 
 class Model336InputChannel(IntEnum):
-    """Enumeration where "NONE" is an option for sensor input"""
+    """Enumeration where "NONE" is an option for sensor input."""
     NONE = 0
     CHANNEL_A = 1
     CHANNEL_B = 2
     CHANNEL_C = 3
     CHANNEL_D = 4
     CHANNEL_D2 = 5
     CHANNEL_D3 = 6
     CHANNEL_D4 = 7
     CHANNEL_D5 = 8
 
 
 class Model336DisplaySetupMode(IntEnum):
-    """Front panel display setup enum"""
+    """Front panel display setup enum."""
     INPUT_A = 0
     INPUT_B = 1
     INPUT_C = 2
     INPUT_D = 3
     CUSTOM = 4
     FOUR_LOOP = 5
     ALL_INPUTS = 6
     INPUT_D2 = 7
     INPUT_D3 = 8
     INPUT_D4 = 9
     INPUT_D5 = 10
 
 
 class Model336InputSensorType(IntEnum):
-    """Sensor type enumeration. THERMOCOUPLE is only valid with the 3060 option,
-        CAPACITANCE is only valid with the 3061 option
+    """Sensor type enumeration.
+
+        THERMOCOUPLE is only valid with the 3060 option, CAPACITANCE is only valid with the 3061 option.
     """
     DISABLED = 0
     DIODE = 1
     PLATINUM_RTD = 2
     NTC_RTD = 3
     THERMOCOUPLE = 4
     CAPACITANCE = 5
@@ -74,155 +75,135 @@
 class Model336DiodeRange(IntEnum):
     """Diode voltage range enumeration"""
     TWO_POINT_FIVE_VOLTS = 0
     TEN_VOLTS = 1
 
 
 class Model336RTDRange(IntEnum):
-    """RTD resistance range enumeration. THIRTY_THOUSAND_OHM and
-        ONE_HUNDRED_THOUSAND_OHM are only valid for NTC RTDs
+    """RTD resistance range enumeration.
+
+        THIRTY_THOUSAND_OHM and ONE_HUNDRED_THOUSAND_OHM are only valid for NTC RTDs.
     """
     TEN_OHM = 0
     THIRTY_OHM = 1
     HUNDRED_OHM = 2
     THREE_HUNDRED_OHM = 3
     ONE_THOUSAND_OHM = 4
     THREE_THOUSAND_OHM = 5
     TEN_THOUSAND_OHM = 6
     THIRTY_THOUSAND_OHM = 7
     ONE_HUNDRED_THOUSAND_OHM = 8
 
 
 class Model336ThermocoupleRange(IntEnum):
-    """Thermocouple range enumeration"""
+    """Thermocouple range enumeration."""
     FIFTY_MILLIVOLT = 0
 
 
 class Model336InputSensorSettings:
-    """Class object used in the get/set_input_sensor methods"""
+    """Class object used in the get/set_input_sensor methods."""
 
     def __init__(self, sensor_type, autorange_enable, compensation, units, input_range=None):
-        """Constructor for the InputSensorSettings class
+        """Constructor for the InputSensorSettings class.
 
             Args:
                 sensor_type (Model336InputSensorType):
-                    * Specifies input sensor type
-
+                    Specifies input sensor type
                 autorange_enable (bool):
-                    * Specifies autoranging
-                    * False = off and True = on
-
+                    Specifies auto-ranging (False = off, True = on)
                 compensation (bool):
-                    * Specifies input compensation
-                    * False = off and True = on
-
+                    Specifies input compensation (False = off, True = on)
                 units (Model336InputSensorUnits):
-                    * Specifies the preferred units parameter for sensor readings and for the control setpoint
-
+                    Specifies the preferred units parameter for sensor readings and for the control set-point.
                 input_range (IntEnum)
-                    * Specifies input range if autorange_enable is false
-                    * See IntEnum classes:
-                        * Model336DiodeRange
-                        * Model336RTDRange
-                        * Model336ThermocoupleRange
+                    Specifies input range if autorange_enable is false.
+                    See IntEnum classes: Model336DiodeRange, Model336RTDRange, andModel336ThermocoupleRange.
 
         """
         self.sensor_type = sensor_type
         self.autorange_enable = autorange_enable
         self.compensation = compensation
         self.units = units
         self.input_range = input_range
 
 
 class Model336HeaterOutputMode(IntEnum):
-    """Control loop enumeration"""
+    """Control loop enumeration."""
     OFF = 0
     CLOSED_LOOP = 1
     ZONE = 2
     OPEN_LOOP = 3
     MONITOR_OUT = 4
     WARMUP_SUPPLY = 5
 
 
 class Model336HeaterRange(IntEnum):
-    """Current mode heater enumerations"""
+    """Current mode heater enumerations."""
     OFF = 0
     LOW = 1
     MEDIUM = 2
     HIGH = 3
 
 
 class Model336HeaterVoltageRange(IntEnum):
-    """Voltage mode heater enumerations"""
+    """Voltage mode heater enumerations."""
     VOLTAGE_OFF = 0
     VOLTAGE_ON = 1
 
 
 class Model336DisplayUnits(IntEnum):
-    """Panel display units enumeration"""
+    """Panel display units enumeration."""
     KELVIN = 1
     CELSIUS = 2
     SENSOR_UNITS = 3
     MINIMUM_DATA = 4
     MAXIMUM_DATA = 5
     SENSOR_NAME = 6
 
 
 class Model336ControlLoopZoneSettings:
-    """Control loop configuarion for a particular heater output and zone"""
+    """Control loop configuration for a particular heater output and zone."""
 
     def __init__(self, upper_bound, proportional, integral, derivative, manual_out_value, heater_range, channel, rate):
-        """Constructor
+        """Constructor.
 
             Args:
                 upper_bound (float):
-                    * Specifies the upper Setpoint boundary of this zone in kelvin
-
+                    Specifies the upper set-point boundary of this zone in kelvin.
                 proportional (float):
-                    * Specifies the proportional gain for this zone
-                    * 0.1 to 1000
-
+                    Specifies the proportional gain for this zone (0.1 to 1000).
                 integral (float):
-                    * Specifies the integral gain for this zone
-                    * 0.1 to 1000
-
+                    Specifies the integral gain for this zone (0.1 to 1000).
                 derivative (float):
-                    * Specifies the derivative gain for this zone
-                    * 0 to 200 %
-
+                    Specifies the derivative gain for this zone (0 to 200 %).
                 manual_out_value (float):
-                    * Specifies the manual output for this zone
-                    * 0 to 100 %
-
+                    Specifies the manual output for this zone (0 to 100 %).
                 heater_range (Model336HeaterRange):
-                    * Specifies the heater range for this zone
-                    * See Model336HeaterRange IntEnum class
-
+                    Specifies the heater range for this zone.
+                    See Model336HeaterRange IntEnum class.
                 channel (Model336InputChannel):
-                    * See Model336InputChannel IntEnum class
-                    * Passing the NONE member will use the previously assigned sensor
-
+                    See Model336InputChannel IntEnum class.
+                    Passing the NONE member will use the previously assigned sensor.
                 rate (float):
-                    * Specifies the ramp rate for this zone
-                    * 0 - 100 K/min
+                    Specifies the ramp rate for this zone ( 0 - 100 K/min).
 
         """
 
         self.upper_bound = upper_bound
         self.proportional = proportional
         self.integral = integral
         self.derivative = derivative
         self.manual_out_value = manual_out_value
         self.heater_range = heater_range
         self.channel = channel
         self.rate = rate
 
 
 class Model336StatusByteRegister(RegisterBase):
-    """Class object representing the status byte register LSB to MSB"""
+    """Class object representing the status byte register LSB to MSB."""
 
     bit_names = [
         "",
         "",
         "",
         "",
         "message_available_summary_bit",
@@ -239,15 +220,15 @@
         self.message_available_summary_bit = message_available_summary_bit
         self.event_status_summary_bit = event_status_summary_bit
         self.service_request = service_request
         self.operation_summary_bit = operation_summary_bit
 
 
 class Model336ServiceRequestEnable(RegisterBase):
-    """Class object representing the service request enable register LSB to MSB"""
+    """Class object representing the service request enable register LSB to MSB."""
 
     bit_names = [
         "",
         "",
         "",
         "",
         "message_available_summary_bit",
@@ -262,15 +243,15 @@
                  operation_summary_bit):
         self.message_available_summary_bit = message_available_summary_bit
         self.event_status_summary_bit = event_status_summary_bit
         self.operation_summary_bit = operation_summary_bit
 
 
 class Model336InputReadingStatus(RegisterBase):
-    """Class object representing the input staus flag bits"""
+    """Class object representing the input status flag bits."""
 
     bit_names = [
         "invalid_reading",
         "",
         "",
         "",
         "temp_underrange",
@@ -284,15 +265,15 @@
         self.temp_underrange = temp_underrange
         self.temp_overrange = temp_overrange
         self.sensor_units_zero = sensor_units_zero
         self.sensor_units_overrange = sensor_units_overrange
 
 
 class Model336(TemperatureController):
-    """A class object representing the Lake Shore Model 336 cryogenic temperature controller"""
+    """A class object representing the Lake Shore Model 336 cryogenic temperature controller."""
 
     vid_pid = [(0x1FB9, 0x0301)]
 
     # Initiate enum types for temperature controllers class
     _input_channel_enum = Model336InputChannel
     _display_units_enum = Model336DisplayUnits
 
@@ -336,103 +317,93 @@
     set_interface = TemperatureController._set_interface
     get_interface = TemperatureController._get_interface
     get_tuning_control_status = TemperatureController._get_tuning_control_status
     set_diode_excitation_current = TemperatureController._set_diode_excitation_current
     get_diode_excitation_current = TemperatureController._get_diode_excitation_current
 
     def set_monitor_output_heater(self, output, channel, units, high_value, low_value, polarity):
-        """Configures a voltage-controlled output. Use the set_heater_output_mode
-        command to set the output mode to Monitor Out.
+        """Configures a voltage-controlled output.
+
+            Use the set_heater_output_mode command to set the output mode to Monitor Out.
 
             Args:
                 output (int):
-                    * Voltage-controlled output to configure
-                    * 3 or 4
-
+                    Voltage-controlled output to configure (3 or 4)
                 channel (Model336InputChannel):
-                    * Specifies which sensor input to monitor
-                    * A member of the Model336InputChannel IntEnum class
-
+                    Specifies which sensor input to monitor.
+                    A member of the Model336InputChannel IntEnum class.
                 units (Model336InputSensorUnits):
-                    * Specifies the units on which to base the output voltage
-                    * A member of the Model336InputSensorUnits IntEnum class
-
+                    Specifies the units on which to base the output voltage.
+                    A member of the Model336InputSensorUnits IntEnum class.
                 high_value (float):
-                    * Represents the data at which the Monitor Out reaches +100% output
-                    * Entered in the units designated by the <units> argument
-
+                    Represents the data at which the Monitor Out reaches +100% output.
+                    Entered in the units designated by the <units> argument.
                 low_value (float):
-                    * Represents the data at which the analog output reaches -100% output if bipolar,
-                    * or 0% outputif unipolar. Entered in the units designated by the <units> argument
-
+                    Represents the data at which the analog output reaches -100% output if bipolar,
+                    or 0% output if unipolar. Entered in the units designated by the <units> argument.
                 polarity (Model336Polarity):
-                    * Specifies whether the output voltage is unipolar or bipolar
-                    * Member of the Model336Polarity IntEnum class
+                    Specifies whether the output voltage is unipolar or bipolar.
+                    Member of the Model336Polarity IntEnum class.
 
         """
         command_string = f"ANALOG {output},{channel},{units},{high_value},{low_value},{polarity}"
         self.command(command_string)
 
     def get_monitor_output_heater(self, output):
-        """Used to obtain all monitor out parameters for a specific output
+        """Used to obtain all monitor out parameters for a specific output.
 
             Args:
                 output (int):
-                    * Voltage-controlled output to configure
-                    * 3 or 4
+                    Voltage-controlled output to configure (3 or 4).
 
-            Return:
+            Returns:
                 (dict):
-                    * See set_monitor_output_heater arguments
+                    See set_monitor_output_heater arguments
 
         """
         response = self.query(f"ANALOG? {output}").split(",")
         return {"channel": Model336InputChannel(int(response[0])),
                 "units": Model336InputSensorUnits(int(response[1])),
                 "high_value": float(response[2]),
                 "low_value": float(response[3]),
                 "polarity": Model336Polarity(int(response[4]))}
 
     def set_display_setup(self, mode, num_fields="", displayed_output=""):
-        """Sets the display mode
+        """Sets the display mode.
 
             Args:
                 mode (Model336DisplaySetupMode):
-                    * Member of Model336DisplaySetupMode IntEnum class
-                    * Specifies display mode for default and 3062 options
-
+                    Member of Model336DisplaySetupMode IntEnum class
+                    Specifies display mode for default and 3062 options
                 num_fields (IntEnum)
-                    * When mode is set to custom, specifies the number of fields
-                        * Member of Model336DisplayFields
-                    * When mode is set to all inputs, specifies size of readings
-                        * Member of Model336DisplayFieldsSize
-
+                    When mode is set to custom, specifies the number of fields (Member of Model336DisplayFields).
+                    When mode is set to all inputs, specifies size of readings (Member of Model336DisplayFieldsSize).
                 displayed_output (int):
-                    * Configures the bottom half of the custom display screen
-                    * Only required if mode is set to CUSTOM
-                        * Output: 1 - 4
+                    Configures the bottom half of the custom display screen.
+                    Only required if mode is set to CUSTOM.
+                    Output: (1 - 4)
 
         """
         if mode == Model336DisplaySetupMode.CUSTOM:
             if not isinstance(num_fields, Model336DisplayFields):
                 raise InstrumentException("num_fields argument must be of type \"Model336DisplaySetupCustom\"")
         elif mode == Model336DisplaySetupMode.ALL_INPUTS:
             if not isinstance(num_fields, Model336DisplayFieldsSize):
                 raise InstrumentException("num_fields argument must be of type \"Model336DisplaySetupAllInputs\"")
 
         command_string = f"DISPLAY {mode},{num_fields},{displayed_output}"
         self.command(command_string)
 
     def get_display_setup(self):
-        """Returns the display mode
+        """Returns the display mode.
 
-            Return:
-                (dict)
-                    * See set_display_setup method arguments
-                    * Keys: "mode", "num_fields", "displayed_output"
+            Returns:
+                (dict):
+                    See set_display_setup method arguments.
+                    Keys: "mode", "num_fields", "displayed_output"
 
         """
         display_setup_response = self.query("DISPLAY?").split(",")
         mode = Model336DisplaySetupMode(int(display_setup_response[0]))
         if mode == Model336DisplaySetupMode.CUSTOM:
             num_fields = Model336DisplayFields(int(display_setup_response[1]))
             displayed_output = int(display_setup_response[2])
@@ -444,49 +415,41 @@
             displayed_output = None
 
         return {"mode": mode,
                 "num_fields": num_fields,
                 "displayed_output": displayed_output}
 
     def set_heater_setup(self, output, heater_resistance, max_current, heater_output):
-        """Method to configure the heaters
+        """Method to configure the heaters.
 
             Args:
                 output (int):
-                    * Specifies which heater output to configure
-                    * 1 or 2
-
+                    Specifies which heater output to configure (1 or 2).
                 heater_resistance (Model336HeaterResistance):
-                    * Member of Model336HeaterResistance IntEnum class
-
+                    Member of Model336HeaterResistance IntEnum class.
                 max_current (float):
-                    * User defined maximum output current (see table 4-11 for max current and resistance relationships)
-
+                    User defined maximum output current (see table 4-11 for max current and resistance relationships).
                 heater_output (Model336HeaterOutputUnits):
-                    * Specifies whether the heater output displays in current or power
-                    * Member of Model336HeaterOutputUnits IntEnum class
+                    Specifies whether the heater output displays in current or power.
+                    Member of Model336HeaterOutputUnits IntEnum class.
 
         """
         self.command(f"HTRSET {output},{heater_resistance},0,{max_current},{heater_output}")
 
     def get_heater_setup(self, heater_output):
         """Returns the heater configuration status.
 
             Args:
                 heater_output (int):
-                    * Specifies which heater output to configure
-                    * 1 or 2
+                    Specifies which heater output to configure (1 or 2)
 
-            Return:
+            Returns:
                 (dict):
-                    * See set_heater_setup arguments
-                    * Keys:
-                        * heater_resistance
-                        * max_current
-                        * output_display_mode
+                    See set_heater_setup arguments
+                    Keys: heater_resistance, max_current, output_display_mode.
 
         """
         heater_setup = self.query(f"HTRSET? {heater_output}").split(",")
         if int(heater_setup[1]) == 0:
             max_current = float(heater_setup[2])
         else:
             preset_currents = ["USER", 0.707, 1.0, 1.141, 2.0]
@@ -498,21 +461,18 @@
                 "output_display_mode": Model336HeaterOutputUnits(int(heater_setup[3]))}
 
     def set_input_sensor(self, channel, sensor_parameters):
         """Sets the sensor type and associated parameters.
 
             Args:
                 channel (str):
-                    * Specifies input to configure
-                        * "A" - "D"
-                    * 3062 option:
-                        * "D1" - "D5"
-
+                    Specifies input to configure ("A" - "D"):
+                    3062 option ("D1" - "D5")
                 sensor_parameters (Model336InputSensorSettings):
-                    * See Model336InputSensorSettings class
+                    See Model336InputSensorSettings class.
 
         """
         autorange_enable = sensor_parameters.autorange_enable
         if autorange_enable:
             input_range = 0
         else:
             input_range = sensor_parameters.input_range
@@ -522,20 +482,19 @@
         self.command(command_string)
 
     def get_input_sensor(self, channel):
         """Returns the sensor type and associated parameters.
 
             Args:
                 channel (str):
-                    * Specifies sensor input to configure
-                    * "A" or "B"
+                    Specifies sensor input to configure ("A" or "B")
 
-            Return:
+            Returns:
                 (Model336InputSensorSettings):
-                    * See Model336InputSensorSettings class
+                    See Model336InputSensorSettings class.
 
         """
         sensor_config = self.query(f"INTYPE? {channel}").split(",")
         sensor_type = Model336InputSensorType(int(sensor_config[0]))
         autorange_enable = bool(int(sensor_config[1]))
         if autorange_enable:
             input_range = 0
@@ -554,233 +513,209 @@
                                            bool(int(sensor_config[3])),
                                            Model336InputSensorUnits(int(sensor_config[4])),
                                            input_range)
 
     def get_all_kelvin_reading(self):
         """Returns the temperature value in kelvin of all channels.
 
-            Return:
-                (list: float)
-                    * [channel_A, channel_B, channel_C, channel_D]
+            Returns:
+                (list: float):
+                    [channel_A, channel_B, channel_C, channel_D]
 
         """
         kelvin_reading = self.query("KRDG? 0").split(",")
         return [float(channel) for channel in kelvin_reading]
 
     def set_heater_output_mode(self, output, mode, channel, powerup_enable=False):
         """Configures the heater output mode.
 
             Args:
                 output (int):
-                    * Specifies which output to configure
-                    * 1 - 4
-
+                    Specifies which output to configure (1 - 4)
                 mode (Model336HeaterOutputMode):
-                    * Member of Model336HeaterOutputMode IntEnum class
-                    * Specifies the control mode
-
+                    Member of Model336HeaterOutputMode IntEnum class.
+                    Specifies the control mode.
                 channel (Model336InputChannel):
-                    * Model336InputChannel IntEnum class
-                    * Specifies which input to use for control
-
-                powerup_enable (bool)
-                    * Specifies whether the output remains on (True)
-                    * or shuts off after power cycle (False)
+                    Model336InputChannel IntEnum class.
+                    Specifies which input to use for control.
+                powerup_enable (bool):
+                    Specifies whether the output remains on (True)
+                    or shuts off after power cycle (False).
 
         """
         command_string = f"OUTMODE {output},{mode},{channel},{int(powerup_enable)}"
         self.command(command_string)
 
     def get_heater_output_mode(self, output):
         """Returns the heater output mode for a given output and whether powerup is enabled.
 
             Args:
                 output (int):
-                    * Specifies which output to retrieve
-                    * 1 - 4
+                    Specifies which output to retrieve (1 - 4).
 
-            Return:
+            Returns:
                 (dict):
-                    * See set_heater_output_mode method arguments
-                    * Keys:
-                        * mode
-                        * channel
-                        * powerup_enable
+                    See set_heater_output_mode method arguments.
+                    Keys: mode, channel, powerup_enable.
 
         """
         outmode = self.query(f"OUTMODE? {output}").split(",")
         return {"mode": Model336HeaterOutputMode(int(outmode[0])),
                 "channel": Model336InputChannel(int(outmode[1])),
                 "powerup_enable": bool(int(outmode[2]))}
 
     def set_heater_range(self, output, heater_range):
         """Sets the heater range for a particular output.
-        The range setting has no effect if an output is in
-        the Off mode, and does not apply to an output in Monitor
-        Out mode. An output in Monitor Out mode is always on.
+
+            The range setting has no effect if an output is in
+            the Off mode, and does not apply to an output in Monitor
+            Out mode. An output in Monitor Out mode is always on.
 
             Args:
                 output (int):
-                    * Specifies which output to configure
-                    * 1 - 4
-
+                    Specifies which output to configure (1 - 4).
                 heater_range (IntEnum):
-                    * For Outputs 1 and 2:
-                        * Member of Model336HeaterRange IntEnum class
-                    * For Outputs 3 and 4:
-                        * Model336HeaterVoltageRange IntEnum class
+                    For Outputs 1 and 2: Member of Model336HeaterRange IntEnum class.
+                    For Outputs 3 and 4: Model336HeaterVoltageRange IntEnum class.
 
         """
         self.command(f"RANGE {output},{heater_range}")
 
     def get_heater_range(self, output):
         """Returns the heater range for a particular output.
 
             Args:
                 output (int):
-                    * Specifies which output to query (1 or 2)
+                    Specifies which output to query (1 or 2).
 
-            Return:
+            Returns:
                 (IntEnum):
-                    * For Outputs 1 and 2:
-                        * Member of Model336HeaterRange IntEnum class
-                    * For Outputs 3 and 4:
-                        * Member of Model336HeaterVoltageRange IntEnum class
+                    For Outputs 1 and 2: Member of Model336HeaterRange IntEnum class.
+                    For Outputs 3 and 4: Member of Model336HeaterVoltageRange IntEnum class.
 
         """
         heater_range = int(self.query(f"RANGE? {output}"))
 
         if output in (3, 4):
             heater_range = Model336HeaterVoltageRange(heater_range)
         else:
             heater_range = Model336HeaterRange(heater_range)
 
         return heater_range
 
     def all_heaters_off(self):
-        """Recreates the front panel safety feature of shutting off all heaters"""
+        """Recreates the front panel safety feature of shutting off all heaters."""
         self.command("RANGE 1,0;RANGE 2,0;RANGE 3,0;RANGE 4,0")
 
     def get_input_reading_status(self, channel):
-        """Retruns the state of the input status flag bits.
+        """Reruns the state of the input status flag bits.
 
             Args:
                 channel (str):
-                    * Specifies which channel to query
-                    * "A" - "D"
-                    * "D1" - "D5" for 3062 option
+                    Specifies which channel to query ("A" - "D").
+                    Use "D1" - "D5" for 3062 option.
 
-            Return:
+            Returns:
                 (Model336InputReadingStatus):
-                    * Boolean representation of each bit in the input status flag register
+                    Boolean representation of each bit in the input status flag register.
 
         """
         response = int(self.query(f"RDGST? {channel}"))
         return Model336InputReadingStatus.from_integer(response)
 
     def get_all_sensor_reading(self):
-        """Returns the sensor unit reading of all channels
+        """Returns the sensor unit reading of all channels.
 
-            Return:
+            Returns:
                 (list: float):
-                    * [channel_A, channel_B, channel_C, channel_D]
+                    [channel_A, channel_B, channel_C, channel_D]
 
         """
         sensor_reading = self.query("SRDG? 0").split(",")
         return [float(channel) for channel in sensor_reading]
 
     def set_warmup_supply_parameter(self, output, control, percentage):
-        """Warmup mode applies only to voltage heater outputs 3 and 4. The Output mode and Control
-            Input parameters must be configured using the set_monitor_out_parameters() method.
+        """Warmup mode applies only to voltage heater outputs 3 and 4.
+
+            The Output mode and Control Input parameters must be configured using the set_monitor_out_parameters()
+            method.
 
             Args:
                 output (int):
-                    * Specifies which output to configure
-                    * 3 or 4
-
+                    Specifies which output to configure (3 or 4).
                 control (Model336ControlTypes):
-                    * Member of the Model336ControlTypes IntEnum class
-
+                    Member of the Model336ControlTypes IntEnum class.
                 percentage (float):
-                    * Specifies the percentage of full scale (10 V) Monitor Out
-                    * voltage to apply to turn on the external power supply
-                        * A value of 50.5 translates to a 50.5 percent output voltage
+                    Specifies the percentage of full scale (10 V) Monitor Out voltage to apply to turn on the external
+                    power supply. (A value of 50.5 translates to a 50.5 percent output voltage).
 
         """
         command_string = f"WARMUP {output},{control},{percentage}"
         self.command(command_string)
 
     def get_warmup_supply_parameter(self, output):
         """Returns the warmup supply configuration for a particular output.
 
             Args:
                 output (int):
-                    * Specifies which analog voltage heater output to retrieve
-                    * 3 or 4
+                    Specifies which analog voltage heater output to retrieve (3 or 4).
 
-            Return:
+            Returns:
                 (dict):
-                    * See set_warmup_supply_parameter method arguments
+                    See set_warmup_supply_parameter method arguments
 
         """
         warmup_supply = self.query(f"WARMUP? {output}").split(",")
         return {"control": Model336ControlTypes(int(warmup_supply[0])),
                 "percentage": float(warmup_supply[1])}
 
     def set_control_loop_zone_table(self, output, zone, control_loop_zone):
         """Configures the output zone parameters.
 
             Args:
                 output (int):
-                    * Specifies which analog voltage heater output to configure
-                    * 1 or 2
-
+                    Specifies which analog voltage heater output to configure (1 or 2).
                 zone (int):
-                    * Specifies which zone in the table to configure
-                    * 1 to 10
-
+                    Specifies which zone in the table to configure (1 to 10).
                 control_loop_zone (Model336ControlLoopZoneSettings):
-                    * See Model336ControlLoopZoneSettings class
+                    See Model336ControlLoopZoneSettings class.
 
         """
         command_string = (f"ZONE {output},{zone},{control_loop_zone.upper_bound},{control_loop_zone.proportional}," +
                             f"{control_loop_zone.integral},{control_loop_zone.derivative}," +
                             f"{control_loop_zone.manual_out_value},{control_loop_zone.heater_range}," +
                             f"{control_loop_zone.channel},{control_loop_zone.rate}")
         self.command(command_string)
 
     def get_control_loop_zone_table(self, output, zone):
         """Returns a list of zone control parameters for a selected output and zone.
 
             Args:
                 output (int):
-                    * Specifies which heater output to query
-                    * 1 or 2
-
+                    Specifies which heater output to query (1 or 2).
                 zone (int):
-                    * Specifies which zone in the table to query
-                    * 1 to 10
+                    Specifies which zone in the table to query (1 to 10).
 
-            Return:
+            Returns:
                 (Model336ControlLoopZoneSettings):
-                    * See Model336ControlLoopZoneSettings class
+                    See Model336ControlLoopZoneSettings class.
 
         """
         zone_parameters = self.query(f"ZONE? {output},{zone}").split(",")
         return Model336ControlLoopZoneSettings(float(zone_parameters[0]),
                                                float(zone_parameters[1]),
                                                float(zone_parameters[2]),
                                                float(zone_parameters[3]),
                                                float(zone_parameters[4]),
                                                Model336HeaterRange(int(zone_parameters[5])),
                                                Model336InputChannel(int(zone_parameters[6])),
                                                float(zone_parameters[7]))
 
     def _autotune_error(self):
-        """Method to raise an excecption if autotune error has occured"""
+        """Method to raise an exception if autotune error has occurred."""
 
         tuning_status = self.query("TUNEST?").split(",")
 
         if bool(int(tuning_status[2])):
             raise InstrumentException("An autotune error is present")
```

### Comparing `lakeshore-1.6.1/lakeshore/model_350.py` & `lakeshore-1.7.0/lakeshore/model_648.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Implements functionality unique to the Lake Shore Model 350 cryogenic temperature controller"""
+"""Implements functionality unique to the Lake Shore Model 648 electromagnet power supply."""
 import serial
 
 from .generic_instrument import GenericInstrument
 
 
-class Model350(GenericInstrument):
-    """A class object representing the Lake Shore Model 350 cryogenic temperature controller"""
+class Model648(GenericInstrument):
+    """A class object representing the Lake Shore Model 648 electromagnet power supply."""
 
-    vid_pid = [(0x1FB9, 0x0302)]
+    vid_pid = [(0x1FB9, 0x0602)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=57600,
                  data_bits=7,
                  stop_bits=1,
```

### Comparing `lakeshore-1.6.1/lakeshore/model_372.py` & `lakeshore-1.7.0/lakeshore/model_372.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Implements functionality unique to the Lake Shore Model 372 AC bridge and temperature controller"""
+"""Implements functionality unique to the Lake Shore Model 372 AC bridge and temperature controller."""
 from enum import Enum, IntEnum
 
 from .temperature_controllers import TemperatureController, CurveTemperatureCoefficient, InterfaceMode, \
     BrightnessLevel, HeaterError, CurveHeader, StandardEventRegister, DisplayFields, Polarity, HeaterOutputUnits, \
     HeaterResistance, Interface, OperationEvent
 from .generic_instrument import RegisterBase
 
@@ -18,25 +18,27 @@
 Model372CurveHeader = CurveHeader
 Model372OperationEventRegister = OperationEvent
 Model372StandardEventRegister = StandardEventRegister
 
 
 class Model372OutputMode(IntEnum):
     """Enumeration of the different modes for heater output setup."""
+
     OFF = 0
     MONITOR_OUT = 1
     OPEN_LOOP = 2
     ZONE = 3
     STILL = 4
     CLOSED_LOOP = 5
     WARMUP = 6
 
 
 class Model372InputChannel(Enum):
-    """Enumeration of the input channels of the Model 372"""
+    """Enumeration of the input channels of the Model 372."""
+
     NONE = 0
     ONE = 1
     TWO = 2
     THREE = 3
     FOUR = 4
     FIVE = 5
     SIX = 6
@@ -51,77 +53,88 @@
     FIFTEEN = 15
     SIXTEEN = 16
     CONTROL = "A"
 
 
 class Model372SensorExcitationMode(IntEnum):
     """Enumeration of the possible excitation modes for an input sensor."""
+
     VOLTAGE = 0
     CURRENT = 1
 
 
 class Model372AutoRangeMode(IntEnum):
-    """Enumeration for the possible modes of the auto ranging feature. ROX102B mode is a special autoranging mode
-    that applies only to Lake Shore ROX-102B sensor."""
+    """Enumeration for the possible modes of the auto ranging feature.
+
+        ROX102B mode is a special auto-ranging mode that applies only to Lake Shore ROX-102B sensor.
+    """
+
     OFF = 0
     CURRENT = 1
     ROX102B = 2
 
 
 class Model372InputSensorUnits(IntEnum):
     """Enumeration of the units to handle input readings and display in."""
+
     KELVIN = 1
     OHMS = 2
 
 
 class Model372MonitorOutputSource(IntEnum):
     """Enumeration of the source for an output to monitor."""
+
     OFF = 0
     CS_NEG = 1
     CS_POS = 2
     VCM_NEG = 3
     VCM_POS = 4
     VDIF = 5
     VAD_MEASUREMENT = 6
     VAD_CONTROL = 7
 
 
 class Model372RelayControlMode(IntEnum):
-    """Enumeration of the control modes of the configurable relays of the 372"""
+    """Enumeration of the control modes of the configurable relays of the 372."""
+
     RELAY_OFF = 0
     RELAY_ON = 1
     ALARMS = 2
     SAMPLE_HEATER_ZONE = 3
     WARMUP_HEATER_ZONE = 4
 
 
 class Model372DisplayMode(IntEnum):
-    """Enumeration of the possible information to display"""
+    """Enumeration of the possible information to display."""
+
     MEASUREMENT_INPUT = 0
     CONTROL_INPUT = 1
     CUSTOM = 2
 
 
 class Model372DisplayInfo(IntEnum):
-    """Enumeration of the information to a display in the bottom left of the custom display mode"""
+    """Enumeration of the information to a display in the bottom left of the custom display mode."""
+
     NONE = 0
     SAMPLE_HEATER = 1
     WARMUP_HEATER = 2
     ACTIVE_SCAN_CHANNEL = 3
 
 
 class Model372CurveFormat(IntEnum):
-    """Enumeration of the units to use in a calibration curve"""
+    """Enumeration of the units to use in a calibration curve."""
+
     OHM_PER_KELVIN = 3
     LOGOHM_PER_KELVIN = 4
     OHM_PER_KELVIN_CUBIC_SPLINE = 7
 
 
 class Model372DisplayFieldUnits(IntEnum):
     """Enumeration for the possible units to display in a single display field."""
+
     KELVIN = 1
     OHMS = 2
     QUADRATURE = 3
     MINIMUM_DATA = 4
     MAXIMUM_DATA = 5
     SENSOR_NAME = 6
 
@@ -137,23 +150,25 @@
     RANGE_10_MILLI_AMPS = 6
     RANGE_31_POINT_6_MILLI_AMPS = 7
     RANGE_100_MILLI_AMPS = 8
 
 
 class Model372InputFrequency(IntEnum):
     """Defines the enumeration of the excitation frequency of an input."""
+
     FREQUENCY_9_POINT_8_HZ = 1
     FREQUENCY_13_POINT_7_HZ = 2
     FREQUENCY_16_POINT_2_HZ = 3
     FREQUENCY_11_POINT_6_HZ = 4
     FREQUENCY_18_POINT_2_HZ = 5
 
 
 class Model372MeasurementInputVoltageRange(IntEnum):
     """Enumerates the possible voltage ranges for a measurement input."""
+
     RANGE_2_MICRO_VOLTS = 1
     RANGE_6_POINT_32_MICRO_VOLTS = 2
     RANGE_20_MICRO_VOLTS = 3
     RANGE_63_POINT_2_MICRO_VOLTS = 4
     RANGE_200_MICRO_VOLTS = 5
     RANGE_632_MICRO_VOLTS = 6
     RANGE_2_MILLI_VOLTS = 7
@@ -162,14 +177,15 @@
     RANGE_63_POINT_2_MILLI_VOLTS = 10
     RANGE_200_MILLI_VOLTS = 11
     RANGE_632_MILLI_VOLTS = 12
 
 
 class Model372MeasurementInputCurrentRange(IntEnum):
     """Enumeration of the current range of a measurement input."""
+
     RANGE_1_PICO_AMP = 1
     RANGE_3_POINT_16_PICO_AMPS = 2
     RANGE_10_PICO_AMPS = 3
     RANGE_31_POINT_6_PICO_AMPS = 4
     RANGE_100_PICO_AMPS = 5
     RANGE_316_PICO_AMPS = 6
     RANGE_1_NANO_AMP = 7
@@ -188,24 +204,26 @@
     RANGE_3_POINT_16_MILLI_AMPS = 20
     RANGE_10_MILLI_AMPS = 21
     RANGE_31_POINT_6_MILLI_AMPS = 22
 
 
 class Model372ControlInputCurrentRange(IntEnum):
     """Enumeration of the current range of the control input. """
+
     RANGE_316_PICO_AMPS = 1
     RANGE_1_NANO_AMP = 2
     RANGE_3_POINT_16_NANO_AMPS = 3
     RANGE_10_NANO_AMPS = 4
     RANGE_31_POINT_6_NANO_AMPS = 5
     RANGE_100_NANO_AMPS = 6
 
 
 class Model372MeasurementInputResistance(IntEnum):
     """Enumeration of the resistance range of a measurement input."""
+
     RANGE_2_MILLI_OHMS = 1
     RANGE_6_POINT_32_MILLI_OHMS = 2
     RANGE_20_MILLI_OHMS = 3
     RANGE_63_POINT_2_MILLI_OHMS = 4
     RANGE_200_MILLI_OHMS = 5
     RANGE_632_MILLI_OHMS = 6
     RANGE_2_OHMS = 7
@@ -223,88 +241,80 @@
     RANGE_2_MEGA_OHMS = 19
     RANGE_6_POINT_32_MEGA_OHMS = 20
     RANGE_20_MEGA_OHMS = 21
     RANGE_63_POINT_2_MEGA_OHMS = 22
 
 
 class Model372HeaterOutput(IntEnum):
-    """Enumeration of model372 heater output"""
+    """Enumeration of model372 heater output."""
+
     WARM_UP_HEATER = 1
     STILL_HEATER = 2
 
 
 class Model372InputChannelSettings:
-    """Class object representing parameters for the channel settings of an Model372InputChannel"""
+    """Class object representing parameters for the channel settings of an Model372InputChannel."""
 
     def __init__(self,
                  enable,
                  dwell_time,
                  pause_time,
                  curve_number,
                  temperature_coefficient=None):
         """The constructor for Model372InputChannelSettings class.
 
             Args:
                 enable (bool):
-                    * Whether to enable or disable input
-
-                dwell_time (int)
-                    * Specifies a value for the autoscanning dwell time in seconds. Not applicable to control input.
-                    * Options are: 1 to 200 s
-
-                pause_time (int)
-                    * Specifies a value for the change pause time in seconds.
-                    * Options are: 3 to 200 s
-
+                    Whether to enable or disable input.
+                dwell_time (int):
+                    Specifies a value for the auto-scanning dwell time in seconds. Not applicable to control input.
+                    Options are: 1 to 200 s.
+                pause_time (int):
+                    Specifies a value for the change pause time in seconds. Options are:
+                    3 to 200 s.
                 curve_number (int):
-                    * Specifies which calibration curve to use on input sensor.
-                    * Options are: 0 (none), 1 - 59
-
-                temperature_coefficient (Model372CurveTemperatureCoefficient)
-                    * Sets coefficient for temperature control if no curve is selected.
+                    Specifies which calibration curve to use on input sensor. Options are:
+                    0 (none), or 1 - 59.
+                temperature_coefficient (Model372CurveTemperatureCoefficient):
+                    Sets coefficient for temperature control if no curve is selected.
 
         """
         self.enable = enable
         self.dwell_time = dwell_time
         self.pause_time = pause_time
         self.curve_number = curve_number
         self.temperature_coefficient = temperature_coefficient
 
 
 class Model372InputSetupSettings:
-    """Class object representing parameters for the sensor and measurement settings of an Model372InputChannel"""
+    """Class object representing parameters for the sensor and measurement settings of an Model372InputChannel."""
 
     def __init__(self,
                  mode,
                  excitation_range,
                  auto_range,
                  current_source_shunted,
                  units,
                  resistance_range=None):
         """The constructor for Model372InputSetupSettings class.
 
             Args:
                 mode (Model372SensorExcitationMode):
-                    * Determines whether to use current or voltage for sensor excitation.
-
-                excitation_range (IntEnum)
-                    * the voltage or current (depending on mode) excitation range.
-
-                auto_range (Model372AutoRangeMode)
-                    * Specifies whether auto range is Off, Autoranging Current, or in ROX 102B mode.
-
+                    Determines whether to use current or voltage for sensor excitation.
+                excitation_range (IntEnum):
+                    The voltage or current (depending on mode) excitation range.
+                auto_range (Model372AutoRangeMode):
+                    Specifies whether auto range is Off, Auto-ranging Current, or in ROX 102B mode.
                 current_source_shunted (bool):
-                    * Specifies whether or not the current source is shunted. If current source is shunted,
-                        excitation is off. If current source is not shunted, excitation is on.
-
-                units (Model372InputSensorUnits)
-                    * Specifies the preferred units, Kelvin or Ohms, for the sensor.
-
+                    Specifies whether the current source is shunted. If current source is shunted,
+                    excitation is off. If current source is not shunted, excitation is on.
+                units (Model372InputSensorUnits):
+                    Specifies the preferred units, Kelvin or Ohms, for the sensor.
                 resistance_range (Model372MeasurementInputResistance):
-                    * For measurement inputs only, specifies the measurement input resistance range.
+                    For measurement inputs only, specifies the measurement input resistance range.
 
         """
         self.mode = mode
         self.excitation_range = excitation_range
         self.auto_range = auto_range
         self.resistance_range = resistance_range
         self.current_source_shunted = current_source_shunted
@@ -321,74 +331,64 @@
                  reading_filter,
                  delay,
                  polarity=None):
         """The constructor for Model372HeaterOutputSettings class.
 
             Args:
                 output_mode (Model372OutputMode):
-                    * The control or output mode to configure the heater for. Defines how the output is controlled.
-
+                    The control or output mode to configure the heater for. Defines how the output is controlled.
                 input_channel (Model372InputChannel):
-                    * Which input to control output from in a control loop.
-
+                    Which input to control output from in a control loop.
                 powerup_enable (bool):
-                    * Specifies whether output stays on after powerup cycle.
-                    * True if enabled, False if disabled.
-
+                    Specifies whether output stays on after powerup cycle.
+                    True if enabled, False if disabled.
                 reading_filter (bool):
-                    * Specifies whether readings are filtered on unfiltered.
-                    * True if filtered, False if unfiltered
-
+                    Specifies whether readings are filtered on unfiltered.
+                    True if filtered, False if unfiltered.
                 delay (int):
-                    * Specifies delay in seconds for setpoint during AutoScanning. Options are:
-                    * 1 - 255
-
+                    Specifies delay in seconds for set-point during AutoScanning. Options are:
+                    1 - 255.
                 polarity (Model372Polarity):
-                    * Specifies output polarity. Not applicable to warmup heater.
+                    Specifies output polarity. Not applicable to warmup heater.
 
         """
         self.output_mode = output_mode
         self.input_channel = input_channel
         self.powerup_enable = powerup_enable
         self.polarity = polarity
         self.reading_filter = reading_filter
         self.delay = delay
 
 
 class Model372AlarmParameters:
-    """Sets up an alarm for an input channel"""
+    """Sets up an alarm for an input channel."""
 
     def __init__(self,
                  high_value,
                  low_value,
                  deadband,
                  latch_enable,
                  audible=None,
                  visible=None):
         """The constructor for Model372AlarmParameters class.
 
             Args:
                 high_value (int):
-                    * Sets value for source to be checked against to set high alarm
-
+                    Sets value for source to be checked against to set high alarm.
                 low_value (int):
-                    * Sets value for source to be checked against to set low alarm
-
+                    Sets value for source to be checked against to set low alarm.
                 deadband (int):
-                    * Sets value that source must change outside of an alarm condition
-                      to deactivate an unlatched alarm.
-
-                latch_enable (bool)
-                    * Specifies if alarm is latched or not
-
-                audible (bool)
-                    * Specifies if an alarm is audible or not
-
-                visible (bool)
-                    * Specifies if an alarm is visible via LED on front panel or not
+                    Sets value that source must change outside an alarm condition
+                    to deactivate an unlatched alarm.
+                latch_enable (bool):
+                    Specifies if alarm is latched or not.
+                audible (bool):
+                    Specifies if an alarm is audible or not.
+                visible (bool):
+                    Specifies if an alarm is visible via LED on front panel or not.
 
         """
         self.high_value = high_value
         self.low_value = low_value
         self.deadband = deadband
         self.latch_enable = latch_enable
         self.audible = audible
@@ -408,64 +408,59 @@
                  ramp_rate,
                  relay_1,
                  relay_2):
         """The constructor for Model372ControlLoopZoneSettings class.
 
             Args:
                 upper_bound (float):
-                    * upper bound setpoint in Kelvin
-
-                p_value (float)
-                    * The gain for a PID system. Options are:
-                    * 0.0 - 1000
-
-                i_value (float)
-                    * The integral value for a PID system. Options are:
-                    * 0 - 10000
-
-                d_value (float)
-                    * The rate for a PID system. Options are:
-                    * 0 - 2500
-
-                manual_output (float)
-                    * Percentage full scale manual output
-
-                heater_range (float or bool)
-                    * Heater range for the control zone.
-                    * Entered as a float for the sample heater
-                    * Entered as a bool for the warm-up heater
-
-                ramp_rate (float)
-                    * Specifies ramp rate for this zone
-
-                relay_1 (bool)
-                    * Specifies if relay 1 is on or off
-                    * Only applicable if relay is configured in zone mode and relay's control
-                        output matches configured output.
-
-                relay_2 (bool)
-                    * Specifies if relay 2 is on or off
-                    * Only applicable if relay is configured in zone mode and relay's control
-                        output matches configured output.
+                    Upper bound setpoint in Kelvin.
+                p_value (float):
+                    The gain for a PID system. Options are:
+                    0.0 - 1000.
+                i_value (float):
+                    The integral value for a PID system. Options are:
+                    0 - 10000.
+                d_value (float):
+                    The rate for a PID system. Options are:
+                    0 - 2500.
+                manual_output (float):
+                    Percentage full scale manual output.
+                heater_range (float or bool):
+                    Heater range for the control zone.
+                    Entered as a float for the sample heater.
+                    Entered as a bool for the warm-up heater.
+                ramp_rate (float):
+                    Specifies ramp rate for this zone.
+                relay_1 (bool):
+                    Specifies if relay 1 is on or off.
+                    Only applicable if relay is configured in zone mode and relay's control
+                    output matches configured output.
+                relay_2 (bool):
+                    Specifies if relay 2 is on or off.
+                    Only applicable if relay is configured in zone mode and relay's control
+                    output matches configured output.
 
         """
         self.upper_bound = upper_bound
         self.p_value = p_value
         self.i_value = i_value
         self.d_value = d_value
         self.manual_output = manual_output
         self.heater_range = heater_range
         self.ramp_rate = ramp_rate
         self.relay_1 = relay_1
         self.relay_2 = relay_2
 
 
 class Model372ReadingStatusRegister(RegisterBase):
-    """Class object representing the reading status of an input. While not a literal register, the return of an int
-    representation of multiple booleans makes it convenient to represent this functionality as a register."""
+    """Class object representing the reading status of an input.
+
+        While not a literal register, the return of an int representation of multiple booleans makes it convenient to
+        represent this functionality as a register.
+    """
     bit_names = [
         "current_source_overload",
         "voltage_common_mode_stage_overload",
         "voltage_mixer_stage_overload",
         "voltage_differential_stage_overload",
         "resistance_over",
         "resistance_under",
@@ -569,15 +564,15 @@
         self.d_2 = d_2
         self.d_3 = d_3
         self.d_4 = d_4
         self.d_5 = d_5
 
 
 class Model372(TemperatureController):
-    """A class object representing the Lake Shore Model 372 AC bridge and temperature controller"""
+    """A class object representing the Lake Shore Model 372 AC bridge and temperature controller."""
 
     vid_pid = [(0x1FB9, 0x0305)]
 
     # Override enums in base class
     _curve_format_enums = Model372CurveFormat
     _input_channel_enum = Model372InputChannel
     _display_units_enum = Model372DisplayFieldUnits
@@ -599,16 +594,19 @@
         # Call the parent init, then fill in values specific to the 372
         TemperatureController.__init__(self, serial_number, com_port, baud_rate, timeout, ip_address,
                                        tcp_port, **kwargs)
         # Disable emulation upon initialization
         self._disable_emulation_mode()
 
     def clear_interface(self):
-        """Clears the interace, such as all bits in the status byte register and the standard event
-        status register. Does not clear the instrument."""
+        """Clears the interface.
+
+            Clears all bits in the status byte register and the standard event status register. Does not clear the
+            instrument.
+        """
         self.command("*CLS")
 
     def reset_instrument(self):
         """Resets the instrument to power-up settings and parameters."""
         self.command("*RST")
 
     def _disable_emulation_mode(self):
@@ -631,15 +629,15 @@
         self.command(f"DISPLAY {mode},{number_of_fields},{displayed_info}")
 
     def get_display_mode(self):
         """Returns the current mode of the display.
 
             Returns:
                 (Model372DisplayMode):
-                    Enumerated object representing the current mode of the display
+                    Enumerated object representing the current mode of the display.
 
         """
         settings_string = self.query("DISPLAY?")
         separated_settings = settings_string.split(",")
         return Model372DisplayMode(int(separated_settings[0]))
 
     def get_custom_display_settings(self):
@@ -658,48 +656,46 @@
                 'number_of_fields': Model372DisplayFields(int(separated_settings[1])),
                 'displayed_info': Model372DisplayInfo(int(separated_settings[2]))}
 
     def get_resistance_reading(self, input_channel):
         """Returns the input reading in Ohms.
 
             Args:
-                input_channel (str or int)
-                    * Specifies which input channel to read from. Options are:
-                        * 1-16
-                        * "A" (for control input)
+                input_channel (str or int):
+                    Specifies which input channel to read from. Options are:
+                    1-16, or "A" (for control input).
 
             Returns:
                 (float):
-                    * Sensor reading in Ohms
+                    Sensor reading in Ohms.
 
         """
         return float(self.query(f"RDGR? {str(input_channel)}"))
 
     def get_quadrature_reading(self, input_channel):
         """Returns the imaginary part of the reading in Ohms. Only valid for measurement inputs.
 
             Args:
-                input_channel (int)
-                    * Specifies which input channel to read from. Options are:
-                        * 1-16
+                input_channel (int):
+                    Specifies which input channel to read from. Options are:
+                    1-16.
 
             Returns:
                 (float):
-                    * The imaginary part of the sensor reading, in Ohms
+                    The imaginary part of the sensor reading, in Ohms.
         """
         return float(self.query(f"QRDG? {str(input_channel)}"))
 
     def get_all_input_readings(self, input_channel):
         """Returns the kelvin reading, resistance reading, and, if a measurement input, the quadrature reading.
 
             Args:
-                input_channel (str or int)
-                    * Specifies which input channel to read from. Options are:
-                        * 1-16
-                        * "A" (for control input)
+                input_channel (str or int):
+                    Specifies which input channel to read from. Options are:
+                    1-16, or "A" (for control input).
 
             Returns:
                 (dict):
                     * If measurement input:
                         * {kelvin: float, resistance: float, power: float, quadrature: float)
                     * If control input:
                         * {kelvin: float, resistance: float, power: float}
@@ -717,23 +713,22 @@
 
         return readings
 
     def get_input_setup_parameters(self, input_channel):
         """Returns the settings on the specified input.
 
             Args:
-                input_channel (str or int)
-                    * Specifies which input channel to read from. Options are:
-                        * 1-16
-                        * "A" (control input)
+                input_channel (str or int):
+                    Specifies which input channel to read from. Options are:
+                    1-16, or "A" (control input).
 
             Returns:
-                input_sensor_settings (Model372InputSetupSettings)
-                    * object of Model372InputSetupSettings representing the parameters of the excitation of the sensor
-                        on the specified channel
+                input_sensor_settings (Model372InputSetupSettings):
+                    object of Model372InputSetupSettings representing the parameters of the excitation of the sensor
+                    on the specified channel
 
         """
         sensor_settings = self.query(f"INTYPE? {str(input_channel)}")
         separated_settings = sensor_settings.split(",")
         # Determine which enum to use to interpret excitation value:
         if input_channel == "A":
             excitation_range = Model372ControlInputCurrentRange(int(separated_settings[1]))
@@ -754,22 +749,20 @@
                                                            resistance_range)
         return input_sensor_settings
 
     def configure_input(self, input_channel, settings):
         """Sets the desired setup settings on the specified input.
 
             Args:
-                input_channel (str or int)
-                    * Specifies which input channel to read from. Options are:
-                        * 1-16
-                        * "A" (control input)
-
-                settings (Model372InputSetupSettings)
-                    * object of Model372InputSetupSettings representing the parameters of the excitation of the sensor
-                        on the specified channel
+                input_channel (str or int):
+                    Specifies which input channel to read from. Options are:
+                    1-16, or "A" (control input).
+                settings (Model372InputSetupSettings):
+                    Object of Model372InputSetupSettings representing the parameters of the excitation of the sensor
+                    on the specified channel.
 
         """
         # Handle control input not setting resistance range
         if input_channel == "A":
             resistance_range = 0
         else:
             resistance_range = format(settings.resistance_range)
@@ -780,247 +773,232 @@
                          f"{str(format(settings.units))}")
         self.command(command_string)
 
     def disable_input(self, input_channel):
         """Disables the desired input channel.
 
             Args:
-                input_channel (str or int)
-                    * Specifies which input channel to disable. Options are:
-                    * 1-16
-                    * "A" (control input)
+                input_channel (str or int):
+                    Specifies which input channel to disable. Options are:
+                    1-16, or "A" (control input).
 
         """
         self.command(f"INSET {str(input_channel)},0,0,0,0,0")
 
     def get_input_channel_parameters(self, input_channel):
-        """Returns the settings on the specified input channel
+        """Returns the settings on the specified input channel.
 
                 Args:
-                    input_channel (str or int)
-                        * Specifies which input channel to read from. Options are:
-                            * 1-16
-                            * "A" (control input)
+                    input_channel (str or int):
+                        Specifies which input channel to read from. Options are:
+                        1-16, or "A" (control input).
 
                 Returns:
-                    input_channel_settings (Model372InputChannelSettings)
-                        * Contains variables representing the different channel settings parameters
+                    input_channel_settings (Model372InputChannelSettings):
+                        Contains variables representing the different channel settings parameters.
 
         """
         input_parameters = self.query(f"INSET? {str(input_channel)}")
         separated_parameters = input_parameters.split(",")
         temperature_coefficient = Model372CurveTemperatureCoefficient(int(separated_parameters[4]))
         input_channel_settings = Model372InputChannelSettings(bool(int(separated_parameters[0])),
                                                               int(separated_parameters[1]),
                                                               int(separated_parameters[2]),
                                                               int(separated_parameters[3]),
                                                               temperature_coefficient)
         return input_channel_settings
 
     def set_input_channel_parameters(self, input_channel, settings):
-        """Sets the desired channel settings on the specified input channel
+        """Sets the desired channel settings on the specified input channel.
 
             Args:
-                input_channel (str or int)
-                    * Specifies which input channel to read from. Options are:
-                        * 1-16
-                        * "A" (control input)
-
-                settings (Model372InputChannelSettings)
-                    * Defines how to set the various parameters
+                input_channel (str or int):
+                    Specifies which input channel to read from. Options are:
+                    1-16, or
+                    "A" (control input).
+                settings (Model372InputChannelSettings):
+                    Defines how to set the various parameters.
 
         """
         if settings.temperature_coefficient is None:
             temperature_coefficient = ""
         else:
             temperature_coefficient = format(settings.temperature_coefficient)
         command_string = (f"INSET {str(input_channel)},{str(int(settings.enable))}," +
                          f"{str(settings.dwell_time)},{str(settings.pause_time)}," +
                          f"{str(settings.curve_number)},{str(temperature_coefficient)}")
         self.command(command_string)
 
     def get_analog_heater_output(self, output_channel):
-        """Returns the output of the warm-up or analog/still heater
+        """Returns the output of the warm-up or analog/still heater.
 
-           Args:
-                output_channel (int)
-                    * Specifies which heater to read from. Options:
-                        * 1 output 1 (warm up heater)
-                        * 2 output 2 (analog heater)
+            Args:
+                output_channel (int):
+                    Specifies which heater to read from. Options:
+                        1 output 1 (warm up heater), or
+                        2 output 2 (analog heater).
 
             Returns:
-                reading (float)
-                    * Output of the analog heater being queried
+                reading (float):
+                    Output of the analog heater being queried.
 
         """
         return float(self.query(f"AOUT? {str(output_channel)}"))
 
     def all_off(self):
-        """Recreates the front panel safety feature of shutting off all heaters"""
+        """Recreates the front panel safety feature of shutting off all heaters."""
         self.command("RANGE 0,0")
         self.command("RANGE 1,0")
         self.command("RANGE 2,0")
 
     def set_heater_output_range(self, output_channel, heater_range):
-        """Sets the output range
+        """Sets the output range.
 
-              Args:
-                    output_channel (int)
-                        * Specifies which heater to set. Options:
-                            * 0: sample heater
-                            * 1: output 1 (warm up heater)
-                            * 2: output 2 (analog heater)
-
-                    heater_range (Enum or bool)
-                        * Specifies the range of the output. Options:
-
-                            Sample Heater (Enum):
-                                * Object of type Model372SampleHeaterOutputRange
-
-                            Warmup Heater/Still Heater (bool):
-                                * False: output off
-                                * True: output on
+            Args:
+                output_channel (int):
+                    Specifies which heater to set. Options:
+                    0: sample heater,
+                    1: output 1 (warm up heater), or
+                    2: output 2 (analog heater).
+                heater_range (Enum or bool):
+                    Specifies the range of the output. Options:
+                    Sample Heater (Enum) - Object of type Model372SampleHeaterOutputRange.
+                    Warmup Heater/Still Heater (bool) - False: output off, True: output on.
 
         """
         if output_channel == 0:
             range_value = format(heater_range)
         else:
             range_value = int(heater_range)
 
         self.command(f"RANGE {str(output_channel)},{str(range_value)}")
 
     def get_heater_output_range(self, output_channel):
-        """Return's the range of the output on a given channel
+        """Return's the range of the output on a given channel.
 
-              Args:
-                    output_channel (int)
-                        * Specifies which heater to read from. Options:
-                            * 0: sample heater
-                            * 1: output 1 (warm up heater)
-                            * 2: output 2 (analog heater)
+            Args:
+                output_channel (int):
+                    Specifies which heater to read from. Options:
+                    0: sample heater,
+                    1: output 1 (warm up heater), or
+                    2: output 2 (analog heater).
 
-                Returns:
-                    heater_range (bool or Enum)
-                        * If channel 1 or 2, returns bool for if output is on or off.
-                        * If channel 0, an object of enum type Model372SampleHeaterOutputRange
+            Returns:
+                heater_range (bool or Enum):
+                    If channel 1 or 2, returns bool for if output is on or off.
+                    If channel 0, an object of enum type Model372SampleHeaterOutputRange.
 
         """
         key = int(self.query(f"RANGE? {str(output_channel)}"))
         if output_channel == 0:
             output_range = Model372SampleHeaterOutputRange(key)
         else:
             output_range = bool(key)
 
         return output_range
 
-    # Filter methods different than in temperature_instrument
+    # Filter methods different from in temperature_instrument
     def set_filter(self, input_channel, state, settle_time, window):
         """Sets a filter for the specified input channel.
 
             Args:
-                input_channel (str or int)
-                    * Specifies which input channel to read from. Options are:
-                        * 0 (all channels/measurement inputs)
-                        * 1-16
-                        * "A" (control input)
-
-                state (bool)
-                    * Specifies whether to turn filter on or off. Options are:
-                        * False for off, True for on
-
-                settle_time (float)
-                    * Specifies filter settle time. Options are:
-                        * 1 - 200 s
-
-                window (float)
-                    * Specifies what percent of full scale reading limits the filtering function.
-                    * Options are:
-                        * 1 - 80
+                input_channel (str or int):
+                    Specifies which input channel to read from. Options are:
+                    0 (all channels/measurement inputs),
+                    1-16, or
+                    "A" (control input).
+                state (bool):
+                    Specifies whether to turn filter on or off. Options are:
+                    False for off, or
+                    True for on.
+                settle_time (float):
+                    Specifies filter settle time. Options are:
+                    1 - 200 s.
+                window (float):
+                    Specifies what percent of full scale reading limits the filtering function. Options are:
+                    1 - 80.
 
         """
 
         self.command(f"FILTER {str(input_channel)},{str(int(state))},{str(settle_time)},{str(window)}")
 
     def get_filter(self, input_channel):
         """Returns information about the filter set on the specified channel.
 
             Args:
-                input_channel (str or int)
-                    * Specifies which input channel to read from. Options are:
-                    * 1-16
-                    * "A" (control input)
+                input_channel (str or int):
+                    Specifies which input channel to read from. Options are:
+                    1-16, or "A" (control input).
 
             Returns:
-                state (bool)
-                    * Specifies whether to turn filter on or off.
-
-                settle_time (int)
-                    * Specifies filter settle time.
-
-                window (int)
-                    * Specifies what percent of full scale reading limits the filtering function.
+                state (bool):
+                    Specifies whether to turn filter on or off.
+                settle_time (int):
+                    Specifies filter settle time.
+                window (int):
+                    Specifies what percent of full scale reading limits the filtering function.
 
         """
         output_string = self.query(f"FILTER? {str(input_channel)}")
         separated_response = output_string.split(",")
         return {"state": bool(int(separated_response[0])),
                 "settle_time": int(separated_response[1]),
                 "window": int(separated_response[2])}
 
     def set_ieee_interface_parameter(self, address):
         """Sets the IEEE address of the instrument.
 
             Args:
-                address (int)
-                * Specifies the IEEE address. Options are:
-                * 1 - 30
+                address (int):
+                    Specifies the IEEE address. Options are:
+                    1 - 30.
 
         """
         self.command(f"IEEE 0,0,{str(address)}")
 
     def get_ieee_interface_parameter(self):
         """Returns the IEEE address of the instrument.
 
             Returns:
-                address (int)
-                    * The IEEE address.
+                address (int):
+                    The IEEE address.
 
         """
         return int(self.query("IEEE?"))
 
     def get_excitation_power(self, input_channel):
-        """Returns the most recent power calculation for the selected input channel
+        """Returns the most recent power calculation for the selected input channel.
 
-                Args:
-                    input_channel (str or int)
-                        * Specifies which input channel to read from. Options are:
-                        * 1-16
-                        * "A" (control input)
+            Args:
+                input_channel (str or int):
+                    Specifies which input channel to read from. Options are:
+                    1-16, or
+                    "A" (control input).
 
-                Returns:
-                    power (float)
-                        * Most recent power calculation for the input being queried
+            Returns:
+                power (float):
+                    Most recent power calculation for the input being queried.
 
         """
         return float(self.query(f"RDGPWR? {str(input_channel)}"))
 
     def get_heater_output_settings(self, output_channel):
         """Returns the mode and settings of the given output channel.
 
-                Args:
-                    output_channel (int)
-                        * Specifies which heater to read from. Options:
-                            * 0: sample heater
-                            * 1: output 1 (warm up heater)
-                            * 2: output 2 (analog heater)
+            Args:
+                output_channel (int):
+                    Specifies which heater to read from. Options:
+                    0: sample heater,
+                    1: output 1 (warm up heater), or
+                    2: output 2 (analog heater).
 
-                Returns:
-                    outputmode_settings (Model372HeaterOutputSettings)
-                        * Object of class Model372HeaterOutputSettings whose variables are set to reflect the
-                            current output settings of the queried heater.
+            Returns:
+                outputmode_settings (Model372HeaterOutputSettings):
+                    Object of class Model372HeaterOutputSettings whose variables are set to reflect the
+                    current output settings of the queried heater.
 
         """
         output_mode = self.query(f"OUTMODE? {str(output_channel)}")
         separated_response = output_mode.split(",")
         # Handle special case of control input not being an int
         if separated_response[1] == "A":
             input_channel = Model372InputChannel('A')
@@ -1031,26 +1009,26 @@
                                             input_channel,
                                             bool(int(separated_response[2])),
                                             bool(int(separated_response[4])),
                                             int(separated_response[5]),
                                             Model372Polarity(int(separated_response[3])))
 
     def configure_heater(self, output_channel, settings):
-        """Sets up a heater output. Analog heaters (outputs 1 and 2) might need to configure further settings in
-        configure_analog_heater.
+        """Sets up a heater output.
 
-            Args:
-                output_channel (int)
-                    * Specifies which heater to read from. Options:
-                        * 0: sample heater
-                        * 1: output 1 (warm up heater)
-                        * 2: output 2 (analog heater)
+            Analog heaters (outputs 1 and 2) might need to configure further settings in configure_analog_heater.
 
-                settings (Model372HeaterOutputSettings)
-                    * Defines how to set the output mode settings
+            Args:
+                output_channel (int):
+                    Specifies which heater to read from. Options:
+                    0: sample heater,
+                    1: output 1 (warm up heater), or
+                    2: output 2 (analog heater).
+                settings (Model372HeaterOutputSettings):
+                    Defines how to set the output mode settings.
 
         """
         if settings.polarity is None:
             polarity = 0
         else:
             polarity = format(settings.polarity)
 
@@ -1070,326 +1048,331 @@
 
         self.command(command_string)
 
     def set_common_mode_reduction(self, state):
         """Sets common mode reduction to given state for all measurement channels.
 
             Args:
-                state (bool)
-                    * Sets CMR to enabled or disable. Options are:
-                    * False (for disable) or True (for enable)
+                state (bool):
+                    Sets CMR to enabled or disable. Options are:
+                    False (for disable), or
+                    True (for enable).
 
         """
         self.command(f"CMR {str(int(state))}")
 
     def get_common_mode_reduction(self):
-        """Returns whether or not CMR is set for measurement channels
+        """Returns whether CMR is set for measurement channels.
 
             Returns:
-                * False (boolean) if CMR is disabled
-                * True (boolean) if CMR is enabled
+                False (boolean) if CMR is disabled, or
+                True (boolean) if CMR is enabled.
 
         """
         return bool(int(self.query("CMR?")))
 
     def set_scanner_status(self, input_channel, status):
-        """Sets the scanner to the specified channel, and enables or disables auto scan
+        """Sets the scanner to the specified channel, and enables or disables auto scan.
 
             Args:
-                input_channel (int)
-                    * Specifies which measurement input to set the scanner to. Options are:
-                        * 1 - 16
-
-                status (bool)
-                    * Specifies whether to turn auto scan feature on. Options are:
-                        * False (disable) or True (enable)
+                input_channel (int):
+                    Specifies which measurement input to set the scanner to. Options are:
+                    1 - 16.
+                status (bool):
+                    Specifies whether to turn auto scan feature on. Options are:
+                    False (disable), True (enable).
 
         """
         self.command(f"SCAN {str(input_channel)},{str(int(status))}")
 
     def get_scanner_status(self):
-        """Returns which channel the scanner is on and whether the auto scan feature is enabled
+        """Returns which channel the scanner is on and whether the auto scan feature is enabled.
 
             Returns:
-                input_channel (int)
-                    * The measurement channel the scanner is currently on.
+                input_channel (int):
+                    The measurement channel the scanner is currently on.
 
-                status (bool)
-                    * True if autoscan in on, False if autoscan is off
+                status (bool):
+                    True if auto-scan in on, or
+                    False if auto-scan is off.
 
         """
         response = self.query("SCAN?")
         separated_response = response.split(",")
         return {"input_channel": int(separated_response[0]),
                 "status": bool(int(separated_response[1]))}
 
     def set_alarm_beep(self, status):
-        """Enables or disables a beep for alarms
+        """Enables or disables a beep for alarms.
 
             Args:
-                status (bool)
-                    * False (for disable) or True (for enable)
+                status (bool):
+                    False (for disable), or
+                    True (for enable).
 
         """
         self.command(f"BEEP {str(int(status))}")
 
     def get_alarm_beep_status(self):
         """Returns whether beep for alarms is enabled or disabled.
 
             Returns
-                status (bool)
-                        * Returns True is beep is enabled.
-                        * Returns False is beep is disabled.
+                status (bool):
+                    True (beep is enabled), or
+                    False (beep is disabled).
 
         """
         return bool(int(self.query("BEEP?")))
 
     def set_still_output(self, power):
-        """Sets the still output of the still/analog heater to power% of full power. Heater gets configured for
-        Still mode if not currently configured.
+        """Sets the still output of the still/analog heater to power% of full power.
+
+            Heater gets configured for still mode if not currently configured.
 
             Args:
-                  power (float)
-                      * Specifies the percent of full power for still output. Options are:
-                        * 0 - 100
+                power (float):
+                    Specifies the percent of full power for still output. Options are:
+                    0 - 100.
 
         """
         settings = self.get_heater_output_settings(2)
         settings.output_mode = Model372OutputMode.STILL
         self.configure_heater(2, settings)
         self.command(f"STILL {str(power)}")
 
     def get_still_output(self):
         """Returns the percent of full power being outputted by still heater in still mode.
 
             Returns:
-                    power (float)
-                        * percent of full power being outputted by heater.
+                    power (float):
+                        Percent of full power being outputted by heater.
 
         """
         return float(self.query("STILL?"))
 
     def set_warmup_output(self, auto_control, current):
         """Sets up the warmup output to continuous control at the percent current specified.
-        Configures the warmup heater for continuous control mode from the control input.
+
+            Configures the warmup heater for continuous control mode from the control input.
 
             Args:
-                auto_control (bool)
-                    * Specifies whether or not to turn on auto control. Options are:
-                        * False for auto off, True for continuous
+                auto_control (bool):
+                    Specifies whether to turn on auto control. Options are:
+                    False for auto off, or
+                    True for continuous.
 
-                current (float)
-                    * Specifies percent of full current to apply to external output. Options are:
-                        * 0 - 100
+                current (float):
+                    Specifies percent of full current to apply to external output. Options are:
+                    0 - 100
 
         """
         settings = self.get_heater_output_settings(1)
         settings.output_mode = Model372OutputMode.WARMUP
         self.configure_heater(1, settings)
         self.command(f"WARMUP {str(int(auto_control))},{str(current)}")
 
     def get_warmup_output(self):
         """Returns the control setting and percent current outputted in the warmup heater in warmup mode.
 
             Returns:
-                auto_control (bool)
-                    * Specifies whether or not to turn on auto control. Returns:
-                        * False for auto off, True for continuous
+                auto_control (bool):
+                    Specifies whether to turn on auto control. Returns:
+                    False for auto off, or
+                    True for continuous
 
-                current (float)
-                    * Specifies percent of full current to apply to external output.
+                current (float):
+                    Specifies percent of full current to apply to external output.
 
         """
         output_string = self.query("WARMUP?")
         separated_response = output_string.split(",")
         return {'auto_control': bool(int(separated_response[0])),
                 'current': float(separated_response[1])}
 
     def set_setpoint_kelvin(self, output_channel, setpoint):
-        """Sets the control setpoint in Kelvin. Changes input parameters so preferred units are Kelvin.
+        """Sets the control set-point in Kelvin. Changes input parameters so preferred units are Kelvin.
 
             Args:
-                output_channel (int)
-                    * Specifies which heater to set a setpoint. Options are:
-                        * 0: sample heater
-                        * 1: output 1 (warm up heater)
+                output_channel (int):
+                    Specifies which heater to set a set-point. Options are:
+                    0: sample heater, or
+                    1: output 1 (warm up heater).
 
-                setpoint (float)
-                    * Specifies the setpoint the heater ramps to, in Kelvin.
+                setpoint (float):
+                    Specifies the set-point the heater ramps to, in Kelvin.
 
         """
         # First, get control input from OUTMODE settings to change preferred units
         outmode_settings = self.get_heater_output_settings(output_channel)
         control_input = outmode_settings.input_channel.value
         settings = self.get_input_setup_parameters(control_input)
         settings.units = Model372InputSensorUnits.KELVIN
         self.configure_input(control_input, settings)
         # Set setpoint now that units are configured properly
         self.command(f"SETP {str(output_channel)},{str(setpoint)}")
 
     def set_setpoint_ohms(self, output_channel, setpoint):
-        """Sets the control setpoint in Ohms. Changes input parameters so preferred units are Ohms.
+        """Sets the control set-point in Ohms. Changes input parameters so preferred units are Ohms.
 
             Args:
-                output_channel (int)
-                    * Specifies which heater to set a setpoint. Options are:
-                        * 0: sample heater
-                        * 1: output 1 (warm up heater)
+                output_channel (int):
+                    Specifies which heater to set a set-point. Options are:
+                    0: sample heater, or
+                    1: output 1 (warm up heater).
 
-                setpoint (float)
-                    * Specifies the setpoint the heater ramps to, in Kelvin.
+                setpoint (float):
+                    Specifies the set-point the heater ramps to, in Kelvin.
 
         """
 
         # First, get control input from OUTMODE settings to change preferred units
         outmode_settings = self.get_heater_output_settings(output_channel)
         control_input = outmode_settings.input_channel.value
         # Change settings to change preferred units to Ohms
         settings = self.get_input_setup_parameters(control_input)
         settings.units = Model372InputSensorUnits.OHMS
         self.configure_input(control_input, settings)
         # Set setpoint
         self.command(f"SETP {str(output_channel)},{str(setpoint)}")
 
     def get_setpoint_kelvin(self, output_channel):
-        """Returns the setpoint for the given output channel in kelvin. Changes the control input's preferred
-        units to Kelvin as a result.
+        """Returns the set-point for the given output channel in kelvin.
+
+            Changes the control input's preferred units to Kelvin as a result.
 
             Args:
-                output_channel (int)
-                    * Specifies which heater to set a setpoint. Options are:
-                        * 0: sample heater
-                        * 1: output 1 (warm up heater)
+                output_channel (int):
+                    Specifies which heater to set a set-point. Options are:
+                    0: sample heater, or
+                    1: output 1 (warm up heater).
 
             Returns:
-                setpoint (float)
-                    * Setpoint of the output in Kelvin.
+                setpoint (float):
+                    Set-point of the output in Kelvin.
 
         """
         outmode_settings = self.get_heater_output_settings(output_channel)
         control_input = outmode_settings.input_channel.value
         settings = self.get_input_setup_parameters(control_input)
         settings.units = Model372InputSensorUnits.KELVIN
         self.configure_input(control_input, settings)
         return float(self.query(f"SETP? {str(output_channel)}"))
 
     def get_setpoint_ohms(self, output_channel):
-        """Returns the setpoint for the given output channel in kelvin. Changes the control input's preferred
-        units to Kelvin as a result.
+        """Returns the set-point for the given output channel in kelvin.
+
+            Changes the control input's preferred units to Kelvin as a result.
 
             Args:
-                output_channel (int)
-                    * Specifies which heater to set a setpoint. Options are:
-                        * 0: sample heater
-                        * 1: output 1 (warm up heater)
+                output_channel (int):
+                    Specifies which heater to set a set-point. Options are:
+                    0: sample heater, or
+                    1: output 1 (warm up heater).
 
             Returns:
-                setpoint (float)
-                    * Setpoint of the output in Ohms.
+                setpoint (float):
+                    Set-point of the output in Ohms.
 
         """
         outmode_settings = self.get_heater_output_settings(output_channel)
         control_input = outmode_settings.input_channel.value
         settings = self.get_input_setup_parameters(control_input)
         settings.units = Model372InputSensorUnits.OHMS
         self.configure_input(control_input, settings)
         return float(self.query(f"SETP? {str(output_channel)}"))
 
     def get_excitation_frequency(self, input_channel):
         """Returns the excitation frequency in Hz for either the measurement or control inputs.
 
             Args:
-                input_channel (int or str)
-                    * Specifies which input to get frequency from. Options are:
-                        * 0 : measurement inputs
-                        * "A" : control input
+                input_channel (int or str):
+                    Specifies which input to get frequency from. Options are:
+                    0 : measurement inputs, or
+                    "A" : control input.
 
             Returns:
-                frequency (Enum)
-                    * The excitation frequency in Hz, returned as an object of Model372InputFrequency Enum type
+                frequency (Enum):
+                    The excitation frequency in Hz, returned as an object of Model372InputFrequency Enum type.
 
         """
         key = int(self.query(f"FREQ? {str(input_channel)}"))
         return Model372InputFrequency(key)
 
     def set_excitation_frequency(self, input_channel, frequency):
         """Sets the excitation frequency (in Hz) for either the measurement or control inputs.
 
             Args:
-                input_channel (int or str)
-                    * Specifies which input to get frequency from. Options are:
-                        * 0 : measurement inputs
-                        * "A" : control input
+                input_channel (int or str):
+                    Specifies which input to get frequency from. Options are:
+                    0 : measurement inputs, or
+                    "A" : control input.
 
-                frequency (Enum)
-                    * The excitation frequency in Hz (if float), represented as an object of type Model372InputFrequency
+                frequency (Enum):
+                    The excitation frequency in Hz (if float), represented as an object of type Model372InputFrequency.
 
         """
         self.command(f"FREQ {input_channel},{frequency}")
 
     def set_digital_output(self, bit_weight):
         """Sets the status of the 5 digital output lines to high or low.
 
             Args:
-                bit_weight (DigitalOutputRegister)
-                    * Determines which bits to set or reset
+                bit_weight (DigitalOutputRegister):
+                    Determines which bits to set or reset.
 
         """
         bit_weight_integer = bit_weight.to_integer()
         self.command(f"DOUT {str(bit_weight_integer)}")
 
     def get_digital_output(self):
-        """Returns which digital output bits are set or reset by representing them in a binary
-        number.
+        """Returns which digital output bits are set or reset by representing them in a binary number.
 
             Returns:
-                bit_weight (DigitalOutputRegister)
-                    * Determines which bits to set or reset
+                bit_weight (DigitalOutputRegister):
+                    Determines which bits to set or reset.
 
         """
         bit_weight_integer = int(self.query("DOUT?"))
         return Model372DigitalOutputRegister.from_integer(bit_weight_integer)
 
     def set_interface(self, interface):
         """Sets the interface for the instrument to communicate over.
 
             Args:
-                interface (Model372Interface)
-                    * selects the interface based on the values as defined in the Model372Interface enum class
+                interface (Model372Interface):
+                    Selects the interface based on the values as defined in the Model372Interface enum class.
 
         """
         self.command(f"INTSEL {interface}")
 
     def get_interface(self):
         """Returns the interface connected to the instrument.
 
             Returns:
-                interface (Model372Interface)
-                    * returns the interface as an object of the Model372Interface enum class.
+                interface (Model372Interface):
+                    Returns the interface as an object of the Model372Interface enum class.
 
         """
         value = int(self.query("INTSEL?"))
         return Model372Interface(value)
 
     def set_alarm_parameters(self, input_channel, alarm_enable, alarm_settings=None):
         """Sets an alarm on the specified channel as defined by parameters.
 
             Args:
-                input_channel (int or str)
-                    * Defines which channel to configure an alarm on. Options are:
-                        * 0 for all measurement inputs
-                        * 1 - 16
-                        * "A" for control input
-
+                input_channel (int or str):
+                    Defines which channel to configure an alarm on. Options are:
+                    0 for all measurement inputs,
+                    1 - 16, or
+                    "A" for control input.
                 alarm_enable (bool)
-                    * Defines whether to turn alarm on or off
-
+                    Defines whether to turn alarm on or off.
                 alarm_settings (Model372AlarmParameters)
-                    * Model372AlarmParameters object containing desired alarm settings
-                    * Optional if alarm is disabled
+                    Model372AlarmParameters object containing desired alarm settings.
+                    Optional if alarm is disabled.
 
         """
         if alarm_settings is not None:
             if alarm_settings.visible is None:
                 visible = ""
             else:
                 visible = int(alarm_settings.visible)
@@ -1407,110 +1390,106 @@
         else:
             self.command(f"ALARM {input_channel},0,0,0,0,0,0,0")
 
     def get_alarm_parameters(self, input_channel):
         """Returns the parameters for the alarm set for the input at the specified channel.
 
             Args:
-                input_channel (int or str)
-                    * Defines which channel to configure an alarm on. Options are:
-                    * 1 - 16
-                    * "A" for control input
+                input_channel (int or str):
+                    Defines which channel to configure an alarm on. Options are: 1 - 16, or "A" for control input.
 
             Returns:
                 (dict):
-                    {alarm_enable: bool, alarm_settings: Model372AlarmParameters
+                    {"alarm_enable": bool, "alarm_settings": Model372AlarmParameters}
 
         """
         settings_string = self.query(f"ALARM? {str(input_channel)}")
         separated_settings = settings_string.split(",")
         alarm_settings = Model372AlarmParameters(int(separated_settings[2]),
                                                  int(separated_settings[3]), int(separated_settings[4]),
                                                  bool(int(separated_settings[5])), bool(int(separated_settings[6])),
                                                  bool(int(separated_settings[7])))
 
         return {'alarm_enable': bool(int(separated_settings[0])),
                 'alarm_settings': alarm_settings}
 
     def set_relay_for_sample_heater_control_zone(self, relay_number):
-        """Configures a relay to follow the sample heater output as part of a control zone. Settings can be
-        further configured in set_control_loop_zone_parameters method.
+        """Configures a relay to follow the sample heater output as part of a control zone.
+
+            Settings can be further configured in set_control_loop_zone_parameters method.
 
             Args:
                 relay_number (int):
-                    * The relay to configure.
-                    * Options are:
-                        * 1 or 2
+                    The relay to configure. Options are: 1 or 2.
 
         """
         self.command(f"RELAY {relay_number},3,0,0")
 
     def set_relay_for_warmup_heater_control_zone(self, relay_number):
-        """Configures a relay to follow the warm up heater output as part of a control zone. Settings can be
-            further configured in set_control_loop_zone_parameters method.
+        """Configures a relay to follow the warm-up heater output as part of a control zone.
+
+            Settings can be further configured in set_control_loop_zone_parameters method.
 
                 Args:
                     relay_number (int):
-                        * The relay to configure.
-                        * Options are:
-                            * 1 or 2
+                        The relay to configure. Options are: 1 or 2.
 
             """
         self.command(f"RELAY {relay_number},4,0,0")
 
     def get_ieee_interface_mode(self):
         """Returns the IEEE interface mode of the instrument.
 
             Returns:
-                mode (Model372InterfaceMode)
-                    * returns the mode as an enum type of class Model372InterfaceMode
+                mode (Model372InterfaceMode):
+                    Returns the mode as an enum type of class Model372InterfaceMode.
 
         """
         value = int(self.query("MODE?"))
         return Model372InterfaceMode(value)
 
     def set_ieee_interface_mode(self, mode):
         """Sets the IEEE interface mode of the instrument.
 
             Args:
-                mode (Model372InterfaceMode)
-                    * Defines the mode of the instrument as an object of the enum type Model372IEEEInterfaceMode
+                mode (Model372InterfaceMode):
+                    Defines the mode of the instrument as an object of the enum type Model372IEEEInterfaceMode.
 
         """
         value = format(mode)
         self.command(f"MODE {str(value)}")
 
     def set_monitor_output_source(self, source):
         """Sets the source of the monitor output. Also affects the reference output.
 
             Args:
-                source (Model372MonitorOutputSource)
-                    * Defines the source to run the monitor output off of.
+                source (Model372MonitorOutputSource):
+                    Defines the source to run the monitor output off of.
 
         """
         value = format(source)
         self.command(f"MONITOR {str(value)}")
 
     def get_monitor_output_source(self):
         """Returns the source for the monitor output.
 
             Returns:
-                source (Model372MonitorOutputSource)
-                    * returns the source as an object of the Model372MonitorOutputSource class.
+                source (Model372MonitorOutputSource):
+                    Returns the source as an object of the Model372MonitorOutputSource class.
 
         """
         value = int(self.query("MONITOR?"))
         return Model372MonitorOutputSource(value)
 
     def get_warmup_heater_setup(self):
         """Returns the settings regarding the resistance, current and units of the warmup heater (output channel 1).
 
             Returns:
                 (dict):
-                    {resistance: float, max_current: float, units: Model372HeaterOutputUnits}
+                    {"resistance": float, "max_current": float, "units": Model372HeaterOutputUnits}
         """
         settings_string = self.query("HTRSET? 1")
         separated_settings = settings_string.split(",")
         # Check to see if current is enumerated or custom
         if int(separated_settings[1]) == 1:
             max_current = 0.45
         elif int(separated_settings[1]) == 2:
@@ -1523,72 +1502,72 @@
                 'units': Model372HeaterOutputUnits(int(separated_settings[3]))}
 
     def get_sample_heater_setup(self):
         """Returns the setup of the sample heater (channel 0).
 
             Returns:
                 (dict):
-                    {resistance: float, units: Model372HeaterOutputUnits}
+                    {"resistance": float, "units": Model372HeaterOutputUnits}
         """
         settings_string = self.query("HTRSET? 0")
         separated_settings = settings_string.split(",")
         return {'resistance': float(separated_settings[0]),
                 'units': Model372HeaterOutputUnits(int(separated_settings[3]))}
 
     def setup_warmup_heater(self, resistance, max_current, units):
-        """Configures the current and power of the warmup heater (output channel 1). The max current must not cause
-        the heater to exceed it's max power (calculated by I = sqrt(P/R)) or it's max voltage (calculated by
-        I = V/R). Check your heater's specifications before setting the max current, and use the lower current
-        produced from the two calculations.
+        """Configures the current and power of the warmup heater (output channel 1).
+
+            The max current must not cause the heater to exceed it's max power (calculated by I = sqrt(P/R)) or it's
+            max voltage (calculated by I = V/R). Check your heater's specifications before setting the max current, and
+            use the lower current produced from the two calculations.
 
             Args:
                 resistance (Model372HeaterResistance):
-                    * Heater load in ohms, as an object of the enum type Model372HeaterResistance
-
+                    Heater load in ohms, as an object of the enum type Model372HeaterResistance.
                 max_current (float):
-                    * User specified max current in A.
-
+                    User specified max current in A.
                 units (Model372HeaterOutputUnits):
-                    * Defines which units the output is displayed in (Current (A) or Power (W))
+                    Defines which units the output is displayed in (Current (A) or Power (W)).
 
         """
         command_string = f"HTRSET 1,{resistance},0,{max_current},{units}"
         self.command(command_string)
 
     def setup_sample_heater(self, resistance, units):
         """Configures the current and power of the sample heater (output channel 0.)
 
             Args:
                 resistance (float):
-                    * Heater load in ohms. Options are:
-                        * 1 - 2000
+                    Heater load in ohms. Options are: 1 - 2000.
 
                 units (Model372HeaterOutputUnits):
-                    * Defines which units the output is displayed in (Current (A) or Power (W))
+                    Defines which units the output is displayed in (Current (A) or Power (W)).
 
         """
         command_string = f"HTRSET 0,{resistance},0,0,{units}"
         self.command(command_string)
 
     def configure_analog_monitor_output_heater(self, source, high_value, low_value, settings=None):
-        """Configures the still heater's analog settings for Monitor Out mode. Can fully configure the heater by
-        including the settings parameter, but it is recommended to configure non-analog properties of the heater through
-        the configure_heater method.
+        """Configures the still heater's analog settings for Monitor Out mode.
+
+            Can fully configure the heater by including the settings parameter, but it is recommended to configure
+            non-analog properties of the heater through the configure_heater method.
 
             Args:
-                source (Model372InputSensorUnits)
-                    The units to use for channel data
-                high_value (float)
-                    The data at which the output reaches +100% output
-                low_value (float)
-                    The data at which the outputs reaches 0% output for unipolar output, or -100% for bipolar
+                source (Model372InputSensorUnits):
+                    The units to use for channel data.
+                high_value (float):
+                    The data at which the output reaches +100% output.
+                low_value (float):
+                    The data at which the outputs reach 0% output for unipolar output, or -100% for bipolar.
                     output.
-                settings (Model372HeaterOutputSettings)
+                settings (Model372HeaterOutputSettings):
                     Optional if heater is already configured using configure_heater. Gives non-analog configurations
                     for heater.
+
         """
         if settings is None:
             # Use the settings already configured to avoid changing any settings
             settings = self.get_heater_output_settings(2)
         # Retrieve value from input_channel enum
         if isinstance(settings.input_channel, Model372InputChannel):
             input_channel = settings.input_channel.value
@@ -1598,122 +1577,116 @@
         self.command(command_string)
 
     def get_analog_monitor_output_settings(self):
         """Retrieves the analog monitor settings of output 2 configured in monitor output mode.
 
             Returns:
                 (dict):
-                    {source: Model372InputSensorUnits, high_value: float, low_value: float}
+                    {"source": Model372InputSensorUnits, "high_value": float, "low_value": float}
+
         """
         settings_string = self.query("ANALOG? 2")
         separated_settings = settings_string.split(",")
         return {'source': Model372InputSensorUnits(int(separated_settings[3])),
                 'high_value': float(separated_settings[4]),
                 'low_value': float(separated_settings[5])}
 
     def configure_analog_heater(self, output_channel, manual_value, settings=None):
         """Configures the analog settings of a heater for modes other than Monitor Out.
-        (Use configure_analog_monitor_out_heater for Monitor Out mode). Can fully configure the heater by including the
-        settings parameter, but it is recommended to first configure the heater using the configure_heater method before
-        using this method.
+
+            (Use configure_analog_monitor_out_heater for Monitor Out mode). Can fully configure the heater by including
+            the settings parameter, but it is recommended to first configure the heater using the configure_heater
+            method before using this method.
 
             Args:
                 output_channel (Model372HeaterOutput):
                     The output to configure.
-
                 manual_value (float):
                     The value of the analog output as it applies to the set analog mode.
-
-                settings (Model372HeaterOutputSettings)
+                settings (Model372HeaterOutputSettings):
                     Optional if heater is already configured using configure_heater. Gives non-analog configurations
                     for heater.
+
         """
         if settings is None:
             settings = self.get_heater_output_settings(output_channel)
         if isinstance(settings.input_channel, Model372InputChannel):
             input_channel = settings.input_channel.value
         else:
             input_channel = settings.input_channel
         command_string = f"ANALOG {output_channel},{settings.output_mode},{settings.polarity},{input_channel},0,0,0,{manual_value}"
         self.command(command_string)
 
     def get_analog_manual_value(self, output_channel):
-        """Returns the manual value of an analog heater. The manual value is the analog value used for Open Loop,
-        Closed Loop, Warm Up, or Still mode.
+        """Returns the manual value of an analog heater.
+
+            The manual value is the analog value used for Open Loop, Closed Loop, Warm Up, or Still mode.
 
             Args:
                 output_channel (int):
-                    The analog output to query. Options are:
-                        * 1 (Warm up heater)
-                        * 2 (Still heater)
+                    The analog output to query. Options are: 1 (Warm up heater), or 2 (Still heater).
 
             Returns:
                 (float):
                     The manual analog value for the heater.
         """
         settings_string = self.query(f"ANALOG? {str(output_channel)}")
         separated_settings = settings_string.split(",")
         return float(separated_settings[6])
 
     def set_website_login(self, username, password):
         """Sets the username and password to connect instrument to website.
 
             Args:
-                username (str)
-                    * username to set for login. Must be less than or equal to 15 characters. Method
-                        automatically puts quotation marks around string, so they are not needed in the
-                        string literal passed into the method.
-
-                password (str)
-                    * password to set for login. Must be less than or equal to 15 characters. Method
-                        automatically puts quotation marks around string, so they are not needed in the
-                        string literal passed into the method.
+                username (str):
+                    Username to set for login. Must be less than or equal to 15 characters. Method
+                    automatically puts quotation marks around string, so they are not needed in the
+                    string literal passed into the method.
+                password (str):
+                    Password to set for login. Must be less than or equal to 15 characters. Method
+                    automatically puts quotation marks around string, so they are not needed in the
+                    string literal passed into the method.
 
         """
         self.command(f"WEBLOG \"{username}\",\"{password}\"")
 
     def get_website_login(self):
         """Returns the set username and password for web login for the instrument.
 
             Returns:
                 username (str):
-                    * The current set username for the web login
-
+                    The current set username for the web login
                 password (str):
-                    * The current set password for the web login
+                    The current set password for the web login
 
         """
         username_password = self.query("WEBLOG?")
         separated_string = username_password.split(",")
         # Remove padded whitespace in the returned username and password
         username_split = separated_string[0].split(" ")
         username = username_split[0]
         password_split = separated_string[1].split(" ")
         password = password_split[0]
         return {"username": username,
                 "password": password}
 
     def get_control_loop_zone_parameters(self, output_channel, zone):
-        """Returns the settings parameters of the control loop on the specified output channel
-        and zone.
+        """Returns the settings parameters of the control loop on the specified output channel and zone.
 
             Args:
-                output_channel (int)
-                    * Channel of the heater being queried. Options are:
-                        * 0 for sample heater
-                        * 1 for warm-up heater
-
-                zone (int)
-                    * Control loop zone to configure. Options are:
-                        * 1 - 10
+                output_channel (int):
+                    Channel of the heater being queried. Options are: 0 for sample heater, or 1 for warm-up heater.
+                zone (int):
+                    Control loop zone to configure. Options are: 1 - 10.
 
             Returns:
-                settings (Model372ControlLoopZoneSettings)
-                    * An object of the Model372ControlLoopZoneSettings class containing information of the
-                        settings in the values of its variables.
+                settings (Model372ControlLoopZoneSettings):
+                    An object of the Model372ControlLoopZoneSettings class containing information of the
+                    settings in the values of its variables.
+
         """
         settings_string = self.query(f"ZONE? {str(output_channel)},{str(zone)}")
         separated_settings = settings_string.split(",")
         # Use if statement to use correct dictionary to convert range to bool or float
         if output_channel == 0:
             heater_range = Model372SampleHeaterOutputRange(int(separated_settings[5]))
         else:
@@ -1722,30 +1695,24 @@
                                                    float(separated_settings[2]), float(separated_settings[3]),
                                                    float(separated_settings[4]), heater_range,
                                                    float(separated_settings[6]), bool(int(separated_settings[7])),
                                                    bool(int(separated_settings[8])))
         return settings
 
     def set_control_loop_parameters(self, output_channel, zone, settings):
-        """Returns the parameters of the control loop set in the specified zone for the specified
-        heater output.
+        """Returns the parameters of the control loop set in the specified zone for the specified heater output.
 
             Args:
-                 output_channel (int)
-                    * Channel of the heater being queried. Options are:
-                        * 0 for sample heater
-                        * 1 for warm-up heater
-
-                zone (int)
-                    * Control loop zone to configure. Options are:
-                        * 1 - 10
-
-                settings (Model372ControlLoopZoneSettings)
-                    * An object of the Model372ControlLoopZoneSettings with the variable set to
-                        configure the desired settings.
+                output_channel (int):
+                    Channel of the heater being queried. Options are: 0 for sample heater, or 1 for warm-up heater.
+                zone (int):
+                    Control loop zone to configure. Options are: 1 - 10.
+                settings (Model372ControlLoopZoneSettings):
+                    An object of the Model372ControlLoopZoneSettings with the variable set to
+                    configure the desired settings.
 
         """
         # Use if statement to correctly interpret range variable
         if output_channel == 0:
             heater_range = format(settings.heater_range)
         else:
             heater_range = int(settings.heater_range)
@@ -1755,23 +1722,22 @@
                          f"{str(int(settings.relay_1))},{str(int(settings.relay_2))}")
         self.command(command_string)
 
     def get_reading_status(self, input_channel):
         """Returns any flags raised during a measurement reading.
 
             Args:
-                input_channel (str or int)
-                    * The input whose reading status is being queried. Options are:
-                        * 1 - 16
-                        * "A" (control input)
+                input_channel (str or int):
+                    The input whose reading status is being queried. Options are:
+                    1 - 16, or "A" (control input).
 
             Returns:
-                bit_states (dict)
-                    * Dictionary containing the names of the flag and a boolean value corresponding to
-                        if the flag is raised or not.
+                bit_states (dict):
+                    Dictionary containing the names of the flag and a boolean value corresponding to
+                    if the flag is raised or not.
 
         """
         integer_representation = int(self.query(f"RDGST? {str(input_channel)}"))
         bit_states = Model372ReadingStatusRegister.from_integer(integer_representation)
         return bit_states
```

### Comparing `lakeshore-1.6.1/lakeshore/model_425.py` & `lakeshore-1.7.0/lakeshore/model_350.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Implements functionality unique to the Lake Shore Model 425 Gaussmeter"""
+"""Implements functionality unique to the Lake Shore Model 350 cryogenic temperature controller."""
 import serial
 
 from .generic_instrument import GenericInstrument
 
 
-class Model425(GenericInstrument):
-    """A class object representing the Lake Shore Model 425 Gaussmeter"""
+class Model350(GenericInstrument):
+    """A class object representing the Lake Shore Model 350 cryogenic temperature controller."""
 
-    vid_pid = [(0x1FB9, 0x0401)]
+    vid_pid = [(0x1FB9, 0x0302)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=57600,
                  data_bits=7,
                  stop_bits=1,
```

### Comparing `lakeshore-1.6.1/lakeshore/model_643.py` & `lakeshore-1.7.0/lakeshore/model_643.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Implements functionality unique to the Lake Shore Model 643 electromagnet magnet power supply"""
+"""Implements functionality unique to the Lake Shore Model 643 electromagnet magnet power supply."""
 import serial
 
 from .generic_instrument import GenericInstrument
 
 
 class Model643(GenericInstrument):
-    """A class object representing the Lake Shore Model 643 electromagnet magnet power supply"""
+    """A class object representing the Lake Shore Model 643 electromagnet magnet power supply."""
 
     vid_pid = [(0x1FB9, 0x0601)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=57600,
```

### Comparing `lakeshore-1.6.1/lakeshore/requires_firmware_version.py` & `lakeshore-1.7.0/lakeshore/requires_firmware_version.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import functools
 from packaging.version import Version
 
 from lakeshore.xip_instrument import XIPInstrumentException
 
 
 def requires_firmware_version(required_version):
-    """Decorator for raising an error when the instrument firmware
-    is not up to date with the function's required version."""
+    """Decorator for raising an error when the instrument firmware is not up-to-date with required version."""
 
     def decorator_version_check(func):
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
             # Raise an error if the instrument version is earlier than the required version.
-            if Version(required_version) > Version(self.firmware_version):
+            if Version(required_version) > Version(self.firmware_version.split('-')[0]):
                 raise XIPInstrumentException(func.__name__ + ' requires instrument firmware version ' +
                                              str(required_version) +
                                              ' or later. Please update your instrument.')
 
             value = func(self, *args, **kwargs)
 
             return value
```

### Comparing `lakeshore-1.6.1/lakeshore/ssm_base_module.py` & `lakeshore-1.7.0/lakeshore/ssm_base_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Implements the BaseModule class used with the Measure and Source Modules of the M81."""
 
 from lakeshore.xip_instrument import RegisterBase
 
 
 class SSMSystemModuleQuestionableRegister(RegisterBase):
-    """Class object representing the questionable status register of a module"""
+    """Class object representing the questionable status register of a module."""
 
     bit_names = [
         "read_error",
         "unrecognized_pod_error",
         "port_direction_error",
         "factory_calibration_failure",
         "self_calibration_failure"
@@ -25,14 +25,14 @@
         self.unrecognized_pod_error = unrecognized_pod_error
         self.port_direction_error = port_direction_error
         self.factory_calibration_failure = factory_calibration_failure
         self.self_calibration_failure = self_calibration_failure
 
 
 class BaseModule:
-    """Class for interaction with a specific channel, not specific to source or measure"""
+    """Class for interaction with a specific channel, not specific to source or measure."""
 
     def __init__(self, module_number, device):
         self.module_number = module_number
         self.device = device
         self.questionable_register = SSMSystemModuleQuestionableRegister
         self.firmware_version = self.device.firmware_version
```

### Comparing `lakeshore-1.6.1/lakeshore/ssm_measure_module.py` & `lakeshore-1.7.0/lakeshore/ssm_measure_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 from warnings import warn
 from lakeshore.xip_instrument import RegisterBase
 from lakeshore.ssm_base_module import SSMSystemModuleQuestionableRegister, BaseModule
 
 
 class SSMSystemMeasureModuleOperationRegister(RegisterBase):
-    """Class object representing the operation status register of a measure module"""
+    """Class object representing the operation status register of a measure module."""
 
     bit_names = [
         "overload",
         "settling",
         "unlocked"
     ]
 
@@ -22,242 +22,258 @@
             unlocked):
         self.overload = overload
         self.settling = settling
         self.unlocked = unlocked
 
 # pylint: disable=R0904
 class MeasureModule(BaseModule):
-    """Class for interaction with a specific measure channel of the M81 instrument"""
+    """Class for interaction with a specific measure channel of the M81 instrument."""
 
     def get_name(self):
-        """Returns the user-settable name of the module"""
+        """Returns the user-settable name of the module."""
 
         return self.device.query(f'SENSe{self.module_number}:NAME?').strip('\"')
 
     def set_name(self, new_name):
-        """Set the name of the module"""
+        """Set the name of the module."""
 
         self.device.command(f'SENSe{self.module_number}:NAME "{new_name}"')
 
     def get_notes(self):
-        """Returns the user-settable notes of the module"""
+        """Returns the user-settable notes of the module."""
 
         return self.device.query(f'SENSe{self.module_number}:NOTes?').strip('\"')
 
     def set_notes(self, new_note):
-        """Set the notes of the module"""
+        """Set the notes of the module."""
 
         self.device.command(f'SENSe{self.module_number}:NOTes "{new_note}"')
 
     def get_model(self):
-        """Returns the model of the module (i.e. VM-10)"""
+        """Returns the model of the module (i.e. VM-10)."""
 
         return self.device.query(f'SENSe{self.module_number}:MODel?').strip('\"')
 
     def get_serial(self):
-        """Returns the serial number of the module (i.e. LSA1234)"""
+        """Returns the serial number of the module (i.e. LSA1234)."""
 
         return self.device.query(f'SENSe{self.module_number}:SERial?').strip('\"')
 
     def get_hw_version(self):
-        """Returns the hardware version of the module"""
+        """Returns the hardware version of the module."""
 
         return int(self.device.query(f'SENSe{self.module_number}:HWVersion?'))
 
     def get_self_cal_status(self):
-        """Returns the status of the last self calibration of the module"""
+        """Returns the status of the last self calibration of the module."""
 
         return self.device.query(f'SENSe{self.module_number}:SCALibration:STATus?')
 
     def run_self_cal(self):
-        """Run a self calibration for the module"""
+        """Run a self calibration for the module."""
 
         self.device.command(f'SENSe{self.module_number}:SCALibration:RUN')
 
     def reset_self_cal(self):
-        """Restore factory self calibration for the module"""
+        """Restore factory self calibration for the module."""
 
         self.device.command(f'SENSe{self.module_number}:SCALibration:RESet')
 
     def get_averaging_time(self):
         """Returns the averaging time of the module in Power Line Cycles. Not relevant in lock-in mode."""
 
         return float(self.device.query(f'SENSe{self.module_number}:NPLCycles?'))
 
     def set_averaging_time(self, nplc):
         """Sets the averaging time of the module. Not relevant in lock-in mode.
 
             Args:
                 nplc (float):
-                    The new number of power line cycles to average
+                    The new number of power line cycles to average.
         """
 
         self.device.command(f'SENSe{self.module_number}:NPLCycles {float(nplc)}')
 
     def get_mode(self):
         """Returns the measurement mode of the module. 'DC', 'AC', or 'LIA'."""
 
         return self.device.query(f'SENSe{self.module_number}:MODE?')
 
     def set_mode(self, mode):
-        """Sets the measurement mode of the module
+        """Sets the measurement mode of the module.
 
             Args:
                 mode (str):
-                    The new measurement mode ('DC', 'AC', or 'LIA')
+                    The new measurement mode ('DC', 'AC', or 'LIA').
         """
 
         self.device.command(f'SENSe{self.module_number}:MODE {mode}')
 
     def get_coupling(self):
         """Return input coupling of the module. 'AC' or 'DC'."""
 
         return self.device.query(f'SENSe{self.module_number}:COUPling?')
 
     def set_coupling(self, coupling):
-        """Sets the input coupling of the module
+        """Sets the input coupling of the module.
 
             Args:
                 coupling (str):
-                    The new input coupling ('AC' or 'DC')
+                    The new input coupling ('AC' or 'DC').
         """
 
         self.device.command(f'SENSe{self.module_number}:COUPling {coupling}')
 
     def use_ac_coupling(self):
-        """Sets the input coupling of the module to 'AC'"""
+        """Sets the input coupling of the module to 'AC'."""
 
         self.set_coupling('AC')
 
     def use_dc_coupling(self):
-        """Sets the input coupling of the module to 'DC'"""
+        """Sets the input coupling of the module to 'DC'."""
 
         self.set_coupling('DC')
 
     def get_input_configuration(self):
         """Returns the input configuration of the module. 'AB', 'A', or 'GROUND'."""
         return self.device.query(f'SENSe{self.module_number}:CONFiguration?')
 
     def set_input_configuration(self, input_configuration):
-        """Sets the input configuration of the module
+        """Sets the input configuration of the module.
 
             Args:
                 input_configuration (str):
-                    The new input configuration ('AB', 'A', or 'GROUND')
+                    The new input configuration ('AB', 'A', or 'GROUND').
         """
 
         self.device.command(f'SENSe{self.module_number}:CONFiguration {input_configuration}')
 
     def enable_bias_voltage(self):
-        """Enables the bias voltage applied to the amplifier"""
+        """Enables the bias voltage applied to the amplifier."""
 
         self.device.command(f'SENSe{self.module_number}:BIAS:STATe 1')
 
     def disable_bias_voltage(self):
-        """Disables the bias voltage applied to the amplifier"""
+        """Disables the bias voltage applied to the amplifier."""
 
         self.device.command(f'SENSe{self.module_number}:BIAS:STATe 0')
 
     def get_bias_voltage_enabled(self):
-        """Return whether the bias voltage is enabled"""
+        """Return whether the bias voltage is enabled."""
 
         return bool(int(self.device.query(f'SENSe{self.module_number}:BIAS:STATe?')))
 
     def get_bias_voltage(self):
-        """Return the bias voltage applied on the amplifier input in Volts"""
+        """Return the bias voltage applied on the amplifier input in Volts."""
 
         return float(self.device.query(f'SENSe{self.module_number}:BIAS:VOLTage:DC?'))
 
     def set_bias_voltage(self, bias_voltage):
-        """Sets the bias voltage applied on the amplifier input
+        """Sets the bias voltage applied on the amplifier input.
 
             Args:
                 bias_voltage (float):
-                    The new bias voltage in Volts
+                    The new bias voltage in Volts.
         """
 
         self.device.command(f'SENSe{self.module_number}:BIAS:VOLTage:DC {str(bias_voltage)}')
 
     def get_filter_state(self):
-        """Returns whether the hardware filter is engaged"""
+        """Returns whether the hardware filter is engaged."""
 
         return bool(int(self.device.query(f'SENSe{self.module_number}:FILTer:STATe?')))
 
     def get_lowpass_corner_frequency(self):
-        """Returns the low pass filter cuttoff frequency. 'NONE', 'F10', 'F30', 'F100', 'F300', 'F1000', 'F3000', or 'F10000'."""
+        """Returns the low pass filter cutoff frequency.
+
+            'NONE', 'F10', 'F30', 'F100', 'F300', 'F1000', 'F3000', or 'F10000'.
+        """
 
         return self.device.query(f'SENSe{self.module_number}:FILTer:LPASs:FREQuency?')
 
     def get_lowpass_rolloff(self):
-        """Returns the low pass filter roll-off. 'R6' or 'R12'."""
+        """Returns the low pass filter roll-off.
+
+            'R6' or 'R12'.
+        """
 
         return self.device.query(f'SENSe{self.module_number}:FILTer:LPASs:ATTenuation?')
 
     def get_highpass_corner_frequency(self):
-        """Returns the high pass filter cuttoff frequency. 'NONE', 'F10', 'F30', 'F100', 'F300', 'F1000', or 'F3000'."""
+        """Returns the high pass filter cutoff frequency.
+
+            'NONE', 'F10', 'F30', 'F100', 'F300', 'F1000', or 'F3000'.
+        """
 
         return self.device.query(f'SENSe{self.module_number}:FILTer:HPASs:FREQuency?')
 
     def get_highpass_rolloff(self):
-        """Returns the high pass filter roll-off. 'R6' or 'R12'."""
+        """Returns the high pass filter roll-off.
+
+            'R6' or 'R12'.
+        """
 
         return self.device.query(f'SENSe{self.module_number}:FILTer:HPASs:ATTenuation?')
 
     def get_gain_allocation_strategy(self):
-        """Returns the gain allocation strategy used for the hardware filter. 'NOISE', or 'RESERVE'."""
+        """Returns the gain allocation strategy used for the hardware filter.
+
+            'NOISE', or 'RESERVE'.
+        """
 
         return self.device.query(f'SENSe{self.module_number}:FILTer:OPTimization?')
 
     def set_gain_allocation_strategy(self, optimization_type):
-        """Sets the gain allocation strategy used for the hardware filter
+        """Sets the gain allocation strategy used for the hardware filter.
 
             Args:
                 optimization_type (str):
-                    The new optimization type ('NOISE', or 'RESERVE')
+                    The new optimization type ('NOISE', or 'RESERVE').
         """
 
         self.device.command(f'SENSe{self.module_number}:FILTer:OPTimization {optimization_type}')
 
     def configure_input_lowpass_filter(self, corner_frequency, rolloff='R12'):
-        """Configure the input low pass filter
+        """Configure the input low pass filter.
 
             Args:
                 corner_frequency (str):
-                    The low pass corner frequency ('NONE', 'F10', 'F30', 'F100', 'F300', 'F1000', 'F3000', or 'F10000'). F10 = 10 Hz, etc.
-
+                    The low pass corner frequency.
+                    ('NONE', 'F10', 'F30', 'F100', 'F300', 'F1000', 'F3000', or 'F10000'). F10 = 10 Hz, etc.
                 rolloff (str):
-                    The low pass roll-off ('R6' or 'R12'). R6 = 6 dB/Octave, R12 = 12 dB/Octave.
+                    The low pass roll-off.
+                    ('R6' or 'R12'). R6 = 6 dB/Octave, R12 = 12 dB/Octave.
         """
 
         self.device.command(f'SENSe{self.module_number}:FILTer:LPASs:FREQuency {corner_frequency}')
         self.device.command(f'SENSe{self.module_number}:FILTer:LPASs:ATTenuation {rolloff}')
         self.device.command(f'SENSe{self.module_number}:FILTer:STATe 1')
 
     def configure_input_highpass_filter(self, corner_frequency, rolloff='R12'):
-        """Configure the input high pass filter
+        """Configure the input high pass filter.
 
             Args:
                 corner_frequency (str):
-                    The high pass corner frequency ('NONE', 'F10', 'F30', 'F100', 'F300', 'F1000', or 'F3000'). F10 = 10 Hz, etc.
-
+                    The high pass corner frequency.
+                    ('NONE', 'F10', 'F30', 'F100', 'F300', 'F1000', or 'F3000'). F10 = 10 Hz, etc.
                 rolloff (str):
                     The high pass roll-off ('R6' or 'R12'). R6 = 6 dB/Octave, R12 = 12 dB/Octave.
         """
 
         self.device.command(f'SENSe{self.module_number}:FILTer:HPASs:FREQuency {corner_frequency}')
         self.device.command(f'SENSe{self.module_number}:FILTer:HPASs:ATTenuation {rolloff}')
         self.device.command(f'SENSe{self.module_number}:FILTer:STATe 1')
 
     def disable_input_filters(self):
-        """Disables the hardware filters"""
+        """Disables the hardware filters."""
 
         self.device.command(f'SENSe{self.module_number}:FILTer:STATe 0')
 
     def get_current_range(self):
-        """Returns the current range in Amps"""
+        """Returns the current range in Amps."""
 
         return float(self.device.query(f'SENSe{self.module_number}:CURRent:RANGe?'))
 
     def get_i_range(self):
         """
         Returns the current range in Amps
 
@@ -265,15 +281,15 @@
            Use get_current_range instead
         """
 
         warn('The get_i_range method is deprecated. Use get_current_range instead.', DeprecationWarning)
         return self.get_current_range()
 
     def get_current_autorange_status(self):
-        """Returns whether autoranging is enabled for the module"""
+        """Returns whether auto-ranging is enabled for the module."""
 
         return bool(int(self.device.query(f'SENSe{self.module_number}:CURRent:RANGe:AUTO?')))
 
     def get_i_autorange_status(self):
         """
         Returns whether autoranging is enabled for the module
 
@@ -281,15 +297,15 @@
            Use get_current_autorange_status instead
         """
 
         warn('The get_i_autorange_status method is deprecated. Use get_current_autorange_status instead.', DeprecationWarning)
         return self.get_current_autorange_status()
 
     def configure_current_range(self, autorange, max_level=None):
-        """Configure current ranging for the module
+        """Configure current ranging for the module.
 
             Args:
                 autorange (bool):
                     True to enable real time range decisions by the module. False for manual ranging.
 
                 max_level (float):
                     The largest current that needs to be measured by the module in Amps.
@@ -310,39 +326,37 @@
 
         .. deprecated:: 1.5.4
            Use configure_current_range instead
 
             Args:
                 autorange (bool):
                     True to enable real time range decisions by the module. False for manual ranging.
-
                 max_level (float):
                     The largest current that needs to be measured by the module in Amps.
         """
 
         warn('The configure_i_range method is deprecated. Use configure_current_range instead.', DeprecationWarning)
         self.configure_current_range(autorange, max_level)
 
     def get_voltage_range(self):
-        """Returns the voltage range in Volts"""
+        """Returns the voltage range in Volts."""
 
         return float(self.device.query(f'SENSe{self.module_number}:VOLTage:RANGe?'))
 
     def get_voltage_autorange_status(self):
-        """Returns whether autoranging is enabled for the module"""
+        """Returns whether auto-ranging is enabled for the module."""
 
         return bool(int(self.device.query(f'SENSe{self.module_number}:VOLTage:RANGe:AUTO?')))
 
     def configure_voltage_range(self, autorange, max_level):
-        """Configure voltage ranging for the module
+        """Configure voltage ranging for the module.
 
             Args:
                 autorange (bool):
                     True to enable real time range decisions by the module. False for manual ranging.
-
                 max_level (float):
                     The largest voltage that needs to be measured by the module in Volts.
         """
 
         if autorange:
             if max_level is not None:
                 raise ValueError('If autorange is selected, a manual range cannot be specified.')
@@ -364,101 +378,102 @@
                 reference_source (str):
                     The new reference source ('S1', 'S2', 'S3', 'RIN')
         """
 
         self.device.command(f'SENSe{self.module_number}:LIA:RSOurce {reference_source}')
 
     def get_reference_harmonic(self):
-        """Returns the lock-in reference harmonic"""
+        """Returns the lock-in reference harmonic."""
 
         return int(self.device.query(f'SENSe{self.module_number}:LIA:DHARmonic?'))
 
     def set_reference_harmonic(self, harmonic):
-        """Sets the lock-in reference harmonic
+        """Sets the lock-in reference harmonic.
 
             Args:
                 harmonic (int):
-                    The new reference harmonic. 1 is the fundamental frequency, 2 is twice the fundamental frequency, etc.
+                    The new reference harmonic.
+                    1 is the fundamental frequency, 2 is twice the fundamental frequency, etc.
         """
 
         self.device.command(f'SENSe{self.module_number}:LIA:DHARmonic {str(harmonic)}')
 
     def get_reference_phase_shift(self):
-        """Returns the lock-in reference phase shift in degrees"""
+        """Returns the lock-in reference phase shift in degrees."""
 
         return float(self.device.query(f'SENSe{self.module_number}:LIA:DPHase?'))
 
     def set_reference_phase_shift(self, phase_shift):
-        """Sets the lock-in reference phase shift
+        """Sets the lock-in reference phase shift.
 
             Args:
                 phase_shift (float):
-                    The new reference phase shift in degrees
+                    The new reference phase shift in degrees.
         """
         self.device.command(f'SENSe{self.module_number}:LIA:DPHase {str(phase_shift)}')
 
     def auto_phase(self):
-        """Executes a one time adjustment of the reference phase shift such that the present phase measurement is zero."""
+        """Executes a one time adjustment of the reference phase shift so that the present phase measurement is zero."""
 
         self.device.command(f'SENSe{self.module_number}:LIA:DPHase:AUTO')
 
     def get_lock_in_time_constant(self):
-        """Returns the lock-in time constant in seconds"""
+        """Returns the lock-in time constant in seconds."""
 
         return float(self.device.query(f'SENSe{self.module_number}:LIA:TIMEconstant?'))
 
     def set_lock_in_time_constant(self, time_constant):
-        """Sets the lock-in time constant
+        """Sets the lock-in time constant.
 
             Args:
                 time_constant (float):
-                    The new time constant in seconds
+                    The new time constant in seconds.
         """
         self.device.command(f'SENSe{self.module_number}:LIA:TIMEconstant {str(time_constant)}')
 
     def get_lock_in_settle_time(self, settle_percent=0.01):
-        """Returns the lock-in settle time in seconds
+        """Returns the lock-in settle time in seconds.
 
             Args:
-                settle_percent (float)
-                    The desired percent signal has settled to in percent
-                    A value of `0.1` is interpreted as 0.1 %
+                settle_percent (float):
+                    The desired percent signal has settled to in percent.
+                    A value of `0.1` is interpreted as 0.1 %.
         """
         return float(self.device.query(f'SENSe{self.module_number}:LIA:STIMe? {str(settle_percent)}'))
 
     def get_lock_in_equivalent_noise_bandwidth(self):
-        """Returns the equivalent noise bandwidth (ENBW) in Hz"""
+        """Returns the equivalent noise bandwidth (ENBW) in Hz."""
         return float(self.device.query(f'SENSe{self.module_number}:LIA:ENBW?'))
 
     def get_lock_in_rolloff(self):
         """Returns the lock-in PSD output filter roll-off for the present module. 'R6', 'R12', 'R18' or 'R24'."""
 
         return self.device.query(f'SENSe{self.module_number}:LIA:ROLLoff?')
 
     def set_lock_in_rolloff(self, rolloff):
-        """Sets the lock-in PSD output filter roll-off
+        """Sets the lock-in PSD output filter roll-off.
 
             Args:
                 rolloff (str):
-                    The new PSD output filter roll-off ('R6', 'R12', 'R18' or 'R24')
+                    The new PSD output filter roll-off ('R6', 'R12', 'R18' or 'R24').
         """
 
         self.device.command(f'SENSe{self.module_number}:LIA:ROLLoff {rolloff}')
 
     def get_lock_in_iir_state(self):
-        """Returns the state of the lock-in PSD output IIR filter"""
+        """Returns the state of the lock-in PSD output IIR filter."""
 
         return bool(int(self.device.query(f'SENSe{self.module_number}:LIA:IIR:STATe?')))
 
     def set_lock_in_iir_state(self, state):
-        """Sets the state of the lock-in PSD output IIR filter
+        """Sets the state of the lock-in PSD output IIR filter.
 
             Args:
                 state (bool):
-                    The new state of the PSD output IIR filter
+                    The new state of the PSD output IIR filter.
         """
 
         self.device.command(f'SENSe{self.module_number}:LIA:IIR:STATe {str(int(state))}')
 
     def enable_lock_in_iir(self):
         """Sets the state of the lock-in PSD output IIR filter to True."""
 
@@ -466,24 +481,24 @@
 
     def disable_lock_in_iir(self):
         """Sets the state of the lock-in PSD output IIR filter to False."""
 
         self.set_lock_in_iir_state(False)
 
     def get_lock_in_fir_state(self):
-        """Returns the state of the lock-in PSD output FIR filter"""
+        """Returns the state of the lock-in PSD output FIR filter."""
 
         return bool(int(self.device.query(f'SENSe{self.module_number}:LIA:FIR:STATe?')))
 
     def set_lock_in_fir_state(self, state):
-        """Sets the state of the lock-in PSD output FIR filter
+        """Sets the state of the lock-in PSD output FIR filter.
 
             Args:
                 state (bool):
-                    The new state of the PSD output FIR filter
+                    The new state of the PSD output FIR filter.
         """
 
         self.device.command(f'SENSe{self.module_number}:LIA:FIR:STATe {str(int(state))}')
 
     def enable_lock_in_fir(self):
         """Sets the state of the lock-in PSD output FIR filter to True."""
 
@@ -491,377 +506,390 @@
 
     def disable_lock_in_fir(self):
         """Sets the state of the lock-in PSD output FIR filter to False."""
 
         self.set_lock_in_fir_state(False)
 
     def get_lock_in_fir_cycles(self):
-        """Returns the number of FIR cycles"""
+        """Returns the number of FIR cycles."""
 
         return int(self.device.query(f'SENSe{self.module_number}:LIA:FIR:CYCLes?'))
 
     def set_lock_in_fir_cycles(self, cycles):
-        """Sets the number of FIR cycles
+        """Sets the number of FIR cycles.
 
             Args:
                 cycles (int):
-                    The desired number of FIR cycles, between 1 and 100
+                    The desired number of FIR cycles, between 1 and 100.
         """
 
         self.device.command(f'SENSe{self.module_number}:LIA:FIR:CYCLes {str(int(cycles))}')
 
     def setup_dc_measurement(self, nplc=1):
-        """Setup the module for DC measurement
+        """Set up the module for DC measurement.
 
             Args:
                 nplc (float):
-                    The new number of power line cycles to average
+                    The new number of power line cycles to average.
         """
 
         self.set_mode('DC')
         self.set_averaging_time(nplc)
 
     def setup_ac_measurement(self, nplc=1):
-        """Setup the module for DC measurement
+        """Set up the module for DC measurement.
 
             Args:
                 nplc (float):
-                    The new number of power line cycles to average
+                    The new number of power line cycles to average.
         """
 
         self.set_mode('AC')
         self.set_averaging_time(nplc)
 
     def setup_lock_in_measurement(self,
                                   reference_source,
                                   time_constant,
                                   rolloff='R24',
                                   reference_phase_shift=0.0,
                                   reference_harmonic=1,
                                   use_fir=True):
-        """Setup the module for lock-in measurement
+        """Set up the module for lock-in measurement.
 
             Args:
                 reference_source (str):
-                    Lock-in reference source ('S1', 'S2', 'S3', 'RIN')
-
+                    Lock-in reference source ('S1', 'S2', 'S3', 'RIN').
                 time_constant (float):
-                    Time constant in seconds
-
+                    Time constant in seconds.
                 rolloff (str):
-                    Lock-in PSD output filter roll-off ('R6', 'R12', 'R18' or 'R12')
-
+                    Lock-in PSD output filter roll-off ('R6', 'R12', 'R18' or 'R12').
                 reference_phase_shift (float):
-                    Lock-in reference phase shift in degrees
-
+                    Lock-in reference phase shift in degrees.
                 reference_harmonic (int):
-                    Lock-in reference harmonic. 1 is the fundamental frequency, 2 is twice the fundamental frequency, etc.
-
+                    Lock-in reference harmonic. 1 is the fundamental frequency, 2 is twice the fundamental frequency,
+                    etc.
                 use_fir (bool):
-                    Enable or disable the PSD output FIR filter
+                    Enable or disable the PSD output FIR filter.
         """
 
         self.set_mode('LIA')
         self.set_reference_source(reference_source)
         self.set_lock_in_time_constant(time_constant)
         self.set_lock_in_rolloff(rolloff)
         self.set_reference_phase_shift(reference_phase_shift)
         self.set_reference_harmonic(reference_harmonic)
         self.set_lock_in_fir_state(use_fir)
 
     def zero_relative_baseline(self):
-        """Sets the present measurement as the baseline value for calculating relative readings"""
+        """Sets the present measurement as the baseline value for calculating relative readings."""
 
         self.device.command(f'SENSe{self.module_number}:RELative:ZERO')
 
     def set_relative_baseline(self, baseline):
-        """Sets the relative baseline"""
+        """Sets the relative baseline."""
 
         self.device.command(f'SENSe{self.module_number}:RELative:BASEline {str(baseline)}')
 
     def get_relative_baseline(self):
-        """Returns the relative baseline"""
+        """Returns the relative baseline."""
 
         return float(self.device.query(f'SENSe{self.module_number}:RELative:BASEline?'))
 
     def get_multiple(self, *data_sources):
         """This function is deprecated. Use fetch_multiple() instead."""
 
         return self.fetch_multiple(*data_sources)
 
     def get_dc(self):
-        """Returns the DC measurement in module units"""
+        """Returns the DC measurement in module units."""
 
         return float(self.device.query(f'READ:SENSe{self.module_number}:DC?'))
 
     def get_dc_relative(self):
-        """Returns the relative DC measurement in module units"""
+        """Returns the relative DC measurement in module units."""
 
         return float(self.device.query(f'READ:SENSe{self.module_number}:DC:RELative?'))
 
     def get_dc_minimum(self):
-        """Returns the minimum DC indication in module units"""
+        """Returns the minimum DC indication in module units."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:DC?'))
 
     def get_dc_maximum(self):
-        """Returns the maximum DC indication in module units"""
+        """Returns the maximum DC indication in module units."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:DC?'))
 
     def get_rms(self):
-        """Returns the RMS measurement in module units"""
+        """Returns the RMS measurement in module units."""
 
         return float(self.device.query(f'READ:SENSe{self.module_number}:RMS?'))
 
     def get_rms_relative(self):
-        """Returns the relative RMS measurement in module units"""
+        """Returns the relative RMS measurement in module units."""
 
         return float(self.device.query(f'READ:SENSe{self.module_number}:RMS:RELative?'))
 
     def get_rms_minimum(self):
-        """Returns the minimum RMS indication in module units"""
+        """Returns the minimum RMS indication in module units."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:RMS?'))
 
     def get_rms_maximum(self):
-        """Returns the maximum RMS indication in module units"""
+        """Returns the maximum RMS indication in module units."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:RMS?'))
 
     def get_peak_to_peak(self):
-        """Returns the peak to peak measurement in module units"""
+        """Returns the peak to peak measurement in module units."""
 
         return float(self.device.query(f'READ:SENSe{self.module_number}:PTPeak?'))
 
     def get_peak_to_peak_minimum(self):
-        """Returns the minimum peak to peak indication in module units"""
+        """Returns the minimum peak to peak indication in module units."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:PTPeak?'))
 
     def get_peak_to_peak_maximum(self):
-        """Returns the maximum peak to peak indication in module units"""
+        """Returns the maximum peak to peak indication in module units."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:PTPeak?'))
 
     def get_positive_peak(self):
-        """Returns the positive peak measurement in module units"""
+        """Returns the positive peak measurement in module units."""
 
         return float(self.device.query(f'READ:SENSe{self.module_number}:PPEak?'))
 
     def get_positive_peak_minimum(self):
-        """Returns the minimum positive peak indication in module units"""
+        """Returns the minimum positive peak indication in module units."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:PPEak?'))
 
     def get_positive_peak_maximum(self):
-        """Returns the maximum positive peak indication in module units"""
+        """Returns the maximum positive peak indication in module units."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:PPEak?'))
 
     def get_negative_peak(self):
-        """Returns the negative peak measurement in module units"""
+        """Returns the negative peak measurement in module units."""
 
         return float(self.device.query(f'READ:SENSe{self.module_number}:NPEak?'))
 
     def get_negative_peak_minimum(self):
-        """Returns the minimum negative peak indication in module units"""
+        """Returns the minimum negative peak indication in module units."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:NPEak?'))
 
     def get_negative_peak_maximum(self):
-        """Returns the maximum negative peak indication in module units"""
+        """Returns the maximum negative peak indication in module units."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:NPEak?'))
 
     def get_lock_in_x(self):
-        """Returns the present X measurement from the lock-in"""
+        """Returns the present X measurement from the lock-in."""
 
         return float(self.device.query(f'FETCh:SENSe{self.module_number}:LIA:X?'))
 
     def get_lock_in_x_minimum(self):
-        """Returns the minimum X indication from the lock in"""
+        """Returns the minimum X indication from the lock in."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:LIA:X?'))
 
     def get_lock_in_x_maximum(self):
-        """Returns the maximum X indication from the lock in"""
+        """Returns the maximum X indication from the lock in."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:LIA:X?'))
 
     def get_lock_in_y(self):
-        """Returns the present Y measurement from the lock-in"""
+        """Returns the present Y measurement from the lock-in."""
 
         return float(self.device.query(f'FETCh:SENSe{self.module_number}:LIA:Y?'))
 
     def get_lock_in_y_minimum(self):
-        """Returns the minimum Y indication from the lock in"""
+        """Returns the minimum Y indication from the lock in."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:LIA:Y?'))
 
     def get_lock_in_y_maximum(self):
-        """Returns the maximum Y indication from the lock in"""
+        """Returns the maximum Y indication from the lock in."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:LIA:Y?'))
 
     def get_lock_in_r(self):
-        """Returns the present magnitude measurement from the lock-in"""
+        """Returns the present magnitude measurement from the lock-in."""
 
         return float(self.device.query(f'FETCh:SENSe{self.module_number}:LIA:R?'))
 
     def get_lock_in_r_minimum(self):
-        """Returns the minimum magnitude indication from the lock in"""
+        """Returns the minimum magnitude indication from the lock in."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:LIA:R?'))
 
     def get_lock_in_r_maximum(self):
-        """Returns the maximum magnitude indication from the lock in"""
+        """Returns the maximum magnitude indication from the lock in."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:LIA:R?'))
 
     def get_lock_in_theta(self):
-        """Returns the present angle measurement from the lock-in"""
+        """Returns the present angle measurement from the lock-in."""
 
         return float(self.device.query(f'FETCh:SENSe{self.module_number}:LIA:THETa?'))
 
     def get_lock_in_theta_minimum(self):
-        """Returns the minimum angle indication from the lock in"""
+        """Returns the minimum angle indication from the lock in."""
 
         return float(self.device.query(f'STATistic:MINimum:SENSe{self.module_number}:LIA:THETa?'))
 
     def get_lock_in_theta_maximum(self):
-        """Returns the maximum angle indication from the lock in"""
+        """Returns the maximum angle indication from the lock in."""
 
         return float(self.device.query(f'STATistic:MAXimum:SENSe{self.module_number}:LIA:THETa?'))
 
     def get_lock_in_frequency(self):
-        """Returns the present detected frequency from the Phase Locked Loop (PLL)"""
+        """Returns the present detected frequency from the Phase Locked Loop (PLL)."""
 
         return float(self.device.query(f'FETCh:SENSe{self.module_number}:LIA:FREQuency?'))
 
     def get_pll_lock_status(self):
         """Returns the present lock status of the PLL. True if locked, False if unlocked."""
 
         return bool(int(self.device.query(f'FETCh:SENSe{self.module_number}:LIA:LOCK?')))
 
     def get_present_questionable_status(self):
-        """Returns the names of the questionable status register bits and their values"""
+        """Returns the names of the questionable status register bits and their values."""
 
         response = self.device.query(f'STATus:QUEStionable:SENSe{self.module_number}:CONDition?', check_errors=False)
         status_register = SSMSystemModuleQuestionableRegister.from_integer(response)
 
         return status_register
 
     def get_questionable_events(self):
         """Returns the names of questionable event status register bits that are currently high.
-        The event register is latching and values are reset when queried."""
+
+            The event register is latching and values are reset when queried.
+        """
 
         response = self.device.query(f'STATus:QUEStionable:SENSe{self.module_number}:EVENt?', check_errors=False)
         status_register = SSMSystemModuleQuestionableRegister.from_integer(response)
 
         return status_register
 
     def get_questionable_event_enable_mask(self):
         """Returns the names of the questionable event enable register bits and their values.
-        These values determine which questionable bits propagate to the questionable event register."""
+
+            These values determine which questionable bits propagate to the questionable event register.
+        """
 
         response = self.device.query(f'STATus:QUEStionable:SENSe{self.module_number}:ENABle?', check_errors=False)
         status_register = SSMSystemModuleQuestionableRegister.from_integer(response)
 
         return status_register
 
     def set_questionable_event_enable_mask(self, register_mask):
         """Configures the values of the questionable event enable register bits.
-        These values determine which questionable bits propagate to the questionable event register.
+
+            These values determine which questionable bits propagate to the questionable event register.
 
             Args:
                 register_mask ([Instrument]QuestionableRegister):
                     An instrument specific QuestionableRegister class object with all bits configured true or false.
         """
 
         integer_representation = register_mask.to_integer()
         self.device.command(f'STATus:QUEStionable:SENSe{self.module_number}:ENABle {integer_representation}', check_errors=False)
 
     def get_present_operation_status(self):
-        """Returns the names of the operation status register bits and their values"""
+        """Returns the names of the operation status register bits and their values."""
 
         response = self.device.query(f'STATus:OPERation:SENSe{self.module_number}:CONDition?', check_errors=False)
         status_register = SSMSystemMeasureModuleOperationRegister.from_integer(response)
 
         return status_register
 
     def get_operation_events(self):
         """Returns the names of operation event status register bits that are currently high.
-        The event register is latching and values are reset when queried."""
+
+            The event register is latching and values are reset when queried.
+        """
 
         response = self.device.query(f'STATus:OPERation:SENSe{self.module_number}:EVENt?', check_errors=False)
         status_register = SSMSystemMeasureModuleOperationRegister.from_integer(response)
 
         return status_register
 
     def get_operation_event_enable_mask(self):
         """Returns the names of the operation event enable register bits and their values.
-        These values determine which operation bits propagate to the operation event register."""
+
+            These values determine which operation bits propagate to the operation event register.
+        """
 
         response = self.device.query(f'STATus:OPERation:SENSe{self.module_number}:ENABle?', check_errors=False)
         status_register = SSMSystemMeasureModuleOperationRegister.from_integer(response)
 
         return status_register
 
     def set_operation_event_enable_mask(self, register_mask):
         """Configures the values of the operation event enable register bits.
-        These values determine which operation bits propagate to the operation event register.
+
+            These values determine which operation bits propagate to the operation event register.
 
             Args:
                 register_mask ([Instrument]OperationRegister):
                     An instrument specific OperationRegister class object with all bits configured true or false.
         """
 
         integer_representation = register_mask.to_integer()
         self.device.command(f'STATus:OPERation:SENSe{self.module_number}:ENABle {integer_representation}', check_errors=False)
 
     def get_identify_state(self):
         """Returns the identification state for the given pod."""
+
         response = bool(int(self.device.query(f'SENSe{self.module_number}:IDENtify?', check_errors=False)))
         return response
 
     def set_identify_state(self, state):
         """Sets the identification state for the given pod.
 
             Args:
                 state (bool):
-                    The desired state for the LED, 1 for identify, 0 for normal state
+                    The desired state for the LED, 1 for identify, 0 for normal state.
         """
+
         self.device.command(f'SENSe{self.module_number}:IDENtify {int(state)}', check_errors=False)
 
     def get_dark_mode_state(self):
-        """Returns the dark mode state for the given pod"""
+        """Returns the dark mode state for the given pod."""
+
         response = self.device.query(f'SENSe{self.module_number}:DMODe?', cherk_errors=False)
         return response
 
     def set_dark_mode_state(self, state):
         """Configures the dark mode state for the given pod.
 
             Args:
                 state (bool):
-                    The desired operation for the LED, 1 for normal mode, 0 for dark mode
+                    The desired operation for the LED, 1 for normal mode, 0 for dark mode.
         """
+
         self.device.command(f'SENSe{self.module_number}:DMODe {state}', check_errors=False)
 
     def get_frequency_range_threshold(self):
-        """Returns the frequency range threshold for the module. Frequency range threshold normalized to the -3 db
-           point. For example, a value of 0.1 means 10 % of the -3 db point.
+        """Returns the frequency range threshold for the module.
+
+            Frequency range threshold normalized to the -3 db point. For example, a value of 0.1 means 10 % of the
+            -3 db point.
         """
 
         return float(self.device.query(f'SENSe{self.module_number}:FRTHreshold?'))
 
     def set_frequency_range_threshold(self, threshold):
         """Sets the frequency range threshold for the specified module.
-        When the modules range is set to Auto, a range such that the frequency of the signal does not exceed the given
-        percentage of the bandwidth of the range will be chosen.
+
+            When the modules range is set to Auto, a range such that the frequency of the signal does not exceed the
+            given percentage of the bandwidth of the range will be chosen.
 
         Args:
             threshold (float):
                 Frequency range threshold normalized to the -3 db point with a valid range of 0.0 to 1.0.
                 For example, a value of 0.1 means 10 % of the -3 db point.
         """
 
@@ -897,66 +925,64 @@
 
     def get_resistance_source(self):
         """Returns the present source module being used to calculate resistance."""
 
         return self.device.query(f'CALCulate:SENSe{self.module_number}:RESistance:SOURce?')
 
     def reset_settings(self):
-        """Resets the settings for the specified module to their power on defaults.
-        """
+        """Resets the settings for the specified module to their power on defaults."""
 
         self.device.command(f'SENSe{self.module_number}:PRESet')
 
     def unload(self):
-        """Unloads the specified module.
-        """
+        """Unloads the specified module."""
 
         self.device.command(f'SENSe{self.module_number}:UNLoad')
 
     def get_load_state(self):
-        """Returns the loaded state for the specified module.
-        """
+        """Returns the loaded state for the specified module."""
 
         response = bool(int(self.device.query(f'SENSe{self.module_number}:LOAD?')))
         return response
 
     def fetch_multiple(self, *data_sources):
-        """Gets a list of the latest values corresponding to the input data sources for this module, and returns them
-        as soon as possible.
+        """Returns a list of the latest values corresponding to the input data sources for this module quickly
 
             Args:
-                data_sources (SSMSystemDataSourceMnemonic or str): Variable length list of data sources.
+                data_sources (SSMSystemDataSourceMnemonic or str):
+                    Variable length list of data sources.
 
             Returns:
-                Tuple of values corresponding to the given data sources for this module
+                Tuple of values corresponding to the given data sources for this module.
         """
 
         elements = [(data_source, self.module_number) for data_source in data_sources]
         return self.device.fetch_multiple(*elements)
 
     def read_multiple(self, *data_sources):
-        """Initiates measurement of new values corresponding to the input data sources for this module, and returns them
-        after the measurement is complete.
+        """Returns new values after measurement based on present input data source.
+
+            Initiates measurement of new values corresponding to the input data sources for this module and returns them
+            after the measurement is complete.
 
             Args:
-                data_sources (SSMSystemReadDataSourceMnemonic or str): Variable length list of data sources.
+                data_sources (SSMSystemReadDataSourceMnemonic or str):
+                    Variable length list of data sources.
 
             Returns:
-                Tuple of values corresponding to the given data sources for this module
+                Tuple of values corresponding to the given data sources for this module.
         """
 
         elements = [(data_source, self.module_number) for data_source in data_sources]
         return self.device.read_multiple(*elements)
 
     def get_self_cal_datetime(self):
-        """Returns the self calibration date and time for the specified module.
-        """
+        """Returns the self calibration date and time for the specified module."""
 
         response = self.device.query(f'SENSe{self.module_number}:SCALibration:DATE?').split(',')
         return datetime(int(response[0]), int(response[1]), int(response[2]), int(response[3]),int(response[4]), int(response[5]))
 
     def get_self_cal_temperature(self):
-        """Returns the self calibration temperature for the specified module.
-        """
+        """Returns the self calibration temperature for the specified module."""
 
         return float(self.device.query(f'SENSe{self.module_number}:SCALibration:TEMP?'))
```

### Comparing `lakeshore-1.6.1/lakeshore/ssm_settings_profiles.py` & `lakeshore-1.7.0/lakeshore/ssm_settings_profiles.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-"""Implements functionality unique to settings profiles"""
+"""Implements functionality unique to settings profiles."""
 
 import json
 
 
 class SettingsProfiles:
-    """Class for interaction with settings profiles"""
+    """Class for interaction with settings profiles."""
 
     def __init__(self, device):
         self.device = device
 
     def get_summary(self, name):
         """Returns a list containing a profile's description and module models.
 
         Args:
-            name (str): Name of the profile to query.
+            name (str):
+                Name of the profile to query.
         """
 
         response = self.device.query(f'PROFile:SUMMary? "{name}"')
 
         return [element.replace('"', '').strip() for element in response.split(',')]
 
     def create(self, name, description=''):
         """Create a new profile using the present instrument configuration.
 
         Args:
-            name (str): Unique name to give the profile.
-            description (str): Optional description of the profile.
+            name (str):
+                Unique name to give the profile.
+            description (str):
+                Optional description of the profile.
         """
 
         self.device.command(f'PROFile:CREAte "{name}", "{description}"')
 
     def get_list(self):
         """Returns a list of the saved profile names."""
 
@@ -39,83 +42,93 @@
 
         return [profile.strip('"') for profile in response.split(',')]
 
     def get_description(self, name):
         """Returns a profile's description.
 
         Args:
-            name (str): Name of the profile to get the description for.
+            name (str):
+                Name of the profile to get the description for.
         """
 
         return self.device.query(f'PROFile:DESCription? "{name}"').strip('"')
 
     def set_description(self, name, description):
         """Sets a profile's description. Any existing description will be overwritten.
 
         Args:
-            name (str): Name of the profile to get the description for.
-            description (str): The new description of the profile.
+            name (str):
+                Name of the profile to get the description for.
+            description (str):
+                The new description of the profile.
         """
 
         self.device.command(f'PROFile:DESCription "{name}","{description}"')
 
     def get_json(self, name):
         """Returns a JSON object of a given profile.
 
         Args:
-            name (str): Name of the profile.
+            name (str):
+                Name of the profile.
         """
 
         response = self.device.query(f'PROFile:JSON? "{name}"')
         json_string = response.strip('"').replace('""', '"')
         return json.loads(json_string)
 
     def rename(self, name, new_name):
         """Rename a profile. New name must be unique.
 
         Args:
-            name (str): The name of the profile to rename.
-            new_name (str): The new name of the profile.
+            name (str):
+                The name of the profile to rename.
+            new_name (str):
+                The new name of the profile.
         """
 
         self.device.command(f'PROFile:REName "{name}","{new_name}"')
 
     def update(self, name):
         """Update a profile with the present instrument configuration.
 
         Args:
-            name (str): The name of the profile to update.
+            name (str):
+                The name of the profile to update.
         """
 
         self.device.command(f'PROFile:UPDate "{name}"')
 
     def get_valid_for_restore(self, name):
         """Returns if a profile is valid to restore.
 
         Args:
-            name (str): The name of the profile to validate.
+            name (str):
+                The name of the profile to validate.
         """
 
         response = self.device.query(f'PROFile:RESTore:VALid? "{name}"')
         return bool(response)
 
     def restore(self, name):
         """Restore a profile.
 
         Args:
-            name (str): The name of the profile to restore.
+            name (str):
+                The name of the profile to restore.
         """
 
         self.device.command(f'PROFile:RESTore "{name}"')
 
     def delete(self, name):
-        """Delete a profile
+        """Delete a profile.
 
         Args:
-            name (str): The name of the profile to delete.
+            name (str):
+                The name of the profile to delete.
         """
 
         self.device.command(f'PROFile:DELete "{name}"')
 
     def delete_all(self):
         """Delete all profiles."""
```

### Comparing `lakeshore-1.6.1/lakeshore/ssm_source_module.py` & `lakeshore-1.7.0/lakeshore/ssm_source_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from lakeshore.xip_instrument import RegisterBase
 from lakeshore.ssm_base_module import SSMSystemModuleQuestionableRegister, BaseModule
 from lakeshore.requires_firmware_version import requires_firmware_version
 
 
 class SSMSystemSourceModuleOperationRegister(RegisterBase):
-    """Class object representing the operation status register of a source module"""
+    """Class object representing the operation status register of a source module."""
 
     bit_names = [
         "v_limit",
         "i_limit",
         "sweeping"
     ]
 
@@ -26,327 +26,326 @@
         self.v_limit = v_limit
         self.i_limit = i_limit
         self.sweeping = sweeping
 
 
 # pylint: disable=R0904
 class SourceModule(BaseModule):
-    """Class for interaction with a specific source channel of the M81 instrument"""
+    """Class for interaction with a specific source channel of the M81 instrument."""
 
     def get_multiple(self, *data_sources):
         r"""This function is deprecated. Use fetch_multiple() instead."""
 
         return self.fetch_multiple(*data_sources)
 
     def fetch_multiple(self, *data_sources):
-        r"""Gets a list of the latest values corresponding to the input data sources for this module, and returns them
-        as soon as possible.
+        r"""Gets a list of the latest values corresponding to the input data sources for this module.
 
         Args:
-            data_sources (SSMSystemDataSourceMnemonic or str): Variable length list of data sources.
+            data_sources (SSMSystemDataSourceMnemonic or str):
+                Variable length list of data sources.
 
         Returns:
-            Tuple of values corresponding to the given data sources for this module
+            Tuple of values corresponding to the given data sources for this module.
         """
 
         elements = [(data_source, self.module_number) for data_source in data_sources]
         return self.device.fetch_multiple(*elements)
 
     def get_name(self):
-        """Returns the user-settable name of the module"""
+        """Returns the user-settable name of the module."""
 
         return self.device.query(f'SOURce{self.module_number}:NAME?').strip('\"')
 
     def set_name(self, new_name):
-        """Set the name of the module"""
+        """Set the name of the module."""
 
         self.device.command(f'SOURce{self.module_number}:NAME "{new_name}"')
 
     def get_notes(self):
-        """Returns the user-settable notes of the module"""
+        """Returns the user-settable notes of the module."""
 
         return self.device.query(f'SOURce{self.module_number}:NOTes?').strip('\"')
 
     def set_notes(self, new_note):
-        """Set the notes of the module"""
+        """Set the notes of the module."""
 
         self.device.command(f'SOURce{self.module_number}:NOTes "{new_note}"')
 
     def get_model(self):
-        """Returns the model of the module (i.e. BCS-10)"""
+        """Returns the model of the module (i.e. BCS-10)."""
 
         return self.device.query(f'SOURce{self.module_number}:MODel?').strip('\"')
 
     def get_serial(self):
-        """Returns the serial number of the module (i.e. LSA1234)"""
+        """Returns the serial number of the module (i.e. LSA1234)."""
 
         return self.device.query(f'SOURce{self.module_number}:SERial?').strip('\"')
 
     def get_hw_version(self):
-        """Returns the hardware version of the module"""
+        """Returns the hardware version of the module."""
 
         return int(self.device.query(f'SOURce{self.module_number}:HWVersion?'))
 
     def get_self_cal_status(self):
-        """Returns the status of the last self calibration of the module"""
+        """Returns the status of the last self calibration of the module."""
 
         return self.device.query(f'SOURce{self.module_number}:SCALibration:STATus?')
 
     def run_self_cal(self):
-        """Run a self calibration for the module"""
+        """Run a self calibration for the module."""
 
         self.device.command(f'SOURce{self.module_number}:SCALibration:RUN')
 
     def reset_self_cal(self):
-        """Restore factory self calibration for the module"""
+        """Restore factory self calibration for the module."""
 
         self.device.command(f'SOURce{self.module_number}:SCALibration:RESet')
 
     def get_enable_state(self):
-        """Returns the output state of the module"""
+        """Returns the output state of the module."""
 
         return bool(int(self.device.query(f'SOURce{self.module_number}:STATe?')))
 
     def set_enable_state(self, state):
-        """Sets the enable state of the module
+        """Sets the enable state of the module.
 
             Args:
                 state (bool):
-                    The new output state
+                    The new output state.
         """
 
         self.device.command(f'SOURce{self.module_number}:STATe {str(int(state))}')
 
     def enable(self):
-        """Sets the enable state of the module to True"""
+        """Sets the enable state of the module to True."""
 
         self.set_enable_state(True)
 
     def disable(self):
-        """Sets the enable state of the module to False"""
+        """Sets the enable state of the module to False."""
 
         self.set_enable_state(False)
 
     def get_excitation_mode(self):
         """Returns the excitation mode of the module. 'CURRENT' or 'VOLTAGE'."""
 
         return self.device.ExcitationType(self.device.query(f'SOURce{self.module_number}:FUNCtion:MODE?'))
 
     def set_excitation_mode(self, excitation_mode):
-        """Sets the excitation mode of the module
+        """Sets the excitation mode of the module.
 
             Args:
                 excitation_mode (SSMSystem.ExcitationType):
-                    The new excitation mode ('CURRENT' or 'VOLTAGE')
+                    The new excitation mode ('CURRENT' or 'VOLTAGE').
         """
 
         if isinstance(excitation_mode, self.device.ExcitationType):
             mode = excitation_mode.name
         else:
             mode = excitation_mode
 
         self.device.command(f'SOURce{self.module_number}:FUNCtion:MODE {mode}')
 
     def go_to_current_mode(self):
-        """Sets the excitation mode of the module to 'CURRENT'"""
+        """Sets the excitation mode of the module to 'CURRENT'."""
 
         self.set_excitation_mode(self.device.ExcitationType.CURRENT)
 
     def go_to_voltage_mode(self):
-        """Sets the excitation mode of the module to 'VOLTAGE'"""
+        """Sets the excitation mode of the module to 'VOLTAGE'."""
 
         self.set_excitation_mode(self.device.ExcitationType.VOLTAGE)
 
     def get_shape(self):
         """Returns the signal shape of the module. 'DC' or 'SINUSOID'."""
 
         return self.device.query(f'SOURce{self.module_number}:FUNCtion:SHAPe?')
 
     def set_shape(self, shape):
-        """Sets the signal shape of the module
+        """Sets the signal shape of the module.
 
             Args:
                 shape (str):
-                    The new signal shape ('DC', 'SINUSOID', 'TRIANGLE', 'SQUARE')
+                    The new signal shape ('DC', 'SINUSOID', 'TRIANGLE', 'SQUARE').
         """
 
         self.device.command(f'SOURce{self.module_number}:FUNCtion:SHAPe {shape}')
 
     def get_frequency(self):
-        """Returns the excitation frequency of the module"""
+        """Returns the excitation frequency of the module."""
 
         return float(self.device.query(f'SOURce{self.module_number}:FREQuency?'))
 
     def set_frequency(self, frequency):
-        """Sets the excitation frequency of the module
+        """Sets the excitation frequency of the module.
 
             Args:
                 frequency (float):
-                    The new excitation frequency
+                    The new excitation frequency.
         """
         self.device.command(f'SOURce{self.module_number}:FREQuency {str(frequency)}')
 
     def get_sync_state(self):
         """Returns whether the source channel synchronization feature is engaged
 
-            If true, this channel will ignore its own frequency, and instead track the frequency of the synchronization source.
+            If true, this channel will ignore its own frequency, and instead track the frequency of the synchronization
+            source.
             If false, this channel will generate its own frequency.
         """
 
         return bool(int(self.device.query(f'SOURce{self.module_number}:SYNChronize:STATe?')))
 
     def get_sync_source(self):
-        """Returns the channel used for frequency synchronization"""
+        """Returns the channel used for frequency synchronization."""
 
         return self.device.query(f'SOURce{self.module_number}:SYNChronize:SOURce?')
 
     def get_sync_phase_shift(self):
-        """Returns the phase shift applied between the synchronization source and this channel"""
+        """Returns the phase shift applied between the synchronization source and this channel."""
 
         return float(self.device.query(f'SOURce{self.module_number}:SYNChronize:PHASe?'))
 
     def configure_sync(self, source, phase_shift, enable_sync=True):
-        """Configure the source channel synchronization feature
+        """Configure the source channel synchronization feature.
 
             Args:
                 source (str):
                     The channel used for synchronization ('S1', 'S2', 'S3', or 'RIN').
                     This channel will follow the frequency set for the specified channel.
-
                 phase_shift (float):
                     The phase shift applied between the synchronization source and this channel in degrees.
-
                 enable_sync (bool):
-                    If true, this channel will ignore its own frequency, and instead track the frequency of the synchronization source.
+                    If true, this channel will ignore its own frequency, and instead track the frequency of the
+                    synchronization source.
                     If false, this channel will generate its own frequency.
         """
         self.device.command(f'SOURce{self.module_number}:SYNChronize:SOURce {source}')
         self.device.command(f'SOURce{self.module_number}:SYNChronize:PHASe {str(phase_shift)}')
         self.device.command(f'SOURce{self.module_number}:SYNChronize:STATe {str(int(enable_sync))}')
 
     def get_duty(self):
-        """Returns the duty cycle of the module"""
+        """Returns the duty cycle of the module."""
 
         return float(self.device.query(f'SOURce{self.module_number}:DCYCle?'))
 
     def set_duty(self, duty):
-        """Sets the duty cycle of the module
+        """Sets the duty cycle of the module.
 
             Args:
                 duty (float):
-                    The new duty cycle
+                    The new duty cycle.
         """
 
         self.device.command(f'SOURce{self.module_number}:DCYCle {str(duty)}')
 
     def get_coupling(self):
         """Returns the coupling type of the module. 'AC' or 'DC'."""
 
         return self.device.query(f'SOURce{self.module_number}:COUPling?')
 
     def set_coupling(self, coupling):
-        """Sets the coupling of the module
+        """Sets the coupling of the module.
 
             Args:
                 coupling (str):
-                    The new coupling type ('AC', or 'DC')
+                    The new coupling type ('AC', or 'DC').
         """
         self.device.command(f'SOURce{self.module_number}:COUPling {coupling}')
 
     def use_ac_coupling(self):
-        """Sets the coupling type of the module to 'AC'"""
+        """Sets the coupling type of the module to 'AC'."""
 
         self.set_coupling('AC')
 
     def use_dc_coupling(self):
-        """Sets the coupling type of the module to 'DC'"""
+        """Sets the coupling type of the module to 'DC'."""
 
         self.set_coupling('DC')
 
     def get_guard_state(self):
-        """Returns the guard state of the module"""
+        """Returns the guard state of the module."""
 
         return bool(int(self.device.query(f'SOURce{self.module_number}:GUARd?')))
 
     def set_guard_state(self, guard_state):
-        """Sets the guard state of the module
+        """Sets the guard state of the module.
 
             Args:
                 guard_state (bool):
-                    The new guard state (True to enable guards, False to disable guards)
+                    The new guard state (True to enable guards, False to disable guards).
         """
 
         self.device.command(f'SOURce{self.module_number}:GUARd {str(int(guard_state))}')
 
     def enable_guards(self):
-        """Sets the guard state of the module to True"""
+        """Sets the guard state of the module to True."""
 
         self.set_guard_state(True)
 
     def disable_guards(self):
-        """Sets the guard state of the module to False"""
+        """Sets the guard state of the module to False."""
 
         self.set_guard_state(False)
 
     def get_cmr_source(self):
         """Returns the Common Mode Reduction (CMR) source. 'INTernal', or 'EXTernal'."""
 
         return self.device.query(f'SOURce{self.module_number}:CMR:SOURce?')
 
     def set_cmr_source(self, cmr_source):
         """Sets the Common Mode Reduction (CMR) source.
 
             Args:
                 cmr_source (str):
-                    The new CMR source ('INTernal', or 'EXTernal')
+                    The new CMR source ('INTernal', or 'EXTernal').
         """
 
         self.device.command(f'SOURce{self.module_number}:CMR:SOURce {cmr_source}')
 
     def get_cmr_state(self):
-        """Returns the Common Mode Reduction (CMR) state of the module"""
+        """Returns the Common Mode Reduction (CMR) state of the module."""
 
         return bool(int(self.device.query(f'SOURce{self.module_number}:CMR:STATe?')))
 
     def set_cmr_state(self, cmr_state):
-        """Sets the Common Mode Reduction (CMR) state of the module
+        """Sets the Common Mode Reduction (CMR) state of the module.
 
             Args:
                 cmr_state (bool):
-                    The new CMR state (True to enable CMR, False to disable CMR)
+                    The new CMR state (True to enable CMR, False to disable CMR).
         """
 
         self.device.command(f'SOURce{self.module_number}:CMR:STATe {str(int(cmr_state))}')
 
     def enable_cmr(self):
-        """Sets the CMR state of the module to True"""
+        """Sets the CMR state of the module to True."""
 
         self.set_cmr_state(True)
 
     def disable_cmr(self):
-        """Sets the CMR state of the module to False"""
+        """Sets the CMR state of the module to False."""
 
         self.set_cmr_state(False)
 
     def configure_cmr(self, cmr_source, cmr_state=True):
-        """Configure Common Mode Reduction (CMR)
+        """Configure Common Mode Reduction (CMR).
 
             Args:
                 cmr_source (str):
-                    The new CMR source ('INTernal', or 'EXTernal')
-
+                    The new CMR source ('INTernal', or 'EXTernal').
                 cmr_state (bool):
-                    The new CMR state (True to enable CMR, False to disable CMR)
+                    The new CMR state (True to enable CMR, False to disable CMR).
         """
 
         self.set_cmr_source(cmr_source)
         self.set_cmr_state(cmr_state)
 
     def get_current_range(self):
-        """Returns the present current range of the module in Amps"""
+        """Returns the present current range of the module in Amps."""
 
         return float(self.device.query(f'SOURce{self.module_number}:CURRent:RANGe?'))
 
     def get_i_range(self):
         """
         Returns the present current range of the module in Amps
         
@@ -354,15 +353,15 @@
            Use get_current_range instead.
         """
 
         warn("The get_i_range method is deprecated, use get_current_range instead", DeprecationWarning)
         return self.get_current_range()
 
     def get_current_ac_range(self):
-        """Returns the present AC current range of the module in Amps"""
+        """Returns the present AC current range of the module in Amps."""
 
         return float(self.device.query(f'SOURce{self.module_number}:CURRent:RANGe:AC?'))
 
     def get_i_ac_range(self):
         """
         Returns the present AC current range of the module in Amps
         
@@ -370,15 +369,15 @@
            Use get_current_ac_range instead.
         """
 
         warn("The get_i_ac_range method is deprecated, use get_current_ac_range instead", DeprecationWarning)
         return self.get_current_ac_range()
 
     def get_current_dc_range(self):
-        """Returns the present DC current range of the module in Amps"""
+        """Returns the present DC current range of the module in Amps."""
 
         return float(self.device.query(f'SOURce{self.module_number}:CURRent:RANGe:DC?'))
 
     def get_i_dc_range(self):
         """
         Returns the present DC current range of the module in Amps
         
@@ -386,15 +385,15 @@
            Use get_current_dc_range instead.
         """
 
         warn("The get_i_dc_range method is deprecated, use get_current_dc_range instead", DeprecationWarning)
         return self.get_current_dc_range()
 
     def get_current_autorange_status(self):
-        """Returns whether automatic selection of the current range is enabled for this module"""
+        """Returns whether automatic selection of the current range is enabled for this module."""
 
         return bool(int(self.device.query(f'SOURce{self.module_number}:CURRent:RANGe:AUTO?')))
 
     def get_i_autorange_status(self):
         """
         Returns whether automatic selection of the current range is enabled for this module
         
@@ -402,28 +401,27 @@
            Use get_current_autorange_status instead.
         """
 
         warn("The get_i_autorange_status method is deprecated, use get_current_autorange_status instead", DeprecationWarning)
         return self.get_current_autorange_status()
 
     def configure_current_range(self, autorange, max_level=None, max_ac_level=None, max_dc_level=None):
-        """Sets up current ranging for this module
+        """Sets up current ranging for this module.
 
             Args:
                 autorange (bool):
                     True to enable automatic range selection. False for manual ranging.
-
                 max_level (float):
                     The largest current that needs to be sourced.
-
                 max_ac_level (float):
-                    The largest AC current that needs to be sourced. Separate AC and DC ranges are only available on some modules.
-
+                    The largest AC current that needs to be sourced. Separate AC and DC ranges are only available on
+                    some modules.
                 max_dc_level (float):
-                    The largest DC current that needs to be sourced. Separate AC and DC ranges are only available on some modules.
+                    The largest DC current that needs to be sourced. Separate AC and DC ranges are only available on
+                    some modules.
         """
 
         if autorange:
             if max_level is not None or max_ac_level is not None or max_dc_level is not None:
                 raise ValueError('If autorange is selected, a manual range cannot be specified.')
 
             self.device.command(f'SOURce{self.module_number}:CURRent:RANGe:AUTO 1')
@@ -442,33 +440,30 @@
     def configure_i_range(self, autorange, max_level=None, max_ac_level=None, max_dc_level=None):
         """
         Sets up current ranging for this module
 
             Args:
                 autorange (bool):
                     True to enable automatic range selection. False for manual ranging.
-
                 max_level (float):
                     The largest current that needs to be sourced.
-
                 max_ac_level (float):
                     The largest AC current that needs to be sourced. Separate AC and DC ranges are only available on some modules.
-
                 max_dc_level (float):
                     The largest DC current that needs to be sourced. Separate AC and DC ranges are only available on some modules.
         
         .. deprecated:: 1.5.4
            Use configure_current_range instead.
         """
 
         warn("The configure_i_range method is deprecated, use configure_current_range instead", DeprecationWarning)
         self.configure_current_range(autorange, max_level, max_ac_level, max_dc_level)
 
     def get_current_amplitude(self):
-        """Returns the current amplitude for the module in Amps"""
+        """Returns the current amplitude for the module in Amps."""
 
         return float(self.device.query(f'SOURce{self.module_number}:CURRent:LEVel:AMPLitude?'))
 
     def get_i_amplitude(self):
         """
         Returns the current amplitude for the module in Amps
         
@@ -476,19 +471,19 @@
            Use get_current_amplitude instead.
         """
 
         warn("The get_i_amplitude method is deprecated, use get_current_amplitude instead", DeprecationWarning)
         return self.get_current_amplitude()
 
     def set_current_amplitude(self, amplitude):
-        """Sets the current amplitude for the module
+        """Sets the current amplitude for the module.
 
             Args:
                 amplitude (float):
-                    The new current amplitude in Amps
+                    The new current amplitude in Amps.
         """
         self.device.command(f'SOURce{self.module_number}:CURRent:LEVel:AMPLitude {str(amplitude)}')
 
     def set_i_amplitude(self, amplitude):
         """
         Sets the current amplitude for the module
 
@@ -500,15 +495,15 @@
            Use set_current_amplitude instead.
         """
 
         warn("The set_i_amplitude method is deprecated, use set_current_amplitude instead", DeprecationWarning)
         self.set_current_amplitude(amplitude)
 
     def get_current_offset(self):
-        """Returns the current offset for the module in Amps"""
+        """Returns the current offset for the module in Amps."""
 
         return float(self.device.query(f'SOURce{self.module_number}:CURRent:LEVel:OFFSet?'))
 
     def get_i_offset(self):
         """
         Returns the current offset for the module in Amps
         
@@ -516,19 +511,19 @@
            Use get_current_offset instead.
         """
 
         warn("The get_i_offset method is deprecated, use get_current_offset instead", DeprecationWarning)
         return self.get_current_offset()
 
     def set_current_offset(self, offset):
-        """Sets the current offset for the module
+        """Sets the current offset for the module.
 
             Args:
                 offset (float):
-                    The new current offset in Amps
+                    The new current offset in Amps.
         """
 
         self.device.command(f'SOURce{self.module_number}:CURRent:LEVel:OFFSet {str(offset)}')
 
     def set_i_offset(self, offset):
         """
         Sets the current offset for the module
@@ -541,49 +536,45 @@
            Use set_current_offset instead.
         """
 
         warn("The set_i_offset method is deprecated, use set_current_offset instead", DeprecationWarning)
         self.set_current_offset(offset)
 
     def apply_dc_current(self, level, output_enable=True):
-        """Apply DC current
+        """Apply DC current.
 
             Args:
                 level (float):
-                    DC current level in Amps
-
+                    DC current level in Amps.
                 output_enable (bool):
-                    Turns the module output on if true; off if false
+                    Turns the module output on if true; off if false.
         """
 
         if not output_enable:
             self.disable()
 
         self.set_excitation_mode('CURRent')
         self.set_shape('DC')
         self.set_current_amplitude(level)
 
         if output_enable:
             self.enable()
 
     def apply_ac_current(self, frequency, amplitude, offset=0.0, output_enable=True):
-        """Apply AC current
+        """Apply AC current.
 
             Args:
                 frequency (float):
-                    Excitation frequency in Hz
-
+                    Excitation frequency in Hz.
                 amplitude (float):
-                    Current amplitude in Amps
-
+                    Current amplitude in Amps.
                 offset (float):
-                    Current offset in Amps
-
+                    Current offset in Amps.
                 output_enable (bool):
-                    Turns the module output on if true; off if false
+                    Turns the module output on if true; off if false.
         """
 
         if not output_enable:
             self.disable()
 
         self.set_excitation_mode('CURRent')
         self.set_frequency(frequency)
@@ -591,15 +582,15 @@
         self.set_current_amplitude(amplitude)
         self.set_current_offset(offset)
 
         if output_enable:
             self.enable()
 
     def get_current_limit(self):
-        """Returns the current limit enforced by the module in Amps"""
+        """Returns the current limit enforced by the module in Amps."""
 
         return float(self.device.query(f'SOURce{self.module_number}:CURRent:PROTection?'))
 
     def get_i_limit(self):
         """
         Returns the current limit enforced by the module in Amps
         
@@ -607,19 +598,19 @@
            Use get_current_limit instead.
         """
 
         warn("The get_i_limit method is deprecated, use get_current_limit instead", DeprecationWarning)
         return self.get_current_limit()
 
     def set_current_limit(self, current_limit):
-        """Sets the current limit enforced by the module
+        """Sets the current limit enforced by the module.
 
             Args:
                 current_limit (float):
-                    The new limit to apply in Amps
+                    The new limit to apply in Amps.
         """
         self.device.command(f'SOURce{self.module_number}:CURRent:PROTection {str(current_limit)}')
 
     def set_i_limit(self, i_limit):
         """
         Sets the current limit enforced by the module
 
@@ -631,15 +622,18 @@
            Use set_current_limit instead.
         """
 
         warn("The set_i_limit method is deprecated, use set_current_limit instead", DeprecationWarning)
         self.set_current_limit(i_limit)
 
     def get_current_limit_status(self):
-        """Returns whether the current limit circuitry is presently engaged and limiting the current sourced by the module"""
+        """Returns whether the current limit circuitry is presently engaged.
+
+            This limits the current sourced by the module.
+        """
 
         return bool(int(self.device.query(f'SOURce{self.module_number}:CURRent:PROTection:TRIPped?')))
 
     def get_i_limit_status(self):
         """
         Returns whether the current limit circuitry is presently engaged and limiting the current sourced by the module
         
@@ -647,48 +641,47 @@
            Use get_current_limit_status instead.
         """
 
         warn("The get_i_limit_status method is deprecated, use get_current_limit_status instead", DeprecationWarning)
         return self.get_current_limit_status()
 
     def get_voltage_range(self):
-        """Returns the present voltage range of the module in Volts"""
+        """Returns the present voltage range of the module in Volts."""
 
         return float(self.device.query(f'SOURce{self.module_number}:VOLTage:RANGe?'))
 
     def get_voltage_ac_range(self):
-        """Returns the present AC voltage range of the module in Volts"""
+        """Returns the present AC voltage range of the module in Volts."""
 
         return float(self.device.query(f'SOURce{self.module_number}:VOLTage:RANGe:AC?'))
 
     def get_voltage_dc_range(self):
-        """Returns the present DC voltage range of the module in Volts"""
+        """Returns the present DC voltage range of the module in Volts."""
 
         return float(self.device.query(f'SOURce{self.module_number}:VOLTage:RANGe:DC?'))
 
     def get_voltage_autorange_status(self):
-        """Returns whether automatic selection of the voltage range is enabled for this module"""
+        """Returns whether automatic selection of the voltage range is enabled for this module."""
 
         return bool(int(self.device.query(f'SOURce{self.module_number}:VOLTage:RANGe:AUTO?')))
 
     def configure_voltage_range(self, autorange, max_level=None, max_ac_level=None, max_dc_level=None):
-        """Sets up voltage ranging for this module
+        """Sets up voltage ranging for this module.
 
             Args:
                 autorange (bool):
                     True to enable automatic range selection. False for manual ranging.
-
                 max_level (float):
                     The largest voltage that needs to be sourced.
-
                 max_ac_level (float):
-                    The largest AC voltage that needs to be sourced. Separate AC and DC ranges are only available on some modules.
-
+                    The largest AC voltage that needs to be sourced. Separate AC and DC ranges are only available on
+                    some modules.
                 max_dc_level (float):
-                    The largest DC voltage that needs to be sourced. Separate AC and DC ranges are only available on some modules.
+                    The largest DC voltage that needs to be sourced. Separate AC and DC ranges are only available on
+                    some modules.
         """
 
         if autorange:
             if max_level is not None or max_ac_level is not None or max_dc_level is not None:
                 raise ValueError('If autorange is selected, a manual range cannot be specified.')
 
             self.device.command(f'SOURce{self.module_number}:VOLTage:RANGe:AUTO 1')
@@ -701,79 +694,75 @@
             else:
                 if max_ac_level is not None:
                     self.device.command(f'SOURce{self.module_number}:VOLTage:RANGe:AC {str(max_ac_level)}')
                 if max_dc_level is not None:
                     self.device.command(f'SOURce{self.module_number}:VOLTage:RANGe:DC {str(max_dc_level)}')
 
     def get_voltage_amplitude(self):
-        """Returns the voltage amplitude for the module in Volts"""
+        """Returns the voltage amplitude for the module in Volts."""
 
         return float(self.device.query(f'SOURce{self.module_number}:VOLTage:LEVel:AMPLitude?'))
 
     def set_voltage_amplitude(self, amplitude):
-        """Sets the voltage amplitude for the module
+        """Sets the voltage amplitude for the module.
 
             Args:
                 amplitude (float):
-                    The new voltage amplitude in Volts
+                    The new voltage amplitude in Volts.
         """
 
         self.device.command(f'SOURce{self.module_number}:VOLTage:LEVel:AMPLitude {str(amplitude)}')
 
     def get_voltage_offset(self):
-        """Returns the voltage offset for the module in Volts"""
+        """Returns the voltage offset for the module in Volts."""
 
         return float(self.device.query(f'SOURce{self.module_number}:VOLTage:LEVel:OFFSet?'))
 
     def set_voltage_offset(self, offset):
-        """Sets the voltage offset for the module
+        """Sets the voltage offset for the module.
 
             Args:
                 offset (float):
-                    The new voltage offset in Volts
+                    The new voltage offset in Volts.
         """
 
         self.device.command(f'SOURce{self.module_number}:VOLTage:LEVel:OFFSet {str(offset)}')
 
     def apply_dc_voltage(self, level, output_enable=True):
-        """Apply DC voltage
+        """Apply DC voltage.
 
             Args:
                 level (float):
-                    DC voltage level in Volts
-
+                    DC voltage level in Volts.
                 output_enable (bool):
-                    Turns the module output on if true; off if false
+                    Turns the module output on if true; off if false.
         """
 
         if not output_enable:
             self.disable()
 
         self.set_excitation_mode('VOLTage')
         self.set_shape('DC')
         self.set_voltage_amplitude(level)
 
         if output_enable:
             self.enable()
 
     def apply_ac_voltage(self, frequency, amplitude, offset=0.0, output_enable=True):
-        """Apply AC voltage
+        """Apply AC voltage.
 
             Args:
                 frequency (float):
-                    Excitation frequency in Hz
-
+                    Excitation frequency in Hz.
                 amplitude (float):
-                    Voltage amplitude in Volts
-
+                    Voltage amplitude in Volts.
                 offset (float):
-                    Voltage offset in Volts
-
+                    Voltage offset in Volts.
                 output_enable (bool):
-                    Turns the module output on if true; off if false
+                    Turns the module output on if true; off if false.
         """
 
         if not output_enable:
             self.disable()
 
         self.set_excitation_mode(self.device.ExcitationType.VOLTAGE)
         self.set_frequency(frequency)
@@ -781,100 +770,113 @@
         self.set_voltage_amplitude(amplitude)
         self.set_voltage_offset(offset)
 
         if output_enable:
             self.enable()
 
     def get_voltage_limit(self):
-        """Returns the voltage limit enforced by the module in Volts"""
+        """Returns the voltage limit enforced by the module in Volts."""
 
         return float(self.device.query(f'SOURce{self.module_number}:VOLTage:PROTection?'))
 
     def set_voltage_limit(self, voltage_limit):
-        """Sets the voltage limit enforced by the module
+        """Sets the voltage limit enforced by the module.
 
             Args:
                 voltage_limit (float):
-                    The new limit to apply in Volts
+                    The new limit to apply in Volts.
         """
 
         self.device.command(f'SOURce{self.module_number}:VOLTage:PROTection {str(voltage_limit)}')
 
     def get_voltage_limit_status(self):
-        """Returns whether the voltage limit circuitry is presently engaged and limiting the voltage at the output of the module"""
+        """Returns whether the voltage limit circuitry is presently engaged.
+
+            This limits the voltage at the output of the module.
+         """
 
         return bool(int(self.device.query(f'SOURce{self.module_number}:VOLTage:PROTection:TRIPped?')))
 
     def get_present_questionable_status(self):
-        """Returns the names of the questionable status register bits and their values"""
+        """Returns the names of the questionable status register bits and their values."""
 
         response = self.device.query(f'STATus:QUEStionable:SOURce{self.module_number}:CONDition?', check_errors=False)
         status_register = SSMSystemModuleQuestionableRegister.from_integer(response)
 
         return status_register
 
     def get_questionable_events(self):
         """Returns the names of questionable event status register bits that are currently high.
-        The event register is latching and values are reset when queried."""
+
+            The event register is latching and values are reset when queried.
+        """
 
         response = self.device.query(f'STATus:QUEStionable:SOURce{self.module_number}:EVENt?', check_errors=False)
         status_register = SSMSystemModuleQuestionableRegister.from_integer(response)
 
         return status_register
 
     def get_questionable_event_enable_mask(self):
         """Returns the names of the questionable event enable register bits and their values.
-        These values determine which questionable bits propagate to the questionable event register."""
+
+            These values determine which questionable bits propagate to the questionable event register.
+        """
 
         response = self.device.query(f'STATus:QUEStionable:SOURce{self.module_number}:ENABle?', check_errors=False)
         status_register = SSMSystemModuleQuestionableRegister.from_integer(response)
 
         return status_register
 
     def set_questionable_event_enable_mask(self, register_mask):
         """Configures the values of the questionable event enable register bits.
-        These values determine which questionable bits propagate to the questionable event register.
+
+            These values determine which questionable bits propagate to the questionable event register.
 
             Args:
                 register_mask ([Instrument]QuestionableRegister):
                     An instrument specific QuestionableRegister class object with all bits configured true or false.
         """
 
         integer_representation = register_mask.to_integer()
         self.device.command(f'STATus:QUEStionable:SOURce{self.module_number}:ENABle {integer_representation}', check_errors=False)
 
     def get_present_operation_status(self):
-        """Returns the names of the operation status register bits and their values"""
+        """Returns the names of the operation status register bits and their values."""
 
         response = self.device.query(f'STATus:OPERation:SOURce{self.module_number}:CONDition?', check_errors=False)
         status_register = SSMSystemSourceModuleOperationRegister.from_integer(response)
 
         return status_register
 
     def get_operation_events(self):
         """Returns the names of operation event status register bits that are currently high.
-        The event register is latching and values are reset when queried."""
+
+            The event register is latching and values are reset when queried.
+        """
 
         response = self.device.query(f'STATus:OPERation:SOURce{self.module_number}:EVENt?', check_errors=False)
         status_register = SSMSystemSourceModuleOperationRegister.from_integer(response)
 
         return status_register
 
     def get_operation_event_enable_mask(self):
         """Returns the names of the operation event enable register bits and their values.
-        These values determine which operation bits propagate to the operation event register."""
+
+            These values determine which operation bits propagate to the operation event register.
+        """
 
         response = self.device.query(f'STATus:OPERation:SOURce{self.module_number}:ENABle?', check_errors=False)
         status_register = SSMSystemSourceModuleOperationRegister.from_integer(response)
 
         return status_register
 
     def set_operation_event_enable_mask(self, register_mask):
         """Configures the values of the operation event enable register bits.
-        These values determine which operation bits propagate to the operation event register.
+
+            These values determine which operation bits propagate to the operation event register.
 
             Args:
                 register_mask ([Instrument]OperationRegister):
                     An instrument specific OperationRegister class object with all bits configured true or false.
         """
 
         integer_representation = register_mask.to_integer()
@@ -886,194 +888,188 @@
         return response
 
     def set_identify_state(self, state):
         """Configures the identification state for the given pod.
 
             Args:
                 state (bool):
-                    The desired state for the LED, 1 for identify, 0 for normal state
+                    The desired state for the LED, 1 for identify, 0 for normal state.
         """
         self.device.command(f'SOURce{self.module_number}:IDENtify {int(state)}', check_errors=False)
 
     def get_dark_mode_state(self):
-        """Returns the dark mode state for the given pod"""
+        """Returns the dark mode state for the given pod."""
         response = self.device.query(f'SOURce{self.module_number}:DMODe?', cherk_errors=False)
         return response
 
     def set_dark_mode_state(self, state):
         """Configures the dark mode state for the given pod.
 
             Args:
                 state (bool):
-                    The desired operation for the LED, 1 for normal mode, 0 for dark mode
+                    The desired operation for the LED, 1 for normal mode, 0 for dark mode.
         """
         self.device.command(f'SOURce{self.module_number}:DMODe {state}', check_errors=False)
 
     def get_voltage_output_limit_high(self):
         """Returns the present voltage high output limit."""
         response = float(self.device.query(f'SOURce{self.module_number}:VOLTage:LIMit:HIGH?', cherk_errors=False))
         return response
 
     def set_voltage_output_limit_high(self, limit):
         """Configures the high voltage output limit.
-        The voltage output limits are software defined limits preventing the user from entering an output which could
-        potentially damage the module's load.
-        When the shape is not DC, the limit is applied to the sum of the offset and amplitude.
-        The high voltage output limit is bounded between -10 V and 10 V, and must be greater than the low voltage output limit.
+
+            The voltage output limits are software defined limits preventing the user from entering an output which
+            could potentially damage the module's load. When the shape is not DC, the limit is applied to the sum of
+            the offset and amplitude. The high voltage output limit is bounded between -10 V and 10 V, and must be
+            greater than the low voltage output limit.
 
             Args:
                 limit (float):
                     The desired high output limit.
         """
         self.device.command(f'SOURce{self.module_number}:VOLTage:LIMit:HIGH {limit}', check_errors=False)
 
     def get_voltage_output_limit_low(self):
         """Returns the present voltage low output limit."""
         response = float(self.device.query(f'SOURce{self.module_number}:VOLTage:LIMit:LOW?', cherk_errors=False))
         return response
 
     def set_voltage_output_limit_low(self, limit):
         """Configures the low voltage output limit.
-        The voltage output limits are software defined limits preventing the user from entering an output which could
-        potentially damage the module's load.
-        When the shape is not DC, the limit is applied to the sum of the offset and amplitude.
-        The low voltage output limit is bounded between -10 V and 10 V, and must be less than the high voltage output limit.
+
+            The voltage output limits are software defined limits preventing the user from entering an output which
+            could potentially damage the module's load. When the shape is not DC, the limit is applied to the sum of
+            the offset and amplitude. The low voltage output limit is bounded between -10 V and 10 V, and must be less
+            than the high voltage output limit.
 
             Args:
                 limit (float):
                     The desired low voltage output limit.
         """
         self.device.command(f'SOURce{self.module_number}:VOLTage:LIMit:LOW {limit}', check_errors=False)
 
     def get_current_output_limit_high(self):
         """Returns the present current high output limit."""
         response = float(self.device.query(f'SOURce{self.module_number}:CURRent:LIMit:HIGH?', cherk_errors=False))
         return response
 
     def set_current_output_limit_high(self, limit):
         """Configures the high current output limit.
-        The current output limits are software defined limits preventing the user from entering an output which could
-        potentially damage the module's load.
-        When the shape is not DC, the limit is applied to the sum of the offset and amplitude.
-        The high current output limit is bounded between -10 V and 10 V, and must be greater than the low current output limit.
+
+            The current output limits are software defined limits preventing the user from entering an output which
+            could potentially damage the module's load. When the shape is not DC, the limit is applied to the sum of
+            the offset and amplitude. The high current output limit is bounded between -10 V and 10 V, and must be
+            greater than the low current output limit.
 
             Args:
                 limit (float):
                     The desired high output limit.
         """
         self.device.command(f'SOURce{self.module_number}:CURRent:LIMit:HIGH {str(limit)}', check_errors=False)
 
     def get_current_output_limit_low(self):
         """Returns the present current low output limit."""
         response = float(self.device.query(f'SOURce{self.module_number}:CURRent:LIMit:LOW?', cherk_errors=False))
         return response
 
     def set_disable_on_compliance(self, disable_on_compliance):
         """Configures the module for disable on compliance.
-        When disable on compliance is turned on, the module will disable output when in compliance.
-        Otherwise, the module will continue to output, even when in compliance.
+
+            When disable on compliance is turned on, the module will disable output when in compliance.
+            Otherwise, the module will continue to output, even when in compliance.
 
             Args:
                 disable_on_compliance (bool):
-                    1 for the module to disable when in compliance; 0 for the module to remain enabled, even in compliance
+                    1 for the module to disable when in compliance; 0 for the module to remain enabled, even in
+                    compliance.
         """
         self.device.command(f'SOURce{self.module_number}:DOCompliance {int(disable_on_compliance)}', check_errors=False)
 
     def get_disable_on_compliance(self):
         """Returns the present state of disable on compliance."""
         response = bool(self.device.query(f'SOURce{self.module_number}:DOCompliance?', check_errors=False))
         return response
 
     def set_current_output_limit_low(self, limit):
         """Configures the low current output limit.
-        The current output limits are software defined limits preventing the user from entering an output which could
-        potentially damage the module's load.
-        When the shape is not DC, the limit is applied to the sum of the offset and amplitude.
-        The low current output limit is bounded between -10 V and 10 V, and must be less than the high current output limit.
+
+            The current output limits are software defined limits preventing the user from entering an output which
+            could potentially damage the module's load. When the shape is not DC, the limit is applied to the sum of
+            the offset and amplitude. The low current output limit is bounded between -10 V and 10 V, and must be less
+            than the high current output limit.
 
             Args:
                 limit (float):
                     The desired low current output limit.
         """
         self.device.command(f'SOURce{self.module_number}:CURRent:LIMit:LOW {str(limit)}', check_errors=False)
 
     def reset_settings(self):
-        """Resets the settings for the specified module to their power on defaults.
-        """
+        """Resets the settings for the specified module to their power on defaults."""
 
         self.device.command(f'SOURce{self.module_number}:PRESet')
 
     def unload(self):
-        """Unloads the specified module.
-        """
+        """Unloads the specified module."""
 
         self.device.command(f'SOURce{self.module_number}:UNLoad')
 
     def get_load_state(self):
-        """Returns the loaded state for the specified module.
-        """
+        """Returns the loaded state for the specified module."""
 
         response = bool(int(self.device.query(f'SOURce{self.module_number}:LOAD?')))
         return response
 
     def get_self_cal_datetime(self):
-        """Returns the self calibration date and time for the specified module.
-        """
+        """Returns the self calibration date and time for the specified module."""
 
         response = self.device.query(f'SOURce{self.module_number}:SCALibration:DATE?').split(',')
         return datetime(int(response[0]), int(response[1]), int(response[2]), int(response[3]), int(response[4]), int(response[5]))
 
     def get_self_cal_temperature(self):
-        """Returns the self calibration temperature for the specified module.
-        """
+        """Returns the self calibration temperature for the specified module."""
 
         response = float(self.device.query(f'SOURce{self.module_number}:SCALibration:TEMP?'))
         return response
 
     @requires_firmware_version('1.7.0')
     def get_source_sweep_step_size(self, sweep_type):
-        """
-        Returns the step size of the source sweep for the specified module.
-        Step size is a calculated parameter derived from the relevant sweep type's span and points.
+        """Returns the step size of the source sweep for the specified module.
+
+            Step size is a calculated parameter derived from the relevant sweep type's span and points.
 
         Args:
             sweep_type (SourceSweepType):
                 The type of sweep for which to return the step size.
         """
 
         response = float(self.device.query(f'SOURce{self.module_number}:{sweep_type}:STEP?'))
         return response
 
     @requires_firmware_version('1.7.0')
     def get_source_sweep_time(self):
-        """
-        Returns the overall runtime of the source sweep for the specified module in seconds.
-        Sweep time is a calculated parameter derived from the dwell time and number of points.
+        """Returns the overall runtime of the source sweep for the specified module in seconds.
+
+            Sweep time is a calculated parameter derived from the dwell time and number of points.
         """
 
         response = float(self.device.query(f'SOURce{self.module_number}:SWEep:TIME?'))
         return response
 
     @requires_firmware_version('1.7.0')
-    def abort_source_sweep(self):
-        """Aborts all in progress source sweep for the specified module."""
-
-        self.device.command(f'SOURce{self.module_number}:SWEep:ABORt')
-
-    @requires_firmware_version('1.7.0')
     def get_source_sweep_state(self):
         """Returns the state of the source sweep on the specified module."""
 
         response = bool(int(self.device.query(f'SOURce{self.module_number}:SWEep:STATus?')))
         return response
 
     @requires_firmware_version('1.7.0')
     def set_sweep_configuration(self, sweep_settings):
-        """
-        Configures a source sweep for the specified module.
+        """Configures a source sweep for the specified module.
 
         Args:
             sweep_settings (SourceSweepSettings):
                 The configuration for a specific sweep on the specified module.
         """
 
         self.device.command(f'SOURce{self.module_number}:SWEep:DWELl {sweep_settings.dwell}')
@@ -1083,16 +1079,15 @@
         self.device.command(f'SOURce{self.module_number}:SWEep:DIRection:RTRip {int(sweep_settings.round_trip)}')
         self.device.command(f'SOURce{self.module_number}:{sweep_settings.sweep_type}:MODE SWEep')
         self.device.command(f'SOURce{self.module_number}:{sweep_settings.sweep_type}:STARt {sweep_settings.start}')
         self.device.command(f'SOURce{self.module_number}:{sweep_settings.sweep_type}:STOP {sweep_settings.stop}')
 
     @requires_firmware_version('1.7.0')
     def get_sweep_configuration(self, sweep_type):
-        """
-        Returns a SourceSweepSettings of the present sweep configuration for the specified module.
+        """Returns a SourceSweepSettings of the present sweep configuration for the specified module.
 
         Args:
             sweep_type (SourceSweepType):
                 The sweep type for which to return the sweep settings.
         """
 
         return self.device.SourceSweepSettings(
@@ -1110,36 +1105,33 @@
         """Disables all source signals that support sweeping on the specified module."""
 
         for sweep_type in self.device.SourceSweepType:
             self.device.command(f'SOURce{self.module_number}:{sweep_type}:MODE FIXED')
 
     @requires_firmware_version('1.7.0')
     def disable_sweeping(self, sweep_type):
-        """
-        Disables the sweeping of the specified sweep type on the specified module.
+        """Disables the sweeping of the specified sweep type on the specified module.
 
         Args:
             sweep_type (SourceSweepType):
                 The type of sweep to disable.
         """
 
         self.device.command(f'SOURce{self.module_number}:{sweep_type}:MODE FIXED')
 
     def set_voltage_ramp_configuration(self, stop_amplitude, start_amplitude=None, slew_rate=1.0):
-        """
-        Sets up a parameter sweep that ramps the voltage output to the desired amplitude using the smallest
-        possible step size.
+        """Sets up a parameter sweep that ramps the voltage output to the desired amplitude.
+
+            Uses the smallest possible step size.
 
         Args:
             stop_amplitude (float):
                 The voltage amplitude of the output when the ramp completes.
-
             start_amplitude (float):
                 The voltage amplitude of the output when the ramp starts. Default is the present amplitude setting.
-
             slew_rate (float):
                 The rate in volts per second to ramp the output. Default is 1 volt per second.
         """
         # Use the present voltage amplitude as the starting point if no start is specified
         if start_amplitude is None:
             start_amplitude = self.get_voltage_amplitude()
 
@@ -1155,25 +1147,23 @@
                                                        points=num_points,
                                                        dwell=dwell_time,
                                                        direction=self.device.SourceSweepSettings.Direction.UP,
                                                        round_trip=False)
         self.set_sweep_configuration(sweep_config)
 
     def set_current_ramp_configuration(self, stop_amplitude, start_amplitude=None, slew_rate=0.001):
-        """
-        Sets up a parameter sweep that ramps the current output to the desired amplitude using the smallest
-        possible step size.
+        """Sets up a parameter sweep that ramps the current output to the desired amplitude.
+
+            Uses the smallest possible step size.
 
         Args:
             stop_amplitude (float):
                 The current amplitude of the output when the ramp completes.
-
             start_amplitude (float):
                 The current amplitude of the output when the ramp starts. Default is the present amplitude setting.
-
             slew_rate (float):
                 The rate in amps per second to ramp the output. Default is 1 mA per second.
         """
         # Use the present voltage amplitude as the starting point if no start is specified
         if start_amplitude is None:
             start_amplitude = self.get_current_amplitude()
```

### Comparing `lakeshore-1.6.1/lakeshore/ssm_system.py` & `lakeshore-1.7.0/lakeshore/ssm_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 except NotImplementedError:
     pass  # Proceed without wakepy on linux without systemd
 except KeyError:
     pass  # Proceed without wakepy on linux without dbus
 
 
 class SSMSystemOperationRegister(RegisterBase):
-    """Class object representing the operation status register"""
+    """Class object representing the operation status register."""
 
     bit_names = [
         "s1_summary",
         "s2_summary",
         "s3_summary",
         "m1_summary",
         "m2_summary",
@@ -47,15 +47,15 @@
         self.m1_summary = m1_summary
         self.m2_summary = m2_summary
         self.m3_summary = m3_summary
         self.data_stream_in_progress = data_stream_in_progress
 
 
 class SSMSystemQuestionableRegister(RegisterBase):
-    """Class object representing the questionable status register"""
+    """Class object representing the questionable status register."""
 
     bit_names = [
         "s1_summary",
         "s2_summary",
         "s3_summary",
         "m1_summary",
         "m2_summary",
@@ -90,15 +90,15 @@
         self.critical_runtime_error = critical_runtime_error
         self.heartbeat = heartbeat
         self.calibration = calibration
         self.data_stream_overflow = data_stream_overflow
 
 
 class SSMSystem(XIPInstrument, SSMSystemEnums):
-    """Class for interaction with the M81 instrument"""
+    """Class for interaction with the M81 instrument."""
 
     vid_pid = [(0x1FB9, 0x0704), (0x10C4, 0xEA60)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=921600,
@@ -131,60 +131,60 @@
         self.stream_lock = Lock()
 
         # Sweeping limits
         self.min_sweep_dwell = 0.000_2
         self.max_sweep_points = 100_001
 
     def load_modules(self):
-        """Loads all unloaded modules. Connected modules must be loaded before they can be used"""
+        """Loads all unloaded modules. Connected modules must be loaded before they can be used."""
         self.command('SYSTem:LOAD')
 
     def get_num_measure_channels(self):
-        """Returns the number of measure channels supported by the instrument"""
+        """Returns the number of measure channels supported by the instrument."""
 
         return int(self.query('SENSe:NCHannels?'))
 
     def get_num_source_channels(self):
         """Returns the number of source channels supported by the instrument"""
 
         return int(self.query('SOURce:NCHannels?'))
 
     def get_source_module(self, port_number):
-        """Returns a SourceModule instance for the given port number"""
+        """Returns a SourceModule instance for the given port number."""
 
         try:
             return self.source_modules[port_number - 1]
         except IndexError:
             raise IndexError(
                 f'Invalid port number. Must be between 1 and {self.get_num_source_channels()}') from None
 
     def get_source_pod(self, port_number):
-        """alias of get_source_module"""
+        """Alias of get_source_module."""
         return self.get_source_module(port_number)
 
     def get_source_module_by_name(self, module_name):
-        """Return the SourceModule instance that matches the specified name"""
+        """Return the SourceModule instance that matches the specified name."""
 
         return self._locate_module_by_name(module_name, self.source_modules)
 
     def get_measure_module(self, port_number):
-        """Returns a MeasureModule instance for the given port number"""
+        """Returns a MeasureModule instance for the given port number."""
 
         try:
             return self.measure_modules[port_number - 1]
         except IndexError:
             raise IndexError(
                 f'Invalid port number. Must be between 1 and {self.get_num_measure_channels()}') from None
 
     def get_measure_pod(self, port_number):
-        """alias of get_measure_module"""
+        """Alias of get_measure_module."""
         return self.get_measure_module(port_number)
 
     def get_measure_module_by_name(self, module_name):
-        """Return the MeasureModule instance that matches the specified name"""
+        """Return the MeasureModule instance that matches the specified name."""
 
         return self._locate_module_by_name(module_name, self.measure_modules)
 
     @staticmethod
     def _locate_module_by_name(module_name, set_of_modules):
         module_names = []
         for module in set_of_modules:
@@ -248,34 +248,36 @@
         warn("The get_multiple method is deprecated, use fetch_multiple instead", DeprecationWarning)
         return self.fetch_multiple(*data_sources)
 
     def get_multiple_min_max_values(self, *data_sources):
         """Gets a synchronized minimum and maximum value for each specified data source.
 
             Args:
-                data_sources (str, int): Pairs of (DATASOURCE_MNEMONIC, CHANNEL_INDEX).
+                data_sources (str, int):
+                    Pairs of (DATASOURCE_MNEMONIC, CHANNEL_INDEX).
         """
 
         elements = ','.join(f'{mnemonic},{index}' for (mnemonic, index) in data_sources)
         response_values = self.query(f'STAT:MMAX? {elements}').split(',')
 
         return [(float(response_values[i]), float(response_values[i + 1])) for i in range(0, len(response_values), 2)]
 
     def stream_data(self, rate, num_points, *data_sources):
         """Generator object to stream data from the instrument.
 
             Args:
-                rate (int): Desired transfer rate in points/sec.
-                num_points (int): Number of points to return. None to stream indefinitely.
-
+                rate (int):
+                    Desired transfer rate in points/sec.
+                num_points (int):
+                    Number of points to return. None to stream indefinitely.
                 data_sources (SSMSystemDataSourceMnemonic or str, int):
                     Variable length list of pairs of (DATA_SOURCE, CHANNEL_INDEX).
 
             Yields:
-                A single row of stream data as a tuple
+                A single row of stream data as a tuple.
         """
 
         with self.stream_lock:
             with keepawake(keep_screen_awake=True):
                 self.command('TRACe:RESEt')
                 self._configure_stream_elements(data_sources)
                 self.command('TRACe:FORMat:ENCOding B64')
@@ -308,35 +310,41 @@
             if overflow_occurred:
                 raise XIPInstrumentException('Data loss occurred during this data stream.')
 
     def get_data(self, rate, num_points, *data_sources):
         """Like stream_data, but returns a list.
 
             Args:
-                rate (int): Desired transfer rate in points/sec.
-                num_points (int): Number of points to return.
-
+                rate (int):
+                    Desired transfer rate in points/sec.
+                num_points (int):
+                    Number of points to return.
                 data_sources (SSMSystemDataSourceMnemonic or str, int):
                     Variable length list of pairs of (DATA_SOURCE, CHANNEL_INDEX).
 
             Returns:
-                All available stream data as a list of tuples
+                All available stream data as a list of tuples.
         """
 
         return list(self.stream_data(rate, num_points, *data_sources))
 
     def log_data_to_csv_file(self, rate, num_points, file, *data_sources, **kwargs):
         """Like stream_data, but logs directly to a CSV file.
 
             Args:
-                rate (int): Desired transfer rate in points/sec.
-                file (IO): File to log to.
-                num_points (int): Number of points to log.
-                data_sources (SSMSystemDataSourceMnemonic or str, int): Pairs of (DATA_SOURCE, CHANNEL_INDEX).
-                write_header (bool): If true, a header row is written with column names.
+                rate (int):
+                    Desired transfer rate in points/sec.
+                file (IO):
+                    File to log to.
+                num_points (int):
+                    Number of points to log.
+                data_sources (SSMSystemDataSourceMnemonic or str, int):
+                    Pairs of (DATA_SOURCE, CHANNEL_INDEX).
+                write_header (bool):
+                    If true, a header row is written with column names.
         """
         write_header = kwargs.pop('write_header', True)
 
         if write_header:
             self._configure_stream_elements(data_sources)
             header = self.query('TRACe:FORMat:HEADer?').strip('\"')
             file.write(header + '\n')
@@ -350,72 +358,71 @@
 
     def get_ref_in_edge(self):
         """Returns the active edge of the reference input. 'RISing' or 'FALLing'."""
 
         return self.query('INPut:REFerence:EDGe?')
 
     def set_ref_in_edge(self, edge):
-        """Sets the active edge of the reference input
+        """Sets the active edge of the reference input.
 
             Args:
                 edge (str):
-                    The new active edge ('RISing', or 'FALLing')
+                    The new active edge ('RISing', or 'FALLing').
         """
 
         self.command(f'INPut:REFerence:EDGe {edge}')
 
     def get_ref_out_source(self):
         """Returns the channel used for the reference output. 'S1', 'S2', or 'S3'."""
 
         return self.query('OUTPut:REFerence:SOURce?')
 
     def set_ref_out_source(self, ref_out_source):
         """Sets the channel used for the reference output.
 
             Args:
                 ref_out_source (str):
-                    The new reference out source ('S1', 'S2', or 'S3')
+                    The new reference out source ('S1', 'S2', or 'S3').
         """
 
         self.command(f'OUTPut:REFerence:SOURce {ref_out_source}')
 
     def get_ref_out_state(self):
-        """Returns the enable state of reference out"""
+        """Returns the enable state of reference out."""
 
         return bool(int(self.query('OUTPut:REFerence:STATe?')))
 
     def set_ref_out_state(self, ref_out_state):
-        """Sets the enable state of reference out
+        """Sets the enable state of reference out.
 
             Args:
                 ref_out_state (bool):
-                    The new reference out state (True to enable reference out, False to disable reference out)
+                    The new reference out state (True to enable reference out, False to disable reference out).
         """
 
         self.command(f'OUTPut:REFerence:STATe {str(int(ref_out_state))}')
 
     def enable_ref_out(self):
-        """Sets the enable state of reference out to True"""
+        """Sets the enable state of reference out to True."""
 
         self.set_ref_out_state(True)
 
     def disable_ref_out(self):
-        """Sets the enable state of reference out to False"""
+        """Sets the enable state of reference out to False."""
 
         self.set_ref_out_state(False)
 
     def configure_ref_out(self, ref_out_source, ref_out_state=True):
-        """Configure the reference output
+        """Configure the reference output.
 
             Args:
                 ref_out_source (str):
-                    The new reference out source ('S1', 'S2', or 'S3')
-
+                    The new reference out source ('S1', 'S2', or 'S3').
                 ref_out_state (bool):
-                    The new reference out state (True to enable reference out, False to disable reference out)
+                    The new reference out state (True to enable reference out, False to disable reference out).
         """
 
         self.set_ref_out_source(ref_out_source)
         self.set_ref_out_state(ref_out_state)
 
     def get_mon_out_mode(self):
         """Returns the channel used for the monitor output. 'M1', 'M2', 'M3', or 'MANUAL'."""
@@ -423,173 +430,169 @@
         return self.query('OUTPut:MONitor:MODe?')
 
     def set_mon_out_mode(self, mon_out_source):
         """Sets the channel used for the monitor output.
 
             Args:
                 mon_out_source (str):
-                    The new monitor out source ('M1', 'M2', 'M3', or 'MANUAL')
+                    The new monitor out source ('M1', 'M2', 'M3', or 'MANUAL').
         """
 
         self.command(f'OUTPut:MONitor:MODe {mon_out_source}')
 
     def get_mon_out_state(self):
-        """Returns the enable state of monitor out"""
+        """Returns the enable state of monitor out."""
 
         return bool(int(self.query('OUTPut:MONitor:STATe?')))
 
     def set_mon_out_state(self, mon_out_state):
-        """Sets the enable state of monitor out
+        """Sets the enable state of monitor out.
 
             Args:
                 mon_out_state (bool):
-                    The new monitor out state (True to enable monitor out, False to disable monitor out)
+                    The new monitor out state (True to enable monitor out, False to disable monitor out).
         """
 
         self.command(f'OUTPut:MONitor:STATe {str(int(mon_out_state))}')
 
     def enable_mon_out(self):
-        """Sets the enable state of monitor out to True"""
+        """Sets the enable state of monitor out to True."""
 
         self.set_mon_out_state(True)
 
     def disable_mon_out(self):
-        """Sets the enable state of monitor out to False"""
+        """Sets the enable state of monitor out to False."""
 
         self.set_mon_out_state(False)
 
     def configure_mon_out(self, mon_out_source, mon_out_state=True):
-        """Configure the monitor output
+        """Configure the monitor output.
 
             Args:
                 mon_out_source (str):
-                    The new monitor out source ('M1', 'M2', or 'M3')
-
+                    The new monitor out source ('M1', 'M2', or 'M3').
                 mon_out_state (bool):
-                    The new monitor out state (True to enable monitor out, False to disable monitor out)
+                    The new monitor out state (True to enable monitor out, False to disable monitor out).
         """
 
         self.set_mon_out_mode(mon_out_source)
         self.set_mon_out_state(mon_out_state)
 
     def get_mon_out_scale(self):
         """Returns the monitor out scaling factor of the configured module."""
 
         return float(self.query('OUTPut:MONitor:SCALe?'))
 
     def get_head_cal_datetime(self):
-        """Returns the date and time of the head calibration"""
+        """Returns the date and time of the head calibration."""
 
         response = self.query('CALibration:DATE?').split(',')
         return datetime(int(response[0]), int(response[1]), int(response[2]), int(response[3]), int(response[4]), int(response[5]))
 
     def get_head_cal_temperature(self):
-        """Returns the temperature of the head calibration"""
+        """Returns the temperature of the head calibration."""
 
         return float(self.query('CALibration:TEMPerature?'))
 
     def get_head_self_cal_status(self):
-        """Returns the status of the last head self calibration"""
+        """Returns the status of the last head self calibration."""
 
         return self.query('CALibration:SCALibration:STATus?')
 
     def get_head_self_cal_datetime(self):
-        """Returns the datetime of the last head self calibration"""
+        """Returns the datetime of the last head self calibration."""
 
         response = self.query('CALibration:SCALibration:DATE?').split(',')
         return datetime(int(response[0]), int(response[1]), int(response[2]), int(response[3]), int(response[4]), int(response[5]))
 
     def get_head_self_cal_temperature(self):
-        """Returns the temperature of the last head self calibration"""
+        """Returns the temperature of the last head self calibration."""
 
         return float(self.query('CALibration:SCALibration:TEMPerature?'))
 
     def run_head_self_calibration(self):
-        """"Runs a self calibration for the head"""
+        """Runs a self calibration for the head."""
 
         self.command('CALibration:SCALibration:RUN')
 
     def reset_head_self_calibration(self):
-        """"Restore the factory self calibration"""
+        """"Restore the factory self calibration."""
 
         self.command('CALibration:SCALibration:RESet')
 
     def set_mon_out_manual_level(self, manual_level):
-        """Set the manual level of monitor out when the mode is MANUAL
+        """Set the manual level of monitor out when the mode is MANUAL.
 
             Args:
                 manual_level (float):
-                    The new monitor out manual level
+                    The new monitor out manual level.
         """
 
         self.command(f'OUTPut:MONitor:MLEVel {str(manual_level)}')
 
     def get_mon_out_manual_level(self):
-        """Returns the manual level of monitor out"""
+        """Returns the manual level of monitor out."""
 
         return float(self.query('OUTPut:MONitor:MLEVel?'))
 
     def configure_mon_out_manual_mode(self, manual_level, mon_out_state=True):
-        """Configures the monitor output for manual mode
+        """Configures the monitor output for manual mode.
 
             Args:
                 manual_level (float):
-                    The new monitor out manual level
-
+                    The new monitor out manual level.
                 mon_out_state (bool):
-                    The new monitor out state (True to enable monitor out, False to disable monitor out)
+                    The new monitor out state (True to enable monitor out, False to disable monitor out).
         """
 
         self.set_mon_out_manual_level(manual_level)
         self.set_mon_out_mode('MANUAL')
         self.set_mon_out_state(mon_out_state)
 
     def get_line_frequency(self):
-        """Returns the line frequency in Hz"""
+        """Returns the line frequency in Hz."""
 
         return float(self.query('SYSTem:LFRequency?'))
 
     def get_detected_line_frequency(self):
-        """Returns the detected line frequency in Hz"""
+        """Returns the detected line frequency in Hz."""
 
         return float(self.query('SYSTem:LFRequency:DETected?'))
 
     def get_line_frequency_detection_error_status(self):
         """Returns the line frequency detection error status. True if the frequency is out of bounds."""
 
         return bool(int(self.query('SYSTem:LFRequency:ERRor?')))
 
     def fetch_multiple(self, *data_sources):
-        """Gets a list of the latest values corresponding to the input data sources, and returns them as soon as
-        possible.
+        """Gets a list of the latest values corresponding to the input data sources, and returns them quickly.
 
             Args:
                 data_sources (SSMSystemDataSourceMnemonic or str, int):
                     Variable length list of pairs of (DATA_SOURCE, CHANNEL_INDEX).
-
             Returns:
-                Tuple of values corresponding to the given data sources
+                Tuple of values corresponding to the given data sources.
         """
 
         elements = ','.join(f'{mnemonic},{index}' for (mnemonic, index) in data_sources)
         response_values_with_indices = enumerate(self.query(f'FETCh? {elements}').split(','))
 
         return tuple(
             (self.data_source_lookup[data_sources[i][0].upper()])(value) for (i, value) in response_values_with_indices)
 
     def read_multiple(self, *data_sources):
-        """Initiates measurement of new values corresponding to the input data sources, and returns them after the
-        measurement is complete.
+        """Initiates measurement of new values corresponding to the input data sources.
+
+            Returns values after the measurement is complete.
 
             Args:
                 data_sources (SSMSystemReadDataSourceMnemonic or str, int):
                     Variable length list of pairs of (DATA_SOURCE, CHANNEL_INDEX).
-
             Returns:
-                Tuple of values corresponding to the given data sources
+                Tuple of values corresponding to the given data sources.
         """
 
         elements = ','.join(f'{mnemonic},{index}' for (mnemonic, index) in data_sources)
         response_values_with_indices = enumerate(self.query(f'READ? {elements}').split(','))
 
         return tuple(
             (self.data_source_lookup[data_sources[i][0].upper()])(value) for (i, value) in response_values_with_indices)
```

### Comparing `lakeshore-1.6.1/lakeshore/ssm_system_enums.py` & `lakeshore-1.7.0/lakeshore/ssm_system_enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Contains enumerations specific to the M81 """
+"""Contains enumerations specific to the M81."""
 
 from enum import Enum
 
 
 class SSMSystemEnums:
-    """Class for collecting the enumerations specific to the SSMSystem without bulking up that class size"""
+    """Class for collecting the enumerations specific to the SSMSystem without bulking up that class size."""
 
     class DataSourceMnemonic(str, Enum):
-        """Enumeration of M81 data source mnemonics"""
+        """Enumeration of M81 data source mnemonics."""
         RELATIVE_TIME = 'RTIMe'
         SOURCE_AMPLITUDE = 'SAMPlitude'
         SOURCE_OFFSET = 'SOFFset'
         SOURCE_FREQUENCY = 'SFRequency'
         SOURCE_RANGE = 'SRANge'
         SOURCE_VOLTAGE_LIMIT = 'SVLimit'
         SOURCE_CURRENT_LIMIT = 'SILimit'
@@ -34,15 +34,15 @@
         GENERAL_PURPOSE_OUTPUT_STATES = 'GPOStates'
 
         # Gets around having to use .value to access the string
         def __str__(self) -> str:
             return str.__str__(self)
 
     class ReadDataSourceMnemonic(str, Enum):
-        """Enumeration of M81 read data source mnemonics"""
+        """Enumeration of M81 read data source mnemonics."""
         MEASURE_DC = 'MDC'
         MEASURE_RMS = 'MRMs'
         MEASURE_POSITIVE_PEAK = 'MPPeak'
         MEASURE_NEGATIVE_PEAK = 'MNPeak'
         MEASURE_PEAK_TO_PEAK = 'MPTPeak'
         MEASURE_RANGE = 'MRANge'
 
@@ -59,14 +59,15 @@
         def __str__(self) -> str:
             return str.__str__(self)
 
     class SourceSweepType(str, Enum):
         """Class representing the available sweep types for a source module."""
         CURRENT_AMPLITUDE = 'CURRent'
         VOLTAGE_AMPLITUDE = 'VOLTage'
+        FREQUENCY = 'FREQuency'
 
         # Gets around having to use .value to access the string
         def __str__(self) -> str:
             return str.__str__(self)
 
     class SourceSweepSettings:
         """Class to configure a parameter sweep on a source module."""
@@ -77,26 +78,25 @@
             LOGARITHMIC = 'LOGARITHMIC'
 
             # Gets around having to use .value to access the string
             def __str__(self) -> str:
                 return str.__str__(self)
 
         class Direction(str, Enum):
-            """Class object representing the possible directions for sweeping"""
+            """Class object representing the possible directions for sweeping."""
             DOWN = 'DOWN'
             UP = 'UP'
 
             # Gets around having to use .value to access the string
             def __str__(self) -> str:
                 return str.__str__(self)
 
         def __init__(self, sweep_type, start, stop, points, dwell,
                      direction=Direction.UP, round_trip=False, spacing=SweepSpacing.LINEAR):
-            """
-            Constructor for SourceModuleSweepSettings class
+            """Constructor for SourceModuleSweepSettings class.
 
             Args:
                 sweep_type (SourceSweepType):
                     The type of sweep to perform.
                 start (float):
                     Sets the start value of the source sweep.
                 stop (float):
```

### Comparing `lakeshore-1.6.1/lakeshore/temperature_controllers.py` & `lakeshore-1.7.0/lakeshore/temperature_controllers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,152 +1,150 @@
-"""Implements a parent class for temperature controllers that contains shared methods between similar
-instruments."""
+"""Implements a parent class for temperature controllers that contains shared methods between similar instruments."""
 
 from enum import IntEnum
 import serial
 from .generic_instrument import GenericInstrument, InstrumentException, RegisterBase
 
 
 class AlarmSettings:
-    """Class used to disable or configure an alarm in conjunction with the set/get_alarm_parameters() method"""
+    """Class used to disable or configure an alarm in conjunction with the set/get_alarm_parameters() method."""
 
     def __init__(self, high_value, low_value, deadband, latch_enable, audible=None, visible=None, alarm_enable=None):
-        """Constructor for AlarmSettings class
+        """Constructor for AlarmSettings class.
 
             Args:
                 high_value (float):
-                    Sets the value the source is checked against to activate the high alarm
+                    Sets the value the source is checked against to activate the high alarm.
                 low_value (float):
                     Sets the value the source is checked against to activate low alarm.
                 deadband (float):
-                    Sets the value that the source must change outside of an alarm
+                    Sets the value that the source must change outside an alarm.
                     condition to deactivate an unlatched alarm.
                 latch_enable (bool):
-                    * Specifies a latched alarm
-                    * False = off, True = on
+                    Specifies a latched alarm.
+                    False = off, True = on
                 audible (bool):
-                    * Specifies if the internal speaker will beep when an alarm condition occurs
-                    * False = off, True = on
+                    Specifies if the internal speaker will beep when an alarm condition occurs.
+                    False = off, True = on
                 visible (bool):
-                    * Specifies if the Alarm LED on the instrument front panel will blink
-                        when an alarm condition occurs
-                    * False = off, True = on
+                    Specifies if the Alarm LED on the instrument front panel will blink when an alarm condition occurs.
+                    False = off, True = on
         """
         self.high_value = high_value
         self.low_value = low_value
         self.deadband = deadband
         self.latch_enable = latch_enable
         self.audible = audible
         self.visible = visible
         self.alarm_enable = alarm_enable
 
 
 class RelayControlMode(IntEnum):
-    """Relay operating mode enumeration"""
+    """Relay operating mode enumeration."""
     RELAY_OFF = 0
     RELAY_ON = 1
     ALARMS = 2
 
 
 class RelayControlAlarm(IntEnum):
     """Enumeration of the setting determining which alarm(s) cause a relay to close in alarm mode."""
     LOW_ALARM = 0
     HIGH_ALARM = 1
     BOTH_ALARMS = 2
 
 
 class InterfaceMode(IntEnum):
-    """Enumeration for the mode of the remote interface"""
+    """Enumeration for the mode of the remote interface."""
     LOCAL = 0
     REMOTE = 1
     REMOTE_LOCAL_LOCK = 2
 
 
 class HeaterError(IntEnum):
-    """Enumeration for possible errors flagged by the heater"""
+    """Enumeration for possible errors flagged by the heater."""
     NO_ERROR = 0
     HEATER_OPEN_LOAD = 1
     HEATER_SHORT = 2
 
 
 class CurveFormat(IntEnum):
-    """Enumerations specify formats for temperature sensor curves"""
+    """Enumerations specify formats for temperature sensor curves."""
     MILLIVOLT_PER_KELVIN = 1
     VOLTS_PER_KELVIN = 2
     OHMS_PER_KELVIN = 3
     LOG_OHMS_PER_KELVIN = 4
 
 
 class CurveTemperatureCoefficient(IntEnum):
-    """Enumerations specify positive/negative temperature sensor curve coefficients"""
+    """Enumerations specify positive/negative temperature sensor curve coefficients."""
     NEGATIVE = 1
     POSITIVE = 2
 
 
 class BrightnessLevel(IntEnum):
-    """Enumerator to specify the brightness level of an instrument display"""
+    """Enumerator to specify the brightness level of an instrument display."""
     QUARTER = 0
     HALF = 1
     THREE_QUARTERS = 2
     FULL = 3
 
 
 class AutotuneMode(IntEnum):
-    """Enumerator used to represent the different autotune control modes"""
+    """Enumerator used to represent the different autotune control modes."""
     P_ONLY = 0
     P_I = 1
     P_I_D = 2
 
 
 class HeaterResistance(IntEnum):
-    """Enumerator used to represent the different heater resistances"""
+    """Enumerator used to represent the different heater resistances."""
     HEATER_25_OHM = 1
     HEATER_50_OHM = 2
 
 
 class Polarity(IntEnum):
-    """Enumerator for unipolar or bipolar output operation"""
+    """Enumerator for unipolar or bipolar output operation."""
     UNIPOLAR = 0
     BIPOLAR = 1
 
 
 class DiodeCurrent(IntEnum):
-    """Enumerator used to represent diode current ranges"""
+    """Enumerator used to represent diode current ranges."""
     TEN_MICROAMPS = 0
     ONE_MILLIAMP = 1
 
 
 class HeaterOutputUnits(IntEnum):
-    """Enumerator used to represent heater output unit settings"""
+    """Enumerator used to represent heater output unit settings."""
     CURRENT = 1
     POWER = 2
 
 
 class Interface(IntEnum):
-    """Enumerator used to represent remote interface communication methods"""
+    """Enumerator used to represent remote interface communication methods."""
     USB = 0
     ETHERNET = 1
     IEEE488 = 2
 
 
 class InputSensorUnits(IntEnum):
-    """Enumerator used to represent temperature sensor unit options"""
+    """Enumerator used to represent temperature sensor unit options."""
     KELVIN = 1
     CELSIUS = 2
     SENSOR = 3
 
 
 class ControlTypes(IntEnum):
-    """Enumerator used to represent the control type settings"""
+    """Enumerator used to represent the control type settings."""
     AUTO_OFF = 0
     CONTINUOUS = 1
 
 
 class LanStatus(IntEnum):
-    """Represents the different status states for the lan connection"""
+    """Represents the different status states for the lan connection."""
     STATIC_IP = 0
     DHCP = 1
     AUT0_IP = 2
     ADDRESS_NOT_ACQUIRED_ERROR = 3
     DUPLICATE_INITIAL_IP_ERROR = 4
     DUPLICATE_ONGOING_IP_ERROR = 5
     CABLE_UNPLUGGED = 6
@@ -165,47 +163,43 @@
 class DisplayFieldsSize(IntEnum):
     """Enumeration of the display fields when mode is set to all inputs."""
     SMALL = 0
     LARGE = 1
 
 
 class CurveHeader:
-    """A class to configure the temperature sensor curve header parameters"""
+    """A class to configure the temperature sensor curve header parameters."""
 
     def __init__(self, curve_name, serial_number, curve_data_format, temperature_limit, coefficient):
-        """Constructor for CurveHeader class
+        """Constructor for CurveHeader class.
 
             Args:
                 curve_name (str):
-                    * Specifies curve name (limit of 15 characters)
-
+                    Specifies curve name (limit of 15 characters).
                 serial_number (str):
-                    * Specifies curve serial number (limit of 10 characters)
-
+                    Specifies curve serial number (limit of 10 characters).
                 curve_data_format (IntEnum):
-                    * Member of the instrument's CurveFormat IntEnum class
-                    * Specifies the curve data format
-
+                    Member of the instrument's CurveFormat IntEnum class.
+                    Specifies the curve data format.
                 temperature_limit (float):
-                    * Specifies the curve temperature limit in Kelvin
-
+                    Specifies the curve temperature limit in Kelvin.
                 coefficient (IntEnum):
-                    * Member of instrument's CurveTemperatureCoefficient IntEnum class
-                    * Specifies the curve temperature coefficient
+                    Member of instrument's CurveTemperatureCoefficient IntEnum class.
+                    Specifies the curve temperature coefficient.
 
         """
         self.curve_name = curve_name
         self.serial_number = serial_number
         self.curve_data_format = curve_data_format
         self.temperature_limit = temperature_limit
         self.coefficient = coefficient
 
 
 class StandardEventRegister(RegisterBase):
-    """Class object representing the standard event register"""
+    """Class object representing the standard event register."""
 
     bit_names = [
         "operation_complete",
         "",
         "query_error",
         "",
         "execution_error",
@@ -224,15 +218,15 @@
         self.query_error = query_error
         self.execution_error = execution_error
         self.command_error = command_error
         self.power_on = power_on
 
 
 class OperationEvent(RegisterBase):
-    """Class object representing the status byte register LSB to MSB"""
+    """Class object representing the status byte register LSB to MSB."""
 
     bit_names = [
         "alarm",
         "sensor_overload",
         "loop_2_ramp_done",
         "loop_1_ramp_done",
         "new_sensor_reading",
@@ -257,15 +251,15 @@
         self.new_sensor_reading = new_sensor_reading
         self.autotune_process_completed = autotune_process_completed
         self.calibration_error = calibration_error
         self.processor_communication_error = processor_communication_error
 
 
 class TemperatureController(GenericInstrument):
-    """Base class for all temperature controller instruments"""
+    """Base class for all temperature controller instruments."""
 
     # Enum aliases
     _relay_control_mode_enum = RelayControlMode
     _input_channel_enum = IntEnum
     _display_units_enum = IntEnum
     _heater_error_enum = HeaterError
     _curve_format_enums = CurveFormat
@@ -288,44 +282,44 @@
             raise InstrumentException('Query Error')
         if event_register.command_error:
             raise InstrumentException('Command Error: Invalid Command or Query')
         if event_register.execution_error:
             raise InstrumentException('Execution Error: Instrument not able to execute command or query.')
 
     def command(self, *commands, check_errors=True):
-        """Send a SCPI command or multiple commands to the instrument
+        """Sends an SCPI command or multiple commands to the instrument.
 
             Args:
                 commands (str):
-                    * A serial command
+                    A serial command.
 
             Kwargs:
                 check_errors (bool):
-                    * Chooses whether to check for and raise errors after sending a command. True by default.
+                    Chooses whether to check for and raise errors after sending a command. True by default.
 
         """
 
         # Group all commands and queries a single string with SCPI delimiters.
         command_string = ";:".join(commands)
 
         if check_errors:
             self.query(command_string)
         else:
             command_string += ";*OPC?"
             self.query(command_string, check_errors=False)
 
     def query(self, *queries, check_errors=True):
-        """Send a query to the instrument and return the response
+        """Send a query to the instrument and return the response.
 
             Args:
                 queries (str):
-                    * A serial query ending in a question mark
+                    A serial query ending in a question mark.
 
-            Return:
-               * The instrument query response as a string.
+            Returns:
+                The instrument query response as a string.
 
         """
 
         # Group all commands and queries a single string with SCPI delimiters.
         query_string = ";:".join(queries)
 
         # Append the query with an additional error buffer query.
@@ -340,796 +334,758 @@
             self._error_check(error_code)
             response = ';'.join(response_list)
 
         return response
 
     def get_standard_event_enable_mask(self):
         """Returns the names of the standard event enable register bits and their values.
-        These values determine which bits propagate to the standard event register"""
+
+            These values determine which bits propagate to the standard event register.
+        """
 
         response = self.query("*ESE?", check_errors=False)
         return StandardEventRegister.from_integer(response)
 
     def set_standard_event_enable_mask(self, register_mask):
         """Configures values of the standard event enable register bits.
-        These values determine which bits propagate to the standard event register
+
+            These values determine which bits propagate to the standard event register.
 
             Args:
                 register_mask (StandardEventRegister):
-                    An StandardEventRegister class object with all bits set to a value
+                    A StandardEventRegister class object with all bits set to a value.
 
         """
         integer_representation = register_mask.to_integer()
         self.command(f"*ESE {str(integer_representation)}")
 
     def clear_interface_command(self):
-        """Clears the bits in the Status Byte Register, Standard Event Status Register, and Operation Event Register,
-        and terminates all pending operations. Clears the interface, but not the controller."""
+        """Clears the bits in the SBR, SESR, OER, and terminates all operations.
+
+            Clears the bits in the Status Byte Register, Standard Event Status Register, and Operation Event Register.
+            Terminates all pending operations. Clears the interface, but not the controller."""
 
         self.command("*CLS")
 
     def reset_instrument(self):
-        """Sets controller parameters to power-up settings"""
+        """Sets controller parameters to power-up settings."""
 
         self.command("*RST")
 
     def set_service_request(self, register_mask):
-        """Manually enable/disable the mask of the corresponding status flag bit in the status
-        byte register
+        """Manually enable/disable the mask of the corresponding status-flag bit in the status byte register.
 
             Args:
                 register_mask (service_request_enable):
-                    * A service_request_enable class object with all bits configured
+                    A service_request_enable class object with all bits configured.
 
         """
         integer_representation = register_mask.to_integer()
         self.command(f"*SRE {str(integer_representation)}")
 
     def get_service_request(self):
-        """Returns the status byte register bits and their values as a class instance"""
+        """Returns the status byte register bits and their values as a class instance."""
 
         response = self.query("*SRE?")
         return self.service_request_enable.from_integer(response)
 
     def get_status_byte(self):
-        """Returns the status flag bits as a class instance without resetting the register"""
+        """Returns the status flag bits as a class instance without resetting the register."""
 
         response = self.query("*STB?")
         return self.status_byte_register.from_integer(response)
 
     def get_self_test(self):
-        """Instrument self test result completed at power up
+        """Instrument self test result completed at power up.
 
-            Return:
+            Returns:
                 (bool):
-                    * True = errors found
-                    * False = no errors found
+                    True = errors found.
+                    False = no errors found.
 
         """
         return bool(int(self.query("*TST?")))
 
     def get_kelvin_reading(self, input_channel):
-        """Returns the temperature value in kelvin of the given channel
+        """Returns the temperature value in kelvin of the given channel.
 
             Args:
                 input_channel:
-                    * Selects the channel to retrieve measurement
+                    Selects the channel to retrieve measurement.
 
         """
         return float(self.query(f"KRDG? {input_channel}"))
 
     def get_sensor_reading(self, input_channel):
         """Returns the sensor reading in the sensor's units.
 
             Returns:
                 reading (float):
-                    * The raw sensor reading in the units of the connected sensor
+                    The raw sensor reading in the units of the connected sensor.
 
         """
         return float(self.query(f"SRDG? {input_channel}"))
 
     def set_sensor_name(self, input_channel, sensor_name):
-        """Sets a given name to a sensor on the specified channel
+        """Sets a given name to a sensor on the specified channel.
 
             Args:
                 input_channel (str or int):
-                    * Specifies which input_channel channel to read from
-
+                    Specifies which input_channel channel to read from.
                 sensor_name(str):
-                    * Name user wants to give to the sensor on the specified channel
+                    Name user wants to give to the sensor on the specified channel.
 
         """
         self.command(f"INNAME {input_channel},\"{sensor_name}\"")
 
     def get_sensor_name(self, input_channel):
-        """Returns the name of the sensor on the specified channel
+        """Returns the name of the sensor on the specified channel.
 
             Args:
                 input_channel (str or int):
-                    * Specifies which input_channel channel to read from.
+                    Specifies which input_channel channel to read from.
 
             Returns:
-                name (str)
-                    * Name associated with the sensor
+                name (str):
+                    Name associated with the sensor.
 
         """
         return self.query(f"INNAME? {input_channel}")
 
     def set_curve_header(self, curve_number, curve_header):
-        """Configures the user curve header
+        """Configures the user curve header.
 
             Args:
                 curve_number:
-                    * Specifies which curve to configure
-
+                    Specifies which curve to configure.
                 curve_header (CurveHeader):
-                    * Instrument's CurveHeader class object containing the desired curve information
+                    Instrument's CurveHeader class object containing the desired curve information.
 
         """
         command_string = (f"CRVHDR {curve_number},\"{curve_header.curve_name}\",\"{curve_header.serial_number}\"," +
                         f"{curve_header.curve_data_format},{curve_header.temperature_limit},{curve_header.coefficient}")
         self.command(command_string)
 
     def get_curve_header(self, curve_number):
-        """Returns parameters set on a particular user curve header
+        """Returns parameters set on a particular user curve header.
 
             Args:
                 curve_number (int):
-                    * Specifies a curve to retrieve
+                    Specifies a curve to retrieve.
 
             Returns:
                 (CurveHeader):
-                    * A CurveHeader class object containing the curve information
+                    A CurveHeader class object containing the curve information.
 
         """
         response = self.query(f"CRVHDR? {curve_number}")
         curve_header = response.split(",")
         return CurveHeader(curve_header[0],
                            curve_header[1],
                            self._curve_format_enums(int(curve_header[2])),
                            float(curve_header[3]),
                            self._curve_coefficient_enums(int(curve_header[4])))
 
     def set_curve_data_point(self, curve, index, sensor_units, temperature, curvature=None):
-        """Configures a user curve point
+        """Configures a user curve point.
 
             Args:
                 curve (int or str):
-                    * Specifies which curve to configure
-
+                    Specifies which curve to configure.
                 index (int):
-                    * Specifies the points index in the curve
-
+                    Specifies the points index in the curve.
                 sensor_units (float):
-                    * Specifies sensor units for this point to 6 digits
-
+                    Specifies sensor units for this point to 6 digits.
                 temperature (float):
-                    * Specifies the corresponding temperature in Kelvin for this point to 6 digits
-
-                curvature (float)
-                    * Optional argument
-                    * Specify only if the point is part of a cubic spindle curve
-                    * The curvature value scale used to calculate spindle coefficients to 6 digits
+                    Specifies the corresponding temperature in Kelvin for this point to 6 digits.
+                curvature (float):
+                    Specify only if the point is part of a cubic spindle curve.
+                    The curvature value scale used to calculate spindle coefficients to 6 digits. Optional parameter.
 
         """
         if curvature:
             command_string = f"CRVPT {curve},{index},{sensor_units},{temperature},{curvature}"
         else:
             command_string = f"CRVPT {curve},{index},{sensor_units},{temperature}"
         self.command(command_string)
 
     def get_curve_data_point(self, curve, index):
-        """Returns a standard or user curve data point
+        """Returns a standard or user curve data point.
 
             Args:
                 curve (int):
-                    * Specifies which curve to query
-
+                    Specifies which curve to query.
                 index (int):
-                    * Specifies the points index in the curve
+                    Specifies the points index in the curve.
 
-            Return:
-                curve_point (tuple)
-                    * (sensor_units: float, temp_value: float, curvature_value: float (optional))
+            Returns:
+                curve_point (tuple):
+                    (sensor_units: float, temp_value: float, curvature_value: float (optional)).
 
         """
         curve_point = self.query(f"CRVPT? {curve},{index}").split(",")
         curve_point = [float(index) for index in curve_point]
         return tuple(curve_point)
 
     def get_curve(self, curve):
-        """Returns a list of all the data points in a particular curve
+        """Returns a list of all the data points in a particular curve.
 
             Args:
                 curve (int):
-                    * Specifies which curve to set
+                    Specifies which curve to set.
 
-            Return:
+            Returns:
                 data_points (list: tuple):
-                    * A list containing every point in the curve represented as a tuple
-                        * (sensor_units: float, temp_value: float, curvature_value: float (optional))
+                    A list containing every point in the curve represented as a tuple.
+                    (sensor_units: float, temp_value: float, curvature_value: float (optional)).
 
         """
         true_point_index = 200
         data_points = []
         for i in range(0, 200):
             point = self.get_curve_data_point(curve, i + 1)
             data_points.append(point)
             if point[0] != 0 or point[1] != 0:
                 true_point_index = i
 
         # Remove all extraneous points
         return data_points[:true_point_index]
 
     def set_curve(self, curve, data_points):
-        """Method to define a user curve using a list of data points
+        """Method to define a user curve using a list of data points.
 
             Args:
                 curve (int):
-                    * Specifies which curve to set
-
+                    Specifies which curve to set.
                 data_points (list):
-                    * A list containing every point in the curve represented as a tuple
-                        * (sensor_units: float, temp_value: float, curvature_value: float (optional))
+                    A list containing every point in the curve represented as a tuple.
+                    (sensor_units: float, temp_value: float, curvature_value: float (optional)).
 
         """
         self.delete_curve(curve)
 
         for index, point in data_points:
             if len(point) > 2:
                 self.set_curve_data_point(curve, index + 1, point[0], point[1], point[2])
             else:
                 self.set_curve_data_point(curve, index + 1, point[0], point[1])
 
     def delete_curve(self, curve):
-        """Deletes the user curve
+        """Deletes the user curve.
 
             Args:
                 curve (int):
-                    * Specifies a user curve to delete
+                    Specifies a user curve to delete.
 
         """
         self.command(f"CRVDEL {curve}")
 
     def set_alarm_parameters(self, input_channel, alarm_enable, alarm_settings=None):
-        """Configures the alarm parameters for an input
+        """Configures the alarm parameters for an input.
 
             Args:
                 input_channel (str):
-                    * Specifies which input to configure
-
+                    Specifies which input to configure.
                 alarm_enable (bool):
-                    * Specifies whether to turn on the alarm for the input, or turn the alarm off.
-
+                    Specifies whether to turn on the alarm for the input, or turn the alarm off.
                 alarm_settings (AlarmSettings):
-                    * See AlarmSettings class. Required only if alarm_enable is set to True
+                    See AlarmSettings class. Required only if alarm_enable is set to True.
 
         """
         if alarm_enable:
             command_string = (f"ALARM {input_channel},{int(alarm_enable)},{alarm_settings.high_value}," +
                             f"{alarm_settings.low_value},{alarm_settings.deadband}," +
                             f"{int(alarm_settings.latch_enable)},{int(alarm_settings.audible)},{int(alarm_settings.visible)}")
             self.command(command_string)
         else:
             self.command(f"ALARM {input_channel},{int(alarm_enable)},,,,,,")
 
     def get_alarm_parameters(self, input_channel):
-        """Returns the present state of all alarm parameters
+        """Returns the present state of all alarm parameters.
 
             Args:
                 input_channel (str):
-                    * Specifies which input to configure
+                    Specifies which input to configure.
 
-            Return:
+            Returns:
                 alarm_settings (AlarmSettings):
-                    * See AlarmSettings class
+                    See AlarmSettings class.
 
         """
         parameters = self.query(f"ALARM? {input_channel}").split(",")
         return AlarmSettings(float(parameters[1]), float(parameters[2]),
                              float(parameters[3]), bool(int((parameters[4]))),
                              audible=bool(int(parameters[5])), visible=bool(int(parameters[6])),
                              alarm_enable=bool(int(parameters[0])))
 
     def get_alarm_status(self, channel):
-        """Returns the high state and low state of the alarm for the specified channel
+        """Returns the high state and low state of the alarm for the specified channel.
 
                 Args:
                     channel (str or int)
-                        * Specifies which input channel to read from.
+                        Specifies which input channel to read from.
 
                 Return:
-                    (dict)
-                        * Keys:
-                        * "high_state": bool
-                            * True if high state is on, False if high state is off
-                        * "low_state" bool
-                            * True if low state is on, False if low state is off
+                    (dict):
+                        {"high_state": bool, "low_state" bool}
 
         """
         response = self.query(f"ALARMST? {channel}")
         separated_response = response.split(",")
         return {"high_state_enabled": bool(int(separated_response[0])),
                 "low_state_enabled": bool(int(separated_response[1]))}
 
     def reset_alarm_status(self):
         """Clears the high and low status of all alarms."""
         self.command("ALMRST")
 
     def _get_analog_output_percentage(self, output):
-        """Returns the output percentage of the analog voltage output
+        """Returns the output percentage of the analog voltage output.
 
             Args:
                 output (int):
-                    * Specifies which analog voltage output to query
+                    Specifies which analog voltage output to query.
 
-            Return:
+            Returns:
                 (float):
-                    * Analog voltage heater output percentage
+                    Analog voltage heater output percentage.
 
         """
         return float(self.query(f"AOUT? {output}"))
 
     def _set_autotune(self, output, mode):
-        """Initiates autotuning of the heater control loop.
+        """Initiates auto-tuning of the heater control loop.
 
             Args:
                 output (int):
-                    * Specifies the output associated with the loop to be Autotuned
-
+                    Specifies the output associated with the loop to be Auto-tuned.
                 mode (IntEnum):
-                    * Specifies the Autotune mode
-                    * Member of instrument's AutoTuneMode IntEnum class
+                    Specifies the Autotune mode.
+                    Member of instrument's AutoTuneMode IntEnum class.
 
         """
         self.command(f"ATUNE {output},{mode}")
 
         # Ensure autotune starts without error
         self._autotune_error()
 
     def _set_contrast_level(self, contrast_level):
-        """Sets the display contrast level on the front panel
+        """Sets the display contrast level on the front panel.
 
             Args:
-                contrast_level (int)
-                    * Contrast value
-                    * 1 - 32
+                contrast_level (int):
+                    Contrast value:
+                    1 - 32.
 
         """
         self.command(f"BRIGT {contrast_level}")
 
     def _get_contrast_level(self):
-        """Returns the contrast level of front display"""
+        """Returns the contrast level of front display."""
 
         return int(self.query("BRIGT?"))
 
     def _set_brightness(self, brightness):
-        """Method to set the front display brightness
+        """Method to set the front display brightness.
 
             Args:
-                brightness (IntEnum)
-                    * A member of the instrument's BrightnessLevel IntEnum class
+                brightness (IntEnum):
+                    A member of the instrument's BrightnessLevel IntEnum class.
 
         """
         self.command(f"BRIGT {brightness}")
 
     def _get_brightness(self):
-        """Method to query the front display brightness
+        """Method to query the front display brightness.
 
-            Return:
+            Returns:
                 (IntEnum):
-                    * A member of the instrument's BrightnessLevel IntEnum class
+                    A member of the instrument's BrightnessLevel IntEnum class.
 
         """
         return BrightnessLevel(int(self.query("BRIGT?")))
 
     def _get_celsius_reading(self, channel):
-        """Returns the temperature in celsius of any channel
+        """Returns the temperature in Celsius of any channel.
 
             Args:
-                channel (str)
-                    * "A" - "D" (in addition, "D1" - "D5" for 3062 option)
+                channel (str):
+                    "A" - "D" (in addition, "D1" - "D5" for 3062 option).
 
         """
         return float(self.query(f"CRDG? {channel}"))
 
     def _set_diode_excitation_current(self, channel, excitation_current):
-        """The 10 uA excitation current is the only calibrated excitation current, and is used in
-        almost all applications. The Model 336 will default the 10 uA current setting any time the
-        input sensor type is changed.
+        """Sets the excitation current of a specific channel.
+
+            The 10 uA excitation current is the only calibrated excitation current, and is used in
+            almost all applications. The Model 336 will default the 10 uA current setting any time the
+            input sensor type is changed.
 
             Args:
                 channel (str):
-                    * Specifies which sensor input to configure
-                    * "A" - "D"
+                    Specifies which sensor input to configure:
+                    "A" - "D".
 
                 excitation_current (IntEnum):
-                    * A member of the instrument's DiodeCurrent IntEnum class
+                    A member of the instrument's DiodeCurrent IntEnum class.
 
         """
         self.command(f"DIOCUR {channel},{excitation_current}")
 
     def _get_diode_excitation_current(self, channel):
         """Returns the diode excitation current setting as a string.
 
             Args:
                 channel (str):
-                    * Specifies which input to return
-                    * "A" - "D"
+                    Specifies which input to return:
+                    "A" - "D".
 
-            Return:
+            Returns:
                 (IntEnum):
-                    * A member of the instrument's DiodeCurrent IntEnum class
-                    * Diode excitation current
+                    A member of the instrument's DiodeCurrent IntEnum class.
+                    Diode excitation current.
 
         """
         response = int(self.query(f"DIOCUR? {channel}"))
         return DiodeCurrent(response)
 
     def set_display_field_settings(self, field, input_channel, display_units):
         """Configures a display field when the display is in custom mode.
 
             Args:
                 field (int):
-                    * Defines which field of the display is being configured
-
-                input_channel (IntEnum)
-                    * Defines which input to display.
-                    * A member of the instrument's InputChannel IntEnum class
-
-                display_units (IntEnum)
-                    * Defines which units to display reading in.
-                    * A member of the instrument's DisplayUnits IntEnum class
+                    Defines which field of the display is being configured.
+                input_channel (IntEnum):
+                    Defines which input to display.
+                    A member of the instrument's InputChannel IntEnum class.
+                display_units (IntEnum):
+                    Defines which units to display reading in.
+                    A member of the instrument's DisplayUnits IntEnum class.
 
         """
         self.command(f"DISPFLD {field},{input_channel},{display_units}")
 
     def get_display_field_settings(self, field):
         """Returns the settings of the specified display field when display is in Custom mode.
 
             Args:
                 field (int)
-                    Defines which field of the display to retrieve settings from
+                    Defines which field of the display to retrieve settings from.
 
-            Return:
+            Returns:
                 (dict):
-                    * See set_display_field_settings method
-                    * Keys:
-                    * "input_channel": IntEnum
-                    * "display_units": IntEnum
+                    See set_display_field_settings method.
+                    {"input_channel": IntEnum, "display_units": IntEnum}
 
         """
         separated_settings = self.query(f"DISPFLD? {field}").split(",")
         return {'input_channel': self._input_channel_enum(int(separated_settings[0])),
                 'display_units': self._display_units_enum(int(separated_settings[1]))}
 
     def _set_filter(self, input_channel, filter_enable, data_points, reset_threshold):
-        """Configures the input_channel filter parameter
+        """Configures the input_channel filter parameter.
 
             Args:
                 input_channel (int or str):
-                    * Specifies which input channel to configure
-
+                    Specifies which input channel to configure.
                 filter_enable (bool):
-                    * Specified whether the filtering function is enabled or not
-
+                    Specified whether the filtering function is enabled or not.
                 data_points (int):
-                    * Specifies how many points the filter function uses
-                    * 2 - 64
-
+                    Specifies how many points the filter function uses:
+                    2 - 64.
                 reset_threshold (int):
-                    * Specifies what percent of full scale reading limits the filtering function.
-                    * When a raw reading differs from a filtered value by more than this threshold,
-                        the filter averaging resets.
-                    * Options are:
-                        * 1% - 10%
+                    Specifies what percent of full scale reading limits the filtering function.
+                    When a raw reading differs from a filtered value by more than this threshold,
+                    the filter averaging resets.
+                    Options are:
+                    1% - 10%.
 
         """
         self.command(f"FILTER {input_channel},{int(filter_enable)},{data_points},{reset_threshold}")
 
     def _get_filter(self, input_channel):
-        """Returns the input_channel filter configuration
+        """Returns the input_channel filter configuration.
 
             Args:
                 input_channel (int or str):
-                    * Specifies which input channel to configure
+                    Specifies which input channel to configure.
 
-            Return:
+            Returns:
                 (dict)
-                    * Keys:
-                    * "filter_enable": bool
-                        * Specified whether the filtering function is enabled or not
-
-                    * "data_points": int
-                        * Specifies how many points the filter function uses
-
-                    * "reset_threshold": int
-                        * 1% - 10%
-                        * Specifies what percent of full scale reading limits the filtering function. When a raw
-                          reading differs from a filtered value by more than this threshold, the filter averaging
-                          resets.
+                    {"filter_enable": bool, "data_points": int, "reset_threshold": int}
+                        filter_enable: Specified whether the filtering function is enabled or not.
+                        data_points: Specifies how many points the filter function uses.
+                        reset_threshold: Specifies what percent of full scale reading limits the filtering function. When a
+                        raw reading differs from a filtered value by more than this threshold, the filter averaging
+                        resets (1% - 10%).
 
         """
         filter_settings = self.query(f"FILTER? {input_channel}").split(",")
         return {"filter_enable": bool(int(filter_settings[0])),
                 "data_points": int(filter_settings[1]),
                 "reset_threshold": int(filter_settings[2])}
 
     def get_heater_output(self, output):
-        """Sample heater output in percent, scale is dependent upon the instrument used and heater configuration
+        """Sample heater output in percent, scale is dependent upon the instrument used and heater configuration.
 
             Args:
                 output (int):
-                    * Heater output to query
+                    Heater output to query.
 
-            Return:
+            Returns:
                 (float):
-                    * percent of full scale current/voltage/power
+                    percent of full scale current/voltage/power.
 
         """
         return float(self.query(f"HTR? {output}"))
 
     def get_heater_status(self, output):
-        """Returns the heater error code state, error is cleared upon querying the heater status
+        """Returns the heater error code state, error is cleared upon querying the heater status.
 
             Args:
                 output (int):
-                    * Specifies which heater output to query (1 or 2)
+                    Specifies which heater output to query (1 or 2).
 
-            Return:
+            Returns:
                 (IntEnum):
-                     * Object of instrument's HeaterError type
+                    Object of instrument's HeaterError type.
 
         """
         status_code = int(self.query(f"HTRST? {output}"))
         return self._heater_error_enum(status_code)
 
     def set_ieee_488(self, address):
-        """Specifies the IEEE address
+        """Specifies the IEEE address.
 
             Args:
                 address (int):
-                    * 1-30 (0 and 31 reserved)
+                    1-30 (0 and 31 reserved).
 
         """
         self.command(f"IEEE {address}")
 
     def get_ieee_488(self):
-        """Returns the IEEE address set
+        """Returns the IEEE address set.
 
-            Return:
+            Returns:
                 address (int):
-                    * 1-30 (0 and 31 reserved)
+                    1-30 (0 and 31 reserved).
 
         """
         return int(self.query("IEEE?"))
 
     def set_input_curve(self, input_channel, curve_number):
-        """Specifies the curve an input uses for temperature conversion
+        """Specifies the curve an input uses for temperature conversion.
 
             Args:
                 input_channel (str or int):
-                    * Specifies which input to configure
-
+                    Specifies which input to configure.
                 curve_number (int):
-                    * 0 = none, 1-20 = standard curves, 21-59 = user curves
+                    0 = none, 1-20 = standard curves, 21-59 = user curves.
 
         """
         self.command(f"INCRV {input_channel},{curve_number}")
         # Check that the user mapped an input to a curve (not just set the input to no curve)
         if curve_number != 0:
             # Query the curve mapped to input_channel, if the query returns zero,
             # an invalid curve was selected for the specified input
             set_curve = self.get_input_curve(input_channel)
             if set_curve == 0:
                 raise InstrumentException("The specified curve type does not match the configured input type")
 
     def get_input_curve(self, input_channel):
-        """Returns the curve number being used for a given input
+        """Returns the curve number being used for a given input.
 
             Args:
                 input_channel (str or int):
-                    * Specifies which input to query
-            Return:
+                    Specifies which input to query.
+
+            Returns:
                 curve_number (int):
-                    * 0-59
+                    0-59.
 
         """
         return int(self.query(f"INCRV? {input_channel}"))
 
     def _set_interface(self, interface):
-        """Selects the remote interface for the instrument
+        """Selects the remote interface for the instrument,
 
             Args:
                 interface (IntEnum):
-                    * Member of instrument's Interface IntEnum class
+                    Member of instrument's Interface IntEnum class,
 
         """
         self.command(f"INTSEL {interface}")
 
     def _get_interface(self):
-        """Returns the remote interface for the instrument
+        """Returns the remote interface for the instrument.
 
-            Return:
+            Returns:
                 (IntEnum):
-                    * Member of instrument's Interface IntEnum class
+                    Member of instrument's Interface IntEnum class.
 
         """
         interface_response = self.query("INTSEL?")
         return Interface(int(interface_response))
 
     def set_led_state(self, state):
         """Sets the front panel LEDs to on or off.
 
             Args:
-                state (bool)
-                    * Sets the LEDs to functional or nonfunctional
-                    * False if disabled, True enabled.
+                state (bool):
+                    Sets the LEDs to functional or nonfunctional.
+                    False if disabled, True enabled.
 
         """
         self.command(f"LEDS {int(state)}")
 
     def get_led_state(self):
-        """Returns whether or not front panel LEDs are enabled.
+        """Returns whether front panel LEDs are enabled.
 
-            Return:
-                (bool)
-                    * Specifies whether front panel LEDs are functional
-                    * False if disabled, True enabled.
+            Returns:
+                (bool):
+                    Specifies whether front panel LEDs are functional.
+                    False if disabled, True enabled.
 
         """
         return bool(int(self.query("LEDS?")))
 
     def set_keypad_lock(self, state, code):
         """Locks or unlocks front panel keypad (except for alarms and disabling heaters).
 
             Args:
-                state (bool)
-                    * Sets the keypad to locked or unlocked. Options are:
-                    * False for unlocked or True for locked
-
-                code (int)
-                    * Specifies 3 digit lock-out code. Options are:
-                    * 000 - 999
+                state (bool):
+                    Sets the keypad to locked or unlocked. Options are:
+                    False for unlocked or True for locked.
+                code (int):
+                    Specifies 3 digit lock-out code. Options are:
+                    000 - 999.
 
         """
         self.command(f"LOCK {int(state)},{code}")
 
     def get_keypad_lock(self):
         """Returns the state of the keypad lock and the lock-out code.
 
-            Return:
+            Returns:
                 (dict):
-                    * Keys:
-                        * "state": bool
-                        * "code": int
+                    {"state": bool, "code": int}
 
         """
         output_string = self.query("LOCK?")
         separated_response = output_string.split(",")
         return {'state': bool(int(separated_response[0])),
                 'code': int(separated_response[1])}
 
     def get_min_max_data(self, input_channel):
-        """Returns the minimum and maximum data from an input
+        """Returns the minimum and maximum data from an input.
 
             Args:
                 input_channel (str):
-                    * Specifies which input to query
+                    Specifies which input to query.
 
-            Return:
+            Returns:
                 (dict):
-                    * keys:
-                        * "minimum": float
-                        * "maximum": float
+                    {"minimum": float, "maximum": float}
 
         """
         min_max_data = self.query(f"MDAT? {input_channel}").split(",")
         return {"minimum": float(min_max_data[0]),
                 "maximum": float(min_max_data[1])}
 
     def reset_min_max_data(self):
-        """Resets the minimum and maximum input data"""
+        """Resets the minimum and maximum input data."""
         self.command("MNMXRST")
 
     def set_remote_interface_mode(self, mode):
-        """Places the instrument in one of three interface modes
+        """Places the instrument in one of three interface modes.
 
             Args:
                 mode (IntEnum):
-                    * A member of the instrument's InterfaceMode IntEnum class
+                    A member of the instrument's InterfaceMode IntEnum class.
 
         """
         self.command(f"MODE {mode}")
 
     def get_remote_interface_mode(self):
-        """Returns the state of the interface mode
+        """Returns the state of the interface mode.
 
-            Return:
+            Returns:
                 (IntEnum):
-                    * A member of the instrument's InterfaceMode IntEnum class
+                    A member of the instrument's InterfaceMode IntEnum class.
 
         """
         mode = int(self.query("MODE?"))
         return InterfaceMode(mode)
 
     def set_manual_output(self, output, value):
-        """When instrument is in closed loop PID, Zone, or Open Loop modes a manual output may be set
+        """When instrument is in closed loop PID, Zone, or Open Loop modes a manual output may be set.
 
             Args:
                 output (int):
-                    * Specifies output to configure
-
+                    Specifies output to configure.
                 value (float):
-                    * Specifies value for manual output in percent
+                    Specifies value for manual output in percent.
 
         """
         self.command(f"MOUT {output},{value}")
 
     def get_manual_output(self, output):
-        """Returns the manual output value in percent
+        """Returns the manual output value in percent.
 
             Args:
                 output (int):
-                    * Specifies output to query
+                    Specifies output to query.
 
-            Return:
+            Returns:
                 (float):
-                    * Manual output percent
+                    Manual output percent.
 
         """
         return float(self.query(f"MOUT? {output}"))
 
     def _set_network_settings(self, dhcp_enable, auto_ip_enable, ip_address, sub_mask, gateway, primary_dns,
                               secondary_dns, pref_host, pref_domain, description):
-        """Network class constructor
+        """Network class constructor.
 
             Args:
                 dhcp_enable (bool):
-                    * Enable or disable DHCP
-
+                    Enable or disable DHCP.
                 auto_ip_enable (bool):
-                    * Enable or disable dynamically configured link-local addressing (Auto IP)
-
+                    Enable or disable dynamically configured link-local addressing (Auto IP).
                 ip_address (str):
-                    * IP address for static configuration.
-
+                    IP address for static configuration.
                 sub_mask (str):
-                    * Subnet mask for static configuration.
-
+                    Subnet mask for static configuration.
                 gateway (str):
-                    * Gateway address for static configuration.
-
+                    Gateway address for static configuration.
                 primary_dns (str):
-                    * Primary DNS address for static configuration.
-
+                    Primary DNS address for static configuration.
                 secondary_dns (str):
-                    * Secondary DNS address for static configuration.
-
+                    Secondary DNS address for static configuration.
                 pref_host (str):
-                    * Preferred Hostname (15 character maximum)
-
+                    Preferred Hostname (15 character maximum).
                 pref_domain (str):
-                    * Preferred Domain name (64 character maximum)
-
+                    Preferred Domain name (64 character maximum).
                 description (str):
-                    * Instrument description (32 character maximum)
+                    Instrument description (32 character maximum).
 
         """
         command_string = (f"NET {int(dhcp_enable)},{int(auto_ip_enable)},{ip_address}," +
                         f"{sub_mask},{gateway},{primary_dns},{secondary_dns},\"{pref_host}\"," +
                         f"\"{pref_domain}\",\"{description}\"")
         self.command(command_string)
 
     def _get_network_settings(self):
-        """Method to retrieve the IP settings
+        """Method to retrieve the IP settings.
 
-            Return:
+            Returns:
                 (dict):
-                    * See set_network_settings arguments
+                    See set_network_settings arguments.
 
         """
         network_response = self.query("NET?").split(",")
         return {"dhcp_enable": bool(int(network_response[0])),
                 "auto_ip_enable": bool(int(network_response[1])),
                 "ip_address": network_response[2],
                 "sub_mask": network_response[3],
@@ -1137,46 +1093,30 @@
                 "primary_dns": network_response[5],
                 "secondary_dns": network_response[6],
                 "pref_host": network_response[7],
                 "pref_domain": network_response[8],
                 "description": network_response[9]}
 
     def _get_network_configuration(self):
-        """Method to return the configured ethernet parameters
+        """Method to return the configured ethernet parameters.
 
             Return:
-                (dict)
-                    * Keys:
-                    * "lan_status": LanStatus
-                        * Current status of the ethernet connection
-                        * Member of the instrument's LanStatus IntEnum class
-
-                    * "ip_address": str
-                        * Configured IP address
-
-                    * "sub_mask": str
-                        * Configured subnet mask
-
-                    * "gateway": str
-                        * Configured gateway address
-
-                    * "primary_dns": str
-                        * Configured primary DNS address
-
-                    * "secondary_dns": str
-                        * Configured secondary DNS address
-
-                    * "hostname" str
-                        * Assigned hostname
-
-                    * "domain": str
-                        * Assigned domain
-
-                    * "mac_address": str
-                        * Module MAC address
+                (dict):
+                    {"lan_status": LanStatus, "ip_address": str, "sub_mask": str, "gateway": str, "primary_dns": str,
+                        "secondary_dns": str, "hostname" str, "domain": str, "mac_address": str}
+                        lan_status: Current status of the ethernet connection. Member of the instrument's LanStatus
+                        IntEnum class.
+                        ip_address: Configured IP address.
+                        sub_mask: Configured subnet mask.
+                        gateway: Configured gateway address.
+                        primary_dns: Configured primary DNS address.
+                        secondary_dns: Configured secondary DNS address.
+                        hostname: Assigned hostname.
+                        domain: Assigned domain.
+                        mac_address: Module MAC address.
 
         """
         ethernet = self.query("NETID?").split(",")
         return {"lan_status": LanStatus(int(ethernet[0])),
                 "ip_address": ethernet[1],
                 "sub_mask": ethernet[2],
                 "gateway": ethernet[3],
@@ -1190,26 +1130,29 @@
         """Returns the names of the operation condition register bits and their values."""
 
         response = self.query("OPST?")
         return OperationEvent.from_integer(response)
 
     def _get_operation_event_enable(self):
         """Returns the names of the operation event enable register and their values.
-        These values determine which bits propagate to the operation condition register."""
+
+            These values determine which bits propagate to the operation condition register.
+        """
 
         response = self.query("OPSTE?")
         return OperationEvent.from_integer(response)
 
     def _set_operation_event_enable(self, register_mask):
         """Configures values of the operation event enable register bits.
-        These values determine which bits propagate to the standard event register.
+
+            These values determine which bits propagate to the standard event register.
 
             Args:
                 register_mask (OperationEvent):
-                    * An OperationEvent class object with all bits configured true or false
+                    An OperationEvent class object with all bits configured true or false.
 
         """
         integer_representation = register_mask.to_integer()
         self.command(f"OPSTE {integer_representation}")
 
     def _get_operation_event(self):
         """Returns the names of the operation event register bits and their values."""
@@ -1219,432 +1162,391 @@
         return status_register
 
     def set_heater_pid(self, output, gain, integral, derivative):
         """Configure the closed loop control parameters of the heater output.
 
             Args:
                 output (int):
-                     * Specifies which output's control loop to configure
-
+                    Specifies which output's control loop to configure.
                 gain (float):
-                    * Proportional term in PID control.
-                    * This controls how strongly the control output reacts to the present error.
-
+                    Proportional term in PID control.
+                    This controls how strongly the control output reacts to the present error.
                 integral (float):
-                    * Integral term in PID control.
-                    * This controls how strongly the control output reacts to the past error history
-
+                    Integral term in PID control.
+                    This controls how strongly the control output reacts to the past error history.
                 derivative (float):
-                    * Derivative term in PID control
-                    * This value controls how quickly the present field setpoint will transition to a new setpoint.
-                    * The ramp rate is configured in field units per second.
+                    Derivative term in PID control.
+                    This value controls how quickly the present field set point will transition to a new set-point.
+                    The ramp rate is configured in field units per second.
 
         """
         self.command(f"PID {output},{gain},{integral},{derivative}")
 
     def get_heater_pid(self, output):
-        """Returns the closed loop control parameters of the heater output
+        """Returns the closed loop control parameters of the heater output.
 
             Args:
                 output (int):
-                    * Specifies which output's control loop to query
+                    Specifies which output's control loop to query.
 
-            Return:
+            Returns:
                 (dict):
-                    * Keys:
-                    * "gain": float
-                        * Proportional term in PID control.
-
-                    * "integral": float
-                        * Integral term in PID control.
-
-                    * "ramp_rate": float
-                        * Derivative term in PID control
+                    {"gain": float, "integral": float, "ramp_rate": float}
+                        gain: Proportional term in PID control.
+                        integral: Integral term in PID control.
+                        ramp_rate: Derivative term in PID control.
 
         """
         pid_values = self.query(f"PID? {output}")
         pid_values = pid_values.split(",")
         return {"gain": float(pid_values[0]),
                 "integral": float(pid_values[1]),
                 "ramp_rate": float(pid_values[2])}
 
     def set_setpoint_ramp_parameter(self, output, ramp_enable, rate_value):
-        """Sets the control loop of a particular output
+        """Sets the control loop of a particular output.
 
             Args:
                 output (int):
-                    * Specifies which output's control loop to configure
-
+                    Specifies which output's control loop to configure.
                 ramp_enable (bool):
-                    * Specifies whether ramping is off or on (False = Off or True = On)
-
+                    Specifies whether ramping is off or on (False = Off or True = On).
                 rate_value (float):
-                    * 0.1 to 100
-                    * Specifies setpoint ramp rate in kelvin per minute.
-                    * The rate is always positive but will respond to ramps up or down.
-                    * A rate of 0 is interpreted as infinite, and will respond as if setpoint ramping were off
+                    Specifies set-point ramp rate in kelvin per minute.
+                    The rate is always positive but will respond to ramps up or down.
+                    A rate of 0 is interpreted as infinite, and will respond as if set-point ramping were off.
+                    (0.1 to 100)
 
         """
         self.command(f"RAMP {output},{int(ramp_enable)},{rate_value}")
 
     def get_setpoint_ramp_parameter(self, output):
-        """Returns the control loop parameters of a particular output
+        """Returns the control loop parameters of a particular output.
 
             Args:
                 output (int):
-                    * Specifies which output's control loop to return
+                    Specifies which output's control loop to return.
 
-            Return:
+            Returns:
                 (dict):
-                    * Keys:
-                    * "ramp_enable": bool
-                    * "rate_value": float
+                    {"ramp_enable": bool, "rate_value": float}
 
         """
         parameters = self.query(f"RAMP? {output}").split(",")
         return {"ramp_enable": bool(int(parameters[0])),
                 "rate_value": float(parameters[1])}
 
     def get_setpoint_ramp_status(self, output):
-        """"Returns whether or not the setpoint is ramping
+        """Returns whether the set-point is ramping.
 
             Args:
                 output (int):
-                    * Specifies which output's control loop to query
+                    Specifies which output's control loop to query.
 
-            Return:
+            Returns:
                 (bool):
-                    * Ramp status
-                    * False = Not ramping, True = Ramping
+                    Ramp status.
+                    False = Not ramping, True = Ramping.
 
         """
         return bool(int(self.query(f"RAMPST? {output}")))
 
     def turn_relay_on(self, relay_number):
         """Turns the specified relay on.
 
             Args:
                 relay_number (int):
-                    * The relay to turn on.
-                    * Options are:
-                        * 1 or 2
+                    The relay to turn on.
+                    Options are:
+                    1 or 2.
 
         """
         self.command(f"RELAY {relay_number},1,,")
 
     def turn_relay_off(self, relay_number):
         """Turns the specified relay off.
 
             Args:
                 relay_number (int):
-                    * The relay to turn off.
-                    * Options are:
-                        * 1 or 2
+                    The relay to turn off.
+                    Options are:
+                    1 or 2.
 
         """
         self.command(f"RELAY {relay_number},0,,")
 
     def set_relay_alarms(self, relay_number, activating_input_channel, alarm_relay_trigger_type):
         """Sets a relay to turn on and off automatically based on the state of the alarm of the specified input channel.
 
             Args:
                 relay_number (int):
-                    * The relay to configure.
-                    * Options are:
-                        * 1 or 2
-
+                    The relay to configure.
+                    Options are:
+                    1 or 2.
                 activating_input_channel (str or int):
-                    * Specifies which input alarm activates the relay
-
+                    Specifies which input alarm activates the relay.
                 alarm_relay_trigger_type (RelayControlAlarm):
-                    * Specifies the type of alarm that triggers the relay
+                    Specifies the type of alarm that triggers the relay.
 
         """
         self.command(f"RELAY {relay_number},2,{activating_input_channel},{alarm_relay_trigger_type}")
 
     def get_relay_alarm_control_parameters(self, relay_number):
-        """Returns the relay alarm configuration for either of the two configurable relays. Relay must be
-        configured for alarm mode to retrieve parameters.
+        """Returns the relay alarm configuration for either of the two configurable relays.
+
+            Relay must be configured for alarm mode to retrieve parameters.
 
             Args:
                 relay_number (int)
-                    * Specifies which relay to query
-                    * Options are:
-                        * 1 or 2
+                    Specifies which relay to query.
+                    Options are:
+                    1 or 2.
 
-            Return:
+            Returns:
                 (dict):
-                    * Keys:
-                    * "activating_input_channel": str
-                    * "alarm_relay_trigger_type": RelayControlAlarm
+                    {"activating_input_channel": str, "alarm_relay_trigger_type": RelayControlAlarm}
 
         """
         relay_config = self.query(f"RELAY? {relay_number}").split(",")
         activating_input_channel = relay_config[1]
         alarm_relay_trigger_type = RelayControlAlarm(int(relay_config[2]))
         return {'activating_input_channel': activating_input_channel,
                 'alarm_relay_trigger_type': alarm_relay_trigger_type}
 
     def get_relay_control_mode(self, relay_number):
         """Returns the configured mode of the specified relay.
 
             Args:
                 relay_number (int):
-                    * Specifies which relay to query
-                    * Options are:
-                        * 1 or 2
+                    Specifies which relay to query.
+                    Options are:
+                    1 or 2.
 
             Returns:
                 (IntEnum):
-                    * The configured mode of the relay
-                    * Represented as a member of the instrument's RelayControlMode IntEnum class
+                    The configured mode of the relay.
+                    Represented as a member of the instrument's RelayControlMode IntEnum class.
 
         """
         relay_settings = self.query(f"RELAY? {str(relay_number)}")
         split_relay_settings = relay_settings.split(",")
         return self._relay_control_mode_enum(int(split_relay_settings[0]))
 
     def get_relay_status(self, relay_channel):
         """Returns whether the relay at the specified channel is On or Off.
 
             Args:
-                relay_channel (int)
-                    * The relay channel to query.
+                relay_channel (int):
+                    The relay channel to query.
 
             Returns:
-                (bool)
-                    * True if relay is on, False if relay is off.
+                (bool):
+                    True if relay is on, False if relay is off.
 
         """
         return bool(int(self.query(f"RELAYST? {relay_channel}")))
 
     def _set_soft_cal_curve_dt_470(self, curve_number, serial_number, calibration_point_1=(4.2, 1.62622),
                                    calibration_point_2=(77.35, 1.02032), calibration_point_3=(305, 0.50691)):
         """Creates a SoftCal curve from any 1-3 temperature/sensor points using the preconfigured DT-470 curve.
-            When a calibration point other than one or more the default value(s) is entered a SoftCal curve is generated
+
+            When a calibration point other than one or more the default value(s) is entered a SoftCal curve is
+            generated.
 
             Args:
                 curve_number (int):
-                    * The curve number to save the generated curve to.
-                    * Options are:
-                        * 21 - 59
-
+                    The curve number to save the generated curve to.
+                    Options are:  21 - 59.
                 serial_number (str):
-                    * Specifies the curve serial number.
-                    * Limited to 10 characters.
-
+                    Specifies the curve serial number.
+                    Limited to 10 characters.
                 calibration_point_1 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
-
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional parameter.
                 calibration_point_2 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
-
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
                 calibration_point_3 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
 
         """
         command_string = (f"SCAL {1},{curve_number},{serial_number},{calibration_point_1[0]}," +
                         f"{calibration_point_1[1]},{calibration_point_2[0]},{calibration_point_2[1]}," +
                         f"{calibration_point_3[0]},{calibration_point_3[1]}")
         self.command(command_string)
 
     def _set_soft_cal_curve_pt_100(self, curve_number, serial_number, calibration_point_1=(77.35, 20.234),
                                    calibration_point_2=(305, 112.384), calibration_point_3=(480, 178.353)):
         """Creates a SoftCal curve from any 1-3 temperature/sensor points using the preconfigured PT-100 curve.
-            When a calibration point other than one or more the default value(s) is entered a SoftCal curve is generated
+
+            When a calibration point other than one or more the default value(s) is entered a SoftCal curve is
+            generated.
 
             Args:
                 curve_number (int):
-                    * The curve number to save the generated curve to.
-                    * Options are:
-                        * 21 - 59
-
+                    The curve number to save the generated curve to.
+                    Options are:
+                    21 - 59.
                 serial_number (str):
-                    * Specifies the curve serial number.
-                    * Limited to 10 characters.
-
+                    Specifies the curve serial number.
+                    Limited to 10 characters.
                 calibration_point_1 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
-
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
                 calibration_point_2 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
-
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
                 calibration_point_3 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
 
         """
         command_string = (f"SCAL {6},{curve_number},{serial_number}," +
                         f"{calibration_point_1[0]},{calibration_point_1[1]}," +
                         f"{calibration_point_2[0]},{calibration_point_2[1]}," +
                         f"{calibration_point_3[0]},{calibration_point_3[1]}")
         self.command(command_string)
 
     def _set_soft_cal_curve_pt_1000(self, curve_number, serial_number, calibration_point_1=(77.35, 202.34),
                                     calibration_point_2=(305, 1123.84), calibration_point_3=(480, 1783.53)):
         """Creates a SoftCal curve from any 1-3 temperature/sensor points using the preconfigured PT-1000 curve.
-            When a calibration point other than one or more the default value(s) is entered a SoftCal curve is generated
+
+            When a calibration point other than one or more the default value(s) is entered a SoftCal curve is
+            generated.
 
             Args:
                 curve_number (int):
-                    * The curve number to save the generated curve to.
-                    * Options are:
-                        * 21 - 59
-
+                    The curve number to save the generated curve to.
+                    Options are:
+                    21 - 59.
                 serial_number (str):
-                    * Specifies the curve serial number.
-                    * Limited to 10 characters.
-
+                    Specifies the curve serial number.
+                    Limited to 10 characters.
                 calibration_point_1 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
-
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
                 calibration_point_2 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
-
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
                 calibration_point_3 (tuple):
-                    * Tuple of two floats in the form (temperature_value, sensor_value)
-                    * Optional parameter
+                    Tuple of two floats in the form (temperature_value, sensor_value). Optional Parameter.
 
         """
         command_string = (f"SCAL {7},{curve_number},{serial_number}," +
                         f"{calibration_point_1[0]},{calibration_point_1[1]}," +
                         f"{calibration_point_2[0]},{calibration_point_2[1]}," +
                         f"{calibration_point_3[0]},{calibration_point_3[1]}")
         self.command(command_string)
 
     def set_control_setpoint(self, output, value):
-        """Control settings, that is, P, I, D, and Setpoint, are assigned to outputs,
-        which results in the settings being applied to the control loop formed by the
-        output and its control input
+        """Set set-point for specific output's control loop.
+
+            Control settings, that is, P, I, D, and Set-point, are assigned to outputs,
+            which results in the settings being applied to the control loop formed by the
+            output and its control input.
 
             Args:
                 output (int):
-                    * Specifies which output's control loop to configure
-
+                    Specifies which output's control loop to configure.
                 value (float):
-                    The value for the setpoint (in the preferred units of the control loop sensor)
+                    The value for the set-point (in the preferred units of the control loop sensor).
 
         """
         self.command(f"SETP {output},{value}")
 
     def get_control_setpoint(self, output):
-        """Returns the value for a given control output
+        """Returns the value for a given control output.
 
             Args:
                 output (int):
-                    * Specifies which output's control loop to query (1 or 2)
+                    Specifies which output's control loop to query (1 or 2).
 
-            Return:
+            Returns:
                 value (float):
-                    * The value for the setpoint (in the preferred units of the control loop sensor)
+                    The value for the set-point (in the preferred units of the control loop sensor).
 
         """
         return float(self.query(f"SETP? {output}"))
 
     def _get_thermocouple_junction_temp(self):
-        """This method returns the temperature of the ceramic thermocouple block
-        used in the room temperature compensation calculation
+        """Returns the temperature of the ceramic thermocouple block from the room temperature compensation calculation.
 
-            Return:
+            Returns:
                 (float):
-                    * temperature of the ceramic thermocouple block (kelvin)
+                    Temperature of the ceramic thermocouple block (kelvin).
 
         """
         return float(self.query("TEMP?"))
 
     def set_temperature_limit(self, input_channel, limit):
-        """After a set temperature limit is exceeded, all control outputs will shut down
+        """After a set temperature limit is exceeded, all control outputs will shut down.
 
             Args:
                 input_channel (str or int):
-                    * Specifies which input to configure
-
+                    Specifies which input to configure.
                 limit (float):
-                    * The temperature limit in kelvin for which to shut down all control outputs when exceeded.
-                    * A limit of zero will turn the feature off
+                    The temperature limit in kelvin for which to shut down all control outputs when exceeded.
+                    A limit of zero will turn the feature off.
 
         """
         self.command(f"TLIMIT {input_channel},{limit}")
 
     def get_temperature_limit(self, input_channel):
-        """Returns the value of the temperature limit in kelvin
+        """Returns the value of the temperature limit in kelvin.
 
             Args:
                 input_channel (str or int):
-                    * Specifies which input to query
+                    Specifies which input to query.
 
         """
         return float(self.query(f"TLIMIT? {input_channel}"))
 
     def _get_tuning_control_status(self):
-        """If initial conditions are not met when starting the autotune procedure, causing the
-        autotuning process to never actually begin, then the error status will be set to 1 and
-        the stage status will be stage 00
+        """Returns dictionary of tuning control status values.
 
-            Return:
+            If initial conditions are not met when starting the autotune procedure, causing the
+            auto-tuning process to never actually begin, then the error status will be set to 1 and
+            the stage status will be stage 00.
+
+            Returns:
                 (dict):
-                    * Keys:
-                    * active_tuning_enable (bool):
-                        * False = no active tuning, True = active tuning
-
-                    * output (int):
-                        * Heater output of the control loop being tuned
-
-                    * tuning_error (bool):
-                        * False = no tuning error, True = tuning error
-
-                    * stage_status (int):
-                        * Specifies the current stage in the Autotune process.
-                        * If tuning error occurred, stage status represents stage that failed
+                    {"active_tuning_enable": bool, "output": int, "tuning_error": bool, "stage_status": int}
+                        active_tuning_enable: False = no active tuning, True = active tuning.
+                        output: Heater output of the control loop being tuned.
+                        tuning_error: False = no tuning error, True = tuning error.
+                        stage_status: Specifies the current stage in the Autotune process. If tuning error occurred,
+                        stage status represents stage that failed.
 
         """
         tuning_status = self.query("TUNEST?").split(",")
         return {"active_tuning_enable": bool(int(tuning_status[0])),
                 "output": int(tuning_status[1]),
                 "tuning_error": bool(int(tuning_status[2])),
                 "stage_status": int(tuning_status[3])}
 
     def _set_website_login(self, username, password):
         """Sets the username and password for the web interface.
 
             Args:
                 username (str):
-                    * 15 character string representing the website username
-
+                    15 character string representing the website username.
                 password (str):
-                    * 15 character string representing the website password
+                    15 character string representing the website password.
 
         """
         self.command(f"WEBLOG \"{username}\",\"{password}\"")
 
     def _get_website_login(self):
         """Method to return the username and password for the web interface.
 
-            Return:
-                website_login (dict):
-                    * A dictionary containing 15 character string type items
-                    * Keys:
-                    * "username": str
-                    * "password": str
+            Returns:
+                website_login (dict): A dictionary containing 15 character string type items.
+                    {"username": str, "password": str}
 
         """
         login_response = self.query("WEBLOG?").split(",")
         return {"username": login_response[0],
                 "password": login_response[1]}
 
     def _get_identity(self):
         return self.query('*IDN?', check_errors=False).split(',')
 
     def _autotune_error(self):
-        """Method to raise an excecption if autotune error has occured"""
+        """Method to raise an exception if autotune error has occurred."""
 
         tuning_status = self.query("TUNEST?").split(",")
 
         if bool(int(tuning_status[2])):
             raise InstrumentException("An autotune error is present")
```

### Comparing `lakeshore-1.6.1/lakeshore/teslameter.py` & `lakeshore-1.7.0/lakeshore/teslameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 DataPoint = namedtuple("DataPoint", ['elapsed_time', 'time_stamp',
                                      'magnitude', 'x', 'y', 'z',
                                      'field_control_set_point',
                                      'input_state'])
 
 
 class TeslameterOperationRegister(RegisterBase):
-    """Class object representing the operation status register"""
+    """Class object representing the operation status register."""
 
     bit_names = [
         "no_probe",
         "overload",
         "ranging",
         "",
         "",
@@ -39,15 +39,15 @@
         self.overload = overload
         self.ranging = ranging
         self.ramp_done = ramp_done
         self.no_data_on_breakout_adapter = no_data_on_breakout_adapter
 
 
 class TeslameterQuestionableRegister(RegisterBase):
-    """Class object representing the questionable status register"""
+    """Class object representing the questionable status register."""
 
     bit_names = [
         "x_axis_sensor_error",
         "y_axis_sensor_error",
         "z_axis_sensor_error",
         "probe_eeprom_read_error",
         "temperature_compensation_error",
@@ -78,49 +78,50 @@
         self.field_control_slew_rate_limit = field_control_slew_rate_limit
         self.field_control_at_voltage_limit = field_control_at_voltage_limit
         self.calibration_error = calibration_error
         self.heartbeat_error = heartbeat_error
 
 
 class Teslameter(XIPInstrument):
-    """A class object representing a Lake Shore F41 or F71 Teslameter"""
+    """A class object representing a Lake Shore F41 or F71 Teslameter."""
 
     vid_pid = [(0x1FB9, 0x0405), (0x1FB9, 0x0406)]
 
     def __init__(self,
                  serial_number=None,
                  com_port=None,
                  baud_rate=115200,
                  flow_control=True,
                  timeout=2.0,
                  ip_address=None,
                  tcp_port=7777,
                  **kwargs):
 
         # Call the parent init, then fill in values specific to the Teslameter
-        XIPInstrument.__init__(self, serial_number, com_port, baud_rate, flow_control, timeout, ip_address, tcp_port, **kwargs)
+        XIPInstrument.__init__(self, serial_number, com_port, baud_rate, flow_control, timeout, ip_address, tcp_port,
+                               **kwargs)
         self.status_byte_register = StatusByteRegister
         self.standard_event_register = StandardEventRegister
         self.operation_register = TeslameterOperationRegister
         self.questionable_register = TeslameterQuestionableRegister
 
     @requires_firmware_version('1.1.2018091003')
     def stream_buffered_data(self, length_of_time_in_seconds, sample_rate_in_ms):
         """Yield a generator object for the buffered field data.
-        Useful for getting the data in real time when doing a lengthy acquisition.
+
+            Useful for getting the data in real time when doing a lengthy acquisition.
 
             Args:
                 length_of_time_in_seconds (float):
                     The period of time over which to stream the data.
-
                 sample_rate_in_ms (int):
                     The averaging window (sampling period) of the instrument.
 
             Returns:
-               A generator object that returns the data as datapoint tuples
+               A generator object that returns the data as datapoint tuples.
         """
 
         # Set the sample rate
         self.command("SENSE:AVERAGE:COUNT " + str(sample_rate_in_ms / 10))
 
         # Round the length of time to the nearest 10 milliseconds.
         length_of_time_in_seconds = round(length_of_time_in_seconds, 2)
@@ -170,39 +171,36 @@
                     # Unpack the parsed point into a namedtuple and append it to the list
                     new_point = DataPoint(elapsed_time_in_seconds, *point_data)
 
                     yield new_point
 
     @requires_firmware_version('1.1.2018091003')
     def get_buffered_data_points(self, length_of_time_in_seconds, sample_rate_in_ms):
-        """Returns a list of namedtuples that contain the buffered data.
+        """Returns a list of named tuples that contain the buffered data.
 
             Args:
                 length_of_time_in_seconds (float):
                     The period of time over which to collect the data.
-
                 sample_rate_in_ms (int):
                     The averaging window (sampling period) of the instrument.
 
             Returns:
-               The data as a list of datapoint tuples
+               The data as a list of datapoint tuples.
         """
         return list(self.stream_buffered_data(length_of_time_in_seconds, sample_rate_in_ms))
 
     @requires_firmware_version('1.1.2018091003')
     def log_buffered_data_to_file(self, length_of_time_in_seconds, sample_rate_in_ms, file):
         """Creates or appends a CSV file with the buffered data and excel-friendly timestamps.
 
             Args:
                 length_of_time_in_seconds (float):
                     The period of time over which to collect the data.
-
                 sample_rate_in_ms (int):
                     The averaging window (sampling period) of the instrument.
-
                 file (file_object):
                     Field measurement data will be written to this file object in a CSV format.
         """
         # Open the file and write in header information.
         file.write('time elapsed,date,time,' +
                    'magnitude,x,y,z,field control set point,input state\n')
 
@@ -308,26 +306,23 @@
         self.command(f"SENS:RELATIVE:BASELINE {str(baseline_field)}")
 
     def configure_field_measurement_setup(self, mode="DC", autorange=True, expected_field=None, averaging_samples=20):
         """Configures the field measurement settings.
 
             Args:
                 mode (str):
-                    * Modes are as follows:
-                    * "DC"
-                    * "AC" (0.1 - 500 Hz)
-                    * "HIFR" (50 Hz - 100 kHz)
-
+                    Modes are as follows:
+                    "DC",
+                    "AC" (0.1 - 500 Hz), and
+                    "HIFR" (50 Hz - 100 kHz).
                 autorange (bool):
-                    Chooses whether the instrument automatically selects the best range for the measured value
-
+                    Chooses whether the instrument automatically selects the best range for the measured value.
                 expected_field (float):
                     When autorange is False, the expected_field is the largest field expected to be measured.
                     It sets the lowest instrument field range capable of measuring the value.
-
                 averaging_samples (int):
                     The number of field samples to average. Each sample is 10 milliseconds of field information.
 
         """
         self.command(f"SENS:MODE {mode}")
         self.command(f"SENS:RANGE:AUTO {str(int(autorange))}")
         if expected_field is not None:
@@ -344,19 +339,18 @@
         return measurement_setup
 
     def configure_temperature_compensation(self, temperature_source="PROBE", manual_temperature=None):
         """Configures how temperature compensation is applied to the field readings.
 
             Args:
                 temperature_source (str):
-                    * Determines where the temperature measurement is drawn from. Options are:
-                    * "PROBE" (Compensation is based on measurement of a thermistor in the probe)
-                    * "MTEM" (Compensation is based on a manual temperature value provided by the user)
-                    * "NONE" (Temperature compensation is not applied)
-
+                    Determines where the temperature measurement is drawn from. Options are:
+                    "PROBE" (Compensation is based on measurement of a thermistor in the probe),
+                    "MTEM" (Compensation is based on a manual temperature value provided by the user),
+                    "NONE" (Temperature compensation is not applied).
                 manual_temperature (float):
                     Sets the temperature provided by the user for MTEMP (manual temperature) source in Celsius.
 
         """
         self.command(f"SENS:TCOM:TSOURCE {temperature_source}")
         if manual_temperature is not None:
             self.command(f"SENS:TCOM:MTEM {str(manual_temperature)}")
@@ -370,17 +364,17 @@
         return float(self.query("SENS:TCOM:MTEM?"))
 
     def configure_field_units(self, units="TESLA"):
         """Configures the field measurement units of the instrument.
 
             Args:
                 units (str):
-                    * A unit of magnetic field. Options are:
-                    * "TESLA"
-                    * "GAUSS"
+                    A unit of magnetic field. Options are:
+                    "TESLA", or
+                    "GAUSS".
 
         """
         self.command(f"UNIT:FIELD {units}")
 
     def get_field_units(self):
         """Returns the magnetic field units of the instrument."""
         return self.query("UNIT:FIELD?")
@@ -388,15 +382,14 @@
     @requires_firmware_version("1.1.2018091003")
     def configure_field_control_limits(self, voltage_limit=10.0, slew_rate_limit=10.0):
         """Configures the limits of the field control output.
 
             Args:
                 voltage_limit (float):
                     The maximum voltage permitted at the field control output. Must be between 0 and 10V.
-
                 slew_rate_limit (float):
                     The maximum rate of change of the field control output voltage in volts per second.
 
         """
         self.command(f"SOURCE:FIELD:VLIMIT {str(voltage_limit)}")
         self.command(f"SOURCE:FIELD:SLEW {str(slew_rate_limit)}")
 
@@ -410,18 +403,17 @@
 
     @requires_firmware_version("1.1.2018091003")
     def configure_field_control_output_mode(self, mode="CLLOOP", output_enabled=True):
         """Configure the field control mode and state.
 
             Args:
                 mode (str):
-                    * Determines whether the field control is in open or closed loop mode
-                    * "CLLOOP" (closed loop control)
-                    * "OPLOOP" (open loop control, voltage output)
-
+                    Determines whether the field control is in open or closed loop mode. Options:
+                    "CLLOOP" (closed loop control), or
+                    "OPLOOP" (open loop control, voltage output).
                 output_enabled (bool):
                     Turn the field control voltage output on or off.
 
         """
 
         self.command(f"SOURCE:FIELD:MODE {mode}")
         self.command(f"SOURCE:FIELD:STATE {str(int(output_enabled))}")
@@ -439,21 +431,19 @@
         """Configures the closed loop control parameters of the field control output.
 
             Args:
                 gain (float):
                     Also known as P or Proportional in PID control.
                     This controls how strongly the control output reacts to the present error.
                     Note that the integral value is multiplied by the gain value.
-
                 integral (float):
                     Also known as I or Integral in PID control.
-                    This controls how strongly the control output reacts to the past error *history*
-
+                    This controls how strongly the control output reacts to the past error *history*.
                 ramp_rate (float):
-                    This value controls how quickly the present field setpoint will transition to a new setpoint.
+                    This value controls how quickly the present field set-point will transition to a new set-point.
                     The ramp rate is configured in field units per second.
 
         """
         if gain is not None:
             self.command(f"SOURCE:FIELD:CLL:GAIN {str(gain)}")
         if integral is not None:
             self.command(f"SOURCE:FIELD:CLL:INTEGRAL {str(integral)}")
@@ -487,189 +477,190 @@
     @requires_firmware_version("1.1.2018091003")
     def get_field_control_open_loop_voltage(self):
         """Returns the field control open loop voltage."""
         return float(self.query("SOURCE:FIELD:OPL:VOLTAGE?"))
 
     @requires_firmware_version("1.4.2019061411")
     def set_analog_output(self, analog_output_mode):
-        """Configures what signal is provided by the analog output BNC"""
+        """Configures what signal is provided by the analog output BNC."""
         warnings.warn(
             "set_analog_output will be depreciated in a future version, use set_analog_output_signal instead",
             PendingDeprecationWarning
         )
         self.command(f"SOURCE:AOUT {analog_output_mode}")
 
     @requires_firmware_version("1.6.2019092002")
     def set_analog_output_signal(self, analog_output_mode):
-        """Configures what signal is provided by the analog output BNC
+        """Configures what signal is provided by the analog output BNC.
 
             Args:
                 analog_output_mode (str):
-                    * Configures what signal is provided by the analog output BNC. Options are:
-                    * "OFF"  (output off)
-                    * "XRAW" (raw amplified X channel Hall voltage)
-                    * "YRAW" (raw amplified Y channel Hall voltage)
-                    * "ZRAW" (raw amplified Z channel Hall voltage)
-                    * "XCOR" (Corrrected X channel field measurement)
-                    * "YCOR" (Corrected Y channel field measurement)
-                    * "ZCOR" (Corrected Z channel field measurement)
-                    * "MCOR" (Corrected magnitude field measurement)
+                    Configures what signal is provided by the analog output BNC. Options:
+                    "OFF" (output off),
+                    "XRAW" (raw amplified X channel Hall voltage),
+                    "YRAW" (raw amplified Y channel Hall voltage),
+                    "ZRAW" (raw amplified Z channel Hall voltage),
+                    "XCOR" (Corrrected X channel field measurement),
+                    "YCOR" (Corrected Y channel field measurement),
+                    "ZCOR" (Corrected Z channel field measurement), or
+                    "MCOR" (Corrected magnitude field measurement)
 
         """
         self.command(f"SOURCE:AOUT {analog_output_mode}")
 
     @requires_firmware_version("1.6.2019092002")
     def configure_corrected_analog_output_scaling(self, scale_factor, baseline):
         """Configures the conversion between field reading and analog output voltage.
 
             Args:
                 scale_factor (float):
                     Scale factor in volts per unit field.
-
                 baseline (float):
                     The field value at which the analog output voltage is zero.
 
         """
         self.command(f"SOURCE:AOUT:SFACTOR {str(scale_factor)}", f"SOURCE:AOUT:BASELINE {str(baseline)}")
 
     @requires_firmware_version("1.6.2019092002")
     def get_corrected_analog_output_scaling(self):
         """Returns the scale factor and baseline of the corrected analog out."""
         return float(self.query("SOURCE:AOUT:SFACTOR?")), float(self.query("SOURCE:AOUT:BASELINE?"))
 
     def get_analog_output(self):
-        """Returns what signal is being provided by the analog output"""
+        """Returns what signal is being provided by the analog output."""
         warnings.warn(
             "get_analog_output will be depreciated in a future version, use get_analog_output_signal instead",
             PendingDeprecationWarning
         )
         return self.query("SOURCE:AOUT?")
 
     def get_analog_output_signal(self):
-        """Returns what signal is being provided by the analog output"""
+        """Returns what signal is being provided by the analog output."""
         return self.query("SOURCE:AOUT?")
 
     @requires_firmware_version("1.6.2019092002")
     def enable_high_frequency_filters(self):
-        """Applies filtering to the high frequency RMS measurements"""
+        """Applies filtering to the high frequency RMS measurements."""
         self.command("SENSE:FILT 1")
 
     @requires_firmware_version("1.6.2019092002")
     def disable_high_frequency_filters(self):
-        """Turns off filtering of the high frequency mode measurements"""
+        """Turns off filtering of the high frequency mode measurements."""
         self.command("SENSE:FILT 0")
 
     @requires_firmware_version("1.6.2019092002")
     def set_frequency_filter_type(self, filter_type):
-        """Configures which filter is applied to the high frequency measurements
+        """Configures which filter is applied to the high frequency measurements.
 
             Args:
                 filter_type (str):
-                    * "LPASS"  (low pass filter)
-                    * "HPASS" (high pass filter)
-                    * "BPASS" (band pass filter)
+                    Options: "LPASS" (low pass filter), "HPASS" (high pass filter), or "BPASS" (band pass filter).
         """
         self.command(f"SENSE:FILT:TYPE {str(filter_type)}")
 
     @requires_firmware_version("1.6.2019092002")
     def get_frequency_filter_type(self):
-        """Returns the type of filter that is or will be applied to the high frequency measurements"""
+        """Returns the type of filter that is or will be applied to the high frequency measurements."""
         return self.query("SENSE:FILTER:TYPE?")
 
     @requires_firmware_version("1.6.2019092002")
     def get_low_pass_filter_cutoff(self):
-        """Returns the cutoff frequency setting of the low pass filter"""
+        """Returns the cutoff frequency setting of the low pass filter."""
         return float(self.query("SENSE:FILTER:LPASS:CUTOFF?"))
 
     @requires_firmware_version("1.6.2019092002")
     def set_low_pass_filter_cutoff(self, cutoff_frequency):
-        """Configures the low pass filter cutoff
+        """Configures the low pass filter cutoff.
 
             Args:
-                cutoff_frequency (float)
+                cutoff_frequency (float):
+                    Options: NONE, F10, F30, F100, F300, F1000, F3000, or F10000
+                    F10 = 10 Hz, etc.
         """
         self.command(f"SENSE:FILTER:LPASS:CUTOFF {str(cutoff_frequency)}")
 
     @requires_firmware_version("1.6.2019092002")
     def get_high_pass_filter_cutoff(self):
-        """Returns the cutoff frequency setting of the low pass filter"""
+        """Returns the cutoff frequency setting of the low pass filter."""
         return float(self.query("SENSE:FILTER:HPASS:CUTOFF?"))
 
     @requires_firmware_version("1.6.2019092002")
     def set_high_pass_filter_cutoff(self, cutoff_frequency):
-        """Configures the high pass filter cutoff
+        """Configures the high pass filter cutoff.
 
             Args:
-                cutoff_frequency (float)
+                cutoff_frequency (float):
+                    Options: NONE, F10, F30, F100, F300, F1000, F3000, or F10000
+                    F10 = 10 Hz, etc.
         """
         self.command(f"SENSE:FILTER:HPASS:CUTOFF {str(cutoff_frequency)}")
 
     @requires_firmware_version("1.6.2019092002")
     def get_band_pass_filter_center(self):
-        """Returns the center of the band pass filter"""
+        """Returns the center of the band pass filter."""
         return float(self.query("SENSE:FILTER:BPASS:CENTER?"))
 
     @requires_firmware_version("1.6")
     def set_band_pass_filter_center(self, center_frequency):
-        """Configures the band pass filter parameters
+        """Configures the band pass filter parameters.
 
             Args:
                 center_frequency (float):
-                    The frequency at which the gain of the filter is 1
+                    The frequency at which the gain of the filter is 1.
         """
         self.command(f"SENSE:FILTER:BPASS:CENTER {str(center_frequency)}")
 
     @requires_firmware_version("1.6.2019092002")
     def enable_qualifier(self):
-        """Enables the qualifier"""
+        """Enables the qualifier."""
         self.command("SENSE:QUALIFIER 1")
 
     @requires_firmware_version("1.6.2019092002")
     def disable_qualifier(self):
-        """Disables the qualifier"""
+        """Disables the qualifier."""
         self.command("SENSE:QUALIFIER 0")
 
     @requires_firmware_version("1.6.2019092002")
     def is_qualifier_condition_met(self):
-        """Returns whether the qualifier condition is met"""
+        """Returns whether the qualifier condition is met."""
         return bool(int(self.query("SENSE:QUALIFIER:CONDITION?")))
 
     @requires_firmware_version("1.6.2019092002")
     def enable_qualifier_latching(self):
-        """Enables the qualifier condition latching"""
+        """Enables the qualifier condition latching."""
         self.command("SENSE:QUALIFIER:LATCH 1")
 
     @requires_firmware_version("1.6.2019092002")
     def disable_qualifier_latching(self):
-        """Disables the qualifier condition latching"""
+        """Disables the qualifier condition latching."""
         self.command("SENSE:QUALIFIER:LATCH 0")
 
     @requires_firmware_version("1.6.2019092002")
     def get_qualifier_latching_setting(self):
-        """Returns whether the qualifier latches"""
+        """Returns whether the qualifier latches."""
         return self.query("SENSE:QUALIFIER:LATCH?")
 
     @requires_firmware_version("1.6.2019092002")
     def set_qualifier_latching_setting(self, latching):
-        """Sets whether the qualifier latches
+        """Sets whether the qualifier latches.
 
             Args:
                 latching (bool):
-                    Determines whether the qualifier latches
+                    Determines whether the qualifier latches.
         """
         self.command(f"SENSE:QUALIFIER:LATCH {str(latching)}")
 
     @requires_firmware_version("1.6.2019092002")
     def reset_qualifier_latch(self):
-        """Resets the condition status of the qualifier"""
+        """Resets the condition status of the qualifier."""
         self.command("SENSE:QUALIFIER:LRESET")
 
     @requires_firmware_version("1.6.2019092002")
     def get_qualifier_configuration(self):
-        """Returns the threshold mode and field threshold values"""
+        """Returns the threshold mode and field threshold values."""
         response = self.query("SENSE:QUALIFIER:THRESHOLD?")
         elements = response.split(',')
         mode = elements[0]
         threshold_field_low = float(elements[1])
         threshold = (mode, threshold_field_low)
         if len(elements) == 3:
             threshold_field_upper = float(elements[2])
@@ -678,27 +669,20 @@
 
     @requires_firmware_version("1.6.2019092002")
     def configure_qualifier(self, mode, lower_field, upper_field=None):
         """Sets the threshold condition of the qualifier.
 
             Args:
                 mode (str):
-                    The type of threshold condition used by the qualifer
-                    * "OVER"
-                    * "UNDER"
-                    * "BETWEEN"
-                    * "OUTSIDE"
-                    * "ABSBETWEEN"
-                    * "ABSOUTSIDE"
-
+                    The type of threshold condition used by the qualifier.
+                    Options: "OVER", "UNDER", "BETWEEN", "OUTSIDE", "ABSBETWEEN", or "ABSOUTSIDE".
                 lower_field (float):
-                    The lower field value threshold used by the qualifier
-
+                    The lower field value threshold used by the qualifier.
                 upper_field (float):
-                    The upper field value threshold used by the qualifier. Not used for OVER or UNDER
+                    The upper field value threshold used by the qualifier. Not used for OVER or UNDER.
         """
         if upper_field is None:
             self.command(f"SENSE:QUALIFIER:THRESHOLD {mode},{str(lower_field)}")
         else:
             self.command(f"SENSE:QUALIFIER:THRESHOLD {mode},{str(lower_field)},{str(upper_field)}")
```

### Comparing `lakeshore-1.6.1/lakeshore/xip_instrument.py` & `lakeshore-1.7.0/lakeshore/xip_instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import serial
 
 from .generic_instrument import GenericInstrument, InstrumentException, RegisterBase
 
 
 class StatusByteRegister(RegisterBase):
-    """Class object representing the status byte register"""
+    """Class object representing the status byte register."""
 
     bit_names = [
         "",
         "",
         "error_available",
         "questionable_summary",
         "message_available_summary",
@@ -33,15 +33,15 @@
         self.message_available_summary = message_available_summary
         self.event_status_summary = event_status_summary
         self.master_summary = master_summary
         self.operation_summary = operation_summary
 
 
 class StandardEventRegister(RegisterBase):
-    """Class object representing the standard event register"""
+    """Class object representing the standard event register."""
 
     bit_names = [
         "operation_complete",
         "query_error",
         "device_specific_error",
         "execution_error",
         "command_error",
@@ -65,15 +65,15 @@
 
 
 class XIPInstrumentException(Exception):
     """Names a new type of exception specific to XIP instrument connectivity."""
 
 
 class XIPInstrument(GenericInstrument):
-    """Parent class that implements functionality shared by all XIP instruments"""
+    """Parent class that implements functionality shared by all XIP instruments."""
 
     def __init__(self,
                  serial_number,
                  com_port,
                  baud_rate,
                  flow_control,
                  timeout,
@@ -88,23 +88,22 @@
         self.standard_event_register = StandardEventRegister
         self.operation_register = None
         self.questionable_register = None
         if clear_errors_on_init:
             self.command('SYSTem:ERRor:CLEar', check_errors=False)
 
     def command(self, *commands, check_errors=True):
-        """Send a SCPI command or multiple commands to the instrument
+        """Send an SCPI command or multiple commands to the instrument.
 
             Args:
                 commands (str):
                     Any number of SCPI commands.
-
-            Kwargs:
                 check_errors (bool):
                     Chooses whether to query the SCPI error queue and raise errors as exceptions. True by default.
+                    Optional Parameter.
 
         """
 
         # Group all commands into a single string with SCPI delimiters.
         command_string = ";:".join(commands)
 
         # Pass the string to the query function if it contains a question mark.
@@ -114,29 +113,30 @@
         else:
             with self.dut_lock:
                 # Send command to the instrument over serial. If serial is not configured, send it over TCP.
                 if self.device_serial is not None:
                     self._usb_command(command_string)
                 elif self.device_tcp is not None:
                     self._tcp_command(command_string)
+                elif self.user_connection is not None:
+                    self._user_connection_command(command_string)
                 else:
                     raise InstrumentException("No connections configured")
 
                 self.logger.info('Sent SCPI command to %s: %s', self.serial_number, command_string)
 
     def query(self, *queries, check_errors=True):
-        """Send a SCPI query or multiple queries to the instrument and return the response(s)
+        """Sends an SCPI query or multiple queries to the instrument and return the response(s).
 
             Args:
                 queries (str):
                     Any number of SCPI queries or commands.
-
-            Kwargs:
                 check_errors (bool):
                     Chooses whether to query the SCPI error queue and raise errors as exceptions. True by default.
+                    Optional Parameter.
 
             Returns:
                The instrument query response as a string.
 
         """
 
         # Group all commands and queries a single string with SCPI delimiters.
@@ -148,14 +148,16 @@
 
         # Query the instrument over serial. If serial is not configured, use TCP.
         with self.dut_lock:
             if self.device_serial is not None:
                 response = self._usb_query(query_string)
             elif self.device_tcp is not None:
                 response = self._tcp_query(query_string)
+            elif self.user_connection is not None:
+                response = self._user_connection_query(query_string)
             else:
                 raise InstrumentException("No connections configured")
 
             self.logger.info('Sent SCPI query to %s: %s', self.serial_number, query_string)
             self.logger.info('Received SCPI response from %s: %s', self.serial_number, response)
 
         if check_errors:
@@ -166,219 +168,231 @@
             self._error_check(error_response)
             response = ';'.join(response_list)
 
         return response
 
     @staticmethod
     def _error_check(error_response):
-        """Evaluates the instrument response"""
+        """Evaluates the instrument response."""
 
         # If the error buffer returns an error, raise an exception with that includes the error.
         if "No error" not in error_response:
             raise XIPInstrumentException("SCPI command error(s): " + error_response)
 
     def get_status_byte(self):
-        """Returns named bits of the status byte register and their values"""
+        """Returns named bits of the status byte register and their values."""
 
         response = self.query("*STB?", check_errors=False)
         status_register = self.status_byte_register.from_integer(response)
 
         return status_register
 
     def get_service_request_enable_mask(self):
         """Returns the named bits of the status byte service request enable register.
-        This register determines which bits propagate to the master summary status bit"""
+
+            This register determines which bits propagate to the master summary status bit.
+        """
 
         response = self.query("*SRE?", check_errors=False)
         status_register = self.status_byte_register.from_integer(response)
 
         return status_register
 
     def set_service_request_enable_mask(self, register_mask):
         """Configures values of the service request enable register bits.
-        This register determines which bits propagate to the master summary bit
+
+            This register determines which bits propagate to the master summary bit.
 
             Args:
                 register_mask (StatusByteRegister):
                     A StatusByteRegister class object with all bits configured true or false.
         """
 
         integer_representation = register_mask.to_integer()
         self.command(f"*SRE {str(integer_representation)}", check_errors=False)
 
     def get_standard_events(self):
-        """Returns the names of the standard event register bits and their values"""
+        """Returns the names of the standard event register bits and their values."""
 
         response = self.query("*ESR?", check_errors=False)
         status_register = self.standard_event_register.from_integer(response)
 
         return status_register
 
     def get_standard_event_enable_mask(self):
         """Returns the names of the standard event enable register bits and their values.
-        These values determine which bits propagate to the standard event register"""
+
+            These values determine which bits propagate to the standard event register.
+        """
 
         response = self.query("*ESE?", check_errors=False)
         status_register = self.standard_event_register.from_integer(response)
 
         return status_register
 
     def set_standard_event_enable_mask(self, register_mask):
         """Configures values of the standard event enable register bits.
-        These values determine which bits propagate to the standard event register
+
+            These values determine which bits propagate to the standard event register.
 
             Args:
                 register_mask (StandardEventRegister):
                     A StandardEventRegister class object with all bits configured true or false.
         """
 
         integer_representation = register_mask.to_integer()
         self.command(f"*ESE {str(integer_representation)}", check_errors=False)
 
     def get_present_operation_status(self):
-        """Returns the names of the operation status register bits and their values"""
+        """Returns the names of the operation status register bits and their values."""
 
         response = self.query("STATus:OPERation:CONDition?", check_errors=False)
         status_register = self.operation_register.from_integer(response)
 
         return status_register
 
     def get_operation_events(self):
         """Returns the names of operation event status register bits that are currently high.
-        The event register is latching and values are reset when queried."""
+
+            The event register is latching and values are reset when queried.
+        """
 
         response = self.query("STATus:OPERation:EVENt?", check_errors=False)
         status_register = self.operation_register.from_integer(response)
 
         return status_register
 
     def get_operation_event_enable_mask(self):
         """Returns the names of the operation event enable register bits and their values.
-        These values determine which operation bits propagate to the operation event register."""
+
+            These values determine which operation bits propagate to the operation event register.
+        """
 
         response = self.query("STATus:OPERation:ENABle?", check_errors=False)
         status_register = self.operation_register.from_integer(response)
 
         return status_register
 
     def set_operation_event_enable_mask(self, register_mask):
         """Configures the values of the operation event enable register bits.
-        These values determine which operation bits propagate to the operation event register.
+
+            These values determine which operation bits propagate to the operation event register.
 
             Args:
                 register_mask ([Instrument]OperationRegister):
                     An instrument specific OperationRegister class object with all bits configured true or false.
         """
 
         integer_representation = register_mask.to_integer()
         self.command(f"STATus:OPERation:ENABle {str(integer_representation)}", check_errors=False)
 
     def get_present_questionable_status(self):
-        """Returns the names of the questionable status register bits and their values"""
+        """Returns the names of the questionable status register bits and their values."""
 
         response = self.query("STATus:QUEStionable:CONDition?", check_errors=False)
         status_register = self.questionable_register.from_integer(response)
 
         return status_register
 
     def get_questionable_events(self):
         """Returns the names of questionable event status register bits that are currently high.
-        The event register is latching and values are reset when queried."""
+
+            The event register is latching and values are reset when queried.
+        """
 
         response = self.query("STATus:QUEStionable:EVENt?", check_errors=False)
         status_register = self.questionable_register.from_integer(response)
 
         return status_register
 
     def get_questionable_event_enable_mask(self):
         """Returns the names of the questionable event enable register bits and their values.
-        These values determine which questionable bits propagate to the questionable event register."""
+
+            These values determine which questionable bits propagate to the questionable event register.
+        """
 
         response = self.query("STATus:QUEStionable:ENABle?", check_errors=False)
         status_register = self.questionable_register.from_integer(response)
 
         return status_register
 
     def set_questionable_event_enable_mask(self, register_mask):
         """Configures the values of the questionable event enable register bits.
-        These values determine which questionable bits propagate to the questionable event register.
+
+            These values determine which questionable bits propagate to the questionable event register.
 
             Args:
                 register_mask ([Instrument]QuestionableRegister):
                     An instrument specific QuestionableRegister class object with all bits configured true or false.
         """
 
         integer_representation = self.questionable_register.to_integer(register_mask)
         self.command(f"STATus:QUEStionable:ENABle {str(integer_representation)}", check_errors=False)
 
     def reset_status_register_masks(self):
-        """Resets status register masks to preset values"""
+        """Resets status register masks to preset values."""
         self.command("STATus:PRESet", check_errors=False)
 
     def modify_service_request_mask(self, bit_name, value):
         """Gets the service request enable mask, changes a bit, and sets the register.
 
             Args:
                 bit_name (str):
                     The name of the bit to modify.
-
                 value (bool):
                     Determines whether the bit masks (false) or passes (true) the corresponding state.
 
         """
 
         mask_register = self.get_service_request_enable_mask()
 
         setattr(mask_register, bit_name, value)
 
         self.set_service_request_enable_mask(mask_register)
 
     def modify_standard_event_register_mask(self, bit_name, value):
-        """Gets the standard event register mask, changes a bit, and sets the register
+        """Gets the standard event register mask, changes a bit, and sets the register.
 
             Args:
                 bit_name (str):
                     The name of the bit to modify.
-
                 value (bool):
                     Determines whether the bit masks (false) or passes (true) the corresponding state.
 
         """
 
         mask_register = self.get_standard_event_enable_mask()
 
         setattr(mask_register, bit_name, value)
 
         self.set_standard_event_enable_mask(mask_register)
 
     def modify_operation_register_mask(self, bit_name, value):
-        """Gets the operation condition register mask, changes a bit, and sets the register
+        """Gets the operation condition register mask, changes a bit, and sets the register.
 
             Args:
                 bit_name (str):
                     The name of the bit to modify.
-
                 value (bool):
                     Determines whether the bit masks (false) or passes (true) the corresponding state.
 
         """
 
         mask_register = self.get_operation_event_enable_mask()
 
         setattr(mask_register, bit_name, value)
 
         self.set_operation_event_enable_mask(mask_register)
 
     def modify_questionable_register_mask(self, bit_name, value):
-        """Gets the questionable condition register mask, changes a bit, and sets the register
+        """Gets the questionable condition register mask, changes a bit, and sets the register.
 
             Args:
                 bit_name (str):
                     The name of the bit to modify.
-
                 value (bool):
                     Determines whether the bit masks (false) or passes (true) the corresponding state.
 
         """
 
         mask_register = self.get_questionable_event_enable_mask()
```

### Comparing `lakeshore-1.6.1/lakeshore.egg-info/PKG-INFO` & `lakeshore-1.7.0/lakeshore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeshore
-Version: 1.6.1
+Version: 1.7.0
 Summary: A package to connect to and interact with Lake Shore instruments.
 Home-page: https://github.com/lakeshorecryotronics/python-driver
 Maintainer: Lake Shore Cryotronics, Inc.
 Maintainer-email: service@lakeshore.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lakeshore-1.6.1/lakeshore.egg-info/SOURCES.txt` & `lakeshore-1.7.0/lakeshore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.1/setup.py` & `lakeshore-1.7.0/setup.py`

 * *Files identical despite different names*

