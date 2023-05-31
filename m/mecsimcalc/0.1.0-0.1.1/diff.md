# Comparing `tmp/mecsimcalc-0.1.0.tar.gz` & `tmp/mecsimcalc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecsimcalc-0.1.0.tar", last modified: Wed May 31 21:39:58 2023, max compression
+gzip compressed data, was "mecsimcalc-0.1.1.tar", last modified: Wed May 31 22:58:41 2023, max compression
```

## Comparing `mecsimcalc-0.1.0.tar` & `mecsimcalc-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22654 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/mecsimcalc/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/spreadsheet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/mecsimcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:41.396383 mecsimcalc-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-31 22:58:41.396383 mecsimcalc-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22654 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:41.396383 mecsimcalc-0.1.1/mecsimcalc/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/mecsimcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/mecsimcalc/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/mecsimcalc/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/mecsimcalc/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/mecsimcalc/spreadsheet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/mecsimcalc/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/mecsimcalc/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:41.396383 mecsimcalc-0.1.1/mecsimcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-31 22:58:41.000000 mecsimcalc-0.1.1/mecsimcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-31 22:58:41.000000 mecsimcalc-0.1.1/mecsimcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:58:41.000000 mecsimcalc-0.1.1/mecsimcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 22:58:41.000000 mecsimcalc-0.1.1/mecsimcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 22:58:41.000000 mecsimcalc-0.1.1/mecsimcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:58:41.396383 mecsimcalc-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 22:58:27.000000 mecsimcalc-0.1.1/setup.py
```

### Comparing `mecsimcalc-0.1.0/LICENSE` & `mecsimcalc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.0/PKG-INFO` & `mecsimcalc-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecsimcalc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful functions for MecSimCalc.com
 Author: MecSimCalc
 Author-email: <info@mecsimcalc.com>
 Keywords: python,MecSimCalc,Calculator,Simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Mecsimcalc v0.1.0 documentation
+# Mecsimcalc v0.1.1 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
```

### Comparing `mecsimcalc-0.1.0/README.md` & `mecsimcalc-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Mecsimcalc v0.1.0 documentation
+# Mecsimcalc v0.1.1 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
```

### Comparing `mecsimcalc-0.1.0/mecsimcalc/__init__.py` & `mecsimcalc-0.1.1/mecsimcalc/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from general_utils import input_to_file, metadata_to_filetype
+from . import input_to_file, metadata_to_filetype
 
-from image_utils import input_to_PIL, file_to_PIL, print_img
+from . import input_to_PIL, file_to_PIL, print_img
 
-from plotting_utils import print_plot
+from . import print_plot
 
-from spreadsheet_utils import input_to_dataframe, file_to_dataframe, print_dataframe
+from . import input_to_dataframe, file_to_dataframe, print_dataframe
 
-from table_utils import table_to_dataframe, print_table
+from . import table_to_dataframe, print_table
 
-from text_utils import string_to_file
+from . import string_to_file
 
 
 __all__ = [
     "input_to_dataframe",
     "file_to_dataframe",
     "input_to_file",
     "input_to_PIL",
```

### Comparing `mecsimcalc-0.1.0/mecsimcalc/general_utils.py` & `mecsimcalc-0.1.1/mecsimcalc/general_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.0/mecsimcalc/image_utils.py` & `mecsimcalc-0.1.1/mecsimcalc/image_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.0/mecsimcalc/plotting_utils.py` & `mecsimcalc-0.1.1/mecsimcalc/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.0/mecsimcalc/spreadsheet_utils.py` & `mecsimcalc-0.1.1/mecsimcalc/spreadsheet_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.0/mecsimcalc/table_utils.py` & `mecsimcalc-0.1.1/mecsimcalc/table_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.0/mecsimcalc/text_utils.py` & `mecsimcalc-0.1.1/mecsimcalc/text_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.0/mecsimcalc.egg-info/PKG-INFO` & `mecsimcalc-0.1.1/mecsimcalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecsimcalc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful functions for MecSimCalc.com
 Author: MecSimCalc
 Author-email: <info@mecsimcalc.com>
 Keywords: python,MecSimCalc,Calculator,Simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Mecsimcalc v0.1.0 documentation
+# Mecsimcalc v0.1.1 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
```

### Comparing `mecsimcalc-0.1.0/setup.py` & `mecsimcalc-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 DESCRIPTION = "Useful functions for MecSimCalc.com"
 
 # Setting up
 setup(
     name="mecsimcalc",
     version=VERSION,
     author="MecSimCalc",
```

