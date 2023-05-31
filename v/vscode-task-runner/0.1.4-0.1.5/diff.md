# Comparing `tmp/vscode_task_runner-0.1.4.tar.gz` & `tmp/vscode_task_runner-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vscode_task_runner-0.1.4.tar", max compression
+gzip compressed data, was "vscode_task_runner-0.1.5.tar", max compression
```

## Comparing `vscode_task_runner-0.1.4.tar` & `vscode_task_runner-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/LICENSE
--rw-r--r--   0        0        0     7680 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/README.md
--rw-r--r--   0        0        0     1332 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/__init__.py
--rw-r--r--   0        0        0       39 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/__main__.py
--rw-r--r--   0        0        0     2756 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/console.py
--rw-r--r--   0        0        0     1551 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/constants.py
--rw-r--r--   0        0        0     1193 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/executor.py
--rw-r--r--   0        0        0     3740 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/helpers.py
--rw-r--r--   0        0        0     1835 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/json_parser.py
--rw-r--r--   0        0        0     1464 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/models.py
--rw-r--r--   0        0        0     9296 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/task.py
--rw-r--r--   0        0        0     7497 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/terminal_task_system.py
--rw-r--r--   0        0        0     8651 1970-01-01 00:00:00.000000 vscode_task_runner-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-31 23:04:21.629002 vscode_task_runner-0.1.5/LICENSE
+-rw-r--r--   0        0        0     7679 2023-05-31 23:04:21.629002 vscode_task_runner-0.1.5/README.md
+-rw-r--r--   0        0        0     1331 2023-05-31 23:04:21.629002 vscode_task_runner-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/__main__.py
+-rw-r--r--   0        0        0     2780 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/console.py
+-rw-r--r--   0        0        0     1557 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/constants.py
+-rw-r--r--   0        0        0     1199 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/executor.py
+-rw-r--r--   0        0        0     3981 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/helpers.py
+-rw-r--r--   0        0        0     1842 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/json_parser.py
+-rw-r--r--   0        0        0     1489 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/models.py
+-rw-r--r--   0        0        0     9315 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/task.py
+-rw-r--r--   0        0        0     7523 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/terminal_task_system.py
+-rw-r--r--   0        0        0     8749 1970-01-01 00:00:00.000000 vscode_task_runner-0.1.5/PKG-INFO
```

### Comparing `vscode_task_runner-0.1.4/LICENSE` & `vscode_task_runner-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.4/README.md` & `vscode_task_runner-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 source code and reimplemented in Python.
 
 This pairs well with VS Code extensions that add buttons to run tasks such as
 [actboy168.tasks](https://marketplace.visualstudio.com/items?itemName=actboy168.tasks).
 
 ## Usage
 
-Python 3.10+ is required.
+Python 3.8+ is required.
 
 Install with pip/pipx:
 
 ```bash
 pip install vscode-task-runner
 ```
```

### Comparing `vscode_task_runner-0.1.4/pyproject.toml` & `vscode_task_runner-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "vscode-task-runner"
-    version = "0.1.4"
+    version = "0.1.5"
     description = "Task runner for VS Code tasks.json"
     license = "MIT"
     readme = "README.md"
     homepage = "https://github.com/NathanVaughn/vscode-task-runner"
     repository = "https://github.com/NathanVaughn/vscode-task-runner.git"
     authors = ["Nathan Vaughn <nvaughn51@gmail.com>"]
     classifiers = [
@@ -14,15 +14,15 @@
     ]
     packages = [{ include = "vtr" }]
 
 [tool.poetry.urls]
     Issues = "https://github.com/NathanVaughn/vscode-task-runner/issues"
 
 [tool.poetry.dependencies]
-    python      = ">=3.10,<4.0"
+    python      = ">=3.8,<4.0"
     shellingham = "^1.5.0.post1"
     pyjson5     = "^1.6.2"
     dacite      = "^1.8.1"
 
 [tool.poetry.group.dev.dependencies]
     pre-commit  = "^3.2.0"
     pytest      = "^7.3.1"
```

### Comparing `vscode_task_runner-0.1.4/vtr/console.py` & `vscode_task_runner-0.1.5/vtr/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import argparse
 import itertools
 import os
+from typing import Dict
 
 import vtr.executor
 import vtr.json_parser
 from vtr.task import Task
 
 
 def run() -> None:
     task_label_help_text = "One or more task labels to run. This is case sensitive."
 
     # parse the tasks.json
     try:
         all_tasks_data, tasks_json = vtr.json_parser.load_vscode_tasks_data()
         # build task objects
-        all_tasks: dict[str, Task] = {
+        all_tasks: Dict[str, Task] = {
             t["label"]: Task(all_tasks_data, t["label"])
             for t in all_tasks_data["tasks"]
             if t.get("type", "process") in ["process", "shell"]
         }
     except FileNotFoundError:
         all_tasks = {}
         task_label_help_text += (
```

### Comparing `vscode_task_runner-0.1.4/vtr/constants.py` & `vscode_task_runner-0.1.5/vtr/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import platform
-from typing import Literal
+from typing import Dict, Literal
 
 from vtr.models import ShellQuotingOptions, ShellQuotingOptionsEscape, ShellType
 
-PLATFORM_KEYS: dict[
+PLATFORM_KEYS: Dict[
     Literal["Windows", "Linux", "Darwin"], Literal["windows", "linux", "osx"]
 ] = {
     "Windows": "windows",
     "Linux": "linux",
     "Darwin": "osx",
 }
```

### Comparing `vscode_task_runner-0.1.4/vtr/executor.py` & `vscode_task_runner-0.1.5/vtr/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import subprocess
 import sys
-from typing import Optional
+from typing import List, Optional
 
 import vtr.helpers
 from vtr.task import Task
 
 
 def execute_task(
-    task: Task, index: int, total: int, extra_args: Optional[list[str]] = None
+    task: Task, index: int, total: int, extra_args: Optional[List[str]] = None
 ) -> None:
     """
     Execute a given task. A 1-based index and total number of tasks must be provided
     for printing.
     """
     if task.is_virtual:
         print(f'[{index}/{total}] Task "{task.label}" has no direct command to execute')
@@ -25,15 +25,15 @@
     proc = subprocess.run(cmd, shell=False, cwd=task.cwd, env=task.env)
 
     if proc.returncode != 0:
         print(f'Task "{task.label}" returned with exit code {proc.returncode}')
         sys.exit(proc.returncode)
 
 
-def collect_task(task: Task, all_tasks: Optional[list[Task]] = None) -> list[Task]:
+def collect_task(task: Task, all_tasks: Optional[List[Task]] = None) -> List[Task]:
     """
     Given a task, return the given task and all child tasks, recursively.
     """
     if all_tasks is None:
         all_tasks = []
 
     for child_task in task.depends_on:
```

### Comparing `vscode_task_runner-0.1.4/vtr/helpers.py` & `vscode_task_runner-0.1.5/vtr/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import shutil
+from typing import List, Union
 
 import dacite
 import shellingham
 
 import vtr.constants
 from vtr.models import (
     CommandString,
@@ -11,37 +12,43 @@
     ShellConfiguration,
     ShellQuoting,
     ShellType,
 )
 
 
 def identify_shell_type(shell_executable: str) -> ShellType:
+    # sourcery skip: assign-if-exp, reintroduce-else
     """
     Try to identify what type of shell it is based on the executable.
     """
     shell_executable_which = shutil.which(shell_executable)
     if shell_executable_which is None:
         raise FileNotFoundError(f"Shell executable {shell_executable} not found")
 
     shell_executable = shell_executable_which
-    shell_basename = os.path.basename(shell_executable)
+
+    # https://stackoverflow.com/a/41659825
+    shell_basename = os.path.basename(shell_executable.replace("\\", os.path.sep))
+    if shell_basename.endswith(".exe"):
+        # .removesuffix is only available 3.9+
+        shell_basename = shell_basename[:-4]
 
     # don't check for .exe because it could be running powershell
     # core on Linux
-    if any(i in shell_basename for i in ("pwsh", "powershell")):
+    if shell_basename in ["pwsh", "powershell"]:
         return ShellType.PowerShell
 
-    if shell_basename == "cmd.exe":
+    if shell_basename == "cmd":
         return ShellType.CMD
 
-    if shell_basename == "wsl.exe":
+    if shell_basename == "wsl":
         return ShellType.WSL
 
     # bash.exe is a thing on Windows too
-    if shell_basename.endswith("sh") or shell_basename.endswith("sh.exe"):
+    if shell_basename.endswith("sh"):
         return ShellType.SH
 
     return ShellType.Unknown
 
 
 def get_parent_shell() -> ShellConfiguration:
     """
@@ -79,38 +86,38 @@
     # just make sure path is fully resolved
     if shell_executable := shutil.which(shell_executable):
         return ShellConfiguration(executable=shell_executable)
     else:
         raise FileNotFoundError("A shell could not be found")
 
 
-def stringify(value: str | int | float | bool) -> str:
+def stringify(value: Union[str, int, float, bool]) -> str:
     """
     Make sure the incoming value is close enough to a string, and convert it.
     """
 
     if not isinstance(value, (str, int, float, bool)):
         raise ValueError(f"Value '{value}' is not a string/number/boolean")
 
     return str(value)
 
 
-def combine_string(value: str | list[str]) -> str:
+def combine_string(value: Union[str, List[str]]) -> str:
     """
     Given either a single string, or list of string, return a single string.
     A list will be joined by spaces.
     """
     if isinstance(value, str):
         return value
 
     assert all(isinstance(i, str) for i in value)
     return " ".join(value)
 
 
-def load_command_string(data: dict | str | list[str]) -> CommandString:
+def load_command_string(data: Union[dict, str, List[str]]) -> CommandString:
     """
     Given data, either return the string, or loads into a the QuotedString dataclass.
     """
     if isinstance(data, (str, list)):
         return combine_string(data)
 
     elif isinstance(data, dict):
```

### Comparing `vscode_task_runner-0.1.4/vtr/json_parser.py` & `vscode_task_runner-0.1.5/vtr/json_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-from typing import Any
+from typing import Any, Tuple
 
 import pyjson5
 
 import vtr.constants
 
 
 def replace_env_vars(string: str) -> str:
@@ -43,15 +43,15 @@
         for key, value in vtr.constants.PREDEFINED_VARIABLES.items():
             data = data.replace(key, value)
         return replace_env_vars(data)
     else:
         return data
 
 
-def load_vscode_tasks_data(path: str = os.getcwd()) -> tuple[dict, str]:
+def load_vscode_tasks_data(path: str = os.getcwd()) -> Tuple[dict, str]:
     """
     Given a working directory, loads the vscode tasks config, and replaces
     all the variables. Returns raw dict data and the filename that was loaded.
     """
     tasks_json = os.path.join(path, ".vscode", "tasks.json")
 
     if not os.path.isfile(tasks_json):
```

### Comparing `vscode_task_runner-0.1.4/vtr/models.py` & `vscode_task_runner-0.1.5/vtr/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Optional
+from typing import List, Optional, Union
 
 
 @dataclass
 class ShellQuotingOptionsEscape:
     # https://github.com/microsoft/vscode/blob/eef30e7165e19b33daa1e15e92fa34ff4a5df0d3/src/vs/workbench/contrib/tasks/common/tasks.ts#L70-L71
     escape_character: str
-    characters_to_escape: list[str]
+    characters_to_escape: List[str]
 
 
 @dataclass
 class ShellQuotingOptions:
     # https://github.com/microsoft/vscode/blob/eef30e7165e19b33daa1e15e92fa34ff4a5df0d3/src/vs/workbench/contrib/tasks/common/tasks.ts#L65-L83
     strong: Optional[str] = None
-    escape: Optional[ShellQuotingOptionsEscape | str] = None
+    escape: Optional[Union[ShellQuotingOptionsEscape, str]] = None
     weak: Optional[str] = None
 
 
 class ShellQuoting(Enum):
     """
     Enum for shell quoting options
     """
@@ -36,19 +36,19 @@
     WSL = auto()
     Unknown = auto()
 
 
 @dataclass
 class ShellConfiguration:
     executable: Optional[str] = None
-    args: Optional[list[str]] = None
+    args: Optional[List[str]] = None
     quoting: Optional[ShellQuotingOptions] = None
 
 
 @dataclass
 class QuotedString:
     value: str
     quoting: ShellQuoting
 
 
-CommandString = str | QuotedString
+CommandString = Union[str, QuotedString]
 # https://github.com/microsoft/vscode/blob/eef30e7165e19b33daa1e15e92fa34ff4a5df0d3/src/vs/workbench/contrib/tasks/common/tasks.ts#L320
```

### Comparing `vscode_task_runner-0.1.4/vtr/task.py` & `vscode_task_runner-0.1.5/vtr/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 import shutil
-from typing import Any, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional, Tuple
 
 import dacite
 
 import vtr.constants
 import vtr.helpers
 import vtr.terminal_task_system
 from vtr.models import CommandString, ShellConfiguration, ShellType
@@ -104,15 +104,15 @@
         # make sure the working directory exists
         if not os.path.isdir(task_cwd):
             raise FileNotFoundError(f"Working directory '{task_cwd}' does not exist")
 
         return task_cwd
 
     @property
-    def env(self) -> dict[str, str]:
+    def env(self) -> Dict[str, str]:
         """
         Gets the environment variables for the task. This merges with the current
         environment variables.
         """
         # copy the current environment
         env = os.environ.copy()
 
@@ -149,15 +149,15 @@
         """
         Gets the command for the task.
         """
         raw_task_command = self._get_task_setting("command")
         return vtr.helpers.load_command_string(raw_task_command)
 
     @property
-    def args(self) -> list[CommandString]:
+    def args(self) -> List[CommandString]:
         """
         Get the arguments for the task.
         """
         task_args = self._get_task_setting("args")
 
         # no args given
         if task_args is None:
@@ -169,15 +169,15 @@
 
         for i, arg in enumerate(task_args):
             task_args[i] = vtr.helpers.load_command_string(arg)
 
         return task_args
 
     @property
-    def shell(self) -> tuple[ShellConfiguration, ShellType]:
+    def shell(self) -> Tuple[ShellConfiguration, ShellType]:
         """
         Gets the shell configuration the task is going to run under.
         """
         shell_dict = self._get_options_setting("shell")
 
         if shell_dict is not None:
             # if shell settings defined
@@ -199,15 +199,15 @@
             )
 
         assert shell_configuration.executable is not None
         return shell_configuration, vtr.helpers.identify_shell_type(
             shell_configuration.executable
         )
 
-    def subprocess_command(self, extra_args: Optional[list[str]] = None) -> list[str]:
+    def subprocess_command(self, extra_args: Optional[List[str]] = None) -> List[str]:
         """
         Generate the list of strings to pass to subprocess.
         """
         if extra_args is None:
             extra_args = []
 
         if self.type_ == "process":
@@ -267,15 +267,15 @@
                 ),
             )
 
         else:
             raise ValueError("Unsupported task type")
 
     @property
-    def depends_on(self) -> list[Task]:
+    def depends_on(self) -> List[Task]:
         """
         Return a list of tasks this task depends on.
         """
         depends_on_setting = self._get_task_setting("dependsOn")
 
         # return empty list if not set
         if depends_on_setting is None:
```

### Comparing `vscode_task_runner-0.1.4/vtr/terminal_task_system.py` & `vscode_task_runner-0.1.5/vtr/terminal_task_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This file has functions from
 vscode/src/vs/workbench/contrib/tasks/browser/terminalTaskSystem.ts
 re-implemented in Python.
 """
 
 import copy
 import re
-from typing import Optional
+from typing import List, Optional, Tuple, Union
 
 import vtr.constants
 from vtr.models import (
     CommandString,
     ShellConfiguration,
     ShellQuoting,
     ShellQuotingOptions,
@@ -32,16 +32,16 @@
     else:
         shell_config.quoting = vtr.constants.DEFAULT_OS_QUOTING[
             vtr.constants.PLATFORM_KEY
         ]
 
 
 def _add_all_argument(
-    shell_command_args: list[str], configured_shell_args: list[str]
-) -> list[str]:
+    shell_command_args: List[str], configured_shell_args: List[str]
+) -> List[str]:
     # https://github.com/microsoft/vscode/blob/eef30e7165e19b33daa1e15e92fa34ff4a5df0d3/src/vs/workbench/contrib/tasks/browser/terminalTaskSystem.ts#L1256-L1272
 
     # converted with ChatGPT
     combined_shell_args = copy.deepcopy(configured_shell_args)
     for element in shell_command_args:
         should_add_shell_command_arg = all(
             (arg.lower() != element)
@@ -59,25 +59,25 @@
         if should_add_shell_command_arg:
             combined_shell_args.append(element)
 
     return combined_shell_args
 
 
 def create_shell_launch_config(
-    shell_type: ShellType, shell_args: list[str] | str, command_line: str
-) -> list[str]:
+    shell_type: ShellType, shell_args: Union[List[str], str], command_line: str
+) -> List[str]:
     # https://github.com/microsoft/vscode/blob/eef30e7165e19b33daa1e15e92fa34ff4a5df0d3/src/vs/workbench/contrib/tasks/browser/terminalTaskSystem.ts#L1107-L1177
 
     # manually converted and simplified
 
     # convert a single shell args string into a list
     if isinstance(shell_args, str):
         shell_args = [shell_args]
 
-    to_add: list[str] = []
+    to_add: List[str] = []
 
     # skip all this if the user has already manually specific arguments
     if not shell_args:
         # this cannot happen in our case, since we don't have default
         # arguments loaded from settings.
 
         # Under Mac remove -l to not start it as a login shell.
@@ -103,15 +103,15 @@
     return combined_shell_args
 
 
 def build_shell_command_line(
     shell_type: ShellType,
     shell_quoting_options: ShellQuotingOptions,
     task_command: CommandString,
-    args: list[CommandString],
+    args: List[CommandString],
 ) -> str:
     # Python re-implementation of
     # https://github.com/microsoft/vscode/blob/ab7c32a5b5275c3fa9552675b6b6035888068fd7/src/vs/workbench/contrib/tasks/browser/terminalTaskSystem.ts#L1476-L1573
 
     # Largely done by ChatGPT with some manual tweaks
 
     def needs_quotes(value: str) -> bool:
@@ -149,15 +149,15 @@
                 shell_quoting_options.weak,
             ]:
                 quote = ch
             elif ch == " ":
                 return True
         return False
 
-    def quote(value: str, kind: ShellQuoting) -> tuple[str, bool]:
+    def quote(value: str, kind: ShellQuoting) -> Tuple[str, bool]:
         if kind == ShellQuoting.Strong and shell_quoting_options.strong:
             return (
                 shell_quoting_options.strong + value + shell_quoting_options.strong,
                 True,
             )
         elif kind == ShellQuoting.Weak and shell_quoting_options.weak:
             return (
@@ -174,15 +174,15 @@
             escape_char = shell_quoting_options.escape.escape_character
             return (
                 regexp.sub(lambda match: escape_char + match.group(), value),
                 True,
             )
         return (value, False)
 
-    def quote_if_necessary(value: CommandString) -> tuple[str, bool]:
+    def quote_if_necessary(value: CommandString) -> Tuple[str, bool]:
         if isinstance(value, str):
             if needs_quotes(value):
                 # default of strong quoting
                 return quote(value, ShellQuoting.Strong)
             else:
                 return (value, False)
         else:
@@ -191,15 +191,15 @@
     # If we have no args and the command is a string then use the command to stay
     # backwards compatible with the old command line model. To allow variable resolving
     # with spaces we do continue if the resolved value is different than the original
     # one and the resolved one needs quoting.
     if not args and isinstance(task_command, str):
         return task_command
 
-    result: list[str] = []
+    result: List[str] = []
     command_quoted = False
     arg_quoted = False
     value, quoted = quote_if_necessary(task_command)
     result.append(value)
     command_quoted = quoted
     for arg in args:
         value, quoted = quote_if_necessary(arg)
```

### Comparing `vscode_task_runner-0.1.4/PKG-INFO` & `vscode_task_runner-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: vscode-task-runner
-Version: 0.1.4
+Version: 0.1.5
 Summary: Task runner for VS Code tasks.json
 Home-page: https://github.com/NathanVaughn/vscode-task-runner
 License: MIT
 Author: Nathan Vaughn
 Author-email: nvaughn51@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: pyjson5 (>=1.6.2,<2.0.0)
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
@@ -42,15 +44,15 @@
 source code and reimplemented in Python.
 
 This pairs well with VS Code extensions that add buttons to run tasks such as
 [actboy168.tasks](https://marketplace.visualstudio.com/items?itemName=actboy168.tasks).
 
 ## Usage
 
-Python 3.10+ is required.
+Python 3.8+ is required.
 
 Install with pip/pipx:
 
 ```bash
 pip install vscode-task-runner
 ```
```

