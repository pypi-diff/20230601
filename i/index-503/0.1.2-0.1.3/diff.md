# Comparing `tmp/index_503-0.1.2.tar.gz` & `tmp/index_503-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.1.2.tar", max compression
+gzip compressed data, was "index_503-0.1.3.tar", max compression
```

## Comparing `index_503-0.1.2.tar` & `index_503-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-06-01 01:55:53.640358 index_503-0.1.2/LICENSE
--rw-r--r--   0        0        0     3481 2023-06-01 01:55:53.640358 index_503-0.1.2/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 01:55:54.392376 index_503-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 01:55:54.348375 index_503-0.1.2/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/file.py
--rw-r--r--   0        0        0     7108 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/index.py
--rw-r--r--   0        0        0      475 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/main.py
--rw-r--r--   0        0        0     2384 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/py.typed
--rw-r--r--   0        0        0      761 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/util.py
--rw-r--r--   0        0        0     3437 2023-06-01 01:55:53.644358 index_503-0.1.2/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 02:12:50.413482 index_503-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3481 2023-06-01 02:12:50.413482 index_503-0.1.3/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 02:12:51.197494 index_503-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 02:12:51.153493 index_503-0.1.3/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/file.py
+-rw-r--r--   0        0        0     7471 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/index.py
+-rw-r--r--   0        0        0      475 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/main.py
+-rw-r--r--   0        0        0     2384 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/py.typed
+-rw-r--r--   0        0        0      761 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/util.py
+-rw-r--r--   0        0        0     3437 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.3/PKG-INFO
```

### Comparing `index_503-0.1.2/LICENSE` & `index_503-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.1.2/README.md` & `index_503-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.1.2/pyproject.toml` & `index_503-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.1.2"
+version = "0.1.3"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.1.2/src/index_503/file.py` & `index_503-0.1.3/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.2/src/index_503/index.py` & `index_503-0.1.3/src/index_503/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 _LOGGER = logging.getLogger(__name__)
 
 CACHE_FILE = "cache.json"
 
 
 def repair_metadata_file(
     metadata_file: Path, canonical_name_to_metadata_name: Dict[str, str]
-) -> None:
+) -> bool:
     """Repair the metadata file."""
     metadata_file_content = metadata_file.read_text().splitlines()
     # We have to parse the metadata file manually because the dist_meta library
     # doesn't support every version of the METADATA file.
     modified = False
     for index, line in enumerate(metadata_file_content):
         if line.startswith("Requires-Dist: "):
@@ -44,14 +44,16 @@
                 items[1] = metadata_name
                 metadata_file_content[index] = " ".join(items)
                 modified = True
         if line == "":
             break
     if modified:
         metadata_file.write_text("\n".join(metadata_file_content))
+        return True
+    return False
 
 
 def make_index(origin_path: Path) -> Tuple[Path, Dict[str, List["WheelFile"]]]:
     """Generate a simple repository of Python wheels.
 
     This function will take a directory of wheels at the top level
     of a webserver and generate a simple repository of wheels.
@@ -76,67 +78,69 @@
 
     with tempfile.TemporaryDirectory(
         dir=str(target_path_parent), ignore_cleanup_errors=True
     ) as temp_dir:
         temp_dir_path = Path(temp_dir)
         all_wheel_files: set[str] = set()
         canonical_name_to_metadata_name: Dict[str, str] = {}
-        metadata_files_to_repair: List[Path] = []
+        new_wheel_file_objects: List[WheelFile] = []
+        file_name_as_posix_to_metadata_path: Dict[str, Path] = {}
 
         for wheel_file in glob.glob(str(origin_path.joinpath("*.whl"))):
             wheel_path = Path(wheel_file)
             wheel_file_name = wheel_path.name
             all_wheel_files.add(wheel_file_name)
             target_file = temp_dir_path.joinpath(wheel_file_name)
-            metadata_filename = target_file.with_suffix(
-                f"{target_file.suffix}.metadata"
-            )
+            metadata_path = target_file.with_suffix(f"{target_file.suffix}.metadata")
             wheel_file_symlink_target = f"../{origin_name}/{wheel_path.name}"
             wheel_cache = cache.get(wheel_file_name)
 
             if wheel_cache and wheel_cache["version"] == WHEEL_FILE_VERSION:
                 wheel_file_obj = WheelFile(**wheel_cache)
                 projects[wheel_file_obj.metadata_name].append(wheel_file_obj)
-                previous_metadata_filename = target_path.joinpath(
-                    metadata_filename.name
-                )
+                previous_metadata_filename = target_path.joinpath(metadata_path.name)
                 canonical_name = wheel_file_obj.canonical_name
                 metadata_name = wheel_file_obj.metadata_name
                 canonical_name_to_metadata_name[canonical_name] = metadata_name
-                copyfile(previous_metadata_filename, metadata_filename)
+                copyfile(previous_metadata_filename, metadata_path)
                 os.symlink(wheel_file_symlink_target, target_file)
                 continue
 
             with distributions.WheelDistribution.from_path(wheel_path) as wd:
                 if not wd.has_file("METADATA"):  # pragma: no cover
                     _LOGGER.warning(f"METADATA file not found in {wheel_path}")
                     continue
                 metadata_string = wd.read_file("METADATA")
                 wheel_metadata = metadata.loads(metadata_string)
 
-            metadata_filename.write_text(metadata_string)
-            metadata_files_to_repair.append(metadata_filename)
+            metadata_path.write_text(metadata_string)
             metadata_name = wheel_metadata["Name"]
             canonical_name = canonicalize_name(metadata_name)
+            file_name_as_posix = target_file.relative_to(temp_dir_path).as_posix()
+            file_name_as_posix_to_metadata_path[file_name_as_posix] = metadata_path
             wheel_file_obj = WheelFile(
                 version=WHEEL_FILE_VERSION,
                 metadata_name=metadata_name,
                 canonical_name=canonical_name,
-                filename=target_file.relative_to(temp_dir_path).as_posix(),
+                filename=file_name_as_posix,
                 wheel_hash=get_sha256_hash(wheel_path),
                 requires_python=wheel_metadata.get("Requires-Python"),
-                metadata_hash=get_sha256_hash(metadata_filename),
+                metadata_hash=get_sha256_hash(metadata_path),
             )
+            new_wheel_file_objects.append(wheel_file_obj)
             canonical_name_to_metadata_name[canonical_name] = metadata_name
             projects[metadata_name].append(wheel_file_obj)
             cache[wheel_file_name] = asdict(wheel_file_obj)
             os.symlink(wheel_file_symlink_target, target_file)
 
-        for metadata_filename in metadata_files_to_repair:
-            repair_metadata_file(metadata_filename, canonical_name_to_metadata_name)
+        for wheel_file_obj in new_wheel_file_objects:
+            file_name_as_posix = wheel_file_obj.filename
+            metadata_path = file_name_as_posix_to_metadata_path[file_name_as_posix]
+            if repair_metadata_file(metadata_path, canonical_name_to_metadata_name):
+                wheel_file_obj.metadata_hash = get_sha256_hash(metadata_path)
 
         removed_wheels = set(cache.keys()) - all_wheel_files
         for old_wheel_file in removed_wheels:
             del cache[old_wheel_file]
 
         index_content = str(generate_index(projects.keys()))
         write_utf8_file(temp_dir_path.joinpath("index.html"), index_content)
```

### Comparing `index_503-0.1.2/src/index_503/page_generator.py` & `index_503-0.1.3/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.2/src/index_503/util.py` & `index_503-0.1.3/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.2/src/index_503/wheel_file.py` & `index_503-0.1.3/src/index_503/wheel_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from html import escape
 from typing import Optional, Union
 
 from airium import Airium
 from typing_extensions import Literal
 from yarl import URL
 
-WHEEL_FILE_VERSION = 1
+WHEEL_FILE_VERSION = 2
 
 
 @dataclass
 class WheelFile:
     """
     Represents a wheel file in the repository.
     """
```

### Comparing `index_503-0.1.2/PKG-INFO` & `index_503-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.1.2
+Version: 0.1.3
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
-Metadata-Version: 2.1 Name: index-503 Version: 0.1.2 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.1.3 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

