# Comparing `tmp/index_503-0.1.1.tar.gz` & `tmp/index_503-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.1.1.tar", max compression
+gzip compressed data, was "index_503-0.1.2.tar", max compression
```

## Comparing `index_503-0.1.1.tar` & `index_503-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-06-01 01:51:53.492920 index_503-0.1.1/LICENSE
--rw-r--r--   0        0        0     3481 2023-06-01 01:51:53.492920 index_503-0.1.1/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 01:51:54.256930 index_503-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 01:51:54.212930 index_503-0.1.1/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/file.py
--rw-r--r--   0        0        0     6904 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/index.py
--rw-r--r--   0        0        0      475 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/main.py
--rw-r--r--   0        0        0     2384 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/py.typed
--rw-r--r--   0        0        0      761 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/util.py
--rw-r--r--   0        0        0     3437 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 01:55:53.640358 index_503-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3481 2023-06-01 01:55:53.640358 index_503-0.1.2/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 01:55:54.392376 index_503-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 01:55:54.348375 index_503-0.1.2/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/file.py
+-rw-r--r--   0        0        0     7108 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/index.py
+-rw-r--r--   0        0        0      475 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/main.py
+-rw-r--r--   0        0        0     2384 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/py.typed
+-rw-r--r--   0        0        0      761 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/util.py
+-rw-r--r--   0        0        0     3437 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.2/PKG-INFO
```

### Comparing `index_503-0.1.1/LICENSE` & `index_503-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.1.1/README.md` & `index_503-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.1.1/pyproject.toml` & `index_503-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.1.1"
+version = "0.1.2"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.1.1/src/index_503/file.py` & `index_503-0.1.2/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.1/src/index_503/index.py` & `index_503-0.1.2/src/index_503/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 
             if wheel_cache and wheel_cache["version"] == WHEEL_FILE_VERSION:
                 wheel_file_obj = WheelFile(**wheel_cache)
                 projects[wheel_file_obj.metadata_name].append(wheel_file_obj)
                 previous_metadata_filename = target_path.joinpath(
                     metadata_filename.name
                 )
+                canonical_name = wheel_file_obj.canonical_name
+                metadata_name = wheel_file_obj.metadata_name
+                canonical_name_to_metadata_name[canonical_name] = metadata_name
                 copyfile(previous_metadata_filename, metadata_filename)
                 os.symlink(wheel_file_symlink_target, target_file)
                 continue
 
             with distributions.WheelDistribution.from_path(wheel_path) as wd:
                 if not wd.has_file("METADATA"):  # pragma: no cover
                     _LOGGER.warning(f"METADATA file not found in {wheel_path}")
```

### Comparing `index_503-0.1.1/src/index_503/page_generator.py` & `index_503-0.1.2/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.1/src/index_503/util.py` & `index_503-0.1.2/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.1/src/index_503/wheel_file.py` & `index_503-0.1.2/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.1/PKG-INFO` & `index_503-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.1.1
+Version: 0.1.2
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
-Metadata-Version: 2.1 Name: index-503 Version: 0.1.1 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.1.2 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

