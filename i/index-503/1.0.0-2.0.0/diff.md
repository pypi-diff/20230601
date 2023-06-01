# Comparing `tmp/index_503-1.0.0.tar.gz` & `tmp/index_503-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-1.0.0.tar", max compression
+gzip compressed data, was "index_503-2.0.0.tar", max compression
```

## Comparing `index_503-1.0.0.tar` & `index_503-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-06-01 18:17:36.318697 index_503-1.0.0/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-01 18:17:36.318697 index_503-1.0.0/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 18:17:37.058697 index_503-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 18:17:37.018697 index_503-1.0.0/src/index_503/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/cache.py
--rw-r--r--   0        0        0     1336 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/file.py
--rw-r--r--   0        0        0     6867 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/py.typed
--rw-r--r--   0        0        0     1513 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/util.py
--rw-r--r--   0        0        0     5246 2023-06-01 18:17:36.318697 index_503-1.0.0/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 index_503-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 19:15:54.291295 index_503-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-01 19:15:54.291295 index_503-2.0.0/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 19:15:55.211337 index_503-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 19:15:55.163335 index_503-2.0.0/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/cache.py
+-rw-r--r--   0        0        0     1336 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/file.py
+-rw-r--r--   0        0        0     6952 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/py.typed
+-rw-r--r--   0        0        0     1513 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/util.py
+-rw-r--r--   0        0        0     5246 2023-06-01 19:15:54.295295 index_503-2.0.0/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4742 1970-01-01 00:00:00.000000 index_503-2.0.0/PKG-INFO
```

### Comparing `index_503-1.0.0/LICENSE` & `index_503-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-1.0.0/README.md` & `index_503-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `index_503-1.0.0/pyproject.toml` & `index_503-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "1.0.0"
+version = "2.0.0"
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
-python = "^3.8"
+python = "^3.9"
 click = "^8.1.3"
 airium = "^0.2.5"
 yarl = "^1.9.2"
 natsort = "^8.3.1"
 dist-meta = "^0.8.0"
 consolekit = "^1.4.1"
```

### Comparing `index_503-1.0.0/src/index_503/cache.py` & `index_503-2.0.0/src/index_503/cache.py`

 * *Files identical despite different names*

### Comparing `index_503-1.0.0/src/index_503/file.py` & `index_503-2.0.0/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-1.0.0/src/index_503/index.py` & `index_503-2.0.0/src/index_503/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import logging
 import os
-import tempfile
 from collections import defaultdict
 from operator import attrgetter
 from pathlib import Path
 from shutil import copyfile, rmtree
+from tempfile import mkdtemp
 from typing import Dict, List, Set
 
 from natsort import natsorted
 from yarl import URL
 
 from .cache import IndexCache
 from .file import write_utf8_file
@@ -50,29 +50,31 @@
         self.target_path = target_path
         self.cache = IndexCache(target_path)
 
     def make_index(self) -> Path:
         """Generate a simple repository of Python wheels."""
         target_path = self.target_path
         old_index = target_path.readlink() if target_path.exists() else None
-
-        with tempfile.TemporaryDirectory(
-            dir=str(self.target_path.parent), ignore_cleanup_errors=True
-        ) as temp_dir:
+        temp_dir = mkdtemp(None, None, str(self.target_path.parent))
+        try:
             self.cache.load()
             temp_dir_path = Path(temp_dir)
 
             self._make_index_at_temp_dir(temp_dir_path)
             self._atomic_replace_old_index(temp_dir_path, target_path)
 
             if old_index:
                 _LOGGER.debug("Removing old index %s", old_index)
                 rmtree(old_index)
 
             return self.target_path
+        except Exception:
+            _LOGGER.exception("Error generating index")
+            rmtree(temp_dir)
+            raise
 
     def _atomic_replace_old_index(self, temp_dir_path: Path, target_path: Path) -> None:
         """Atomically replace the old index with the new one."""
         final_name = target_path.parent / (target_path.name + "-" + temp_dir_path.name)
         final_build_name = final_name.parent / (final_name.name + "-build")
 
         _LOGGER.debug("Renaming %s with %s", temp_dir_path, final_name)
```

### Comparing `index_503-1.0.0/src/index_503/metadata.py` & `index_503-2.0.0/src/index_503/metadata.py`

 * *Files identical despite different names*

### Comparing `index_503-1.0.0/src/index_503/page_generator.py` & `index_503-2.0.0/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-1.0.0/src/index_503/util.py` & `index_503-2.0.0/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-1.0.0/src/index_503/wheel_file.py` & `index_503-2.0.0/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-1.0.0/PKG-INFO` & `index_503-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 1.0.0
+Version: 2.0.0
 Summary: PEP 503 index builder
 Home-page: https://github.com/bdraco/index-503
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: airium (>=0.2.5,<0.3.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: consolekit (>=1.4.1,<2.0.0)
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: index-503 Version: 1.0.0 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 2.0.0 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
-Nick Koston Author-email: nick@koston.org Requires-Python: >=3.8,<4.0
+Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
-Libraries Requires-Dist: airium (>=0.2.5,<0.3.0) Requires-Dist: click
-(>=8.1.3,<9.0.0) Requires-Dist: consolekit (>=1.4.1,<2.0.0) Requires-Dist:
-dist-meta (>=0.8.0,<0.9.0) Requires-Dist: natsort (>=8.3.1,<9.0.0) Requires-
-Dist: yarl (>=1.9.2,<2.0.0) Project-URL: Bug Tracker, https://github.com/
-bdraco/index-503/issues Project-URL: Changelog, https://github.com/bdraco/
-index-503/blob/main/CHANGELOG.md Project-URL: Documentation, https://index-
-503.readthedocs.io Project-URL: Repository, https://github.com/bdraco/index-503
-Description-Content-Type: text/markdown # Index 503
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development :: Libraries Requires-Dist: airium (>=0.2.5,<0.3.0)
+Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: consolekit
+(>=1.4.1,<2.0.0) Requires-Dist: dist-meta (>=0.8.0,<0.9.0) Requires-Dist:
+natsort (>=8.3.1,<9.0.0) Requires-Dist: yarl (>=1.9.2,<2.0.0) Project-URL: Bug
+Tracker, https://github.com/bdraco/index-503/issues Project-URL: Changelog,
+https://github.com/bdraco/index-503/blob/main/CHANGELOG.md Project-URL:
+Documentation, https://index-503.readthedocs.io Project-URL: Repository, https:
+//github.com/bdraco/index-503 Description-Content-Type: text/markdown # Index
+503
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 PEP 503 index builder ## Usage If you have a directory full of wheels like
 `musllinux`: `index-503 musllinux` This will produce a `musllinux-index`
 directory with a PEP 503 index symlinked to the original directory without
 disturbing the original directory. Running this again will replace the original
```

