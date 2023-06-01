# Comparing `tmp/soundmonitor-0.0.1.tar.gz` & `tmp/soundmonitor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundmonitor-0.0.1.tar", last modified: Thu Jun  1 20:11:58 2023, max compression
+gzip compressed data, was "soundmonitor-0.0.2.tar", last modified: Thu Jun  1 20:33:06 2023, max compression
```

## Comparing `soundmonitor-0.0.1.tar` & `soundmonitor-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 20:11:58.866982 soundmonitor-0.0.1/
--rw-rw-rw-   0        0        0    11548 2023-05-31 20:34:36.000000 soundmonitor-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4879 2023-06-01 20:11:58.870076 soundmonitor-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4269 2023-06-01 20:08:44.000000 soundmonitor-0.0.1/README.md
--rw-rw-rw-   0        0        0      817 2023-06-01 20:08:44.000000 soundmonitor-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      645 2023-06-01 20:11:58.872714 soundmonitor-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-01 19:46:21.000000 soundmonitor-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:11:58.848419 soundmonitor-0.0.1/soundmonitor/
--rw-rw-rw-   0        0        0       89 2023-06-01 15:51:10.000000 soundmonitor-0.0.1/soundmonitor/__init__.py
--rw-rw-rw-   0        0        0    12634 2023-06-01 15:49:18.000000 soundmonitor-0.0.1/soundmonitor/modules.py
--rw-rw-rw-   0        0        0     8393 2023-06-01 14:20:20.000000 soundmonitor-0.0.1/soundmonitor/utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:11:58.864913 soundmonitor-0.0.1/soundmonitor.egg-info/
--rw-rw-rw-   0        0        0     4879 2023-06-01 20:11:58.000000 soundmonitor-0.0.1/soundmonitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-06-01 20:11:58.000000 soundmonitor-0.0.1/soundmonitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 20:11:58.000000 soundmonitor-0.0.1/soundmonitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-01 20:11:58.000000 soundmonitor-0.0.1/soundmonitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-01 20:11:58.000000 soundmonitor-0.0.1/soundmonitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 20:33:06.526437 soundmonitor-0.0.2/
+-rw-rw-rw-   0        0        0    11548 2023-05-31 20:34:36.000000 soundmonitor-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4866 2023-06-01 20:33:06.526938 soundmonitor-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4256 2023-06-01 20:28:05.000000 soundmonitor-0.0.2/README.md
+-rw-rw-rw-   0        0        0      817 2023-06-01 20:31:15.000000 soundmonitor-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      645 2023-06-01 20:33:06.528346 soundmonitor-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-06-01 19:46:21.000000 soundmonitor-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:33:06.516194 soundmonitor-0.0.2/soundmonitor/
+-rw-rw-rw-   0        0        0       89 2023-06-01 15:51:10.000000 soundmonitor-0.0.2/soundmonitor/__init__.py
+-rw-rw-rw-   0        0        0    12634 2023-06-01 15:49:18.000000 soundmonitor-0.0.2/soundmonitor/modules.py
+-rw-rw-rw-   0        0        0     8393 2023-06-01 14:20:20.000000 soundmonitor-0.0.2/soundmonitor/utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:33:06.525397 soundmonitor-0.0.2/soundmonitor.egg-info/
+-rw-rw-rw-   0        0        0     4866 2023-06-01 20:33:06.000000 soundmonitor-0.0.2/soundmonitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-06-01 20:33:06.000000 soundmonitor-0.0.2/soundmonitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 20:33:06.000000 soundmonitor-0.0.2/soundmonitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-01 20:33:06.000000 soundmonitor-0.0.2/soundmonitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 20:33:06.000000 soundmonitor-0.0.2/soundmonitor.egg-info/top_level.txt
```

### Comparing `soundmonitor-0.0.1/LICENSE` & `soundmonitor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soundmonitor-0.0.1/PKG-INFO` & `soundmonitor-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundmonitor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Long-term sound level measurements analysis in Python
 Author: Valérian Fraisse
 Author-email: Valérian Fraisse <valerian.fraisse@mail.mcgill.ca>
 Project-URL: Homepage, https://github.com/valerianF/soundmonitor
 Project-URL: Bug Tracker, https://github.com/valerianF/soundmonitor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,17 +32,15 @@
 ## Usage
 
 ### Read sound level monitor data
 
 A function is included to read data in the form of either .csv, .xls, .xlsx or .txt files from a sound level monitor and convert them to a DataFrame with datetime or pandas TimeStamp index. Multiple files can be read at once, and the resulting data will be concatenated in a single DataFrame. Note that you must indicate the datasheet's indexes corresponding to date, time and captured equivalent sound level. Reading files with pandas and automatic parsing into datetime values can be computationaly expensive and the process can last a few minutes, depending on the input data.
 
 ```python
-import os
 from datetime import datetime
-
 import soundmonitor as sm
 
 # Load example .xslx data within the github repository
 df = sm.utilities.load_data(['tests/data/test.xlsx'], datetimeindex=0, valueindex=1)
 
 # Filter out data between or outside specified dates and times if required
 df = sm.utilities.filter_data(df, datetime(2022,8,10,3), datetime(2022,8,10,4), between=True)
```

### Comparing `soundmonitor-0.0.1/README.md` & `soundmonitor-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 ## Usage
 
 ### Read sound level monitor data
 
 A function is included to read data in the form of either .csv, .xls, .xlsx or .txt files from a sound level monitor and convert them to a DataFrame with datetime or pandas TimeStamp index. Multiple files can be read at once, and the resulting data will be concatenated in a single DataFrame. Note that you must indicate the datasheet's indexes corresponding to date, time and captured equivalent sound level. Reading files with pandas and automatic parsing into datetime values can be computationaly expensive and the process can last a few minutes, depending on the input data.
 
 ```python
-import os
 from datetime import datetime
-
 import soundmonitor as sm
 
 # Load example .xslx data within the github repository
 df = sm.utilities.load_data(['tests/data/test.xlsx'], datetimeindex=0, valueindex=1)
 
 # Filter out data between or outside specified dates and times if required
 df = sm.utilities.filter_data(df, datetime(2022,8,10,3), datetime(2022,8,10,4), between=True)
```

### Comparing `soundmonitor-0.0.1/pyproject.toml` & `soundmonitor-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "soundmonitor"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Valérian Fraisse", email="valerian.fraisse@mail.mcgill.ca" },
 ]
 description = "Long-term sound level measurements analysis in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 
 dependencies = [
-    "matplotlib >= 3.7.0",
+    "matplotlib >= 3.5.3",
     "numpy >= 1.21.6",
     "pandas >= 1.3.5",
     "xlrd >= 2.0.1",
     "openpyxl >= 3.1.2",
 ]
 
 classifiers = [
```

### Comparing `soundmonitor-0.0.1/setup.cfg` & `soundmonitor-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6f75 6e64 6d6f 6e69 746f 720d   = soundmonitor.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 4c6f 6e67 2d74 6572 6d20 736f 756e 6420  Long-term sound 
 00000050: 6c65 7665 6c20 6d65 6173 7572 656d 656e  level measuremen
 00000060: 7473 2061 6e61 6c79 7369 7320 696e 2050  ts analysis in P
 00000070: 7974 686f 6e0d 0a61 7574 686f 7220 3d20  ython..author = 
 00000080: 5661 6cc3 a972 6961 6e20 4672 6169 7373  Val..rian Fraiss
 00000090: 650d 0a61 7574 686f 725f 656d 6169 6c20  e..author_email 
@@ -26,15 +26,15 @@
 00000190: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
 000001a0: 2f45 6e67 696e 6565 7269 6e67 0d0a 0d0a  /Engineering....
 000001b0: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
 000001c0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
 000001d0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 000001e0: 3d33 2e37 0d0a 696e 7374 616c 6c5f 7265  =3.7..install_re
 000001f0: 7175 6972 6573 203d 200d 0a09 6d61 7470  quires = ...matp
-00000200: 6c6f 746c 6962 203e 3d20 332e 372e 300d  lotlib >= 3.7.0.
+00000200: 6c6f 746c 6962 203e 3d20 332e 352e 330d  lotlib >= 3.5.3.
 00000210: 0a09 6e75 6d70 7920 3e3d 2031 2e32 312e  ..numpy >= 1.21.
 00000220: 360d 0a09 7061 6e64 6173 203e 3d20 312e  6...pandas >= 1.
 00000230: 332e 350d 0a09 786c 7264 203e 3d20 322e  3.5...xlrd >= 2.
 00000240: 302e 310d 0a09 6f70 656e 7079 786c 203e  0.1...openpyxl >
 00000250: 3d20 332e 312e 320d 0a0d 0a5b 6567 675f  = 3.1.2....[egg_
 00000260: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
 00000270: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date =
```

### Comparing `soundmonitor-0.0.1/soundmonitor/modules.py` & `soundmonitor-0.0.2/soundmonitor/modules.py`

 * *Files identical despite different names*

### Comparing `soundmonitor-0.0.1/soundmonitor/utilities.py` & `soundmonitor-0.0.2/soundmonitor/utilities.py`

 * *Files identical despite different names*

### Comparing `soundmonitor-0.0.1/soundmonitor.egg-info/PKG-INFO` & `soundmonitor-0.0.2/soundmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundmonitor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Long-term sound level measurements analysis in Python
 Author: Valérian Fraisse
 Author-email: Valérian Fraisse <valerian.fraisse@mail.mcgill.ca>
 Project-URL: Homepage, https://github.com/valerianF/soundmonitor
 Project-URL: Bug Tracker, https://github.com/valerianF/soundmonitor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,17 +32,15 @@
 ## Usage
 
 ### Read sound level monitor data
 
 A function is included to read data in the form of either .csv, .xls, .xlsx or .txt files from a sound level monitor and convert them to a DataFrame with datetime or pandas TimeStamp index. Multiple files can be read at once, and the resulting data will be concatenated in a single DataFrame. Note that you must indicate the datasheet's indexes corresponding to date, time and captured equivalent sound level. Reading files with pandas and automatic parsing into datetime values can be computationaly expensive and the process can last a few minutes, depending on the input data.
 
 ```python
-import os
 from datetime import datetime
-
 import soundmonitor as sm
 
 # Load example .xslx data within the github repository
 df = sm.utilities.load_data(['tests/data/test.xlsx'], datetimeindex=0, valueindex=1)
 
 # Filter out data between or outside specified dates and times if required
 df = sm.utilities.filter_data(df, datetime(2022,8,10,3), datetime(2022,8,10,4), between=True)
```

