# Comparing `tmp/openepd-0.4.0.tar.gz` & `tmp/openepd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.4.0.tar", max compression
+gzip compressed data, was "openepd-0.5.0.tar", max compression
```

## Comparing `openepd-0.4.0.tar` & `openepd-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-05-29 15:43:07.684257 openepd-0.4.0/LICENSE
--rw-r--r--   0        0        0     2841 2023-05-29 15:43:07.684257 openepd-0.4.0/README.md
--rw-r--r--   0        0        0     3051 2023-05-29 15:43:07.684257 openepd-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     2155 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     2178 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/common.py
--rw-r--r--   0        0        0     7763 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0     8887 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3811 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     2855 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     1137 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3342 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1519 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0        0 2023-05-29 15:43:07.684257 openepd-0.4.0/src/openepd/py.typed
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 10:35:52.967121 openepd-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2841 2023-06-01 10:35:52.967121 openepd-0.5.0/README.md
+-rw-r--r--   0        0        0     3051 2023-06-01 10:35:52.967121 openepd-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     2613 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     2178 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0     7763 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     8887 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3811 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     2855 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     1137 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3342 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1519 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:35:52.967121 openepd-0.5.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.5.0/PKG-INFO
```

### Comparing `openepd-0.4.0/LICENSE` & `openepd-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/README.md` & `openepd-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/pyproject.toml` & `openepd-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "0.4.0"
+version = "0.5.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.4.0"
+version = "0.5.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.4.0/src/openepd/__init__.py` & `openepd-0.5.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/__version__.py` & `openepd-0.5.0/src/openepd/__version__.py`

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

### Comparing `openepd-0.4.0/src/openepd/model/__init__.py` & `openepd-0.5.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/model/base.py` & `openepd-0.5.0/src/openepd/model/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,14 +34,26 @@
         allow_population_by_field_name = True
         use_enum_values = True
 
     def has_values(self) -> bool:
         """Return True if the model has any values."""
         return len(self.dict(exclude_unset=True, exclude_none=True)) > 0
 
+    def set_ext_field(self, key: str, value: AnySerializable) -> None:
+        """Add an extension field to the model."""
+        if self.ext is None:
+            self.ext = {}
+        self.ext[key] = value
+
+    def get_ext_field(self, key: str, default: AnySerializable = None) -> AnySerializable | None:
+        """Get an extension field from the model."""
+        if self.ext is None:
+            return default
+        return self.ext.get(key, default)
+
     @classmethod
     def is_allowed_field_name(cls, field_name: str) -> bool:
         """
         Return True if the field name is defined in the module.
 
         Both property name and aliases are checked.
         """
```

### Comparing `openepd-0.4.0/src/openepd/model/common.py` & `openepd-0.5.0/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/model/epd.py` & `openepd-0.5.0/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/model/lcia.py` & `openepd-0.5.0/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/model/org.py` & `openepd-0.5.0/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/model/pcr.py` & `openepd-0.5.0/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/model/specs/__init__.py` & `openepd-0.5.0/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/model/specs/concrete.py` & `openepd-0.5.0/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/src/openepd/model/standard.py` & `openepd-0.5.0/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-0.4.0/PKG-INFO` & `openepd-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 0.4.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 0.5.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

