# Comparing `tmp/strategais-0.1.2.tar.gz` & `tmp/strategais-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.1.2.tar", last modified: Thu Jun  1 01:43:02 2023, max compression
+gzip compressed data, was "strategais-0.1.3.tar", last modified: Thu Jun  1 01:53:41 2023, max compression
```

## Comparing `strategais-0.1.2.tar` & `strategais-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 01:43:02.484635 strategais-0.1.2/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.2/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 01:43:02.484462 strategais-0.1.2/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.2/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 01:43:02.484679 strategais-0.1.2/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1387 2023-06-01 01:41:47.000000 strategais-0.1.2/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 01:43:02.483334 strategais-0.1.2/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       53 2023-05-28 04:49:57.000000 strategais-0.1.2/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     2936 2023-06-01 01:31:49.000000 strategais-0.1.2/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.2/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.2/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 01:43:02.484231 strategais-0.1.2/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 01:43:02.000000 strategais-0.1.2/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      290 2023-06-01 01:43:02.000000 strategais-0.1.2/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 01:43:02.000000 strategais-0.1.2/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      472 2023-06-01 01:43:02.000000 strategais-0.1.2/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 01:43:02.000000 strategais-0.1.2/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 01:53:41.644151 strategais-0.1.3/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.3/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 01:53:41.643977 strategais-0.1.3/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.3/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 01:53:41.644196 strategais-0.1.3/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1387 2023-06-01 01:52:49.000000 strategais-0.1.3/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 01:53:41.642701 strategais-0.1.3/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       53 2023-05-28 04:49:57.000000 strategais-0.1.3/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     3031 2023-06-01 01:48:20.000000 strategais-0.1.3/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.3/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.3/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 01:53:41.643584 strategais-0.1.3/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 01:53:41.000000 strategais-0.1.3/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      290 2023-06-01 01:53:41.000000 strategais-0.1.3/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 01:53:41.000000 strategais-0.1.3/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      472 2023-06-01 01:53:41.000000 strategais-0.1.3/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 01:53:41.000000 strategais-0.1.3/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.1.2/LICENSE` & `strategais-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.1.2/PKG-INFO` & `strategais-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

### Comparing `strategais-0.1.2/README.md` & `strategais-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `strategais-0.1.2/setup.py` & `strategais-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.1.2', 
+    version='0.1.3', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     install_requires=[
         'fastapi',
         'fastapi_utils',
```

### Comparing `strategais-0.1.2/strategais/__main__.py` & `strategais-0.1.3/strategais/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 if args.llm:
     spec = importlib.util.spec_from_file_location("llm", args.llm)
     llm_module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(llm_module)
     chatbot = llm_module.main_chat()
 else:
     def main_chat(question):
+        from huggingface_hub import login
+        login(os.getenv('HUGGINGFACEHUB_API_TOKEN'))
         from transformers.tools import HfAgent
         agent = HfAgent("https://api-inference.huggingface.co/models/bigcode/starcoder")
         return agent.chat(question)
     
     chatbot = main_chat
 
 server = FastAPI(
```

### Comparing `strategais-0.1.2/strategais/save_tools.py` & `strategais-0.1.3/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.1.2/strategais.egg-info/PKG-INFO` & `strategais-0.1.3/strategais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

