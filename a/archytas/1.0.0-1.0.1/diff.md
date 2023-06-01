# Comparing `tmp/archytas-1.0.0.tar.gz` & `tmp/archytas-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-1.0.0.tar", max compression
+gzip compressed data, was "archytas-1.0.1.tar", max compression
```

## Comparing `archytas-1.0.0.tar` & `archytas-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32472 2023-05-31 19:52:28.418704 archytas-1.0.0/LICENSE
--rw-r--r--   0        0        0     2088 2023-05-31 19:52:28.418704 archytas-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/__init__.py
--rw-r--r--   0        0        0     8291 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/agent.py
--rw-r--r--   0        0        0     9746 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/demo_tools.py
--rw-r--r--   0        0        0     4129 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/prompt.py
--rw-r--r--   0        0        0     3166 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/python.py
--rw-r--r--   0        0        0     7521 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/react.py
--rw-r--r--   0        0        0     1462 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/repl.py
--rw-r--r--   0        0        0    18506 2023-05-31 19:52:28.422704 archytas-1.0.0/archytas/tool_utils.py
--rw-r--r--   0        0        0     4586 2023-05-31 19:52:28.422704 archytas-1.0.0/archytas/tools.py
--rw-r--r--   0        0        0     1251 2023-05-31 19:52:28.422704 archytas-1.0.0/archytas/utils.py
--rw-r--r--   0        0        0      780 2023-05-31 19:52:28.458704 archytas-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-06-01 14:07:03.452519 archytas-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2088 2023-06-01 14:07:03.452519 archytas-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/__init__.py
+-rw-r--r--   0        0        0     9054 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/agent.py
+-rw-r--r--   0        0        0     9746 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/demo_tools.py
+-rw-r--r--   0        0        0     4129 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/prompt.py
+-rw-r--r--   0        0        0     3166 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/python.py
+-rw-r--r--   0        0        0     7630 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/react.py
+-rw-r--r--   0        0        0     1462 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/repl.py
+-rw-r--r--   0        0        0    18506 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/tool_utils.py
+-rw-r--r--   0        0        0     4586 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/tools.py
+-rw-r--r--   0        0        0     1251 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/utils.py
+-rw-r--r--   0        0        0      780 2023-06-01 14:07:03.512519 archytas-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-1.0.1/PKG-INFO
```

### Comparing `archytas-1.0.0/LICENSE` & `archytas-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/README.md` & `archytas-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/archytas/agent.py` & `archytas-1.0.1/archytas/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import openai
 import logging
 from openai.error import Timeout, APIError, APIConnectionError, RateLimitError, ServiceUnavailableError
 from tenacity import before_sleep_log, retry as tenacity_retry, retry_if_exception_type as retry_if, stop_after_attempt, wait_exponential
-from typing import Literal, Callable, ContextManager
+from typing import Callable, ContextManager
 from enum import Enum
 
+from rich import print as rprint
 from rich.spinner import Spinner
 from rich.live import Live
 
 
 logger = logging.getLogger(__name__)
 retry = tenacity_retry(
     reraise=True,
@@ -40,42 +41,54 @@
 def cli_spinner(): 
     return Live(Spinner('dots', speed=2, text="thinking..."), refresh_per_second=30, transient=True)
 class no_spinner:
     def __enter__(self): pass
     def __exit__(self, *args): pass
 
 class Agent:
-    def __init__(self, *, model:str='gpt-4', prompt:str="You are a helpful assistant.", api_key:str|None=None, spinner:Callable[[], ContextManager]|None=cli_spinner):
+    def __init__(self, *, model:str='gpt-4', prompt:str="You are a helpful assistant.", api_key:str|None=None, spinner:Callable[[], ContextManager]|None=cli_spinner, rich_print:bool=True):
         """
         Agent class for managing communication with OpenAI's API.
 
         Args:
             model (str, optional): The name of the model to use. Defaults to 'gpt-4'. At present, GPT-4 is the only model that works reliably.
             prompt (str, optional): The prompt to use when starting a new conversation. Defaults to "You are a helpful assistant.".
             api_key (str, optional): The OpenAI API key to use. Defaults to None. If None, the API key will be read from the OPENAI_API_KEY environment variable.
+            spinner ((fn -> ContextManager) | None, optional): A function that returns a context manager that is run every time the LLM is generating a response. Defaults to cli_spinner which is used to display a spinner in the terminal.
+            rich_print (bool, optional): Whether to use rich to print messages. Defaults to True. Can also be set via the DISABLE_RICH_PRINT environment variable.
 
         Raises:
             Exception: If no API key is given.
         """
 
+        self.rich_print = bool(rich_print and not os.environ.get("DISABLE_RICH_PRINT", False))
         self.model = model
         self.system_message = Message(role=Role.system, content=prompt)
         self.messages: list[Message] = []
-        self.spinner = spinner if spinner is not None else no_spinner
+        if spinner is not None and self.rich_print:
+            self.spinner = spinner
+        else:
+            self.spinner = no_spinner
 
         # use to generate unique ids for context messages
         self._current_context_id = 0
 
         # check that an api key was given, and set it
         if api_key is None:
             api_key = os.environ.get('OPENAI_API_KEY', None)
         if not api_key:
             raise Exception("No OpenAI API key given. Please set the OPENAI_API_KEY environment variable or pass the api_key argument to the Agent constructor.")
         openai.api_key = api_key
 
+    def print(self, *args, **kwargs):
+        if self.rich_print:
+            rprint(*args, **kwargs)
+        else:
+            print(*args, **kwargs)
+
     def new_context_id(self) -> int:
         """Generate a new context id."""
         self._current_context_id += 1
         return self._current_context_id
 
     def add_context(self, context:str, *, lifetime:int|None=None) -> int:
         """
```

### Comparing `archytas-1.0.0/archytas/demo_tools.py` & `archytas-1.0.1/archytas/demo_tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/archytas/prompt.py` & `archytas-1.0.1/archytas/prompt.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/archytas/python.py` & `archytas-1.0.1/archytas/python.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/archytas/react.py` & `archytas-1.0.1/archytas/react.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from archytas.agent import Agent
 from archytas.prompt import build_prompt, build_all_tool_names
 from archytas.tools import ask_user
 from archytas.tool_utils import make_tool_dict
 import json
-from rich import print
 import pdb
 import sys
 import logging
 
 logger = logging.Logger('archytas')
 
 class FailedTaskError(Exception): ...
@@ -102,15 +101,15 @@
             except AssertionError as e:
                 action_str = self.error(str(e))
                 continue
 
             # print action
             if self.verbose:
                 #TODO: better coloring
-                print(f"thought: {thought}\ntool: {tool_name}\ntool_input: {tool_input}\n")
+                self.print(f"thought: {thought}\ntool: {tool_name}\ntool_input: {tool_input}\n")
 
             # exit ReAct loop if agent says final_answer or fail_task
             if tool_name == 'final_answer':
                 return tool_input
             if tool_name == 'fail_task':
                 raise FailedTaskError(tool_input)
 
@@ -138,15 +137,15 @@
             if controller.state == LoopController.STOP_SUCCESS:
                 return tool_output
             if controller.state == LoopController.STOP_FATAL:
                 raise FailedTaskError(tool_output)
 
             # have the agent observe the result, and get the next action
             if self.verbose:
-                print(f"observation: {tool_output}\n")
+                self.print(f"observation: {tool_output}\n")
             action_str = self.observe(tool_output)
 
 
     @staticmethod
     def extract_action(action:dict) -> tuple[str, str, str]:
         """Verify that action has the correct keys. Otherwise, raise an error"""
         assert isinstance(action, dict), f"Action must be a json dictionary, got {type(action)}"
@@ -176,11 +175,15 @@
     def error(self, mesg) -> str:
         """error handling. If too many errors, break the ReAct loop. Otherwise tell the agent, and continue"""
 
         self.errors += 1
         if self.errors >= self.max_errors:
             raise FailedTaskError(f"Too many errors during task. Last error: {mesg}")
         if self.verbose:
-            print(f"[red]error: {mesg}[/red]", file=sys.stderr)
+            if self.rich_print:
+                self.print(f"[red]error: {mesg}[/red]", file=sys.stderr)
+            else:
+                self.print(f"error: {mesg}", file=sys.stderr)
+
 
         #tell the agent about the error, and get its response (call parent .error method)
         return super().error(mesg)
```

### Comparing `archytas-1.0.0/archytas/repl.py` & `archytas-1.0.1/archytas/repl.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/archytas/tool_utils.py` & `archytas-1.0.1/archytas/tool_utils.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/archytas/tools.py` & `archytas-1.0.1/archytas/tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/archytas/utils.py` & `archytas-1.0.1/archytas/utils.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.0/pyproject.toml` & `archytas-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "1.0.0"
+version = "1.0.1"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
```

### Comparing `archytas-1.0.0/PKG-INFO` & `archytas-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

