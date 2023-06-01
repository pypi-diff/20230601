# Comparing `tmp/index_503-0.1.7.tar.gz` & `tmp/index_503-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.1.7.tar", max compression
+gzip compressed data, was "index_503-0.1.8.tar", max compression
```

## Comparing `index_503-0.1.7.tar` & `index_503-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-06-01 13:08:55.567221 index_503-0.1.7/LICENSE
--rw-r--r--   0        0        0     3481 2023-06-01 13:08:55.567221 index_503-0.1.7/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 13:08:56.363241 index_503-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 13:08:56.319240 index_503-0.1.7/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/file.py
--rw-r--r--   0        0        0     7496 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/py.typed
--rw-r--r--   0        0        0      792 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/util.py
--rw-r--r--   0        0        0     4585 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 13:16:32.567199 index_503-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3481 2023-06-01 13:16:32.567199 index_503-0.1.8/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 13:16:33.315205 index_503-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 13:16:33.275205 index_503-0.1.8/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/file.py
+-rw-r--r--   0        0        0     7539 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/py.typed
+-rw-r--r--   0        0        0      792 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/util.py
+-rw-r--r--   0        0        0     4585 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.8/PKG-INFO
```

### Comparing `index_503-0.1.7/LICENSE` & `index_503-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.1.7/README.md` & `index_503-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.1.7/pyproject.toml` & `index_503-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.1.7"
+version = "0.1.8"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.1.7/src/index_503/file.py` & `index_503-0.1.8/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.7/src/index_503/index.py` & `index_503-0.1.8/src/index_503/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,31 +67,31 @@
 
     def __init__(self, origin_path: Path) -> None:
         """Generate a simple repository of Python wheels."""
         self.origin_path = origin_path
         self.origin_name = origin_path.name
         target_path = origin_path.parent / (origin_path.name + "-index")
         self.target_path = target_path
-        self.old_index = target_path.readlink() if target_path.exists() else None
-        self.target_path_parent = target_path.parent
         self.cache = IndexCache(target_path)
-        self.canonical_name_to_metadata_name: Dict[str, str] = {}
 
     def make_index(self) -> Path:
         """Generate a simple repository of Python wheels."""
         with tempfile.TemporaryDirectory(
-            dir=str(self.target_path_parent), ignore_cleanup_errors=True
+            dir=str(self.target_path.parent), ignore_cleanup_errors=True
         ) as temp_dir:
             temp_dir_path = Path(temp_dir)
 
             self._make_index_at_temp_dir(temp_dir_path)
             self._atomic_replace_old_index(temp_dir_path)
 
-            if self.old_index:
-                rmtree(self.old_index)
+            old_index = (
+                self.target_path.readlink() if self.target_path.exists() else None
+            )
+            if old_index:
+                rmtree(old_index)
 
             return self.target_path
 
     def _atomic_replace_old_index(self, temp_dir_path: Path) -> None:
         """Atomically replace the old index with the new one."""
         final_name = self.target_path.parent / (
             self.target_path.name + "-" + temp_dir_path.name
@@ -109,14 +109,15 @@
 
     def _make_index_at_temp_dir(self, temp_dir_path: Path) -> None:
         """Generate a simple repository of Python wheels in a temp dir."""
         new_wheel_file_objects: List[WheelFile] = []
         projects: Dict[str, List[WheelFile]] = defaultdict(list)
         wheel_file_name_to_metadata_path: Dict[str, Path] = {}
         all_wheel_files: Set[str] = set()
+        canonical_name_to_metadata_name: Dict[str, str] = {}
 
         for wheel_file in glob.glob(str(self.origin_path.joinpath("*.whl"))):
             wheel_path = Path(wheel_file)
             wheel_file_name = wheel_path.name
             all_wheel_files.add(wheel_file_name)
             target_file = temp_dir_path.joinpath(wheel_file_name)
             metadata_path = target_file.with_suffix(f"{target_file.suffix}.metadata")
@@ -134,38 +135,39 @@
                 wheel_file_name_to_metadata_path[wheel_file_name] = metadata_path
                 new_wheel_file_objects.append(wheel_file_obj)
                 self.cache.cache[wheel_file_name] = asdict(wheel_file_obj)
 
             canonical_name = wheel_file_obj.canonical_name
             metadata_name = wheel_file_obj.metadata_name
             projects[metadata_name].append(wheel_file_obj)
-            self.canonical_name_to_metadata_name[canonical_name] = metadata_name
+            canonical_name_to_metadata_name[canonical_name] = metadata_name
             os.symlink(wheel_file_symlink_target, target_file)
 
         self.cache.remove_stale_keys(all_wheel_files)
         self.repair_metadata_files(
-            new_wheel_file_objects, wheel_file_name_to_metadata_path
+            new_wheel_file_objects,
+            wheel_file_name_to_metadata_path,
+            canonical_name_to_metadata_name,
         )
         self.generate_index_pages(temp_dir_path, projects)
         self.cache.write_to_new(temp_dir_path)
 
     def repair_metadata_files(
         self,
         new_wheel_file_objects: List[WheelFile],
-        wheel_file_name_to_metadata_path: Dict[str, Path] = {},
+        wheel_file_name_to_metadata_path: Dict[str, Path],
+        canonical_name_to_metadata_name: Dict[str, str],
     ) -> None:
         """Repair the metadata files."""
         # Now fix all the metadata files and update the sha256 hash + cache
         for wheel_file_obj in new_wheel_file_objects:
             wheel_file_name = wheel_file_obj.filename
             metadata_path = wheel_file_name_to_metadata_path[wheel_file_name]
 
-            if repair_metadata_file(
-                metadata_path, self.canonical_name_to_metadata_name
-            ):
+            if repair_metadata_file(metadata_path, canonical_name_to_metadata_name):
                 wheel_file_obj.metadata_hash = get_sha256_hash(metadata_path)
                 self.cache.cache[wheel_file_name] = asdict(wheel_file_obj)
 
     def generate_index_pages(
         self, temp_dir_path: Path, projects: Dict[str, List[WheelFile]]
     ) -> None:
         """Generate the index pages."""
```

### Comparing `index_503-0.1.7/src/index_503/metadata.py` & `index_503-0.1.8/src/index_503/metadata.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.7/src/index_503/page_generator.py` & `index_503-0.1.8/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.7/src/index_503/util.py` & `index_503-0.1.8/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.7/src/index_503/wheel_file.py` & `index_503-0.1.8/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.7/PKG-INFO` & `index_503-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.1.7
+Version: 0.1.8
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
-Metadata-Version: 2.1 Name: index-503 Version: 0.1.7 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.1.8 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

