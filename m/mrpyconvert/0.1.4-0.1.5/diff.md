# Comparing `tmp/mrpyconvert-0.1.4.tar.gz` & `tmp/mrpyconvert-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrpyconvert-0.1.4.tar", max compression
+gzip compressed data, was "mrpyconvert-0.1.5.tar", max compression
```

## Comparing `mrpyconvert-0.1.4.tar` & `mrpyconvert-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2022-04-19 22:33:27.705840 mrpyconvert-0.1.4/LICENSE
--rw-r--r--   0        0        0       94 2023-03-23 20:24:49.074668 mrpyconvert-0.1.4/README.md
--rw-r--r--   0        0        0       46 2023-05-31 23:07:30.786223 mrpyconvert-0.1.4/mrpyconvert/__init__.py
--rw-r--r--   0        0        0     1798 2023-03-23 20:24:49.121983 mrpyconvert-0.1.4/mrpyconvert/dicom_sorter.py
--rw-r--r--   0        0        0    15813 2023-03-23 20:24:49.191366 mrpyconvert-0.1.4/mrpyconvert/mrpyconvert.py
--rw-r--r--   0        0        0      424 2023-05-31 23:07:36.685758 mrpyconvert-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mrpyconvert-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-04-19 22:33:27.705840 mrpyconvert-0.1.5/LICENSE
+-rw-r--r--   0        0        0       94 2023-03-23 20:24:49.074668 mrpyconvert-0.1.5/README.md
+-rw-r--r--   0        0        0       46 2023-05-31 23:07:30.786223 mrpyconvert-0.1.5/mrpyconvert/__init__.py
+-rw-r--r--   0        0        0     1798 2023-03-23 20:24:49.121983 mrpyconvert-0.1.5/mrpyconvert/dicom_sorter.py
+-rw-r--r--   0        0        0    15813 2023-03-23 20:24:49.191366 mrpyconvert-0.1.5/mrpyconvert/mrpyconvert.py
+-rw-r--r--   0        0        0      426 2023-05-31 23:17:35.955261 mrpyconvert-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 mrpyconvert-0.1.5/PKG-INFO
```

### Comparing `mrpyconvert-0.1.4/LICENSE` & `mrpyconvert-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.4/mrpyconvert/dicom_sorter.py` & `mrpyconvert-0.1.5/mrpyconvert/dicom_sorter.py`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.4/mrpyconvert/mrpyconvert.py` & `mrpyconvert-0.1.5/mrpyconvert/mrpyconvert.py`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.4/PKG-INFO` & `mrpyconvert-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mrpyconvert
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tool to create scripts to convert dicom to bids
 License: MIT
 Author: Jolinda Smith
 Author-email: jolinda@uoregon.edu
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydicom (>=2.2,<3.0)
 Description-Content-Type: text/markdown
```

