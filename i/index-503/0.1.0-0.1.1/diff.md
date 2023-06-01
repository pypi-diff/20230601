# Comparing `tmp/index_503-0.1.0.tar.gz` & `tmp/index_503-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.1.0.tar", max compression
+gzip compressed data, was "index_503-0.1.1.tar", max compression
```

## Comparing `index_503-0.1.0.tar` & `index_503-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-05-31 20:36:35.113400 index_503-0.1.0/LICENSE
--rw-r--r--   0        0        0     3481 2023-05-31 20:36:35.113400 index_503-0.1.0/README.md
--rw-r--r--   0        0        0     2299 2023-05-31 20:36:35.889403 index_503-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-31 20:36:35.849403 index_503-0.1.0/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/file.py
--rw-r--r--   0        0        0     5034 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/index.py
--rw-r--r--   0        0        0      475 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/main.py
--rw-r--r--   0        0        0     2588 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/py.typed
--rw-r--r--   0        0        0      522 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/util.py
--rw-r--r--   0        0        0     3224 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 01:51:53.492920 index_503-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3481 2023-06-01 01:51:53.492920 index_503-0.1.1/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 01:51:54.256930 index_503-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 01:51:54.212930 index_503-0.1.1/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/file.py
+-rw-r--r--   0        0        0     6904 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/index.py
+-rw-r--r--   0        0        0      475 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/main.py
+-rw-r--r--   0        0        0     2384 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/py.typed
+-rw-r--r--   0        0        0      761 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/util.py
+-rw-r--r--   0        0        0     3437 2023-06-01 01:51:53.492920 index_503-0.1.1/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.1/PKG-INFO
```

### Comparing `index_503-0.1.0/LICENSE` & `index_503-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.1.0/README.md` & `index_503-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.1.0/pyproject.toml` & `index_503-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.1.0"
+version = "0.1.1"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.1.0/src/index_503/file.py` & `index_503-0.1.1/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.0/src/index_503/page_generator.py` & `index_503-0.1.1/src/index_503/page_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import re
 from typing import Iterable, Union
 
 from airium import Airium
 from natsort import natsorted
 from yarl import URL
 
+from .util import canonicalize_name
 from .wheel_file import WheelFile
 
 
 # modified from https://github.com/repo-helper/simple503/blob/master/simple503/__init__.py
 def generate_index(projects: Iterable[str]) -> Airium:
     """
     Generate the simple repository index page, containing a list of all projects.
@@ -68,23 +68,14 @@
             for wheel_file in files:
                 wheel_file.as_anchor(page, base_url)
                 page.br()
 
     return page
 
 
-_canonicalize_regex = re.compile(r"[-_.]+")
-# PEP 427: The build number must start with a digit.
-
-
-def canonicalize_name(name: str) -> str:
-    # This is taken from PEP 503.
-    return _canonicalize_regex.sub("-", name).lower()
-
-
 def get_meta_tags(page: Airium) -> None:
     from . import __version__
 
     # Not part of the spec, but allowed
     page.meta(name="generator", content=f"index503 version {__version__}")
     page.meta(name="pypi:repository-version", content="1.0")
     page.meta(charset="UTF-8")
```

### Comparing `index_503-0.1.0/src/index_503/util.py` & `index_503-0.1.1/src/index_503/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 import json
+import re
 from hashlib import sha256
 from pathlib import Path
 from typing import Any, Dict
 
+_canonicalize_regex = re.compile(r"[-_.]+")
+# PEP 427: The build number must start with a digit.
+
+
+def canonicalize_name(name: str) -> str:
+    # This is taken from PEP 503.
+    return _canonicalize_regex.sub("-", name).lower()
+
 
 def get_sha256_hash(filename: Path) -> str:
     """Get SHA256 hash of a file."""
     with filename.open("rb") as f:
         bytes = f.read()  # read entire file as bytes
         return sha256(bytes).hexdigest()
```

### Comparing `index_503-0.1.0/src/index_503/wheel_file.py` & `index_503-0.1.1/src/index_503/wheel_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,26 +25,35 @@
 from html import escape
 from typing import Optional, Union
 
 from airium import Airium
 from typing_extensions import Literal
 from yarl import URL
 
+WHEEL_FILE_VERSION = 1
+
 
 @dataclass
 class WheelFile:
     """
     Represents a wheel file in the repository.
     """
 
-    #: The name of the wheel file.
-    name: str
+    # The version of the wheel file format.
+    version: int
+
+    # The canonicalized name of the project.
+    canonical_name: str
 
+    # The filename of the wheel file.
     filename: str
 
+    # The Name field from the METADATA file.
+    metadata_name: str
+
     wheel_hash: str  # sha256
     """
     The hash of the wheel file.
 
     Repositories SHOULD choose a hash function from one of the ones guaranteed
     to be available via the hashlib module in the Python standard library
     (currently ``md5``, ``sha1``, ``sha224``, ``sha256``, ``sha384``, ``sha512``).
```

### Comparing `index_503-0.1.0/PKG-INFO` & `index_503-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.1.0
+Version: 0.1.1
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
-Metadata-Version: 2.1 Name: index-503 Version: 0.1.0 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.1.1 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

