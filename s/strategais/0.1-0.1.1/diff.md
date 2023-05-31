# Comparing `tmp/strategais-0.1.tar.gz` & `tmp/strategais-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.1.tar", last modified: Wed May 31 23:10:10 2023, max compression
+gzip compressed data, was "strategais-0.1.1.tar", last modified: Wed May 31 23:39:17 2023, max compression
```

## Comparing `strategais-0.1.tar` & `strategais-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-05-31 23:10:10.397839 strategais-0.1/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1139 2023-05-31 23:10:10.397564 strategais-0.1/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-05-31 23:10:10.397891 strategais-0.1/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1283 2023-05-31 23:07:26.000000 strategais-0.1/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-05-31 23:10:10.395841 strategais-0.1/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       53 2023-05-28 04:49:57.000000 strategais-0.1/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     2958 2023-05-31 22:58:57.000000 strategais-0.1/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-05-31 23:10:10.397173 strategais-0.1/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1139 2023-05-31 23:10:10.000000 strategais-0.1/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      290 2023-05-31 23:10:10.000000 strategais-0.1/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-05-31 23:10:10.000000 strategais-0.1/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      472 2023-05-31 23:10:10.000000 strategais-0.1/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-05-31 23:10:10.000000 strategais-0.1/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-05-31 23:39:17.978816 strategais-0.1.1/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.1/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-05-31 23:39:17.978588 strategais-0.1.1/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.1/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-05-31 23:39:17.978873 strategais-0.1.1/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1387 2023-05-31 23:34:58.000000 strategais-0.1.1/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-05-31 23:39:17.977455 strategais-0.1.1/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       53 2023-05-28 04:49:57.000000 strategais-0.1.1/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     2958 2023-05-31 22:58:57.000000 strategais-0.1.1/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.1/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.1/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-05-31 23:39:17.978386 strategais-0.1.1/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-05-31 23:39:17.000000 strategais-0.1.1/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      290 2023-05-31 23:39:17.000000 strategais-0.1.1/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-05-31 23:39:17.000000 strategais-0.1.1/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      472 2023-05-31 23:39:17.000000 strategais-0.1.1/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-05-31 23:39:17.000000 strategais-0.1.1/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.1/LICENSE` & `strategais-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.1/PKG-INFO` & `strategais-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1
+Version: 0.1.1
+Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

### Comparing `strategais-0.1/README.md` & `strategais-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `strategais-0.1/setup.py` & `strategais-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.1', 
+    version='0.1.1', 
+    description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     install_requires=[
         'fastapi',
         'fastapi_utils',
         'uvicorn',
```

### Comparing `strategais-0.1/strategais/__main__.py` & `strategais-0.1.1/strategais/__main__.py`

 * *Files identical despite different names*

### Comparing `strategais-0.1/strategais/save_tools.py` & `strategais-0.1.1/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.1/strategais.egg-info/PKG-INFO` & `strategais-0.1.1/strategais.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1
+Version: 0.1.1
+Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

