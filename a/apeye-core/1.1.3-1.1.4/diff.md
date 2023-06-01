# Comparing `tmp/apeye_core-1.1.3.tar.gz` & `tmp/apeye_core-1.1.4.tar.gz`

## Comparing `apeye_core-1.1.3.tar` & `apeye_core-1.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 apeye_core-1.1.3/requirements.txt
--rw-r--r--   0        0        0    20996 2020-02-02 00:00:00.000000 apeye_core-1.1.3/apeye_core/__init__.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 apeye_core-1.1.3/apeye_core/_tld.py
--rw-r--r--   0        0        0    18573 2020-02-02 00:00:00.000000 apeye_core-1.1.3/apeye_core/email_validator.py
--rw-r--r--   0        0        0   241256 2020-02-02 00:00:00.000000 apeye_core-1.1.3/apeye_core/public_suffix_list.dat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apeye_core-1.1.3/apeye_core/py.typed
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 apeye_core-1.1.3/.gitignore
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 apeye_core-1.1.3/LICENSE
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 apeye_core-1.1.3/README.rst
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 apeye_core-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     7632 2020-02-02 00:00:00.000000 apeye_core-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 apeye_core-1.1.4/requirements.txt
+-rw-r--r--   0        0        0    21056 2020-02-02 00:00:00.000000 apeye_core-1.1.4/apeye_core/__init__.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 apeye_core-1.1.4/apeye_core/_tld.py
+-rw-r--r--   0        0        0    18573 2020-02-02 00:00:00.000000 apeye_core-1.1.4/apeye_core/email_validator.py
+-rw-r--r--   0        0        0   241256 2020-02-02 00:00:00.000000 apeye_core-1.1.4/apeye_core/public_suffix_list.dat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apeye_core-1.1.4/apeye_core/py.typed
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 apeye_core-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 apeye_core-1.1.4/LICENSE
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 apeye_core-1.1.4/README.rst
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 apeye_core-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7632 2020-02-02 00:00:00.000000 apeye_core-1.1.4/PKG-INFO
```

### Comparing `apeye_core-1.1.3/apeye_core/__init__.py` & `apeye_core-1.1.4/apeye_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 if TYPE_CHECKING:
 	# stdlib
 	from typing import NoReturn
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2022 Dominic Davis-Foster"
 __license__: str = "BSD 3-Clause License"
-__version__: str = "1.1.3"
+__version__: str = "1.1.4"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["URL", "URLPath", "Domain", "URLType", "URLPathType"]
 
 # NOTE: Use the relevant version numbers for apeye itself.
 
 URLType = TypeVar("URLType", bound="URL")
@@ -121,17 +121,17 @@
 		if not hasattr(self, "_root"):
 			self._load_parts()  # type: ignore[attr-defined]
 
 		try:
 			return self._str  # type: ignore
 		except AttributeError:
 			if hasattr(self, "_parts"):
-				parts = self._parts
+				parts = self._parts  # type: ignore[attr-defined]
 			else:
-				parts = self._tail
+				parts = self._tail  # type: ignore[attr-defined]
 
 			self._str = self._format_parsed_parts(self._drv, self._root, parts) or ''  # type: ignore
 			return self._str
 
 	def __repr__(self) -> str:
 		return super().__repr__()
```

### Comparing `apeye_core-1.1.3/apeye_core/_tld.py` & `apeye_core-1.1.4/apeye_core/_tld.py`

 * *Files identical despite different names*

### Comparing `apeye_core-1.1.3/apeye_core/email_validator.py` & `apeye_core-1.1.4/apeye_core/email_validator.py`

 * *Files identical despite different names*

### Comparing `apeye_core-1.1.3/apeye_core/public_suffix_list.dat` & `apeye_core-1.1.4/apeye_core/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `apeye_core-1.1.3/.gitignore` & `apeye_core-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `apeye_core-1.1.3/LICENSE` & `apeye_core-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apeye_core-1.1.3/README.rst` & `apeye_core-1.1.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/apeye-core
 	:target: https://github.com/domdfcoding/apeye-core/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/apeye-core
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/apeye-core/v1.1.3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/apeye-core/v1.1.4
 	:target: https://github.com/domdfcoding/apeye-core/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/apeye-core
 	:target: https://github.com/domdfcoding/apeye-core/commit/master
 	:alt: GitHub last commit
```

### Comparing `apeye_core-1.1.3/pyproject.toml` & `apeye_core-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatch-requirements-txt",]
 build-backend = "hatchling.build"
 
 [project]
 name = "apeye-core"
-version = "1.1.3"
+version = "1.1.4"
 description = "Core (offline) functionality for the apeye library."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "url",]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `apeye_core-1.1.3/PKG-INFO` & `apeye_core-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeye-core
-Version: 1.1.3
+Version: 1.1.4
 Summary: Core (offline) functionality for the apeye library.
 Project-URL: Homepage, https://github.com/domdfcoding/apeye-core
 Project-URL: Issue Tracker, https://github.com/domdfcoding/apeye-core/issues
 Project-URL: Source Code, https://github.com/domdfcoding/apeye-core
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2022, Dominic Davis-Foster
         
@@ -143,15 +143,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/apeye-core
 	:target: https://github.com/domdfcoding/apeye-core/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/apeye-core
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/apeye-core/v1.1.3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/apeye-core/v1.1.4
 	:target: https://github.com/domdfcoding/apeye-core/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/apeye-core
 	:target: https://github.com/domdfcoding/apeye-core/commit/master
 	:alt: GitHub last commit
```

