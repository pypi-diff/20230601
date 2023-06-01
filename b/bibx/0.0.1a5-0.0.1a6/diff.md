# Comparing `tmp/bibx-0.0.1a5.tar.gz` & `tmp/bibx-0.0.1a6.tar.gz`

## Comparing `bibx-0.0.1a5.tar` & `bibx-0.0.1a6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bibx-0.0.1a5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bibx-0.0.1a5/Makefile
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 bibx-0.0.1a5/.github/workflows/cd.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bibx-0.0.1a5/.github/workflows/ci.yml
--rw-r--r--   0        0        0  2221838 2020-02-02 00:00:00.000000 bibx-0.0.1a5/docs/examples/bit-pattern-savedrecs.txt
--rw-r--r--   0        0        0  5022778 2020-02-02 00:00:00.000000 bibx-0.0.1a5/docs/examples/scopus.bib
--rw-r--r--   0        0        0  2955913 2020-02-02 00:00:00.000000 bibx-0.0.1a5/docs/examples/scopus.ris
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 bibx-0.0.1a5/docs/examples/single-article.txt
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/__main__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/cli.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/article.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection_builders/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection_builders/base.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection_builders/cross_ref.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection_builders/generic.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection_builders/scopus_bib.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection_builders/scopus_ris.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection_builders/simple.py
--rw-r--r--   0        0        0    13050 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/_entities/collection_builders/wos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/algorithms/__init__.py
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 bibx-0.0.1a5/src/bibx/algorithms/sap.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bibx-0.0.1a5/tests/test_works.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bibx-0.0.1a5/tests/algorithms/test_sap.py
--rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 bibx-0.0.1a5/tests/entities/collection_builders/test_scopus_bib.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 bibx-0.0.1a5/tests/entities/collection_builders/test_scopus_ris.py
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 bibx-0.0.1a5/tests/entities/collection_builders/test_wos.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 bibx-0.0.1a5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bibx-0.0.1a5/LICENSE
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 bibx-0.0.1a5/README.md
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bibx-0.0.1a5/pyproject.toml
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 bibx-0.0.1a5/PKG-INFO
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bibx-0.0.1a6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bibx-0.0.1a6/Makefile
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 bibx-0.0.1a6/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bibx-0.0.1a6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0  2221838 2020-02-02 00:00:00.000000 bibx-0.0.1a6/docs/examples/bit-pattern-savedrecs.txt
+-rw-r--r--   0        0        0  5022778 2020-02-02 00:00:00.000000 bibx-0.0.1a6/docs/examples/scopus.bib
+-rw-r--r--   0        0        0  2955913 2020-02-02 00:00:00.000000 bibx-0.0.1a6/docs/examples/scopus.ris
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 bibx-0.0.1a6/docs/examples/single-article.txt
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/__main__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/cli.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/article.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection_builders/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection_builders/base.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection_builders/cross_ref.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection_builders/generic.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection_builders/scopus_bib.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection_builders/scopus_ris.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection_builders/simple.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/_entities/collection_builders/wos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/algorithms/__init__.py
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 bibx-0.0.1a6/src/bibx/algorithms/sap.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bibx-0.0.1a6/tests/test_works.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bibx-0.0.1a6/tests/algorithms/test_sap.py
+-rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 bibx-0.0.1a6/tests/entities/collection_builders/test_scopus_bib.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 bibx-0.0.1a6/tests/entities/collection_builders/test_scopus_ris.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 bibx-0.0.1a6/tests/entities/collection_builders/test_wos.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 bibx-0.0.1a6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bibx-0.0.1a6/LICENSE
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 bibx-0.0.1a6/README.md
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bibx-0.0.1a6/pyproject.toml
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 bibx-0.0.1a6/PKG-INFO
```

### Comparing `bibx-0.0.1a5/.pre-commit-config.yaml` & `bibx-0.0.1a6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/.github/workflows/cd.yml` & `bibx-0.0.1a6/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/.github/workflows/ci.yml` & `bibx-0.0.1a6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/docs/examples/bit-pattern-savedrecs.txt` & `bibx-0.0.1a6/docs/examples/bit-pattern-savedrecs.txt`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/docs/examples/scopus.bib` & `bibx-0.0.1a6/docs/examples/scopus.bib`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/docs/examples/scopus.ris` & `bibx-0.0.1a6/docs/examples/scopus.ris`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/docs/examples/single-article.txt` & `bibx-0.0.1a6/docs/examples/single-article.txt`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/src/bibx/__init__.py` & `bibx-0.0.1a6/src/bibx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Sap",
     "read_scopus_bib",
     "read_scopus_ris",
     "read_wos",
     "read_any",
 ]
 
-__version__ = "0.0.1a5"
+__version__ = "0.0.1a6"
 
 
 def read_scopus_bib(*files: TextIO) -> Collection:
     """
     Takes any number of bibtex files from scopus and generates a collection.
 
     :param files: Scopus bib files open.
```

### Comparing `bibx-0.0.1a5/src/bibx/cli.py` & `bibx-0.0.1a6/src/bibx/cli.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/src/bibx/exceptions.py` & `bibx-0.0.1a6/src/bibx/exceptions.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/src/bibx/_entities/article.py` & `bibx-0.0.1a6/src/bibx/_entities/article.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/src/bibx/_entities/collection.py` & `bibx-0.0.1a6/src/bibx/_entities/collection.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/src/bibx/_entities/collection_builders/scopus_bib.py` & `bibx-0.0.1a6/src/bibx/_entities/collection_builders/scopus_bib.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/src/bibx/_entities/collection_builders/scopus_ris.py` & `bibx-0.0.1a6/src/bibx/_entities/collection_builders/scopus_ris.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/src/bibx/_entities/collection_builders/wos.py` & `bibx-0.0.1a6/src/bibx/_entities/collection_builders/wos.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,9 +348,9 @@
             return {}
 
         if key in cls.FIELDS:
             field = cls.FIELDS[key]
             parsed_value = field.parse(value)
             return {new_key: parsed_value for new_key in [field.key, *field.aliases]}
 
-        logger.info(f"Found an unknown field with key {key} and value {value}")
+        logger.debug(f"Found an unknown field with key {key} and value {value}")
         return {key: _ident(value)}
```

### Comparing `bibx-0.0.1a5/src/bibx/algorithms/sap.py` & `bibx-0.0.1a6/src/bibx/algorithms/sap.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/tests/algorithms/test_sap.py` & `bibx-0.0.1a6/tests/algorithms/test_sap.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/tests/entities/collection_builders/test_scopus_bib.py` & `bibx-0.0.1a6/tests/entities/collection_builders/test_scopus_bib.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/tests/entities/collection_builders/test_scopus_ris.py` & `bibx-0.0.1a6/tests/entities/collection_builders/test_scopus_ris.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/tests/entities/collection_builders/test_wos.py` & `bibx-0.0.1a6/tests/entities/collection_builders/test_wos.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/.gitignore` & `bibx-0.0.1a6/.gitignore`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/LICENSE` & `bibx-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/README.md` & `bibx-0.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/pyproject.toml` & `bibx-0.0.1a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a5/PKG-INFO` & `bibx-0.0.1a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibx
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: Python bibliometric tools.
 Author-email: Core of Science Team <technology@coreofscience.org>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: bibliometrics,science,text mining
 Requires-Dist: bibtexparser~=1.4.0
 Requires-Dist: networkx~=3.0
```

