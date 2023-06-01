# Comparing `tmp/spaces-0.2.0.tar.gz` & `tmp/spaces-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.2.0.tar", max compression
+gzip compressed data, was "spaces-0.2.1.tar", max compression
```

## Comparing `spaces-0.2.0.tar` & `spaces-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.2.0/README.md
--rw-r--r--   0        0        0     1302 2023-06-01 09:07:32.352913 spaces-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-23 16:06:07.578194 spaces-0.2.0/spaces/__init__.py
--rw-r--r--   0        0        0       61 2023-05-23 12:16:01.390521 spaces-0.2.0/spaces/config.py
--rw-r--r--   0        0        0      259 2023-05-30 12:29:38.149333 spaces-0.2.0/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-31 17:56:04.987325 spaces-0.2.0/spaces/gpu/client.py
--rw-r--r--   0        0        0     1107 2023-05-23 15:41:58.726616 spaces-0.2.0/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3579 2023-05-30 13:33:47.192592 spaces-0.2.0/spaces/gpu/torch.py
--rw-r--r--   0        0        0     6528 2023-05-31 15:42:07.658085 spaces-0.2.0/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0     1147 2023-05-29 13:46:54.364944 spaces-0.2.0/spaces/gradio.py
--rw-r--r--   0        0        0     1386 2023-05-30 13:53:53.832283 spaces-0.2.0/spaces/utils.py
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.2.0/setup.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.2.1/README.md
+-rw-r--r--   0        0        0     1426 2023-06-01 10:22:15.138220 spaces-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-23 16:06:07.578194 spaces-0.2.1/spaces/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-23 12:16:01.390521 spaces-0.2.1/spaces/config.py
+-rw-r--r--   0        0        0      259 2023-05-30 12:29:38.149333 spaces-0.2.1/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-31 17:56:04.987325 spaces-0.2.1/spaces/gpu/client.py
+-rw-r--r--   0        0        0     1142 2023-06-01 10:17:22.403085 spaces-0.2.1/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3579 2023-05-30 13:33:47.192592 spaces-0.2.1/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     6528 2023-05-31 15:42:07.658085 spaces-0.2.1/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0     1147 2023-06-01 10:07:38.324798 spaces-0.2.1/spaces/gradio.py
+-rw-r--r--   0        0        0     1386 2023-05-30 13:53:53.832283 spaces-0.2.1/spaces/utils.py
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.2.1/setup.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.2.1/PKG-INFO
```

### Comparing `spaces-0.2.0/pyproject.toml` & `spaces-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spaces"
-version = "0.2.0"
+version = "0.2.1"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
 
@@ -20,14 +20,15 @@
 pytest-dotenv = "^0.5.2"
 pytest-mock = "^3.10.0"
 requests-mock = "^1.10.0"
 pytest-timeout = "^2.1.0"
 poethepoet = "^0.20.0"
 coverage = "^7.2.6"
 pytest-ordering = "^0.6"
+pyright = "^1.1.311"
 
 [tool.poetry.group.test.dependencies]
 diffusers = "^0.16.1"
 transformers = "^4.29.1"
 accelerate = "^0.19.0"
 xformers = "^0.0.19"
 
@@ -37,24 +38,30 @@
 env_files = ["tests/.env"]
 
 [tool.coverage.run]
 source = ["spaces"]
 concurrency = ["thread", "multiprocessing"]
 
 [tool.coverage.report]
+fail_under = 100
 exclude_also = [
     "^\\s*if TYPE_CHECKING:\\s*$",
     "^\\s*\\.\\.\\.\\s*$",
 ]
 
 [tool.poe.tasks.test]
-shell = """
+shell = """set -e
+    pyright
     coverage run -m pytest
     coverage combine -q
     coverage report
     coverage xml
     coverage html
 """
 
+[tool.pyright]
+include = ["spaces", "tests"]
+pythonVersion = "3.9"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `spaces-0.2.0/spaces/gpu/client.py` & `spaces-0.2.1/spaces/gpu/client.py`

 * *Files identical despite different names*

### Comparing `spaces-0.2.0/spaces/gpu/decorator.py` & `spaces-0.2.1/spaces/gpu/decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 """
+from __future__ import annotations
 
 import inspect
 from typing import Callable
 from typing import Generator
 from typing import overload
 
 from .wrappers import _Param
```

### Comparing `spaces-0.2.0/spaces/gpu/torch.py` & `spaces-0.2.1/spaces/gpu/torch.py`

 * *Files identical despite different names*

### Comparing `spaces-0.2.0/spaces/gpu/wrappers.py` & `spaces-0.2.1/spaces/gpu/wrappers.py`

 * *Files identical despite different names*

### Comparing `spaces-0.2.0/spaces/gradio.py` & `spaces-0.2.1/spaces/gradio.py`

 * *Files identical despite different names*

### Comparing `spaces-0.2.0/spaces/utils.py` & `spaces-0.2.1/spaces/utils.py`

 * *Files identical despite different names*

### Comparing `spaces-0.2.0/setup.py` & `spaces-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.2.0/PKG-INFO` & `spaces-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

