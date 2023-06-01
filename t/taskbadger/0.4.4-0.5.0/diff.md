# Comparing `tmp/taskbadger-0.4.4.tar.gz` & `tmp/taskbadger-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbadger-0.4.4.tar", max compression
+gzip compressed data, was "taskbadger-0.5.0.tar", max compression
```

## Comparing `taskbadger-0.4.4.tar` & `taskbadger-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-05-24 19:36:29.577478 taskbadger-0.4.4/LICENSE
--rw-r--r--   0        0        0     1649 2023-05-24 19:36:29.577478 taskbadger-0.4.4/README.md
--rw-r--r--   0        0        0     1808 2023-05-24 19:36:29.577478 taskbadger-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      462 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/__init__.py
--rw-r--r--   0        0        0     5175 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/cli.py
--rw-r--r--   0        0        0     3253 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/config.py
--rw-r--r--   0        0        0      250 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/exceptions.py
--rw-r--r--   0        0        0     1008 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/integrations.py
--rw-r--r--   0        0        0      155 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/__init__.py
--rw-r--r--   0        0        0       47 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/__init__.py
--rw-r--r--   0        0        0     3318 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_cancel.py
--rw-r--r--   0        0        0     5393 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_create.py
--rw-r--r--   0        0        0     5005 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_get.py
--rw-r--r--   0        0        0     5097 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_list.py
--rw-r--r--   0        0        0     5676 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_partial_update.py
--rw-r--r--   0        0        0     5556 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_update.py
--rw-r--r--   0        0        0        0 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/__init__.py
--rw-r--r--   0        0        0     3123 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_cancel.py
--rw-r--r--   0        0        0     5770 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_create.py
--rw-r--r--   0        0        0     4662 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_get.py
--rw-r--r--   0        0        0     5872 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_list.py
--rw-r--r--   0        0        0     5359 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_partial_update.py
--rw-r--r--   0        0        0     5167 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_update.py
--rw-r--r--   0        0        0     2673 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/client.py
--rw-r--r--   0        0        0      282 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/errors.py
--rw-r--r--   0        0        0     1022 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/__init__.py
--rw-r--r--   0        0        0     3234 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/action.py
--rw-r--r--   0        0        0     1152 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/action_config.py
--rw-r--r--   0        0        0     2405 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/action_request.py
--rw-r--r--   0        0        0     1190 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/action_request_config.py
--rw-r--r--   0        0        0     2590 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/paginated_task_list.py
--rw-r--r--   0        0        0     2638 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/patched_action_request.py
--rw-r--r--   0        0        0     1228 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/patched_action_request_config.py
--rw-r--r--   0        0        0     6107 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/patched_task_request.py
--rw-r--r--   0        0        0     1222 2023-05-24 19:36:29.577478 taskbadger-0.4.4/taskbadger/internal/models/patched_task_request_data.py
--rw-r--r--   0        0        0      339 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/internal/models/status_enum.py
--rw-r--r--   0        0        0     7435 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/internal/models/task.py
--rw-r--r--   0        0        0     1146 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/internal/models/task_data.py
--rw-r--r--   0        0        0     5965 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/internal/models/task_request.py
--rw-r--r--   0        0        0     1184 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/internal/models/task_request_data.py
--rw-r--r--   0        0        0       26 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/internal/py.typed
--rw-r--r--   0        0        0      974 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/internal/types.py
--rw-r--r--   0        0        0     1176 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/safe_sdk.py
--rw-r--r--   0        0        0    10426 2023-05-24 19:36:29.581478 taskbadger-0.4.4/taskbadger/sdk.py
--rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 taskbadger-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 14:47:47.951661 taskbadger-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1716 2023-06-01 14:47:47.951661 taskbadger-0.5.0/README.md
+-rw-r--r--   0        0        0     1808 2023-06-01 14:47:47.955661 taskbadger-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      482 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/__init__.py
+-rw-r--r--   0        0        0     5153 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/cli.py
+-rw-r--r--   0        0        0     3253 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/config.py
+-rw-r--r--   0        0        0      299 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/exceptions.py
+-rw-r--r--   0        0        0     2158 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/integrations.py
+-rw-r--r--   0        0        0      155 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/__init__.py
+-rw-r--r--   0        0        0     3318 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_cancel.py
+-rw-r--r--   0        0        0     5393 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_create.py
+-rw-r--r--   0        0        0     5005 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_get.py
+-rw-r--r--   0        0        0     5097 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_list.py
+-rw-r--r--   0        0        0     5676 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_partial_update.py
+-rw-r--r--   0        0        0     5556 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_update.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/__init__.py
+-rw-r--r--   0        0        0     3123 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_cancel.py
+-rw-r--r--   0        0        0     5770 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_create.py
+-rw-r--r--   0        0        0     4662 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_get.py
+-rw-r--r--   0        0        0     5872 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_list.py
+-rw-r--r--   0        0        0     5359 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_partial_update.py
+-rw-r--r--   0        0        0     5167 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_update.py
+-rw-r--r--   0        0        0     2673 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/client.py
+-rw-r--r--   0        0        0      282 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/errors.py
+-rw-r--r--   0        0        0     1022 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/__init__.py
+-rw-r--r--   0        0        0     3234 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/action.py
+-rw-r--r--   0        0        0     1152 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/action_config.py
+-rw-r--r--   0        0        0     2405 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/action_request.py
+-rw-r--r--   0        0        0     1190 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/action_request_config.py
+-rw-r--r--   0        0        0     2590 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/paginated_task_list.py
+-rw-r--r--   0        0        0     2638 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/patched_action_request.py
+-rw-r--r--   0        0        0     1228 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/patched_action_request_config.py
+-rw-r--r--   0        0        0     6107 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/patched_task_request.py
+-rw-r--r--   0        0        0     1222 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/patched_task_request_data.py
+-rw-r--r--   0        0        0      339 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/status_enum.py
+-rw-r--r--   0        0        0     7435 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/task.py
+-rw-r--r--   0        0        0     1146 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/task_data.py
+-rw-r--r--   0        0        0     5965 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/task_request.py
+-rw-r--r--   0        0        0     1184 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/task_request_data.py
+-rw-r--r--   0        0        0       26 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/py.typed
+-rw-r--r--   0        0        0      974 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/types.py
+-rw-r--r--   0        0        0     1185 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/safe_sdk.py
+-rw-r--r--   0        0        0    10444 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/sdk.py
+-rw-r--r--   0        0        0     3131 1970-01-01 00:00:00.000000 taskbadger-0.5.0/PKG-INFO
```

### Comparing `taskbadger-0.4.4/LICENSE` & `taskbadger-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/README.md` & `taskbadger-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,27 +27,25 @@
     token="***"
 )
 ```
 
 #### API Example
 
 ```python
-from taskbadger import Task, Action, EmailIntegration
+from taskbadger import Task, Action, EmailIntegration, WebhookIntegration
 
 # create a new task with custom data and an action definition
 task = Task.create(
     "task name",
     data={
         "custom": "data"
     },
     actions=[
-        Action(
-            "*/10%,success,error",
-            integration=EmailIntegration(to="me@example.com")
-        )
+        Action("*/10%,success,error", integration=EmailIntegration(to="me@example.com")),
+        Action("cancelled", integration=WebhookIntegration(id="webhook:demo")),
     ]
 )
 
 # update the task status to 'processing' and set the value to 0
 task.started()
 try:
    for i in range(100):
```

### Comparing `taskbadger-0.4.4/pyproject.toml` & `taskbadger-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskbadger"
-version = "0.4.4"
+version = "0.5.0"
 description = "The official Python SDK for Task Badger"
 license = "Apache-2.0"
 
 authors = []
 
 readme = "README.md"
 packages = [
```

### Comparing `taskbadger-0.4.4/taskbadger/cli.py` & `taskbadger-0.5.0/taskbadger/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 @app.command(context_settings={"allow_extra_args": True, "ignore_unknown_options": False})
 def run(
     ctx: typer.Context,
     name: str,
     monitor_id: str = typer.Option(None, help="Associate this task with a monitor."),
     update_frequency: int = typer.Option(5, metavar="SECONDS", min=5, max=300, help="Seconds between updates."),
-    action_def: Tuple[str, integrations.Integrations, str] = typer.Option(
+    action_def: Tuple[str, str, str] = typer.Option(
         (None, None, None),
         "--action",
         "-a",
         metavar="<trigger integration config>",
         show_default=False,
         help="Action definition e.g. 'success,error email to:me@email.com'",
     ),
@@ -59,15 +59,15 @@
 
     Example:
 
         [on black]taskbadger run 'my task' -- ./my-script.sh arg -v[/]
     """
     _configure_api(ctx)
     action = None
-    if all(action_def):
+    if any(action_def):
         trigger, integration, config = action_def
         action = Action(trigger, integrations.from_config(integration, config))
     stale_timeout = update_frequency * 2
     try:
         task = Task.create(
             name,
             status=StatusEnum.PROCESSING,
```

### Comparing `taskbadger-0.4.4/taskbadger/config.py` & `taskbadger-0.5.0/taskbadger/config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/integrations.py` & `taskbadger-0.5.0/taskbadger/internal/models/patched_action_request_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-import dataclasses
-from enum import Enum
-from typing import Any, Dict
+from typing import Any, Dict, List, Type, TypeVar
 
-from taskbadger.internal.models import ActionRequest, ActionRequestConfig
+import attr
 
+T = TypeVar("T", bound="PatchedActionRequestConfig")
 
-class Integrations(str, Enum):
-    email = "email"
 
+@attr.s(auto_attribs=True)
+class PatchedActionRequestConfig:
+    """ """
 
-def from_config(integration: Integrations, config: str):
-    if integration == Integrations.email:
-        split_ = [tuple(item.split(":", 1)) for item in config.split(",")]
-        kwargs = dict(split_)
-        return EmailIntegration(**kwargs)
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
+    def to_dict(self) -> Dict[str, Any]:
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
 
-class Integration:
-    name: str
+        return field_dict
 
-    def request_config(self):
-        raise NotImplementedError
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        patched_action_request_config = cls()
 
+        patched_action_request_config.additional_properties = d
+        return patched_action_request_config
 
-@dataclasses.dataclass
-class Action:
-    trigger: str
-    integration: Integration
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
 
-    def to_dict(self) -> Dict[str, Any]:
-        return ActionRequest(self.trigger, self.integration.name, self.integration.request_config()).to_dict()
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
 
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
 
-@dataclasses.dataclass
-class EmailIntegration(Integration):
-    name = "email"
-    to: str  # custom type
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
 
-    def request_config(self) -> ActionRequestConfig:
-        return ActionRequestConfig.from_dict({"to": self.to})
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_cancel.py` & `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_cancel.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_create.py` & `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_create.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_get.py` & `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_get.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_list.py` & `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_partial_update.py` & `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_partial_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/action_endpoints/action_update.py` & `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_cancel.py` & `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_cancel.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_create.py` & `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_create.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_get.py` & `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_get.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_list.py` & `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_partial_update.py` & `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_partial_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/api/task_endpoints/task_update.py` & `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/client.py` & `taskbadger-0.5.0/taskbadger/internal/client.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/__init__.py` & `taskbadger-0.5.0/taskbadger/internal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/action.py` & `taskbadger-0.5.0/taskbadger/internal/models/action.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/action_config.py` & `taskbadger-0.5.0/taskbadger/internal/models/action_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/action_request.py` & `taskbadger-0.5.0/taskbadger/internal/models/action_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/action_request_config.py` & `taskbadger-0.5.0/taskbadger/internal/models/action_request_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/paginated_task_list.py` & `taskbadger-0.5.0/taskbadger/internal/models/paginated_task_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/patched_action_request.py` & `taskbadger-0.5.0/taskbadger/internal/models/patched_action_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/patched_action_request_config.py` & `taskbadger-0.5.0/taskbadger/internal/models/patched_task_request_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PatchedActionRequestConfig")
+T = TypeVar("T", bound="PatchedTaskRequestData")
 
 
 @attr.s(auto_attribs=True)
-class PatchedActionRequestConfig:
-    """ """
+class PatchedTaskRequestData:
+    """Custom metadata"""
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        patched_action_request_config = cls()
+        patched_task_request_data = cls()
 
-        patched_action_request_config.additional_properties = d
-        return patched_action_request_config
+        patched_task_request_data.additional_properties = d
+        return patched_task_request_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/patched_task_request.py` & `taskbadger-0.5.0/taskbadger/internal/models/patched_task_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/patched_task_request_data.py` & `taskbadger-0.5.0/taskbadger/internal/models/task_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PatchedTaskRequestData")
+T = TypeVar("T", bound="TaskData")
 
 
 @attr.s(auto_attribs=True)
-class PatchedTaskRequestData:
+class TaskData:
     """Custom metadata"""
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        patched_task_request_data = cls()
+        task_data = cls()
 
-        patched_task_request_data.additional_properties = d
-        return patched_task_request_data
+        task_data.additional_properties = d
+        return task_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/task.py` & `taskbadger-0.5.0/taskbadger/internal/models/task.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/task_data.py` & `taskbadger-0.5.0/taskbadger/internal/models/task_request_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TaskData")
+T = TypeVar("T", bound="TaskRequestData")
 
 
 @attr.s(auto_attribs=True)
-class TaskData:
+class TaskRequestData:
     """Custom metadata"""
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        task_data = cls()
+        task_request_data = cls()
 
-        task_data.additional_properties = d
-        return task_data
+        task_request_data.additional_properties = d
+        return task_request_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `taskbadger-0.4.4/taskbadger/internal/models/task_request.py` & `taskbadger-0.5.0/taskbadger/internal/models/task_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/internal/types.py` & `taskbadger-0.5.0/taskbadger/internal/types.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.4.4/taskbadger/safe_sdk.py` & `taskbadger-0.5.0/taskbadger/safe_sdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 try:
     from typing import ParamSpec
 except ImportError:
     from typing_extensions import ParamSpec
 
 
-from .sdk import Mug, create_task, update_task
+from .sdk import Badger, create_task, update_task
 
 P = ParamSpec("P")
 
 log = logging.getLogger("taskbadger")
 
 
 def create_task_safe(name: str, **kwargs: P.kwargs) -> Optional[str]:
@@ -20,15 +20,15 @@
     Arguments:
         name: The name of the task.
         **kwargs: See [taskbadger.create_task][]
 
     Returns:
         Task ID or None
     """
-    if not Mug.is_configured:
+    if not Badger.is_configured:
         return None
 
     try:
         task = create_task(name, **kwargs)
     except Exception:
         log.exception("Error creating task '%s'", name)
     else:
@@ -38,14 +38,14 @@
 def update_task_safe(task_id: str, **kwargs: P.kwargs) -> None:
     """Safely update a task. Any errors are handled and logged.
 
     Arguments:
         task_id: The ID of the task to update.
         **kwargs: See [taskbadger.update_task][]
     """
-    if not Mug.is_configured:
+    if not Badger.is_configured:
         return
 
     try:
         update_task(task_id, **kwargs)
     except Exception:
         log.exception("Error updating task '%s'", task_id)
```

### Comparing `taskbadger-0.4.4/taskbadger/sdk.py` & `taskbadger-0.5.0/taskbadger/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     organization_slug = organization_slug or os.environ.get("TASKBADGER_ORG")
     project_slug = project_slug or os.environ.get("TASKBADGER_PROJECT")
     token = token or os.environ.get("TASKBADGER_API_KEY")
 
     if host and organization_slug and project_slug and token:
         client = AuthenticatedClient(host, token)
         settings = Settings(client, organization_slug, project_slug)
-        Mug.current.bind(settings)
+        Badger.current.bind(settings)
     else:
         raise ConfigurationError(
             host=host,
             organization_slug=organization_slug,
             project_slug=project_slug,
             token=token,
         )
@@ -157,15 +157,15 @@
     kwargs = _make_args(id=task_id, json_body=body)
     response = task_partial_update.sync_detailed(**kwargs)
     _check_response(response)
     return Task(response.parsed)
 
 
 def _make_args(**kwargs):
-    settings = Mug.current.settings
+    settings = Badger.current.settings
     ret_args = dataclasses.asdict(settings)
     ret_args.update(kwargs)
     return ret_args
 
 
 def _get_settings():
     return _local.get()
@@ -187,34 +187,34 @@
 
 
 class MugMeta(type):
     @property
     def current(cls):
         mug = _local.get(None)
         if mug is None:
-            mug = Mug(GLOBAL_MUG)
+            mug = Badger(GLOBAL_MUG)
             _local.set(mug)
         return mug
 
 
-class Mug(metaclass=MugMeta):
+class Badger(metaclass=MugMeta):
     def __init__(self, settings_or_mug=None):
-        if isinstance(settings_or_mug, Mug):
+        if isinstance(settings_or_mug, Badger):
             self.settings = settings_or_mug.settings
         else:
             self.settings = settings_or_mug
 
     def bind(self, settings):
         self.settings = settings
 
     def is_configured(self):
         return self.settings is not None
 
 
-GLOBAL_MUG = Mug()
+GLOBAL_MUG = Badger()
 _local.set(GLOBAL_MUG)
 
 
 class Task:
     """The Task class provides a convenient Python API to interact
     with Task Badger tasks.
     """
```

### Comparing `taskbadger-0.4.4/PKG-INFO` & `taskbadger-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskbadger
-Version: 0.4.4
+Version: 0.5.0
 Summary: The official Python SDK for Task Badger
 Home-page: https://taskbadger.net/
 License: Apache-2.0
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -59,27 +59,25 @@
     token="***"
 )
 ```
 
 #### API Example
 
 ```python
-from taskbadger import Task, Action, EmailIntegration
+from taskbadger import Task, Action, EmailIntegration, WebhookIntegration
 
 # create a new task with custom data and an action definition
 task = Task.create(
     "task name",
     data={
         "custom": "data"
     },
     actions=[
-        Action(
-            "*/10%,success,error",
-            integration=EmailIntegration(to="me@example.com")
-        )
+        Action("*/10%,success,error", integration=EmailIntegration(to="me@example.com")),
+        Action("cancelled", integration=WebhookIntegration(id="webhook:demo")),
     ]
 )
 
 # update the task status to 'processing' and set the value to 0
 task.started()
 try:
    for i in range(100):
```

