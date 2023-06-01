# Comparing `tmp/catencfamily-0.0.5.tar.gz` & `tmp/catencfamily-0.0.6.tar.gz`

## Comparing `catencfamily-0.0.5.tar` & `catencfamily-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.5/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.5/src/catencfamily/catencfamily.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.5/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.5/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 catencfamily-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 catencfamily-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.6/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.6/src/catencfamily/cef.py
+-rw-r--r--   0        0        0    44680 2020-02-02 00:00:00.000000 catencfamily-0.0.6/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.6/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 catencfamily-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 catencfamily-0.0.6/PKG-INFO
```

### Comparing `catencfamily-0.0.5/src/catencfamily/catencfamily.py` & `catencfamily-0.0.6/src/catencfamily/cef.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.5/LICENSE` & `catencfamily-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.5/README.md` & `catencfamily-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.5/pyproject.toml` & `catencfamily-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.5/PKG-INFO` & `catencfamily-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.5
+Version: 0.0.6
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

