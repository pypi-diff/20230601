# Comparing `tmp/strategais-0.1.9.tar.gz` & `tmp/strategais-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.1.9.tar", last modified: Thu Jun  1 03:45:09 2023, max compression
+gzip compressed data, was "strategais-0.2.0.tar", last modified: Thu Jun  1 19:32:16 2023, max compression
```

## Comparing `strategais-0.1.9.tar` & `strategais-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:45:09.969594 strategais-0.1.9/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.1.9/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:45:09.969451 strategais-0.1.9/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1024 2023-05-31 23:04:48.000000 strategais-0.1.9/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 03:45:09.969635 strategais-0.1.9/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1486 2023-06-01 03:44:02.000000 strategais-0.1.9/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:45:09.967919 strategais-0.1.9/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.1.9/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     3757 2023-06-01 03:43:54.000000 strategais-0.1.9/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.1.9/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.1.9/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:45:09.968867 strategais-0.1.9/strategais/templates/
--rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.1.9/strategais/templates/index.html
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 03:45:09.968753 strategais-0.1.9/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1233 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 03:45:09.000000 strategais-0.1.9/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 19:32:16.769478 strategais-0.2.0/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.0/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1234 2023-06-01 19:32:16.769331 strategais-0.2.0/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1025 2023-06-01 16:15:47.000000 strategais-0.2.0/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 19:32:16.769521 strategais-0.2.0/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1486 2023-06-01 16:20:14.000000 strategais-0.2.0/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 19:32:16.767652 strategais-0.2.0/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.0/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     3971 2023-06-01 16:19:04.000000 strategais-0.2.0/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.0/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.0/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 19:32:16.768777 strategais-0.2.0/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.0/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 19:32:16.768625 strategais-0.2.0/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1234 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.1.9/LICENSE` & `strategais-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.1.9/PKG-INFO` & `strategais-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
@@ -19,14 +19,14 @@
 
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
 | -p | --port | 8000 | The port to serve the server on. |
 | -e | --env | 'main.env' | The .env file to load. |
-| -l | --llm | 'path/hfagen_llm.py' | The path to the Python file that defines the LLM to use. |
+| -l | --llm | 'path/hfagent_llm.py' | The path to the Python file that defines the LLM to use. |
 
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

### Comparing `strategais-0.1.9/README.md` & `strategais-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
 | -p | --port | 8000 | The port to serve the server on. |
 | -e | --env | 'main.env' | The .env file to load. |
-| -l | --llm | 'path/hfagen_llm.py' | The path to the Python file that defines the LLM to use. |
+| -l | --llm | 'path/hfagent_llm.py' | The path to the Python file that defines the LLM to use. |
 
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

### Comparing `strategais-0.1.9/setup.py` & `strategais-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.1.9', 
+    version='0.2.0', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     package_data={'strategais': ['templates/*.html']},
     install_requires=[
         'fastapi',
```

### Comparing `strategais-0.1.9/strategais/__main__.py` & `strategais-0.2.0/strategais/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .llm_tools import *
 import json
 import asyncio
 import uvicorn
 
 from fastapi import FastAPI, Request, WebSocket  # ,Response, Body, Form,
 from fastapi.middleware.cors import CORSMiddleware
-from fastapi.responses import HTMLResponse
+from fastapi.responses import HTMLResponse, RedirectResponse
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from fastapi.openapi.docs import (
     get_redoc_html,
     get_swagger_ui_html,
     get_swagger_ui_oauth2_redirect_html,
 )
@@ -74,25 +74,33 @@
 server.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"], )
 
+
+@server.get("/",
+            tags=['Chat'],
+            summary="Chat API",
+            description="Returns the chat response to the question.")
+def root():
+    return RedirectResponse(url='/docs')
+
 @server.get("/keepalive",
             tags=['Keep Alive API'],
             summary="Keep Alive API",
             description="Returns the server timestamp.")
 def keepalive_get():
     import datetime
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     return {'timestamp': timestamp}
     
-@server.get("/chat",
-            tags=['Chat API'],
+@server.get("/chat/api",
+            tags=['Chat'],
             summary="Chat API",
             description="Returns the chat response to the question.")
 def chat_get(question: str = 'Hello World?'):
     return {"answer": chatbot(question)}
 
 @server.websocket("/chat/ws")
 async def chat_endpoint(websocket: WebSocket):
@@ -100,23 +108,21 @@
     while True:
         question = await websocket.receive_text()
         await websocket.send_text(chatbot(question))
 
 import urllib3
 urllib3.disable_warnings()
 
-
 import pkg_resources
 
 template_path = pkg_resources.resource_filename('strategais', 'templates')
 templates = Jinja2Templates(directory=template_path)
 
-
-@server.get("/", response_class=HTMLResponse,
-            tags=['Landing API'],
+@server.get("/chat", response_class=HTMLResponse,
+            tags=['Chat'],
             summary="Chat Home Page",
             description="Chat Home Page")
 def index_html(request: Request):
     return templates.TemplateResponse("index.html", {"request": request})
 
 if __name__ == "__main__":
     uvicorn.run(server, host="0.0.0.0", port=args.port, log_level="info")
```

### Comparing `strategais-0.1.9/strategais/save_tools.py` & `strategais-0.2.0/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.1.9/strategais/templates/index.html` & `strategais-0.2.0/strategais/templates/index.html`

 * *Files identical despite different names*

### Comparing `strategais-0.1.9/strategais.egg-info/PKG-INFO` & `strategais-0.2.0/strategais.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
@@ -19,14 +19,14 @@
 
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
 | -p | --port | 8000 | The port to serve the server on. |
 | -e | --env | 'main.env' | The .env file to load. |
-| -l | --llm | 'path/hfagen_llm.py' | The path to the Python file that defines the LLM to use. |
+| -l | --llm | 'path/hfagent_llm.py' | The path to the Python file that defines the LLM to use. |
 
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

