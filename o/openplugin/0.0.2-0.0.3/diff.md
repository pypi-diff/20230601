# Comparing `tmp/openplugin-0.0.2.tar.gz` & `tmp/openplugin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-0.0.2.tar", max compression
+gzip compressed data, was "openplugin-0.0.3.tar", max compression
```

## Comparing `openplugin-0.0.2.tar` & `openplugin-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,21 @@
--rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.2/README.md
--rw-r--r--   0        0        0      659 2023-05-31 17:20:20.388850 openplugin-0.0.2/openplugin/__init__.py
--rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.2/openplugin/__main__.py
--rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.2/openplugin/api/__init__.py
--rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.2/openplugin/api/http_error.py
--rw-r--r--   0        0        0      873 2023-05-31 17:17:32.611062 openplugin-0.0.2/openplugin/api/imprompt.py
--rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.2/openplugin/api/langchain.py
--rw-r--r--   0        0        0     8095 2023-05-31 17:14:33.045786 openplugin-0.0.2/openplugin/bindings/imprompt/imprompt_plugin_selector.py
--rw-r--r--   0        0        0     5322 2023-05-31 17:14:46.276595 openplugin-0.0.2/openplugin/bindings/langchain/langchain_plugin_selector.py
--rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.2/openplugin/interfaces/plugin_selector.py
--rw-r--r--   0        0        0      562 2023-05-31 19:01:14.915142 openplugin-0.0.2/openplugin/main.py
--rw-r--r--   0        0        0      521 2023-05-31 19:01:50.001865 openplugin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.3/README.md
+-rw-r--r--   0        0        0      755 2023-06-01 14:36:35.893659 openplugin-0.0.3/openplugin/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.3/openplugin/__main__.py
+-rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.3/openplugin/api/__init__.py
+-rw-r--r--   0        0        0      997 2023-05-31 17:20:23.760389 openplugin-0.0.3/openplugin/api/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      527 2023-05-31 17:20:23.802639 openplugin-0.0.3/openplugin/api/__pycache__/http_error.cpython-39.pyc
+-rw-r--r--   0        0        0     1087 2023-05-31 17:20:23.802009 openplugin-0.0.3/openplugin/api/__pycache__/imprompt.cpython-39.pyc
+-rw-r--r--   0        0        0     1068 2023-05-31 17:20:23.761199 openplugin-0.0.3/openplugin/api/__pycache__/langchain.cpython-39.pyc
+-rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.3/openplugin/api/http_error.py
+-rw-r--r--   0        0        0      874 2023-06-01 14:05:00.648019 openplugin-0.0.3/openplugin/api/imprompt.py
+-rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.3/openplugin/api/langchain.py
+-rw-r--r--   0        0        0     6742 2023-05-31 17:20:23.751111 openplugin-0.0.3/openplugin/bindings/imprompt/__pycache__/imprompt_plugin_selector.cpython-39.pyc
+-rw-r--r--   0        0        0     8095 2023-05-31 17:14:33.045786 openplugin-0.0.3/openplugin/bindings/imprompt/imprompt_plugin_selector.py
+-rw-r--r--   0        0        0     4468 2023-06-01 14:01:53.279483 openplugin-0.0.3/openplugin/bindings/langchain/__pycache__/langchain_plugin_selector.cpython-39.pyc
+-rw-r--r--   0        0        0     5324 2023-05-31 20:38:23.595623 openplugin-0.0.3/openplugin/bindings/langchain/langchain_plugin_selector.py
+-rw-r--r--   0        0        0     8202 2023-05-31 17:20:13.387156 openplugin-0.0.3/openplugin/interfaces/__pycache__/plugin_selector.cpython-39.pyc
+-rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.3/openplugin/interfaces/plugin_selector.py
+-rw-r--r--   0        0        0      562 2023-05-31 19:01:14.915142 openplugin-0.0.3/openplugin/main.py
+-rw-r--r--   0        0        0      981 2023-06-01 14:35:38.650961 openplugin-0.0.3/openplugin/utils/run_plugin_selector.py
+-rw-r--r--   0        0        0      521 2023-06-01 14:38:20.672191 openplugin-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.3/PKG-INFO
```

### Comparing `openplugin-0.0.2/README.md` & `openplugin-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.2/openplugin/__init__.py` & `openplugin-0.0.3/openplugin/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from openplugin.interfaces.plugin_selector import MessageType, PluginSelector, PluginOperation, Response, Message, LLM, Plugin, \
-    ToolSelectorConfig, Config, LLMProvider, ToolSelectorProvider
-from openplugin.bindings.langchain.langchain_plugin_selector import LangchainPluginSelector
+from openplugin.utils.run_plugin_selector import run_plugin_selector
 from openplugin.bindings.imprompt.imprompt_plugin_selector import ImpromptPluginSelector
+from openplugin.bindings.langchain.langchain_plugin_selector import LangchainPluginSelector
+from openplugin.interfaces.plugin_selector import MessageType, PluginSelector, PluginOperation, Response, Message, LLM, \
+    Plugin, ToolSelectorConfig, Config, LLMProvider, ToolSelectorProvider
 
 __all__ = (
     "PluginSelector",
     "MessageType",
     "PluginOperation",
     "Response",
     "Message",
     "LLM",
     "Plugin",
     "ToolSelectorConfig",
     "Config",
     "LLMProvider",
     "ToolSelectorProvider",
     "LangchainPluginSelector",
-    "ImpromptPluginSelector"
+    "ImpromptPluginSelector",
+    "run_plugin_selector"
 )
```

### Comparing `openplugin-0.0.2/openplugin/api/__init__.py` & `openplugin-0.0.3/openplugin/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.2/openplugin/api/imprompt.py` & `openplugin-0.0.3/openplugin/api/imprompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,7 +23,8 @@
     selector = ImpromptPluginSelector(tool_selector_config, plugins, config, llm)
     try:
         response = selector.run(messages)
         return response
     except Exception as e:
         print(e)
         return JSONResponse(status_code=500, content={"message": "Failed to run plugin"})
+
```

### Comparing `openplugin-0.0.2/openplugin/api/langchain.py` & `openplugin-0.0.3/openplugin/api/langchain.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.2/openplugin/bindings/imprompt/imprompt_plugin_selector.py` & `openplugin-0.0.3/openplugin/bindings/imprompt/imprompt_plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.2/openplugin/bindings/langchain/langchain_plugin_selector.py` & `openplugin-0.0.3/openplugin/bindings/langchain/langchain_plugin_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         return AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION
     raise ValueError(f"Pipeline name {pipeline_name} not supported")
 
 
 def _get_llm(llm: LLM, api_key: str):
     if llm.provider == LLMProvider.OpenAI:
         if api_key is None:
-            api_key=os.environ["OPENAPI_KEY"]
+            api_key = os.environ["OPENAPI_KEY"]
         os.environ["OPENAI_API_KEY"] = api_key
         llm = OpenAI(
             model_name=llm.model_name,
             temperature=llm.temperature,
             max_tokens=llm.max_tokens,
             top_p=llm.top_p,
             frequency_penalty=llm.frequency_penalty,
```

### Comparing `openplugin-0.0.2/openplugin/interfaces/plugin_selector.py` & `openplugin-0.0.3/openplugin/interfaces/plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.2/openplugin/main.py` & `openplugin-0.0.3/openplugin/main.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.2/pyproject.toml` & `openplugin-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openplugin"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["shrikant <shrikant.pm14@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain = "^0.0.178"
```

### Comparing `openplugin-0.0.2/PKG-INFO` & `openplugin-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

