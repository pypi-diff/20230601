# Comparing `tmp/computing-toolbox-0.0.4.tar.gz` & `tmp/computing-toolbox-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.0.4.tar", last modified: Tue May 30 18:09:41 2023, max compression
+gzip compressed data, was "computing-toolbox-0.1.0.tar", last modified: Thu Jun  1 03:58:49 2023, max compression
```

## Comparing `computing-toolbox-0.0.4.tar` & `computing-toolbox-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:41.038226 computing-toolbox-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-30 18:09:41.034226 computing-toolbox-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:09:41.038226 computing-toolbox-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:41.034226 computing-toolbox-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:41.034226 computing-toolbox-0.0.4/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:41.034226 computing-toolbox-0.0.4/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:41.034226 computing-toolbox-0.0.4/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-30 18:09:31.000000 computing-toolbox-0.0.4/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:09:41.034226 computing-toolbox-0.0.4/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-30 18:09:41.000000 computing-toolbox-0.0.4/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-30 18:09:41.000000 computing-toolbox-0.0.4/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:09:41.000000 computing-toolbox-0.0.4/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-30 18:09:41.000000 computing-toolbox-0.0.4/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 18:09:41.000000 computing-toolbox-0.0.4/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.716709 computing-toolbox-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 03:58:49.716709 computing-toolbox-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:58:49.716709 computing-toolbox-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.712708 computing-toolbox-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.712708 computing-toolbox-0.1.0/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.712708 computing-toolbox-0.1.0/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.716709 computing-toolbox-0.1.0/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-01 03:58:40.000000 computing-toolbox-0.1.0/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:58:49.712708 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 03:58:49.000000 computing-toolbox-0.1.0/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.0.4/LICENSE` & `computing-toolbox-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.0.4/PKG-INFO` & `computing-toolbox-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.0.4
+Version: 0.1.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.0.4/README.md` & `computing-toolbox-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.0.4/pyproject.toml` & `computing-toolbox-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "computing-toolbox"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="Pedro Mayorga", email="ppmayorga80@gmail.com" },
 ]
 description = "Computing Toolbox for daily computations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `computing-toolbox-0.0.4/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.1.0/src/computing_toolbox/gcp/gs.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,40 +25,39 @@
         path = os.path.join(*args)
         if not path.startswith("gs://"):
             path = f"gs://{path}"
         return path
 
     @classmethod
     def exists(cls, path: str) -> bool:
-        """Test if a file or directory exists in Google Cloud Storage"""
+        """Test if a file or directory exists in Google Cloud Storage
+        if path is a directory make sure to write a '/' at the end of `path`
+
+        """
         try:
             _ = smart_open.open(path)
             return True
         except Exception:
             return False
 
     @classmethod
-    def list_files(cls, path: str, re_filter: str = "") -> Sequence[str]:
+    def list_files(cls, path: str, re_filter: str = r".*") -> Sequence[str]:
         """Given a path and a regex filter, list all files/dirs that match the filter
 
         :param path: the initial path where we start the search
         :param re_filter: a regular expression string in raw format, empty string means no filter (default: )
         :return: an iterator that walk over the files within `path` matching the `re_filter`
         """
         # compute the bucket and object names
         bucket_name, object_name = cls.split(path)
         # define if we have a regex function
-        re_filter_fn = re.compile(re_filter) if re_filter else None
+        re_filter_fn = re.compile(re_filter)
 
         # 1. walk over all objects within the path in the form (bucket_name,object_name)
         client = storage.Client()
         for blob in client.list_blobs(bucket_name, prefix=object_name):
             # 1.1 build the filename
             filename = cls.join(bucket_name, blob.name)
             # 1.2 decide if we have a regex function
-            if re_filter_fn:
-                # 1.2.1 if so, yield only the filename that pass the regex filter
-                if re_filter_fn.findall(filename):
-                    yield filename
-            # 1.3 if we don't have a regex function, no filter is applied
-            else:
+            # 1.2.1 if so, yield only the filename that pass the regex filter
+            if re_filter_fn.findall(filename):
                 yield filename
```

### Comparing `computing-toolbox-0.0.4/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.1.0/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.0.4/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.1.0/src/computing_toolbox/utils/deep_get.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     x={"name":{"first":"John","last":"Lennon"},"age":[None]}
     deep_get(x,["name","last"],"") -> "Lennon"
     deep_get(x,["name","last","middle"],"") -> ""
     deep_get(x,["age",0],3) -> 3
 
 """
 
-from typing import Union, List
+from typing import Union
 
 
-def deep_get(obj: Union[dict, List[any]], path: List[Union[str, int]],
+def deep_get(obj: Union[dict, list], path: list[Union[str, int]],
              default_value: any):
     """Gets the value at `path` of `x`.
     If the resolved value is None or some value in path doesn't exist,
     the `default_value` is returned in its place.
 
     :param obj: Object to search
     :param path: list of keys/int for successive deep search
```

### Comparing `computing-toolbox-0.0.4/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.1.0/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.0.4/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.1.0/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.0.4
+Version: 0.1.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.0.4/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.1.0/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,11 @@
 src/computing_toolbox.egg-info/requires.txt
 src/computing_toolbox.egg-info/top_level.txt
 src/computing_toolbox/gcp/__init__.py
 src/computing_toolbox/gcp/gs.py
 src/computing_toolbox/gcp/secret_manager.py
 src/computing_toolbox/utils/__init__.py
 src/computing_toolbox/utils/deep_get.py
+src/computing_toolbox/utils/es_long_search.py
+src/computing_toolbox/utils/http_fake_headers.py
+src/computing_toolbox/utils/http_request.py
 src/computing_toolbox/utils/tictoc.py
```

