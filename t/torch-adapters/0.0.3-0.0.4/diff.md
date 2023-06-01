# Comparing `tmp/torch_adapters-0.0.3.tar.gz` & `tmp/torch_adapters-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_adapters-0.0.3.tar", max compression
+gzip compressed data, was "torch_adapters-0.0.4.tar", max compression
```

## Comparing `torch_adapters-0.0.3.tar` & `torch_adapters-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.3/LICENSE
--rw-r--r--   0        0        0      223 2023-05-30 00:02:18.733760 torch_adapters-0.0.3/README.md
--rw-r--r--   0        0        0      576 2023-05-29 22:43:21.437313 torch_adapters-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.3/src/torch_adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.3/src/torch_adapters/adapters/__init__.py
--rw-r--r--   0        0        0     1146 2023-05-30 14:37:46.194482 torch_adapters-0.0.3/src/torch_adapters/adapters/lora.py
--rw-r--r--   0        0        0      193 2023-05-30 14:23:42.706006 torch_adapters-0.0.3/src/torch_adapters/adapters/mixin.py
--rw-r--r--   0        0        0     3078 2023-05-30 14:31:33.729317 torch_adapters-0.0.3/src/torch_adapters/adapters/prefix_tuning_embedding.py
--rw-r--r--   0        0        0     3033 2023-05-30 14:37:46.906561 torch_adapters-0.0.3/src/torch_adapters/utils.py
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 torch_adapters-0.0.3/setup.py
--rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 torch_adapters-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.4/LICENSE
+-rw-r--r--   0        0        0      223 2023-05-30 00:02:18.733760 torch_adapters-0.0.4/README.md
+-rw-r--r--   0        0        0      576 2023-06-01 21:32:25.317945 torch_adapters-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.4/src/torch_adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.4/src/torch_adapters/adapters/__init__.py
+-rw-r--r--   0        0        0     1146 2023-05-30 14:37:46.194482 torch_adapters-0.0.4/src/torch_adapters/adapters/lora.py
+-rw-r--r--   0        0        0      193 2023-05-30 14:23:42.706006 torch_adapters-0.0.4/src/torch_adapters/adapters/mixin.py
+-rw-r--r--   0        0        0     3161 2023-06-01 19:54:15.021807 torch_adapters-0.0.4/src/torch_adapters/adapters/prompt_tuning.py
+-rw-r--r--   0        0        0     2970 2023-06-01 21:11:08.412133 torch_adapters-0.0.4/src/torch_adapters/utils.py
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 torch_adapters-0.0.4/setup.py
+-rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 torch_adapters-0.0.4/PKG-INFO
```

### Comparing `torch_adapters-0.0.3/LICENSE` & `torch_adapters-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_adapters-0.0.3/pyproject.toml` & `torch_adapters-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-adapters"
-version = "0.0.3"
+version = "0.0.4"
 description = "Small Library of Torch Adaptation modules"
 authors = ["ma2za <mazzapaolo2019@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "torch_adapters", from = "src" }]
 
 repository = "https://github.com/ma2za/torch-adapters"
```

### Comparing `torch_adapters-0.0.3/src/torch_adapters/adapters/lora.py` & `torch_adapters-0.0.4/src/torch_adapters/adapters/lora.py`

 * *Files identical despite different names*

### Comparing `torch_adapters-0.0.3/src/torch_adapters/utils.py` & `torch_adapters-0.0.4/src/torch_adapters/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from operator import attrgetter
 from typing import List, Dict
 
 import torch
 from torch import nn
 
 from .adapters.lora import LoRA
-from .adapters.prefix_tuning_embedding import PrefixTuningEmbedding, PrefixTokenTypeEmbedding, \
-    PrefixAbsolutePositionalEmbedding
+from .adapters.prompt_tuning import PromptTuningEmbedding, PromptTokenTypeEmbedding, \
+    PromptAbsolutePositionalEmbedding
 
 
 # TODO group in una utility class
 
 # TODO consider if unify in one add method with configuration
 
 
@@ -24,48 +24,51 @@
     :param layers_names:
     :param config:
     :return:
     """
     for name, module in model.named_modules():
         if any([i in name for i in layers_names]):
             module_name, attr_name = name.rsplit(".", 1)
-            # TODO check if this check must be added
-            # if attr_name not in layers_names:
-            #   continue
-            module: torch.nn.Module = attrgetter(module_name)(model)
-            attr: torch.nn.Linear = attrgetter(name)(model)
+            if attr_name not in layers_names:
+                continue
+            module: nn.Module = attrgetter(module_name)(model)
+            attr: nn.Linear = attrgetter(name)(model)
+
+            # TODO specialize exception
+            if not isinstance(attr, nn.Linear):
+                raise Exception
+
             module.__setattr__(attr_name, LoRA(
                 attr,
                 alpha=config.get("alpha", 8),
                 r=config.get("r", 8)
             ))
     return model
 
 
-def add_prefix_tuning_embedding(model: nn.Module, embeddings: Dict, config: Dict) -> nn.Module:
+def add_prompt_tuning(model: nn.Module, embeddings: Dict, config: Dict) -> nn.Module:
     for name, module in model.named_modules():
         if any([i in name for i in embeddings.keys()]):
             module_name, attr_name = name.rsplit(".", 1)
             if attr_name not in embeddings.keys():
                 continue
             module: nn.Module = attrgetter(module_name)(model)
             attr: nn.Embedding = attrgetter(name)(model)
             embedding_type = embeddings.get(attr_name)
             extended_embedding = None
             if embedding_type == "word":
-                extended_embedding = PrefixTuningEmbedding(src=attr,
-                                                           prefix_length=config.get("prefix_length", 30),
-                                                           hidden_rank=config.get("hidden_rank"))
+                extended_embedding = PromptTuningEmbedding(src=attr,
+                                                           prompt_length=config.get("prompt_length", 30))
             elif embedding_type == "token_type":
-                extended_embedding = PrefixTokenTypeEmbedding(src=attr,
-                                                              prefix_length=config.get("prefix_length", 30))
+                extended_embedding = PromptTokenTypeEmbedding(src=attr,
+                                                              prompt_length=config.get("prompt_length", 30))
             elif embedding_type == "position":
                 # TODO check relative embeddings
-                extended_embedding = PrefixAbsolutePositionalEmbedding(src=attr,
-                                                                       prefix_length=config.get("prefix_length", 30))
+                extended_embedding = PromptAbsolutePositionalEmbedding(src=attr,
+                                                                       prompt_length=config.get("prompt_length", 30))
             if extended_embedding is None:
                 # TODO replace with custom exception
                 raise Exception
             module.__setattr__(attr_name, extended_embedding)
     return model
```

### Comparing `torch_adapters-0.0.3/setup.py` & `torch_adapters-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'torch-adapters',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Small Library of Torch Adaptation modules',
     'long_description': '# Torch Adapters\n\n> <em>"During a gold rush, sell shovels."</em>\n\n# Introduction\n\nSmall Library of Torch Adaptation modules\n\n# Installation\n\nYou can install torch-adapters using:\n\n    $ pip install torch-adapters\n\n# Usage\n\n',
     'author': 'ma2za',
     'author_email': 'mazzapaolo2019@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ma2za/torch-adapters',
```

### Comparing `torch_adapters-0.0.3/PKG-INFO` & `torch_adapters-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-adapters
-Version: 0.0.3
+Version: 0.0.4
 Summary: Small Library of Torch Adaptation modules
 Home-page: https://github.com/ma2za/torch-adapters
 License: MIT
 Keywords: lora,adapters,llm,transformers,bert
 Author: ma2za
 Author-email: mazzapaolo2019@gmail.com
 Requires-Python: >=3.8,<4.0
```

