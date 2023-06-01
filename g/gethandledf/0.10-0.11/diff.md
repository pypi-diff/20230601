# Comparing `tmp/gethandledf-0.10.tar.gz` & `tmp/gethandledf-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gethandledf-0.10.tar", last modified: Tue May 16 03:13:16 2023, max compression
+gzip compressed data, was "gethandledf-0.11.tar", last modified: Thu Jun  1 08:51:47 2023, max compression
```

## Comparing `gethandledf-0.10.tar` & `gethandledf-0.11.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 03:13:16.510568 gethandledf-0.10/
--rw-rw-rw-   0        0        0     1148 2023-05-16 03:13:06.000000 gethandledf-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      235 2023-05-16 03:13:05.000000 gethandledf-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     4143 2023-05-16 03:13:16.510568 gethandledf-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3460 2023-05-16 03:10:44.000000 gethandledf-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 03:13:16.507576 gethandledf-0.10/gethandledf/
--rw-rw-rw-   0        0        0     7490 2022-10-26 21:50:10.000000 gethandledf-0.10/gethandledf/Eula.txt
--rw-rw-rw-   0        0        0     3460 2023-05-16 03:10:44.000000 gethandledf-0.10/gethandledf/README.md
--rw-rw-rw-   0        0        0     5553 2023-05-16 03:03:38.000000 gethandledf-0.10/gethandledf/__init__.py
--rwxrwxrwx   0        0        0   761240 2022-10-26 21:50:28.000000 gethandledf-0.10/gethandledf/handle.exe
--rwxrwxrwx   0        0        0   416144 2022-10-26 21:50:28.000000 gethandledf-0.10/gethandledf/handle64.exe
--rwxrwxrwx   0        0        0   367512 2022-10-26 21:50:28.000000 gethandledf-0.10/gethandledf/handle64a.exe
--rw-rw-rw-   0        0        0       67 2023-05-16 03:13:15.000000 gethandledf-0.10/gethandledf/requirements.txt
--rw-rw-rw-   0        0        0    54606 2023-05-16 03:13:15.000000 gethandledf-0.10/gethandledf/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-16 03:13:16.510568 gethandledf-0.10/gethandledf.egg-info/
--rw-rw-rw-   0        0        0     4143 2023-05-16 03:13:16.000000 gethandledf-0.10/gethandledf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-05-16 03:13:16.000000 gethandledf-0.10/gethandledf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 03:13:16.000000 gethandledf-0.10/gethandledf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-16 03:13:16.000000 gethandledf-0.10/gethandledf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 03:13:16.000000 gethandledf-0.10/gethandledf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-16 03:13:16.511566 gethandledf-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-05-16 03:13:15.000000 gethandledf-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:51:47.020935 gethandledf-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-06-01 08:51:40.000000 gethandledf-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      235 2023-06-01 08:51:39.000000 gethandledf-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     4145 2023-06-01 08:51:47.020935 gethandledf-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3460 2023-05-16 03:10:44.000000 gethandledf-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:51:47.016947 gethandledf-0.11/gethandledf/
+-rw-rw-rw-   0        0        0     7490 2023-05-16 18:01:45.000000 gethandledf-0.11/gethandledf/Eula.txt
+-rw-rw-rw-   0        0        0     3460 2023-05-16 03:10:44.000000 gethandledf-0.11/gethandledf/README.md
+-rw-rw-rw-   0        0        0    10448 2023-06-01 08:50:10.000000 gethandledf-0.11/gethandledf/__init__.py
+-rwxrwxrwx   0        0        0   761240 2023-05-16 18:01:45.000000 gethandledf-0.11/gethandledf/handle.exe
+-rwxrwxrwx   0        0        0   416144 2023-05-16 18:01:45.000000 gethandledf-0.11/gethandledf/handle64.exe
+-rwxrwxrwx   0        0        0   367512 2023-05-16 18:01:45.000000 gethandledf-0.11/gethandledf/handle64a.exe
+-rw-rw-rw-   0        0        0       67 2023-06-01 08:51:46.000000 gethandledf-0.11/gethandledf/requirements.txt
+-rw-rw-rw-   0        0        0    54606 2023-06-01 08:51:46.000000 gethandledf-0.11/gethandledf/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-01 08:51:47.019910 gethandledf-0.11/gethandledf.egg-info/
+-rw-rw-rw-   0        0        0     4145 2023-06-01 08:51:46.000000 gethandledf-0.11/gethandledf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-01 08:51:46.000000 gethandledf-0.11/gethandledf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:51:46.000000 gethandledf-0.11/gethandledf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-01 08:51:46.000000 gethandledf-0.11/gethandledf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:51:46.000000 gethandledf-0.11/gethandledf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-01 08:51:47.020935 gethandledf-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1483 2023-06-01 08:51:46.000000 gethandledf-0.11/setup.py
```

### Comparing `gethandledf-0.10/LICENSE.rst` & `gethandledf-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gethandledf-0.10/PKG-INFO` & `gethandledf-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gethandledf
-Version: 0.10
+Version: 0.11
 Summary: Retrieves the list of handles using the 'handle.exe' command and return the data as a pandas DataFrame.
 Home-page: https://github.com/hansalemaos/gethandledf
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: wmic,process,pid,handle
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+
 # Retrieves the list of handles using the 'handle.exe' command and return the data as a pandas DataFrame.
 
 ## pip install gethandledf
 
 ### Tested against Windows 10 / Python 3.10 / Anaconda
 
 ## Python
```

### Comparing `gethandledf-0.10/README.md` & `gethandledf-0.11/README.md`

 * *Files identical despite different names*

### Comparing `gethandledf-0.10/gethandledf/Eula.txt` & `gethandledf-0.11/gethandledf/Eula.txt`

 * *Files identical despite different names*

### Comparing `gethandledf-0.10/gethandledf/README.md` & `gethandledf-0.11/gethandledf/README.md`

 * *Files identical despite different names*

### Comparing `gethandledf-0.10/gethandledf/handle.exe` & `gethandledf-0.11/gethandledf/handle.exe`

 * *Files identical despite different names*

### Comparing `gethandledf-0.10/gethandledf/handle64.exe` & `gethandledf-0.11/gethandledf/handle64.exe`

 * *Files identical despite different names*

### Comparing `gethandledf-0.10/gethandledf/handle64a.exe` & `gethandledf-0.11/gethandledf/handle64a.exe`

 * *Files identical despite different names*

### Comparing `gethandledf-0.10/gethandledf/thirdparty.json` & `gethandledf-0.11/gethandledf/thirdparty.json`

 * *Files identical despite different names*

### Comparing `gethandledf-0.10/gethandledf.egg-info/PKG-INFO` & `gethandledf-0.11/gethandledf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gethandledf
-Version: 0.10
+Version: 0.11
 Summary: Retrieves the list of handles using the 'handle.exe' command and return the data as a pandas DataFrame.
 Home-page: https://github.com/hansalemaos/gethandledf
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: wmic,process,pid,handle
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+
 # Retrieves the list of handles using the 'handle.exe' command and return the data as a pandas DataFrame.
 
 ## pip install gethandledf
 
 ### Tested against Windows 10 / Python 3.10 / Anaconda
 
 ## Python
```

### Comparing `gethandledf-0.10/setup.py` & `gethandledf-0.11/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
-# import codecs
-# import os
+import codecs
+import os
 # 
-# here = os.path.abspath(os.path.dirname(__file__))
+here = os.path.abspath(os.path.dirname(__file__))
 # 
-# with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-#     long_description = "\n" + fh.read()\
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+#long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Retrieves the list of handles using the 'handle.exe' command and return the data as a pandas DataFrame.'''
 
 # Setting up
 setup(
     name="gethandledf",
     version=VERSION,
     license='MIT',
```

