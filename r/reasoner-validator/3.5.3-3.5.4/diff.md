# Comparing `tmp/reasoner_validator-3.5.3.tar.gz` & `tmp/reasoner_validator-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.5.3.tar", max compression
+gzip compressed data, was "reasoner_validator-3.5.4.tar", max compression
```

## Comparing `reasoner_validator-3.5.3.tar` & `reasoner_validator-3.5.4.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1153 2023-05-31 22:35:44.910859 reasoner_validator-3.5.3/LICENSE
--rw-r--r--   0        0        0    12066 2023-05-31 22:35:44.910859 reasoner_validator-3.5.3/README.md
--rw-r--r--   0        0        0      131 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/Makefile
--rw-r--r--   0        0        0     2288 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/conf.py
--rw-r--r--   0        0        0    18216 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/index.rst
--rw-r--r--   0        0        0      795 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/make.bat
--rw-r--r--   0        0        0      136 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36025 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/pyproject.toml
--rw-r--r--   0        0        0    20298 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    59895 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39243 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    26512 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     7035 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    13781 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     9165 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/versioning.py
--rw-r--r--   0        0        0        0 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/__init__.py
--rw-r--r--   0        0        0   104709 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    31906 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_response_validator.py
--rw-r--r--   0        0        0     4546 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_semver.py
--rw-r--r--   0        0        0    26567 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_validate.py
--rw-r--r--   0        0        0    19013 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_validation_report.py
--rw-r--r--   0        0        0     2068 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_workflows.py
--rw-r--r--   0        0        0    14105 1970-01-01 00:00:00.000000 reasoner_validator-3.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/LICENSE
+-rw-r--r--   0        0        0    12164 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/README.md
+-rw-r--r--   0        0        0      131 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/Makefile
+-rw-r--r--   0        0        0     2288 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/conf.py
+-rw-r--r--   0        0        0    18216 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36025 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/pyproject.toml
+-rw-r--r--   0        0        0    20298 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    59895 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39243 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    26512 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     7977 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13781 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     9922 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/__init__.py
+-rw-r--r--   0        0        0   104709 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    42178 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_data/sample_trapi_schema.yaml
+-rw-r--r--   0        0        0    31906 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_response_validator.py
+-rw-r--r--   0        0        0     4546 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_semver.py
+-rw-r--r--   0        0        0     1746 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26567 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_validate.py
+-rw-r--r--   0        0        0    19013 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2068 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_workflows.py
+-rw-r--r--   0        0        0    14203 1970-01-01 00:00:00.000000 reasoner_validator-3.5.4/PKG-INFO
```

### Comparing `reasoner_validator-3.5.3/LICENSE` & `reasoner_validator-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/README.md` & `reasoner_validator-3.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 Then build the documentation locally:
 
 ```bash
 cd ../docs
 make html
 ```
 
-The resulting **index.html** and related pages are now available for viewing within the docs subfolder __build/html_.
+The resulting **index.html** and related pages describing the programmatic API are now available for viewing within the docs subfolder __build/html_.  
 
 ## Validation Run as a Web Service
 
 The Reasoner Validator is available wrapped as a simple web service.  The service may be run directly or as a Docker container.
 
 ### API
 
@@ -134,15 +134,15 @@
   "strict_validation": true,
   "response": {<some full JSON object of a TRAPI query Response...>}
 }
 ```
 
 The request body consists of JSON data structure with two top level tag:
 
-- An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). 
+- An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). This value may also be a GitHub branch name (e.g. '**master**').
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
 - An **optional** `sources` with an object dictionary (example shown) specifying the ARA and KP sources involved in the TRAPI call (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "sources" or any of the subsidiary tags may be omitted (default to None)
 - An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors. 
 - A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
```

### Comparing `reasoner_validator-3.5.3/docs/Makefile` & `reasoner_validator-3.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/docs/conf.py` & `reasoner_validator-3.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/docs/index.rst` & `reasoner_validator-3.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/docs/make.bat` & `reasoner_validator-3.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/docs/validation_codes_dictionary.md` & `reasoner_validator-3.5.4/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/pyproject.toml` & `reasoner_validator-3.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.5.3"
+version = "3.5.4"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.5.3/reasoner_validator/__init__.py` & `reasoner_validator-3.5.4/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.5.4/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/reasoner_validator/codes.yaml` & `reasoner_validator-3.5.4/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/reasoner_validator/report.py` & `reasoner_validator-3.5.4/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/reasoner_validator/sri/util.py` & `reasoner_validator-3.5.4/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.5.4/reasoner_validator/trapi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """TRAPI Validation Functions."""
-from typing import Optional
+from typing import Optional, Dict
+from os.path import isfile
 import copy
 from functools import lru_cache
 
 import jsonschema
 import requests
 
 from yaml import load, CLoader as Loader
@@ -19,21 +20,42 @@
     branches
 )
 
 import logging
 logger = logging.getLogger(__name__)
 
 
+class TRAPIAccessError(RuntimeError):
+    pass
+
+
 @lru_cache()
-def _load_schema(schema_version: str):
-    """Load schema from GitHub."""
-    result = requests.get(
-        f"https://raw.githubusercontent.com/{GIT_ORG}/{GIT_REPO}/{schema_version}/TranslatorReasonerAPI.yaml"
-    )
-    spec = load(result.text, Loader=Loader)
+def _load_schema(schema_version: str) -> Dict:
+    """
+    Load schema from GitHub version or directly from a local schema file.
+    :param schema_version: either a Github 'v' prefixed SemVer version of a
+           TRAPI schema or a file name (path) from which the TRAPI schema may be read in.
+    :return: Dict, schema components
+    """
+    spec: Dict
+    if schema_version.lower().endswith(".yaml"):
+        # treat as a candidate TRAPI schema file path or name (the latter, assumed local)
+        if not isfile(schema_version):
+            raise TRAPIAccessError(f"Candidate TRAPI schema file '{schema_version}' does not exist!")
+        with open(schema_version, "r") as schema_file:
+            spec = load(schema_file, Loader=Loader)
+        if spec is None:
+            raise TRAPIAccessError(f"Candidate TRAPI schema file '{schema_version}' could not be retrieved!")
+    else:
+        result = requests.get(
+            f"https://raw.githubusercontent.com/{GIT_ORG}/{GIT_REPO}/{schema_version}/TranslatorReasonerAPI.yaml"
+        )
+        schema_text: str = result.text
+        spec = load(schema_text, Loader=Loader)
+
     components = spec["components"]["schemas"]
     for component, schema in components.items():
         openapi_to_jsonschema(schema, version=schema_version)
     schemas = dict()
     for component in components:
         # build json schema against which we validate
         subcomponents = copy.deepcopy(components)
@@ -41,25 +63,22 @@
         schema["components"] = {"schemas": subcomponents}
         schemas[component] = schema
     return schemas
 
 
 def load_schema(target: str):
     """
-    Load schema from GitHub.
-    :param target: release semver or git branch name containing the target TRAPI schema.
+    Load schema from GitHub release or branch, or from a locally specified YAML schema file.
+    :param target: release semver, schema file path (with '.yaml' file extension)
+                    or a git branch name, all referencing a target TRAPI schema.
     :return: loaded TRAPI schema
     """
     mapped_release = get_latest_version(target)
     if mapped_release:
         schema_version = mapped_release
-    elif target in branches:
-        # cases in which a branch name is
-        # given instead of a release number
-        schema_version = target
     else:
         err_msg: str = f"No TRAPI version {target}"
         logger.error(err_msg)
         raise ValueError(err_msg)
 
     return _load_schema(schema_version)
```

### Comparing `reasoner_validator-3.5.3/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.5.4/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/reasoner_validator/validation_codes.py` & `reasoner_validator-3.5.4/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/reasoner_validator/versioning.py` & `reasoner_validator-3.5.4/reasoner_validator/versioning.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Utilities."""
 import re
 from typing import NamedTuple, Optional, List
 from os import environ
-from functools import lru_cache
 from re import sub
 import requests
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
 
@@ -215,20 +214,38 @@
 SemVer.__ge__ = _semver_ge_
 
 _latest = dict()
 
 
 # Provide an accessor function for retrieving the latest version in string format
 def get_latest_version(release_tag: str) -> Optional[str]:
+    """
+    Return the latest TRAPI version corresponding to the release tag given.
+    Note that if the release tag looks like a YAML file, then it is assumed
+    to be a direct schema specification. If a Git branch name in the schema
+    repository, the branch name is also passed on.
+
+    :param release_tag: (possibly partial) SemVer string, Git branch name,
+                        or YAML schema file name identifying a release.
+    :return: 'best' latest release of SemVer specification or the YAML file directly returned.
+    """
     global _latest
-    # strip any prefix from the release tag to ensure that
-    # only the SemVer part is used for the latest version lookup
-    release = sub(r'^[^0-9]+', '', release_tag)
-    latest: SemVer = _latest.get(release, None)
-    return str(latest) if latest else None
+
+    if release_tag.lower().endswith(".yaml"):
+        return release_tag
+    elif release_tag in branches:
+        # cases in which a branch name is
+        # given instead of a release number
+        return release_tag
+    else:
+        # strip any prefix from the release tag to ensure that
+        # only the SemVer part is used for the latest version lookup
+        release = sub(r'^[^0-9]+', '', release_tag)
+        latest: SemVer = _latest.get(release, None)
+        return str(latest) if latest else None
 
 
 def _set_preferred_version(release_tag: str, target_release: SemVer):
     global _latest
     latest_4_release_tag: Optional[SemVer] = _latest.get(release_tag, None)
     if not latest_4_release_tag or (target_release >= latest_4_release_tag):
         _latest[release_tag] = target_release
```

### Comparing `reasoner_validator-3.5.3/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.5.4/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/tests/test_response_validator.py` & `reasoner_validator-3.5.4/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/tests/test_semver.py` & `reasoner_validator-3.5.4/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/tests/test_validate.py` & `reasoner_validator-3.5.4/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/tests/test_validation_report.py` & `reasoner_validator-3.5.4/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/tests/test_workflows.py` & `reasoner_validator-3.5.4/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.3/PKG-INFO` & `reasoner_validator-3.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.5.3
+Version: 3.5.4
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -151,15 +151,15 @@
 Then build the documentation locally:
 
 ```bash
 cd ../docs
 make html
 ```
 
-The resulting **index.html** and related pages are now available for viewing within the docs subfolder __build/html_.
+The resulting **index.html** and related pages describing the programmatic API are now available for viewing within the docs subfolder __build/html_.  
 
 ## Validation Run as a Web Service
 
 The Reasoner Validator is available wrapped as a simple web service.  The service may be run directly or as a Docker container.
 
 ### API
 
@@ -177,15 +177,15 @@
   "strict_validation": true,
   "response": {<some full JSON object of a TRAPI query Response...>}
 }
 ```
 
 The request body consists of JSON data structure with two top level tag:
 
-- An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). 
+- An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). This value may also be a GitHub branch name (e.g. '**master**').
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
 - An **optional** `sources` with an object dictionary (example shown) specifying the ARA and KP sources involved in the TRAPI call (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "sources" or any of the subsidiary tags may be omitted (default to None)
 - An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors. 
 - A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
```

