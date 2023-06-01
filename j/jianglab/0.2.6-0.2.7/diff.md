# Comparing `tmp/jianglab-0.2.6.tar.gz` & `tmp/jianglab-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.2.6.tar", last modified: Tue May 30 19:31:37 2023, max compression
+gzip compressed data, was "jianglab-0.2.7.tar", last modified: Thu Jun  1 16:04:09 2023, max compression
```

## Comparing `jianglab-0.2.6.tar` & `jianglab-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 19:31:37.894437 jianglab-0.2.6/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 19:31:37.893840 jianglab-0.2.6/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.6/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 19:31:37.888096 jianglab-0.2.6/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.2.6/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    12735 2023-05-30 19:31:25.000000 jianglab-0.2.6/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.2.6/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 19:31:37.892311 jianglab-0.2.6/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 19:31:37.000000 jianglab-0.2.6/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-05-30 19:31:37.000000 jianglab-0.2.6/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-05-30 19:31:37.000000 jianglab-0.2.6/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       87 2023-05-30 19:31:37.000000 jianglab-0.2.6/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-05-30 19:31:37.000000 jianglab-0.2.6/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-05-30 19:31:37.894688 jianglab-0.2.6/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      892 2023-05-30 19:31:20.000000 jianglab-0.2.6/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 16:04:09.890548 jianglab-0.2.7/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 16:04:09.890233 jianglab-0.2.7/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.7/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 16:04:09.887489 jianglab-0.2.7/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.2.7/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    12710 2023-06-01 16:02:23.000000 jianglab-0.2.7/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.2.7/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 16:04:09.889726 jianglab-0.2.7/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-01 16:04:09.000000 jianglab-0.2.7/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-01 16:04:09.890672 jianglab-0.2.7/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      924 2023-06-01 16:04:04.000000 jianglab-0.2.7/setup.py
```

### Comparing `jianglab-0.2.6/PKG-INFO` & `jianglab-0.2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `jianglab-0.2.6/README.md` & `jianglab-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.2.6/jianglab/common_functions.py` & `jianglab-0.2.7/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from tqdm import tqdm
 from scipy.signal import find_peaks
 import matplotlib.pyplot as plt
 import gspread
 import pandas as pd
 from oauth2client.service_account import ServiceAccountCredentials
 import scipy.signal as signal
-import pickle5 as pickle
 from tqdm import tqdm
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
     '''
         Convert frame_ref to onset_index
         input:
             frame_ref: 2d array, first row is the light, second row is the frame
```

### Comparing `jianglab-0.2.6/jianglab.egg-info/PKG-INFO` & `jianglab-0.2.7/jianglab.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `jianglab-0.2.6/setup.py` & `jianglab-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.2.6',
+    version='0.2.7',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
         "tqdm",
         "scipy",
         "gspread",
         "oauth2client",
-        "pickle5"
 
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 )
```

