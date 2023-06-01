# Comparing `tmp/tuneflow-devkit-py-0.8.5.tar.gz` & `tmp/tuneflow-devkit-py-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-devkit-py-0.8.5.tar", last modified: Thu Jun  1 00:26:45 2023, max compression
+gzip compressed data, was "tuneflow-devkit-py-0.8.6.tar", last modified: Thu Jun  1 00:46:51 2023, max compression
```

## Comparing `tuneflow-devkit-py-0.8.5.tar` & `tuneflow-devkit-py-0.8.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.5/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.5/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-06-01 00:26:18.000000 tuneflow-devkit-py-0.8.5/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.828805 tuneflow-devkit-py-0.8.5/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/
--rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     7096 2023-06-01 00:19:56.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/debugger.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8697 2023-06-01 00:19:06.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/translate_utils.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/validation_utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.5/test/test_runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.5/test/test_validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.6/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.6/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-06-01 00:46:10.000000 tuneflow-devkit-py-0.8.6/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     7096 2023-06-01 00:19:56.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/debugger.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8805 2023-06-01 00:42:29.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/translate_utils.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4786 2023-06-01 00:41:52.000000 tuneflow-devkit-py-0.8.6/test/test_runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.6/test/test_validation_utils.py
```

### Comparing `tuneflow-devkit-py-0.8.5/LICENSE` & `tuneflow-devkit-py-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.5/PKG-INFO` & `tuneflow-devkit-py-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.5
+Version: 0.8.6
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.5/README.md` & `tuneflow-devkit-py-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.5/pyproject.toml` & `tuneflow-devkit-py-0.8.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-devkit-py"
-version = "0.8.5"
+version = "0.8.6"
 authors = [{ name = "Andantei", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     "AI",
     "music",
```

### Comparing `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/debugger.py` & `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/debugger.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/runner.py` & `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from tuneflow_py import TuneflowPlugin, Song
 from typing import Type, List
 import json
 from msgpack import unpackb, packb
 from tuneflow_devkit.validation_utils import validate_plugin, find_match_plugin_info
 from collections import defaultdict
 from fastapi import FastAPI, Request, Response, Depends, BackgroundTasks
-from pathlib import Path
 import asyncio
 import functools
 from fastapi.middleware.cors import CORSMiddleware
 import traceback
 from nanoid import generate as generate_nanoid
+from urllib.parse import urljoin
 
 
 class Runner:
     def __init__(self, plugin_class_list: List[Type[TuneflowPlugin]], bundle_file_path: str) -> None:
         '''
         Creates a server for a plugin bundle.
 
@@ -72,17 +72,22 @@
 
         @app.middleware("http")
         async def add_vary_origin_header(request: Request, call_next):
             response = await call_next(request)
             response.headers["Vary"] = 'Origin'
             return response
 
-        get_info_path = str(Path(path_prefix).joinpath('plugin-bundle-info'))
-        init_plugin_path = str(Path(path_prefix).joinpath('init-plugin-params'))
-        run_plugin_path = str(Path(path_prefix).joinpath('jobs'))
+        if not path_prefix.endswith('/'):
+            path_prefix += '/'
+
+        get_info_path = urljoin(path_prefix, 'plugin-bundle-info')
+        init_plugin_path = urljoin(path_prefix, 'init-plugin-params')
+        run_plugin_path = urljoin(path_prefix, 'jobs')
+
+        print(f'Serving bundle info at: {get_info_path}')
 
         def init_plugin_task(plugin_class: Type[TuneflowPlugin], song: Song):
             try:
                 params_config = plugin_class.params(song)
                 return {"status": "OK",
                         "paramsConfig": params_config,
                         "params": plugin_class._get_default_params(param_config=params_config)
```

### Comparing `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/translate_utils.py` & `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/translate_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/validation_utils.py` & `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/PKG-INFO` & `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.5
+Version: 0.8.6
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.5/test/test_runner.py` & `tuneflow-devkit-py-0.8.6/test/test_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,26 @@
 
         client = TestClient(app)
         response = client.get("/plugin-bundle-info")
         assert response.status_code == 200
         with open(bundle_file_path, 'r') as bundle_file:
             bundle_info = json.load(bundle_file)
             assert response.json() == bundle_info
+    
+    def test_runner_path_prefix(self):
+        bundle_file_path = str(pathlib.PurePath(
+            __file__).parent.joinpath('hello_world_plugin.bundle.json'))
+        app = Runner(plugin_class_list=[HelloWorldPlugin], bundle_file_path=bundle_file_path).start(path_prefix='/plugins/test')
+
+        client = TestClient(app)
+        response = client.get("/plugins/test/plugin-bundle-info")
+        assert response.status_code == 200
+        with open(bundle_file_path, 'r') as bundle_file:
+            bundle_info = json.load(bundle_file)
+            assert response.json() == bundle_info
 
     def test_auth_enabled_runner(self):
         bundle_file_path = str(pathlib.PurePath(
             __file__).parent.joinpath('hello_world_plugin.bundle.json'))
 
         def auth_failed_handler():
             raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED)
```

### Comparing `tuneflow-devkit-py-0.8.5/test/test_validation_utils.py` & `tuneflow-devkit-py-0.8.6/test/test_validation_utils.py`

 * *Files identical despite different names*

