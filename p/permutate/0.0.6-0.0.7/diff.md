# Comparing `tmp/permutate-0.0.6.tar.gz` & `tmp/permutate-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permutate-0.0.6.tar", max compression
+gzip compressed data, was "permutate-0.0.7.tar", max compression
```

## Comparing `permutate-0.0.6.tar` & `permutate-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3697 2023-05-31 17:06:56.759040 permutate-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-05-31 14:00:12.890922 permutate-0.0.6/permutate/__init__.py
--rw-r--r--   0        0        0       48 2023-05-31 17:06:56.770244 permutate-0.0.6/permutate/__main__.py
--rw-r--r--   0        0        0     2311 2023-05-31 17:06:56.770874 permutate-0.0.6/permutate/job_request_schema.py
--rw-r--r--   0        0        0    10079 2023-05-31 17:06:56.771081 permutate-0.0.6/permutate/job_response_schema.py
--rw-r--r--   0        0        0     1153 2023-05-31 17:06:56.771661 permutate-0.0.6/permutate/logger.py
--rw-r--r--   0        0        0     2357 2023-05-31 17:06:56.771839 permutate-0.0.6/permutate/main.py
--rw-r--r--   0        0        0     7498 2023-06-01 15:42:12.502459 permutate-0.0.6/permutate/runner.py
--rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.6/permutate/singleton.py
--rw-r--r--   0        0        0     3436 2023-05-31 17:06:56.772174 permutate-0.0.6/permutate/templates/job_result_template.html
--rw-r--r--   0        0        0     2001 2023-05-31 17:06:56.772299 permutate-0.0.6/permutate/workspace/plugin_test.yaml
--rw-r--r--   0        0        0      750 2023-06-01 15:48:05.529705 permutate-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 permutate-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     8712 2023-06-01 20:24:56.599704 permutate-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 14:00:12.890922 permutate-0.0.7/permutate/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-31 17:06:56.770244 permutate-0.0.7/permutate/__main__.py
+-rw-r--r--   0        0        0     2354 2023-06-01 16:23:45.772329 permutate-0.0.7/permutate/job_request_schema.py
+-rw-r--r--   0        0        0    10079 2023-05-31 17:06:56.771081 permutate-0.0.7/permutate/job_response_schema.py
+-rw-r--r--   0        0        0     1153 2023-05-31 17:06:56.771661 permutate-0.0.7/permutate/logger.py
+-rw-r--r--   0        0        0     2357 2023-05-31 17:06:56.771839 permutate-0.0.7/permutate/main.py
+-rw-r--r--   0        0        0     7518 2023-06-01 19:41:00.861159 permutate-0.0.7/permutate/runner.py
+-rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.7/permutate/singleton.py
+-rw-r--r--   0        0        0     3436 2023-05-31 17:06:56.772174 permutate-0.0.7/permutate/templates/job_result_template.html
+-rw-r--r--   0        0        0     2032 2023-06-01 16:38:51.520700 permutate-0.0.7/permutate/workspace/plugin_test.yaml
+-rw-r--r--   0        0        0      602 2023-06-01 21:33:39.569472 permutate-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     9458 1970-01-01 00:00:00.000000 permutate-0.0.7/PKG-INFO
```

### Comparing `permutate-0.0.6/permutate/job_request_schema.py` & `permutate-0.0.7/permutate/job_request_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     expected_plugin_used: str
     expected_api_used: str
     expected_parameters: Dict[str, str]
     expected_response: str
 
 
 class Config(BaseModel):
+    use_openplugin_library: Optional[bool]
     openai_api_key: Optional[str]
     langchain_tool_selector: Optional[str]
     imprompt_tool_selector: Optional[str]
     auto_translate_to_languages: List[str]
 
 
 class JobRequest(YamlModel):
```

### Comparing `permutate-0.0.6/permutate/job_response_schema.py` & `permutate-0.0.7/permutate/job_response_schema.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.6/permutate/logger.py` & `permutate-0.0.7/permutate/logger.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.6/permutate/main.py` & `permutate-0.0.7/permutate/main.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.6/permutate/runner.py` & `permutate-0.0.7/permutate/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import json
 import requests
 import webbrowser
 from tqdm import tqdm
 from .logger import logger
 from datetime import datetime
+from openplugin import run_plugin_selector
 from .job_request_schema import JobRequest
 from .job_response_schema import JobResponse, JobSummary, JobDetail
-import importlib.util
-
-found_openplugin_lib = importlib.util.find_spec("openplugin") is not None
 
 
 class Runner:
 
     def __init__(self, show_progress_bar: bool = True):
         self.show_progress_bar = show_progress_bar
         if self.show_progress_bar:
@@ -75,18 +73,21 @@
             }],
             "plugins": plugin_group.dict().get("plugins"),
             "config": config.dict(),
             "tool_selector_config": permutation.tool_selector,
             "llm": permutation.llm
         })
         passed = True
-        if found_openplugin_lib:
-            from openplugin import run_plugin_selector
-            response_json = run_plugin_selector(payload)
-            if response_json is None:
+        if config.use_openplugin_library:
+            try:
+                response_json = run_plugin_selector(payload)
+                if response_json is None:
+                    passed = False
+            except Exception as e:
+                print(e)
                 passed = False
         else:
             if permutation.tool_selector.get("provider") == "Imprompt":
                 url = config.imprompt_tool_selector
             elif permutation.tool_selector.get("provider") == "Langchain":
                 url = config.langchain_tool_selector
             else:
```

### Comparing `permutate-0.0.6/permutate/singleton.py` & `permutate-0.0.7/permutate/singleton.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.6/permutate/templates/job_result_template.html` & `permutate-0.0.7/permutate/templates/job_result_template.html`

 * *Files identical despite different names*

### Comparing `permutate-0.0.6/permutate/workspace/plugin_test.yaml` & `permutate-0.0.7/permutate/workspace/plugin_test.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 version: 1.0.0
 name: klarna_plugin_test
 config:
+  use_openplugin_library: true
   langchain_tool_selector: http://localhost:8006/api/langchain/run-plugin
   imprompt_tool_selector: http://localhost:8006/api/imprompt/run-plugin
   auto_translate_to_languages:
     - English
     - Spanish
 test_plugin:
     manifest_url: https://www.klarna.com/.well-known/ai-plugin.json
```

### Comparing `permutate-0.0.6/pyproject.toml` & `permutate-0.0.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 [tool.poetry]
 name = "permutate"
-version = "0.0.6"
+version = "0.0.7"
 description = "Testing framework for LLM Plugins"
 authors = ["shrikant <shrikant.pm14@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "2.29.0"
 pydantic = "^1.10.8"
 pydantic-yaml = "^0.11.2"
 tqdm = "^4.65.0"
 pyyaml = "^6.0"
 typer = { extras = ["all"], version = "^0.9.0" }
 jinja2 = "^3.1.2"
-openplugin = { version = "^0.0.8", optional = true }
-
-[tool.poetry.extras]
-openplugin = ["openplugin"]
-
-[tool.poetry.group.openplugin.dependencies]
-openplugin = "^0.0.8"
+openplugin = "^0.0.9"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
```

