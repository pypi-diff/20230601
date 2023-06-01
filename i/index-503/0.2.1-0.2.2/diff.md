# Comparing `tmp/index_503-0.2.1.tar.gz` & `tmp/index_503-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.2.1.tar", max compression
+gzip compressed data, was "index_503-0.2.2.tar", max compression
```

## Comparing `index_503-0.2.1.tar` & `index_503-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-06-01 13:42:00.012419 index_503-0.2.1/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-01 13:42:00.012419 index_503-0.2.1/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 13:42:00.824430 index_503-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 13:42:00.780429 index_503-0.2.1/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-01 13:42:00.016419 index_503-0.2.1/src/index_503/file.py
--rw-r--r--   0        0        0     7997 2023-06-01 13:42:00.016419 index_503-0.2.1/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-01 13:42:00.016419 index_503-0.2.1/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-01 13:42:00.016419 index_503-0.2.1/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-01 13:42:00.016419 index_503-0.2.1/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 13:42:00.016419 index_503-0.2.1/src/index_503/py.typed
--rw-r--r--   0        0        0     1513 2023-06-01 13:42:00.016419 index_503-0.2.1/src/index_503/util.py
--rw-r--r--   0        0        0     4585 2023-06-01 13:42:00.016419 index_503-0.2.1/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 index_503-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 13:44:41.422170 index_503-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-01 13:44:41.422170 index_503-0.2.2/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 13:44:42.190170 index_503-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 13:44:42.150170 index_503-0.2.2/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/cache.py
+-rw-r--r--   0        0        0     1336 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/file.py
+-rw-r--r--   0        0        0     7067 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/py.typed
+-rw-r--r--   0        0        0     1513 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/util.py
+-rw-r--r--   0        0        0     4585 2023-06-01 13:44:41.426170 index_503-0.2.2/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 index_503-0.2.2/PKG-INFO
```

### Comparing `index_503-0.2.1/LICENSE` & `index_503-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.2.1/README.md` & `index_503-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.2.1/pyproject.toml` & `index_503-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.2.1"
+version = "0.2.2"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.2.1/src/index_503/file.py` & `index_503-0.2.2/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.1/src/index_503/index.py` & `index_503-0.2.2/src/index_503/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import glob
-import json
 import logging
 import os
 import tempfile
 from collections import defaultdict
 from dataclasses import asdict
 from operator import attrgetter
 from pathlib import Path
 from shutil import copyfile, rmtree
-from typing import Any, Dict, List, Set
+from typing import Dict, List, Set
 
 from natsort import natsorted
 from yarl import URL
 
+from .cache import IndexCache
 from .file import write_utf8_file
 from .metadata import repair_metadata_file
 from .page_generator import generate_index, generate_project_page
-from .util import canonicalize_name, exclusive_lock, get_sha256_hash, load_json_file
+from .util import canonicalize_name, exclusive_lock, get_sha256_hash
 from .wheel_file import WHEEL_FILE_VERSION, WheelFile
 
 _LOGGER = logging.getLogger(__name__)
 
 CACHE_FILE = "cache.json"
 
 
@@ -38,38 +38,14 @@
     This will generate
     musllinux-index
     """
     with exclusive_lock(origin_path):
         return IndexMaker(origin_path).make_index()
 
 
-class IndexCache:
-    def __init__(self, target_path: Path) -> None:
-        """Cache of WheelFiles between runs."""
-        cache_file = target_path.joinpath(CACHE_FILE)
-        self.cache_file = cache_file
-        self.cache: Dict[str, Dict[str, Any]] = {}
-
-    def load(self) -> None:
-        """Load the cache from a file."""
-        if self.cache_file.exists():
-            self.cache = load_json_file(self.cache_file)
-
-    def write_to_new(self, target: Path) -> None:
-        """Write the cache to a new file."""
-        new_cache_file = target.joinpath(CACHE_FILE)
-        write_utf8_file(new_cache_file, json.dumps(self.cache))
-
-    def remove_stale_keys(self, all_wheel_files: Set[str]) -> None:
-        """Remove any wheel file names that no longer exist."""
-        removed_wheels = set(self.cache.keys()) - all_wheel_files
-        for old_wheel_file in removed_wheels:
-            del self.cache[old_wheel_file]
-
-
 class IndexMaker:
     """Generate a simple repository of Python wheels."""
 
     def __init__(self, origin_path: Path) -> None:
         """Generate a simple repository of Python wheels."""
         self.origin_path = origin_path
         self.origin_name = origin_path.name
```

### Comparing `index_503-0.2.1/src/index_503/metadata.py` & `index_503-0.2.2/src/index_503/metadata.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.1/src/index_503/page_generator.py` & `index_503-0.2.2/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.1/src/index_503/util.py` & `index_503-0.2.2/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.1/src/index_503/wheel_file.py` & `index_503-0.2.2/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.2.1/PKG-INFO` & `index_503-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.2.1
+Version: 0.2.2
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
-Metadata-Version: 2.1 Name: index-503 Version: 0.2.1 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.2.2 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

