# Comparing `tmp/index_503-0.1.8.tar.gz` & `tmp/index_503-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.1.8.tar", max compression
+gzip compressed data, was "index_503-0.2.0.tar", max compression
```

## Comparing `index_503-0.1.8.tar` & `index_503-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-06-01 13:16:32.567199 index_503-0.1.8/LICENSE
--rw-r--r--   0        0        0     3481 2023-06-01 13:16:32.567199 index_503-0.1.8/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 13:16:33.315205 index_503-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 13:16:33.275205 index_503-0.1.8/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/file.py
--rw-r--r--   0        0        0     7539 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/py.typed
--rw-r--r--   0        0        0      792 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/util.py
--rw-r--r--   0        0        0     4585 2023-06-01 13:16:32.567199 index_503-0.1.8/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 13:31:30.061381 index_503-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-01 13:31:30.061381 index_503-0.2.0/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 13:31:30.977381 index_503-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 13:31:30.929381 index_503-0.2.0/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-01 13:31:30.065381 index_503-0.2.0/src/index_503/file.py
+-rw-r--r--   0        0        0     7597 2023-06-01 13:31:30.065381 index_503-0.2.0/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-01 13:31:30.065381 index_503-0.2.0/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-01 13:31:30.065381 index_503-0.2.0/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-01 13:31:30.065381 index_503-0.2.0/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:31:30.065381 index_503-0.2.0/src/index_503/py.typed
+-rw-r--r--   0        0        0     1512 2023-06-01 13:31:30.065381 index_503-0.2.0/src/index_503/util.py
+-rw-r--r--   0        0        0     4585 2023-06-01 13:31:30.065381 index_503-0.2.0/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 index_503-0.2.0/PKG-INFO
```

### Comparing `index_503-0.1.8/LICENSE` & `index_503-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.1.8/README.md` & `index_503-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 `index-503 musllinux`
 
 This will produce a `musllinux-index` directory with a PEP 503 index symlinked to the original directory without disturbing the original directory.
 
 Running this again will replace the original index and delete the old index in an atomic manner.
 
-The caller is responsible for ensuring that there are no simultaneous executions.
+A lock will be held in the parent directory to prevent concurrent executions.
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install index-503`
```

#### html2text {}

```diff
@@ -2,14 +2,14 @@
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 PEP 503 index builder ## Usage If you have a directory full of wheels like
 `musllinux`: `index-503 musllinux` This will produce a `musllinux-index`
 directory with a PEP 503 index symlinked to the original directory without
 disturbing the original directory. Running this again will replace the original
-index and delete the old index in an atomic manner. The caller is responsible
-for ensuring that there are no simultaneous executions. ## Installation Install
-this via pip (or your favourite package manager): `pip install index-503` ##
-Credits This package was created with [Copier](https://copier.readthedocs.io/
-) and the [browniebroke/pypackage-template](https://github.com/browniebroke/
-pypackage-template) project template. This project borrows heavily from Dominic
-Davis-Foster's simple503 https://github.com/repo-helper/simple503
+index and delete the old index in an atomic manner. A lock will be held in the
+parent directory to prevent concurrent executions. ## Installation Install this
+via pip (or your favourite package manager): `pip install index-503` ## Credits
+This package was created with [Copier](https://copier.readthedocs.io/) and the
+[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
+template) project template. This project borrows heavily from Dominic Davis-
+Foster's simple503 https://github.com/repo-helper/simple503
```

### Comparing `index_503-0.1.8/pyproject.toml` & `index_503-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.1.8"
+version = "0.2.0"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.1.8/src/index_503/file.py` & `index_503-0.2.0/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.8/src/index_503/index.py` & `index_503-0.2.0/src/index_503/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from natsort import natsorted
 from yarl import URL
 
 from .file import write_utf8_file
 from .metadata import repair_metadata_file
 from .page_generator import generate_index, generate_project_page
-from .util import canonicalize_name, get_sha256_hash, load_json_file
+from .util import canonicalize_name, exclusive_lock, get_sha256_hash, load_json_file
 from .wheel_file import WHEEL_FILE_VERSION, WheelFile
 
 _LOGGER = logging.getLogger(__name__)
 
 CACHE_FILE = "cache.json"
 
 
@@ -34,15 +34,16 @@
 
     Example
     musllinux
 
     This will generate
     musllinux-index
     """
-    return IndexMaker(origin_path).make_index()
+    with exclusive_lock(origin_path):
+        return IndexMaker(origin_path).make_index()
 
 
 class IndexCache:
     def __init__(self, target_path: Path) -> None:
         """Cache of WheelFiles between runs."""
         cache_file = target_path.joinpath(CACHE_FILE)
         self.cache_file = cache_file
```

### Comparing `index_503-0.1.8/src/index_503/metadata.py` & `index_503-0.2.0/src/index_503/metadata.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.8/src/index_503/page_generator.py` & `index_503-0.2.0/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.8/src/index_503/wheel_file.py` & `index_503-0.2.0/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.8/PKG-INFO` & `index_503-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.1.8
+Version: 0.2.0
 Summary: PEP 503 index builder
 Home-page: https://github.com/bdraco/index-503
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -71,15 +71,15 @@
 
 `index-503 musllinux`
 
 This will produce a `musllinux-index` directory with a PEP 503 index symlinked to the original directory without disturbing the original directory.
 
 Running this again will replace the original index and delete the old index in an atomic manner.
 
-The caller is responsible for ensuring that there are no simultaneous executions.
+A lock will be held in the parent directory to prevent concurrent executions.
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install index-503`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: index-503 Version: 0.1.8 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.2.0 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -20,14 +20,14 @@
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 PEP 503 index builder ## Usage If you have a directory full of wheels like
 `musllinux`: `index-503 musllinux` This will produce a `musllinux-index`
 directory with a PEP 503 index symlinked to the original directory without
 disturbing the original directory. Running this again will replace the original
-index and delete the old index in an atomic manner. The caller is responsible
-for ensuring that there are no simultaneous executions. ## Installation Install
-this via pip (or your favourite package manager): `pip install index-503` ##
-Credits This package was created with [Copier](https://copier.readthedocs.io/
-) and the [browniebroke/pypackage-template](https://github.com/browniebroke/
-pypackage-template) project template. This project borrows heavily from Dominic
-Davis-Foster's simple503 https://github.com/repo-helper/simple503
+index and delete the old index in an atomic manner. A lock will be held in the
+parent directory to prevent concurrent executions. ## Installation Install this
+via pip (or your favourite package manager): `pip install index-503` ## Credits
+This package was created with [Copier](https://copier.readthedocs.io/) and the
+[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
+template) project template. This project borrows heavily from Dominic Davis-
+Foster's simple503 https://github.com/repo-helper/simple503
```

