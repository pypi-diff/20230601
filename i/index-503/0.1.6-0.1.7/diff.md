# Comparing `tmp/index_503-0.1.6.tar.gz` & `tmp/index_503-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.1.6.tar", max compression
+gzip compressed data, was "index_503-0.1.7.tar", max compression
```

## Comparing `index_503-0.1.6.tar` & `index_503-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-06-01 03:16:49.437121 index_503-0.1.6/LICENSE
--rw-r--r--   0        0        0     3481 2023-06-01 03:16:49.437121 index_503-0.1.6/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 03:16:50.385128 index_503-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 03:16:50.337128 index_503-0.1.6/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/file.py
--rw-r--r--   0        0        0     7996 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/index.py
--rw-r--r--   0        0        0      475 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/main.py
--rw-r--r--   0        0        0     2384 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/py.typed
--rw-r--r--   0        0        0      761 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/util.py
--rw-r--r--   0        0        0     3398 2023-06-01 03:16:49.437121 index_503-0.1.6/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 13:08:55.567221 index_503-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3481 2023-06-01 13:08:55.567221 index_503-0.1.7/README.md
+-rw-r--r--   0        0        0     2299 2023-06-01 13:08:56.363241 index_503-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-01 13:08:56.319240 index_503-0.1.7/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/file.py
+-rw-r--r--   0        0        0     7496 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/py.typed
+-rw-r--r--   0        0        0      792 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/util.py
+-rw-r--r--   0        0        0     4585 2023-06-01 13:08:55.567221 index_503-0.1.7/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.7/PKG-INFO
```

### Comparing `index_503-0.1.6/LICENSE` & `index_503-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.1.6/README.md` & `index_503-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `index_503-0.1.6/pyproject.toml` & `index_503-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.1.6"
+version = "0.1.7"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.1.6/src/index_503/file.py` & `index_503-0.1.7/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.6/src/index_503/page_generator.py` & `index_503-0.1.7/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.1.6/src/index_503/util.py` & `index_503-0.1.7/src/index_503/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, Dict
 
 _canonicalize_regex = re.compile(r"[-_.]+")
 # PEP 427: The build number must start with a digit.
 
 
 def canonicalize_name(name: str) -> str:
+    """Canonicalize a name."""
     # This is taken from PEP 503.
     return _canonicalize_regex.sub("-", name).lower()
 
 
 def get_sha256_hash(filename: Path) -> str:
     """Get SHA256 hash of a file."""
     with filename.open("rb") as f:
```

### Comparing `index_503-0.1.6/src/index_503/wheel_file.py` & `index_503-0.1.7/src/index_503/wheel_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,42 +19,47 @@
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 import posixpath
 from dataclasses import dataclass
 from html import escape
+from pathlib import Path
 from typing import Optional, Union
 
 from airium import Airium
+from dist_meta import metadata
 from typing_extensions import Literal
 from yarl import URL
 
+from .metadata import extract_metadata_from_wheel_file
+from .util import canonicalize_name, get_sha256_hash
+
 WHEEL_FILE_VERSION = 9
 
+HASH_FORMAT = "sha256"
+
 
 @dataclass
 class WheelFile:
-    """
-    Represents a wheel file in the repository.
-    """
+    """Represents a wheel file in the repository."""
 
-    # The version of the wheel file format.
     version: int
+    """The version of the wheel file format."""
 
-    # The canonicalized name of the project.
     canonical_name: str
+    """The canonicalized name of the project."""
 
-    # The filename of the wheel file.
     filename: str
+    """The filename of the wheel file."""
 
-    # The Name field from the METADATA file.
     metadata_name: str
+    """The Name field from the METADATA file."""
 
-    wheel_hash: str  # sha256
+    wheel_hash: str  # HASH_FORMAT
     """
     The hash of the wheel file.
 
     Repositories SHOULD choose a hash function from one of the ones guaranteed
     to be available via the hashlib module in the Python standard library
     (currently ``md5``, ``sha1``, ``sha224``, ``sha256``, ``sha384``, ``sha512``).
     The current recommendation is to use ``sha256``.
@@ -81,19 +86,44 @@
 
         :param page:
         :param base_url: The base URL of the Python package repository.
         """
 
         base_url = URL(base_url)
 
-        href = f"{base_url / self.filename}#sha256={self.wheel_hash}"
+        href = f"{base_url / self.filename}#{HASH_FORMAT}={self.wheel_hash}"
         kwargs = {"href": href}
 
         if self.requires_python is not None:
             kwargs["data-requires-python"] = escape(self.requires_python)
         if self.metadata_hash is True:
             kwargs["data-dist-info-metadata"] = "true"
         elif self.metadata_hash is not None:
-            kwargs["data-dist-info-metadata"] = f"sha256={self.metadata_hash}"
+            kwargs["data-dist-info-metadata"] = f"{HASH_FORMAT}={self.metadata_hash}"
 
         with page.a(**kwargs):
             page(posixpath.basename(self.filename))
+
+    @classmethod
+    def from_wheel(
+        cls,
+        wheel_path: Path,
+        metadata_path: Path,
+    ) -> Optional["WheelFile"]:
+        """Create a :class:`~.WheelFile` from a wheel file and its metadata file."""
+        metadata_string = extract_metadata_from_wheel_file(wheel_path)
+        if not metadata_string:
+            return None
+        metadata_path.write_text(metadata_string)
+        wheel_metadata = metadata.loads(metadata_string)
+        wheel_file_name = wheel_path.name
+        metadata_name = wheel_metadata["Name"]
+        canonical_name = canonicalize_name(metadata_name)
+        return cls(
+            version=WHEEL_FILE_VERSION,
+            metadata_name=metadata_name,
+            canonical_name=canonical_name,
+            filename=wheel_file_name,
+            wheel_hash=get_sha256_hash(wheel_path),
+            requires_python=wheel_metadata.get("Requires-Python"),
+            metadata_hash=get_sha256_hash(metadata_path),
+        )
```

### Comparing `index_503-0.1.6/PKG-INFO` & `index_503-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: index-503 Version: 0.1.6 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.1.7 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

