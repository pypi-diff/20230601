# Comparing `tmp/ango-1.0.7.tar.gz` & `tmp/ango-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.7.tar", last modified: Wed May 31 06:32:26 2023, max compression
+gzip compressed data, was "ango-1.0.8.tar", last modified: Thu Jun  1 11:05:04 2023, max compression
```

## Comparing `ango-1.0.7.tar` & `ango-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-31 06:32:26.967955 ango-1.0.7/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-31 06:32:26.967955 ango-1.0.7/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.7/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-31 06:32:26.967955 ango-1.0.7/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.7/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-31 06:32:26.967955 ango-1.0.7/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.7/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.7/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-05-30 11:15:47.000000 ango-1.0.7/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.7/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5437 2023-05-30 11:15:47.000000 ango-1.0.7/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14428 2023-05-31 06:31:57.000000 ango-1.0.7/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-31 06:32:26.967955 ango-1.0.7/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-31 06:32:26.000000 ango-1.0.7/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-31 06:32:26.000000 ango-1.0.7/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-31 06:32:26.000000 ango-1.0.7/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-31 06:32:26.000000 ango-1.0.7/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-31 06:32:26.000000 ango-1.0.7/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-31 06:32:26.967955 ango-1.0.7/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-31 06:32:13.000000 ango-1.0.7/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-01 11:05:04.213060 ango-1.0.8/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-01 11:05:04.213060 ango-1.0.8/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.8/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-01 11:05:04.213060 ango-1.0.8/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.8/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-01 11:05:04.213060 ango-1.0.8/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.8/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.8/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-05-30 11:15:47.000000 ango-1.0.8/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.8/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5036 2023-06-01 09:29:39.000000 ango-1.0.8/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14428 2023-05-31 06:31:57.000000 ango-1.0.8/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-01 11:05:04.213060 ango-1.0.8/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-01 11:05:04.213060 ango-1.0.8/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-06-01 11:04:59.000000 ango-1.0.8/setup.py
```

### Comparing `ango-1.0.7/PKG-INFO` & `ango-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.7
+Version: 1.0.8
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.7/README.md` & `ango-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.7/ango/models/label_category.py` & `ango-1.0.8/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.7/ango/plugin_logger.py` & `ango-1.0.8/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.7/ango/plugins.py` & `ango-1.0.8/ango/plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         scheduler = AsyncIOScheduler()
         scheduler.add_job(self.heartbeat, 'interval', seconds=60)
         scheduler.start()
         self.logger = logging.getLogger()
         self.callback = callback
 
     def on_connect(self):
-        self.logger.warning("Connected")
         self.heartbeat()
+        self.logger.warning("Connected")
 
     def on_disconnect(self):
         self.logger.warning("Disconnected")
 
     def heartbeat(self):
         self.emit('heartbeat', {"id": self.id, "secret": self.secret})
 
@@ -106,23 +106,18 @@
     def on_plugin(self, data):
         workflow = data.get('workflow')
         if not workflow:
             return super().on_plugin(data)
         #data["logger"] = self._get_logger(data)
         data["batches"] = data.get('tags', [])
         api_key = data.get('apiKey')
-        task_id = data.get('labeltask').get('_id')
+        task_id = data.get('taskId')
         sdk = SDK(api_key=api_key, host=self.host)
         answer = self.callback(**data)
-        annotation = {
-            "tools": answer.get("answer").get("objects") + data.get('labeltask').get("answer").get("tools"),
-            "classifications": answer.get("answer").get("classifications") + data.get('labeltask').get("answer").get("classifications"),
-            "relations": answer.get("answer").get("relations") + data.get('labeltask').get("answer").get("relations")
-        }
-        return sdk._annotate(task_id, annotation);
+        return sdk._annotate(task_id, answer.get("answer"));
 
 class FileExplorerPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 
 class BatchModelPlugin(Plugin):
```

### Comparing `ango-1.0.7/ango/sdk.py` & `ango-1.0.8/ango/sdk.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.7/ango.egg-info/PKG-INFO` & `ango-1.0.8/ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.7
+Version: 1.0.8
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.7/setup.py` & `ango-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.7",
+    version="1.0.8",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

