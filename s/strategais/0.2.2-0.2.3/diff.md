# Comparing `tmp/strategais-0.2.2.tar.gz` & `tmp/strategais-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.2.2.tar", last modified: Thu Jun  1 20:11:38 2023, max compression
+gzip compressed data, was "strategais-0.2.3.tar", last modified: Thu Jun  1 20:36:20 2023, max compression
```

## Comparing `strategais-0.2.2.tar` & `strategais-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:11:38.510134 strategais-0.2.2/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.2/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1308 2023-06-01 20:11:38.509981 strategais-0.2.2/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1099 2023-06-01 19:57:37.000000 strategais-0.2.2/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 20:11:38.510176 strategais-0.2.2/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1506 2023-06-01 20:10:56.000000 strategais-0.2.2/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:11:38.508375 strategais-0.2.2/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.2/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     4331 2023-06-01 19:55:34.000000 strategais-0.2.2/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.2/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.2/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:11:38.509339 strategais-0.2.2/strategais/templates/
--rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.2/strategais/templates/index.html
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:11:38.509215 strategais-0.2.2/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1308 2023-06-01 20:11:38.000000 strategais-0.2.2/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 20:11:38.000000 strategais-0.2.2/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 20:11:38.000000 strategais-0.2.2/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      503 2023-06-01 20:11:38.000000 strategais-0.2.2/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 20:11:38.000000 strategais-0.2.2/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:36:20.607353 strategais-0.2.3/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.3/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1308 2023-06-01 20:36:20.605756 strategais-0.2.3/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1099 2023-06-01 19:57:37.000000 strategais-0.2.3/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 20:36:20.607500 strategais-0.2.3/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1351 2023-06-01 20:35:13.000000 strategais-0.2.3/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:36:20.602594 strategais-0.2.3/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.3/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     4331 2023-06-01 19:55:34.000000 strategais-0.2.3/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.3/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.3/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:36:20.604864 strategais-0.2.3/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.3/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:36:20.604486 strategais-0.2.3/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1308 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      425 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.2.2/LICENSE` & `strategais-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.2.2/PKG-INFO` & `strategais-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

### Comparing `strategais-0.2.2/README.md` & `strategais-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `strategais-0.2.2/setup.py` & `strategais-0.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.2.2', 
+    version='0.2.3', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     package_data={'strategais': ['templates/*.html']},
     install_requires=[
         'fastapi',
@@ -22,42 +22,35 @@
         'pandas',
         'requests',
         'scikit-learn',
         'scipy',
         'SQLAlchemy',
         'pydantic',
         'aiofiles',
-        'openpyxl',
-        'xlrd==1.2.0',
         'psycopg2-binary',
         'watchdog[watchmedo]',
         'email-validator',
         'boto3',
         'jinja2',
         'python-multipart',
         'httpx',
-        'neo4j',
         'sse-starlette',
         'langchain',
         'python-dotenv',
         'openai',
         'huggingface_hub',
         'chromadb',
         'redis',
-        'streamlit',
-        'streamlit-pills==0.3.0',
         'sentence_transformers',
         'unstructured',
         'pydantic',
-        'xformers',
         'datasets', 
         'loralib', 
         'sentencepiece', 
         'transformers',
-        'xformers',
         'pytorch-lightning',
         'torch',
         'accelerate',
         'torchaudio'
     ],
 )
```

### Comparing `strategais-0.2.2/strategais/__main__.py` & `strategais-0.2.3/strategais/__main__.py`

 * *Files identical despite different names*

### Comparing `strategais-0.2.2/strategais/save_tools.py` & `strategais-0.2.3/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.2.2/strategais/templates/index.html` & `strategais-0.2.3/strategais/templates/index.html`

 * *Files identical despite different names*

### Comparing `strategais-0.2.2/strategais.egg-info/PKG-INFO` & `strategais-0.2.3/strategais.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

