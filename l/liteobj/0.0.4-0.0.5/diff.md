# Comparing `tmp/liteobj-0.0.4.tar.gz` & `tmp/liteobj-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteobj-0.0.4.tar", last modified: Tue May 30 23:38:59 2023, max compression
+gzip compressed data, was "liteobj-0.0.5.tar", last modified: Thu Jun  1 19:00:33 2023, max compression
```

## Comparing `liteobj-0.0.4.tar` & `liteobj-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:38:59.970169 liteobj-0.0.4/
--rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.4/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-05-30 23:38:59.970169 liteobj-0.0.4/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1066 2023-05-25 23:05:01.000000 liteobj-0.0.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:38:59.970169 liteobj-0.0.4/liteobj/
--rw-r--r--   0 user      (1000) user      (1000)       20 2023-05-25 22:02:13.000000 liteobj-0.0.4/liteobj/__init__.py
--rwxr-xr-x   0 user      (1000) user      (1000)     3056 2023-05-30 23:38:02.000000 liteobj-0.0.4/liteobj/lite.py
--rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.4/liteobj/requirements.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:38:59.970169 liteobj-0.0.4/liteobj.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      275 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       29 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-30 23:38:59.970169 liteobj-0.0.4/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)      706 2023-05-30 22:51:51.000000 liteobj-0.0.4/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 19:00:33.342050 liteobj-0.0.5/
+-rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.5/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 19:00:33.342050 liteobj-0.0.5/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1221 2023-06-01 19:00:09.000000 liteobj-0.0.5/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 19:00:33.342050 liteobj-0.0.5/liteobj/
+-rw-r--r--   0 user      (1000) user      (1000)       20 2023-05-25 22:02:13.000000 liteobj-0.0.5/liteobj/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     3212 2023-06-01 18:46:53.000000 liteobj-0.0.5/liteobj/lite.py
+-rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.5/liteobj/requirements.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 19:00:33.342050 liteobj-0.0.5/liteobj.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      275 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       29 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 19:00:33.342050 liteobj-0.0.5/setup.cfg
+-rwxr-xr-x   0 user      (1000) user      (1000)      706 2023-06-01 18:38:23.000000 liteobj-0.0.5/setup.py
```

### Comparing `liteobj-0.0.4/LICENSE` & `liteobj-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `liteobj-0.0.4/README.md` & `liteobj-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,38 @@
 ## Install
 
 Install from pip
 ```
 pip install liteobj
 ```
 
-## Quickstart Example with Gradio
+## Quickstart Example with Gradio App
 ```
 git clone https://github.com/1lint/liteobj
 cd liteobj
-pip install liteobj==0.0.3 gradio==3.31.0
-lite demo.yaml launch --server_port=7680 --server_name=0.0.0.0
+pip install liteobj==0.0.5 gradio==3.32.0
+lite demo.yaml launch --server_port=7860 --server_name=0.0.0.0
 ```
 CLI syntax is 
 ```
 lite {config_path} {object_method} {method_args} {method_kwargs}
 ```
+
 `config_path` is path to the yaml file to instantiate, and is the only required parameter. Returns the instantiated object instance
 `object_method` is the name of the object method to invoke once the object is instantiated. If passed, returns the output of the object method
 `method_args` and `method_kwargs` are passed directly into the object method. 
 
+Example use as python library 
+```python
+from liteobj import lite
+demo = lite("demo.yaml")
+demo.launch(server_port=7860, server_name="0.0.0.0")
+```
+
+
 ## Tutorial
 (tutorial currently out of date, to be updated)
 See [tutorial.ipynb](https://github.com/1lint/liteobj/blob/master/tutorial.ipynb) for example use of `liteobj` to quickly run training with pytorch-lightning
```

### Comparing `liteobj-0.0.4/liteobj/lite.py` & `liteobj-0.0.5/liteobj/lite.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 from importlib import import_module
 from fire import Fire
-from omegaconf import OmegaConf, DictConfig
-from typing import Any, List
+from omegaconf import OmegaConf, DictConfig, ListConfig
+from typing import Any
 import sys
 from time import time
 from pathlib import Path
 
 SUPER_CONFIG_KEY = 'super'
 CLASS_STRING = 'class_string' 
 
 KWARGS = 'kwargs'
 ARGS = 'args'
 METHOD_KEY = 'method'
 
 METADATA_KEY = 'lite_metadata'
 
-# pack args and kwargs into a list
-def listify(*args, **kwargs) -> List:
-    return [*args, *kwargs.values()]
-
 # recursively load config with superconfigs
 def load_config(yaml_file: str|Path) -> DictConfig:
 
     config = OmegaConf.load(yaml_file)
 
     if SUPER_CONFIG_KEY in config:
         super_configs = []
         for super_config in config[SUPER_CONFIG_KEY]:
             super_configs.append(load_config(super_config))
         config = OmegaConf.unsafe_merge(*super_configs, config)
         
     return config
 
+def process_param(param):
+    
+    if isinstance(param, ListConfig):
+        output_list = []
+        for element in param:
+            element = process_param(element)
+            output_list.append(element)
+        return output_list
+    else:
+        param = instantiate(param) if hasattr(param, CLASS_STRING) else param
+        return param
+
+
 # recursively instantiate objects that have objects as parameters
 def instantiate(config: OmegaConf) -> Any:
 
     class_string = config.get(CLASS_STRING, None)
     if class_string is None:
         raise ValueError(f"Cannot instantiate object without '{CLASS_STRING}' key")
     
@@ -46,30 +55,29 @@
     method_string = config.get(METHOD_KEY, "")
     if method_string is None:
         return module_attribute
 
     kwargs = {}
     if KWARGS in config:
         for k, v in config[KWARGS].items():
-            kwargs[k] = instantiate(v) if hasattr(v, CLASS_STRING) else v
+            kwargs[k] = process_param(v)
  
     args = []
     if ARGS in config:
         for item in config[ARGS]:
-            item = instantiate(item) if hasattr(item, CLASS_STRING) else item
-            args.append(item)
+            args.append(process_param(item))
 
     if method_string == "":
         return module_attribute(*args, **kwargs)
     else:
         method = getattr(module_attribute, method_string)
         return method(*args, **kwargs)
 
 # convenience method for running object from yaml
-def run(yaml_file: str|Path, method_string: str=None, *args, **kwargs) -> Any:
+def lite(yaml_file: str|Path, method_string: str=None, *args, **kwargs) -> Any:
 
     yaml_file = Path(yaml_file)
     sys.path.append(str(Path.cwd()))
     sys.path.append(str(yaml_file.parent.resolve()))
 
     config = load_config(yaml_file)
 
@@ -91,11 +99,11 @@
     try:
         method = getattr(object, method_string)
         return object, method(*args, **kwargs)
     except KeyboardInterrupt:
         return object, None
 
 def main():
-    return Fire(run)
+    return Fire(lite)
 
 if __name__ == '__main__':
     main()
```

### Comparing `liteobj-0.0.4/setup.py` & `liteobj-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 00000060: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
 00000070: 6d65 6e74 7320 3d20 6f70 656e 2866 227b  ments = open(f"{
 00000080: 7265 706f 5f6e 616d 657d 2f7b 7265 7175  repo_name}/{requ
 00000090: 6972 656d 656e 7473 5f66 6e7d 2229 2e72  irements_fn}").r
 000000a0: 6561 6428 292e 7370 6c69 7428 290d 0a0d  ead().split()...
 000000b0: 0a73 6574 7570 286e 616d 653d 7265 706f  .setup(name=repo
 000000c0: 5f6e 616d 652c 0d0a 2020 2020 2020 7665  _name,..      ve
-000000d0: 7273 696f 6e3d 2730 2e30 2e34 272c 0d0a  rsion='0.0.4',..
+000000d0: 7273 696f 6e3d 2730 2e30 2e35 272c 0d0a  rsion='0.0.5',..
 000000e0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
 000000f0: 6e3d 2743 7265 6174 6520 6c69 6768 7477  n='Create lightw
 00000100: 6569 6768 7420 636f 6e66 6967 7320 666f  eight configs fo
 00000110: 7220 696e 7374 616e 7469 6174 696e 6720  r instantiating 
 00000120: 4d4c 2065 7870 6572 696d 656e 7473 272c  ML experiments',
 00000130: 0d0a 2020 2020 2020 6175 7468 6f72 3d27  ..      author='
 00000140: 316c 696e 7427 2c0d 0a20 2020 2020 2061  1lint',..      a
```

