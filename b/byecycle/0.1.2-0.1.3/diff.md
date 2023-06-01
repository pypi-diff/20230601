# Comparing `tmp/byecycle-0.1.2.tar.gz` & `tmp/byecycle-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byecycle-0.1.2.tar", last modified: Fri May 26 19:25:15 2023, max compression
+gzip compressed data, was "byecycle-0.1.3.tar", last modified: Thu Jun  1 15:08:35 2023, max compression
```

## Comparing `byecycle-0.1.2.tar` & `byecycle-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-05-26 19:23:38.316533 byecycle-0.1.2/LICENSE
--rw-r--r--   0        0        0     5375 2023-05-26 19:23:38.316533 byecycle-0.1.2/README.md
--rw-r--r--   0        0        0     1569 2023-05-26 19:25:15.970280 byecycle-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      147 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/__init__.py
--rw-r--r--   0        0        0     4064 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/cli.py
--rw-r--r--   0        0        0     2583 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/draw/__init__.py
--rw-r--r--   0        0        0    12094 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/graph.py
--rw-r--r--   0        0        0     6959 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/misc.py
--rw-r--r--   0        0        0        0 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/py.typed
--rw-r--r--   0        0        0        0 2023-05-26 19:23:38.316533 byecycle-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      155 2023-05-26 19:23:38.316533 byecycle-0.1.2/tests/test_module_imports.py
--rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 byecycle-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-01 15:07:04.217387 byecycle-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4870 2023-06-01 15:07:04.217387 byecycle-0.1.3/README.md
+-rw-r--r--   0        0        0     1651 2023-06-01 15:08:35.780552 byecycle-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/__init__.py
+-rw-r--r--   0        0        0       79 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/__main__.py
+-rw-r--r--   0        0        0     4097 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/cli.py
+-rw-r--r--   0        0        0     2583 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/draw/__init__.py
+-rw-r--r--   0        0        0    12763 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/graph.py
+-rw-r--r--   0        0        0     8113 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/misc.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/py.typed
+-rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     3295 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0      299 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/test_module_imports.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/test_scenarios/__init__.py
+-rw-r--r--   0        0        0    11315 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/test_scenarios/test_basics.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/test_scenarios/test_drawings.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0      592 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/unit/test_graph.py
+-rw-r--r--   0        0        0     5533 1970-01-01 00:00:00.000000 byecycle-0.1.3/PKG-INFO
```

### Comparing `byecycle-0.1.2/LICENSE` & `byecycle-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `byecycle-0.1.2/README.md` & `byecycle-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 [![license](https://img.shields.io/pypi/l/byecycle)](https://github.com/a-recknagel/byecycle/blob/main/LICENSE)
 [![chat](https://img.shields.io/badge/chat-gitter-mediumturquoise)](https://matrix.to/#/#chextra:gitter.im)
 
 Find and expose cyclic imports in python projects.
 
 ## Installation
 
-`byecycle` uses the build-in [ast module](https://docs.python.org/3/library/ast.html#ast.parse)
+`byecycle` uses the built-in [ast module](https://docs.python.org/3/library/ast.html#ast.parse)
 to parse code files. As a consequence, it can only handle python code within the same
-major version (read: no support for python 1 and 2), and the same or lower minor version 
-of the python interpreter it was installed with. If `byecycle` raises `SyntaxErrors` in 
-code that you know to be working, try using a `byecycle` that is installed with the same 
+major version (read: no support for python 1 and 2), and the same or lower minor version
+of the python interpreter it was installed with. If `byecycle` raises `SyntaxError`s in
+code that you know to be working, try using a `byecycle` that is installed with the same
 python version that can run the code in question.
 
-### From pyPI
-#### Requirements: 
+### From PyPI
+#### Requirements:
  - python 3.11 or higher
  - [pipx](https://pypa.github.io/pipx/installation/)
 ```shell
 pipx install byecycle
 ```
 ---
 
@@ -31,15 +31,15 @@
 #### Requirements:
  - python 3.11 or higher
  - [pdm](https://pdm.fming.dev/)
  - git
 ```shell
 git clone https://github.com/a-recknagel/byecycle.git
 cd byecycle
-pdm install
+pdm install -G:all
 ```
 
 ## Usage
 
 ### As a Command Line Tool
 
 ```shell
@@ -64,48 +64,15 @@
     "byecycle.misc": {
       "tags": [
         "vanilla"
       ],
       "cycle": null
     }
   },
-  "byecycle.draw": {
-    "byecycle": {
-      "tags": [
-        "parent"
-      ],
-      "cycle": null
-    }
-  },
-  "byecycle.cli": {
-    "byecycle": {
-      "tags": [
-        "parent"
-      ],
-      "cycle": null
-    },
-    "byecycle.misc": {
-      "tags": [
-        "vanilla"
-      ],
-      "cycle": null
-    },
-    "byecycle.graph": {
-      "tags": [
-        "vanilla"
-      ],
-      "cycle": null
-    },
-    "byecycle.draw": {
-      "tags": [
-        "vanilla"
-      ],
-      "cycle": null
-    }
-  },
+  [...]
   "byecycle": {
     "byecycle.graph": {
       "tags": [
         "vanilla",
         "parent"
       ],
       "cycle": "complicated"
@@ -114,16 +81,16 @@
 }
 ```
 By default, the result is printed with some rich formatting to highlight types and such.
 If you need the output to be plain ascii, pass the `--no-rich` flag.
 
 ---
 
-For bigger projects, you might get much more complex output. The intent of returning 
-`json` is to have something that can be easily piped into e.g. `jquery` for further 
+For bigger projects, you might get much more complex output. The intent of returning
+`json` is to have something that can be easily piped into e.g. `jq` for further
 processing:
 
 ```shell
 # filter out imports that don't have a cycle
 byecycle byecycle | jq '.[] |= (.[] |= select(.cycle != null) | select(. != {}))'
 ```
 ```json
@@ -182,28 +149,28 @@
 byecycle.cli -> byecycle -> complicated
 byecycle -> byecycle.graph -> complicated
 byecycle -> byecycle.cli -> complicated
 ```
 
 ---
 
-See the help text of `byecycle` for an explanation of tags/`ImportKind`s and 
-cycle/`EdgeKind`s. 
+See the help text of `byecycle` for an explanation of tags/`ImportKind`s and
+cycle/`EdgeKind`s.
 
 In short, if there is a cycle, the tags of all involved imports inform
 the cycle-severity, with the highest severity winning out if multiple apply. The defaults
 can be overriden in order to isolate, filter, or highlight cycles with specific 
-tags/severities.
+severities.
 
 ### To Visualize the Import Graph
 
 If you pass the `--draw` flag<sup>1</sup> on your command-line-call, `byecycle` will create an image of
 the import graph instead:
 
 ```shell
 byecycle byecycle --draw
 ```
 <img src="https://github.com/a-recknagel/byecycle/assets/2063412/e5e8427c-8554-4ce5-9f9f-e2e9eca40742" alt="Plot of imports in the byecycle project" width="320" height="240">
 <img src="https://github.com/a-recknagel/byecycle/assets/2063412/a00586db-e71e-4e74-94ed-0709129920b0" alt="Legend for nodes in the plot" width="320" height="240">
 
 ---
-<sup>[1]<sub> Requires installation of the `draw`-extra, i.e. `pipx install "byecycle[draw]"`.</sub></sup>
+<sup>[1]</sup><sub> Requires installation of the `draw`-extra, i.e. `pipx install "byecycle[draw]"`.</sub>
```

### Comparing `byecycle-0.1.2/pyproject.toml` & `byecycle-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "byecycle"
-version = "0.1.2"
+version = "0.1.3"
 description = "Find and expose cyclic imports in python projects."
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [
     { name = "Arne Caratti", email = "arne.recknagel@hotmail.com" },
 ]
 classifiers = [
@@ -49,14 +49,17 @@
     "mkdocstrings[python]>=0.21.2",
     "mkdocs-material>=9.1.14",
 ]
 test = [
     "pytest>=7.3.1",
     "pytest-cov>=4.1.0",
     "mypy>=1.3.0",
+    "click>=8.1.3",
+    "pip>=23.1.2",
+    "pytest-mock>=3.10.0",
 ]
 security = [
     "safety>=2.3.4",
     "bandit>=1.7.5",
 ]
 
 [tool.mypy]
@@ -77,14 +80,15 @@
 
 [tool.coverage.paths]
 source = [
     "src",
 ]
 
 [tool.coverage.report]
+fail_under = 80
 show_missing = true
 
 [tool.black]
 line-length = 90
 
 [tool.isort]
 profile = "black"
```

### Comparing `byecycle-0.1.2/src/byecycle/cli.py` & `byecycle-0.1.3/src/byecycle/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import importlib
+import importlib.util
 import json
 import os.path
 from pathlib import Path
 
 import networkx as nx  # type: ignore
 import typer
 from rich import print, print_json
@@ -74,40 +74,39 @@
     *,
     dynamic: EdgeKind = severity["dynamic"],
     conditional: EdgeKind = severity["conditional"],
     typing: EdgeKind = severity["typing"],
     parent: EdgeKind = severity["parent"],
     vanilla: EdgeKind = severity["vanilla"],
 ) -> tuple[GraphDict, nx.DiGraph, str]:
-    """Programmatic equivalent to running this package through the CLI.
+    """Programmatic equivalent of running this package through the CLI.
 
     Args:
         project: Either the path to a project source, or the name of an installed package.
         dynamic: Severity of dynamic import cycles.
         conditional: Severity of conditional import cycles.
         typing: Severity of typing-only import cycles.
         parent: Severity of parent-package-resolution related import cycles.
         vanilla: Severity of vanilla import cycles.
 
-
     Returns:
         A dictionary-representation of the import graph.
         The actual import graph.
         The name of the package.
     """
     if os.path.isdir(project):
         project_path = Path(project)
     else:
-        loc = importlib.import_module(project).__file__
-        if loc is None:
+        spec = importlib.util.find_spec(project)
+        if spec is None or spec.origin is None:
             raise RuntimeError(
-                f"Failed trying to resolve {project=} as a package, please pass source "
-                f"code location as proper path."
+                f"Failed trying to resolve {project=} as a package, please pass the "
+                f"source code location as proper path."
             )
-        project_path = Path(loc).parent.resolve()
+        project_path = Path(spec.origin).parent.resolve()
 
     Module.populate(project_path)
     graph = build_digraph(
         [*Module.modules()],
         dynamic=dynamic,
         conditional=conditional,
         typing=typing,
```

### Comparing `byecycle-0.1.2/src/byecycle/draw/__init__.py` & `byecycle-0.1.3/src/byecycle/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `byecycle-0.1.2/src/byecycle/graph.py` & `byecycle-0.1.3/src/byecycle/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,32 +59,44 @@
             for node in Module.modules():
                 if other.startswith(node.name):
                     target = node
                     break
             else:
                 # when calling this function, filter with `startswith(package)` to avoid
                 # this exception
-                raise RuntimeError
+                raise RuntimeError(f"Tried to add non-local import {other=}.")
         else:
             # bad parameter type
-            raise RuntimeError
+            raise RuntimeError(f"Tried to use invalid type {type(other)} as module.")
 
         self.imports[target].add(tag)
 
     def __hash__(self):
+        """Setting the hash of a module to be equal to its name's hash.
+
+        That way, module objects can be found in hash maps by searching for their name
+        as a string. Also means that you can't mix strings and modules in said hash maps
+        without getting very confusing bugs. But, you know, why would you ever want to do
+        that anyway, right?
+        """
         return self.name.__hash__()
 
-    def __repr__(self):
+    def __str__(self):
         imports = {
-            k.name: v if v else "∅"
+            k.name: v
             for k, v in sorted(
                 self.imports.items(), key=lambda x: x[0].name, reverse=True
             )
         }
-        return f"Module('{self.name}') -> {imports}"
+        return f"'{self.name}' -> {imports}"
+
+    @classmethod
+    def reset(cls):
+        cls._modules = []
+        cls._sorted = False
 
     @classmethod
     def modules(cls) -> Iterable[Module]:
         """Accessor for all registered modules."""
         yield from cls._modules
 
     @classmethod
@@ -103,18 +115,19 @@
 
         See Also:
             [discuss.python.org: Partial Modules](https://discuss.python.org/t/question-understanding-imports-a-bit-better-how-are-cycles-avoided/26647/2)
             for a technical explanation of how parent and child modules interact during
             imports.
 
         Notes:
-            This method can only be called once all Nodes have been initialised.
+            This method wil only produce accurate results once all Nodes have been
+            initialised.
         """
         nodes: dict[str, Module] = {node.name: node for node in cls.modules()}
-        for node in cls.modules():
+        for node in [*cls.modules()]:  # node.add() may shuffle cls.modules
             package = node.name.rsplit(".", 1)[0]  # only direct parent, not grandparents
             if package in nodes and package != node.name:
                 node.add(nodes[package], "parent")
 
     @classmethod
     def populate(cls, source_path: Path):
         """Walks down a source tree and registers each python file as a [`Module`][byecycle.graph.Module].
@@ -145,21 +158,26 @@
         :   Due to the module in question being a parent of the current module (in python,
             parent modules are imported before their children)
 
         If a module is imported multiple times in different ways, all their metadata is
         aggregated on the same entry.
 
         Once this method was executed, the [`Module.modules`][byecycle.graph.Module.modules]
-        class-method can called to produce all created modules.
+        class-method can be called to produce all created modules.
+
+        Note:
+            Since `populate` takes place at the class-level, calling this funtion multiple
+            times will clear the data from a previous call.
 
         Args:
             source_path: Location of the source tree of the package that should be walked.
                 The `.name` attribute of this parameter is assumed to be the name of the
                 package in order to identify which imports are local imports.
         """
+        cls.reset()
         node_data: dict[Module, list[tuple[str, ImportKind]]] = {}
         package_name = source_path.name
 
         # walk the project, compile all python files, collect their import statements
         for path in source_path.rglob("*"):
             if not path.name.endswith(".py"):
                 continue
@@ -214,38 +232,35 @@
 
         Returns:
             The identified [`ImportKind`][byecycle.misc.ImportKind], by default `vanilla`.
         """
         parent: ast.AST = node._parent  # type: ignore[union-attr]
         match parent:
             case ast.If(
-                _parent=ast.Module,  # type: ignore[misc]
+                _parent=ast.Module(),  # type: ignore[misc]
                 test=(ast.Name(id="TYPE_CHECKING") | ast.Attribute(attr="TYPE_CHECKING")),
             ):
                 # guarded by `if typing.TYPE_CHECKING:`
                 return "typing"
-            case ast.If(_parent=ast.Module):  # type: ignore[misc]
+            case ast.If(_parent=ast.Module()):  # type: ignore[misc]
                 # probably guarded by `if sys.version >= (x, y, z):`, but doesn't actually
                 # matter -- anything but TYPE_CHECKING is env-dependent during runtime or
                 # too obtuse to consider (I'm not writing code that checks for `if True:`)
                 return "conditional"
-            case ast.AST(_parent=current):  # type: ignore[misc]
+            case _:
                 while True:
                     # test if the import happens somewhere in a function
-                    if isinstance(current, (ast.FunctionDef, ast.AsyncFunctionDef)):
+                    if isinstance(parent, (ast.FunctionDef, ast.AsyncFunctionDef)):
                         return "dynamic"
                     try:
-                        current = current._parent
+                        parent = parent._parent  # type: ignore[attr-defined]
                     except AttributeError:
                         # any nodes that reach this point are treated as regular toplevel
                         # imports, like imports that happen in a class body
                         return "vanilla"
-            case _:
-                # shouldn't happen, but just in case
-                return "vanilla"
 
     def visit_Import(self, node: ast.Import):
         kind = self.find_import_kind(node)
         for alias in node.names:
             self.imports.append((alias.name, kind))
 
     def visit_ImportFrom(self, node: ast.ImportFrom):
@@ -264,15 +279,16 @@
             self.imports.append((f"{module}.{alias.name}", kind))
 
 
 def build_digraph(modules: list[Module], **kwargs: Unpack[SeverityMap]) -> nx.DiGraph:
     """Turns a module-imports-mapping into a smart graph object.
 
     Args:
-        modules: [`Module`][byecycle.graph.Module] objects that know what other local modules they import, and how.
+        modules: [`Module`][byecycle.graph.Module] objects that know what other local
+            modules they import, and how.
         **kwargs: Override the default settings for the severity of the "how" when imports
             in local modules might cause import cycles.
 
     Returns:
         A graph object which allows the kind of operations that you'd want when working
         with graph-like structures. Every edge in the graph has a `tags` and a `cycle`
         entry (accessible with `getitem()`) holding metadata that can help interpret how
@@ -281,14 +297,15 @@
     g = nx.DiGraph()
     g.add_nodes_from([m.name for m in modules])
     for module in modules:
         for import_, tags in module.imports.items():
             g.add_edge(module.name, import_.name, tags=tags)
     for e_0, e_1 in g.edges():
         if g.has_edge(e_1, e_0):
-            g[e_0][e_1]["tags"] = g[e_0][e_1]["tags"] | g[e_1][e_0]["tags"]
-            g[e_0][e_1]["cycle"] = cycle_severity(g[e_0][e_1]["tags"], **kwargs)
+            g[e_0][e_1]["cycle"] = cycle_severity(
+                g[e_0][e_1]["tags"], g[e_1][e_0]["tags"], **kwargs
+            )
         else:
             g[e_0][e_1]["cycle"] = None
     for e_0, e_1 in g.edges():
         g[e_0][e_1]["tags"] = [*g[e_0][e_1]["tags"]]
     return g
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `byecycle-0.1.2/src/byecycle/misc.py` & `byecycle-0.1.3/src/byecycle/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,56 @@
 
 The keys on the first level are the qualnames of importing modules, the keys on the second 
 level are the qualnames of imported modules, and the values on the second level contain
 the metadata dictionary of their keyed imports ([`ImportMetaData`][byecycle.misc.ImportMetaData]).
 Metadata consists of a `tags`-list of [`ImportKind`][byecycle.misc.ImportKind]s and a
 `cycle` which is either an [`EdgeKind`][byecycle.misc.EdgeKind] if there is a cycle, or
 `None` if there isn't.
+
+Example:
+    ```py
+    {
+        "foo": {
+            "foo.a": {
+                "tags": ["vanilla"],
+                "cycle": "complicated"
+            }
+        }
+        "foo.a": {
+            "foo": {
+                "tags": ["parent", "vanilla"],
+                "cycle": "complicated"
+            },
+            "foo.c": {
+                "tags": ["vanilla"],
+                "cycle": None
+            }
+        }
+        "foo.b": {
+            "foo": {
+                "tags": ["parent"],
+                "cycle": "complicated"
+            },
+            "foo.c": {
+                "tags": ["typing"],
+                "cycle": "skip"
+            }
+        }
+        "foo.c": {
+            "foo": {
+                "tags": ["parent"],
+                "cycle": None
+            },
+            "foo.b": {
+                "tags": ["vanilla"],
+                "cycle": "skip"
+            }
+        }
+    }
+    ```
 """
 
 
 class SeverityMap(TypedDict, total=False):
     """Mapping of [`ImportKind`][byecycle.misc.ImportKind]s to [`EdgeKind`][byecycle.misc.ImportKind]s."""
 
     dynamic: EdgeKind
@@ -98,35 +140,37 @@
     "typing": "skip",
     "parent": "complicated",
     "vanilla": "bad",
 }
 
 
 def cycle_severity(
-    cycles: Iterable[ImportKind], **kwargs: Unpack[SeverityMap]
+    tags_a: set[ImportKind], tags_b: set[ImportKind], **kwargs: Unpack[SeverityMap]
 ) -> EdgeKind:
-    """Interpret import tags as to their severity if the import was part of a cycle.
+    """Interpret the severity of an import cycle given their tags.
+
+    In general, all tags get thrown in the same bag and the one with the highest mapped
+    severity "wins". Except for the "vanilla" tag, which will only have its severity
+    considered if both imports had "vanilla" in their tag list.
 
     Args:
-        cycles: The iterable of import-kind tags, at least one entry is expected.
+        tags_a: The set of import-kind tags for the first import statement.
+        tags_b: The set of import-kind tags for the second import statement.
         **kwargs: Valid values are keywords equating to [`ImportKind`][byecycle.misc.ImportKind]s
             mapping to [`EdgeKind`][byecycle.misc.ImportKind]s in order to override that
             [`ImportKind`][byecycle.misc.ImportKind]'s severity-interpretation.
 
     Returns:
         A string denoting the severity of the cycle.
     """
-    cycles = [*cycles]
-    if not cycles:
-        raise RuntimeError("Every import statement needs at least one kind-identifier.")
+    tags: set[ImportKind] = tags_a | tags_b
+    if "vanilla" in tags and ("vanilla" not in tags_a or "vanilla" not in tags_b):
+        tags.remove("vanilla")
     severity_map = cast(SeverityMap, {**_default_cycle_severity, **kwargs})
-    cycles = [c for c in cycles if c != "vanilla"]
-    if not cycles:
-        return severity_map["vanilla"]
-    severity = sorted((severity_map[c] for c in cycles), key=edge_order.get)  # type: ignore
+    severity = sorted((severity_map[t] for t in tags), key=edge_order.get)  # type: ignore[arg-type]
     return severity[0]
 
 
 def path_to_module_name(path: str, base: str, name: str) -> str:
     """Turns a file path into a valid module name.
 
     Just an educated guess on my part, I couldn't find an official reference. Chances are
```

### Comparing `byecycle-0.1.2/PKG-INFO` & `byecycle-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byecycle
-Version: 0.1.2
+Version: 0.1.3
 Summary: Find and expose cyclic imports in python projects.
 Author-Email: Arne Caratti <arne.recknagel@hotmail.com>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: 3.11
@@ -27,23 +27,23 @@
 [![license](https://img.shields.io/pypi/l/byecycle)](https://github.com/a-recknagel/byecycle/blob/main/LICENSE)
 [![chat](https://img.shields.io/badge/chat-gitter-mediumturquoise)](https://matrix.to/#/#chextra:gitter.im)
 
 Find and expose cyclic imports in python projects.
 
 ## Installation
 
-`byecycle` uses the build-in [ast module](https://docs.python.org/3/library/ast.html#ast.parse)
+`byecycle` uses the built-in [ast module](https://docs.python.org/3/library/ast.html#ast.parse)
 to parse code files. As a consequence, it can only handle python code within the same
-major version (read: no support for python 1 and 2), and the same or lower minor version 
-of the python interpreter it was installed with. If `byecycle` raises `SyntaxErrors` in 
-code that you know to be working, try using a `byecycle` that is installed with the same 
+major version (read: no support for python 1 and 2), and the same or lower minor version
+of the python interpreter it was installed with. If `byecycle` raises `SyntaxError`s in
+code that you know to be working, try using a `byecycle` that is installed with the same
 python version that can run the code in question.
 
-### From pyPI
-#### Requirements: 
+### From PyPI
+#### Requirements:
  - python 3.11 or higher
  - [pipx](https://pypa.github.io/pipx/installation/)
 ```shell
 pipx install byecycle
 ```
 ---
 
@@ -51,15 +51,15 @@
 #### Requirements:
  - python 3.11 or higher
  - [pdm](https://pdm.fming.dev/)
  - git
 ```shell
 git clone https://github.com/a-recknagel/byecycle.git
 cd byecycle
-pdm install
+pdm install -G:all
 ```
 
 ## Usage
 
 ### As a Command Line Tool
 
 ```shell
@@ -84,48 +84,15 @@
     "byecycle.misc": {
       "tags": [
         "vanilla"
       ],
       "cycle": null
     }
   },
-  "byecycle.draw": {
-    "byecycle": {
-      "tags": [
-        "parent"
-      ],
-      "cycle": null
-    }
-  },
-  "byecycle.cli": {
-    "byecycle": {
-      "tags": [
-        "parent"
-      ],
-      "cycle": null
-    },
-    "byecycle.misc": {
-      "tags": [
-        "vanilla"
-      ],
-      "cycle": null
-    },
-    "byecycle.graph": {
-      "tags": [
-        "vanilla"
-      ],
-      "cycle": null
-    },
-    "byecycle.draw": {
-      "tags": [
-        "vanilla"
-      ],
-      "cycle": null
-    }
-  },
+  [...]
   "byecycle": {
     "byecycle.graph": {
       "tags": [
         "vanilla",
         "parent"
       ],
       "cycle": "complicated"
@@ -134,16 +101,16 @@
 }
 ```
 By default, the result is printed with some rich formatting to highlight types and such.
 If you need the output to be plain ascii, pass the `--no-rich` flag.
 
 ---
 
-For bigger projects, you might get much more complex output. The intent of returning 
-`json` is to have something that can be easily piped into e.g. `jquery` for further 
+For bigger projects, you might get much more complex output. The intent of returning
+`json` is to have something that can be easily piped into e.g. `jq` for further
 processing:
 
 ```shell
 # filter out imports that don't have a cycle
 byecycle byecycle | jq '.[] |= (.[] |= select(.cycle != null) | select(. != {}))'
 ```
 ```json
@@ -202,28 +169,28 @@
 byecycle.cli -> byecycle -> complicated
 byecycle -> byecycle.graph -> complicated
 byecycle -> byecycle.cli -> complicated
 ```
 
 ---
 
-See the help text of `byecycle` for an explanation of tags/`ImportKind`s and 
-cycle/`EdgeKind`s. 
+See the help text of `byecycle` for an explanation of tags/`ImportKind`s and
+cycle/`EdgeKind`s.
 
 In short, if there is a cycle, the tags of all involved imports inform
 the cycle-severity, with the highest severity winning out if multiple apply. The defaults
 can be overriden in order to isolate, filter, or highlight cycles with specific 
-tags/severities.
+severities.
 
 ### To Visualize the Import Graph
 
 If you pass the `--draw` flag<sup>1</sup> on your command-line-call, `byecycle` will create an image of
 the import graph instead:
 
 ```shell
 byecycle byecycle --draw
 ```
 <img src="https://github.com/a-recknagel/byecycle/assets/2063412/e5e8427c-8554-4ce5-9f9f-e2e9eca40742" alt="Plot of imports in the byecycle project" width="320" height="240">
 <img src="https://github.com/a-recknagel/byecycle/assets/2063412/a00586db-e71e-4e74-94ed-0709129920b0" alt="Legend for nodes in the plot" width="320" height="240">
 
 ---
-<sup>[1]<sub> Requires installation of the `draw`-extra, i.e. `pipx install "byecycle[draw]"`.</sub></sup>
+<sup>[1]</sup><sub> Requires installation of the `draw`-extra, i.e. `pipx install "byecycle[draw]"`.</sub>
```

