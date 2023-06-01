# Comparing `tmp/jianglab-0.2.7.tar.gz` & `tmp/jianglab-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.2.7.tar", last modified: Thu Jun  1 16:04:09 2023, max compression
+gzip compressed data, was "jianglab-0.2.8.tar", last modified: Thu Jun  1 17:42:31 2023, max compression
```

## Comparing `jianglab-0.2.7.tar` & `jianglab-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 16:04:09.890548 jianglab-0.2.7/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 16:04:09.890233 jianglab-0.2.7/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.7/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 16:04:09.887489 jianglab-0.2.7/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.2.7/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    12710 2023-06-01 16:02:23.000000 jianglab-0.2.7/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.2.7/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 16:04:09.889726 jianglab-0.2.7/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-01 16:04:09.890672 jianglab-0.2.7/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      924 2023-06-01 16:04:04.000000 jianglab-0.2.7/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 17:42:31.703123 jianglab-0.2.8/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 17:42:31.702810 jianglab-0.2.8/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.8/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 17:42:31.700202 jianglab-0.2.8/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.2.8/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    12878 2023-06-01 17:42:22.000000 jianglab-0.2.8/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.2.8/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 17:42:31.702317 jianglab-0.2.8/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-01 17:42:31.703247 jianglab-0.2.8/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      924 2023-06-01 17:42:26.000000 jianglab-0.2.8/setup.py
```

### Comparing `jianglab-0.2.7/PKG-INFO` & `jianglab-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.7/README.md` & `jianglab-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.2.7/jianglab/common_functions.py` & `jianglab-0.2.8/jianglab/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 
 def load_raw_data(filepath):
     ''' load raw data from .cmcr or .cmtr file
     filepath: path to the .cmcr or .cmtr file'''
     raw_data = McsCMOSMEA.McsData(filepath)
     return raw_data
 
+def get_acquisition_rate(filepath):
+    raw_data = McsCMOSMEA.McsData(filepath)
+    return 1/(float(raw_data.Acquisition.Sensor_Data.SensorMeta["Tick"])*1e-6) # in Hz
+
 def cmcr_to_nparray(filepath):
     return load_raw_data(filepath).Acquisition.Sensor_Data.SensorData_1_1
 
 def import_cmtr_firing_rate(filename, bin_size = 100): 
     """Import a .cmtr file and return a dictionary of units holding the timestamps and waveforms.
     :param filename: The path to the .cmtr file.
     :return: A dictionary of units holding the timestamps and waveforms.
```

### Comparing `jianglab-0.2.7/jianglab.egg-info/PKG-INFO` & `jianglab-0.2.8/jianglab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.7/setup.py` & `jianglab-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.2.7',
+    version='0.2.8',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

