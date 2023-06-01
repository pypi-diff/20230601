# Comparing `tmp/tgpy-0.9.4.tar.gz` & `tmp/tgpy-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgpy-0.9.4.tar", max compression
+gzip compressed data, was "tgpy-0.9.5.tar", max compression
```

## Comparing `tgpy-0.9.4.tar` & `tgpy-0.9.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1070 2023-05-05 17:58:56.186671 tgpy-0.9.4/LICENSE
--rw-r--r--   0        0        0     3157 2023-05-05 17:58:56.186671 tgpy-0.9.4/README.md
--rw-r--r--   0        0        0     1282 2023-05-05 17:59:10.999044 tgpy-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      478 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/__init__.py
--rw-r--r--   0        0        0       35 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/__main__.py
--rw-r--r--   0        0        0        0 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/_core/__init__.py
--rw-r--r--   0        0        0     1102 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/_core/eval_message.py
--rw-r--r--   0        0        0     2904 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/_core/message_design.py
--rw-r--r--   0        0        0     5442 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/_core/meval.py
--rw-r--r--   0        0        0      429 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/_core/utils.py
--rw-r--r--   0        0        0     3530 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/_handlers/__init__.py
--rw-r--r--   0        0        0     1192 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/__init__.py
--rw-r--r--   0        0        0     1525 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/config.py
--rw-r--r--   0        0        0      449 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/directories.py
--rw-r--r--   0        0        0     4135 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/parse_code.py
--rw-r--r--   0        0        0      686 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/parse_tgpy_message.py
--rw-r--r--   0        0        0     1829 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/tgpy_eval.py
--rw-r--r--   0        0        0     4516 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/transformers.py
--rw-r--r--   0        0        0     2556 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/utils.py
--rw-r--r--   0        0        0     1542 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/context.py
--rw-r--r--   0        0        0     4880 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/main.py
--rw-r--r--   0        0        0     5251 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/modules.py
--rw-r--r--   0        0        0     1776 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/reactions_fix.py
--rw-r--r--   0        0        0     1198 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/compat.py
--rw-r--r--   0        0        0      221 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/constants.py
--rw-r--r--   0        0        0     2618 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/module_manager.py
--rw-r--r--   0        0        0      364 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/ping.py
--rw-r--r--   0        0        0     1263 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/postfix_await.py
--rw-r--r--   0        0        0     2360 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/prevent_eval.py
--rw-r--r--   0        0        0      915 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/restart.py
--rw-r--r--   0        0        0     1273 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/update.py
--rw-r--r--   0        0        0     2509 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/utils.py
--rw-r--r--   0        0        0       62 2023-05-05 17:59:12.495084 tgpy-0.9.4/tgpy/version.py
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 tgpy-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-01 14:42:24.848581 tgpy-0.9.5/LICENSE
+-rw-r--r--   0        0        0     3157 2023-06-01 14:42:24.848581 tgpy-0.9.5/README.md
+-rw-r--r--   0        0        0     1282 2023-06-01 14:42:37.778778 tgpy-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      478 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/__init__.py
+-rw-r--r--   0        0        0       35 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/_core/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/_core/eval_message.py
+-rw-r--r--   0        0        0     2904 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/_core/message_design.py
+-rw-r--r--   0        0        0     5442 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/_core/meval.py
+-rw-r--r--   0        0        0      429 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/_core/utils.py
+-rw-r--r--   0        0        0     3530 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/_handlers/__init__.py
+-rw-r--r--   0        0        0     1192 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/api/__init__.py
+-rw-r--r--   0        0        0     1525 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/api/config.py
+-rw-r--r--   0        0        0      449 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/api/directories.py
+-rw-r--r--   0        0        0     4135 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/api/parse_code.py
+-rw-r--r--   0        0        0      686 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/api/parse_tgpy_message.py
+-rw-r--r--   0        0        0     1829 2023-06-01 14:42:24.852581 tgpy-0.9.5/tgpy/api/tgpy_eval.py
+-rw-r--r--   0        0        0     4516 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/api/transformers.py
+-rw-r--r--   0        0        0     2556 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/api/utils.py
+-rw-r--r--   0        0        0     1542 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/context.py
+-rw-r--r--   0        0        0     5750 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/main.py
+-rw-r--r--   0        0        0     5251 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/modules.py
+-rw-r--r--   0        0        0     1776 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/reactions_fix.py
+-rw-r--r--   0        0        0     1198 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/std/compat.py
+-rw-r--r--   0        0        0      221 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/std/constants.py
+-rw-r--r--   0        0        0     2618 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/std/module_manager.py
+-rw-r--r--   0        0        0      364 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/std/ping.py
+-rw-r--r--   0        0        0     1263 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/std/postfix_await.py
+-rw-r--r--   0        0        0     2360 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/std/prevent_eval.py
+-rw-r--r--   0        0        0      915 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/std/restart.py
+-rw-r--r--   0        0        0     1273 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/std/update.py
+-rw-r--r--   0        0        0     2509 2023-06-01 14:42:24.856582 tgpy-0.9.5/tgpy/utils.py
+-rw-r--r--   0        0        0       62 2023-06-01 14:42:39.138761 tgpy-0.9.5/tgpy/version.py
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 tgpy-0.9.5/PKG-INFO
```

### Comparing `tgpy-0.9.4/LICENSE` & `tgpy-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/README.md` & `tgpy-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/pyproject.toml` & `tgpy-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgpy"
-version = "0.9.4"
+version = "0.9.5"
 description = "Run Python code right in your Telegram messages"
 authors = ["tmat <a@tmat.me>", "vanutp <hello@vanutp.dev>", "ntonee <a12286@yandex.com>"]
 license = "MIT"
 documentation = "https://tgpy.tmat.me/"
 repository = "https://github.com/tm-a-t/TGPy/"
 readme = "README.md"
 classifiers = [
```

### Comparing `tgpy-0.9.4/tgpy/_core/eval_message.py` & `tgpy-0.9.5/tgpy/_core/eval_message.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/_core/message_design.py` & `tgpy-0.9.5/tgpy/_core/message_design.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/_core/meval.py` & `tgpy-0.9.5/tgpy/_core/meval.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/_handlers/__init__.py` & `tgpy-0.9.5/tgpy/_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/api/__init__.py` & `tgpy-0.9.5/tgpy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/api/config.py` & `tgpy-0.9.5/tgpy/api/config.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/api/parse_code.py` & `tgpy-0.9.5/tgpy/api/parse_code.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/api/parse_tgpy_message.py` & `tgpy-0.9.5/tgpy/api/parse_tgpy_message.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/api/tgpy_eval.py` & `tgpy-0.9.5/tgpy/api/tgpy_eval.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/api/transformers.py` & `tgpy-0.9.5/tgpy/api/transformers.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/api/utils.py` & `tgpy-0.9.5/tgpy/api/utils.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/context.py` & `tgpy-0.9.5/tgpy/context.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/main.py` & `tgpy-0.9.5/tgpy/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import asyncio
 import functools
 import logging
+import os.path
+import platform
+import subprocess
+import sys
 
 import aiorun
 import yaml
 from rich.console import Console, Theme
 from telethon import TelegramClient, errors
 from yaml import YAMLError
 
@@ -26,18 +30,40 @@
 
     return await asyncio.get_event_loop().run_in_executor(
         None, wrapper, prompt, password
     )
 
 
 def create_client():
+    device_model = None
+    if sys.platform == 'linux':
+        if os.path.isfile('/sys/devices/virtual/dmi/id/product_name'):
+            with open('/sys/devices/virtual/dmi/id/product_name') as f:
+                device_model = f.read()
+    elif sys.platform == 'darwin':
+        device_model = (
+            subprocess.check_output('sysctl -n hw.model'.split(' ')).decode().strip()
+        )
+    elif sys.platform == 'win32':
+        device_model = ' '.join(
+            subprocess.check_output('wmic computersystem get manufacturer,model')
+            .decode()
+            .replace('Manufacturer', '')
+            .replace('Model', '')
+            .split()
+        )
+
     client = TelegramClient(
         str(SESSION_FILENAME),
         config.get('core.api_id'),
         config.get('core.api_hash'),
+        device_model=device_model,
+        system_version=platform.platform(),
+        lang_code='en',
+        system_lang_code='en-US',
     )
     client.parse_mode = 'html'
     return client
 
 
 async def start_client():
     await app.client.start(
```

### Comparing `tgpy-0.9.4/tgpy/modules.py` & `tgpy-0.9.5/tgpy/modules.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/reactions_fix.py` & `tgpy-0.9.5/tgpy/reactions_fix.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/std/compat.py` & `tgpy-0.9.5/tgpy/std/compat.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/std/module_manager.py` & `tgpy-0.9.5/tgpy/std/module_manager.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/std/postfix_await.py` & `tgpy-0.9.5/tgpy/std/postfix_await.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/std/prevent_eval.py` & `tgpy-0.9.5/tgpy/std/prevent_eval.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/std/restart.py` & `tgpy-0.9.5/tgpy/std/restart.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/std/update.py` & `tgpy-0.9.5/tgpy/std/update.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/tgpy/utils.py` & `tgpy-0.9.5/tgpy/utils.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.4/PKG-INFO` & `tgpy-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgpy
-Version: 0.9.4
+Version: 0.9.5
 Summary: Run Python code right in your Telegram messages
 Home-page: https://github.com/tm-a-t/TGPy/
 License: MIT
 Author: tmat
 Author-email: a@tmat.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tgpy Version: 0.9.4 Summary: Run Python code right
+Metadata-Version: 2.1 Name: tgpy Version: 0.9.5 Summary: Run Python code right
 in your Telegram messages Home-page: https://github.com/tm-a-t/TGPy/ License:
 MIT Author: tmat Author-email: a@tmat.me Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: PyYAML (>=6.0,<7.0) Requires-Dist: aiorun (>=2022.4.1,<2023.0.0)
```

