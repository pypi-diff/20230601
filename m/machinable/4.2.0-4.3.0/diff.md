# Comparing `tmp/machinable-4.2.0.tar.gz` & `tmp/machinable-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machinable-4.2.0.tar", max compression
+gzip compressed data, was "machinable-4.3.0.tar", max compression
```

## Comparing `machinable-4.2.0.tar` & `machinable-4.3.0.tar`

### file list

```diff
@@ -1,28 +1,25 @@
--rw-r--r--   0        0        0      645 2023-03-09 17:40:36.844631 machinable-4.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2023-03-09 17:40:36.844631 machinable-4.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1135 2023-03-09 17:40:36.844631 machinable-4.2.0/README.md
--rw-r--r--   0        0        0     2129 2023-03-09 17:40:36.848631 machinable-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1308 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/__init__.py
--rw-r--r--   0        0        0     3065 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/cli.py
--rw-r--r--   0        0        0    38442 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/collection.py
--rw-r--r--   0        0        0     2790 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/config.py
--rw-r--r--   0        0        0    26527 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/element.py
--rw-r--r--   0        0        0      512 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/errors.py
--rw-r--r--   0        0        0     7610 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/execution.py
--rw-r--r--   0        0        0    15986 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/experiment.py
--rw-r--r--   0        0        0     1567 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/group.py
--rw-r--r--   0        0        0     2345 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/mixin.py
--rw-r--r--   0        0        0    10522 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/project.py
--rw-r--r--   0        0        0       10 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/py.typed
--rw-r--r--   0        0        0     3380 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/record.py
--rw-r--r--   0        0        0      564 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/schedule.py
--rw-r--r--   0        0        0     1854 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/schema.py
--rw-r--r--   0        0        0     1029 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/settings.py
--rw-r--r--   0        0        0       47 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/storage/__init__.py
--rw-r--r--   0        0        0    21367 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/storage/filesystem.py
--rw-r--r--   0        0        0     7424 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/storage/multiple.py
--rw-r--r--   0        0        0    16603 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/storage/storage.py
--rw-r--r--   0        0        0     5193 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/testing.py
--rw-r--r--   0        0        0      359 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/types.py
--rw-r--r--   0        0        0    18698 2023-03-09 17:40:36.848631 machinable-4.2.0/src/machinable/utils.py
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 machinable-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0      795 2023-06-01 07:18:36.030406 machinable-4.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2023-06-01 07:18:36.030406 machinable-4.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1135 2023-06-01 07:18:36.030406 machinable-4.3.0/README.md
+-rw-r--r--   0        0        0     2159 2023-06-01 07:18:36.034407 machinable-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1385 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/__init__.py
+-rw-r--r--   0        0        0     3137 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/cli.py
+-rw-r--r--   0        0        0    37644 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/collection.py
+-rw-r--r--   0        0        0    11403 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/component.py
+-rw-r--r--   0        0        0     2933 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/config.py
+-rw-r--r--   0        0        0    22346 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/element.py
+-rw-r--r--   0        0        0      615 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/errors.py
+-rw-r--r--   0        0        0     6525 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/execution.py
+-rw-r--r--   0        0        0     1596 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/group.py
+-rw-r--r--   0        0        0     7549 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/index.py
+-rw-r--r--   0        0        0    13534 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/interface.py
+-rw-r--r--   0        0        0     2480 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/mixin.py
+-rw-r--r--   0        0        0    10855 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/project.py
+-rw-r--r--   0        0        0       10 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/py.typed
+-rw-r--r--   0        0        0      630 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/schedule.py
+-rw-r--r--   0        0        0     1433 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/schema.py
+-rw-r--r--   0        0        0     1002 2023-06-01 07:18:36.038407 machinable-4.3.0/src/machinable/settings.py
+-rw-r--r--   0        0        0     1041 2023-06-01 07:18:36.038407 machinable-4.3.0/src/machinable/storage.py
+-rw-r--r--   0        0        0      359 2023-06-01 07:18:36.038407 machinable-4.3.0/src/machinable/types.py
+-rw-r--r--   0        0        0    16473 2023-06-01 07:18:36.038407 machinable-4.3.0/src/machinable/utils.py
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 machinable-4.3.0/PKG-INFO
```

### Comparing `machinable-4.2.0/CHANGELOG.md` & `machinable-4.3.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # Changelog
 
 <!-- Please add changes under the Unreleased section that reads 'No current changes' otherwise -->
 
 # Unreleased
 
-- No current changes
+No current changes
+
+# v4.3.0
+
+- Generalized storage (#437)
+- Support for in-session element instances
+- Allow unstructured untyped dict-config
+- Simplified event structure
 
 # v4.2.0
 
 - Convert multiple storage into regular element (#426)
 
 # v4.1
 
 - Revamped CLI using element version syntax  (#422)
 - Allow arbitrary plain file extensions when saving/loading files
-- Filesystem storage stores groups as JSON files instead within the directory name
+- Filesystem storage captures groups within JSON files rather than directory name
 - Represent independent schedule via `None`
 - Adds Execution.on_verify_schedule to verify execution schedule compatibility
 
 # v4.0
 
 - Complete rewrite using elementary approach. Check out the documentation to learn more.
```

### Comparing `machinable-4.2.0/LICENSE.txt` & `machinable-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `machinable-4.2.0/README.md` & `machinable-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `machinable-4.2.0/pyproject.toml` & `machinable-4.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "machinable"
-version = "4.2.0"
+version = "4.3.0"
 description = "A modular configuration system for research projects"
 license = "MIT"
 authors = [
     "Frithjof Gressmann <hello@machinable.org>"
 ]
 maintainers = [
     "Frithjof Gressmann <hello@machinable.org>"
@@ -20,33 +20,33 @@
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Science/Research"
 ]
 include = ["CHANGELOG.md", "src/machinable/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-python-baseconv = "^1.2"
-observable = "^1.0"
 flatten-dict = "^0.4"
 jsonlines = "^3.1"
-pydantic = "^1.10.4"
+pydantic = "^1.10.8"
 arrow = "^1.2"
-importlib-metadata = {version = "^6.0", python = "<3.8"}
+importlib-metadata = {version = "^6.6", python = "<3.8"}
 commandlib = "^0.3.5"
 omegaconf = "^2.3.0"
+dill = "^0.3.6"
+typing-extensions = {version = "^4.5.0", python = "<3.11"}
 
 
 [tool.poetry.dev-dependencies]
 isort = "^5.11.5"
-pyupgrade = "^3.2"
-black = "^23.1.0"
-pytest = "^7.2"
+pyupgrade = "^3.3"
+black = "^23.3.0"
+pytest = "^7.3"
 pre-commit = "^2.21.0"
 editorconfig-checker = "^2.7.1"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.extras]
 all = [
   "numpy",
   "pandas",
 ]
```

### Comparing `machinable-4.2.0/src/machinable/__init__.py` & `machinable-4.3.0/src/machinable/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """machinable"""
 __all__ = [
     "Element",
+    "Interface",
     "Execution",
-    "Experiment",
+    "Component",
     "Project",
-    "Record",
     "Storage",
     "Mixin",
+    "Index",
     "mixin",
     "Schedule",
     "get",
     "get_settings",
 ]
 __doc__ = """A modular system for machinable research code"""
 
@@ -18,33 +19,34 @@
 
 if sys.version_info >= (3, 8):
     from importlib import metadata as importlib_metadata
 else:
     import importlib_metadata
 
 from machinable.cli import from_cli
+from machinable.component import Component
 from machinable.element import Element
 from machinable.execution import Execution
-from machinable.experiment import Experiment
+from machinable.index import Index
+from machinable.interface import Interface
 from machinable.mixin import Mixin, mixin
 from machinable.project import Project
-from machinable.record import Record
 from machinable.schedule import Schedule
 from machinable.settings import get_settings
 from machinable.storage import Storage
-from machinable.types import Optional, VersionType
+from machinable.types import Optional, Union, VersionType
 
 
 def get(
-    module: Optional[str] = None,
+    module: Union[str, Element, None] = None,
     version: VersionType = None,
     predicate: Optional[str] = get_settings().default_predicate,
     **kwargs,
-) -> Element:
-    return Element.get(module, version, predicate, **kwargs)
+) -> Interface:
+    return Interface.get(module, version, predicate, **kwargs)
 
 
 def get_version() -> str:
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
         return "unknown"
```

### Comparing `machinable-4.2.0/src/machinable/cli.py` & `machinable-4.3.0/src/machinable/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,32 +82,34 @@
             print(version)
             return 0
 
         if method == "help" or method is None:
             print("\nmachinable [element_module...] [version...] --method")
             print("\nExample:")
             print(
-                "\tmachinable my_experiment ~ver arg=1 nested.arg=2 --launch\n"
+                "\tmachinable my_component ~ver arg=1 nested.arg=2 --launch\n"
             )
             return 0
 
         print("Invalid argument: ", method)
         return 128
 
-    experiment = None
+    contexts = []
+    component = None
     for module, *version in elements:
         element = machinable.get(module, version)
-        element.__enter__()
-        if isinstance(element, machinable.Experiment):
-            experiment = element
+        contexts.append(element.__enter__())
+        if isinstance(element, machinable.Component):
+            component = element
 
-    if experiment is None:
-        raise ValueError("You have to provide an experiment")
+    if component is None:
+        raise ValueError("You have to provide an component")
 
     for method in methods:
         # check if cli_{method} exists before falling back on {method}
-        target = getattr(
-            experiment, f"cli_{method}", getattr(experiment, method)
-        )
+        target = getattr(component, f"cli_{method}", getattr(component, method))
         target()
 
+    for context in reversed(contexts):
+        context.__exit__()
+
     return 0
```

### Comparing `machinable-4.2.0/src/machinable/collection.py` & `machinable-4.3.0/src/machinable/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 long = int
 unicode = str
 basestring = str
 
 
 if TYPE_CHECKING:
-    from machinable.experiment import Experiment
+    from machinable.component import Component
 
 
 def _get_value(val):
     if callable(val):
         return val()
 
     return val
@@ -1405,82 +1405,58 @@
 
     def singleton(
         self,
         module: str,
         version: VersionType = None,
         predicate: str = get_settings().default_predicate,
         **kwargs,
-    ) -> Union[Any, "Experiment"]:
+    ) -> Union[Any, "Component"]:
         from machinable import Element
 
         instance = Element.make(module, version, **kwargs)
 
         for candidate in self:
             if candidate.matches(instance, predicate):
                 return candidate
 
         return instance
 
     def __str__(self):
         return f"Elements <{len(self.items)}>"
 
 
-class ExperimentCollection(ElementCollection):
+class InterfaceCollection(ElementCollection):
+    pass
+
+
+class ComponentCollection(InterfaceCollection):
     def __str__(self):
         if len(self.items) > 15:
             items = ", ".join([repr(item) for item in self.items[:5]])
             items += " ... "
             items += ", ".join([repr(item) for item in self.items[-5:]])
         else:
             items = ", ".join([repr(item) for item in self.items])
-        return f"Experiments ({len(self.items)}) <{items}>"
+        return f"Components ({len(self.items)}) <{items}>"
 
-    def launch(self) -> "ExperimentCollection":
-        """Executes all experiments in the collection"""
-        for experiment in self:
-            experiment.launch()
+    def launch(self) -> "ComponentCollection":
+        """Executes all components in the collection"""
+        for component in self:
+            component.launch()
 
         return self
 
-    def finished(self) -> "ExperimentCollection":
-        return self.filter(lambda x: x.is_finished())
-
-    def started(self) -> "ExperimentCollection":
-        return self.filter(lambda x: x.is_started())
-
-    def active(self) -> "ExperimentCollection":
-        return self.filter(lambda x: x.is_active())
-
-    def incomplete(self) -> "ExperimentCollection":
-        return self.filter(lambda x: x.is_incomplete())
-
-
-class ExecutionCollection(ElementCollection):
     def status(self, status="started"):
         """Filters the collection by a status attribute
 
         # Arguments
         status: String, status field: 'started', 'finished', 'alive'
         """
         try:
             return self.filter(lambda item: getattr(item, "is_" + status)())
         except AttributeError as _ex:
             raise ValueError(f"Invalid status field: {status}") from _ex
 
-    def __str__(self):
-        return f"Executions <{len(self.items)}>"
-
-
-class RecordCollection(ElementCollection):
-    def as_dataframe(self):
-        """Returns collection as Pandas dataframe"""
-        import pandas
-
-        data = (
-            {k: [row[k] for row in self._items] for k in self._items[0].keys()}
-            if len(self._items) > 0
-            else {}
-        )
-        return pandas.DataFrame.from_dict(data)
 
+class ExecutionCollection(ElementCollection):
     def __str__(self):
-        return f"Records <{len(self.items)}>"
+        return f"Executions <{len(self.items)}>"
```

### Comparing `machinable-4.2.0/src/machinable/config.py` & `machinable-4.3.0/src/machinable/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,29 +41,34 @@
         each_item=each_item,
         always=always,
         check_fields=check_fields,
         allow_reuse=True,
     )
 
 
-def from_element(element: "Element") -> Optional[Model]:
+def from_element(element: "Element") -> Tuple[dict, Optional[Model]]:
     if not isclass(element):
         element = element.__class__
 
     if not hasattr(element, "Config"):
-        return None
+        return {}, None
+
+    config = getattr(element, "Config")
 
-    schema = getattr(element, "Config")
+    # free-form
+    if isinstance(config, collections.abc.Mapping):
+        return config, None
 
+    # schema
     class SchemaConf:
         extra = "forbid"
 
-    model = dataclass(config=SchemaConf)(schema).__pydantic_model__
+    model = dataclass(config=SchemaConf)(config).__pydantic_model__
 
-    return model
+    return model().dict(), model
 
 
 def match_method(definition: str) -> Optional[Tuple[str, str]]:
     fn_match = re.match(r"(?P<method>\w+)\s?\((?P<args>.*)\)", definition)
     if fn_match is None:
         return None
```

### Comparing `machinable-4.2.0/src/machinable/element.py` & `machinable-4.3.0/src/machinable/element.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,36 @@
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import collections
 import copy
 import json
 import os
-import shlex
 import stat
-from functools import wraps
+import sys
+
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
 
 import arrow
+import dill as pickle
 import machinable
 import omegaconf
 import pydantic
-from flatten_dict import flatten
 from machinable import schema
-from machinable.collection import Collection
+from machinable.collection import ElementCollection
 from machinable.config import from_element, match_method, rewrite_config_methods
 from machinable.errors import ConfigurationError, MachinableError
 from machinable.mixin import Mixin
 from machinable.settings import get_settings
-from machinable.types import ElementType, VersionType
-from machinable.utils import Jsonable, unflatten_dict, update_dict
+from machinable.types import DatetimeType, ElementType, VersionType
+from machinable.utils import Jsonable, sentinel, unflatten_dict, update_dict
 from omegaconf import DictConfig, OmegaConf
 
-if TYPE_CHECKING:
-    from machinable.storage import Storage
-
-
-def belongs_to(f: Callable) -> Any:
-    @property
-    @wraps(f)
-    def _wrapper(self: "Element"):
-        name = f.__name__
-        if self.__related__.get(name, None) is None and self.is_mounted():
-            related_class = f()
-            use_cache = True
-            if isinstance(related_class, tuple):
-                related_class, use_cache = related_class
-            related = self.__model__._storage_instance.retrieve_related(
-                self.__model__._storage_id,
-                f"{self.kind.lower()}.{name}",
-            )
-            if related is None:
-                return None
-            element = related_class.from_model(related)
-            if not use_cache:
-                return element
-            self.__related__[name] = element
-
-        return self.__related__.get(name, None)
-
-    return _wrapper
-
-
-has_one = belongs_to
-
-
-def has_many(f: Callable) -> Any:
-    @property
-    @wraps(f)
-    def _wrapper(self: "Element") -> Any:
-        name = f.__name__
-        if self.__related__.get(name, None) is None and self.is_mounted():
-            args = f()
-            use_cache = True
-            if len(args) == 2:
-                related_class, collection = args
-            elif len(args) == 3:
-                related_class, collection, use_cache = args
-            else:
-                assert False, "Invalid number of relation arguments"
-            related = self.__model__._storage_instance.retrieve_related(
-                self.__model__._storage_id,
-                f"{self.kind.lower()}.{name}",
-            )
-            if related is None:
-                return None
-            collected = collection(
-                [related_class.from_model(r) for r in related]
-            )
-            if not use_cache:
-                return collected
-            self.__related__[name] = collected
-
-        return self.__related__.get(name, None)
-
-    return _wrapper
-
 
 class ConfigMethod:
     def __init__(self, element: "Element", prefix="config") -> None:
         self.element = element
         self.prefix = prefix
 
     def __call__(self, function, args) -> Any:
@@ -184,14 +115,20 @@
 
 def defaultversion(
     module: Optional[str], version: VersionType, element: "Element"
 ) -> Tuple[Optional[str], VersionType]:
     if module is not None:
         return module, normversion(version)
 
+    # handle in-session defaults
+    if isinstance(element.default, (list, tuple)) and not isinstance(
+        element.default[0], str
+    ):
+        return element.default[0], element.default[1:] + normversion(version)
+
     default_version = normversion(element.default)
 
     if len(default_version) == 0:
         return module, normversion(version)
 
     if isinstance(default_version[0], str) and not default_version[
         0
@@ -211,17 +148,20 @@
 ) -> Tuple[Optional[str], Optional[List[Union[str, dict]]]]:
     if compact_element is None:
         return None, None
 
     if isinstance(compact_element, str):
         return compact_element, None
 
+    if isinstance(compact_element, omegaconf.listconfig.ListConfig):
+        compact_element = list(compact_element)
+
     if not isinstance(compact_element, (list, tuple)):
         raise ValueError(
-            f"Invalid component defintion. Expected list or str but found {compact_element}"
+            f"Invalid component defintion. Expected list or str but found {type(compact_element)}: {compact_element}"
         )
 
     if len(compact_element) == 0:
         raise ValueError(
             f"Invalid component defintion. Expected str or non-empty list."
         )
 
@@ -263,22 +203,34 @@
 
 def transfer_to(src: "Element", destination: "Element") -> "Element":
     destination.__model__ = src.__model__
 
     return destination
 
 
+def uuid_to_id(uuid: str) -> str:
+    alphabet = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
+
+    # convert uuid hex to base 62 of length 6
+    result = ""
+    for i in range(0, 6 * 2, 2):
+        result += alphabet[int(uuid[i : i + 2], 16) % 62]
+
+    return result
+
+
 def resolve_custom_predicate(predicate: str, element: "Element"):
     from machinable.project import Project
 
     custom = element.on_compute_predicate() or {}
     if isinstance(element, Project):
         custom.update(element.global_predicate() or {})
     else:
         custom.update(Project.get().provider().global_predicate() or {})
+    custom.update(getattr(element, "_starred_predicates", {}))
 
     if custom:
         predicate = predicate.replace(
             "*",
             ",".join(
                 [k.replace("*", "") for k in custom.keys() if k.endswith("*")]
             ),
@@ -313,46 +265,90 @@
     _module_: Optional[str] = None
 
     def __init__(self, version: VersionType = None):
         super().__init__()
         if Element._module_ is None:
             Element._module_ = self.__module__
         self.__model__ = schema.Element(
+            kind=self.kind,
             module=Element._module_,
             version=normversion(version),
             lineage=get_lineage(self),
+            _dump=pickle.dumps(self.__class__)
+            if Element._module_.startswith("__session__")
+            else None,
         )
-        self.__related__ = {}
         self.__mixin__ = None
         self.__mixins__ = {}
         self._config: Optional[DictConfig] = None
         self._predicate: Optional[DictConfig] = None
         self._cache = {}
-        self._deferred_data = {}
 
         Element._module_ = None
 
+    @property
+    def uuid(self) -> str:
+        return self.__model__.uuid
+
+    @property
+    def id(self) -> str:
+        return self.uuid[:6]
+
+    @property
+    def timestamp(self) -> float:
+        return self.__model__.timestamp
+
+    def timestamp_at(self) -> DatetimeType:
+        return arrow.get(self.__model__.timestamp)
+
+    def version(
+        self, version: VersionType = sentinel, overwrite: bool = False
+    ) -> List[Union[str, dict]]:
+        if version is sentinel:
+            return self.__model__.version
+
+        if hasattr(self, "is_mounted") and self.is_mounted():
+            raise MachinableError(
+                f"Cannot change version of mounted element {self}"
+            )
+
+        if overwrite:
+            self.__model__.version = normversion(version)
+        else:
+            self.__model__.version.extend(normversion(version))
+
+        self._clear_caches()
+
+        return self.__model__.version
+
     @classmethod
     def set_default(
         cls,
-        module: Optional[str] = None,
+        module: Union[str, "Element", None] = None,
         version: VersionType = None,
     ) -> None:
+        if module is not None and not isinstance(module, str):
+            cls.default = [module] + normversion(version)
+            return
         cls.default = compact(module, version)
 
-    def as_default(self) -> "Element":
+    def as_default(self) -> Self:
         cls = getattr(machinable, self.kind, Element)
         cls.set_default(self.__model__.module, self.__model__.version)
 
         return self
 
     @classmethod
+    def connected(cls) -> List["Element"]:
+        return _CONNECTIONS[cls.kind]
+
+    @classmethod
     def get(
         cls,
-        module: Optional[str] = None,
+        module: Union[str, "Element", None] = None,
         version: VersionType = None,
         predicate: Optional[str] = get_settings().default_predicate,
         **kwargs,
     ) -> "Element":
         if module is None and version is None:
             if len(_CONNECTIONS[cls.kind]) > 0:
                 return _CONNECTIONS[cls.kind][-1]
@@ -388,128 +384,51 @@
             base_class=base_class,
             **kwargs,
         )
 
     @classmethod
     def instance(
         cls,
-        module: Optional[str] = None,
+        module: Union[None, str, "Element"] = None,
         version: VersionType = None,
         **kwargs,
     ) -> "Element":
         module, version = defaultversion(module, version, cls)
         return cls.make(module, version, base_class=cls, **kwargs)
 
-    def mount(self, storage: "Storage", storage_id: Any) -> bool:
-        if self.__model__ is None:
-            return False
-
-        self.__model__._storage_instance = storage
-        self.__model__._storage_id = storage_id
-
-        return True
-
-    def is_mounted(self) -> bool:
-        if self.__model__ is None:
-            return False
-
-        return (
-            self.__model__._storage_instance is not None
-            and self.__model__._storage_id is not None
-        )
+    @classmethod
+    def singleton(
+        cls,
+        module: Union[str, "Element"],
+        version: VersionType = None,
+        predicate: Optional[str] = get_settings().default_predicate,
+        **kwargs,
+    ) -> "Element":
+        # no-op as elements do not have a storage representation
+        return cls.make(module, version, **kwargs)
 
     @classmethod
     def from_model(cls, model: schema.Element) -> "Element":
         if cls.__module__ != model.module:
             # re-instantiate element class
-            instance = cls.make(model.module)
+            if model.module and model.module.startswith("__session__"):
+                if model._dump is None:
+                    raise RuntimeError(
+                        f"Unable to restore element {model.module}"
+                    )
+                instance = cls.make(pickle.loads(model._dump))
+            else:
+                instance = cls.make(model.module)
         else:
             instance = cls()
 
         instance.set_model(model)
 
         return instance
 
-    @classmethod
-    def find(cls, element_id: str, *args, **kwargs) -> Optional["Element"]:
-        from machinable.storage import Storage
-
-        storage = Storage.get()
-
-        storage_id = getattr(storage, f"find_{cls.kind.lower()}")(
-            element_id, *args, **kwargs
-        )
-
-        if storage_id is None:
-            return None
-
-        return cls.from_storage(storage_id, storage)
-
-    @classmethod
-    def find_many(cls, elements: List[str]) -> "Collection":
-        return cls.collect([cls.find(element_id) for element_id in elements])
-
-    @classmethod
-    def find_by_predicate(
-        cls,
-        module: str,
-        version: VersionType = None,
-        predicate: Optional[str] = get_settings().default_predicate,
-        **kwargs,
-    ) -> "Collection":
-        from machinable.storage import Storage
-
-        storage = Storage.get()
-        try:
-            candidate = cls.make(module, version, **kwargs)
-        except ModuleNotFoundError:
-            return cls.collect([])
-
-        element_type = candidate.kind.lower()
-        handler = f"find_{element_type}_by_predicate"
-
-        if hasattr(storage, handler):
-            if predicate:
-                predicate = OmegaConf.to_container(
-                    OmegaConf.create(
-                        {
-                            p: candidate.predicate[p]
-                            for p in resolve_custom_predicate(
-                                predicate, candidate
-                            )
-                        }
-                    )
-                )
-            storage_ids = getattr(storage, handler)(module, predicate)
-        else:
-            storage_ids = []
-
-        return cls.collect(
-            [
-                cls.from_model(
-                    getattr(storage, f"retrieve_{element_type}")(storage_id)
-                )
-                for storage_id in storage_ids
-            ]
-        )
-
-    @classmethod
-    def singleton(
-        cls,
-        module: str,
-        version: VersionType = None,
-        predicate: Optional[str] = get_settings().default_predicate,
-        **kwargs,
-    ) -> "Collection[Element]":
-        candidates = cls.find_by_predicate(module, version, predicate, **kwargs)
-        if candidates:
-            return candidates[-1]
-
-        return cls.make(module, version, **kwargs)
-
     def on_compute_predicate(self) -> Optional[Dict]:
         """Event to compute a custom predicate dictionary of the element
         where each key presents a predicate that can be used
         during element lookup. Keys marked with a * are automatically
         matched."""
 
     @property
@@ -544,19 +463,18 @@
                     # config method resolver
                     OmegaConf.register_new_resolver(
                         name="config_method",
                         resolver=ConfigMethod(self),
                         replace=True,
                     )
 
-                    # expose raw config so events and config methods can use it
-                    config_model = from_element(self) or pydantic.BaseModel
-                    raw_config = config_model().dict()
+                    # expose default config so events and config methods can use it
+                    default_config, config_model = from_element(self)
 
-                    self._config = OmegaConf.create(raw_config)
+                    self._config = OmegaConf.create(default_config)
 
                     self.on_before_configure(self._config)
 
                     # apply versioning
                     __version = copy.deepcopy(self.__model__.version)
 
                     # compose configuration update
@@ -597,18 +515,19 @@
                     # computed configuration transform
                     self.on_configure()
 
                     # resolve config
                     config = OmegaConf.to_container(self._config, resolve=True)
 
                     # enforce schema
-                    config = config_model(**config).dict()
+                    if config_model is not None:
+                        config = config_model(**config).dict()
 
                     # add introspection data
-                    config["_raw_"] = raw_config
+                    config["_default_"] = default_config
                     config["_version_"] = __version
                     config["_update_"] = config_update
 
                     # make config property accessible for slot components
                     self._config = OmegaConf.create(config)
 
                     # disallow further transformation
@@ -625,43 +544,17 @@
     def module(self) -> Optional[str]:
         return self.__model__.module
 
     @property
     def lineage(self) -> Tuple[str, ...]:
         return self.__model__.lineage
 
-    @property
-    def storage_id(self) -> Optional[str]:
-        if not self.is_mounted():
-            return None
-
-        return self.__model__._storage_id
-
-    @property
-    def storage_instance(self) -> Optional["Storage"]:
-        if not self.is_mounted():
-            return None
-
-        return self.__model__._storage_instance
-
-    @classmethod
-    def from_storage(cls, storage_id, storage=None) -> "Element":
-        if storage is None:
-            from machinable.storage import Storage
-
-            storage = Storage.get()
-
-        return cls.from_model(
-            getattr(storage, f"retrieve_{cls.kind.lower()}")(storage_id)
-        )
-
     @classmethod
-    def collect(cls, elements) -> Collection:
-        """Returns a collection of the element type"""
-        return Collection(elements)
+    def collect(cls, elements) -> ElementCollection:
+        return ElementCollection(elements)
 
     @classmethod
     def model(cls, element: Optional[Any] = None) -> schema.Element:
         if element is not None:
             if isinstance(element, cls):
                 return element.__model__
 
@@ -678,132 +571,47 @@
     def matches(self, element: "Element", predicate: str) -> bool:
         for p in resolve_custom_predicate(predicate, element):
             if not equalversion(self.predicate[p], element.predicate[p]):
                 return False
 
         return True
 
-    def set_model(self, model: schema.Element) -> "Element":
+    def set_model(self, model: schema.Element) -> Self:
         self.__model__ = model
 
         # invalidate cached config
         self._config = None
         self._predicate = None
 
         return self
 
-    def local_directory(
-        self, *append: str, create: bool = False
-    ) -> Optional[str]:
-        if not self.is_mounted():
-            return None
-
-        return self.__model__._storage_instance.local_directory(
-            self, *append, create=create
-        )
-
-    def load_file(self, filepath: str, default=None) -> Optional[Any]:
-        if not self.is_mounted():
-            # has write been deferred?
-            if filepath in self._deferred_data:
-                return self._deferred_data[filepath]
-
-            return default
-
-        data = self.__model__._storage_instance.retrieve_file(self, filepath)
-
-        return data if data is not None else default
-
-    def save_file(self, filepath: str, data: Any) -> str:
-        if os.path.isabs(filepath):
-            raise ValueError("Filepath must be relative")
-
-        if not self.is_mounted():
-            # defer writes until element storage creation
-            self._deferred_data[filepath] = data
-            return "$deferred"
-
-        file = self.__model__._storage_instance.create_file(
-            self, filepath, data
-        )
-
-        # mark scripts as executable
-        if filepath.endswith(".sh"):
-            st = os.stat(file)
-            os.chmod(file, st.st_mode | stat.S_IEXEC)
-
-        return file
-
-    def save_data(self, filepath: str, data: Any) -> str:
-        return self.save_file(os.path.join("data", filepath), data)
-
-    def load_data(self, filepath: str, default=None) -> Optional[Any]:
-        return self.load_file(os.path.join("data", filepath), default)
-
     def serialize(self) -> Dict:
         # ensure that configuration has been parsed
         assert self.config is not None
         return self.__model__.dict()
 
     @classmethod
     def unserialize(cls, serialized):
         return cls.from_model(cls.model()(**serialized))
 
     @classmethod
     def is_connected(cls) -> bool:
         return len(_CONNECTIONS[cls.kind]) > 0
 
-    def to_cli(self) -> str:
-        cli = [self.module]
-        for v in self.__model__.version:
-            if isinstance(v, str):
-                cli.append(v)
-            else:
-                cli.extend(
-                    [
-                        f"{key}={shlex.quote(str(val))}"
-                        for key, val in flatten(v, reducer="dot").items()
-                    ]
-                )
-
-        return " ".join(cli)
-
-    def __enter__(self):
-        _CONNECTIONS[self.kind].append(self)
-        return self
-
-    def __exit__(self, *args, **kwargs):
-        try:
-            _CONNECTIONS[self.kind].pop()
-        except IndexError:
-            pass
-
-    def __reduce__(self) -> Union[str, Tuple[Any, ...]]:
-        return (self.__class__, (), self.serialize())
-
-    def __getstate__(self):
-        return self.serialize()
-
-    def __setstate__(self, state):
-        self.__model__ = self.__class__.model()(**state)
-
-    def __str__(self):
-        return self.__repr__()
-
     def compute_predicate(self) -> Dict:
         from machinable.project import Project
 
         custom = self.on_compute_predicate() or {}
         if isinstance(self, Project):
             custom.update(self.global_predicate() or {})
         else:
             custom.update(Project.get().provider().global_predicate() or {})
 
         config = copy.deepcopy(OmegaConf.to_container(self.config))
-        raw = config.pop("_raw_")
+        default = config.pop("_default_")
         version = config.pop("_version_")
         update = config.pop("_update_")
 
         return {
             "config_update": _filter_enderscores(update),
             "config_update_": update,
             "config": _filter_enderscores(config),
@@ -826,23 +634,67 @@
     def on_configure(self) -> None:
         """Configuration event
         This may be used to apply computed configuration updates
         Do not use to validate the configuration but use validators in the config schema
         that are applied at a later stage.
         """
 
+    def _clear_caches(self) -> None:
+        self._config = None
+        self.__model__.config = None
+
     def __getattr__(self, name) -> Any:
         attr = getattr(self.__mixin__, name, None)
         if attr is not None:
             return attr
         raise AttributeError(
             "{!r} object has no attribute {!r}".format(
                 self.__class__.__name__, name
             )
         )
 
+    def __enter__(self) -> Self:
+        _CONNECTIONS[self.kind].append(self)
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        try:
+            _CONNECTIONS[self.kind].pop()
+        except IndexError:
+            pass
+
+    def __reduce__(self) -> Union[str, Tuple[Any, ...]]:
+        return (self.__class__, (), self.serialize())
+
+    def __getstate__(self):
+        return self.serialize()
+
+    def __setstate__(self, state):
+        self.__model__ = self.__class__.model()(**state)
+
+    def __repr__(self):
+        return f"{self.kind} [{self.id}]"
+
+    def __str__(self):
+        return self.__repr__()
+
+    def __eq__(self, other):
+        return self.uuid == other.uuid
+
+    def __ne__(self, other):
+        return self.uuid != other.uuid
+
 
 def get_lineage(element: "Element") -> Tuple[str, ...]:
     return tuple(
         obj.module if isinstance(obj, Element) else obj.__module__
         for obj in element.__class__.__mro__[1:-3]
     )
+
+
+def get_dump(element: "Element") -> Optional[bytes]:
+    if element.__model__.module.startswith("__session__"):
+        return pickle.dumps(element.__class__)
+
+
+def reset_connections() -> None:
+    _CONNECTIONS.clear()
```

### Comparing `machinable-4.2.0/src/machinable/errors.py` & `machinable-4.3.0/src/machinable/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,7 +20,13 @@
     Bases: MachinableError"""
 
 
 class ExecutionFailed(MachinableError):
     """Execution failed
 
     Bases: MachinableError"""
+
+
+class ComponentException(MachinableError):
+    """Component exception
+
+    Bases: MachinableError"""
```

### Comparing `machinable-4.2.0/src/machinable/execution.py` & `machinable-4.3.0/src/machinable/execution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,116 @@
 from typing import Any, Dict, List, Optional, Union
 
 import copy
+import sys
+
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
 
 from machinable import schema
-from machinable.collection import ExperimentCollection
-from machinable.element import (
-    Element,
-    defaultversion,
-    extract,
-    get_lineage,
-    has_many,
-    has_one,
-)
+from machinable.collection import ComponentCollection
+from machinable.component import Component
+from machinable.element import extract, get_dump, get_lineage
 from machinable.errors import ExecutionFailed
-from machinable.experiment import Experiment
+from machinable.interface import Interface, has_many, has_one
 from machinable.project import Project
 from machinable.schedule import Schedule
 from machinable.settings import get_settings
-from machinable.storage import Storage
 from machinable.types import ElementType, VersionType
 from machinable.utils import sentinel, update_dict
 
 
-class Execution(Element):
+class Execution(Interface):
     kind = "Execution"
     default = get_settings().default_execution
 
     def __init__(
         self,
         version: VersionType = None,
         resources: Optional[Dict] = None,
         schedule: Union[
             Schedule, ElementType, None
         ] = get_settings().default_schedule,
     ):
         super().__init__(version)
         self.__model__ = schema.Execution(
+            kind=self.kind,
             module=self.__model__.module,
             config=self.__model__.config,
             version=self.__model__.version,
             resources=resources,
-            host_info=Project.get().provider().get_host_info(),
             lineage=get_lineage(self),
         )
+        self.__model__._dump = get_dump(self)
         if schedule is not None:
             if not isinstance(schedule, Schedule):
                 schedule = Schedule.make(*extract(schedule))
-            self.__related__["schedule"] = schedule
+            self.push_related("schedule", schedule)
+        self._starred_predicates = {"resources": None}
+
+    def compute_predicate(self) -> Dict:
+        predicates = super().compute_predicate()
+        predicates["resources"] = self.__model__.resources
+        return predicates
 
     @has_one
     def schedule() -> "Schedule":
         return Schedule
 
-    @has_many
-    def experiments() -> ExperimentCollection:
-        return Experiment, ExperimentCollection
+    @has_many(key="execution_history")
+    def executables() -> ComponentCollection:
+        return Component
 
     @property
-    def executables(self) -> "Collection":
-        return self.experiments
+    def pending_executables(self) -> ComponentCollection:
+        return self.executables.filter(lambda e: not e.cached())
 
     def add(
         self,
-        executable: Union[Experiment, List[Experiment]],
+        executable: Union[Component, List[Component]],
         once: bool = False,
-    ) -> "Execution":
+    ) -> Self:
         if isinstance(executable, (list, tuple)):
             for _executable in executable:
                 self.add(_executable)
             return self
 
-        if not isinstance(executable, Experiment):
-            raise ValueError(
-                f"Expected experiment, but found: {type(executable)} {executable}"
-            )
-
-        self.__related__.setdefault("experiments", ExperimentCollection())
-
-        if once and self.__related__["experiments"].contains(
+        if once and self.__related__["executables"].contains(
             lambda x: x == executable
         ):
             # already added
             return self
 
-        self.__related__["experiments"].append(executable)
+        self.push_related("executables", executable)
 
         return self
 
-    def commit(self) -> "Execution":
-        self.on_before_commit()
-
-        # trigger configuration validation for early failure
-        self.executables.each(lambda x: x.config)
+    def commit(self) -> Self:
+        # ensure that configuration is parsed
+        self.executables.map(lambda x: x.config and x.predicate)
 
-        Storage.get().commit(self.executables, self)
-
-        return self
+        return super().commit()
 
     def resources(self, resources: Dict = sentinel) -> Optional[Dict]:
         if resources is sentinel:
             return self.__model__.resources
 
         self.__model__.resources = resources
 
         return self.__model__.resources
 
     def canonicalize_resources(self, resources: Dict) -> Dict:
         return resources
 
-    def default_resources(self, executable: "Experiment") -> Optional[dict]:
+    def default_resources(self, executable: "Component") -> Optional[dict]:
         """Default resources"""
 
-    def compute_resources(self, executable: "Experiment") -> Dict:
+    def compute_resources(self, executable: "Component") -> Dict:
         default_resources = self.default_resources(executable)
 
         if not self.__model__.resources and default_resources is not None:
             return self.canonicalize_resources(default_resources)
 
         if self.__model__.resources and not default_resources:
             resources = copy.deepcopy(self.__model__.resources)
@@ -144,114 +139,71 @@
                 defaults_.pop(removal[1:], None)
                 update_.pop(removal, None)
 
             return update_dict(defaults_, update_)
 
         return {}
 
-    def __call__(self) -> None:
+    def dispatch(self) -> Self:
         if not self.executables:
-            return
-
-        if all(self.executables.map(lambda x: x.is_finished())):
-            return
-
-        self.dispatch()
+            return self
 
-    def dispatch(self) -> "Execution":
-        if not self.executables:
+        if len(self.pending_executables) == 0:
             return self
 
         if self.on_before_dispatch() is False:
             return self
 
         if self.on_verify_schedule() is False:
             raise ExecutionFailed(
                 "The execution does not support the specified schedule."
             )
 
         self.commit()
 
         try:
             # compute resources
-            for executable in self.executables.filter(
-                lambda e: not e.is_finished()
-            ):
-                self.save_file(
-                    f"resources-{executable.experiment_id}.json",
+            for executable in self.pending_executables:
+                executable.save_file(
+                    f"resources-{self.id}.json",
                     self.compute_resources(executable),
                 )
-            self.on_dispatch()
+            self.__call__()
             self.on_after_dispatch()
         except BaseException as _ex:  # pylint: disable=broad-except
             raise ExecutionFailed("Execution failed") from _ex
 
         return self
 
+    def __call__(self) -> None:
+        for executable in self.pending_executables:
+            executable.dispatch()
+
     def on_verify_schedule(self) -> bool:
+        """Event to verify compatibility of the schedule"""
         if self.schedule is None:
             return True
 
         return False
 
     def on_before_dispatch(self) -> Optional[bool]:
         """Event triggered before dispatch of an execution
 
         Return False to prevent the dispatch
         """
-        # forward into on_before_dispatch
-        for executable in self.executables:
-            executable.on_before_dispatch()
 
     def on_before_commit(self) -> Optional[bool]:
         """Event triggered before commit of an execution"""
-        # forward into on_before_commit
-        for executable in self.executables:
-            executable.on_before_commit()
 
     def on_after_dispatch(self) -> None:
         """Event triggered after the dispatch of an execution"""
 
-    def on_dispatch(self):
-        for executable in self.executables:
-            executable()
-
-    @property
-    def timestamp(self) -> float:
-        return self.__model__.timestamp
-
-    @property
-    def host_info(self) -> Optional[Dict]:
-        return self.__model__.host_info
-
-    @property
-    def env_info(self) -> Optional[Dict]:
-        return self.load_file("env.json", None)
-
-    @property
-    def nickname(self) -> str:
-        return self.__model__.nickname
-
     def __iter__(self):
         yield from self.executables
 
     def __exit__(self, *args, **kwargs):
-        self()
+        self.dispatch()
 
         super().__exit__()
 
-    def __str__(self) -> str:
-        return self.__repr__()
-
     def __repr__(self) -> str:
         return "Execution"
-
-    def __eq__(self, other):
-        return (
-            self.nickname == other.nickname
-            and self.timestamp == other.timestamp
-        )
-
-    def __ne__(self, other):
-        return (
-            self.nickname != other.nickname or self.timestamp != other.timestamp
-        )
```

### Comparing `machinable-4.2.0/src/machinable/experiment.py` & `machinable-4.3.0/src/machinable/component.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,338 +1,294 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, List, Optional, Union
 
-import os
 import random
-import stat
 import sys
+import threading
 
 import arrow
+from machinable.settings import get_settings
+
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+from typing import Dict
+
 from machinable import errors, schema
-from machinable.collection import (
-    ElementCollection,
-    ExecutionCollection,
-    ExperimentCollection,
-    RecordCollection,
-)
-from machinable.element import (
-    Element,
-    belongs_to,
-    defaultversion,
-    get_lineage,
-    has_many,
-    normversion,
-)
-from machinable.errors import ConfigurationError
-from machinable.group import Group
+from machinable.collection import ComponentCollection, ExecutionCollection
+from machinable.element import _CONNECTIONS as connected_elements
+from machinable.element import Element, get_dump, get_lineage
+from machinable.interface import Interface, belongs_to, belongs_to_many
 from machinable.project import Project
-from machinable.settings import get_settings
-from machinable.storage.storage import Storage
+from machinable.storage import Storage
 from machinable.types import DatetimeType, TimestampType, VersionType
-from machinable.utils import (
-    Events,
-    generate_seed,
-    sentinel,
-    timestamp_to_directory,
-)
+from machinable.utils import generate_seed, load_file, save_file
 
 if TYPE_CHECKING:
     from machinable.execution import Execution
-    from machinable.record import Record
 
 
-class Experiment(Element):  # pylint: disable=too-many-public-methods
-    kind = "Experiment"
-    default = get_settings().default_experiment
+class Component(Interface):
+    kind = "Component"
+    default = get_settings().default_component
 
     def __init__(
         self,
         version: VersionType = None,
+        uses: Union[None, "Interface", List["Interface"]] = None,
+        derived_from: Optional["Interface"] = None,
         seed: Union[int, None] = None,
-        derived_from: Optional["Experiment"] = None,
-        uses: Union[None, Element, List[Element]] = None,
     ):
-        super().__init__(version=version)
+        super().__init__(version=version, uses=uses, derived_from=derived_from)
         if seed is None:
             seed = generate_seed()
-        self.__model__ = schema.Experiment(
+        self.__model__ = schema.Component(
+            kind=self.kind,
             module=self.__model__.module,
             config=self.__model__.config,
             version=self.__model__.version,
             seed=seed,
             lineage=get_lineage(self),
         )
-        if derived_from is not None:
-            self.__model__.derived_from_id = derived_from.experiment_id
-            self.__model__.derived_from_timestamp = derived_from.timestamp
-            self.__related__["ancestor"] = derived_from
-        self._events: Events = Events()
-        self.__related__["uses"] = ElementCollection()
-        if uses:
-            self.use(uses)
-
-    @belongs_to
-    def group():
-        return Group
-
-    @belongs_to
-    def project():
-        from machinable.project import Project
-
-        return Project
-
-    @has_many
-    def derived() -> ExperimentCollection:
-        """Returns a collection of derived experiments"""
-        return Experiment, ExperimentCollection, False
-
-    @belongs_to
-    def ancestor() -> Optional["Experiment"]:
-        """Returns parent experiment or None if experiment is independent"""
-        return Experiment
+        self.__model__._dump = get_dump(self)
 
-    @has_many
-    def executions() -> "ExecutionCollection":
+    @belongs_to_many(key="execution_history")
+    def executions() -> ExecutionCollection:
         from machinable.execution import Execution
 
-        return Execution, ExecutionCollection
+        return Execution
 
-    @belongs_to
+    @belongs_to(key="execution_history", cached=False)
     def execution() -> "Execution":
         from machinable.execution import Execution
 
-        return Execution, False
+        return Execution
+
+    @property
+    def seed(self) -> int:
+        return self.__model__.seed
+
+    @property
+    def nickname(self) -> str:
+        return self.__model__.nickname
 
-    def launch(self) -> "Experiment":
+    def launch(self) -> Self:
         from machinable.execution import Execution
 
         execution = Execution.get()
 
         execution.add(self)
 
         if Execution.is_connected():
             # commit only, defer execution
             self.commit()
         else:
-            execution()
+            execution.dispatch()
 
         return self
 
-    @has_many
-    def uses() -> "ElementCollection":
-        return Element, ElementCollection
-
-    @classmethod
-    def collect(cls, experiments) -> ExperimentCollection:
-        """Returns a collection of experiments"""
-        return ExperimentCollection(experiments)
-
     @classmethod
-    def from_model(cls, model: schema.Experiment) -> "Experiment":
-        return super().from_model(model)
-
-    def __reduce__(self) -> Union[str, Tuple[Any, ...]]:
-        return (self.__class__, ("",), self.serialize())
-
-    def _assert_editable(self):
-        if self.is_mounted():
-            raise ConfigurationError(
-                "Experiment can not be modified as it has already been executed. "
-                "Use .derive() or Experiment(derived_from) to derive a modified experiment."
-            )
-
-    def _clear_caches(self) -> None:
-        self._config = None
-        self.__model__.config = None
-
-    def use(self, use: Union[Element, List[Element]]) -> "Experiment":
-        self._assert_editable()
-
-        if isinstance(use, (list, tuple)):
-            for _use in use:
-                self.use(_use)
-            return self
-
-        if not isinstance(use, Element):
-            raise ValueError(f"Expected element, but found: {type(use)} {use}")
-
-        self.__related__["uses"].append(use)
-
-        return self
-
-    def group_as(self, group: Union[Group, str]) -> "Experiment":
-        # todo: allow group modifications after execution
-        self._assert_editable()
-
-        if isinstance(group, str):
-            group = Group(group)
-        if not isinstance(group, Group):
-            raise ValueError(
-                f"Expected group, but found: {type(group)} {group}"
-            )
-        group.__related__.setdefault("experiments", ExperimentCollection())
-        group.__related__["experiments"].append(self)
-        self.__related__["group"] = group
-
-        return self
+    def collect(cls, components) -> "ComponentCollection":
+        return ComponentCollection(components)
 
-    def derive(
-        self,
-        module: Optional[str] = None,
-        version: VersionType = None,
-        predicate: Optional[str] = get_settings().default_predicate,
-        **kwargs,
-    ) -> "Experiment":
-        if module is None or predicate is None:
-            return self.make(module, version, derived_from=self, **kwargs)
+    def resources(self) -> Optional[Dict]:
+        if self.execution is None:
+            return None
+        return self.load_file(f"resources-{self.execution.id}.json", None)
 
-        return self.derived.singleton(
-            module, version, predicate, derived_from=self, **kwargs
+    def dispatch(self) -> Self:
+        """Dispatch the component lifecycle"""
+        writes_meta_data = (
+            self.on_write_meta_data() is not False and self.is_mounted()
         )
+        try:
+            self.on_before_dispatch()
 
-    def version(
-        self, version: VersionType = sentinel, overwrite: bool = False
-    ) -> List[Union[str, dict]]:
-        if version is sentinel:
-            return self.__model__.version
+            self.on_seeding()
 
-        self._assert_editable()
+            # meta-data
+            if writes_meta_data:
+                self.update_status("started")
+                self.save_file(
+                    "host.json",
+                    data=Project.get().provider().get_host_info(),
+                )
+
+            def beat():
+                t = threading.Timer(15, beat)
+                t.daemon = True
+                t.start()
+                self.on_heartbeat()
+                if self.on_write_meta_data() is not False and self.is_mounted():
+                    self.update_status("heartbeat")
+                return t
 
-        if overwrite:
-            self.__model__.version = normversion(version)
-        else:
-            self.__model__.version.extend(normversion(version))
+            heartbeat = beat()
 
-        self._clear_caches()
+            self.__call__()
 
-        return self.__model__.version
-
-    def commit(self) -> "Experiment":
-        self.on_before_commit()
+            self.on_success()
+            self.on_finish(success=True)
 
-        Storage.get().commit(self)
+            if heartbeat is not None:
+                heartbeat.cancel()
 
-        return self
+            if writes_meta_data:
+                self.update_status("finished")
 
-    @property
-    def experiment_id(self) -> str:
-        return self.__model__.experiment_id
+            self.on_after_dispatch(success=True)
+        except BaseException as _ex:  # pylint: disable=broad-except
+            self.on_failure(exception=_ex)
+            self.on_finish(success=False)
+            self.on_after_dispatch(success=False)
+            raise errors.ComponentException(
+                f"{self.__class__.__name__} dispatch failed"
+            ) from _ex
+        finally:
+            if writes_meta_data:
+                # propagate changes
+                for storage in Storage.connected():
+                    storage.update(self)
 
     @property
-    def resources(self) -> Optional[Dict]:
-        if self.execution is None:
-            return None
-        return self.execution.load_file(
-            f"resources-{self.experiment_id}.json", None
-        )
-
-    def records(self, scope="default") -> RecordCollection:
-        if not self.is_mounted():
-            return RecordCollection()
+    def host_info(self) -> Optional[Dict]:
+        return self.load_file("host.json", None)
 
-        if f"records.{scope}" in self._cache:
-            return self._cache[f"records.{scope}"]
+    def cached(self) -> bool:
+        return self.is_finished()
 
-        records = RecordCollection(
-            self.__model__._storage_instance.retrieve_records(self, scope)
-        )
-
-        if self.is_finished():
-            self._cache[f"records.{scope}"] = records
-
-        return records
-
-    def record(self, scope="default") -> "Record":
-        from machinable.record import Record
-
-        if f"record.{scope}" not in self._cache:
-            self._cache[f"record.{scope}"] = Record(self, scope)
-
-        return self._cache[f"record.{scope}"]
+    def dispatch_code(self, inline: bool = True) -> Optional[str]:
+        connections = [f"Project('{Project.get().path()}').__enter__()"]
+        for kind, elements in connected_elements.items():
+            if kind in ["Project", "Execution"]:
+                continue
+            for element in elements:
+                jn = element.as_json().replace('"', '\\"').replace("'", "\\'")
+                connections.append(f"Element.from_json('{jn}').__enter__()")
+        context = "\n".join(connections)
+        code = f"""
+        from machinable import Project, Element, Component
+        {context}
+        component__ = Component.find('{self.uuid}')
+        component__.dispatch()
+        """
 
-    def mark_started(
-        self, timestamp: Optional[TimestampType] = None
-    ) -> Optional[DatetimeType]:
-        if self.is_finished():
-            return None
-        return self.__model__._storage_instance.mark_started(self, timestamp)
+        if inline:
+            code = code.replace("\n        ", ";")[1:-1]
+            return f'{sys.executable} -c "{code}"'
 
-    def update_heartbeat(
-        self,
-        timestamp: Union[float, int, DatetimeType, None] = None,
-        mark_finished=False,
-    ) -> Optional[DatetimeType]:
-        if self.is_finished():
-            return None
-        self.__model__._storage_instance.update_heartbeat(
-            self, timestamp, mark_finished
-        )
+        return code.replace("        ", "")[1:-1]
 
     def output(self, incremental: bool = False) -> Optional[str]:
         """Returns the output log"""
         if not self.is_mounted():
             return None
         if incremental:
             read_length = self._cache.get("output_read_length", 0)
             if read_length == -1:
                 return ""
-            output = self.__model__._storage_instance.retrieve_output(self)
+            output = self.load_file("output.log", None)
             if output is None:
                 return None
 
             if self.is_finished():
                 self._cache["output_read_length"] = -1
             else:
                 self._cache["output_read_length"] = len(output)
             return output[read_length:]
 
         if "output" in self._cache:
             return self._cache["output"]
 
-        output = self.__model__._storage_instance.retrieve_output(self)
+        output = self.load_file("output.log", None)
 
         if self.is_finished():
             self._cache["output"] = output
 
         return output
 
-    @property
-    def seed(self) -> int:
-        return self.__model__.seed
-
-    @property
-    def timestamp(self) -> int:
-        return self.__model__.timestamp
+    def update_status(
+        self,
+        status: Literal["started", "heartbeat", "finished"] = "heartbeat",
+        timestamp: Optional[TimestampType] = None,
+    ) -> None:
+        if timestamp is None:
+            timestamp = arrow.now()
+        if isinstance(timestamp, arrow.Arrow):
+            timestamp = arrow.get(timestamp)
+
+        if status == "started":
+            save_file(
+                self.local_directory("started_at"),
+                str(timestamp) + "\n",
+                # starting event can occur multiple times
+                mode="a",
+            )
+        elif status == "heartbeat":
+            save_file(
+                self.local_directory("heartbeat_at"),
+                str(timestamp),
+                mode="w",
+            )
+        elif status == "finished":
+            save_file(
+                self.local_directory("finished_at"),
+                str(timestamp),
+                mode="w",
+            )
+        else:
+            raise ValueError(
+                f"Invalid status {status}; must be one of 'started', 'heartbeat', 'finished'"
+            )
 
     def created_at(self) -> Optional[DatetimeType]:
         if self.timestamp is None:
             return None
 
         return arrow.get(self.timestamp)
 
     def started_at(self) -> Optional[DatetimeType]:
         """Returns the starting time"""
         if not self.is_mounted():
             return None
-        return self.__model__._storage_instance.retrieve_status(self, "started")
+        return self._retrieve_status("started")
 
     def heartbeat_at(self):
         """Returns the last heartbeat time"""
         if not self.is_mounted():
             return None
-        return self.__model__._storage_instance.retrieve_status(
-            self, "heartbeat"
-        )
+        return self._retrieve_status("heartbeat")
 
     def finished_at(self):
         """Returns the finishing time"""
         if not self.is_mounted():
             return None
-        return self.__model__._storage_instance.retrieve_status(
-            self, "finished"
-        )
+        return self._retrieve_status("finished")
+
+    def _retrieve_status(self, field: str) -> Optional[DatetimeType]:
+        fields = ["started", "heartbeat", "finished"]
+        if field not in fields:
+            raise ValueError(f"Invalid field: {field}. Must be on of {fields}")
+        status = load_file(self.local_directory(f"{field}_at"), default=None)
+        if status is None:
+            return None
+        if field == "started":
+            # can have multiple rows, return latest
+            status = status.strip("\n").split("\n")[-1]
+
+        try:
+            return arrow.get(status)
+        except arrow.ParserError:
+            return None
 
     def is_finished(self):
         """True if finishing time has been written"""
         return bool(self.finished_at())
 
     def is_started(self):
         """True if starting time has been written"""
@@ -345,142 +301,44 @@
 
         return (not self.is_finished()) and (
             (arrow.now() - self.heartbeat_at()).seconds < 30
         )
 
     def is_live(self):
         """True if active or finished"""
-        return self.is_finished() or is_active()
+        return self.is_finished() or self.is_active()
 
     def is_incomplete(self):
         """Shorthand for is_started() and not (is_active() or is_finished())"""
         return self.is_started() and not (
             self.is_active() or self.is_finished()
         )
 
-    def __call__(self) -> None:
-        if self.is_finished():
-            return None
-
-        self.dispatch()
-
-    def dispatch(self) -> "Experiment":
-        """Dispatch the experiment lifecycle"""
-        try:
-            self.on_dispatch()
-
-            self.on_seeding()
-
-            if self.on_write_meta_data() is not False and self.is_mounted():
-                self.mark_started()
-                self._events.on("heartbeat", self.update_heartbeat)
-                self._events.heartbeats(seconds=15)
-                if self.execution:
-                    self.execution.save_file(
-                        "env.json",
-                        data=Project.get().provider().get_host_info(),
-                    )
-
-            # create
-            self.on_before_create()
-            self.on_create()
-            self.on_after_create()
-
-            # execute
-            self.on_before_execute()
-            self.on_execute()
-            self.on_after_execute()
-
-            self.on_success()
-            self.on_finish(success=True)
-
-            # destroy
-            self.on_before_destroy()
-            self._events.heartbeats(None)
-            self.on_destroy()
-            if self.on_write_meta_data() is not False and self.is_mounted():
-                self.update_heartbeat(mark_finished=True)
-
-            self.on_after_destroy()
-
-            self.on_after_dispatch(success=True)
-        except BaseException as _ex:  # pylint: disable=broad-except
-            self.on_failure(exception=_ex)
-            self.on_finish(success=False)
-            self.on_after_dispatch(success=False)
-
-            raise errors.ExecutionFailed(
-                f"{self.__class__.__name__} dispatch failed"
-            ) from _ex
-
-        return self
-
     # life cycle
 
-    def on_write_meta_data(self) -> Optional[bool]:
-        """Event triggered before meta-data such as creation time etc. is written to the storage
-
-        Return False to prevent writing of meta-data
-        """
-
-    def on_before_dispatch(self) -> Optional[bool]:
-        """Event triggered before the dispatch of the experiment"""
+    def __call__(self) -> None:
+        ...
 
     def on_before_commit(self) -> Optional[bool]:
-        """Event triggered before the commit of the experiment"""
-
-    def on_dispatch(self):
-        """Lifecycle event triggered at the very beginning of the component dispatch"""
-
-    def on_seeding(self):
-        """Lifecycle event to implement custom seeding using `self.seed`"""
-        random.seed(self.seed)
-
-    def on_before_create(self):
-        """Lifecycle event triggered before components creation"""
-
-    def on_create(self):
-        """Lifecycle event triggered during components creation"""
-
-    def on_after_create(self):
-        """Lifecycle event triggered after components creation"""
-
-    def on_before_execute(self):
-        """Lifecycle event triggered before components execution"""
+        """Event triggered before the commit of the component"""
 
-    def on_execute(self) -> Any:
-        """Lifecycle event triggered at components execution"""
-        return True
-
-    def on_after_execute_iteration(self, iteration: int):
-        """Lifecycle event triggered after execution iteration"""
-
-    def on_after_execute(self):
-        """Lifecycle event triggered after execution"""
-
-    def on_before_destroy(self):
-        """Lifecycle event triggered before components destruction"""
-
-    def on_destroy(self):
-        """Lifecycle event triggered at components destruction"""
+    def on_before_dispatch(self) -> Optional[bool]:
+        """Event triggered before the dispatch of the component"""
 
-    def on_after_destroy(self):
-        """Lifecycle event triggered after components destruction"""
+    def on_success(self):
+        """Lifecycle event triggered iff execution finishes successfully"""
 
     def on_finish(self, success: bool):
         """Lifecycle event triggered right before the end of the component execution
 
         # Arguments
         success: Whether the execution finished sucessfully
         """
 
-    def on_success(self):
-        """Lifecycle event triggered iff execution finishes successfully"""
-
-    def on_failure(self, exception: errors.MachinableError):
+    def on_failure(self, exception: Exception) -> None:
         """Lifecycle event triggered iff the execution finished with an exception
 
         # Arguments
         exception: Execution exception
         """
 
     def on_after_dispatch(self, success: bool):
@@ -488,43 +346,19 @@
 
         This is triggered independent of whether the execution has been successful or not.
 
         # Arguments
         success: Whether the execution finished sucessfully
         """
 
-    # exports
-
-    def dispatch_code(self, inline: bool = True) -> Optional[str]:
-        storage = Storage.get().as_json().replace('"', '\\"')
-        code = f"""
-        from machinable import Project, Storage, Experiment
-        from machinable.errors import StorageError
-        Project('{Project.get().path()}').__enter__()
-        Storage.from_json('{storage}').__enter__()
-        experiment__ = Experiment.find('{self.experiment_id}', timestamp={self.timestamp})
-        experiment__()
-        """
-
-        if inline:
-            code = code.replace("\n        ", ";")[1:-1]
-            return f'{sys.executable} -c "{code}"'
-
-        return code.replace("        ", "")[1:-1]
-
-    def __repr__(self):
-        return f"Experiment [{self.__model__.experiment_id}]"
+    def on_seeding(self):
+        """Lifecycle event to implement custom seeding using `self.seed`"""
+        random.seed(self.seed)
 
-    def __str__(self):
-        return self.__repr__()
+    def on_write_meta_data(self) -> Optional[bool]:
+        """Event triggered before meta-data such as creation time etc. is written to the storage
 
-    def __eq__(self, other):
-        return (
-            self.experiment_id == other.experiment_id
-            and self.timestamp == other.timestamp
-        )
+        Return False to prevent writing of meta-data
+        """
 
-    def __ne__(self, other):
-        return (
-            self.experiment_id != other.experiment_id
-            or self.timestamp != other.timestamp
-        )
+    def on_heartbeat(self) -> None:
+        """Event triggered on heartbeat every 15 seconds"""
```

### Comparing `machinable-4.2.0/src/machinable/group.py` & `machinable-4.3.0/src/machinable/group.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from typing import Any, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Optional, Tuple, Union
 
 from datetime import datetime
 
 from machinable import schema
-from machinable.collection import ExperimentCollection
-from machinable.element import Element, get_lineage, has_many
+from machinable.collection import ComponentCollection
+from machinable.element import get_dump, get_lineage
+from machinable.interface import Interface, has_many
 from machinable.types import VersionType
 
+if TYPE_CHECKING:
+    from machinable.component import Component
+
 
 def normgroup(group: Optional[str]) -> str:
     if group is None:
         return ""
     if not isinstance(group, str):
         raise ValueError(f"Invalid group. Expected str but got '{group}'")
     return group.lstrip("/")
@@ -18,42 +22,38 @@
 
 def resolve_group(group: str) -> Tuple[str, str]:
     group = normgroup(group)
     resolved = datetime.now().strftime(group)
     return group, resolved
 
 
-class Group(Element):
+class Group(Interface):
     """Group element"""
 
     kind = "Group"
 
     def __init__(
         self, group: Optional[str] = None, version: VersionType = None
     ):
         super().__init__(version=version)
         pattern, path = resolve_group(group)
         self.__model__ = schema.Group(
+            kind=self.kind,
             module=self.__model__.module,
             config=self.__model__.config,
             version=self.__model__.version,
             pattern=pattern,
             path=path,
             lineage=get_lineage(self),
         )
+        self.__model__._dump = get_dump(self)
 
     @property
     def pattern(self) -> str:
         return self.__model__.pattern
 
     @property
     def path(self) -> str:
         return self.__model__.path
 
-    @has_many
-    def experiments() -> ExperimentCollection:
-        from machinable.experiment import Experiment
-
-        return Experiment, ExperimentCollection, False
-
     def __repr__(self) -> str:
         return f"Group [{self.path}]"
```

### Comparing `machinable-4.2.0/src/machinable/mixin.py` & `machinable-4.3.0/src/machinable/mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from typing import Any, Callable, Optional
+from typing import TYPE_CHECKING, Any, Callable
 
 from functools import wraps
 from inspect import getattr_static
 
+if TYPE_CHECKING:
+    from machinable.element import Element
+
 
 class Mixin:
     """Mixin base class"""
 
 
 class bind:
     """
@@ -68,17 +71,19 @@
     @property
     @wraps(f)
     def _wrapper(self: "Element"):
         name = f.__name__
         if name not in self.__mixins__:
             mixin_class = f(self)
             if isinstance(mixin_class, str):
-                from machinable.project import Project
+                from machinable.project import Project, import_element
 
-                mixin_class = Project.get()._element(mixin_class, Mixin)
+                mixin_class = import_element(
+                    Project.get().path(), mixin_class, Mixin
+                )
 
             self.__mixins__[name] = bind(self, mixin_class, name)
 
         # assign to __mixin__ for reference
         self.__mixin__ = self.__mixins__[name]
 
         return self.__mixins__[name]
```

### Comparing `machinable-4.2.0/src/machinable/project.py` & `machinable-4.3.0/src/machinable/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 
 import getpass
 import importlib
 import os
 import platform
 import socket
 import sys
+from dataclasses import dataclass
 
 import machinable
 from commandlib import Command
 from machinable import schema
+from machinable.config import Field, validator
 from machinable.element import Element, get_lineage, instantiate, normversion
 from machinable.errors import ConfigurationError
+from machinable.interface import Interface
 from machinable.types import VersionType
 from machinable.utils import (
     find_subclass_in_module,
     get_commit,
     get_diff,
     get_root_commit,
     import_from_directory,
+    is_directory_version,
 )
 
 if TYPE_CHECKING:
     from machinable.project import Project
 
 
 def fetch_link(source, target):
@@ -120,61 +124,91 @@
                 os.symlink(top_level, target, target_is_directory=True)
 
             break
 
     return vendors
 
 
-class Project(Element):
+def import_element(
+    directory: str, module: str, base_class: Any = None
+) -> "Element":
+    if base_class is None:
+        base_class = Element
+
+    # import project-relative
+    module = (
+        import_from_directory(
+            module,
+            directory,
+            or_fail=False,
+        )
+        or module
+    )
+
+    # import globally
+    if isinstance(module, str):
+        try:
+            module = importlib.import_module(module)
+        except ModuleNotFoundError as _e:
+            raise ModuleNotFoundError(
+                f"Could not find module '{module}' in project {directory}"
+            ) from _e
+
+    element_class = find_subclass_in_module(module, base_class)
+    if element_class is None:
+        raise ConfigurationError(
+            f"Could not find an element inheriting from the {base_class.__name__} base class. "
+            f"Is it correctly defined in {module.__name__}?"
+        )
+
+    return element_class
+
+
+class Project(Interface):
     kind = "Project"
 
+    @dataclass
+    class Config:
+        directory: Optional[str] = Field(default_factory=lambda: os.getcwd())
+
+        @validator("directory")
+        def normalize_directory(cls, v):
+            return os.path.normpath(os.path.abspath(os.path.expanduser(v)))
+
     def __init__(
         self,
-        directory: Optional[str] = None,
         version: VersionType = None,
-        name: Optional[str] = None,
     ):
-        super().__init__()
-        if directory is None:
-            directory = os.getcwd()
-        directory = os.path.abspath(directory)
-        if name is None:
-            name = os.path.basename(directory)
+        if is_directory_version(version):
+            # interpret as shortcut for directory
+            version = {"directory": version}
+        super().__init__(version=version)
         self.__model__ = schema.Project(
-            directory=directory,
-            name=name,
+            kind=self.kind,
             version=normversion(version),
             lineage=get_lineage(self),
         )
         self._parent: Optional[Project] = None
         self._provider: str = "_machinable/project"
         self._resolved_provider: Optional[Project] = None
 
-    @classmethod
-    def instance(
-        cls,
-        directory: Optional[str] = None,
-        version: VersionType = None,
-    ) -> "Project":
-        return Project(directory, version).provider()
-
     def provider(self, reload: Union[str, bool] = False) -> "Project":
         """Resolves and returns the provider instance"""
         if isinstance(reload, str):
             self._provider = reload
             self._resolved_provider = None
         if self._resolved_provider is None or reload:
             if isinstance(self._provider, str):
                 self._resolved_provider = find_subclass_in_module(
                     module=import_from_directory(
-                        self._provider, self.__model__.directory
+                        self._provider, self.config.directory
                     ),
                     base_class=Project,
                     default=Project,
-                )(self.__model__.directory, version=self.__model__.version)
+                )(version=self.__model__.version)
             else:
                 self._resolved_provider = Project(
                     version=self.__model__.version
                 )
 
         return self._resolved_provider
 
@@ -183,27 +217,27 @@
         if self.provider().__module__ != "machinable.project":
             return self._provider.replace("/", ".")
 
         return self.provider().__module__
 
     def add_to_path(self) -> None:
         if (
-            os.path.exists(self.__model__.directory)
-            and self.__model__.directory not in sys.path
+            os.path.exists(self.config.directory)
+            and self.config.directory not in sys.path
         ):
             if self.is_root():
-                sys.path.insert(0, self.__model__.directory)
+                sys.path.insert(0, self.config.directory)
             else:
-                sys.path.append(self.__model__.directory)
+                sys.path.append(self.config.directory)
 
     def name(self) -> str:
-        return self.__model__.name
+        return os.path.basename(self.config.directory)
 
     def path(self, *append: str) -> str:
-        return os.path.join(self.__model__.directory, *append)
+        return os.path.join(self.config.directory, *append)
 
     def is_root(self) -> bool:
         return self._parent is None
 
     def get_root(self) -> "Project":
         if self.is_root():
             return self
@@ -223,104 +257,85 @@
                 # todo: how to ignore vendors?
             ]
         except FileNotFoundError:
             return []
 
     def get_code_version(self) -> dict:
         return {
-            "id": get_root_commit(self.__model__.directory),
-            "project": get_commit(self.__model__.directory),
+            "id": get_root_commit(self.config.directory),
+            "project": get_commit(self.config.directory),
             "vendor": {
                 vendor: get_commit(self.path("vendor", vendor))
                 for vendor in self.get_vendors()
             },
         }
 
-    def _element(self, module: str, base_class: Any = None) -> "Element":
-        if base_class is None:
-            base_class = Element
-
-        # import project-relative
-        module = (
-            import_from_directory(
-                module,
-                self.path(),
-                or_fail=False,
-            )
-            or module
-        )
-
-        # import globally
-        if isinstance(module, str):
-            try:
-                module = importlib.import_module(module)
-            except ModuleNotFoundError as _e:
-                raise ModuleNotFoundError(
-                    f"Could not find module '{module}' in project {self.path()}"
-                ) from _e
-
-        element_class = find_subclass_in_module(module, base_class)
-        if element_class is None:
-            raise ConfigurationError(
-                f"Could not find an element inheriting from the {base_class.__name__} base class. "
-                f"Is it correctly defined in {module.__name__}?"
-            )
-
-        return element_class
-
     def element(
         self,
-        module: str,
+        module: Union[str, Element],
         version: VersionType = None,
         base_class: Any = None,
         **constructor_kwargs,
     ) -> "Element":
         module, element_class = self.provider().on_resolve_element(module)
-        if not isinstance(element_class, Element):
-            element_class = self._element(module, base_class)
 
-        return instantiate(
+        if not isinstance(module, str):
+            # interactive session element
+            element_class = module
+            module = "__session__" + element_class.__name__
+        else:
+            # import from project
+            if not isinstance(element_class, Element):
+                element_class = import_element(self.path(), module, base_class)
+
+        element = instantiate(
             module,
             element_class,
             version,
             **constructor_kwargs,
         )
 
+        if isinstance(element, Interface):
+            element.push_related("project", self)
+
+        return element
+
     def get_diff(self) -> Union[str, None]:
         return get_diff(self.path())
 
     def exists(self) -> bool:
-        return os.path.exists(self.__model__.directory)
+        return os.path.exists(self.config.directory)
 
     def serialize(self) -> dict:
         return {
-            "directory": self.__model__.directory,
-            "provider": self._provider,
+            "directory": self.config.directory,
         }
 
     @classmethod
     def unserialize(cls, serialized: dict) -> "Project":
-        return cls(**serialized)
+        return cls(serialized)
 
     def get_host_info(self) -> dict:
         """Returned dictionary will be recorded as host information"""
         return {
             "network_name": platform.node(),
             "hostname": socket.gethostname(),
             "machine": platform.machine(),
             "python_version": platform.python_version(),
             "user": getpass.getuser(),
             "argv": sys.argv,
             "machinable_version": machinable.get_version(),
         }
 
-    def on_resolve_element(self, module: str) -> Tuple[str, Optional[Element]]:
+    def on_resolve_element(
+        self, module: Union[str, Element]
+    ) -> Tuple[Union[str, Element], Optional[Element]]:
         """Override element resolution
 
-        Return altered module string or resolved Element class to be used instead.
+        Return altered module and/or resolved Element class to be used instead.
         """
         return module, None
 
     def on_resolve_vendor(
         self, name: str, source: str, target: str
     ) -> Optional[bool]:
         """Event triggered when vendor is resolved
@@ -341,8 +356,8 @@
         return sys.argv[1:]
 
     def global_predicate(self) -> Dict:
         """Project-wide element predicates."""
         return {}
 
     def __repr__(self) -> str:
-        return f"Project({self.__model__.directory})"
+        return f"Project({self.config.directory})"
```

### Comparing `machinable-4.2.0/src/machinable/schedule.py` & `machinable-4.3.0/src/machinable/schedule.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from machinable import schema
-from machinable.collection import ExecutionCollection
-from machinable.element import Element, get_lineage
+from machinable.element import get_dump, get_lineage
+from machinable.interface import Interface
 from machinable.types import VersionType
 
 
-class Schedule(Element):
+class Schedule(Interface):
     """Schedule base class"""
 
     kind = "Schedule"
 
     def __init__(self, version: VersionType = None):
         super().__init__(version)
         self.__model__ = schema.Schedule(
+            kind=self.kind,
             module=self.__model__.module,
             config=self.__model__.config,
             version=self.__model__.version,
             lineage=get_lineage(self),
         )
+        self.__model__._dump = get_dump(self)
```

### Comparing `machinable-4.2.0/src/machinable/settings.py` & `machinable-4.3.0/src/machinable/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from typing import List, Optional, Union
 
 import json
 import os
 
 from machinable.errors import ConfigurationError
-from machinable.schema import Execution, Experiment
 from machinable.types import ElementType
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class Settings(BaseModel):
     default_predicate: Optional[str] = "config,*"
     default_execution: Optional[ElementType] = None
-    default_experiment: Optional[ElementType] = None
+    default_component: Optional[ElementType] = None
+    default_interface: Optional[ElementType] = None
     default_schedule: Optional[ElementType] = None
     default_group: Optional[str] = "%Y_%U_%a/"
-    default_storage: List[Union[str, dict]] = [
-        "machinable.storage.filesystem",
-        {"directory": "./storage"},
-    ]
+    default_storage: Optional[ElementType] = None
+    default_index: Optional[ElementType] = None
 
 
 def get_settings(file="~/.machinable/settings.json"):
     try:
         with open(os.path.expanduser(file)) as f:
             data = json.load(f)
     except FileNotFoundError:
```

### Comparing `machinable-4.2.0/src/machinable/utils.py` & `machinable-4.3.0/src/machinable/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,130 +1,58 @@
 import types
 from types import ModuleType
 from typing import Any, Callable, List, Mapping, Optional, Tuple, Union
 
+import sys
+
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
 import importlib
 import inspect
 import json
 import os
-import pickle
 import random
 import re
 import string
 import sys
 from keyword import iskeyword
 from pathlib import Path
+from uuid import UUID
 
 import arrow
 import commandlib
+import dill as pickle
 import jsonlines
 import omegaconf
-from baseconv import base62
 from flatten_dict import unflatten as _unflatten_dict
 
 if sys.version_info >= (3, 8):
     from importlib import metadata as importlib_metadata
 else:
     import importlib_metadata
 
 from omegaconf.omegaconf import OmegaConf
 
 sentinel = object()
 
 import json
-import threading
-
-from machinable.types import DatetimeType
-from observable import Observable
-
-
-class Events(Observable):
-    def __init__(self) -> None:
-        super().__init__()
-        self._heartbeat = None
-
-    def trigger(self, event: str, *args: Any, **kw: Any) -> list:
-        """Triggers all handlers which are subscribed to an event.
-        Returns True when there were callbacks to execute, False otherwise."""
-        # upstream pending on issue https://github.com/timofurrer/observable/issues/17
-        callbacks = list(self._events.get(event, []))
-        return [callback(*args, **kw) for callback in callbacks]
-
-    def heartbeats(self, seconds=10):
-        if self._heartbeat is not None:
-            self._heartbeat.cancel()
-
-        if seconds is None or int(seconds) == 0:
-            # disable heartbeats
-            return
-
-        def heartbeat():
-            t = threading.Timer(seconds, heartbeat)
-            t.daemon = True
-            t.start()
-            self.trigger("heartbeat")
-            return t
-
-        self._heartbeat = heartbeat()
-
-
-class Jsonable:
-    def as_json(self, stringify=True, **dumps_kwargs):
-        serialized = self.serialize()
-        if stringify:
-            serialized = json.dumps(serialized, **dumps_kwargs)
-        return serialized
-
-    @classmethod
-    def from_json(cls, serialized, **loads_kwargs):
-        if isinstance(serialized, str):
-            serialized = json.loads(serialized, **loads_kwargs)
-        return cls.unserialize(serialized)
 
-    def clone(self):
-        return self.__class__.from_json(self.as_json())
-
-    def serialize(self) -> dict:
-        raise NotImplementedError
-
-    @classmethod
-    def unserialize(cls, serialized: dict) -> Any:
-        raise NotImplementedError
-
-
-class Connectable:
-    """Connectable trait"""
-
-    __connection__: Optional["Connectable"] = None
-
-    @classmethod
-    def is_connected(cls) -> bool:
-        return cls.__connection__ is not None
-
-    @classmethod
-    def get(cls) -> "Connectable":
-        return cls() if cls.__connection__ is None else cls.__connection__
-
-    def __enter__(self):
-        self._outer_connection = (  # pylint: disable=attribute-defined-outside-init
-            self.__class__.__connection__
-        )
-        self.__class__.__connection__ = self
-        return self
-
-    def __exit__(self, *args, **kwargs):
-        if self.__class__.__connection__ is self:
-            self.__class__.__connection__ = None
-        if getattr(self, "_outer_connection", None) is not None:
-            self.__class__.__connection__ = self._outer_connection
-        return self
+from machinable.types import DatetimeType, VersionType
+from pydantic import BaseModel
 
 
 def serialize(obj):
     """JSON serializer for objects not serializable by default json code"""
+    if isinstance(obj, BaseModel):
+        return obj.dict()
+    if isinstance(obj, UUID):
+        return obj.hex
     if isinstance(obj, DatetimeType):
         return str(obj)
     if isinstance(obj, (omegaconf.DictConfig, omegaconf.ListConfig)):
         return OmegaConf.to_container(obj)
     else:
         raise TypeError(f"Unserializable object {obj} of type {type(obj)}")
 
@@ -140,89 +68,42 @@
     """
     if random_state is None or isinstance(random_state, int):
         random_state = random.Random(random_state)
 
     return random_state.randint(0, 2**31 - 1)
 
 
-def as_color(experiment_id: str):
-    return "".join(
-        encode_experiment_id(decode_experiment_id(i) % 16)
-        for i in experiment_id
-    )
-
-
 def timestamp_to_directory(timestamp: float) -> str:
     return (
         arrow.get(timestamp).strftime("%Y-%m-%dT%H%M%S_%f%z").replace("+", "_")
     )
 
 
-def encode_experiment_id(seed, or_fail=True) -> Optional[str]:
-    """Encodes a seed and returns the corresponding experiment ID
-
-    # Arguments
-    seed: int in the range 62^5 <= seed <= 62^6-1
-    or_fail: If True, raises a Value error instead of returning None
-    """
-    try:
-        if not isinstance(seed, int):
-            raise ValueError
-        if 62**5 <= seed <= 62**6 - 1:
-            return base62.encode(seed)
-        raise ValueError
-    except (ValueError, TypeError) as e:
-        if or_fail:
-            raise ValueError(
-                "Seed has to lie in range 62^5 <= seed <= 62^6-1"
-            ) from e
-        return None
-
-
-def decode_experiment_id(experiment_id, or_fail=True) -> Optional[int]:
-    """Decodes a experiment ID into the corresponding seed
-
-    # Arguments
-    experiment_id: The base62 experiment ID
-    or_fail: If True, raises a Value error instead of returning None
-    """
-    try:
-        if not isinstance(experiment_id, str):
-            raise ValueError
-        value = int(base62.decode(experiment_id))
-        if 62**5 <= value <= 62**6 - 1:
-            return value
-        raise ValueError
-    except (ValueError, TypeError) as e:
-        if or_fail:
-            raise ValueError(
-                f"'{experiment_id}' is not a valid experiment ID"
-            ) from e
-        return None
-
-
-def generate_experiment_id(random_state=None) -> int:
-    if random_state is None or isinstance(random_state, int):
-        random_state = random.Random(random_state)
-
-    # ~ 55x10^9 distinct experiment IDs that if represented in base62 are len 6
-    return random_state.randint(62**5, 62**6 - 1)
-
-
 def is_valid_variable_name(name):
     if not isinstance(name, str):
         return False
     return name.isidentifier() and not iskeyword(name)
 
 
 def is_valid_module_path(name):
     return all(map(is_valid_variable_name, name.split(".")))
 
 
-def random_str(length, random_state=None):
+def is_directory_version(version: VersionType) -> bool:
+    if not isinstance(version, str):
+        return False
+    if not version.startswith("~"):
+        return True
+    if "/" in version or "\\" in version or version == "~":
+        return True
+
+    return False
+
+
+def random_str(length: int, random_state=None):
     if random_state is None or isinstance(random_state, int):
         random_state = random.Random(random_state)
 
     return "".join(
         random_state.choice(
             string.ascii_uppercase + string.ascii_lowercase + string.digits
         )
@@ -640,7 +521,59 @@
             commandlib.Command("git", "rev-list", "--parents", "HEAD")
             .in_dir(repository)
             .output()[-1]
             .replace("\n", "")
         )
     except commandlib.exceptions.CommandError:
         return None
+
+
+class Jsonable:
+    def as_json(self, stringify=True, default=serialize, **dumps_kwargs):
+        serialized = self.serialize()
+        if stringify:
+            serialized = json.dumps(serialized, default=default, **dumps_kwargs)
+        return serialized
+
+    @classmethod
+    def from_json(cls, serialized, **loads_kwargs):
+        if isinstance(serialized, str):
+            serialized = json.loads(serialized, **loads_kwargs)
+        return cls.unserialize(serialized)
+
+    def clone(self):
+        return self.__class__.from_json(self.as_json())
+
+    def serialize(self) -> dict:
+        raise NotImplementedError
+
+    @classmethod
+    def unserialize(cls, serialized: dict) -> Any:
+        raise NotImplementedError
+
+
+class Connectable:
+    """Connectable trait"""
+
+    __connection__: Optional["Connectable"] = None
+
+    @classmethod
+    def is_connected(cls) -> bool:
+        return cls.__connection__ is not None
+
+    @classmethod
+    def get(cls) -> "Connectable":
+        return cls() if cls.__connection__ is None else cls.__connection__
+
+    def __enter__(self) -> Self:
+        self._outer_connection = (  # pylint: disable=attribute-defined-outside-init
+            self.__class__.__connection__
+        )
+        self.__class__.__connection__ = self
+        return self
+
+    def __exit__(self, *args, **kwargs) -> Self:
+        if self.__class__.__connection__ is self:
+            self.__class__.__connection__ = None
+        if getattr(self, "_outer_connection", None) is not None:
+            self.__class__.__connection__ = self._outer_connection
+        return self
```

### Comparing `machinable-4.2.0/PKG-INFO` & `machinable-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machinable
-Version: 4.2.0
+Version: 4.3.0
 Summary: A modular configuration system for research projects
 Home-page: https://machinable.org
 License: MIT
 Keywords: machine-learning,research
 Author: Frithjof Gressmann
 Author-email: hello@machinable.org
 Maintainer: Frithjof Gressmann
@@ -19,21 +19,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Requires-Dist: arrow (>=1.2,<2.0)
 Requires-Dist: commandlib (>=0.3.5,<0.4.0)
+Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: flatten-dict (>=0.4,<0.5)
-Requires-Dist: importlib-metadata (>=6.0,<7.0) ; python_version < "3.8"
+Requires-Dist: importlib-metadata (>=6.6,<7.0) ; python_version < "3.8"
 Requires-Dist: jsonlines (>=3.1,<4.0)
-Requires-Dist: observable (>=1.0,<2.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: python-baseconv (>=1.2,<2.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Documentation, https://machinable.org
 Project-URL: Repository, https://github.com/machinable-org/machinable
 Description-Content-Type: text/markdown
 
 # machinable
 
 <div align="center">
```

