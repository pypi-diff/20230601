# Comparing `tmp/strategais-0.2.0.tar.gz` & `tmp/strategais-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.2.0.tar", last modified: Thu Jun  1 19:32:16 2023, max compression
+gzip compressed data, was "strategais-0.2.1.tar", last modified: Thu Jun  1 20:00:22 2023, max compression
```

## Comparing `strategais-0.2.0.tar` & `strategais-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 19:32:16.769478 strategais-0.2.0/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.0/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1234 2023-06-01 19:32:16.769331 strategais-0.2.0/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1025 2023-06-01 16:15:47.000000 strategais-0.2.0/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 19:32:16.769521 strategais-0.2.0/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1486 2023-06-01 16:20:14.000000 strategais-0.2.0/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 19:32:16.767652 strategais-0.2.0/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.0/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     3971 2023-06-01 16:19:04.000000 strategais-0.2.0/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.0/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.0/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 19:32:16.768777 strategais-0.2.0/strategais/templates/
--rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.0/strategais/templates/index.html
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 19:32:16.768625 strategais-0.2.0/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1234 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 19:32:16.000000 strategais-0.2.0/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:00:22.708879 strategais-0.2.1/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.1/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1308 2023-06-01 20:00:22.708720 strategais-0.2.1/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1099 2023-06-01 19:57:37.000000 strategais-0.2.1/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 20:00:22.708922 strategais-0.2.1/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1486 2023-06-01 19:54:03.000000 strategais-0.2.1/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:00:22.706888 strategais-0.2.1/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.1/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     4331 2023-06-01 19:55:34.000000 strategais-0.2.1/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.1/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.1/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:00:22.708001 strategais-0.2.1/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.1/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:00:22.707871 strategais-0.2.1/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1308 2023-06-01 20:00:22.000000 strategais-0.2.1/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 20:00:22.000000 strategais-0.2.1/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 20:00:22.000000 strategais-0.2.1/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      494 2023-06-01 20:00:22.000000 strategais-0.2.1/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 20:00:22.000000 strategais-0.2.1/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.2.0/LICENSE` & `strategais-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.2.0/PKG-INFO` & `strategais-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
@@ -20,13 +20,13 @@
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
 | -p | --port | 8000 | The port to serve the server on. |
 | -e | --env | 'main.env' | The .env file to load. |
 | -l | --llm | 'path/hfagent_llm.py' | The path to the Python file that defines the LLM to use. |
-
+| -h | --html | 'path/to/other.html' | The path to the HTML file to use. |
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

### Comparing `strategais-0.2.0/README.md` & `strategais-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
 | -p | --port | 8000 | The port to serve the server on. |
 | -e | --env | 'main.env' | The .env file to load. |
 | -l | --llm | 'path/hfagent_llm.py' | The path to the Python file that defines the LLM to use. |
-
+| -h | --html | 'path/to/other.html' | The path to the HTML file to use. |
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

### Comparing `strategais-0.2.0/setup.py` & `strategais-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.2.0', 
+    version='0.2.1', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     package_data={'strategais': ['templates/*.html']},
     install_requires=[
         'fastapi',
```

### Comparing `strategais-0.2.0/strategais/__main__.py` & `strategais-0.2.1/strategais/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 parser = argparse.ArgumentParser(description='Start a Strategais FastAPI server.')
 parser.add_argument('-t', '--title', default='Strategais Server', help='The title of the server.')
 parser.add_argument('-d', '--description', default='Strategais Server', help='The description of the server.')
 parser.add_argument('-p', '--port', type=int, default=8000, help='The port to serve the server on.')
 parser.add_argument('-e', '--env', default='main.env', help='The .env file to load.')
 parser.add_argument('-l', '--llm', help='The path to the Python file that defines the LLM to use.')
+parser.add_argument('-h','--html', help='The path to the HTML file to use.')
 
 args = parser.parse_args()
 
 load_dotenv(args.env)
 
 from huggingface_hub import login
 login(os.getenv('HUGGINGFACEHUB_API_TOKEN'))
@@ -118,11 +119,19 @@
 templates = Jinja2Templates(directory=template_path)
 
 @server.get("/chat", response_class=HTMLResponse,
             tags=['Chat'],
             summary="Chat Home Page",
             description="Chat Home Page")
 def index_html(request: Request):
-    return templates.TemplateResponse("index.html", {"request": request})
+    if args.html:
+        html_dir = os.path.dirname(args.html)
+        html_file = os.path.basename(args.html)
+    else:
+        html_dir = pkg_resources.resource_filename('strategais', 'templates')
+        html_file = 'index.html'
+    templates = Jinja2Templates(directory=html_dir)
+    return templates.TemplateResponse(html_file, {"request": request})
+
 
 if __name__ == "__main__":
     uvicorn.run(server, host="0.0.0.0", port=args.port, log_level="info")
```

### Comparing `strategais-0.2.0/strategais/save_tools.py` & `strategais-0.2.1/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.2.0/strategais/templates/index.html` & `strategais-0.2.1/strategais/templates/index.html`

 * *Files identical despite different names*

### Comparing `strategais-0.2.0/strategais.egg-info/PKG-INFO` & `strategais-0.2.1/strategais.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
@@ -20,13 +20,13 @@
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
 | -p | --port | 8000 | The port to serve the server on. |
 | -e | --env | 'main.env' | The .env file to load. |
 | -l | --llm | 'path/hfagent_llm.py' | The path to the Python file that defines the LLM to use. |
-
+| -h | --html | 'path/to/other.html' | The path to the HTML file to use. |
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

