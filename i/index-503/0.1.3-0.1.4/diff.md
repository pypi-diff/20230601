# Comparing `tmp/index_503-0.1.3.tar.gz` & `tmp/index_503-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.1.3.tar", max compression
+gzip compressed data, was "index_503-0.1.4.tar", max compression
```

## Comparing `index_503-0.1.3.tar` & `index_503-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-06-01 02:12:50.413482 index_503-0.1.3/LICENSE
--rw-r--r--   0        0        0     3481 2023-06-01 02:12:50.413482 index_503-0.1.3/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 02:12:51.197494 index_503-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 02:12:51.153493 index_503-0.1.3/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/file.py
--rw-r--r--   0        0        0     7471 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/index.py
--rw-r--r--   0        0        0      475 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/main.py
--rw-r--r--   0        0        0     2384 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/py.typed
--rw-r--r--   0        0        0      761 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/util.py
--rw-r--r--   0        0        0     3437 2023-06-01 02:12:50.417482 index_503-0.1.3/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 02:56:13.628272 index_503-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3481 2023-06-01 02:56:13.628272 index_503-0.1.4/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 02:56:14.464276 index_503-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 02:56:14.420276 index_503-0.1.4/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-01 02:56:13.628272 index_503-0.1.4/src/index_503/file.py
+-rw-r--r--   0        0        0     7871 2023-06-01 02:56:13.628272 index_503-0.1.4/src/index_503/index.py
+-rw-r--r--   0        0        0      475 2023-06-01 02:56:13.628272 index_503-0.1.4/src/index_503/main.py
+-rw-r--r--   0        0        0     2384 2023-06-01 02:56:13.628272 index_503-0.1.4/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 02:56:13.628272 index_503-0.1.4/src/index_503/py.typed
+-rw-r--r--   0        0        0      761 2023-06-01 02:56:13.628272 index_503-0.1.4/src/index_503/util.py
+-rw-r--r--   0        0        0     3398 2023-06-01 02:56:13.628272 index_503-0.1.4/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.4/PKG-INFO
```

### Comparing `index_503-0.1.3/LICENSE` & `index_503-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.1.3/README.md` & `index_503-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.1.3/pyproject.toml` & `index_503-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.1.3"
+version = "0.1.4"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.1.3/src/index_503/file.py` & `index_503-0.1.4/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.3/src/index_503/index.py` & `index_503-0.1.4/src/index_503/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import tempfile
 from collections import defaultdict
 from dataclasses import asdict
 from operator import attrgetter
 from pathlib import Path
 from shutil import copyfile, rmtree
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 from dist_meta import distributions, metadata
 from natsort import natsorted
 from yarl import URL
 
 from .file import write_utf8_file
 from .page_generator import canonicalize_name, generate_index, generate_project_page
@@ -28,32 +28,43 @@
     metadata_file: Path, canonical_name_to_metadata_name: Dict[str, str]
 ) -> bool:
     """Repair the metadata file."""
     metadata_file_content = metadata_file.read_text().splitlines()
     # We have to parse the metadata file manually because the dist_meta library
     # doesn't support every version of the METADATA file.
     modified = False
+
     for index, line in enumerate(metadata_file_content):
         if line.startswith("Requires-Dist: "):
             items = line.split(" ")
             canonical_name = items[1]
             metadata_name = canonical_name_to_metadata_name.get(canonical_name)
             if metadata_name and metadata_name != canonical_name:
                 _LOGGER.warning(
                     f"Repairing {metadata_file} Requires-Dist {canonical_name} -> {metadata_name}"
                 )
                 items[1] = metadata_name
                 metadata_file_content[index] = " ".join(items)
                 modified = True
         if line == "":
             break
+
     if modified:
         metadata_file.write_text("\n".join(metadata_file_content))
-        return True
-    return False
+
+    return modified
+
+
+def extract_metadata_from_wheel_file(wheel_path: Path) -> Optional[str]:
+    """Extract the METADATA file from a wheel file."""
+    with distributions.WheelDistribution.from_path(wheel_path) as wd:
+        if not wd.has_file("METADATA"):  # pragma: no cover
+            _LOGGER.warning(f"METADATA file not found in {wheel_path}")
+            return None
+        return wd.read_file("METADATA")
 
 
 def make_index(origin_path: Path) -> Tuple[Path, Dict[str, List["WheelFile"]]]:
     """Generate a simple repository of Python wheels.
 
     This function will take a directory of wheels at the top level
     of a webserver and generate a simple repository of wheels.
@@ -84,64 +95,66 @@
         canonical_name_to_metadata_name: Dict[str, str] = {}
         new_wheel_file_objects: List[WheelFile] = []
         file_name_as_posix_to_metadata_path: Dict[str, Path] = {}
 
         for wheel_file in glob.glob(str(origin_path.joinpath("*.whl"))):
             wheel_path = Path(wheel_file)
             wheel_file_name = wheel_path.name
-            all_wheel_files.add(wheel_file_name)
             target_file = temp_dir_path.joinpath(wheel_file_name)
             metadata_path = target_file.with_suffix(f"{target_file.suffix}.metadata")
             wheel_file_symlink_target = f"../{origin_name}/{wheel_path.name}"
-            wheel_cache = cache.get(wheel_file_name)
+            file_name_as_posix = target_file.relative_to(temp_dir_path).as_posix()
+            wheel_cache = cache.get(file_name_as_posix)
+            all_wheel_files.add(file_name_as_posix)
 
             if wheel_cache and wheel_cache["version"] == WHEEL_FILE_VERSION:
                 wheel_file_obj = WheelFile(**wheel_cache)
-                projects[wheel_file_obj.metadata_name].append(wheel_file_obj)
                 previous_metadata_filename = target_path.joinpath(metadata_path.name)
                 canonical_name = wheel_file_obj.canonical_name
                 metadata_name = wheel_file_obj.metadata_name
                 canonical_name_to_metadata_name[canonical_name] = metadata_name
+                projects[metadata_name].append(wheel_file_obj)
                 copyfile(previous_metadata_filename, metadata_path)
                 os.symlink(wheel_file_symlink_target, target_file)
                 continue
 
-            with distributions.WheelDistribution.from_path(wheel_path) as wd:
-                if not wd.has_file("METADATA"):  # pragma: no cover
-                    _LOGGER.warning(f"METADATA file not found in {wheel_path}")
-                    continue
-                metadata_string = wd.read_file("METADATA")
-                wheel_metadata = metadata.loads(metadata_string)
+            metadata_string = extract_metadata_from_wheel_file(wheel_path)
+            if not metadata_string:
+                continue
+            wheel_metadata = metadata.loads(metadata_string)
 
             metadata_path.write_text(metadata_string)
             metadata_name = wheel_metadata["Name"]
             canonical_name = canonicalize_name(metadata_name)
-            file_name_as_posix = target_file.relative_to(temp_dir_path).as_posix()
             file_name_as_posix_to_metadata_path[file_name_as_posix] = metadata_path
             wheel_file_obj = WheelFile(
                 version=WHEEL_FILE_VERSION,
                 metadata_name=metadata_name,
                 canonical_name=canonical_name,
                 filename=file_name_as_posix,
                 wheel_hash=get_sha256_hash(wheel_path),
                 requires_python=wheel_metadata.get("Requires-Python"),
                 metadata_hash=get_sha256_hash(metadata_path),
             )
             new_wheel_file_objects.append(wheel_file_obj)
             canonical_name_to_metadata_name[canonical_name] = metadata_name
             projects[metadata_name].append(wheel_file_obj)
-            cache[wheel_file_name] = asdict(wheel_file_obj)
+            cache[file_name_as_posix] = asdict(wheel_file_obj)
             os.symlink(wheel_file_symlink_target, target_file)
 
+        # Now fix all the metadata files and update the sha256 hash + cache
         for wheel_file_obj in new_wheel_file_objects:
             file_name_as_posix = wheel_file_obj.filename
             metadata_path = file_name_as_posix_to_metadata_path[file_name_as_posix]
+
             if repair_metadata_file(metadata_path, canonical_name_to_metadata_name):
                 wheel_file_obj.metadata_hash = get_sha256_hash(metadata_path)
+                cache[file_name_as_posix] = asdict(wheel_file_obj)
 
+        # Remove any old wheel files from the cache
         removed_wheels = set(cache.keys()) - all_wheel_files
         for old_wheel_file in removed_wheels:
             del cache[old_wheel_file]
 
         index_content = str(generate_index(projects.keys()))
         write_utf8_file(temp_dir_path.joinpath("index.html"), index_content)
         project_base_url = URL("../")
```

### Comparing `index_503-0.1.3/src/index_503/page_generator.py` & `index_503-0.1.4/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.3/src/index_503/util.py` & `index_503-0.1.4/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.3/src/index_503/wheel_file.py` & `index_503-0.1.4/src/index_503/wheel_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from html import escape
 from typing import Optional, Union
 
 from airium import Airium
 from typing_extensions import Literal
 from yarl import URL
 
-WHEEL_FILE_VERSION = 2
+WHEEL_FILE_VERSION = 7
 
 
 @dataclass
 class WheelFile:
     """
     Represents a wheel file in the repository.
     """
@@ -86,16 +86,14 @@
         base_url = URL(base_url)
 
         href = f"{base_url / self.filename}#sha256={self.wheel_hash}"
         kwargs = {"href": href}
 
         if self.requires_python is not None:
             kwargs["data-requires-python"] = escape(self.requires_python)
-
         if self.metadata_hash is True:
             kwargs["data-dist-info-metadata"] = "true"
         elif self.metadata_hash is not None:
-            hash_string = f"sha256={self.metadata_hash}"
-            kwargs["data-dist-info-metadata"] = hash_string
+            kwargs["data-dist-info-metadata"] = f"sha256={self.metadata_hash}"
 
         with page.a(**kwargs):
             page(posixpath.basename(self.filename))
```

### Comparing `index_503-0.1.3/PKG-INFO` & `index_503-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.1.3
+Version: 0.1.4
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
-Metadata-Version: 2.1 Name: index-503 Version: 0.1.3 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.1.4 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

