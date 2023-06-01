# Comparing `tmp/texta-mlp-1.9.0.tar.gz` & `tmp/texta-mlp-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/texta-mlp-1.9.0.tar", last modified: Wed Mar  3 09:03:05 2021, max compression
+gzip compressed data, was "dist/texta-mlp-1.9.1.tar", last modified: Wed Mar 10 08:48:44 2021, max compression
```

## Comparing `texta-mlp-1.9.0.tar` & `texta-mlp-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)    35062 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       38 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    16190 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13853 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2021-03-03 08:17:37.000000 texta-mlp-1.9.0/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      116 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      685 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/texta_mlp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/texta_mlp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30157 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/texta_mlp/concatenator.py
--rw-rw-rw-   0 root         (0) root         (0)    28394 2021-03-01 10:58:13.000000 texta-mlp-1.9.0/texta_mlp/document.py
--rw-rw-rw-   0 root         (0) root         (0)     8591 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/texta_mlp/entity_mapper.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/texta_mlp/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/texta_mlp/fact.py
--rw-rw-rw-   0 root         (0) root         (0)    16847 2021-03-03 08:34:32.000000 texta-mlp-1.9.0/texta_mlp/mlp.py
--rw-rw-rw-   0 root         (0) root         (0)     9713 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/texta_mlp/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)    11414 2021-03-01 10:10:29.000000 texta-mlp-1.9.0/texta_mlp/russian_transliterator.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2021-03-03 08:17:37.000000 texta-mlp-1.9.0/texta_mlp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/texta_mlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16190 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/texta_mlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      459 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/texta_mlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/texta_mlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/texta_mlp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-03-03 09:03:05.000000 texta-mlp-1.9.0/texta_mlp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35062 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       38 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    16531 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14114 2021-03-10 08:34:19.000000 texta-mlp-1.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2021-03-10 08:34:19.000000 texta-mlp-1.9.1/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      116 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      685 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/texta_mlp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/texta_mlp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30157 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/texta_mlp/concatenator.py
+-rw-rw-rw-   0 root         (0) root         (0)    28388 2021-03-10 08:47:33.000000 texta-mlp-1.9.1/texta_mlp/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     8591 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/texta_mlp/entity_mapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/texta_mlp/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/texta_mlp/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)    16847 2021-03-10 08:34:19.000000 texta-mlp-1.9.1/texta_mlp/mlp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9713 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/texta_mlp/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)    11414 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/texta_mlp/russian_transliterator.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2021-03-09 09:31:56.000000 texta-mlp-1.9.1/texta_mlp/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/texta_mlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16531 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/texta_mlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      459 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/texta_mlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/texta_mlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/texta_mlp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-03-10 08:48:44.000000 texta-mlp-1.9.1/texta_mlp.egg-info/top_level.txt
```

### Comparing `texta-mlp-1.9.0/LICENSE` & `texta-mlp-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `texta-mlp-1.9.0/PKG-INFO` & `texta-mlp-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texta-mlp
-Version: 1.9.0
+Version: 1.9.1
 Summary: TEXTA Multilingual Processor (MLP)
 Home-page: https://git.texta.ee/texta/texta-mlp-python
 Author: TEXTA
 Author-email: info@texta.ee
 License: GPLv3
 Description: # TEXTA MLP Python package
         
@@ -19,14 +19,24 @@
         
         ##### From Git
         `pip3 install git+https://git.texta.ee/texta/texta-mlp-python.git`
         
         ### Testing
         `python3 -m pytest -v tests`
         
+        ## Entities
+        MLP extracts following entities:
+        * Persons (missing Estonian model)
+        * Organizations (missing Estonian model)
+        * Geopolitical entities (missing Estonian model)
+        * Phone numbers
+        * Email addresses
+        * Companies (Estonian)
+        * Addresses (Estonian & Russian)
+        
         ## Usage
         
         ### Load MLP
         Supported languages: https://stanzanlp.github.io/stanzanlp/models.html
         ```
         >>> from texta_mlp.mlp import MLP
         >>> mlp = MLP(language_codes=["et","en","ru"])
```

### Comparing `texta-mlp-1.9.0/README.md` & `texta-mlp-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 
 ##### From Git
 `pip3 install git+https://git.texta.ee/texta/texta-mlp-python.git`
 
 ### Testing
 `python3 -m pytest -v tests`
 
+## Entities
+MLP extracts following entities:
+* Persons (missing Estonian model)
+* Organizations (missing Estonian model)
+* Geopolitical entities (missing Estonian model)
+* Phone numbers
+* Email addresses
+* Companies (Estonian)
+* Addresses (Estonian & Russian)
+
 ## Usage
 
 ### Load MLP
 Supported languages: https://stanzanlp.github.io/stanzanlp/models.html
 ```
 >>> from texta_mlp.mlp import MLP
 >>> mlp = MLP(language_codes=["et","en","ru"])
```

### Comparing `texta-mlp-1.9.0/setup.py` & `texta-mlp-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `texta-mlp-1.9.0/texta_mlp/concatenator.py` & `texta-mlp-1.9.1/texta_mlp/concatenator.py`

 * *Files identical despite different names*

### Comparing `texta-mlp-1.9.0/texta_mlp/document.py` & `texta-mlp-1.9.1/texta_mlp/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,16 @@
         return nested_dict_wrapper.convert()
 
 
     def to_json(self, use_default_doc_path=True) -> dict:
         container = dict()
         container["text"] = self.get_words()
         texta_facts = self.facts_to_json()
-        container["lang"] = {"detected_lang": self.dominant_language_code,
-                             "analysis_lang": self.analysis_lang}
+        container["language"] = {"detected": self.dominant_language_code,
+                             "analysis": self.analysis_lang}
         if "lemmas" in self.analyzers: container["lemmas"] = self.get_lemma()
         if "pos_tags" in self.analyzers: container["pos_tags"] = self.get_pos_tags()
         # if "sentiment" in self.analyzers: container["sentiment"] = self.get_sentiment()
         if "transliteration" in self.analyzers and self.__transliteration: container[
             "transliteration"] = self.get_transliteration()
         if use_default_doc_path:
             for fact in texta_facts["texta_facts"]:
```

### Comparing `texta-mlp-1.9.0/texta_mlp/entity_mapper.py` & `texta-mlp-1.9.1/texta_mlp/entity_mapper.py`

 * *Files identical despite different names*

### Comparing `texta-mlp-1.9.0/texta_mlp/fact.py` & `texta-mlp-1.9.1/texta_mlp/fact.py`

 * *Files identical despite different names*

### Comparing `texta-mlp-1.9.0/texta_mlp/mlp.py` & `texta-mlp-1.9.1/texta_mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `texta-mlp-1.9.0/texta_mlp/parsers.py` & `texta-mlp-1.9.1/texta_mlp/parsers.py`

 * *Files identical despite different names*

### Comparing `texta-mlp-1.9.0/texta_mlp/russian_transliterator.py` & `texta-mlp-1.9.1/texta_mlp/russian_transliterator.py`

 * *Files identical despite different names*

### Comparing `texta-mlp-1.9.0/texta_mlp.egg-info/PKG-INFO` & `texta-mlp-1.9.1/texta_mlp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texta-mlp
-Version: 1.9.0
+Version: 1.9.1
 Summary: TEXTA Multilingual Processor (MLP)
 Home-page: https://git.texta.ee/texta/texta-mlp-python
 Author: TEXTA
 Author-email: info@texta.ee
 License: GPLv3
 Description: # TEXTA MLP Python package
         
@@ -19,14 +19,24 @@
         
         ##### From Git
         `pip3 install git+https://git.texta.ee/texta/texta-mlp-python.git`
         
         ### Testing
         `python3 -m pytest -v tests`
         
+        ## Entities
+        MLP extracts following entities:
+        * Persons (missing Estonian model)
+        * Organizations (missing Estonian model)
+        * Geopolitical entities (missing Estonian model)
+        * Phone numbers
+        * Email addresses
+        * Companies (Estonian)
+        * Addresses (Estonian & Russian)
+        
         ## Usage
         
         ### Load MLP
         Supported languages: https://stanzanlp.github.io/stanzanlp/models.html
         ```
         >>> from texta_mlp.mlp import MLP
         >>> mlp = MLP(language_codes=["et","en","ru"])
```

