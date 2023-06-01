# Comparing `tmp/strategais-0.2.3.tar.gz` & `tmp/strategais-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.2.3.tar", last modified: Thu Jun  1 20:36:20 2023, max compression
+gzip compressed data, was "strategais-0.2.4.tar", last modified: Thu Jun  1 21:29:02 2023, max compression
```

## Comparing `strategais-0.2.3.tar` & `strategais-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:36:20.607353 strategais-0.2.3/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.3/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1308 2023-06-01 20:36:20.605756 strategais-0.2.3/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1099 2023-06-01 19:57:37.000000 strategais-0.2.3/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 20:36:20.607500 strategais-0.2.3/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1351 2023-06-01 20:35:13.000000 strategais-0.2.3/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:36:20.602594 strategais-0.2.3/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.3/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     4331 2023-06-01 19:55:34.000000 strategais-0.2.3/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.3/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.3/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:36:20.604864 strategais-0.2.3/strategais/templates/
--rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.3/strategais/templates/index.html
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 20:36:20.604486 strategais-0.2.3/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1308 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      425 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 20:36:20.000000 strategais-0.2.3/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 21:29:02.971056 strategais-0.2.4/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.4/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-01 21:29:02.970909 strategais-0.2.4/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1096 2023-06-01 21:27:39.000000 strategais-0.2.4/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 21:29:02.971098 strategais-0.2.4/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1411 2023-06-01 21:04:47.000000 strategais-0.2.4/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 21:29:02.968614 strategais-0.2.4/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.4/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     4326 2023-06-01 21:26:59.000000 strategais-0.2.4/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.4/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.4/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 21:29:02.970425 strategais-0.2.4/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.4/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 21:29:02.970294 strategais-0.2.4/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-01 21:29:02.000000 strategais-0.2.4/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 21:29:02.000000 strategais-0.2.4/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 21:29:02.000000 strategais-0.2.4/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      463 2023-06-01 21:29:02.000000 strategais-0.2.4/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 21:29:02.000000 strategais-0.2.4/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.2.3/LICENSE` & `strategais-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.2.3/PKG-INFO` & `strategais-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.3
+Version: 0.2.4
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
-| -h | --html | 'path/to/other.html' | The path to the HTML file to use. |
+| | --html | 'path/to/other.html' | The path to the HTML file to use. |
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

### Comparing `strategais-0.2.3/README.md` & `strategais-0.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
 | -p | --port | 8000 | The port to serve the server on. |
 | -e | --env | 'main.env' | The .env file to load. |
 | -l | --llm | 'path/hfagent_llm.py' | The path to the Python file that defines the LLM to use. |
-| -h | --html | 'path/to/other.html' | The path to the HTML file to use. |
+| | --html | 'path/to/other.html' | The path to the HTML file to use. |
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

### Comparing `strategais-0.2.3/setup.py` & `strategais-0.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.2.3', 
+    version='0.2.4', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     package_data={'strategais': ['templates/*.html']},
     install_requires=[
         'fastapi',
@@ -46,11 +46,13 @@
         'datasets', 
         'loralib', 
         'sentencepiece', 
         'transformers',
         'pytorch-lightning',
         'torch',
         'accelerate',
-        'torchaudio'
+        'torchaudio',
+        'cryptography==38.0.4',
+        'xformers==0.0.12'
     ],
 )
```

### Comparing `strategais-0.2.3/strategais/__main__.py` & `strategais-0.2.4/strategais/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 parser = argparse.ArgumentParser(description='Start a Strategais FastAPI server.')
 parser.add_argument('-t', '--title', default='Strategais Server', help='The title of the server.')
 parser.add_argument('-d', '--description', default='Strategais Server', help='The description of the server.')
 parser.add_argument('-p', '--port', type=int, default=8000, help='The port to serve the server on.')
 parser.add_argument('-e', '--env', default='main.env', help='The .env file to load.')
 parser.add_argument('-l', '--llm', help='The path to the Python file that defines the LLM to use.')
-parser.add_argument('-h','--html', help='The path to the HTML file to use.')
+parser.add_argument('--html', help='The path to the HTML file to use.')
 
 args = parser.parse_args()
 
 load_dotenv(args.env)
 
 from huggingface_hub import login
 login(os.getenv('HUGGINGFACEHUB_API_TOKEN'))
```

### Comparing `strategais-0.2.3/strategais/save_tools.py` & `strategais-0.2.4/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.2.3/strategais/templates/index.html` & `strategais-0.2.4/strategais/templates/index.html`

 * *Files identical despite different names*

### Comparing `strategais-0.2.3/strategais.egg-info/PKG-INFO` & `strategais-0.2.4/strategais.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.3
+Version: 0.2.4
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
-| -h | --html | 'path/to/other.html' | The path to the HTML file to use. |
+| | --html | 'path/to/other.html' | The path to the HTML file to use. |
 
 ## 🤔 What is this?
 
 Strategais is a powerful Python library designed to streamline the deployment of web applications powered by Large Language Models (LLMs). This library is built with the developer in mind, providing a suite of tools and utilities that simplify the process of setting up, developing, and deploying LLM-based web applications in a local environment or airgapped environment.
```

