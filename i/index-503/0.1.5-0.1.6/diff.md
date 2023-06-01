# Comparing `tmp/index_503-0.1.5.tar.gz` & `tmp/index_503-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.1.5.tar", max compression
+gzip compressed data, was "index_503-0.1.6.tar", max compression
```

## Comparing `index_503-0.1.5.tar` & `index_503-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-06-01 03:03:21.026161 index_503-0.1.5/LICENSE
--rw-r--r--   0        0        0     3481 2023-06-01 03:03:21.026161 index_503-0.1.5/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 03:03:21.766169 index_503-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 03:03:21.726168 index_503-0.1.5/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-01 03:03:21.030161 index_503-0.1.5/src/index_503/file.py
--rw-r--r--   0        0        0     7890 2023-06-01 03:03:21.030161 index_503-0.1.5/src/index_503/index.py
--rw-r--r--   0        0        0      475 2023-06-01 03:03:21.030161 index_503-0.1.5/src/index_503/main.py
--rw-r--r--   0        0        0     2384 2023-06-01 03:03:21.030161 index_503-0.1.5/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 03:03:21.030161 index_503-0.1.5/src/index_503/py.typed
--rw-r--r--   0        0        0      761 2023-06-01 03:03:21.030161 index_503-0.1.5/src/index_503/util.py
--rw-r--r--   0        0        0     3398 2023-06-01 03:03:21.030161 index_503-0.1.5/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 03:16:49.437121 index_503-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3481 2023-06-01 03:16:49.437121 index_503-0.1.6/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 03:16:50.385128 index_503-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 03:16:50.337128 index_503-0.1.6/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/file.py
+-rw-r--r--   0        0        0     7996 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/index.py
+-rw-r--r--   0        0        0      475 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/main.py
+-rw-r--r--   0        0        0     2384 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/py.typed
+-rw-r--r--   0        0        0      761 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/util.py
+-rw-r--r--   0        0        0     3398 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.6/PKG-INFO
```

### Comparing `index_503-0.1.5/LICENSE` & `index_503-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.1.5/README.md` & `index_503-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.1.5/pyproject.toml` & `index_503-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.1.5"
+version = "0.1.6"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.1.5/src/index_503/file.py` & `index_503-0.1.6/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.5/src/index_503/index.py` & `index_503-0.1.6/src/index_503/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,23 @@
     # We have to parse the metadata file manually because the dist_meta library
     # doesn't support every version of the METADATA file.
     modified = False
 
     for index, line in enumerate(metadata_file_content):
         if line.startswith("Requires-Dist: "):
             items = line.split(" ")
-            canonical_name = canonicalize_name(items[1])
+            original_name = items[1]
+            canonical_name = canonicalize_name(original_name)
             metadata_name = canonical_name_to_metadata_name.get(canonical_name)
-            if metadata_name and metadata_name != canonical_name:
+            if metadata_name and metadata_name != original_name:
                 _LOGGER.warning(
-                    f"Repairing {metadata_file} Requires-Dist {canonical_name} -> {metadata_name}"
+                    "Repairing %s Requires-Dist %s -> %s",
+                    metadata_file,
+                    original_name,
+                    metadata_name,
                 )
                 items[1] = metadata_name
                 metadata_file_content[index] = " ".join(items)
                 modified = True
         if line == "":
             break
```

### Comparing `index_503-0.1.5/src/index_503/page_generator.py` & `index_503-0.1.6/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.5/src/index_503/util.py` & `index_503-0.1.6/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.5/src/index_503/wheel_file.py` & `index_503-0.1.6/src/index_503/wheel_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from html import escape
 from typing import Optional, Union
 
 from airium import Airium
 from typing_extensions import Literal
 from yarl import URL
 
-WHEEL_FILE_VERSION = 8
+WHEEL_FILE_VERSION = 9
 
 
 @dataclass
 class WheelFile:
     """
     Represents a wheel file in the repository.
     """
```

### Comparing `index_503-0.1.5/PKG-INFO` & `index_503-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.1.5
+Version: 0.1.6
 Summary: PEP 503 index builder
 Home-page: https://github.com/bdraco/index-503
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: index-503 Version: 0.1.5 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.1.6 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

