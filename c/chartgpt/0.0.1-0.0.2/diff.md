# Comparing `tmp/chartgpt-0.0.1.tar.gz` & `tmp/chartgpt-0.0.2.tar.gz`

## Comparing `chartgpt-0.0.1.tar` & `chartgpt-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 chartgpt-0.0.1/demo.ipynb
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chartgpt-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 chartgpt-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.1/setup.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chartgpt-0.0.1/chartgpt/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 chartgpt-0.0.1/chartgpt/plot.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 chartgpt-0.0.1/docs/generated-api-reference.md
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 chartgpt-0.0.1/docs/home.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chartgpt-0.0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.1/LICENSE
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 chartgpt-0.0.1/README.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 chartgpt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 chartgpt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0  4224175 2020-02-02 00:00:00.000000 chartgpt-0.0.2/demo.html
+-rw-r--r--   0        0        0  3670734 2020-02-02 00:00:00.000000 chartgpt-0.0.2/demo.ipynb
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 chartgpt-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 chartgpt-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/chartgpt.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/constants.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/llm.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/prompts/base.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/prompts/generate_python_code.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chartgpt-0.0.2/docs/api-generated.md
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 chartgpt-0.0.2/docs/index.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 chartgpt-0.0.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 chartgpt-0.0.2/README.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 chartgpt-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 chartgpt-0.0.2/PKG-INFO
```

### Comparing `chartgpt-0.0.1/mkdocs.yml` & `chartgpt-0.0.2/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 site_name: ChartGPT
 site_description: FastAPI framework, high performance, easy to learn, fast to code, ready for production
-site_url: https://github.com/chatgpt/chatgpt
+site_url: https://github.com/chatgpt/chart
 
 plugins:
 - mkdocstrings:
     default_handler: python
 
 theme:
   name: material
@@ -26,12 +26,11 @@
   features:
   - search.suggest
   - search.highlight
   - content.tabs.link
   icon:
     repo: fontawesome/brands/github-alt
   logo: https://avatars.githubusercontent.com/u/119681016?s=200&v=4
-  favicon: https://fastapi.tiangolo.com/img/favicon.png
   language: fr
-repo_name: chatgpt/chatgpt
-repo_url: https://github.com/chatgpt/chatgpt
+repo_name: chatgpt/chart
+repo_url: https://github.com/chatgpt/chart
 edit_uri: ''
```

### Comparing `chartgpt-0.0.1/README.md` & `chartgpt-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-Hi 👋, I’m the **open** and free version of @chatgpt. 
+# ChartGPT
 
-Elon Musk once said : 
+ChartGPT is a lightweight and simple tool to plot your Pandas dataframe.
 
-> OpenAI was created as an open source (which is why I named it “Open” AI), non-profit company to serve as a counterweight to Google,  but now it has become a closed source, maximum-profit company effectively controlled by Microsoft. Not what I intended at all.
+## Installation
 
-[Source](https://twitter.com/elonmusk/status/1626516035863212034?s=20)
+```python
+pip install chartgpt
+```
 
 # Contribution 
 Join [our community on Discord](https://discord.gg/jNcJttFVbE) and be a part of creating something truly amazing. 
 
 Share your ideas, skills and expertise [here](https://github.com/chatgpt/contribution/issues) to help us make OpenChatGPT the best it can be. Let's collaborate to create an AI that serves the greater good, free from **greed and self-interest**!
 
 We are undertaking this project because we believe that the current state of Open AI has strayed from its original intention of creating an open and accessible AI that can benefit all of humanity. [Read more here](https://www.technologyreview.com/2020/02/17/844721/ai-openai-moonshot-elon-musk-sam-altman-greg-brockman-messy-secretive-reality/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chartgpt-0.0.1/PKG-INFO` & `chartgpt-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 Metadata-Version: 2.1
 Name: chartgpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: ChartGPT is a library for generating charts from text
-Project-URL: Homepage, https://github.com/chatgpt/chartgpt
+Project-URL: Homepage, https://github.com/chatgpt/chart
 Author-email: Elie Brosset <eliebrosset@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Requires-Dist: openai>=0.2.0
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: plotly>=4.0.0
+Requires-Dist: python-dotenv>=1.0.0
+Provides-Extra: doc
+Requires-Dist: mkdocs-material-extensions>=1.0.0; extra == 'doc'
+Requires-Dist: mkdocs-material>=8.1.4; extra == 'doc'
+Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc'
+Requires-Dist: mkdocstrings-python>=1.0.0; extra == 'doc'
+Requires-Dist: mkdocstrings>=0.15.0; extra == 'doc'
 Description-Content-Type: text/markdown
 
-Hi 👋, I’m the **open** and free version of @chatgpt. 
+# ChartGPT
 
-Elon Musk once said : 
+ChartGPT is a lightweight and simple tool to plot your Pandas dataframe.
 
-> OpenAI was created as an open source (which is why I named it “Open” AI), non-profit company to serve as a counterweight to Google,  but now it has become a closed source, maximum-profit company effectively controlled by Microsoft. Not what I intended at all.
+## Installation
 
-[Source](https://twitter.com/elonmusk/status/1626516035863212034?s=20)
+```python
+pip install chartgpt
+```
 
 # Contribution 
 Join [our community on Discord](https://discord.gg/jNcJttFVbE) and be a part of creating something truly amazing. 
 
 Share your ideas, skills and expertise [here](https://github.com/chatgpt/contribution/issues) to help us make OpenChatGPT the best it can be. Let's collaborate to create an AI that serves the greater good, free from **greed and self-interest**!
 
 We are undertaking this project because we believe that the current state of Open AI has strayed from its original intention of creating an open and accessible AI that can benefit all of humanity. [Read more here](https://www.technologyreview.com/2020/02/17/844721/ai-openai-moonshot-elon-musk-sam-altman-greg-brockman-messy-secretive-reality/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

