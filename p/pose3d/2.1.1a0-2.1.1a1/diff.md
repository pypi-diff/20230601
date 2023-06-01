# Comparing `tmp/pose3d-2.1.1a0.tar.gz` & `tmp/pose3d-2.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pose3d-2.1.1a0.tar", max compression
+gzip compressed data, was "pose3d-2.1.1a1.tar", max compression
```

## Comparing `pose3d-2.1.1a0.tar` & `pose3d-2.1.1a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-03-04 10:32:55.657329 pose3d-2.1.1a0/LICENSE
--rw-r--r--   0        0        0      412 2023-03-04 10:32:55.657393 pose3d-2.1.1a0/README.md
--rw-r--r--   0        0        0      134 2023-03-04 10:32:55.658906 pose3d-2.1.1a0/pose3d/__init__.py
--rw-r--r--   0        0        0    11316 2023-05-25 17:18:42.326499 pose3d-2.1.1a0/pose3d/er.py
--rw-r--r--   0        0        0     6589 2023-05-25 17:16:20.866753 pose3d-2.1.1a0/pose3d/et.py
--rw-r--r--   0        0        0     2344 2023-05-25 17:15:18.316495 pose3d-2.1.1a0/pose3d/pose.py
--rw-r--r--   0        0        0     4921 2023-05-25 17:12:54.769996 pose3d-2.1.1a0/pose3d/transform.py
--rw-r--r--   0        0        0     6810 2023-05-25 17:13:54.121857 pose3d-2.1.1a0/pose3d/transform_set.py
--rw-r--r--   0        0        0      597 2023-05-25 17:12:44.209814 pose3d-2.1.1a0/pose3d/utils.py
--rw-r--r--   0        0        0      555 2023-05-25 17:49:03.895610 pose3d-2.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 pose3d-2.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-04 10:32:55.657329 pose3d-2.1.1a1/LICENSE
+-rw-r--r--   0        0        0      819 2023-05-25 18:02:40.423273 pose3d-2.1.1a1/README.md
+-rw-r--r--   0        0        0      134 2023-03-04 10:32:55.658906 pose3d-2.1.1a1/pose3d/__init__.py
+-rw-r--r--   0        0        0    11316 2023-05-25 17:18:42.326499 pose3d-2.1.1a1/pose3d/er.py
+-rw-r--r--   0        0        0     6589 2023-05-25 17:16:20.866753 pose3d-2.1.1a1/pose3d/et.py
+-rw-r--r--   0        0        0     2344 2023-05-25 17:15:18.316495 pose3d-2.1.1a1/pose3d/pose.py
+-rw-r--r--   0        0        0     4921 2023-05-25 17:12:54.769996 pose3d-2.1.1a1/pose3d/transform.py
+-rw-r--r--   0        0        0     6810 2023-05-25 17:13:54.121857 pose3d-2.1.1a1/pose3d/transform_set.py
+-rw-r--r--   0        0        0      597 2023-05-25 17:12:44.209814 pose3d-2.1.1a1/pose3d/utils.py
+-rw-r--r--   0        0        0      555 2023-06-01 16:22:02.993899 pose3d-2.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 pose3d-2.1.1a1/PKG-INFO
```

### Comparing `pose3d-2.1.1a0/LICENSE` & `pose3d-2.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pose3d-2.1.1a0/pose3d/er.py` & `pose3d-2.1.1a1/pose3d/er.py`

 * *Files identical despite different names*

### Comparing `pose3d-2.1.1a0/pose3d/et.py` & `pose3d-2.1.1a1/pose3d/et.py`

 * *Files identical despite different names*

### Comparing `pose3d-2.1.1a0/pose3d/pose.py` & `pose3d-2.1.1a1/pose3d/pose.py`

 * *Files identical despite different names*

### Comparing `pose3d-2.1.1a0/pose3d/transform.py` & `pose3d-2.1.1a1/pose3d/transform.py`

 * *Files identical despite different names*

### Comparing `pose3d-2.1.1a0/pose3d/transform_set.py` & `pose3d-2.1.1a1/pose3d/transform_set.py`

 * *Files identical despite different names*

### Comparing `pose3d-2.1.1a0/pose3d/utils.py` & `pose3d-2.1.1a1/pose3d/utils.py`

 * *Files identical despite different names*

### Comparing `pose3d-2.1.1a0/pyproject.toml` & `pose3d-2.1.1a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pose3d"
-version = "2.1.1a0"
+version = "2.1.1a1"
 description = "Transforming and handling 3D poses and frames."
 authors = ["John Halazonetis <john.halazonetis@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pose3d"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pose3d-2.1.1a0/PKG-INFO` & `pose3d-2.1.1a1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pose3d
-Version: 2.1.1a0
+Version: 2.1.1a1
 Summary: Transforming and handling 3D poses and frames.
 License: MIT
 Author: John Halazonetis
 Author-email: john.halazonetis@icloud.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,13 +22,26 @@
 
 Handling 2D and 3D poses as well as transformations between reference frames.
 
 ## Documentation
 Visit page: <https://johnhalz.github.io/pose3d_python/>
 
 ## Installing Library
-This ibrary is freely available at the Python Package Index. You can install the latest version onto your machine with the following command:
+This library is freely available at the Python Package Index. You can install the latest version onto your machine with the following command:
 
 ``` bash
 pip install --upgrade pose3d
 ```
 
+## Developing
+This repo uses `poetry` as a dependency manager. You will need to download `poetry` onto your machine to be able to develop and push to this repo. You can install all required dependencies for development by running the command:
+
+``` bash
+poetry install
+```
+
+This should automatically make a virtual environment for you as well, which you can activate by running:
+
+``` bash
+poetry shell
+```
+
```

