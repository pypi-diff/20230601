# Comparing `tmp/openplugin-0.0.6.tar.gz` & `tmp/openplugin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-0.0.6.tar", max compression
+gzip compressed data, was "openplugin-0.0.7.tar", max compression
```

## Comparing `openplugin-0.0.6.tar` & `openplugin-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.6/README.md
--rw-r--r--   0        0        0      754 2023-06-01 14:53:19.914449 openplugin-0.0.6/openplugin/__init__.py
--rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.6/openplugin/__main__.py
--rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.6/openplugin/api/__init__.py
--rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.6/openplugin/api/http_error.py
--rw-r--r--   0        0        0      874 2023-06-01 14:05:00.648019 openplugin-0.0.6/openplugin/api/imprompt.py
--rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.6/openplugin/api/langchain.py
--rw-r--r--   0        0        0     8095 2023-05-31 17:14:33.045786 openplugin-0.0.6/openplugin/bindings/imprompt/imprompt_plugin_selector.py
--rw-r--r--   0        0        0     5324 2023-05-31 20:38:23.595623 openplugin-0.0.6/openplugin/bindings/langchain/langchain_plugin_selector.py
--rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.6/openplugin/interfaces/plugin_selector.py
--rw-r--r--   0        0        0      562 2023-05-31 19:01:14.915142 openplugin-0.0.6/openplugin/main.py
--rw-r--r--   0        0        0     1055 2023-06-01 15:06:28.621683 openplugin-0.0.6/openplugin/utils/run_plugin_selector.py
--rw-r--r--   0        0        0      521 2023-06-01 15:08:13.544009 openplugin-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.7/README.md
+-rw-r--r--   0        0        0      754 2023-06-01 14:53:19.914449 openplugin-0.0.7/openplugin/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.7/openplugin/__main__.py
+-rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.7/openplugin/api/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.7/openplugin/api/http_error.py
+-rw-r--r--   0        0        0      874 2023-06-01 14:05:00.648019 openplugin-0.0.7/openplugin/api/imprompt.py
+-rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.7/openplugin/api/langchain.py
+-rw-r--r--   0        0        0     8094 2023-06-01 15:09:41.946666 openplugin-0.0.7/openplugin/bindings/imprompt/imprompt_plugin_selector.py
+-rw-r--r--   0        0        0     5322 2023-06-01 15:09:41.949092 openplugin-0.0.7/openplugin/bindings/langchain/langchain_plugin_selector.py
+-rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.7/openplugin/interfaces/plugin_selector.py
+-rw-r--r--   0        0        0      561 2023-06-01 15:09:41.950905 openplugin-0.0.7/openplugin/main.py
+-rw-r--r--   0        0        0     1055 2023-06-01 15:06:28.621683 openplugin-0.0.7/openplugin/utils/run_plugin_selector.py
+-rw-r--r--   0        0        0      521 2023-06-01 15:10:36.978053 openplugin-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.7/PKG-INFO
```

### Comparing `openplugin-0.0.6/README.md` & `openplugin-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.6/openplugin/__init__.py` & `openplugin-0.0.7/openplugin/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.6/openplugin/api/__init__.py` & `openplugin-0.0.7/openplugin/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.6/openplugin/api/imprompt.py` & `openplugin-0.0.7/openplugin/api/imprompt.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.6/openplugin/api/langchain.py` & `openplugin-0.0.7/openplugin/api/langchain.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.6/openplugin/bindings/imprompt/imprompt_plugin_selector.py` & `openplugin-0.0.7/openplugin/bindings/imprompt/imprompt_plugin_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def initialize_tool_selector(
             self,
             tool_selector_config: ToolSelectorConfig,
             plugins: List[Plugin],
             config: Optional[Config],
             llm: LLM
     ):
-        openai.api_key = os.environ["OPENAPI_KEY"] if config.openai_api_key is None else config.openai_api_key
+        openai.api_key = os.environ["OPENAI_KEY"] if config.openai_api_key is None else config.openai_api_key
         self.llm = llm
         self.total_tokens_used = 0
         pass
 
     def run(self, messages: List[Message]) -> Response:
         start_test_case_time = time.time()
         plugin_operations = self.get_detected_plugin_with_operations(messages)
```

### Comparing `openplugin-0.0.6/openplugin/bindings/langchain/langchain_plugin_selector.py` & `openplugin-0.0.7/openplugin/bindings/langchain/langchain_plugin_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,30 +29,30 @@
         return AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION
     raise ValueError(f"Pipeline name {pipeline_name} not supported")
 
 
 def _get_llm(llm: LLM, api_key: str):
     if llm.provider == LLMProvider.OpenAI:
         if api_key is None:
-            api_key = os.environ["OPENAPI_KEY"]
+            api_key = os.environ["OPENAI_KEY"]
         os.environ["OPENAI_API_KEY"] = api_key
         llm = OpenAI(
             model_name=llm.model_name,
             temperature=llm.temperature,
             max_tokens=llm.max_tokens,
             top_p=llm.top_p,
             frequency_penalty=llm.frequency_penalty,
             presence_penalty=llm.presence_penalty,
             n=llm.n,
             best_of=llm.best_of
         )
         return llm
     elif llm.provider == LLMProvider.OpenAIChat:
         if api_key is None:
-            api_key = os.environ["OPENAPI_KEY"]
+            api_key = os.environ["OPENAI_KEY"]
         os.environ["OPENAI_API_KEY"] = api_key
         llm = ChatOpenAI(
             model_name=llm.model_name,
             temperature=llm.temperature,
             max_retries=llm.max_retries,
             n=llm.n,
             max_tokens=llm.max_tokens
```

### Comparing `openplugin-0.0.6/openplugin/interfaces/plugin_selector.py` & `openplugin-0.0.7/openplugin/interfaces/plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.6/openplugin/main.py` & `openplugin-0.0.7/openplugin/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 def start_server(openai_api_key: Annotated[str, typer.Option(help="OpenAI API Key",
                                                              rich_help_panel="Customization and Utils")]):
     """
     Start the openplugin server
     """
     from openplugin.api import app
     load_dotenv()
-    os.environ["OPENAPI_KEY"] = openai_api_key
+    os.environ["OPENAI_KEY"] = openai_api_key
     uvicorn.run(app, host=os.environ['HOST'], port=int(os.environ['PORT']))
```

### Comparing `openplugin-0.0.6/openplugin/utils/run_plugin_selector.py` & `openplugin-0.0.7/openplugin/utils/run_plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.6/pyproject.toml` & `openplugin-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openplugin"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["shrikant <shrikant.pm14@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain = "^0.0.178"
```

### Comparing `openplugin-0.0.6/PKG-INFO` & `openplugin-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

