# Comparing `tmp/index_503-0.2.2.tar.gz` & `tmp/index_503-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.2.2.tar", max compression
+gzip compressed data, was "index_503-1.0.0.tar", max compression
```

## Comparing `index_503-0.2.2.tar` & `index_503-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-06-01 13:44:41.422170 index_503-0.2.2/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-01 13:44:41.422170 index_503-0.2.2/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 13:44:42.190170 index_503-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 13:44:42.150170 index_503-0.2.2/src/index_503/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/cache.py
--rw-r--r--   0        0        0     1336 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/file.py
--rw-r--r--   0        0        0     7067 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/py.typed
--rw-r--r--   0        0        0     1513 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/util.py
--rw-r--r--   0        0        0     4585 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 index_503-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 18:17:36.318697 index_503-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-01 18:17:36.318697 index_503-1.0.0/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 18:17:37.058697 index_503-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 18:17:37.018697 index_503-1.0.0/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/cache.py
+-rw-r--r--   0        0        0     1336 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/file.py
+-rw-r--r--   0        0        0     6867 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/py.typed
+-rw-r--r--   0        0        0     1513 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/util.py
+-rw-r--r--   0        0        0     5246 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 index_503-1.0.0/PKG-INFO
```

### Comparing `index_503-0.2.2/LICENSE` & `index_503-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.2.2/README.md` & `index_503-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.2.2/pyproject.toml` & `index_503-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.2.2"
+version = "1.0.0"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
@@ -19,15 +19,15 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/bdraco/index-503/issues"
 "Changelog" = "https://github.com/bdraco/index-503/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 click = "^8.1.3"
 airium = "^0.2.5"
 yarl = "^1.9.2"
 natsort = "^8.3.1"
 dist-meta = "^0.8.0"
 consolekit = "^1.4.1"
```

### Comparing `index_503-0.2.2/src/index_503/cache.py` & `index_503-1.0.0/src/index_503/cache.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.2/src/index_503/file.py` & `index_503-1.0.0/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.2/src/index_503/index.py` & `index_503-1.0.0/src/index_503/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import glob
 import logging
 import os
 import tempfile
 from collections import defaultdict
-from dataclasses import asdict
 from operator import attrgetter
 from pathlib import Path
 from shutil import copyfile, rmtree
 from typing import Dict, List, Set
 
 from natsort import natsorted
 from yarl import URL
 
 from .cache import IndexCache
 from .file import write_utf8_file
 from .metadata import repair_metadata_file
 from .page_generator import generate_index, generate_project_page
-from .util import canonicalize_name, exclusive_lock, get_sha256_hash
-from .wheel_file import WHEEL_FILE_VERSION, WheelFile
+from .util import canonicalize_name, exclusive_lock
+from .wheel_file import WheelFile
 
 _LOGGER = logging.getLogger(__name__)
 
-CACHE_FILE = "cache.json"
-
 
 def make_index(origin_path: Path) -> Path:
     """Generate a simple repository of Python wheels.
 
     This function will take a directory of wheels at the top level
     of a webserver and generate a simple repository of wheels.
 
@@ -93,35 +90,34 @@
     def _make_index_at_temp_dir(self, temp_dir_path: Path) -> None:
         """Generate a simple repository of Python wheels in a temp dir."""
         new_wheel_file_objects: List[WheelFile] = []
         projects: Dict[str, List[WheelFile]] = defaultdict(list)
         wheel_file_name_to_metadata_path: Dict[str, Path] = {}
         all_wheel_files: Set[str] = set()
         canonical_name_to_metadata_name: Dict[str, str] = {}
+        raw_cache = self.cache.cache
 
         for wheel_file in glob.glob(str(self.origin_path.joinpath("*.whl"))):
             wheel_path = Path(wheel_file)
             wheel_file_name = wheel_path.name
             all_wheel_files.add(wheel_file_name)
             target_file = temp_dir_path.joinpath(wheel_file_name)
             metadata_path = target_file.with_suffix(f"{target_file.suffix}.metadata")
             wheel_file_symlink_target = f"../{self.origin_name}/{wheel_file_name}"
-            wheel_cache = self.cache.cache.get(wheel_file_name)
 
-            if wheel_cache and wheel_cache["version"] == WHEEL_FILE_VERSION:
-                wheel_file_obj = WheelFile(**wheel_cache)
+            if (wheel_cache := raw_cache.get(wheel_file_name)) and (
+                wheel_file_obj := WheelFile.from_cache(wheel_cache)
+            ):
                 copyfile(self.target_path.joinpath(metadata_path.name), metadata_path)
-            else:
-                maybe_wheel_file_obj = WheelFile.from_wheel(wheel_path, metadata_path)
-                if not maybe_wheel_file_obj:
-                    continue
-                wheel_file_obj = maybe_wheel_file_obj
+            elif wheel_file_obj := WheelFile.from_wheel(wheel_path, metadata_path):
                 wheel_file_name_to_metadata_path[wheel_file_name] = metadata_path
                 new_wheel_file_objects.append(wheel_file_obj)
-                self.cache.cache[wheel_file_name] = asdict(wheel_file_obj)
+                raw_cache[wheel_file_name] = wheel_file_obj.as_dict()
+            else:
+                continue
 
             canonical_name = wheel_file_obj.canonical_name
             metadata_name = wheel_file_obj.metadata_name
             projects[metadata_name].append(wheel_file_obj)
             canonical_name_to_metadata_name[canonical_name] = metadata_name
             os.symlink(wheel_file_symlink_target, target_file)
 
@@ -138,21 +134,22 @@
         self,
         new_wheel_file_objects: List[WheelFile],
         wheel_file_name_to_metadata_path: Dict[str, Path],
         canonical_name_to_metadata_name: Dict[str, str],
     ) -> None:
         """Repair the metadata files."""
         # Now fix all the metadata files and update the sha256 hash + cache
+        raw_cache = self.cache.cache
         for wheel_file_obj in new_wheel_file_objects:
             wheel_file_name = wheel_file_obj.filename
             metadata_path = wheel_file_name_to_metadata_path[wheel_file_name]
 
             if repair_metadata_file(metadata_path, canonical_name_to_metadata_name):
-                wheel_file_obj.metadata_hash = get_sha256_hash(metadata_path)
-                self.cache.cache[wheel_file_name] = asdict(wheel_file_obj)
+                wheel_file_obj.update_metadata(metadata_path)
+                raw_cache[wheel_file_name] = wheel_file_obj.as_dict()
 
     def generate_index_pages(
         self, temp_dir_path: Path, projects: Dict[str, List[WheelFile]]
     ) -> None:
         """Generate the index pages."""
         index_content = str(generate_index(projects.keys()))
         write_utf8_file(temp_dir_path.joinpath("index.html"), index_content)
```

### Comparing `index_503-0.2.2/src/index_503/metadata.py` & `index_503-1.0.0/src/index_503/metadata.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.2/src/index_503/page_generator.py` & `index_503-1.0.0/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.2/src/index_503/util.py` & `index_503-1.0.0/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.2/src/index_503/wheel_file.py` & `index_503-1.0.0/src/index_503/wheel_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 #  MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 import posixpath
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from html import escape
 from pathlib import Path
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from airium import Airium
 from dist_meta import metadata
 from typing_extensions import Literal
 from yarl import URL
 
 from .metadata import extract_metadata_from_wheel_file
@@ -99,14 +99,34 @@
             kwargs["data-dist-info-metadata"] = "true"
         elif self.metadata_hash is not None:
             kwargs["data-dist-info-metadata"] = f"{HASH_FORMAT}={self.metadata_hash}"
 
         with page.a(**kwargs):
             page(posixpath.basename(self.filename))
 
+    def update_metadata(self, metadata_path: Path) -> None:
+        """
+        Update the metadata hash of this wheel file.
+
+        :param metadata_path:
+        """
+
+        self.metadata_hash = get_sha256_hash(metadata_path)
+
+    def as_dict(self) -> Dict[str, Any]:
+        """Return a dictionary representation of this wheel file."""
+        return asdict(self)
+
+    @classmethod
+    def from_cache(cls, cache_data: Dict[str, Any]) -> Optional["WheelFile"]:
+        """Create a :class:`~.WheelFile` from a cache entry."""
+        if cache_data["version"] != WHEEL_FILE_VERSION:
+            return None
+        return cls(**cache_data)
+
     @classmethod
     def from_wheel(
         cls,
         wheel_path: Path,
         metadata_path: Path,
     ) -> Optional["WheelFile"]:
         """Create a :class:`~.WheelFile` from a wheel file and its metadata file."""
```

### Comparing `index_503-0.2.2/PKG-INFO` & `index_503-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.2.2
+Version: 1.0.0
 Summary: PEP 503 index builder
 Home-page: https://github.com/bdraco/index-503
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: airium (>=0.2.5,<0.3.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: index-503 Version: 0.2.2 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 1.0.0 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
-Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
+Nick Koston Author-email: nick@koston.org Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries Requires-Dist: airium
-(>=0.2.5,<0.3.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist:
-consolekit (>=1.4.1,<2.0.0) Requires-Dist: dist-meta (>=0.8.0,<0.9.0) Requires-
-Dist: natsort (>=8.3.1,<9.0.0) Requires-Dist: yarl (>=1.9.2,<2.0.0) Project-
-URL: Bug Tracker, https://github.com/bdraco/index-503/issues Project-URL:
-Changelog, https://github.com/bdraco/index-503/blob/main/CHANGELOG.md Project-
-URL: Documentation, https://index-503.readthedocs.io Project-URL: Repository,
-https://github.com/bdraco/index-503 Description-Content-Type: text/markdown #
-Index 503
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
+Libraries Requires-Dist: airium (>=0.2.5,<0.3.0) Requires-Dist: click
+(>=8.1.3,<9.0.0) Requires-Dist: consolekit (>=1.4.1,<2.0.0) Requires-Dist:
+dist-meta (>=0.8.0,<0.9.0) Requires-Dist: natsort (>=8.3.1,<9.0.0) Requires-
+Dist: yarl (>=1.9.2,<2.0.0) Project-URL: Bug Tracker, https://github.com/
+bdraco/index-503/issues Project-URL: Changelog, https://github.com/bdraco/
+index-503/blob/main/CHANGELOG.md Project-URL: Documentation, https://index-
+503.readthedocs.io Project-URL: Repository, https://github.com/bdraco/index-503
+Description-Content-Type: text/markdown # Index 503
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 PEP 503 index builder ## Usage If you have a directory full of wheels like
 `musllinux`: `index-503 musllinux` This will produce a `musllinux-index`
 directory with a PEP 503 index symlinked to the original directory without
 disturbing the original directory. Running this again will replace the original
```

