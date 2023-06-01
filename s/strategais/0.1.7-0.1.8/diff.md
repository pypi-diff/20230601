# Comparing `tmp/strategais-0.1.7.tar.gz` & `tmp/strategais-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.1.7.tar", last modified: Thu Jun  1 03:20:55 2023, max compression
+gzip compressed data, was "strategais-0.1.8.tar", last modified: Thu Jun  1 03:41:32 2023, max compression
```

## Comparing `strategais-0.1.7.tar` & `strategais-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:20:55.492372 strategais-0.1.7/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.7/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:20:55.492236 strategais-0.1.7/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.7/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 03:20:55.492413 strategais-0.1.7/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1431 2023-06-01 03:19:27.000000 strategais-0.1.7/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:20:55.491155 strategais-0.1.7/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:12:33.000000 strategais-0.1.7/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     3648 2023-06-01 03:09:11.000000 strategais-0.1.7/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.7/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.7/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:20:55.492073 strategais-0.1.7/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:20:55.000000 strategais-0.1.7/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      290 2023-06-01 03:20:55.000000 strategais-0.1.7/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 03:20:55.000000 strategais-0.1.7/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 03:20:55.000000 strategais-0.1.7/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 03:20:55.000000 strategais-0.1.7/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:41:32.363581 strategais-0.1.8/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.8/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:41:32.363446 strategais-0.1.8/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.8/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 03:41:32.363625 strategais-0.1.8/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1486 2023-06-01 03:40:07.000000 strategais-0.1.8/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:41:32.361438 strategais-0.1.8/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       97 2023-06-01 03:29:02.000000 strategais-0.1.8/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     3757 2023-06-01 03:36:17.000000 strategais-0.1.8/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.8/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.8/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:41:32.362795 strategais-0.1.8/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.1.8/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:41:32.362588 strategais-0.1.8/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 03:41:32.000000 strategais-0.1.8/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.1.7/LICENSE` & `strategais-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.1.7/PKG-INFO` & `strategais-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

### Comparing `strategais-0.1.7/README.md` & `strategais-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `strategais-0.1.7/setup.py` & `strategais-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.1.7', 
+    version='0.1.8', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
+    package_data={'strategais': ['templates/*.html']},
     install_requires=[
         'fastapi',
         'fastapi_utils',
         'uvicorn',
         'starlette',
         'websockets',
         'flask',
```

### Comparing `strategais-0.1.7/strategais/__main__.py` & `strategais-0.1.8/strategais/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,15 +100,20 @@
     while True:
         question = await websocket.receive_text()
         await websocket.send_text(chatbot(question))
 
 import urllib3
 urllib3.disable_warnings()
 
-templates = Jinja2Templates(directory=".")
+
+import pkg_resources
+
+template_path = pkg_resources.resource_filename('strategais', 'templates')
+templates = Jinja2Templates(directory=template_path)
+
 
 @server.get("/", response_class=HTMLResponse,
             tags=['Landing API'],
             summary="Chat Home Page",
             description="Chat Home Page")
 def index_html(request: Request):
     return templates.TemplateResponse("index.html", {"request": request})
```

### Comparing `strategais-0.1.7/strategais/save_tools.py` & `strategais-0.1.8/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.1.7/strategais.egg-info/PKG-INFO` & `strategais-0.1.8/strategais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

