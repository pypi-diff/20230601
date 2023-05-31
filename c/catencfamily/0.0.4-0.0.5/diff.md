# Comparing `tmp/catencfamily-0.0.4.tar.gz` & `tmp/catencfamily-0.0.5.tar.gz`

## Comparing `catencfamily-0.0.4.tar` & `catencfamily-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.4/src/catfamilyenc/__init__.py
--rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.4/src/catfamilyenc/catencfamily.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.4/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.4/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 catencfamily-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 catencfamily-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.5/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.5/src/catencfamily/catencfamily.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.5/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 catencfamily-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 catencfamily-0.0.5/PKG-INFO
```

### Comparing `catencfamily-0.0.4/src/catfamilyenc/catencfamily.py` & `catencfamily-0.0.5/src/catencfamily/catencfamily.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.4/LICENSE` & `catencfamily-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.4/README.md` & `catencfamily-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.4/pyproject.toml` & `catencfamily-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.4/PKG-INFO` & `catencfamily-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.4
+Version: 0.0.5
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

