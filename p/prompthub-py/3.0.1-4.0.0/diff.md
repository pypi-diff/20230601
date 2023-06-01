# Comparing `tmp/prompthub_py-3.0.1.tar.gz` & `tmp/prompthub_py-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompthub_py-3.0.1.tar", max compression
+gzip compressed data, was "prompthub_py-4.0.0.tar", max compression
```

## Comparing `prompthub_py-3.0.1.tar` & `prompthub_py-4.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11343 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/LICENSE
--rw-r--r--   0        0        0     1639 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/README.md
--rw-r--r--   0        0        0       65 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/prompthub/__init__.py
--rw-r--r--   0        0        0     1903 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/prompthub/prompt.py
--rw-r--r--   0        0        0      439 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-01 09:13:14.590412 prompthub_py-4.0.0/LICENSE
+-rw-r--r--   0        0        0     1639 2023-06-01 09:13:14.590412 prompthub_py-4.0.0/README.md
+-rw-r--r--   0        0        0       65 2023-06-01 09:13:14.590412 prompthub_py-4.0.0/prompthub/__init__.py
+-rw-r--r--   0        0        0     1880 2023-06-01 09:13:14.590412 prompthub_py-4.0.0/prompthub/prompt.py
+-rw-r--r--   0        0        0      439 2023-06-01 09:13:14.590412 prompthub_py-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-4.0.0/PKG-INFO
```

### Comparing `prompthub_py-3.0.1/LICENSE` & `prompthub_py-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prompthub_py-3.0.1/README.md` & `prompthub_py-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `prompthub_py-3.0.1/prompthub/prompt.py` & `prompthub_py-4.0.0/prompthub/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,47 +19,45 @@
     name: str
     tags: List[str]
     meta: Dict[str, str]
     version: str
     text: str
     description: str
 
-
     def to_yaml(self, file: str):
-        with open(file, 'w') as f:
+        with open(file, "w") as f:
             yaml.safe_dump(asdict(self), f)
 
-
     def to_json(self, file: str):
-        with open(file, 'w') as f:
+        with open(file, "w") as f:
             json.dump(asdict(self), f)
 
 
 def from_json(file: str):
     with open(file) as f:
         data = json.load(f)
         return Prompt(
             data["name"],
             data["tags"],
             data["meta"],
             data["version"],
-            data["prompt_text"],
+            data["text"],
             data["description"],
         )
 
 
 def from_yaml(file: str):
     with open(file) as f:
         data = yaml.safe_load(f)
         return Prompt(
             data["name"],
             data["tags"],
             data["meta"],
             data["version"],
-            data["prompt_text"],
+            data["text"],
             data["description"],
         )
 
 
 def fetch(name: str, timeout: float = 30.0):
     """
     Fetches the specified prompt from PromptHUB and
@@ -75,10 +73,10 @@
     res.raise_for_status()
     j = res.json()
     return Prompt(
         j["name"],
         j["tags"],
         j["meta"],
         j["version"],
-        j["prompt_text"],
+        j["text"],
         j["description"],
     )
```

### Comparing `prompthub_py-3.0.1/PKG-INFO` & `prompthub_py-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthub-py
-Version: 3.0.1
+Version: 4.0.0
 Summary: 
 License: Apache-2.0
 Author: deepset.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

