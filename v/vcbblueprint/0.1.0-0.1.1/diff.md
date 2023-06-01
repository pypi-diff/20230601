# Comparing `tmp/vcbblueprint-0.1.0.tar.gz` & `tmp/vcbblueprint-0.1.1.tar.gz`

## Comparing `vcbblueprint-0.1.0.tar` & `vcbblueprint-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/requirements.txt
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/test_lib.py
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/vcbblueprint.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/LICENSE
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 vcbblueprint-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/test_lib.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/vcbblueprint.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/LICENSE
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/README.md
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 vcbblueprint-0.1.1/PKG-INFO
```

### Comparing `vcbblueprint-0.1.0/test_lib.py` & `vcbblueprint-0.1.1/test_lib.py`

 * *Files identical despite different names*

### Comparing `vcbblueprint-0.1.0/vcbblueprint.py` & `vcbblueprint-0.1.1/vcbblueprint.py`

 * *Files identical despite different names*

### Comparing `vcbblueprint-0.1.0/.github/workflows/python-package.yml` & `vcbblueprint-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `vcbblueprint-0.1.0/LICENSE` & `vcbblueprint-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vcbblueprint-0.1.0/README.md` & `vcbblueprint-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vcbblueprint-0.1.0/pyproject.toml` & `vcbblueprint-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vcbblueprint"
-version = "0.1.0"
+version = "0.1.1"
 description = "A library for decoding Virtual Circuit Board blueprint strings"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["vcb", "blueprint", "virtual circuit board"]
 authors = [
   { name = "Brandon Martin-Anderson", email = "badhill@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+  "numpy~=1.24.0",
+  "zstd~=1.5.0"
+]
+
 [project.urls]
 Homepage = "https://github.com/bmander/vcbblueprint/"
 Repository = "https://github.com/bmander/vcbblueprint.git"
```

### Comparing `vcbblueprint-0.1.0/PKG-INFO` & `vcbblueprint-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcbblueprint
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for decoding Virtual Circuit Board blueprint strings
 Project-URL: Homepage, https://github.com/bmander/vcbblueprint/
 Project-URL: Repository, https://github.com/bmander/vcbblueprint.git
 Author-email: Brandon Martin-Anderson <badhill@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Brandon Martin-Anderson
@@ -28,14 +28,16 @@
         SOFTWARE.
 License-File: LICENSE
 Keywords: blueprint,vcb,virtual circuit board
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: numpy~=1.24.0
+Requires-Dist: zstd~=1.5.0
 Description-Content-Type: text/markdown
 
 # Visual Circuit Board (VCB) Python Library
 
 ## Description
 
 This Python library provides a way to read Visual Circuit Board (VCB) blueprint strings and convert them into a convenient data structure.
```

