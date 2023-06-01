# Comparing `tmp/strategais-0.1.8.tar.gz` & `tmp/strategais-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.1.8.tar", last modified: Thu Jun  1 03:41:32 2023, max compression
+gzip compressed data, was "strategais-0.1.9.tar", last modified: Thu Jun  1 03:45:09 2023, max compression
```

## Comparing `strategais-0.1.8.tar` & `strategais-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:41:32.363581 strategais-0.1.8/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.8/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:41:32.363446 strategais-0.1.8/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.8/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 03:41:32.363625 strategais-0.1.8/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1486 2023-06-01 03:40:07.000000 strategais-0.1.8/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:41:32.361438 strategais-0.1.8/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       97 2023-06-01 03:29:02.000000 strategais-0.1.8/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     3757 2023-06-01 03:36:17.000000 strategais-0.1.8/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.8/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.8/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:41:32.362795 strategais-0.1.8/strategais/templates/
--rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.1.8/strategais/templates/index.html
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:41:32.362588 strategais-0.1.8/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:45:09.969594 strategais-0.1.9/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.9/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:45:09.969451 strategais-0.1.9/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.9/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 03:45:09.969635 strategais-0.1.9/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1486 2023-06-01 03:44:02.000000 strategais-0.1.9/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:45:09.967919 strategais-0.1.9/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.1.9/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     3757 2023-06-01 03:43:54.000000 strategais-0.1.9/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.9/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.9/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:45:09.968867 strategais-0.1.9/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.1.9/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:45:09.968753 strategais-0.1.9/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.1.8/LICENSE` & `strategais-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.1.8/PKG-INFO` & `strategais-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

### Comparing `strategais-0.1.8/README.md` & `strategais-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `strategais-0.1.8/setup.py` & `strategais-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.1.8', 
+    version='0.1.9', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     package_data={'strategais': ['templates/*.html']},
     install_requires=[
         'fastapi',
```

### Comparing `strategais-0.1.8/strategais/__main__.py` & `strategais-0.1.9/strategais/__main__.py`

 * *Files identical despite different names*

### Comparing `strategais-0.1.8/strategais/save_tools.py` & `strategais-0.1.9/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.1.8/strategais/templates/index.html` & `strategais-0.1.9/strategais/templates/index.html`

 * *Files identical despite different names*

### Comparing `strategais-0.1.8/strategais.egg-info/PKG-INFO` & `strategais-0.1.9/strategais.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

