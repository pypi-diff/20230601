# Comparing `tmp/sax-0.8.6.tar.gz` & `tmp/sax-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sax-0.8.6.tar", last modified: Sat Dec 10 15:26:03 2022, max compression
+gzip compressed data, was "sax-0.8.7.tar", last modified: Thu Jun  1 21:42:36 2023, max compression
```

## Comparing `sax-0.8.6.tar` & `sax-0.8.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2022-12-10 15:26:03.948549 sax-0.8.6/
--rw-r--r--   0 flaport   (1000) flaport   (1000)    11344 2022-09-21 21:52:21.000000 sax-0.8.6/LICENSE
--rw-r--r--   0 flaport   (1000) flaport   (1000)     5256 2022-12-10 15:26:03.951882 sax-0.8.6/PKG-INFO
--rw-r--r--   0 flaport   (1000) flaport   (1000)     4847 2022-09-21 21:52:21.000000 sax-0.8.6/README.md
--rw-r--r--   0 flaport   (1000) flaport   (1000)      232 2022-09-21 21:52:21.000000 sax-0.8.6/pyproject.toml
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2022-12-10 15:26:03.948549 sax-0.8.6/sax/
--rw-r--r--   0 flaport   (1000) flaport   (1000)     2699 2022-12-10 15:25:52.000000 sax-0.8.6/sax/__init__.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     6517 2022-12-10 15:25:52.000000 sax-0.8.6/sax/_nbdev.py
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2022-12-10 15:26:03.948549 sax-0.8.6/sax/backends/
--rw-r--r--   0 flaport   (1000) flaport   (1000)      774 2022-12-10 15:25:52.000000 sax-0.8.6/sax/backends/__init__.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     3782 2022-12-10 15:25:52.000000 sax-0.8.6/sax/backends/additive.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     4333 2022-12-10 15:25:52.000000 sax-0.8.6/sax/backends/default.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     3945 2022-12-10 15:25:52.000000 sax-0.8.6/sax/backends/klu.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    10581 2022-12-10 15:25:52.000000 sax-0.8.6/sax/circuit.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     8000 2022-12-10 15:25:52.000000 sax-0.8.6/sax/make_docs.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     8813 2022-12-10 15:25:52.000000 sax-0.8.6/sax/models.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     5770 2022-12-10 15:25:52.000000 sax-0.8.6/sax/multimode.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     6964 2022-12-10 15:25:52.000000 sax-0.8.6/sax/netlist.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     2780 2022-12-10 15:25:52.000000 sax-0.8.6/sax/netlist_cleaning.py
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2022-12-10 15:26:03.948549 sax-0.8.6/sax/nn/
--rw-r--r--   0 flaport   (1000) flaport   (1000)      971 2022-12-10 15:25:52.000000 sax-0.8.6/sax/nn/__init__.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     2749 2022-12-10 15:25:52.000000 sax-0.8.6/sax/nn/core.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     6965 2022-12-10 15:25:52.000000 sax-0.8.6/sax/nn/io.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)      925 2022-12-10 15:25:52.000000 sax-0.8.6/sax/nn/loss.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     2000 2022-12-10 15:25:52.000000 sax-0.8.6/sax/nn/utils.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     1775 2022-12-10 15:25:51.000000 sax-0.8.6/sax/patched.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    10223 2022-12-10 15:25:51.000000 sax-0.8.6/sax/typing_.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    18468 2022-12-10 15:25:52.000000 sax-0.8.6/sax/utils.py
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2022-12-10 15:26:03.948549 sax-0.8.6/sax.egg-info/
--rw-r--r--   0 flaport   (1000) flaport   (1000)     5256 2022-12-10 15:26:03.000000 sax-0.8.6/sax.egg-info/PKG-INFO
--rw-r--r--   0 flaport   (1000) flaport   (1000)      523 2022-12-10 15:26:03.000000 sax-0.8.6/sax.egg-info/SOURCES.txt
--rw-r--r--   0 flaport   (1000) flaport   (1000)        1 2022-12-10 15:26:03.000000 sax-0.8.6/sax.egg-info/dependency_links.txt
--rw-r--r--   0 flaport   (1000) flaport   (1000)      520 2022-12-10 15:26:03.000000 sax-0.8.6/sax.egg-info/requires.txt
--rw-r--r--   0 flaport   (1000) flaport   (1000)        4 2022-12-10 15:26:03.000000 sax-0.8.6/sax.egg-info/top_level.txt
--rw-r--r--   0 flaport   (1000) flaport   (1000)     1108 2022-12-10 15:26:03.951882 sax-0.8.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.600096 sax-0.8.7/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-01 21:41:56.000000 sax-0.8.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      838 2023-06-01 21:42:36.600096 sax-0.8.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-06-01 21:41:56.000000 sax-0.8.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-01 21:41:56.000000 sax-0.8.7/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.596096 sax-0.8.7/sax/
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-06-01 21:41:56.000000 sax-0.8.7/sax/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6517 2023-06-01 21:41:56.000000 sax-0.8.7/sax/_nbdev.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.600096 sax-0.8.7/sax/backends/
+-rw-r--r--   0 root         (0) root         (0)      774 2023-06-01 21:41:56.000000 sax-0.8.7/sax/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-06-01 21:41:56.000000 sax-0.8.7/sax/backends/additive.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-01 21:41:56.000000 sax-0.8.7/sax/backends/default.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2023-06-01 21:41:56.000000 sax-0.8.7/sax/backends/klu.py
+-rw-r--r--   0 root         (0) root         (0)    10676 2023-06-01 21:41:56.000000 sax-0.8.7/sax/circuit.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2023-06-01 21:41:56.000000 sax-0.8.7/sax/make_docs.py
+-rw-r--r--   0 root         (0) root         (0)     8813 2023-06-01 21:41:56.000000 sax-0.8.7/sax/models.py
+-rw-r--r--   0 root         (0) root         (0)     5770 2023-06-01 21:41:56.000000 sax-0.8.7/sax/multimode.py
+-rw-r--r--   0 root         (0) root         (0)     6964 2023-06-01 21:41:56.000000 sax-0.8.7/sax/netlist.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-06-01 21:41:56.000000 sax-0.8.7/sax/netlist_cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.600096 sax-0.8.7/sax/nn/
+-rw-r--r--   0 root         (0) root         (0)      971 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/core.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/io.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/loss.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-06-01 21:41:56.000000 sax-0.8.7/sax/patched.py
+-rw-r--r--   0 root         (0) root         (0)    10223 2023-06-01 21:41:56.000000 sax-0.8.7/sax/typing_.py
+-rw-r--r--   0 root         (0) root         (0)    18468 2023-06-01 21:41:56.000000 sax-0.8.7/sax/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.600096 sax-0.8.7/sax.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 21:42:36.600096 sax-0.8.7/setup.cfg
```

### Comparing `sax-0.8.6/LICENSE` & `sax-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/PKG-INFO` & `sax-0.8.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: sax
-Version: 0.8.6
-Summary: Autograd and XLA for S-parameters
-Author: Floris Laporte
-Author-email: floris.laporte@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/markdown
-Provides-Extra: nojax
-Provides-Extra: jax
-Provides-Extra: full
-Provides-Extra: klu
-Provides-Extra: dev
-License-File: LICENSE
-
 # SAX
 
 > S + Autograd + XLA
 
 ![](docs/logo.svg)
 
 Autograd and XLA for S-parameters - a scatter parameter circuit simulator and
@@ -132,15 +116,15 @@
 plt.figlegend(ncol=2, loc="upper center")
 plt.show()
 ```
 
 ![png](docs/output_10_0.png)
 
 Those are the basics. For more info, check out the **full**
-[SAX Quick Start page](https://flaport.github.io/sax/quick_start) or the rest of the [Documentation](https://flaport.github.io/sax).
+[SAX Quick Start page](https://flaport.github.io/sax/examples/01_quick_start.html) or the rest of the [Documentation](https://flaport.github.io/sax).
 
 ## Installation
 
 On Linux, the recommended way to install SAX is as follows:
 
 ```sh
 pip install sax[jax]
```

### Comparing `sax-0.8.6/sax/__init__.py` & `sax-0.8.7/sax/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __all__ = []
 
 # Internal Cell
 #nbdev_comment from __future__ import annotations
 
 __author__ = "Floris Laporte"
-__version__ = "0.8.6"
+__version__ = "0.8.7"
 
 # Cell
 from functools import partial as partial
 from math import pi as pi
 
 from scipy.constants import c as c
```

### Comparing `sax-0.8.6/sax/_nbdev.py` & `sax-0.8.7/sax/_nbdev.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/backends/__init__.py` & `sax-0.8.7/sax/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/backends/additive.py` & `sax-0.8.7/sax/backends/additive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/08c_backends_additive.ipynb (unless otherwise specified).
 
+
+from __future__ import annotations
+
+
 __all__ = ['split_port', 'graph_edges', 'prune_internal_output_nodes', 'get_possible_paths', 'path_lengths',
            'evaluate_circuit_additive']
 
 # Cell
+#nbdev_comment from __future__ import annotations
+
 from typing import Dict, Tuple
 
 import networkx as nx
 from ..typing_ import SDict, SType, sdict
 
 try:
     import jax.numpy as jnp
```

### Comparing `sax-0.8.6/sax/backends/default.py` & `sax-0.8.7/sax/backends/default.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/backends/klu.py` & `sax-0.8.7/sax/backends/klu.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/circuit.py` & `sax-0.8.7/sax/circuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 # Cell
 #nbdev_comment from __future__ import annotations
 
 import os
 import shutil
 import sys
 from functools import partial
-from pprint import pprint
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, TypedDict, Union
 
 import black
 import networkx as nx
 import numpy as np
 from pydantic import ValidationError
 from sax import reciprocal
 from .backends import circuit_backends
 from .multimode import multimode, singlemode
-from .netlist import Netlist, RecursiveNetlist, load_recursive_netlist
+from .netlist import Netlist, RecursiveNetlist
 from .netlist_cleaning import remove_unused_instances
 from .typing_ import Model, Settings, SType
 from .utils import _replace_kwargs, get_settings, merge_dicts, update_settings
 
 # Cell
 def create_dag(
     netlist: RecursiveNetlist,
@@ -37,62 +36,72 @@
     if models is None:
         models = {}
     assert isinstance(models, dict)
 
     all_models = {}
     g = nx.DiGraph()
 
-    for model_name, subnetlist in netlist.dict()['__root__'].items():
+    for model_name, subnetlist in netlist.dict()["__root__"].items():
         if not model_name in all_models:
             all_models[model_name] = models.get(model_name, subnetlist)
             g.add_node(model_name)
         if model_name in models:
             continue
-        for instance in subnetlist['instances'].values():
-            component = instance['component']
+        for instance in subnetlist["instances"].values():
+            component = instance["component"]
             if not component in all_models:
                 all_models[component] = models.get(component, None)
                 g.add_node(component)
             g.add_edge(model_name, component)
 
     # we only need the nodes that depend on the parent...
     parent_node = next(iter(netlist.__root__.keys()))
     nodes = [parent_node, *nx.descendants(g, parent_node)]
     g = nx.induced_subgraph(g, nodes)
 
     return g
 
 # Cell
 
+
 def draw_dag(dag, with_labels=True, **kwargs):
     _patch_path()
-    if shutil.which('dot'):
-        return nx.draw(dag, nx.nx_pydot.pydot_layout(dag, prog='dot'), with_labels=with_labels, **kwargs)
+    if shutil.which("dot"):
+        return nx.draw(
+            dag,
+            nx.nx_pydot.pydot_layout(dag, prog="dot"),
+            with_labels=with_labels,
+            **kwargs
+        )
     else:
         return nx.draw(dag, _my_dag_pos(dag), with_labels=with_labels, **kwargs)
 
+
 def _patch_path():
-    os_paths = {p: None for p in os.environ.get('PATH', '').split(os.pathsep)}
+    os_paths = {p: None for p in os.environ.get("PATH", "").split(os.pathsep)}
     sys_paths = {p: None for p in sys.path}
     other_paths = {os.path.dirname(sys.executable): None}
-    os.environ['PATH'] = os.pathsep.join({**os_paths, **sys_paths, **other_paths})
+    os.environ["PATH"] = os.pathsep.join({**os_paths, **sys_paths, **other_paths})
+
 
 def _my_dag_pos(dag):
     # inferior to pydot
     in_degree = {}
     for k, v in dag.in_degree():
         if v not in in_degree:
             in_degree[v] = []
         in_degree[v].append(k)
 
     widths = {k: len(vs) for k, vs in in_degree.items()}
     width = max(widths.values())
     height = max(widths) + 1
 
-    horizontal_pos = {k: np.linspace(0, 1, w+2)[1:-1]*width for k, w in widths.items()}
+    horizontal_pos = {
+        k: np.linspace(0, 1, w + 2)[1:-1] * width for k, w in widths.items()
+    }
 
     pos = {}
     for k, vs in in_degree.items():
         for x, v in zip(horizontal_pos[k], vs):
             pos[v] = (x, -k)
     return pos
 
@@ -173,15 +182,17 @@
     netlist = _ensure_recursive_netlist_dict(netlist)
 
     # TODO: do the following two steps *after* recursive netlist parsing.
     netlist = remove_unused_instances(netlist)
     netlist, instance_models = _extract_instance_models(netlist)
 
     recnet: RecursiveNetlist = _validate_net(netlist)
-    dependency_dag: nx.DiGraph = _validate_dag(create_dag(recnet, models))  # directed acyclic graph
+    dependency_dag: nx.DiGraph = _validate_dag(
+        create_dag(recnet, models)
+    )  # directed acyclic graph
     models = _validate_models({**(models or {}), **instance_models}, dependency_dag)
     modes = _validate_modes(modes)
     backend = _validate_circuit_backend(backend)
 
     circuit = None
     new_models = {}
     current_models = {}
@@ -202,53 +213,60 @@
         current_models[model_name] = circuit = _flat_circuit(
             flatnet.instances, connections, ports, current_models, backend
         )
 
     assert circuit is not None
     return circuit, CircuitInfo(dag=dependency_dag, models=current_models)
 
+
 class NetlistDict(TypedDict):
     instances: Dict
     connections: Dict[str, str]
     ports: Dict[str, str]
 
+
 RecursiveNetlistDict = Dict[str, NetlistDict]
 
+
 class CircuitInfo(NamedTuple):
     dag: nx.DiGraph
     models: Dict[str, Model]
 
+
 def _ensure_recursive_netlist_dict(netlist):
     if not isinstance(netlist, dict):
         netlist = netlist.dict()
-    if '__root__' in netlist:
-        netlist = netlist['__root__']
-    if 'instances' in netlist:
-        netlist = {'top_level': netlist}
+    if "__root__" in netlist:
+        netlist = netlist["__root__"]
+    if "instances" in netlist:
+        netlist = {"top_level": netlist}
     netlist = {**netlist}
     for k, v in netlist.items():
         netlist[k] = {**v}
     return netlist
 
+
 def _extract_instance_models(netlist):
     models = {}
     for netname, net in netlist.items():
         net = {**net}
-        net['instances'] = {**net['instances']}
-        for name, inst in net['instances'].items():
+        net["instances"] = {**net["instances"]}
+        for name, inst in net["instances"].items():
             if callable(inst):
                 settings = get_settings(inst)
                 if isinstance(inst, partial) and inst.args:
-                    raise ValueError("SAX circuits and netlists don't support partials with positional arguments.")
+                    raise ValueError(
+                        "SAX circuits and netlists don't support partials with positional arguments."
+                    )
                 while isinstance(inst, partial):
                     inst = inst.func
                 models[inst.__name__] = inst
-                net['instances'][name] = {
-                    'component': inst.__name__,
-                    'settings': settings
+                net["instances"][name] = {
+                    "component": inst.__name__,
+                    "settings": settings,
                 }
         netlist[netname] = net
     return netlist, models
 
 
 def _validate_circuit_backend(backend):
     backend = backend.lower()
```

### Comparing `sax-0.8.6/sax/make_docs.py` & `sax-0.8.7/sax/make_docs.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/models.py` & `sax-0.8.7/sax/models.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/multimode.py` & `sax-0.8.7/sax/multimode.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/netlist.py` & `sax-0.8.7/sax/netlist.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/netlist_cleaning.py` & `sax-0.8.7/sax/netlist_cleaning.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,70 +17,68 @@
 except ImportError:
     import numpy as jnp
     JAX_AVAILABLE = False
 
 # Cell
 def _get_connectivity_netlist(netlist):
     connectivity_netlist = {
-        "instances": natsorted(netlist['instances']),
+        "instances": natsorted(netlist["instances"]),
         "connections": [
-            (c1.split(',')[0], c2.split(',')[0]) for c1, c2 in netlist['connections'].items()
+            (c1.split(",")[0], c2.split(",")[0])
+            for c1, c2 in netlist["connections"].items()
         ],
-        "ports": [(p, c.split(',')[0]) for p, c in netlist['ports'].items()],
+        "ports": [(p, c.split(",")[0]) for p, c in netlist["ports"].items()],
     }
     return connectivity_netlist
 
 # Cell
 def _get_connectivity_graph(netlist):
     graph = nx.Graph()
     connectivity_netlist = _get_connectivity_netlist(netlist)
-    for name in connectivity_netlist['instances']:
+    for name in connectivity_netlist["instances"]:
         graph.add_node(name)
-    for c1, c2 in connectivity_netlist['connections']:
+    for c1, c2 in connectivity_netlist["connections"]:
         graph.add_edge(c1, c2)
-    for c1, c2 in connectivity_netlist['ports']:
+    for c1, c2 in connectivity_netlist["ports"]:
         graph.add_edge(c1, c2)
     return graph
 
 # Cell
 def _get_nodes_to_remove(graph, netlist):
     nodes = set()
-    for port in netlist['ports']:
+    for port in netlist["ports"]:
         nodes |= nx.descendants(graph, port)
     nodes_to_remove = set(graph.nodes) - nodes
     return list(nodes_to_remove)
 
 # Cell
 def _remove_unused_instances_flat(flat_netlist):
     flat_netlist = {**flat_netlist}
 
-    flat_netlist['instances'] = {**flat_netlist['instances']}
-    flat_netlist['connections'] = {**flat_netlist['connections']}
-    flat_netlist['ports'] = {**flat_netlist['ports']}
+    flat_netlist["instances"] = {**flat_netlist["instances"]}
+    flat_netlist["connections"] = {**flat_netlist["connections"]}
+    flat_netlist["ports"] = {**flat_netlist["ports"]}
 
     graph = _get_connectivity_graph(flat_netlist)
     names = set(_get_nodes_to_remove(graph, flat_netlist))
 
-    if names:
-        pass#print(names)
-
     for name in list(names):
-        if name in flat_netlist['instances']:
-            del flat_netlist['instances'][name]
+        if name in flat_netlist["instances"]:
+            del flat_netlist["instances"][name]
 
-    for conn1, conn2 in list(flat_netlist['connections'].items()):
+    for conn1, conn2 in list(flat_netlist["connections"].items()):
         for conn in [conn1, conn2]:
-            name, _ = conn.split(',')
-            if name in names and conn1 in flat_netlist['connections']:
-                del flat_netlist['connections'][conn1]
-
-    for pname, conn in list(flat_netlist['ports'].items()):
-        name, _ = conn.split(',')
-        if name in names and pname in flat_netlist['ports']:
-            del flat_netlist['ports'][pname]
+            name, _ = conn.split(",")
+            if name in names and conn1 in flat_netlist["connections"]:
+                del flat_netlist["connections"][conn1]
+
+    for pname, conn in list(flat_netlist["ports"].items()):
+        name, _ = conn.split(",")
+        if name in names and pname in flat_netlist["ports"]:
+            del flat_netlist["ports"][pname]
 
     return flat_netlist
 
 # Cell
 def remove_unused_instances(recursive_netlist):
     recursive_netlist = {**recursive_netlist}
```

### Comparing `sax-0.8.6/sax/nn/__init__.py` & `sax-0.8.7/sax/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/nn/core.py` & `sax-0.8.7/sax/nn/core.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/nn/io.py` & `sax-0.8.7/sax/nn/io.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/nn/loss.py` & `sax-0.8.7/sax/nn/loss.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/nn/utils.py` & `sax-0.8.7/sax/nn/utils.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/patched.py` & `sax-0.8.7/sax/patched.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/typing_.py` & `sax-0.8.7/sax/typing_.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax/utils.py` & `sax-0.8.7/sax/utils.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.6/sax.egg-info/SOURCES.txt` & `sax-0.8.7/sax.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 sax/__init__.py
 sax/_nbdev.py
 sax/circuit.py
 sax/make_docs.py
 sax/models.py
 sax/multimode.py
 sax/netlist.py
```

### Comparing `sax-0.8.6/sax.egg-info/requires.txt` & `sax-0.8.7/sax.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 orjson
 pydantic<2
 pyyaml
 tables
 tqdm
 
 [dev]
-sax[jax]
+sax[full]
 bump2version
 datamodel-code-generator
 flax
 ipykernel
 ipympl
 ipywidgets
 isort
@@ -35,17 +35,17 @@
 pyyaml
 scipy
 tmm
 tqdm
 twine
 
 [full]
-sax[jax]
+sax[jax,klu]
 bokeh
-gdsfactory>=5.33.11
+gdsfactory>=6
 graphviz
 ipykernel
 ipympl
 ipywidgets
 jupyterlab
 matplotlib
 meep
```

