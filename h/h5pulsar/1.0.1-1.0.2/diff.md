# Comparing `tmp/h5pulsar-1.0.1.tar.gz` & `tmp/h5pulsar-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5pulsar-1.0.1.tar", last modified: Thu Jun  1 01:51:02 2023, max compression
+gzip compressed data, was "h5pulsar-1.0.2.tar", last modified: Thu Jun  1 01:52:56 2023, max compression
```

## Comparing `h5pulsar-1.0.1.tar` & `h5pulsar-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-06-01 01:51:02.160294 h5pulsar-1.0.1/
--rw-r--r--   0 aaron      (501) staff       (20)     1107 2023-05-31 23:19:03.000000 h5pulsar-1.0.1/LICENSE
--rw-r--r--   0 aaron      (501) staff       (20)      545 2023-06-01 01:51:02.160164 h5pulsar-1.0.1/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)       70 2023-05-31 15:20:50.000000 h5pulsar-1.0.1/README.md
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-06-01 01:51:02.158957 h5pulsar-1.0.1/h5pulsar/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2023-05-31 15:17:57.000000 h5pulsar-1.0.1/h5pulsar/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)    16822 2023-05-31 20:41:25.000000 h5pulsar-1.0.1/h5pulsar/derivative_file.py
--rw-r--r--   0 aaron      (501) staff       (20)    22588 2023-05-31 20:54:29.000000 h5pulsar-1.0.1/h5pulsar/h5format.py
--rw-r--r--   0 aaron      (501) staff       (20)    27951 2023-05-31 20:56:49.000000 h5pulsar-1.0.1/h5pulsar/pulsar.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-06-01 01:51:02.160005 h5pulsar-1.0.1/h5pulsar.egg-info/
--rw-r--r--   0 aaron      (501) staff       (20)      545 2023-06-01 01:51:02.000000 h5pulsar-1.0.1/h5pulsar.egg-info/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)      297 2023-06-01 01:51:02.000000 h5pulsar-1.0.1/h5pulsar.egg-info/SOURCES.txt
--rw-r--r--   0 aaron      (501) staff       (20)        1 2023-06-01 01:51:02.000000 h5pulsar-1.0.1/h5pulsar.egg-info/dependency_links.txt
--rw-r--r--   0 aaron      (501) staff       (20)      148 2023-06-01 01:51:02.000000 h5pulsar-1.0.1/h5pulsar.egg-info/requires.txt
--rw-r--r--   0 aaron      (501) staff       (20)        9 2023-06-01 01:51:02.000000 h5pulsar-1.0.1/h5pulsar.egg-info/top_level.txt
--rw-r--r--   0 aaron      (501) staff       (20)      658 2023-06-01 01:48:20.000000 h5pulsar-1.0.1/pyproject.toml
--rw-r--r--   0 aaron      (501) staff       (20)      157 2023-06-01 01:50:44.000000 h5pulsar-1.0.1/requirements.txt
--rw-r--r--   0 aaron      (501) staff       (20)       38 2023-06-01 01:51:02.160333 h5pulsar-1.0.1/setup.cfg
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-06-01 01:52:56.879840 h5pulsar-1.0.2/
+-rw-r--r--   0 aaron      (501) staff       (20)     1107 2023-05-31 23:19:03.000000 h5pulsar-1.0.2/LICENSE
+-rw-r--r--   0 aaron      (501) staff       (20)      545 2023-06-01 01:52:56.879697 h5pulsar-1.0.2/PKG-INFO
+-rw-r--r--   0 aaron      (501) staff       (20)       70 2023-05-31 15:20:50.000000 h5pulsar-1.0.2/README.md
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-06-01 01:52:56.878176 h5pulsar-1.0.2/h5pulsar/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2023-05-31 15:17:57.000000 h5pulsar-1.0.2/h5pulsar/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    16822 2023-05-31 20:41:25.000000 h5pulsar-1.0.2/h5pulsar/derivative_file.py
+-rw-r--r--   0 aaron      (501) staff       (20)    22588 2023-05-31 20:54:29.000000 h5pulsar-1.0.2/h5pulsar/h5format.py
+-rw-r--r--   0 aaron      (501) staff       (20)    27951 2023-05-31 20:56:49.000000 h5pulsar-1.0.2/h5pulsar/pulsar.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-06-01 01:52:56.879463 h5pulsar-1.0.2/h5pulsar.egg-info/
+-rw-r--r--   0 aaron      (501) staff       (20)      545 2023-06-01 01:52:56.000000 h5pulsar-1.0.2/h5pulsar.egg-info/PKG-INFO
+-rw-r--r--   0 aaron      (501) staff       (20)      297 2023-06-01 01:52:56.000000 h5pulsar-1.0.2/h5pulsar.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron      (501) staff       (20)        1 2023-06-01 01:52:56.000000 h5pulsar-1.0.2/h5pulsar.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron      (501) staff       (20)      129 2023-06-01 01:52:56.000000 h5pulsar-1.0.2/h5pulsar.egg-info/requires.txt
+-rw-r--r--   0 aaron      (501) staff       (20)        9 2023-06-01 01:52:56.000000 h5pulsar-1.0.2/h5pulsar.egg-info/top_level.txt
+-rw-r--r--   0 aaron      (501) staff       (20)      658 2023-06-01 01:52:45.000000 h5pulsar-1.0.2/pyproject.toml
+-rw-r--r--   0 aaron      (501) staff       (20)      137 2023-06-01 01:52:40.000000 h5pulsar-1.0.2/requirements.txt
+-rw-r--r--   0 aaron      (501) staff       (20)       38 2023-06-01 01:52:56.879878 h5pulsar-1.0.2/setup.cfg
```

### Comparing `h5pulsar-1.0.1/LICENSE` & `h5pulsar-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `h5pulsar-1.0.1/PKG-INFO` & `h5pulsar-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5pulsar
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fork of Anne Archibald's code to add hdf5 to Pulsar objects
 Author-email: Aaron Johnson <aaron.johnson@nanograv.org>
 Project-URL: Homepage, https://github.com/AaronDJohnson/h5pulsar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `h5pulsar-1.0.1/h5pulsar/derivative_file.py` & `h5pulsar-1.0.2/h5pulsar/derivative_file.py`

 * *Files identical despite different names*

### Comparing `h5pulsar-1.0.1/h5pulsar/h5format.py` & `h5pulsar-1.0.2/h5pulsar/h5format.py`

 * *Files identical despite different names*

### Comparing `h5pulsar-1.0.1/h5pulsar/pulsar.py` & `h5pulsar-1.0.2/h5pulsar/pulsar.py`

 * *Files identical despite different names*

### Comparing `h5pulsar-1.0.1/h5pulsar.egg-info/PKG-INFO` & `h5pulsar-1.0.2/h5pulsar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5pulsar
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fork of Anne Archibald's code to add hdf5 to Pulsar objects
 Author-email: Aaron Johnson <aaron.johnson@nanograv.org>
 Project-URL: Homepage, https://github.com/AaronDJohnson/h5pulsar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `h5pulsar-1.0.1/pyproject.toml` & `h5pulsar-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "h5pulsar"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Aaron Johnson", email="aaron.johnson@nanograv.org" },
 ]
 description = "Fork of Anne Archibald's code to add hdf5 to Pulsar objects"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

