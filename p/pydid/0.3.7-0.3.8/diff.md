# Comparing `tmp/pydid-0.3.7.tar.gz` & `tmp/pydid-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydid-0.3.7.tar", max compression
+gzip compressed data, was "pydid-0.3.8.tar", max compression
```

## Comparing `pydid-0.3.7.tar` & `pydid-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2022-12-22 20:28:42.693198 pydid-0.3.7/LICENSE
--rw-r--r--   0        0        0      848 2022-12-22 20:28:42.693198 pydid-0.3.7/README.md
--rw-r--r--   0        0        0     1680 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/__init__.py
--rw-r--r--   0        0        0      318 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/common.py
--rw-r--r--   0        0        0     2294 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/did.py
--rw-r--r--   0        0        0     2773 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/did_url.py
--rw-r--r--   0        0        0      560 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/doc/__init__.py
--rw-r--r--   0        0        0     8206 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/doc/builder.py
--rw-r--r--   0        0        0     1322 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/doc/corrections.py
--rw-r--r--   0        0        0     8247 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/doc/doc.py
--rw-r--r--   0        0        0     1807 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/doc/generic.py
--rw-r--r--   0        0        0     4647 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/resource.py
--rw-r--r--   0        0        0      912 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/service.py
--rw-r--r--   0        0        0     1002 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/validation.py
--rw-r--r--   0        0        0     8458 2022-12-22 20:28:42.693198 pydid-0.3.7/pydid/verification_method.py
--rw-r--r--   0        0        0     1089 2022-12-22 20:28:42.693198 pydid-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1661 2022-12-22 20:29:37.826436 pydid-0.3.7/setup.py
--rw-r--r--   0        0        0     1714 2022-12-22 20:29:37.826799 pydid-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 15:20:49.282083 pydid-0.3.8/LICENSE
+-rw-r--r--   0        0        0      848 2023-06-01 15:20:49.282083 pydid-0.3.8/README.md
+-rw-r--r--   0        0        0     1680 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/common.py
+-rw-r--r--   0        0        0     2294 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/did.py
+-rw-r--r--   0        0        0     2773 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/did_url.py
+-rw-r--r--   0        0        0      560 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/__init__.py
+-rw-r--r--   0        0        0     8263 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/builder.py
+-rw-r--r--   0        0        0     1322 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/corrections.py
+-rw-r--r--   0        0        0     8247 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/doc.py
+-rw-r--r--   0        0        0     1807 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/generic.py
+-rw-r--r--   0        0        0     4647 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/resource.py
+-rw-r--r--   0        0        0      912 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/service.py
+-rw-r--r--   0        0        0     1002 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/validation.py
+-rw-r--r--   0        0        0     8458 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/verification_method.py
+-rw-r--r--   0        0        0     1089 2023-06-01 15:20:49.282083 pydid-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1661 2023-06-01 15:21:52.866118 pydid-0.3.8/setup.py
+-rw-r--r--   0        0        0     1714 2023-06-01 15:21:52.866602 pydid-0.3.8/PKG-INFO
```

### Comparing `pydid-0.3.7/LICENSE` & `pydid-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/README.md` & `pydid-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/__init__.py` & `pydid-0.3.8/pydid/__init__.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/did.py` & `pydid-0.3.8/pydid/did.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/did_url.py` & `pydid-0.3.8/pydid/did_url.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/doc/__init__.py` & `pydid-0.3.8/pydid/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/doc/builder.py` & `pydid-0.3.8/pydid/doc/builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -165,27 +165,25 @@
         """Remove service from builder."""
         self.services.remove(service)
 
 
 class DIDDocumentBuilder:
     """Builder for constructing DID Documents programmatically."""
 
-    DEFAULT_CONTEXT = ["https://www.w3.org/ns/did/v1"]
-
     def __init__(
         self,
         id: Union[str, DID],
         context: List[str] = None,
         *,
         also_known_as: List[str] = None,
         controller: Union[List[str], List[DID]] = None
     ):
         """Initliaze builder."""
         self.id: DID = DID(id)
-        self.context = context or self.DEFAULT_CONTEXT
+        self.context = context or self.__default_context()
         self.also_known_as = also_known_as
         self.controller = controller
         self.verification_method = VerificationMethodBuilder(self.id)
         self.authentication = RelationshipBuilder(self.id, "auth")
         self.assertion_method = RelationshipBuilder(self.id, "assert")
         self.key_agreement = RelationshipBuilder(self.id, "key-agreement")
         self.capability_invocation = RelationshipBuilder(
@@ -193,14 +191,18 @@
         )
         self.capability_delegation = RelationshipBuilder(
             self.id, "capability-delegation"
         )
         self.service = ServiceBuilder(self.id)
         self.extra = {}
 
+    @staticmethod
+    def __default_context() -> List[str]:
+        return ["https://www.w3.org/ns/did/v1"]
+
     @classmethod
     def from_doc(cls, doc: DIDDocument) -> "DIDDocumentBuilder":
         """Create a Builder from an existing DIDDocument."""
         builder = cls(
             id=doc.id,
             context=doc.context,
             also_known_as=doc.also_known_as,
```

### Comparing `pydid-0.3.7/pydid/doc/corrections.py` & `pydid-0.3.8/pydid/doc/corrections.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/doc/doc.py` & `pydid-0.3.8/pydid/doc/doc.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/doc/generic.py` & `pydid-0.3.8/pydid/doc/generic.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/resource.py` & `pydid-0.3.8/pydid/resource.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/service.py` & `pydid-0.3.8/pydid/service.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/validation.py` & `pydid-0.3.8/pydid/validation.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pydid/verification_method.py` & `pydid-0.3.8/pydid/verification_method.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.7/pyproject.toml` & `pydid-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydid"
-version = "0.3.7"
+version = "0.3.8"
 description = "Python library for validating, constructing, and representing DIDs and DID Documents"
 authors = ["Daniel Bluhm <dbluhm@pm.me>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/Indicio-tech/pydid"
 repository = "https://github.com/Indicio-tech/pydid"
 keywords = [
```

### Comparing `pydid-0.3.7/setup.py` & `pydid-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['inflection>=0.5.1,<0.6.0',
  'pydantic>=1.8.1,<2.0.0',
  'typing-extensions>=4.0.0,<4.1.0']
 
 setup_kwargs = {
     'name': 'pydid',
-    'version': '0.3.7',
+    'version': '0.3.8',
     'description': 'Python library for validating, constructing, and representing DIDs and DID Documents',
     'long_description': '# PyDID\n\n[![pypi release](https://img.shields.io/pypi/v/pydid)](https://pypi.org/project/pydid/)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\nPython library for validating, constructing, and representing DIDs and DID Documents.\n\n## Installation\n\nUsing a virtual environment is generally recommended:\n\n```sh\n$ python -m venv env\n$ source env/bin/activate\n```\n\nInstall with pip:\n\n```sh\n$ pip install pydid\n```\n\n## Development\n\nThis project is managed with [Poetry](https://python-poetry.org/).\n\nTo begin making code changes, clone this repo and do the following to install\ndependencies:\n\n```sh\n$ python -m venv env\n$ source env/bin/activate\n$ pip install poetry\n$ poetry install\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md).\n',
     'author': 'Daniel Bluhm',
     'author_email': 'dbluhm@pm.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Indicio-tech/pydid',
```

### Comparing `pydid-0.3.7/PKG-INFO` & `pydid-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydid
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python library for validating, constructing, and representing DIDs and DID Documents
 Home-page: https://github.com/Indicio-tech/pydid
 License: Apache 2.0
 Keywords: decentralized,identity,ssi
 Author: Daniel Bluhm
 Author-email: dbluhm@pm.me
 Requires-Python: >=3.6.9,<4.0.0
```

