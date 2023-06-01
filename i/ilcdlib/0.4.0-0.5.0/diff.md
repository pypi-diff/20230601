# Comparing `tmp/ilcdlib-0.4.0.tar.gz` & `tmp/ilcdlib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-0.4.0.tar", max compression
+gzip compressed data, was "ilcdlib-0.5.0.tar", max compression
```

## Comparing `ilcdlib-0.4.0.tar` & `ilcdlib-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
--rw-r--r--   0        0        0    11357 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/LICENSE
--rw-r--r--   0        0        0     4949 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/README.md
--rw-r--r--   0        0        0     3341 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    12504 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1334 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     1474 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     5369 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     7981 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     5749 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3650 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3774 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0     8220 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     2596 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1329 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     1185 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3328 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    19409 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1900 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1899 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1212 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     1737 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7086 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     4728 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1206 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     1712 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2382 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 ilcdlib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4949 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/README.md
+-rw-r--r--   0        0        0     3424 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    13825 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1334 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     2883 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     2665 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     5369 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     7981 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     5749 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3650 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3774 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0     8343 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     2596 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1329 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     1185 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3328 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    19523 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     7667 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1899 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1212 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     1737 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7086 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     5103 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0     8127 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     1206 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     1976 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6054 1970-01-01 00:00:00.000000 ilcdlib-0.5.0/PKG-INFO
```

### Comparing `ilcdlib-0.4.0/LICENSE` & `ilcdlib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/README.md` & `ilcdlib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/pyproject.toml` & `ilcdlib-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "0.4.0"
+version = "0.5.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -21,28 +21,30 @@
 
 [tool.poetry.scripts]
 ilcdtool = { callable = "ilcdlib:cli.entrypoint", extras = ["cli"] }
 
 [tool.poetry.dependencies]
 python = "^3.11"
 urllib3 = { version = ">=1.26.16,<2.0.0" }
-openepd = { version = ">=0.4.0,<1.0.0" }
+requests = { version = ">=2.1.0,<3.0.0" }
+openepd = { version = ">=0.5.0,<1.0.0" }
 
 # Optional dependencies
 lxml = { version = "~=4.9.2", optional = true }
 cli-rack = { version = ">=1.0.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 # Unit tests
 coverage = { version = "=6.5", extras = ["toml"] }
 pytest = "~=7.2"
 pytest-subtests = "~=0.4"
 pytest-cov = "~=4.0"
 teamcity-messages = ">=1.31"
 lxml-stubs = { version = ">=0.4.0" }
+types-requests = { version = ">=2.1.0" }
 
 # Dev tools
 black = "~=22.3"
 licenseheaders = "~=0.8"
 flake8 = "~=4.0"
 flake8-import-graph = "==0.1.3"
 flake8-docstrings = "~=1.7.0"
@@ -57,15 +59,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "0.4.0"
+version = "0.5.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
```

### Comparing `ilcdlib-0.4.0/src/ilcdlib/__init__.py` & `ilcdlib-0.5.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/__main__.py` & `ilcdlib-0.5.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/__version__.py` & `ilcdlib-0.5.0/src/ilcdlib/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.4.0"
+VERSION = "0.5.0"
```

### Comparing `ilcdlib-0.4.0/src/ilcdlib/cli.py` & `ilcdlib-0.5.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/common.py` & `ilcdlib-0.5.0/src/ilcdlib/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,14 +105,48 @@
     def __enter__(self) -> Self:
         return self
 
     def __exit__(self, _type, value, traceback):
         self.close()
 
 
+class NoopBaseReader(BaseIlcdMediumSpecificReader):
+    """A stub implementation of BaseIlcdMediumSpecificReader that does nothing."""
+
+    @overload
+    def get_entity_stream(
+        self, entity_type: str, entity_id: str, entity_version: str | None = None, *, binary: Literal[True]
+    ) -> IO[bytes]:
+        ...
+
+    @overload
+    def get_entity_stream(
+        self, entity_type: str, entity_id: str, entity_version: str | None = None, *, binary: Literal[False] = False
+    ) -> TextIO:
+        ...
+
+    def get_entity_stream(
+        self, entity_type: str, entity_id: str, entity_version: str | None = None, *, binary: bool = False
+    ) -> IO[bytes] | TextIO:
+        """Generate exception. This class does not support get_entity_stream."""
+        raise ValueError("NoopBaseReader does not support get_entity_stream")
+
+    def entity_exists(self, entity_type: str, entity_id: str, entity_version: str | None = None) -> bool:
+        """Return False regardless of parameters for this implementation."""
+        return False
+
+    def close(self):
+        """Do nothing. This implementation does not need to be closed."""
+        pass
+
+    def list_entities(self, entity_type: str) -> Sequence[IlcdReference]:
+        """Return empty list. NoopBaseReader does not support get_entity_stream."""
+        return []
+
+
 class IlcdXmlReader:
     """Base class for ILCD xml readers. It provides a set of helper methods to read ILCD data from ILCD xml."""
 
     _LANG_ATTRIB_NAME = "{http://www.w3.org/XML/1998/namespace}lang"
 
     def __init__(self, data_provider: BaseIlcdMediumSpecificReader):
         self.data_provider = data_provider
```

### Comparing `ilcdlib-0.4.0/src/ilcdlib/const.py` & `ilcdlib-0.5.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-0.5.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/dto.py` & `ilcdlib-0.5.0/src/ilcdlib/type.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,30 +13,21 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import NamedTuple
+from typing import Sequence
 
+LangDef = str | Sequence[str | None] | None
 
-class IlcdReference(NamedTuple):
-    """A reference to an ILCD entity."""
 
-    entity_type: str
-    entity_id: str
-    entity_version: str | None
+class LocalizedStr(str):
+    """A string with language code attached."""
 
-    def to_url(self, base_url: str | None) -> str:
-        """Convert the reference to a URL."""
-        prefix = base_url if base_url is not None else "https://unknown.tld"
-        if prefix.endswith("/"):
-            prefix = prefix[:-1]
-        return f"{prefix}/resource/{self.entity_type}/{self.entity_id}?version={self.entity_version}"
+    def __new__(cls, *args, **kwargs):  # noqa: D102
+        return super().__new__(cls, args[0])
 
-
-class ProductClassDef(NamedTuple):
-    """A product class definition."""
-
-    id: str | None
-    name: str | None
+    def __init__(self, s: str, lang: str | None = None):
+        super().__init__()
+        self.lang: str | None = lang
```

### Comparing `ilcdlib-0.4.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-0.5.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/entity/contact.py` & `ilcdlib-0.5.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/entity/flow.py` & `ilcdlib-0.5.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-0.5.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/entity/material.py` & `ilcdlib-0.5.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-0.5.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/entity/unit.py` & `ilcdlib-0.5.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-0.5.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/epd/cli.py` & `ilcdlib-0.5.0/src/ilcdlib/epd/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,16 @@
             )
         lang_list = [lang, None]
         if prioritize_english:
             lang_list.insert(0, "en")
         CLI.print_info("Language priority: " + ",".join([x if x is not None else "any other" for x in lang_list]))
         base_url = self.__extract_base_url(doc_ref)
         open_epd = epd_reader.to_openepd_epd(lang_list, base_url=base_url)
+        if isinstance(medium, Soda4LcaZipReader):
+            open_epd.set_ext_field("ilcd_pdf_url", medium.get_pdf_url())
         CLI.print_data(open_epd.json(indent=2, exclude_none=True, exclude_unset=True))
         if save:
             self.save_results(epd_reader, open_epd, extract_pdf=extract_pdf)
 
     def save_results(self, epd_reader: IlcdEpdReader, result: Epd, *, extract_pdf: bool = False):
         output_dir = Path(epd_reader.get_uuid())
         ensure_dir(output_dir)
```

### Comparing `ilcdlib-0.4.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-0.5.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-0.5.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-0.5.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-0.5.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/epd/factory.py` & `ilcdlib-0.5.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/epd/reader.py` & `ilcdlib-0.5.0/src/ilcdlib/epd/reader.py`

 * *Files identical despite different names*

```diff
@@ -404,14 +404,15 @@
         external_verifier = (
             external_verifier_reader.to_openepd_org(lang, base_url) if external_verifier_reader else None
         )
         pcr_reader = self.get_pcr_reader()
         pcr = pcr_reader.to_openepd_pcr(lang, base_url) if pcr_reader else None
         declared_unit = self.get_declared_unit()
         quantitative_props = self.get_quantitative_product_props_str(lang)
+        own_ref = self.get_own_reference()
         product_name = self.get_product_name(lang)
         if product_name and quantitative_props:
             product_name += "; " + quantitative_props
         material_properties = self.get_material_properties()
         other_product_props = self.get_product_flow_properties()
         product_properties = {}
         if material_properties:
@@ -423,15 +424,16 @@
         if product_properties:
             specs = Specs(ext=create_ext(product_properties))
         else:
             specs = Specs()
         return Epd.construct(
             doctype="openEPD",
             language=lang_code,
-            attachments=create_openepd_attachments(self.get_own_reference(), base_url),
+            attachments=create_openepd_attachments(own_ref, base_url),
+            declaration_url=own_ref.to_url(base_url) if own_ref and base_url else None,
             name=product_name,
             description=self.get_product_description(lang),
             date_published=self.get_date_published(),
             valid_until=self.get_validity_ends_date(),
             program_operator_doc_id=self.get_program_operator_id(),
             manufacturer=manufacturer,
             program_operator=program_operator,
```

### Comparing `ilcdlib-0.4.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-0.5.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/mapping/common.py` & `ilcdlib-0.5.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-0.5.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-0.5.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/mapping/units.py` & `ilcdlib-0.5.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-0.5.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/medium/archive.py` & `ilcdlib-0.5.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-0.5.0/src/ilcdlib/medium/soda4lca.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from urllib.parse import parse_qs
 
 import urllib3
 from urllib3.util import parse_url
 
 from ilcdlib.dto import IlcdReference
 from ilcdlib.medium.archive import ZipIlcdReader
+from ilcdlib.soda4lca.api_client import Soda4LcaXmlApiClient
 from ilcdlib.utils import none_throws
 
 http = urllib3.PoolManager()
 
 
 @dataclass(kw_only=True)
 class IlcdRemotePointer:
@@ -44,14 +45,16 @@
 class Soda4LcaZipReader(ZipIlcdReader):
     """A reader for ILCD zip archives exported from the SODA4LCA interface."""
 
     def __init__(self, endpoint: str):
         pointer = self.soda_endpoint_to_pointer(endpoint)
         if pointer.ref.entity_type != "processes":
             raise ValueError(f"Invalid endpoint {endpoint}. Must point to the process.")
+        self._soda4lca_client = Soda4LcaXmlApiClient(pointer.base_url)
+        self._ref = pointer.ref
         zip_url = self.create_zip_export_endpoint(pointer)
         zip_file = self.dowload_zip_archive(zip_url)
         super().__init__(zip_file)
 
     @classmethod
     def create_zip_export_endpoint(cls, pointer: IlcdRemotePointer) -> str:
         """Create a zip export endpoint from a remote pointer."""
@@ -104,14 +107,18 @@
         """Download a zip archive from a URL."""
         # TODO: Move this to dedicated class
         response = http.request("GET", url)
         if response.status == 200:
             return io.BytesIO(response.data)
         raise ValueError(f"Could not download zip archive from {url}. Status code: {response.status}")
 
+    def get_pdf_url(self) -> str | None:
+        """Get the URL to the PDF document if any."""
+        return self._soda4lca_client.get_download_epd_document_link(self._ref.entity_id, self._ref.entity_version)
+
     @staticmethod
     def __map_type_name(in_: str) -> str:
         match in_:
             case "process" | "showprocess":
                 return "processes"
             case _:
                 return in_
```

### Comparing `ilcdlib-0.4.0/src/ilcdlib/reference_data.py` & `ilcdlib-0.5.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-0.5.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-0.5.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-0.5.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.4.0/src/ilcdlib/utils.py` & `ilcdlib-0.5.0/src/ilcdlib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,30 +13,41 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Any, TypeVar
+from typing import TYPE_CHECKING, Any, Optional, TypeVar
 
 from ilcdlib import const
-from ilcdlib.dto import IlcdReference
 
 T = TypeVar("T")
 
+if TYPE_CHECKING:
+    from ilcdlib.dto import IlcdReference
+
 
 def none_throws(optional: T | None, message: str = "Unexpected `None`") -> T:
     """Convert an optional to its value. Raises an `AssertionError` if the value is `None`."""
     if optional is None:
         raise AssertionError(message)
     return optional
 
 
-def create_openepd_attachments(reference: IlcdReference | None, base_url: str | None = None) -> dict[str, str] | None:
+def no_trailing_slash(val: str) -> str:
+    """Remove all trailing slashes from the given string. Might be useful to normalize URLs."""
+    while val.endswith("/"):
+        val = val[:-1]
+    return val
+
+
+def create_openepd_attachments(
+    reference: Optional["IlcdReference"], base_url: str | None = None
+) -> dict[str, str] | None:
     """Create a dictionary of OpenEPD attachments."""
     if reference is None:
         return None
     return {x: reference.to_url(base_url) for x in const.ILCD_IDENTIFICATION}
 
 
 def create_ext(data: Any) -> dict[str, Any] | None:
```

### Comparing `ilcdlib-0.4.0/src/ilcdlib/xml_parser.py` & `ilcdlib-0.5.0/src/ilcdlib/xml_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         self.__xml_ns = ns_map or {}
 
     @property
     def xml_ns(self) -> dict[str, str]:
         """Get the XML namespace map."""
         return self.__xml_ns
 
-    def get_xml_tree(self, file_stream_or_str: IO | str) -> T_ET.Element:
+    def get_xml_tree(self, file_stream_or_str: IO | str | bytes) -> T_ET.Element:
         """Get the XML tree from a file stream or string."""
-        if isinstance(file_stream_or_str, str):
+        if isinstance(file_stream_or_str, (str, bytes)):
             return ET.fromstring(file_stream_or_str)
         else:
             return ET.parse(file_stream_or_str).getroot()
 
     def get_el_text(self, parent: T_ET.Element, xpath: str, default_val: str | None = None) -> str | None:
         """Get the text of an element."""
         el = parent.find(xpath, self.xml_ns)
```

### Comparing `ilcdlib-0.4.0/PKG-INFO` & `ilcdlib-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 0.4.0
+Version: 0.5.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
@@ -16,15 +16,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: cli
 Provides-Extra: lxml
 Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml"
-Requires-Dist: openepd (>=0.4.0,<1.0.0)
+Requires-Dist: openepd (>=0.5.0,<1.0.0)
+Requires-Dist: requests (>=2.1.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/cchangelabs/ilcdlib
 Description-Content-Type: text/markdown
 
 # ILCD Lib
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 0.4.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 0.5.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: support@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Provides-Extra: cli
 Provides-Extra: lxml Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml" Requires-Dist: openepd
-(>=0.4.0,<1.0.0) Requires-Dist: urllib3 (>=1.26.16,<2.0.0) Project-URL:
-Repository, https://github.com/cchangelabs/ilcdlib Description-Content-Type:
-text/markdown # ILCD Lib
+(>=0.5.0,<1.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
+urllib3 (>=1.26.16,<2.0.0) Project-URL: Repository, https://github.com/
+cchangelabs/ilcdlib Description-Content-Type: text/markdown # ILCD Lib
      [https://img.shields.io/pypi/l/ilcdlib?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/ilcdlib?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/ilcdlib?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/ilcdlib?style=for-the-badge]
   [https://img.shields.io/github/actions/workflow/status/cchangelabs/ilcdlib/
   sanity-check.yml?style=for-the-badge] [https://img.shields.io/github/last-
```

