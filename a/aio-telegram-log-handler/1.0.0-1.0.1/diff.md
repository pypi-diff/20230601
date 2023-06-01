# Comparing `tmp/aio_telegram_log_handler-1.0.0.tar.gz` & `tmp/aio_telegram_log_handler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_telegram_log_handler-1.0.0.tar", last modified: Sun May 28 11:57:23 2023, max compression
+gzip compressed data, was "aio_telegram_log_handler-1.0.1.tar", last modified: Thu Jun  1 20:39:34 2023, max compression
```

## Comparing `aio_telegram_log_handler-1.0.0.tar` & `aio_telegram_log_handler-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:23.692004 aio_telegram_log_handler-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:23.688004 aio_telegram_log_handler-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:23.688004 aio_telegram_log_handler-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/.github/workflows/github-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-28 11:57:23.692004 aio_telegram_log_handler-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:23.688004 aio_telegram_log_handler-1.0.0/aio_telegram_log_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-28 11:57:23.000000 aio_telegram_log_handler-1.0.0/aio_telegram_log_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-28 11:57:23.000000 aio_telegram_log_handler-1.0.0/aio_telegram_log_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:57:23.000000 aio_telegram_log_handler-1.0.0/aio_telegram_log_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-28 11:57:23.000000 aio_telegram_log_handler-1.0.0/aio_telegram_log_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 11:57:23.000000 aio_telegram_log_handler-1.0.0/aio_telegram_log_handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:23.688004 aio_telegram_log_handler-1.0.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/example/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 11:57:23.692004 aio_telegram_log_handler-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:23.688004 aio_telegram_log_handler-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/tests/tghandler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:57:23.692004 aio_telegram_log_handler-1.0.0/tghandler/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/tghandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-28 11:57:15.000000 aio_telegram_log_handler-1.0.0/tghandler/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:34.360954 aio_telegram_log_handler-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:34.356954 aio_telegram_log_handler-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:34.356954 aio_telegram_log_handler-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/.github/workflows/github-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-01 20:39:34.360954 aio_telegram_log_handler-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:34.356954 aio_telegram_log_handler-1.0.1/aio_telegram_log_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-01 20:39:34.000000 aio_telegram_log_handler-1.0.1/aio_telegram_log_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-01 20:39:34.000000 aio_telegram_log_handler-1.0.1/aio_telegram_log_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:39:34.000000 aio_telegram_log_handler-1.0.1/aio_telegram_log_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 20:39:34.000000 aio_telegram_log_handler-1.0.1/aio_telegram_log_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 20:39:34.000000 aio_telegram_log_handler-1.0.1/aio_telegram_log_handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:34.356954 aio_telegram_log_handler-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/docs/ci-docs.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:34.356954 aio_telegram_log_handler-1.0.1/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/example/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:39:34.360954 aio_telegram_log_handler-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:34.356954 aio_telegram_log_handler-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/tests/tghandler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:34.356954 aio_telegram_log_handler-1.0.1/tghandler/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/tghandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-01 20:39:26.000000 aio_telegram_log_handler-1.0.1/tghandler/handler.py
```

### Comparing `aio_telegram_log_handler-1.0.0/.github/workflows/github-ci.yml` & `aio_telegram_log_handler-1.0.1/.github/workflows/github-ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Checks
 
 on: [push]
 
 jobs:
-  build:
+  test:
 
     runs-on: ubuntu-latest
     strategy:
 
       matrix:
         python-version: ["3.9", "3.10", "3.11"]
 
@@ -22,11 +22,46 @@
         run: |
           python -c "import sys; print(sys.version)"
           ls
       - name: Install dependencies
         run: | 
           python -m pip install --upgrade pip
           pip install -e .[test]
+          pip install -e .[linters]
       - name: Running tests
         run: |
           make test
-          
+      - name: Isort
+        run: |
+          isort tghandler --check-only
+      - name: Mypy
+        run: |
+          mypy tghandler/
+      - name: Black
+        run: |
+          black tghandler/ --check
+
+  build:
+
+    runs-on: ubuntu-latest
+
+    steps:
+      - uses: actions/checkout@v3
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.11"
+
+      - name: Display version
+        run: |
+          python -c "import sys; print(sys.version)"
+      - name: Install depends
+        run: python3 -m pip install --upgrade build
+      - name: Build archive
+        run: |
+          mkdir -p artefacts
+          python3 -m build --outdir artefacts/  
+      - uses: actions/Upload-artifact@v3
+        with:
+          name: archive
+          path: artefacts/*.gz
+
```

### Comparing `aio_telegram_log_handler-1.0.0/PKG-INFO` & `aio_telegram_log_handler-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aio_telegram_log_handler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for send some important logs directly to telegram
 Author: Daniil Solynin
 Author-email: Daniil Solynin <solynynd@gmail.com>
 Keywords: telegram,logging,async
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: linters
 
 # Aio-telegram-log
 
 Basic library for sending log to telegram, using python logging module(like handler), but do it asynchronously.
 
 ## Usage
```

### Comparing `aio_telegram_log_handler-1.0.0/README.md` & `aio_telegram_log_handler-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aio_telegram_log_handler-1.0.0/aio_telegram_log_handler.egg-info/PKG-INFO` & `aio_telegram_log_handler-1.0.1/aio_telegram_log_handler.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aio-telegram-log-handler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for send some important logs directly to telegram
 Author: Daniil Solynin
 Author-email: Daniil Solynin <solynynd@gmail.com>
 Keywords: telegram,logging,async
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: linters
 
 # Aio-telegram-log
 
 Basic library for sending log to telegram, using python logging module(like handler), but do it asynchronously.
 
 ## Usage
```

### Comparing `aio_telegram_log_handler-1.0.0/example/main.py` & `aio_telegram_log_handler-1.0.1/example/main.py`

 * *Files identical despite different names*

### Comparing `aio_telegram_log_handler-1.0.0/pyproject.toml` & `aio_telegram_log_handler-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version="1.0.0"
+version="1.0.1"
 name = "aio_telegram_log_handler"
 authors = [
     {name = "Daniil Solynin", email = "solynynd@gmail.com"},
 ]
 description = "Package for send some important logs directly to telegram"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -24,11 +24,22 @@
 
 [project.optional-dependencies]
 test = [
     "pytest>=7",
     "pytest-asyncio>=0.21"
 ]
 
+linters = [
+    "isort",
+    "mypy",
+    "black"
+]
+
+
 [tool.pytest.ini_options]
 minversion="7.0"
 testpaths=["tests"]
-asyncio_mode="auto"
+asyncio_mode="auto"
+
+[[tool.mypy.overrides]]
+module="aiohttp.*"
+ignore_missing_imports = true
```

### Comparing `aio_telegram_log_handler-1.0.0/tests/tghandler_test.py` & `aio_telegram_log_handler-1.0.1/tests/tghandler_test.py`

 * *Files identical despite different names*

### Comparing `aio_telegram_log_handler-1.0.0/tghandler/handler.py` & `aio_telegram_log_handler-1.0.1/tghandler/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import datetime
 import logging
-from typing import Optional, Final
+from typing import Final, Optional, Union
 
 import aiohttp
 
 logger = logging.getLogger(__name__)
 
 
 class TelegramLoggingHandler(logging.Handler):
@@ -47,15 +47,15 @@
 
         await asyncio.gather(*[send(ch_id) for ch_id in self._chat_ids])
 
     async def set_session(self):
         self.session = aiohttp.ClientSession()
 
     def get_message_sender(self, text: str):
-        message = {"text": text}
+        message: dict[str, Union[str, int]] = {"text": text}
 
         async def sender(chat_id: int):
             if self.session is None:
                 logger.warning("can not send logs to telegram because session is None")
 
             message["chat_id"] = chat_id
             try:
@@ -64,11 +64,13 @@
                 logger.warning(f"can not send message to telegram: {e}")
                 return
             return response
 
         return sender
 
     async def send2telegram(self, message: dict):
+        if self.session is None:
+            return None
         async with self.session.post(
             self.format_url("sendMessage"), json=message
         ) as resp:
             return resp
```

