# Comparing `tmp/simply_nwb-0.1.0.tar.gz` & `tmp/simply_nwb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.1.0.tar", last modified: Wed May 31 21:16:56 2023, max compression
+gzip compressed data, was "simply_nwb-0.1.1.tar", last modified: Thu Jun  1 17:11:14 2023, max compression
```

## Comparing `simply_nwb-0.1.0.tar` & `simply_nwb-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.477912 simply_nwb-0.1.0/
--rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      566 2023-05-31 21:16:56.477912 simply_nwb-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-31 21:16:56.477912 simply_nwb-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-05-31 18:00:34.000000 simply_nwb-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.463890 simply_nwb-0.1.0/simply_nwb/
--rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/simply_nwb/__init__.py
--rw-rw-rw-   0        0        0    27237 2023-05-31 18:00:34.000000 simply_nwb-0.1.0/simply_nwb/simple_nwb.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.469890 simply_nwb-0.1.0/simply_nwb/transferring/
--rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.1.0/simply_nwb/transferring/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.470889 simply_nwb-0.1.0/simply_nwb/transferring/filesync/
--rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.1.0/simply_nwb/transferring/filesync/__init__.py
--rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.1.0/simply_nwb/transferring/filesync/oneway.py
--rw-rw-rw-   0        0        0     7339 2023-05-31 20:19:57.000000 simply_nwb-0.1.0/simply_nwb/transferring/nwb_transfer.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.476912 simply_nwb-0.1.0/simply_nwb/transforms/
--rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.1.0/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/simply_nwb/transforms/blackrock.py
--rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.1.0/simply_nwb/transforms/csv.py
--rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.1.0/simply_nwb/transforms/labjack.py
--rw-rw-rw-   0        0        0     1789 2023-05-31 15:31:44.000000 simply_nwb-0.1.0/simply_nwb/transforms/mp4.py
--rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/simply_nwb/transforms/p_erg.py
--rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/simply_nwb/transforms/plaintext.py
--rw-rw-rw-   0        0        0     3874 2023-05-24 18:25:41.000000 simply_nwb-0.1.0/simply_nwb/transforms/tif.py
--rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.1.0/simply_nwb/transforms/yaml.py
--rw-rw-rw-   0        0        0     7593 2023-05-31 16:44:20.000000 simply_nwb-0.1.0/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.467902 simply_nwb-0.1.0/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 17:11:14.258646 simply_nwb-0.1.1/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-06-01 17:11:14.258646 simply_nwb-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.1.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-01 17:11:14.258646 simply_nwb-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-06-01 17:11:08.000000 simply_nwb-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:11:14.244490 simply_nwb-0.1.1/simply_nwb/
+-rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.1.1/simply_nwb/__init__.py
+-rw-rw-rw-   0        0        0    27269 2023-06-01 17:11:08.000000 simply_nwb-0.1.1/simply_nwb/simple_nwb.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:11:14.249491 simply_nwb-0.1.1/simply_nwb/transferring/
+-rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.1.1/simply_nwb/transferring/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:11:14.250630 simply_nwb-0.1.1/simply_nwb/transferring/filesync/
+-rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.1.1/simply_nwb/transferring/filesync/__init__.py
+-rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.1.1/simply_nwb/transferring/filesync/oneway.py
+-rw-rw-rw-   0        0        0     7339 2023-05-31 20:19:57.000000 simply_nwb-0.1.1/simply_nwb/transferring/nwb_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:11:14.257631 simply_nwb-0.1.1/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.1.1/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.1.1/simply_nwb/transforms/blackrock.py
+-rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.1.1/simply_nwb/transforms/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.1.1/simply_nwb/transforms/labjack.py
+-rw-rw-rw-   0        0        0     1789 2023-05-31 15:31:44.000000 simply_nwb-0.1.1/simply_nwb/transforms/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.1.1/simply_nwb/transforms/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.1.1/simply_nwb/transforms/plaintext.py
+-rw-rw-rw-   0        0        0     3874 2023-05-24 18:25:41.000000 simply_nwb-0.1.1/simply_nwb/transforms/tif.py
+-rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.1.1/simply_nwb/transforms/yaml.py
+-rw-rw-rw-   0        0        0     7593 2023-05-31 16:44:20.000000 simply_nwb-0.1.1/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:11:14.248490 simply_nwb-0.1.1/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-06-01 17:11:14.000000 simply_nwb-0.1.1/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-06-01 17:11:14.000000 simply_nwb-0.1.1/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 17:11:14.000000 simply_nwb-0.1.1/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-06-01 17:11:14.000000 simply_nwb-0.1.1/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-01 17:11:14.000000 simply_nwb-0.1.1/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.1.0/LICENSE` & `simply_nwb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/PKG-INFO` & `simply_nwb-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply_nwb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.1.0/setup.py` & `simply_nwb-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.1.0/simply_nwb/simple_nwb.py` & `simply_nwb-0.1.1/simply_nwb/simple_nwb.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from pynwb import NWBFile, TimeSeries
 from pynwb.behavior import BehavioralEvents
 from pynwb.device import Device
 from pynwb.ecephys import ElectrodeGroup
 from pynwb.file import Subject
 from pynwb.ophys import OpticalChannel, TwoPhotonSeries
 
-from transforms import labjack_load_file
-from transforms import blackrock_all_spiketrains, perg_parse_to_table
-from .util import warn_on_name_format, inspect_nwb_obj, nwb_write, panda_df_to_dyn_table, \
+from simply_nwb.transforms import labjack_load_file
+from simply_nwb.transforms import blackrock_all_spiketrains, perg_parse_to_table
+from simply_nwb.util import warn_on_name_format, inspect_nwb_obj, nwb_write, panda_df_to_dyn_table, \
     panda_df_to_list_of_timeseries, dict_to_dyn_tables
 
 
 class SimpleNWB(object):
     _REQUIRED_ARGS = [
         "session_description",
         "session_start_time",
```

### Comparing `simply_nwb-0.1.0/simply_nwb/transferring/__init__.py` & `simply_nwb-0.1.1/simply_nwb/transferring/__init__.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transferring/filesync/oneway.py` & `simply_nwb-0.1.1/simply_nwb/transferring/filesync/oneway.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transferring/nwb_transfer.py` & `simply_nwb-0.1.1/simply_nwb/transferring/nwb_transfer.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transforms/blackrock.py` & `simply_nwb-0.1.1/simply_nwb/transforms/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transforms/csv.py` & `simply_nwb-0.1.1/simply_nwb/transforms/csv.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transforms/labjack.py` & `simply_nwb-0.1.1/simply_nwb/transforms/labjack.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transforms/mp4.py` & `simply_nwb-0.1.1/simply_nwb/transforms/mp4.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transforms/p_erg.py` & `simply_nwb-0.1.1/simply_nwb/transforms/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transforms/plaintext.py` & `simply_nwb-0.1.1/simply_nwb/transforms/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/transforms/tif.py` & `simply_nwb-0.1.1/simply_nwb/transforms/tif.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb/util.py` & `simply_nwb-0.1.1/simply_nwb/util.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.1.0/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.1.1/simply_nwb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-nwb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.1.0/simply_nwb.egg-info/SOURCES.txt` & `simply_nwb-0.1.1/simply_nwb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

