# Comparing `tmp/openplugin-0.0.4.tar.gz` & `tmp/openplugin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-0.0.4.tar", max compression
+gzip compressed data, was "openplugin-0.0.5.tar", max compression
```

## Comparing `openplugin-0.0.4.tar` & `openplugin-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,14 @@
--rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.4/README.md
--rw-r--r--   0        0        0      754 2023-06-01 14:44:47.992850 openplugin-0.0.4/openplugin/__init__.py
--rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.4/openplugin/__main__.py
--rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.4/openplugin/api/__init__.py
--rw-r--r--   0        0        0      997 2023-05-31 17:20:23.760389 openplugin-0.0.4/openplugin/api/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      527 2023-05-31 17:20:23.802639 openplugin-0.0.4/openplugin/api/__pycache__/http_error.cpython-39.pyc
--rw-r--r--   0        0        0     1087 2023-05-31 17:20:23.802009 openplugin-0.0.4/openplugin/api/__pycache__/imprompt.cpython-39.pyc
--rw-r--r--   0        0        0     1068 2023-05-31 17:20:23.761199 openplugin-0.0.4/openplugin/api/__pycache__/langchain.cpython-39.pyc
--rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.4/openplugin/api/http_error.py
--rw-r--r--   0        0        0      874 2023-06-01 14:05:00.648019 openplugin-0.0.4/openplugin/api/imprompt.py
--rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.4/openplugin/api/langchain.py
--rw-r--r--   0        0        0     6742 2023-05-31 17:20:23.751111 openplugin-0.0.4/openplugin/bindings/imprompt/__pycache__/imprompt_plugin_selector.cpython-39.pyc
--rw-r--r--   0        0        0     8095 2023-05-31 17:14:33.045786 openplugin-0.0.4/openplugin/bindings/imprompt/imprompt_plugin_selector.py
--rw-r--r--   0        0        0     4468 2023-06-01 14:01:53.279483 openplugin-0.0.4/openplugin/bindings/langchain/__pycache__/langchain_plugin_selector.cpython-39.pyc
--rw-r--r--   0        0        0     5324 2023-05-31 20:38:23.595623 openplugin-0.0.4/openplugin/bindings/langchain/langchain_plugin_selector.py
--rw-r--r--   0        0        0     8202 2023-05-31 17:20:13.387156 openplugin-0.0.4/openplugin/interfaces/__pycache__/plugin_selector.cpython-39.pyc
--rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.4/openplugin/interfaces/plugin_selector.py
--rw-r--r--   0        0        0      562 2023-05-31 19:01:14.915142 openplugin-0.0.4/openplugin/main.py
--rw-r--r--   0        0        0      954 2023-06-01 14:44:16.146371 openplugin-0.0.4/openplugin/utils/run_plugin_selector.py
--rw-r--r--   0        0        0      521 2023-06-01 14:44:56.336706 openplugin-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.5/README.md
+-rw-r--r--   0        0        0      754 2023-06-01 14:53:19.914449 openplugin-0.0.5/openplugin/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.5/openplugin/__main__.py
+-rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.5/openplugin/api/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.5/openplugin/api/http_error.py
+-rw-r--r--   0        0        0      874 2023-06-01 14:05:00.648019 openplugin-0.0.5/openplugin/api/imprompt.py
+-rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.5/openplugin/api/langchain.py
+-rw-r--r--   0        0        0     8095 2023-05-31 17:14:33.045786 openplugin-0.0.5/openplugin/bindings/imprompt/imprompt_plugin_selector.py
+-rw-r--r--   0        0        0     5324 2023-05-31 20:38:23.595623 openplugin-0.0.5/openplugin/bindings/langchain/langchain_plugin_selector.py
+-rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.5/openplugin/interfaces/plugin_selector.py
+-rw-r--r--   0        0        0      562 2023-05-31 19:01:14.915142 openplugin-0.0.5/openplugin/main.py
+-rw-r--r--   0        0        0      981 2023-06-01 14:48:05.856325 openplugin-0.0.5/openplugin/utils/run_plugin_selector.py
+-rw-r--r--   0        0        0      521 2023-06-01 14:54:03.483611 openplugin-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.5/PKG-INFO
```

### Comparing `openplugin-0.0.4/README.md` & `openplugin-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.4/openplugin/__init__.py` & `openplugin-0.0.5/openplugin/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from openplugin.bindings.imprompt.imprompt_plugin_selector import ImpromptPluginSelector
-from openplugin.bindings.langchain.langchain_plugin_selector import LangchainPluginSelector
 from openplugin.interfaces.plugin_selector import MessageType, PluginSelector, PluginOperation, Response, Message, LLM, \
     Plugin, ToolSelectorConfig, Config, LLMProvider, ToolSelectorProvider
+from openplugin.bindings.imprompt.imprompt_plugin_selector import ImpromptPluginSelector
+from openplugin.bindings.langchain.langchain_plugin_selector import LangchainPluginSelector
 from openplugin.utils.run_plugin_selector import run_plugin_selector
 __all__ = (
     "PluginSelector",
     "MessageType",
     "PluginOperation",
     "Response",
     "Message",
```

### Comparing `openplugin-0.0.4/openplugin/api/__init__.py` & `openplugin-0.0.5/openplugin/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.4/openplugin/api/imprompt.py` & `openplugin-0.0.5/openplugin/api/imprompt.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.4/openplugin/api/langchain.py` & `openplugin-0.0.5/openplugin/api/langchain.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.4/openplugin/bindings/imprompt/imprompt_plugin_selector.py` & `openplugin-0.0.5/openplugin/bindings/imprompt/imprompt_plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.4/openplugin/bindings/langchain/langchain_plugin_selector.py` & `openplugin-0.0.5/openplugin/bindings/langchain/langchain_plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.4/openplugin/interfaces/plugin_selector.py` & `openplugin-0.0.5/openplugin/interfaces/plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.4/openplugin/main.py` & `openplugin-0.0.5/openplugin/main.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.4/openplugin/utils/run_plugin_selector.py` & `openplugin-0.0.5/openplugin/utils/run_plugin_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from openplugin import Message, Plugin, Config, ToolSelectorConfig, LLM
+from openplugin.interfaces.plugin_selector import Message, Plugin, Config, ToolSelectorConfig, LLM
 
 
 def run_plugin_selector(inp_json, binding_name):
     if type(inp_json) == str:
         inp_json = json.loads(inp_json)
     messages = [Message(**m) for m in inp_json["messages"]]
     plugins = [Plugin(**p) for p in inp_json["plugins"]]
```

### Comparing `openplugin-0.0.4/pyproject.toml` & `openplugin-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openplugin"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["shrikant <shrikant.pm14@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain = "^0.0.178"
```

### Comparing `openplugin-0.0.4/PKG-INFO` & `openplugin-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

