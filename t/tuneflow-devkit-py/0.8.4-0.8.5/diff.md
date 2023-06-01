# Comparing `tmp/tuneflow-devkit-py-0.8.4.tar.gz` & `tmp/tuneflow-devkit-py-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-devkit-py-0.8.4.tar", last modified: Sun May 21 00:58:35 2023, max compression
+gzip compressed data, was "tuneflow-devkit-py-0.8.5.tar", last modified: Thu Jun  1 00:26:45 2023, max compression
```

## Comparing `tuneflow-devkit-py-0.8.4.tar` & `tuneflow-devkit-py-0.8.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.4/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.4/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-05-21 00:53:55.000000 tuneflow-devkit-py-0.8.4/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.827463 tuneflow-devkit-py-0.8.4/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/
--rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     7078 2023-05-10 04:50:11.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/debugger.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8679 2023-05-20 23:50:54.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/translate_utils.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/validation_utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.4/test/test_runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.4/test/test_validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.5/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.5/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-06-01 00:26:18.000000 tuneflow-devkit-py-0.8.5/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.828805 tuneflow-devkit-py-0.8.5/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     7096 2023-06-01 00:19:56.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/debugger.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8697 2023-06-01 00:19:06.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/translate_utils.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-06-01 00:26:45.000000 tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:26:45.838805 tuneflow-devkit-py-0.8.5/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.5/test/test_runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.5/test/test_validation_utils.py
```

### Comparing `tuneflow-devkit-py-0.8.4/LICENSE` & `tuneflow-devkit-py-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.4/PKG-INFO` & `tuneflow-devkit-py-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.4
+Version: 0.8.5
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.4/README.md` & `tuneflow-devkit-py-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.4/pyproject.toml` & `tuneflow-devkit-py-0.8.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-devkit-py"
-version = "0.8.4"
+version = "0.8.5"
 authors = [{ name = "Andantei", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     "AI",
     "music",
```

### Comparing `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/debugger.py` & `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Creates a local debug server for a single plugin.
         '''
 
         if plugin_class is None or bundle_file_path is None:
             raise Exception("plugin_class and bundle_file must be provided")
         validate_plugin(plugin_class=plugin_class)
         self._plugin_class = plugin_class
-        with open(bundle_file_path, 'rb') as bundle_file:
+        with open(bundle_file_path, 'rb', encoding='utf-8') as bundle_file:
             bundle_info = json.load(bundle_file)
             # Validate plugin and bundle.
             plugin_info = find_match_plugin_info(
                 bundle_info=bundle_info, provider_id=plugin_class.provider_id(),
                 plugin_id=plugin_class.plugin_id())
             if plugin_info is None:
                 raise Exception(
```

### Comparing `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/runner.py` & `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         A plugin bundle can contain multiple plugins in the same virtualenv, their information is specified in the bundle.json.
         '''
         for plugin_class in plugin_class_list:
             validate_plugin(plugin_class=plugin_class)
         self._plugin_class_list = plugin_class_list
         self._plugin_info_map = defaultdict(dict)
         self._bundle_info: dict | None = None
-        with open(bundle_file_path, 'r') as bundle_file:
+        with open(bundle_file_path, 'r', encoding='utf-8') as bundle_file:
             bundle_info = json.load(bundle_file)
             self._bundle_info = bundle_info
             # Validate plugin and bundle.
             for plugin_class in plugin_class_list:
                 provider_id = plugin_class.provider_id()
                 plugin_id = plugin_class.plugin_id()
                 plugin_info = find_match_plugin_info(
```

### Comparing `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/translate_utils.py` & `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/translate_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/validation_utils.py` & `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/PKG-INFO` & `tuneflow-devkit-py-0.8.5/src/tuneflow_devkit_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.4
+Version: 0.8.5
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.4/test/test_runner.py` & `tuneflow-devkit-py-0.8.5/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.4/test/test_validation_utils.py` & `tuneflow-devkit-py-0.8.5/test/test_validation_utils.py`

 * *Files identical despite different names*

