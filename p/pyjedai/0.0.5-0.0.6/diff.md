# Comparing `tmp/pyjedai-0.0.5.tar.gz` & `tmp/pyjedai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjedai-0.0.5.tar", last modified: Wed May 17 14:21:47 2023, max compression
+gzip compressed data, was "pyjedai-0.0.6.tar", last modified: Thu Jun  1 09:49:46 2023, max compression
```

## Comparing `pyjedai-0.0.5.tar` & `pyjedai-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 14:21:47.907971 pyjedai-0.0.5/
--rw-rw-rw-   0        0        0    11684 2022-09-21 14:32:22.000000 pyjedai-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     7234 2023-05-17 14:21:47.906971 pyjedai-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5557 2023-05-17 14:11:07.000000 pyjedai-0.0.5/README.md
--rw-rw-rw-   0        0        0     2428 2023-05-17 14:13:30.000000 pyjedai-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 14:21:47.908973 pyjedai-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 14:21:47.806873 pyjedai-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 14:21:47.853183 pyjedai-0.0.5/src/pyjedai/
--rw-rw-rw-   0        0        0        0 2022-07-19 14:45:04.000000 pyjedai-0.0.5/src/pyjedai/__init__.py
--rw-rw-rw-   0        0        0    18483 2023-05-05 17:55:55.000000 pyjedai-0.0.5/src/pyjedai/block_building.py
--rw-rw-rw-   0        0        0     8520 2023-05-05 17:55:55.000000 pyjedai-0.0.5/src/pyjedai/block_cleaning.py
--rw-rw-rw-   0        0        0     8107 2023-05-16 13:45:11.000000 pyjedai-0.0.5/src/pyjedai/clustering.py
--rw-rw-rw-   0        0        0    29695 2023-05-15 12:18:45.000000 pyjedai-0.0.5/src/pyjedai/comparison_cleaning.py
--rw-rw-rw-   0        0        0     9857 2023-05-15 14:47:19.000000 pyjedai-0.0.5/src/pyjedai/datamodel.py
--rw-rw-rw-   0        0        0    18898 2023-05-15 10:36:29.000000 pyjedai-0.0.5/src/pyjedai/evaluation.py
--rw-rw-rw-   0        0        0    14566 2023-05-17 08:37:13.000000 pyjedai-0.0.5/src/pyjedai/joins.py
--rw-rw-rw-   0        0        0      774 2022-08-31 12:44:46.000000 pyjedai-0.0.5/src/pyjedai/logs.py
--rw-rw-rw-   0        0        0    24233 2023-05-16 12:56:27.000000 pyjedai-0.0.5/src/pyjedai/matching.py
--rw-rw-rw-   0        0        0     8156 2023-05-16 12:34:27.000000 pyjedai-0.0.5/src/pyjedai/utils.py
--rw-rw-rw-   0        0        0    27635 2023-05-15 11:13:12.000000 pyjedai-0.0.5/src/pyjedai/vector_based_blocking.py
--rw-rw-rw-   0        0        0      955 2022-07-19 14:45:04.000000 pyjedai-0.0.5/src/pyjedai/visualization.py
--rw-rw-rw-   0        0        0    24786 2023-03-21 21:57:00.000000 pyjedai-0.0.5/src/pyjedai/workflow.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:21:47.903961 pyjedai-0.0.5/src/pyjedai.egg-info/
--rw-rw-rw-   0        0        0     7234 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      405 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:46.476420 pyjedai-0.0.6/
+-rw-rw-rw-   0        0        0    11684 2022-09-21 14:32:22.000000 pyjedai-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     7197 2023-06-01 09:49:46.474413 pyjedai-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5557 2023-05-17 14:23:07.000000 pyjedai-0.0.6/README.md
+-rw-rw-rw-   0        0        0     2425 2023-06-01 09:49:26.000000 pyjedai-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:49:46.476420 pyjedai-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:46.396943 pyjedai-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:46.437252 pyjedai-0.0.6/src/pyjedai/
+-rw-rw-rw-   0        0        0        0 2022-07-19 14:45:04.000000 pyjedai-0.0.6/src/pyjedai/__init__.py
+-rw-rw-rw-   0        0        0    18483 2023-05-05 17:55:55.000000 pyjedai-0.0.6/src/pyjedai/block_building.py
+-rw-rw-rw-   0        0        0     8520 2023-05-05 17:55:55.000000 pyjedai-0.0.6/src/pyjedai/block_cleaning.py
+-rw-rw-rw-   0        0        0     8107 2023-05-16 13:45:11.000000 pyjedai-0.0.6/src/pyjedai/clustering.py
+-rw-rw-rw-   0        0        0    29695 2023-05-15 12:18:45.000000 pyjedai-0.0.6/src/pyjedai/comparison_cleaning.py
+-rw-rw-rw-   0        0        0     9931 2023-05-24 11:14:07.000000 pyjedai-0.0.6/src/pyjedai/datamodel.py
+-rw-rw-rw-   0        0        0    18898 2023-05-15 10:36:29.000000 pyjedai-0.0.6/src/pyjedai/evaluation.py
+-rw-rw-rw-   0        0        0    14566 2023-05-17 08:37:13.000000 pyjedai-0.0.6/src/pyjedai/joins.py
+-rw-rw-rw-   0        0        0      774 2022-08-31 12:44:46.000000 pyjedai-0.0.6/src/pyjedai/logs.py
+-rw-rw-rw-   0        0        0    24233 2023-05-16 12:56:27.000000 pyjedai-0.0.6/src/pyjedai/matching.py
+-rw-rw-rw-   0        0        0     8156 2023-05-16 12:34:27.000000 pyjedai-0.0.6/src/pyjedai/utils.py
+-rw-rw-rw-   0        0        0    27952 2023-06-01 09:32:54.000000 pyjedai-0.0.6/src/pyjedai/vector_based_blocking.py
+-rw-rw-rw-   0        0        0      955 2022-07-19 14:45:04.000000 pyjedai-0.0.6/src/pyjedai/visualization.py
+-rw-rw-rw-   0        0        0    24786 2023-05-24 13:22:15.000000 pyjedai-0.0.6/src/pyjedai/workflow.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:46.472536 pyjedai-0.0.6/src/pyjedai.egg-info/
+-rw-rw-rw-   0        0        0     7197 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      428 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/top_level.txt
```

### Comparing `pyjedai-0.0.5/LICENSE` & `pyjedai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/PKG-INFO` & `pyjedai-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyjedai
-Version: 0.0.5
+Version: 0.0.6
 Summary: An open-source library that builds powerful end-to-end Entity Resolution workflows.
 Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>
 License: Apache Software License 2.0
-Project-URL: Homepage, https://github.com/AI-team-UoA/pyJedAI
-Project-URL: Documentation, https://github.com/AI-team-UoA/pyJedAI/wiki
+Project-URL: Homepage, http://pyjedai.rtfd.io
+Project-URL: Documentation, http://pyjedai.rtfd.io
 Project-URL: Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues
 Project-URL: Source code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai
 Keywords: deduplication,entity-resolution,link-discovery
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -119,15 +119,15 @@
 
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Team & Authors
 
-<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
+<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="250"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
 - Jakub Maciejewski
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: pyjedai Version: 0.0.5 Summary: An open-source
+Metadata-Version: 2.1 Name: pyjedai Version: 0.0.6 Summary: An open-source
 library that builds powerful end-to-end Entity Resolution workflows. Author-
 email: Konstantinos Nikoletos
 kon@gmail.com>, George Papadakis
-gmail.com> License: Apache Software License 2.0 Project-URL: Homepage, https://
-github.com/AI-team-UoA/pyJedAI Project-URL: Documentation, https://github.com/
-AI-team-UoA/pyJedAI/wiki Project-URL: Bug Tracker, https://github.com/AI-team-
-UoA/pyJedAI/issues Project-URL: Source code, https://github.com/AI-team-UoA/
-pyJedAI/tree/main/pyjedai Keywords: deduplication,entity-resolution,link-
-discovery Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: Implementation Classifier: Intended Audience
-:: Information Technology Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers Classifier: Natural Language ::
-English Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: Unix Classifier: Operating System :: iOS Classifier: Topic
-:: Database Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE
+gmail.com> License: Apache Software License 2.0 Project-URL: Homepage, http://
+pyjedai.rtfd.io Project-URL: Documentation, http://pyjedai.rtfd.io Project-URL:
+Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues Project-URL: Source
+code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai Keywords:
+deduplication,entity-resolution,link-discovery Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
+Implementation Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Developers Classifier: Natural Language :: English Classifier: Operating
+System :: Microsoft :: Windows Classifier: Operating System :: Unix Classifier:
+Operating System :: iOS Classifier: Topic :: Database Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
```

### Comparing `pyjedai-0.0.5/README.md` & `pyjedai-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Team & Authors
 
-<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
+<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="250"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
 - Jakub Maciejewski
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
```

### Comparing `pyjedai-0.0.5/pyproject.toml` & `pyjedai-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyjedai"
-version = "0.0.5"
+version = "0.0.6"
 description = "An open-source library that builds powerful end-to-end Entity Resolution workflows."
 readme = "README.md"
 authors = [
     { name = "Konstantinos Nikoletos", email = "nikoletos.kon@gmail.com" },
     { name = "George Papadakis", email = "gpapadis84@gmail.com" },
 ]
 license = {text = "Apache Software License 2.0"}
@@ -55,18 +55,19 @@
     "strsim >= 0.0.3",
     "strsimpy >= 0.2.1",
     "tqdm >= 4.64",
     "transformers >= 4.21",
     "sentence-transformers >= 2.2",
     "faiss-cpu >= 1.7",
     "optuna >= 3.0",
-    'tomli; python_version < "3.11"'
+    'tomli; python_version < "3.11"', 
+    "py-stringmatching >= 0.4"
 ]
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest"]
 
 [project.urls]
-"Homepage" = "https://github.com/AI-team-UoA/pyJedAI"
-"Documentation" = "https://github.com/AI-team-UoA/pyJedAI/wiki"
+"Homepage" = "http://pyjedai.rtfd.io"
+"Documentation" = "http://pyjedai.rtfd.io"
 "Bug Tracker" = "https://github.com/AI-team-UoA/pyJedAI/issues"
 "Source code" = "https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai"
```

### Comparing `pyjedai-0.0.5/src/pyjedai/block_building.py` & `pyjedai-0.0.6/src/pyjedai/block_building.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/block_cleaning.py` & `pyjedai-0.0.6/src/pyjedai/block_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/clustering.py` & `pyjedai-0.0.6/src/pyjedai/clustering.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/comparison_cleaning.py` & `pyjedai-0.0.6/src/pyjedai/comparison_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/datamodel.py` & `pyjedai-0.0.6/src/pyjedai/datamodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,23 +121,26 @@
                 if self.id_column_name_1 in self.attributes_1:
                     self.attributes_1.remove(self.id_column_name_1)
             else:
                 raise AttributeError(
                     "Dataset 1 must contain column names if attributes_1 is empty.")
         else:
             self.attributes_1: list = attributes_1
+
         if dataset_2 is not None:
-            if dataset_2.columns.values.tolist():
-                self.attributes_2 = dataset_2.columns.values.tolist()
-                if self.id_column_name_2 in self.attributes_2:
-                    self.attributes_2.remove(self.id_column_name_1)
+
+            if attributes_2 is None:
+                if dataset_2.columns.values.tolist():
+                    self.attributes_2 = dataset_2.columns.values.tolist()
+                    if self.id_column_name_2 in self.attributes_2:
+                        self.attributes_2.remove(self.id_column_name_1)
+                else:
+                    raise AttributeError("Dataset 2 must contain column names if attributes_2 is empty.")
             else:
-                raise AttributeError("Dataset 2 must contain column names if attributes_2 is empty.")
-        else:
-            self.attributes_2: list = attributes_2
+                self.attributes_2: list = attributes_2
 
         # Ground truth data
         if ground_truth is not None:
             self.ground_truth = ground_truth.astype(str)
             self._ids_mapping_1: dict
             self._gt_to_ids_reversed_1: dict
             self._ids_mapping_2: dict
```

### Comparing `pyjedai-0.0.5/src/pyjedai/evaluation.py` & `pyjedai-0.0.6/src/pyjedai/evaluation.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/joins.py` & `pyjedai-0.0.6/src/pyjedai/joins.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/logs.py` & `pyjedai-0.0.6/src/pyjedai/logs.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/matching.py` & `pyjedai-0.0.6/src/pyjedai/matching.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/utils.py` & `pyjedai-0.0.6/src/pyjedai/utils.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/vector_based_blocking.py` & `pyjedai-0.0.6/src/pyjedai/vector_based_blocking.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
             = data, attributes_1, attributes_2, vector_size, num_of_clusters, top_k
         self._progress_bar = tqdm(total=data.num_of_entities,
                                   desc=(self._method_name + ' [' + self.vectorizer + ', ' + self.similarity_search + ']'),
                                   disable=tqdm_disable)
 
         self._si = SubsetIndexer(None, self.data)
         
+        # print(data.attributes_1, data.attributes_2)
         self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
                             .apply(" ".join, axis=1) \
                             .apply(self._tokenize_entity) \
                             .values.tolist()
         
         self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
                     .apply(" ".join, axis=1) \
@@ -288,15 +289,19 @@
         for entity in entities:
             encoded_input = tokenizer(entity,
                                         return_tensors='pt',
                                         truncation=True,
                                         return_attention_mask = True,
                                         max_length=self.max_word_embeddings_size,
                                         padding='max_length')
+
+            encoded_input = {key: value.to(self.device) for key, value in encoded_input.items()}  # Move input tensors to GPU
+
             with torch.no_grad():
+                encoded_input = {key: value.to(self.device) for key, value in encoded_input.items()}  # Move input tensors to GPU
                 output = model(**encoded_input)
                 vector = output.last_hidden_state[:, 0, :]
                 
             vector = vector.cpu().numpy()
             embeddings.append(vector.reshape(-1))
             self._progress_bar.update(1)
```

### Comparing `pyjedai-0.0.5/src/pyjedai/visualization.py` & `pyjedai-0.0.6/src/pyjedai/visualization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai/workflow.py` & `pyjedai-0.0.6/src/pyjedai/workflow.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.5/src/pyjedai.egg-info/PKG-INFO` & `pyjedai-0.0.6/src/pyjedai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyjedai
-Version: 0.0.5
+Version: 0.0.6
 Summary: An open-source library that builds powerful end-to-end Entity Resolution workflows.
 Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>
 License: Apache Software License 2.0
-Project-URL: Homepage, https://github.com/AI-team-UoA/pyJedAI
-Project-URL: Documentation, https://github.com/AI-team-UoA/pyJedAI/wiki
+Project-URL: Homepage, http://pyjedai.rtfd.io
+Project-URL: Documentation, http://pyjedai.rtfd.io
 Project-URL: Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues
 Project-URL: Source code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai
 Keywords: deduplication,entity-resolution,link-discovery
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -119,15 +119,15 @@
 
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Team & Authors
 
-<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
+<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="250"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
 - Jakub Maciejewski
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: pyjedai Version: 0.0.5 Summary: An open-source
+Metadata-Version: 2.1 Name: pyjedai Version: 0.0.6 Summary: An open-source
 library that builds powerful end-to-end Entity Resolution workflows. Author-
 email: Konstantinos Nikoletos
 kon@gmail.com>, George Papadakis
-gmail.com> License: Apache Software License 2.0 Project-URL: Homepage, https://
-github.com/AI-team-UoA/pyJedAI Project-URL: Documentation, https://github.com/
-AI-team-UoA/pyJedAI/wiki Project-URL: Bug Tracker, https://github.com/AI-team-
-UoA/pyJedAI/issues Project-URL: Source code, https://github.com/AI-team-UoA/
-pyJedAI/tree/main/pyjedai Keywords: deduplication,entity-resolution,link-
-discovery Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: Implementation Classifier: Intended Audience
-:: Information Technology Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers Classifier: Natural Language ::
-English Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: Unix Classifier: Operating System :: iOS Classifier: Topic
-:: Database Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE
+gmail.com> License: Apache Software License 2.0 Project-URL: Homepage, http://
+pyjedai.rtfd.io Project-URL: Documentation, http://pyjedai.rtfd.io Project-URL:
+Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues Project-URL: Source
+code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai Keywords:
+deduplication,entity-resolution,link-discovery Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
+Implementation Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Developers Classifier: Natural Language :: English Classifier: Operating
+System :: Microsoft :: Windows Classifier: Operating System :: Unix Classifier:
+Operating System :: iOS Classifier: Topic :: Database Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
```

### Comparing `pyjedai-0.0.5/src/pyjedai.egg-info/SOURCES.txt` & `pyjedai-0.0.6/src/pyjedai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

