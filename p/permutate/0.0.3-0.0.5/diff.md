# Comparing `tmp/permutate-0.0.3.tar.gz` & `tmp/permutate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permutate-0.0.3.tar", max compression
+gzip compressed data, was "permutate-0.0.5.tar", max compression
```

## Comparing `permutate-0.0.3.tar` & `permutate-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3488 2023-05-25 19:24:36.085184 permutate-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-31 14:00:12.890922 permutate-0.0.3/permutate/__init__.py
--rw-r--r--   0        0        0       48 2023-05-31 03:53:49.018228 permutate-0.0.3/permutate/__main__.py
--rw-r--r--   0        0        0     2135 2023-05-30 20:40:58.184224 permutate-0.0.3/permutate/job_request_schema.py
--rw-r--r--   0        0        0     9357 2023-05-31 14:08:14.683949 permutate-0.0.3/permutate/job_response_schema.py
--rw-r--r--   0        0        0     1153 2023-05-31 14:00:27.681618 permutate-0.0.3/permutate/logger.py
--rw-r--r--   0        0        0      681 2023-05-31 14:02:40.510832 permutate-0.0.3/permutate/main.py
--rw-r--r--   0        0        0     7107 2023-05-31 04:56:20.655804 permutate-0.0.3/permutate/runner.py
--rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.3/permutate/singleton.py
--rw-r--r--   0        0        0     3436 2023-05-31 02:50:49.776334 permutate-0.0.3/permutate/templates/job_result_template.html
--rw-r--r--   0        0        0     2046 2023-05-30 18:29:26.750789 permutate-0.0.3/permutate/workspace/plugin_test.yaml
--rw-r--r--   0        0        0      523 2023-05-31 14:10:52.983830 permutate-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 permutate-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3697 2023-05-31 17:06:56.759040 permutate-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 14:00:12.890922 permutate-0.0.5/permutate/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-31 17:06:56.770244 permutate-0.0.5/permutate/__main__.py
+-rw-r--r--   0        0        0     2311 2023-05-31 17:06:56.770874 permutate-0.0.5/permutate/job_request_schema.py
+-rw-r--r--   0        0        0    10079 2023-05-31 17:06:56.771081 permutate-0.0.5/permutate/job_response_schema.py
+-rw-r--r--   0        0        0     1153 2023-05-31 17:06:56.771661 permutate-0.0.5/permutate/logger.py
+-rw-r--r--   0        0        0     2357 2023-05-31 17:06:56.771839 permutate-0.0.5/permutate/main.py
+-rw-r--r--   0        0        0     7474 2023-06-01 15:19:08.121789 permutate-0.0.5/permutate/runner.py
+-rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.5/permutate/singleton.py
+-rw-r--r--   0        0        0     3436 2023-05-31 17:06:56.772174 permutate-0.0.5/permutate/templates/job_result_template.html
+-rw-r--r--   0        0        0     2001 2023-05-31 17:06:56.772299 permutate-0.0.5/permutate/workspace/plugin_test.yaml
+-rw-r--r--   0        0        0      590 2023-06-01 15:21:52.142906 permutate-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 permutate-0.0.5/PKG-INFO
```

### Comparing `permutate-0.0.3/README.md` & `permutate-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 # Permutate
-![Alt text](docs/logo.png?raw=true "Title")
-#### Permutate is an automated testing framework for LLM Plugins. 
+![Alt text](https://github.com/LegendaryAI/permutate/blob/main/docs/permutate-logo.png)
+## Permutate is an automated testing framework for LLM Plugins. 
 
-##### ChatGPT Ignited LLM Plugins
+### ChatGPT Ignited LLM Plugins
 ChatGPT spread like wildfire but it had some limitations, notably, it couldn’t access private data/systems. But this limitation was resolved with the release of OpenAI Plugins. This enabled developers to connect their favorite applications to ChatGPT. Unfortunately, in the rush to release plugins, quality assurance lacked. 
 
 From a software quality perspective, several common problems surfaced:
 <ul>
 <li>Despite the plugin being “installed” in a user’s environment, the plugin wasn’t consistently activated by the user’s text.</li>
 <li>When it was activated, the plugin wasn’t called correctly, leading to undesirable results.</li>
 </ul>
 
 Ultimately, plugin developers chose to remove the bulk of their features just to get basic functions to run correctly. 🙁
 
+  
+---
+  
+![Alt text](https://github.com/LegendaryAI/permutate/blob/main/docs/permutate-overview.png) 
 
-##### Introducing Permutate
+
+---
+  
+  
+### Introducing Permutate
 Permutate is an automated testing framework for LLM Plugins. 
 
 Permutate allows development teams to:
 <ul>
 <li>Define a set of reusable tests for plugins</li>
 <li>Describe the tests using a standard, open format</li>
 <li>Use open source software (Permutate) to execute the tests</li>
 <li>See the results of individual test cases as well as summary statistics</li>
 </ul>
 
-##### The Permutation Problem 
+
+#### The Permutation Problem 
 When users give prompts (instructions to an LLM via chat, etc.), they use a variety of ways of describing what they want. Each sentence variation might work or fail. The goal is to get as many of them to succeed as possible. 
 
 Some technology (the tool selector) must determine what the intent of the command was (aka, intent detection). Additionally, the command might have extra data like “in the morning” or “once per week”. This natural language needs to be mapped back to an API. The Tool Selector must do more than just ‘find the right tool’, it must map language to an API and call it perfectly. 
 
 So, here we go. Given J variations of sample input text, and K variations of "installed" plugins, we use a tool selector and evaluate the performance:
 <ol>
 <li>Is the correct plugin selected?</li>
 <li>Is the correct API operation selected?</li>
 <li>Are the API parameters filled in correctly?</li>
 <li>What was the cost to solve?</li>
 <li>And, what was the round-trip latency?</li>
 </ol>
 
-#### Tool Selectors 
+### Tool Selectors 
 To satisfy these concerns, developers will use a Tool Selector service. Here, they pass in the text, and it identifies the correct plugin to use, the right operations, etc. In some cases, they might return the necessary source code to call the API, with all of the parameters filled in. 
 
 To make life simple, we created OpenPlugin. This is optional. This allows plugin service providers to offer their best implementation possible. If an implementation isn’t giving you the accuracy or performance you need, try another. But more importantly, it allows you to test plugins using basic CI/CD principles.  
 
 #### Is this just for OpenAI?
 No. OpenAI hasn’t (yet) made their tool selector service available to the public. We encourage all vendors to make their tool selector service available. This allows for headless automation testing, and without it, we can anticipate poor plugin quality. 
 
 Until OpenAI makes their Tool Selector service available to the public, you have two options:
 <ol>
 <li>Manual Testing</li>
 <li>UI Testing (e.g., Selenium Hell).</li>
 </ol>
 
-#### Getting started
+### Getting started
+(THIS PROJECT IS NOT RELEASED YET).
+More docs coming soon!
```

### Comparing `permutate-0.0.3/permutate/job_request_schema.py` & `permutate-0.0.5/permutate/job_request_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from datetime import datetime
 from pydantic_yaml import YamlModel
 from typing import List, Optional, Dict
 from pydantic import BaseModel, root_validator
 
 
 class Permutation(BaseModel):
     name: str
@@ -52,14 +53,15 @@
     langchain_tool_selector: Optional[str]
     imprompt_tool_selector: Optional[str]
     auto_translate_to_languages: List[str]
 
 
 class JobRequest(YamlModel):
     version: str
+    name: str
     config: Config
     test_plugin: Plugin
     plugin_groups: List[PluginGroup]
     permutations: List[Permutation]
     test_cases: List[TestCase]
 
     def get_plugin_group_from_name(self, plugin_group_name: str) -> PluginGroup:
@@ -67,7 +69,10 @@
             if plugin_group.name == plugin_group_name:
                 return plugin_group
 
     def get_plugin_group_from_permutation(self, permutation: Permutation) -> PluginGroup:
         for plugin_group in self.plugin_groups:
             if plugin_group.name == permutation.tool_selector.get("plugin_group_name"):
                 return plugin_group
+
+    def get_job_request_name(self):
+        return "{}-{}-{}".format(self.name, self.version, datetime.now().strftime("%Y-%m-%d"))
```

### Comparing `permutate-0.0.3/permutate/job_response_schema.py` & `permutate-0.0.5/permutate/job_response_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -87,20 +87,22 @@
 
 class JobSummaryOut(JobSummary):
     class Config:
         json_encoders = {Decimal: lambda v: float(round(v, 2))}
 
 
 class JobResponse(BaseModel):
+    job_name: str
     started_on: datetime
     completed_on: datetime
     test_plugin: Plugin
     permutations: List[Permutation]
     summary: JobSummary
     details: List[JobDetail]
+    output_directory: str
 
     def get_permutation_by_name(self, name: str):
         for permutation in self.permutations:
             if permutation.name == name:
                 return permutation
 
     def group_details(self):
@@ -114,44 +116,52 @@
     def get_test_cases(self):
         test_cases = {}
         for detail in self.details:
             test_cases[detail.test_case_name] = detail.prompt
         return test_cases
 
     def save_to_csv(self, break_down_by_environment: bool = False):
-        file_location = "workspace/"
         if not break_down_by_environment:
             fieldnames = list(JobSummary.schema()["properties"].keys())
-            with open(f"{file_location}summary.csv", "w") as fp:
+            summary_filename = f"{self.output_directory}{self.job_name}-summary.csv"
+            with open(summary_filename, "w") as fp:
                 writer = csv.DictWriter(fp, fieldnames=fieldnames)
                 writer.writeheader()
                 writer.writerow(json.loads(JobSummaryOut(**self.summary.dict()).json()))
 
             fieldnames = list(JobDetail.schema()["properties"].keys())
-            with open(f"{file_location}details.csv", "w") as fp:
+            detail_filename = f"{self.output_directory}{self.job_name}-details.csv"
+            with open(detail_filename, "w") as fp:
                 writer = csv.DictWriter(fp, fieldnames=fieldnames)
                 writer.writeheader()
                 for detail in self.details:
                     writer.writerow(json.loads(JobDetail(**detail.dict()).json()))
+
+            print(f"Summary csv result\n\t{summary_filename}")
+            print(f"Details csv result\n\t{detail_filename}")
         else:
             for permutation in self.permutations:
                 environment_name = permutation.name
                 fieldnames = list(JobSummary.schema()["properties"].keys())
-                with open(f"{file_location}{environment_name}_summary.csv", "w") as fp:
+                summary_filename = f"{self.output_directory}{self.job_name}{environment_name}_summary.csv"
+                with open(summary_filename, "w") as fp:
                     writer = csv.DictWriter(fp, fieldnames=fieldnames)
                     writer.writeheader()
                     writer.writerow(json.loads(JobSummaryOut(**self.summary.dict()).json()))
 
                 fieldnames = list(JobDetail.schema()["properties"].keys())
-                with open(f"{file_location}{environment_name}_details.csv", "w") as fp:
+                detail_filename = f"{self.output_directory}{self.job_name}{environment_name}_details.csv"
+                with open(detail_filename, "w") as fp:
                     writer = csv.DictWriter(fp, fieldnames=fieldnames)
                     writer.writeheader()
                     for detail in self.details:
                         if detail.permutation_name == permutation.name:
                             writer.writerow(json.loads(JobDetail(**detail.dict()).json()))
+                print(f"Summary csv result\n\t{summary_filename}")
+                print(f"Details csv result\n\t{detail_filename}")
 
     def build_html_table(self) -> str:
         header = [
             "Tool Case Result",
             "Tool",
             "Pipeline",
             "LLM",
@@ -216,10 +226,14 @@
             {"data": self.summary.total_llm_api_cost},
         ])
         plugin = self.test_plugin.name_for_human
         started_on = self.started_on.strftime("%Y-%m-%d %H:%M:%S")
         ended_on = self.completed_on.strftime("%Y-%m-%d %H:%M:%S")
         html = template.render(plugin=plugin, started_on=started_on, ended_on=ended_on, summary_headers=summary_headers,
                                summary_rows=summary_rows, headers=header, rows=rows)
-        with open(f"{current_dir}/workspace/job_result.html", "w") as f:
+        filename = f"{self.job_name}-result.html"
+
+        with open(f"{self.output_directory}{filename}", "w") as f:
             f.write(html)
-        return f"file://{current_dir}/workspace/job_result.html"
+        print(f"HTML result\n\t{self.output_directory}{filename}")
+        absolute_path = os.path.abspath(f"{self.output_directory}{filename}")
+        return f"file://{absolute_path}"
```

### Comparing `permutate-0.0.3/permutate/logger.py` & `permutate-0.0.5/permutate/logger.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.3/permutate/runner.py` & `permutate-0.0.5/permutate/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,44 +2,49 @@
 import requests
 import webbrowser
 from tqdm import tqdm
 from .logger import logger
 from datetime import datetime
 from .job_request_schema import JobRequest
 from .job_response_schema import JobResponse, JobSummary, JobDetail
+import importlib.util
+
+found_openplugin_lib = importlib.util.find_spec("openplugin") is not None
 
 
 class Runner:
 
     def __init__(self, show_progress_bar: bool = True):
         self.show_progress_bar = show_progress_bar
         if self.show_progress_bar:
             self.pbar = tqdm(total=100)
             self.progress_counter = None
 
-    def start(self, file_path: str, save_to_html=True, save_to_csv=True):
+    def start(self, file_path: str, output_directory: str, save_to_html=True, save_to_csv=True):
         logger.info("Starting permutate")
         with open(file_path) as f:
             yaml_file = f.read()
         request = JobRequest.parse_raw(yaml_file)
         self.progress_counter = 100 / (len(request.permutations) * len(request.test_cases))
         batch_job_started_on = datetime.now()
         all_details = []
         for permutation in request.permutations:
             permutation_details = self.single_permutation(request, permutation)
             all_details.extend(permutation_details)
 
         summary = JobSummary.build_from_details(all_details)
         response = JobResponse(
+            job_name=request.get_job_request_name(),
             started_on=batch_job_started_on,
             completed_on=datetime.now(),
             test_plugin=request.test_plugin,
             permutations=request.permutations,
             summary=summary,
-            details=all_details
+            details=all_details,
+            output_directory=output_directory
         )
         if self.show_progress_bar:
             self.pbar.close()
         response.save_to_csv(break_down_by_environment=False) if save_to_csv else None
         if save_to_html:
             url = response.build_html_table()
             webbrowser.open(url)
@@ -75,66 +80,29 @@
                 "message_type": "HumanMessage"
             }],
             "plugins": plugin_group.dict().get("plugins"),
             "config": config.dict(),
             "tool_selector_config": permutation.tool_selector,
             "llm": permutation.llm
         })
-        headers = {'Content-Type': 'application/json'}
-        response = requests.request("POST", url, headers=headers, data=payload)
-        if response.status_code == 200:
+        passed = True
+        if found_openplugin_lib:
+            from openplugin import run_plugin_selector
+            response_json = run_plugin_selector(payload)
+            if response_json is None:
+                passed = False
+        else:
+            headers = {'Content-Type': 'application/json'}
+            response = requests.request("POST", url, headers=headers, data=payload)
+            if response.status_code != 200:
+                passed = False
             response_json = response.json()
-            is_plugin_detected = False
-            is_plugin_operation_found = False
-            is_plugin_parameter_mapped = False
-            parameter_mapped_percentage = 0
-            plugin_operation = None
-            plugin_name = None
-            plugin_parameters_mapped = None
-            for detected_plugin_operation in response_json.get("detected_plugin_operations"):
-                if detected_plugin_operation.get("plugin").get("name_for_model") == test_case.expected_plugin_used or \
-                        detected_plugin_operation.get("plugin").get("name_for_human") == test_case.expected_plugin_used:
-                    is_plugin_detected = True
-                    plugin_name = detected_plugin_operation.get("plugin").get("name_for_human")
-                    if detected_plugin_operation.get("plugin").get("api_called") == test_case.expected_api_used:
-                        is_plugin_operation_found = True
-                    plugin_operation = detected_plugin_operation.get("plugin").get("api_called")
-                    plugin_parameters_mapped = detected_plugin_operation.get("mapped_operation_parameters")
-                    if plugin_parameters_mapped:
-                        expected_params = test_case.expected_parameters
-                        common_pairs = {k: plugin_parameters_mapped[k] for k in plugin_parameters_mapped if
-                                        k in expected_params and plugin_parameters_mapped[k] == expected_params[k]}
-                        if len(common_pairs) == len(expected_params):
-                            parameter_mapped_percentage = 100
-                            is_plugin_parameter_mapped = True
-                        else:
-                            parameter_mapped_percentage = len(common_pairs) / len(expected_params) * 100
 
-            detail = JobDetail(
-                permutation_name=permutation.name,
-                permutation_summary=permutation_summary,
-                test_case_name=test_case.name,
-                is_run_completed=True,
-                language="English",
-                prompt=test_case.prompt,
-                final_output=response_json.get("final_text_response"),
-                match_score="0.0",
-                is_plugin_detected=is_plugin_detected,
-                is_plugin_operation_found=is_plugin_operation_found,
-                is_plugin_parameter_mapped=is_plugin_parameter_mapped,
-                parameter_mapped_percentage=parameter_mapped_percentage,
-                plugin_name=plugin_name,
-                plugin_operation=plugin_operation,
-                plugin_parameters_mapped=plugin_parameters_mapped,
-                response_time_sec=response_json.get("response_time"),
-                total_llm_tokens_used=response_json.get("tokens_used"),
-                llm_api_cost=response_json.get("llm_api_cost")
-            )
-        else:
-            detail = JobDetail(
+        if not passed or response_json is None:
+            return JobDetail(
                 permutation_name=permutation.name,
                 permutation_summary=permutation_summary,
                 test_case_name=test_case.name,
                 is_run_completed=False,
                 language="English",
                 prompt=test_case.prompt,
                 final_output=f"FAILED",
@@ -143,8 +111,55 @@
                 is_plugin_operation_found=False,
                 is_plugin_parameter_mapped=False,
                 parameter_mapped_percentage=0,
                 response_time_sec=0,
                 total_llm_tokens_used=0,
                 llm_api_cost=0
             )
+
+        is_plugin_detected = False
+        is_plugin_operation_found = False
+        is_plugin_parameter_mapped = False
+        parameter_mapped_percentage = 0
+        plugin_operation = None
+        plugin_name = None
+        plugin_parameters_mapped = None
+        for detected_plugin_operation in response_json.get("detected_plugin_operations"):
+            if detected_plugin_operation.get("plugin").get("name_for_model") == test_case.expected_plugin_used or \
+                    detected_plugin_operation.get("plugin").get("name_for_human") == test_case.expected_plugin_used:
+                is_plugin_detected = True
+                plugin_name = detected_plugin_operation.get("plugin").get("name_for_human")
+                if detected_plugin_operation.get("plugin").get("api_called") == test_case.expected_api_used:
+                    is_plugin_operation_found = True
+                plugin_operation = detected_plugin_operation.get("plugin").get("api_called")
+                plugin_parameters_mapped = detected_plugin_operation.get("mapped_operation_parameters")
+                if plugin_parameters_mapped:
+                    expected_params = test_case.expected_parameters
+                    common_pairs = {k: plugin_parameters_mapped[k] for k in plugin_parameters_mapped if
+                                    k in expected_params and plugin_parameters_mapped[k] == expected_params[k]}
+                    if len(common_pairs) == len(expected_params):
+                        parameter_mapped_percentage = 100
+                        is_plugin_parameter_mapped = True
+                    else:
+                        parameter_mapped_percentage = len(common_pairs) / len(expected_params) * 100
+
+        detail = JobDetail(
+            permutation_name=permutation.name,
+            permutation_summary=permutation_summary,
+            test_case_name=test_case.name,
+            is_run_completed=True,
+            language="English",
+            prompt=test_case.prompt,
+            final_output=response_json.get("final_text_response"),
+            match_score="0.0",
+            is_plugin_detected=is_plugin_detected,
+            is_plugin_operation_found=is_plugin_operation_found,
+            is_plugin_parameter_mapped=is_plugin_parameter_mapped,
+            parameter_mapped_percentage=parameter_mapped_percentage,
+            plugin_name=plugin_name,
+            plugin_operation=plugin_operation,
+            plugin_parameters_mapped=plugin_parameters_mapped,
+            response_time_sec=response_json.get("response_time"),
+            total_llm_tokens_used=response_json.get("tokens_used"),
+            llm_api_cost=response_json.get("llm_api_cost")
+        )
         return detail
```

### Comparing `permutate-0.0.3/permutate/singleton.py` & `permutate-0.0.5/permutate/singleton.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.3/permutate/templates/job_result_template.html` & `permutate-0.0.5/permutate/templates/job_result_template.html`

 * *Files identical despite different names*

### Comparing `permutate-0.0.3/permutate/workspace/plugin_test.yaml` & `permutate-0.0.5/permutate/workspace/plugin_test.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 version: 1.0.0
+name: klarna_plugin_test
 config:
-  openai_api_key: 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
   langchain_tool_selector: http://localhost:8006/api/langchain/run-plugin
   imprompt_tool_selector: http://localhost:8006/api/imprompt/run-plugin
   auto_translate_to_languages:
     - English
     - Spanish
 test_plugin:
     manifest_url: https://www.klarna.com/.well-known/ai-plugin.json
```

### Comparing `permutate-0.0.3/pyproject.toml` & `permutate-0.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "permutate"
-version = "0.0.3"
+version = "0.0.5"
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
 
+[tool.poetry.group.openplugin.dependencies]
+openplugin = "^0.0.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 permutate = "permutate.main:app"
```

### Comparing `permutate-0.0.3/PKG-INFO` & `permutate-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permutate
-Version: 0.0.3
+Version: 0.0.5
 Summary: Testing framework for LLM Plugins
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,63 +15,74 @@
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (==2.29.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Permutate
-![Alt text](docs/logo.png?raw=true "Title")
-#### Permutate is an automated testing framework for LLM Plugins. 
+![Alt text](https://github.com/LegendaryAI/permutate/blob/main/docs/permutate-logo.png)
+## Permutate is an automated testing framework for LLM Plugins. 
 
-##### ChatGPT Ignited LLM Plugins
+### ChatGPT Ignited LLM Plugins
 ChatGPT spread like wildfire but it had some limitations, notably, it couldn’t access private data/systems. But this limitation was resolved with the release of OpenAI Plugins. This enabled developers to connect their favorite applications to ChatGPT. Unfortunately, in the rush to release plugins, quality assurance lacked. 
 
 From a software quality perspective, several common problems surfaced:
 <ul>
 <li>Despite the plugin being “installed” in a user’s environment, the plugin wasn’t consistently activated by the user’s text.</li>
 <li>When it was activated, the plugin wasn’t called correctly, leading to undesirable results.</li>
 </ul>
 
 Ultimately, plugin developers chose to remove the bulk of their features just to get basic functions to run correctly. 🙁
 
+  
+---
+  
+![Alt text](https://github.com/LegendaryAI/permutate/blob/main/docs/permutate-overview.png) 
 
-##### Introducing Permutate
+
+---
+  
+  
+### Introducing Permutate
 Permutate is an automated testing framework for LLM Plugins. 
 
 Permutate allows development teams to:
 <ul>
 <li>Define a set of reusable tests for plugins</li>
 <li>Describe the tests using a standard, open format</li>
 <li>Use open source software (Permutate) to execute the tests</li>
 <li>See the results of individual test cases as well as summary statistics</li>
 </ul>
 
-##### The Permutation Problem 
+
+#### The Permutation Problem 
 When users give prompts (instructions to an LLM via chat, etc.), they use a variety of ways of describing what they want. Each sentence variation might work or fail. The goal is to get as many of them to succeed as possible. 
 
 Some technology (the tool selector) must determine what the intent of the command was (aka, intent detection). Additionally, the command might have extra data like “in the morning” or “once per week”. This natural language needs to be mapped back to an API. The Tool Selector must do more than just ‘find the right tool’, it must map language to an API and call it perfectly. 
 
 So, here we go. Given J variations of sample input text, and K variations of "installed" plugins, we use a tool selector and evaluate the performance:
 <ol>
 <li>Is the correct plugin selected?</li>
 <li>Is the correct API operation selected?</li>
 <li>Are the API parameters filled in correctly?</li>
 <li>What was the cost to solve?</li>
 <li>And, what was the round-trip latency?</li>
 </ol>
 
-#### Tool Selectors 
+### Tool Selectors 
 To satisfy these concerns, developers will use a Tool Selector service. Here, they pass in the text, and it identifies the correct plugin to use, the right operations, etc. In some cases, they might return the necessary source code to call the API, with all of the parameters filled in. 
 
 To make life simple, we created OpenPlugin. This is optional. This allows plugin service providers to offer their best implementation possible. If an implementation isn’t giving you the accuracy or performance you need, try another. But more importantly, it allows you to test plugins using basic CI/CD principles.  
 
 #### Is this just for OpenAI?
 No. OpenAI hasn’t (yet) made their tool selector service available to the public. We encourage all vendors to make their tool selector service available. This allows for headless automation testing, and without it, we can anticipate poor plugin quality. 
 
 Until OpenAI makes their Tool Selector service available to the public, you have two options:
 <ol>
 <li>Manual Testing</li>
 <li>UI Testing (e.g., Selenium Hell).</li>
 </ol>
 
-#### Getting started
+### Getting started
+(THIS PROJECT IS NOT RELEASED YET).
+More docs coming soon!
```

