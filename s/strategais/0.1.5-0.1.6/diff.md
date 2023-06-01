# Comparing `tmp/strategais-0.1.5.tar.gz` & `tmp/strategais-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.1.5.tar", last modified: Thu Jun  1 02:17:58 2023, max compression
+gzip compressed data, was "strategais-0.1.6.tar", last modified: Thu Jun  1 02:32:14 2023, max compression
```

## Comparing `strategais-0.1.5.tar` & `strategais-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 02:17:58.813085 strategais-0.1.5/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.5/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 02:17:58.812946 strategais-0.1.5/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.5/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 02:17:58.813126 strategais-0.1.5/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1431 2023-06-01 02:16:50.000000 strategais-0.1.5/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 02:17:58.811757 strategais-0.1.5/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       53 2023-05-28 04:49:57.000000 strategais-0.1.5/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     3027 2023-06-01 02:16:27.000000 strategais-0.1.5/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.5/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.5/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 02:17:58.812729 strategais-0.1.5/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 02:17:58.000000 strategais-0.1.5/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      290 2023-06-01 02:17:58.000000 strategais-0.1.5/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 02:17:58.000000 strategais-0.1.5/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 02:17:58.000000 strategais-0.1.5/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 02:17:58.000000 strategais-0.1.5/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 02:32:14.432004 strategais-0.1.6/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.6/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 02:32:14.431730 strategais-0.1.6/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.6/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 02:32:14.432064 strategais-0.1.6/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1431 2023-06-01 02:31:04.000000 strategais-0.1.6/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 02:32:14.430000 strategais-0.1.6/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       53 2023-05-28 04:49:57.000000 strategais-0.1.6/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     3292 2023-06-01 02:30:40.000000 strategais-0.1.6/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.6/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.6/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 02:32:14.431347 strategais-0.1.6/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 02:32:14.000000 strategais-0.1.6/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      290 2023-06-01 02:32:14.000000 strategais-0.1.6/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 02:32:14.000000 strategais-0.1.6/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 02:32:14.000000 strategais-0.1.6/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 02:32:14.000000 strategais-0.1.6/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.1.5/LICENSE` & `strategais-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.1.5/PKG-INFO` & `strategais-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

### Comparing `strategais-0.1.5/README.md` & `strategais-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `strategais-0.1.5/setup.py` & `strategais-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.1.5', 
+    version='0.1.6', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     install_requires=[
         'fastapi',
         'fastapi_utils',
```

### Comparing `strategais-0.1.5/strategais/__main__.py` & `strategais-0.1.6/strategais/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,21 +74,27 @@
 server.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"], )
 
-@server.get("/keepalive")
+@server.get("/keepalive",
+            tags=['Keep Alive API'],
+            summary="Keep Alive API",
+            description="Returns the server timestamp.")
 def keepalive_get():
     import datetime
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     return {'timestamp': timestamp}
     
-@server.get("/chat")
+@server.get("/chat",
+            tags=['Chat API'],
+            summary="Chat API",
+            description="Returns the chat response to the question.")
 def chat_get(question: str = 'Hello World?'):
     return {"answer": chatbot(question)}
 
 @server.websocket("/chat/ws")
 async def chat_endpoint(websocket: WebSocket):
     await websocket.accept()
     while True:
```

### Comparing `strategais-0.1.5/strategais/save_tools.py` & `strategais-0.1.6/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.1.5/strategais.egg-info/PKG-INFO` & `strategais-0.1.6/strategais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

