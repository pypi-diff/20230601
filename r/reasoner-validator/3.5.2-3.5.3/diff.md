# Comparing `tmp/reasoner_validator-3.5.2.tar.gz` & `tmp/reasoner_validator-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.5.2.tar", max compression
+gzip compressed data, was "reasoner_validator-3.5.3.tar", max compression
```

## Comparing `reasoner_validator-3.5.2.tar` & `reasoner_validator-3.5.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1153 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/LICENSE
--rw-r--r--   0        0        0    12066 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/README.md
--rw-r--r--   0        0        0      131 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/Makefile
--rw-r--r--   0        0        0     2288 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/conf.py
--rw-r--r--   0        0        0    18216 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/index.rst
--rw-r--r--   0        0        0      795 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/make.bat
--rw-r--r--   0        0        0      136 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36025 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/pyproject.toml
--rw-r--r--   0        0        0    20298 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    59678 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39243 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    26512 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     7035 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    13781 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     9165 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/reasoner_validator/versioning.py
--rw-r--r--   0        0        0        0 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/__init__.py
--rw-r--r--   0        0        0   102228 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    31906 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_response_validator.py
--rw-r--r--   0        0        0     4546 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_semver.py
--rw-r--r--   0        0        0    26567 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_validate.py
--rw-r--r--   0        0        0    19013 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_validation_report.py
--rw-r--r--   0        0        0     2068 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_workflows.py
--rw-r--r--   0        0        0    14105 1970-01-01 00:00:00.000000 reasoner_validator-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-05-31 22:35:44.910859 reasoner_validator-3.5.3/LICENSE
+-rw-r--r--   0        0        0    12066 2023-05-31 22:35:44.910859 reasoner_validator-3.5.3/README.md
+-rw-r--r--   0        0        0      131 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/Makefile
+-rw-r--r--   0        0        0     2288 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/conf.py
+-rw-r--r--   0        0        0    18216 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36025 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/pyproject.toml
+-rw-r--r--   0        0        0    20298 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    59895 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39243 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    26512 2023-05-31 22:35:44.914859 reasoner_validator-3.5.3/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     7035 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13781 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     9165 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/__init__.py
+-rw-r--r--   0        0        0   104709 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    31906 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_response_validator.py
+-rw-r--r--   0        0        0     4546 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_semver.py
+-rw-r--r--   0        0        0    26567 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_validate.py
+-rw-r--r--   0        0        0    19013 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2068 2023-05-31 22:35:44.918859 reasoner_validator-3.5.3/tests/test_workflows.py
+-rw-r--r--   0        0        0    14105 1970-01-01 00:00:00.000000 reasoner_validator-3.5.3/PKG-INFO
```

### Comparing `reasoner_validator-3.5.2/LICENSE` & `reasoner_validator-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/README.md` & `reasoner_validator-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/docs/Makefile` & `reasoner_validator-3.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/docs/conf.py` & `reasoner_validator-3.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/docs/index.rst` & `reasoner_validator-3.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/docs/make.bat` & `reasoner_validator-3.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/docs/validation_codes_dictionary.md` & `reasoner_validator-3.5.3/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/pyproject.toml` & `reasoner_validator-3.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.5.2"
+version = "3.5.3"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.5.2/reasoner_validator/__init__.py` & `reasoner_validator-3.5.3/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.5.3/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,27 +199,32 @@
                         )
             else:
                 self.report(
                     code="error.knowledge_graph.node.category.missing",
                     context=self.graph_type.value, identifier=node_id
                 )
 
-            # TODO: Do we need to (or can we) validate here, any other Knowledge Graph node fields? Perhaps not yet?
+            # TODO: Do we need to (or can we) validate here, any other
+            #       Knowledge Graph node fields? Perhaps not yet?
 
         else:  # Query Graph node validation
 
             has_node_ids: bool
             if "ids" in slots and slots["ids"]:
                 has_node_ids = True
                 node_ids = slots["ids"]
-                if not isinstance(node_ids, List):
+                if isinstance(node_ids, List):
+                    # because the validation below is destructive
+                    # to node_ids, we copy the original list
+                    node_ids = node_ids.copy()
+                else:
                     self.report(code="error.query_graph.node.ids.not_array", identifier=node_id)
                     # we'll pretend that the ids were mistakenly
                     # just a scalar string, then continue validating
-                    node_ids = [node_ids]
+                    node_ids = [str(node_ids)]
             else:
                 has_node_ids = False
                 node_ids = list()  # a null "ids" value is permitted in QNodes
 
             if "categories" in slots:
                 categories = slots["categories"]
                 if categories:
```

### Comparing `reasoner_validator-3.5.2/reasoner_validator/codes.yaml` & `reasoner_validator-3.5.3/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/reasoner_validator/report.py` & `reasoner_validator-3.5.3/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/reasoner_validator/sri/util.py` & `reasoner_validator-3.5.3/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.5.3/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.5.3/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/reasoner_validator/validation_codes.py` & `reasoner_validator-3.5.3/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/reasoner_validator/versioning.py` & `reasoner_validator-3.5.3/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.5.3/tests/test_biolink_compliance_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,14 +345,89 @@
 @pytest.mark.parametrize(
     "query",
     [
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 0: Sample small valid TRAPI Query Graph
             {
+                "edges": {
+                    "t_edge": {
+                        "attribute_constraints": [],
+                        "exclude": None,
+                        "knowledge_type": "inferred",
+                        "object": "on",
+                        "option_group_id": None,
+                        "predicates": [
+                            "biolink:treats"
+                        ],
+                        "qualifier_constraints": [],
+                        "subject": "sn"
+                    }
+                },
+                "nodes": {
+                    "on": {
+                        "categories": [
+                            "biolink:Disease"
+                        ],
+                        "constraints": [],
+                        "ids": [
+                            "MONDO:0015564"
+                        ],
+                        "is_set": False,
+                        "option_group_id": None
+                    },
+                    "sn": {
+                        "categories": [
+                            "biolink:ChemicalEntity"
+                        ],
+                        "constraints": [],
+                        "ids": None,
+                        "is_set": False,
+                        "option_group_id": None
+                    }
+                }
+            }
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 1: Simpler small valid TRAPI Query Graph
+            {
+                "nodes": {
+                    "type-2 diabetes": {"ids": ["MONDO:0005148"]},
+                    "drug": {
+                        "categories": ["biolink:Drug"]
+                    }
+                },
+                "edges": {
+                    "treats": {
+                        "subject": "drug",
+                        "predicates": ["biolink:treats"],
+                        "object": "type-2 diabetes"
+                    }
+                }
+            }
+        )
+    ]
+)
+def test_conservation_of_query_graph(query: Tuple):
+    """
+    This test checks for internal glitch where the query graph is somehow deleted
+    """
+    original_graph: Dict = deepcopy(query[1])
+    check_biolink_model_compliance_of_query_graph(graph=query[1], biolink_version=query[0])
+    assert query[1] == original_graph
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 0: Sample small valid TRAPI Query Graph
+            {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
```

### Comparing `reasoner_validator-3.5.2/tests/test_response_validator.py` & `reasoner_validator-3.5.3/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/tests/test_semver.py` & `reasoner_validator-3.5.3/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/tests/test_validate.py` & `reasoner_validator-3.5.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/tests/test_validation_report.py` & `reasoner_validator-3.5.3/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/tests/test_workflows.py` & `reasoner_validator-3.5.3/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.2/PKG-INFO` & `reasoner_validator-3.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.5.2
+Version: 3.5.3
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

