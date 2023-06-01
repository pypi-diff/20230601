# Comparing `tmp/pymilldb-0.0.4.tar.gz` & `tmp/pymilldb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilldb-0.0.4.tar", last modified: Tue May 30 21:12:09 2023, max compression
+gzip compressed data, was "pymilldb-0.0.5.tar", last modified: Thu Jun  1 18:42:50 2023, max compression
```

## Comparing `pymilldb-0.0.4.tar` & `pymilldb-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:12:09.144038 pymilldb-0.0.4/
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1095 2023-05-30 21:05:16.000000 pymilldb-0.0.4/LICENSE
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1001 2023-05-30 21:12:09.144038 pymilldb-0.0.4/PKG-INFO
--rw-r--r--   0 zeus      (1000) zeus      (1000)      493 2023-05-30 21:05:16.000000 pymilldb-0.0.4/README.md
--rw-r--r--   0 zeus      (1000) zeus      (1000)       89 2023-05-30 21:05:16.000000 pymilldb-0.0.4/pyproject.toml
--rw-r--r--   0 zeus      (1000) zeus      (1000)      633 2023-05-30 21:12:09.144038 pymilldb-0.0.4/setup.cfg
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:12:09.144038 pymilldb-0.0.4/src/
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:12:09.144038 pymilldb-0.0.4/src/pymilldb/
--rw-r--r--   0 zeus      (1000) zeus      (1000)      167 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/__init__.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     2669 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/mdb_client.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1554 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/protocol.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1602 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/sampler.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     9871 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/tensor_store.py
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:12:09.144038 pymilldb-0.0.4/src/pymilldb/utils/
--rw-r--r--   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/utils/__init__.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)      353 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/utils/decorators.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)      630 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/utils/graph.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1911 2023-05-30 21:05:16.000000 pymilldb-0.0.4/src/pymilldb/utils/packer.py
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:12:09.144038 pymilldb-0.0.4/src/pymilldb.egg-info/
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1001 2023-05-30 21:12:09.000000 pymilldb-0.0.4/src/pymilldb.egg-info/PKG-INFO
--rw-r--r--   0 zeus      (1000) zeus      (1000)      437 2023-05-30 21:12:09.000000 pymilldb-0.0.4/src/pymilldb.egg-info/SOURCES.txt
--rw-r--r--   0 zeus      (1000) zeus      (1000)        1 2023-05-30 21:12:09.000000 pymilldb-0.0.4/src/pymilldb.egg-info/dependency_links.txt
--rw-r--r--   0 zeus      (1000) zeus      (1000)        9 2023-05-30 21:12:09.000000 pymilldb-0.0.4/src/pymilldb.egg-info/top_level.txt
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.531944 pymilldb-0.0.5/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1095 2023-06-01 18:38:01.000000 pymilldb-0.0.5/LICENSE
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-01 18:42:50.531944 pymilldb-0.0.5/PKG-INFO
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      523 2023-06-01 18:38:01.000000 pymilldb-0.0.5/README.md
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)       89 2023-06-01 18:38:01.000000 pymilldb-0.0.5/pyproject.toml
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      633 2023-06-01 18:42:50.531944 pymilldb-0.0.5/setup.cfg
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.527944 pymilldb-0.0.5/src/
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.531944 pymilldb-0.0.5/src/pymilldb/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      167 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/__init__.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     2669 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/mdb_client.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1554 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/protocol.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1602 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/sampler.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     9875 2023-06-01 18:39:28.000000 pymilldb-0.0.5/src/pymilldb/tensor_store.py
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.531944 pymilldb-0.0.5/src/pymilldb/utils/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/utils/__init__.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      353 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/utils/decorators.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      630 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/utils/graph.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1911 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/utils/packer.py
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.531944 pymilldb-0.0.5/src/pymilldb.egg-info/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-01 18:42:50.000000 pymilldb-0.0.5/src/pymilldb.egg-info/PKG-INFO
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      437 2023-06-01 18:42:50.000000 pymilldb-0.0.5/src/pymilldb.egg-info/SOURCES.txt
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        1 2023-06-01 18:42:50.000000 pymilldb-0.0.5/src/pymilldb.egg-info/dependency_links.txt
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        9 2023-06-01 18:42:50.000000 pymilldb-0.0.5/src/pymilldb.egg-info/top_level.txt
```

### Comparing `pymilldb-0.0.4/LICENSE` & `pymilldb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.4/PKG-INFO` & `pymilldb-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMillDB: A python library for MillenniumDB
 
-**PyMillDB** is a library that implements modules and classes for interacting with [MillenniumDB](https://github.com/MillenniumDB/MillenniumDB).
+**PyMillDB** is a library that implements modules and classes for interacting with [MillenniumDB](https://github.com/MillenniumDB/MillenniumDB). 
 
 Most of the classes in this library require a `MDBClient` instance, which connects to the `pymilldb_server`, found at the `MillenniumDB-Dev/MillenniumAI` branch.
 
 For the `Doxygen` documentation, follow [this link](https://millenniumdb.github.io/PyMillDB/).
 
-This project is still under development.
+For installing the library, just run the `pip install pymdb` command.
```

### Comparing `pymilldb-0.0.4/setup.cfg` & `pymilldb-0.0.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymilldb
-version = 0.0.4
+version = 0.0.5
 author = Vicente Calisto
 author_email = vecalisto@uc.cl
 description = A python library for MillenniumDB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MillenniumDB/PyMillDB
 project_urls =
```

### Comparing `pymilldb-0.0.4/src/pymilldb/mdb_client.py` & `pymilldb-0.0.5/src/pymilldb/mdb_client.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.4/src/pymilldb/protocol.py` & `pymilldb-0.0.5/src/pymilldb/protocol.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.4/src/pymilldb/sampler.py` & `pymilldb-0.0.5/src/pymilldb/sampler.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.4/src/pymilldb/tensor_store.py` & `pymilldb-0.0.5/src/pymilldb/tensor_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         return self.size()
 
     ## Enter context manager.
     def __enter__(self):
         return self
 
     ## Exit context manager.
-    def __exit__(self):
+    def __exit__(self, *_):
         self.close()
 
     ## Get tensors from the store with the pythonic syntax `store[key]`.
     def __getitem__(self, key: Union[int, List[int]]) -> torch.Tensor:
         if isinstance(key, int):
             return self.get(key)
         else:
```

### Comparing `pymilldb-0.0.4/src/pymilldb/utils/graph.py` & `pymilldb-0.0.5/src/pymilldb/utils/graph.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.4/src/pymilldb/utils/packer.py` & `pymilldb-0.0.5/src/pymilldb/utils/packer.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.4/src/pymilldb.egg-info/PKG-INFO` & `pymilldb-0.0.5/src/pymilldb.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMillDB: A python library for MillenniumDB
 
-**PyMillDB** is a library that implements modules and classes for interacting with [MillenniumDB](https://github.com/MillenniumDB/MillenniumDB).
+**PyMillDB** is a library that implements modules and classes for interacting with [MillenniumDB](https://github.com/MillenniumDB/MillenniumDB). 
 
 Most of the classes in this library require a `MDBClient` instance, which connects to the `pymilldb_server`, found at the `MillenniumDB-Dev/MillenniumAI` branch.
 
 For the `Doxygen` documentation, follow [this link](https://millenniumdb.github.io/PyMillDB/).
 
-This project is still under development.
+For installing the library, just run the `pip install pymdb` command.
```

