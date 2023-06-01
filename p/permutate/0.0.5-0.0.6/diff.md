# Comparing `tmp/permutate-0.0.5.tar.gz` & `tmp/permutate-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permutate-0.0.5.tar", max compression
+gzip compressed data, was "permutate-0.0.6.tar", max compression
```

## Comparing `permutate-0.0.5.tar` & `permutate-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3697 2023-05-31 17:06:56.759040 permutate-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-31 14:00:12.890922 permutate-0.0.5/permutate/__init__.py
--rw-r--r--   0        0        0       48 2023-05-31 17:06:56.770244 permutate-0.0.5/permutate/__main__.py
--rw-r--r--   0        0        0     2311 2023-05-31 17:06:56.770874 permutate-0.0.5/permutate/job_request_schema.py
--rw-r--r--   0        0        0    10079 2023-05-31 17:06:56.771081 permutate-0.0.5/permutate/job_response_schema.py
--rw-r--r--   0        0        0     1153 2023-05-31 17:06:56.771661 permutate-0.0.5/permutate/logger.py
--rw-r--r--   0        0        0     2357 2023-05-31 17:06:56.771839 permutate-0.0.5/permutate/main.py
--rw-r--r--   0        0        0     7474 2023-06-01 15:19:08.121789 permutate-0.0.5/permutate/runner.py
--rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.5/permutate/singleton.py
--rw-r--r--   0        0        0     3436 2023-05-31 17:06:56.772174 permutate-0.0.5/permutate/templates/job_result_template.html
--rw-r--r--   0        0        0     2001 2023-05-31 17:06:56.772299 permutate-0.0.5/permutate/workspace/plugin_test.yaml
--rw-r--r--   0        0        0      590 2023-06-01 15:21:52.142906 permutate-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 permutate-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3697 2023-05-31 17:06:56.759040 permutate-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 14:00:12.890922 permutate-0.0.6/permutate/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-31 17:06:56.770244 permutate-0.0.6/permutate/__main__.py
+-rw-r--r--   0        0        0     2311 2023-05-31 17:06:56.770874 permutate-0.0.6/permutate/job_request_schema.py
+-rw-r--r--   0        0        0    10079 2023-05-31 17:06:56.771081 permutate-0.0.6/permutate/job_response_schema.py
+-rw-r--r--   0        0        0     1153 2023-05-31 17:06:56.771661 permutate-0.0.6/permutate/logger.py
+-rw-r--r--   0        0        0     2357 2023-05-31 17:06:56.771839 permutate-0.0.6/permutate/main.py
+-rw-r--r--   0        0        0     7498 2023-06-01 15:42:12.502459 permutate-0.0.6/permutate/runner.py
+-rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.6/permutate/singleton.py
+-rw-r--r--   0        0        0     3436 2023-05-31 17:06:56.772174 permutate-0.0.6/permutate/templates/job_result_template.html
+-rw-r--r--   0        0        0     2001 2023-05-31 17:06:56.772299 permutate-0.0.6/permutate/workspace/plugin_test.yaml
+-rw-r--r--   0        0        0      750 2023-06-01 15:48:05.529705 permutate-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 permutate-0.0.6/PKG-INFO
```

### Comparing `permutate-0.0.5/README.md` & `permutate-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `permutate-0.0.5/permutate/job_request_schema.py` & `permutate-0.0.6/permutate/job_request_schema.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.5/permutate/job_response_schema.py` & `permutate-0.0.6/permutate/job_response_schema.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.5/permutate/logger.py` & `permutate-0.0.6/permutate/logger.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.5/permutate/main.py` & `permutate-0.0.6/permutate/main.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.5/permutate/runner.py` & `permutate-0.0.6/permutate/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,20 +64,14 @@
                 permutation_summary
             )
             permutation_details.append(detail)
         return permutation_details
 
     @staticmethod
     def run_single_permutation_test_case(test_case, config, permutation, plugin_group, permutation_summary):
-        if permutation.tool_selector.get("provider") == "Imprompt":
-            url = config.imprompt_tool_selector
-        elif permutation.tool_selector.get("provider") == "Langchain":
-            url = config.langchain_tool_selector
-        else:
-            raise Exception("Tool selector provider not supported")
         payload = json.dumps({
             "messages": [{
                 "content": test_case.prompt,
                 "message_type": "HumanMessage"
             }],
             "plugins": plugin_group.dict().get("plugins"),
             "config": config.dict(),
@@ -87,14 +81,20 @@
         passed = True
         if found_openplugin_lib:
             from openplugin import run_plugin_selector
             response_json = run_plugin_selector(payload)
             if response_json is None:
                 passed = False
         else:
+            if permutation.tool_selector.get("provider") == "Imprompt":
+                url = config.imprompt_tool_selector
+            elif permutation.tool_selector.get("provider") == "Langchain":
+                url = config.langchain_tool_selector
+            else:
+                raise Exception("Tool selector provider not supported")
             headers = {'Content-Type': 'application/json'}
             response = requests.request("POST", url, headers=headers, data=payload)
             if response.status_code != 200:
                 passed = False
             response_json = response.json()
 
         if not passed or response_json is None:
```

### Comparing `permutate-0.0.5/permutate/singleton.py` & `permutate-0.0.6/permutate/singleton.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.5/permutate/templates/job_result_template.html` & `permutate-0.0.6/permutate/templates/job_result_template.html`

 * *Files identical despite different names*

### Comparing `permutate-0.0.5/permutate/workspace/plugin_test.yaml` & `permutate-0.0.6/permutate/workspace/plugin_test.yaml`

 * *Files identical despite different names*

### Comparing `permutate-0.0.5/pyproject.toml` & `permutate-0.0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 [tool.poetry]
 name = "permutate"
-version = "0.0.5"
+version = "0.0.6"
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
+openplugin = { version = "^0.0.8", optional = true }
+
+[tool.poetry.extras]
+openplugin = ["openplugin"]
 
 [tool.poetry.group.openplugin.dependencies]
-openplugin = "^0.0.2"
+openplugin = "^0.0.8"
+
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 permutate = "permutate.main:app"
```

### Comparing `permutate-0.0.5/PKG-INFO` & `permutate-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: permutate
-Version: 0.0.5
+Version: 0.0.6
 Summary: Testing framework for LLM Plugins
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: openplugin
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: openplugin (>=0.0.8,<0.0.9) ; extra == "openplugin"
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pydantic-yaml (>=0.11.2,<0.12.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (==2.29.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

