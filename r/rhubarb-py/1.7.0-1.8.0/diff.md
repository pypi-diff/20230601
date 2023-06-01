# Comparing `tmp/rhubarb-py-1.7.0.tar.gz` & `tmp/rhubarb_py-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhubarb-py-1.7.0.tar", max compression
+gzip compressed data, was "rhubarb_py-1.8.0.tar", max compression
```

## Comparing `rhubarb-py-1.7.0.tar` & `rhubarb_py-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1079 2021-11-04 23:22:20.209375 rhubarb-py-1.7.0/LICENSE
--rw-r--r--   0        0        0     7269 2022-03-13 16:55:27.443730 rhubarb-py-1.7.0/README.md
--rw-r--r--   0        0        0     3594 2022-08-01 14:44:07.791787 rhubarb-py-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      570 2022-08-01 12:02:35.834589 rhubarb-py-1.7.0/rhubarb/__init__.py
--rw-r--r--   0        0        0    16069 2022-08-01 12:54:45.887676 rhubarb-py-1.7.0/rhubarb/_core.py
--rw-r--r--   0        0        0     3131 2022-08-01 13:50:27.518864 rhubarb-py-1.7.0/rhubarb/backends/base.py
--rw-r--r--   0        0        0       40 2021-11-19 22:48:52.971382 rhubarb-py-1.7.0/rhubarb/backends/exceptions.py
--rw-r--r--   0        0        0     7555 2022-08-01 13:50:47.394799 rhubarb-py-1.7.0/rhubarb/backends/kafka.py
--rw-r--r--   0        0        0     2483 2021-11-28 15:30:00.882623 rhubarb-py-1.7.0/rhubarb/backends/memory.py
--rw-r--r--   0        0        0     3094 2021-11-28 15:31:09.604714 rhubarb-py-1.7.0/rhubarb/backends/postgres.py
--rw-r--r--   0        0        0     4360 2022-08-01 13:51:14.550720 rhubarb-py-1.7.0/rhubarb/backends/rabbitmq.py
--rw-r--r--   0        0        0    13779 2022-08-01 14:42:44.854910 rhubarb-py-1.7.0/rhubarb/backends/redis.py
--rw-r--r--   0        0        0      210 2021-11-04 23:22:44.365494 rhubarb-py-1.7.0/rhubarb/event.py
--rw-r--r--   0        0        0        0 2021-11-04 23:22:20.213375 rhubarb-py-1.7.0/rhubarb/py.typed
--rw-r--r--   0        0        0     8442 2022-08-01 14:48:46.131594 rhubarb-py-1.7.0/setup.py
--rw-r--r--   0        0        0     8455 2022-08-01 14:48:46.132349 rhubarb-py-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-01 14:43:36.441851 rhubarb_py-1.8.0/LICENSE
+-rw-r--r--   0        0        0     7269 2023-06-01 14:43:36.441851 rhubarb_py-1.8.0/README.md
+-rw-r--r--   0        0        0     3651 2023-06-01 16:07:29.866480 rhubarb_py-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      570 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/__init__.py
+-rw-r--r--   0        0        0    16069 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/_core.py
+-rw-r--r--   0        0        0     3131 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/backends/base.py
+-rw-r--r--   0        0        0       40 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/backends/exceptions.py
+-rw-r--r--   0        0        0     7555 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/backends/kafka.py
+-rw-r--r--   0        0        0     2483 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/backends/memory.py
+-rw-r--r--   0        0        0     3094 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/backends/postgres.py
+-rw-r--r--   0        0        0     4360 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/backends/rabbitmq.py
+-rw-r--r--   0        0        0    13779 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/backends/redis.py
+-rw-r--r--   0        0        0      210 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/event.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:43:36.445851 rhubarb_py-1.8.0/rhubarb/py.typed
+-rw-r--r--   0        0        0     8517 1970-01-01 00:00:00.000000 rhubarb_py-1.8.0/PKG-INFO
```

### Comparing `rhubarb-py-1.7.0/LICENSE` & `rhubarb_py-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/README.md` & `rhubarb_py-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/pyproject.toml` & `rhubarb_py-1.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,75 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rhubarb-py"
-packages = [
-    {include = "rhubarb"}
-]
-version = "1.7.0"
+packages = [{ include = "rhubarb" }]
+version = "1.8.0"
 description = "Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API"
 readme = "README.md"
 authors = ["mopeyjellyfish <dev@davidhall.tech>"]
 license = "MIT"
 repository = "https://github.com/mopeyjellyfish/rhubarb"
 homepage = "https://github.com/mopeyjellyfish/rhubarb"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
-keywords = []  #! Update me
+keywords = [] #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
-classifiers = [  #! Update me
+classifiers = [ #! Update me
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
 ]
 
 
-
 [tool.poetry.dependencies]
 python = "^3.9"
 aiokafka = "^0.7.2"
 asyncpg = ">=0.24,<0.27"
 aio-pika = ">=6.8,<9.0"
 anyio = "^3.4.0"
-redis = "4.3.4"
+redis = "^4.3.4"
 
 [tool.poetry.extras]
 redis = ["redis"]
 kafka = ["aiokafka"]
 postgres = ["asyncpg"]
 rabbitmq = ["aio-pika"]
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.4"
-black = {version = "^22.6", allow-prereleases = true}
+black = { version = "^22.6", allow-prereleases = true }
 darglint = "^1.8.0"
-isort = {extras = ["colors"], version = "^5.9.3"}
+isort = { extras = ["colors"], version = "^5.9.3" }
 mypy = "^0.971"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.20.0"
 pydocstyle = "^6.1.1"
 pylint = "^2.14.5"
-pytest = "^6.2.4"
+pytest = "^7.3.1"
 pyupgrade = "^2.37.3"
 safety = "^2.1.1"
 pytest-asyncio = "^0.19.0"
 Sphinx = "^5.1.1"
 sphinx-rtd-theme = "^1.0.0"
 pytest-cov = "^3.0.0"
 asyncpg = ">=0.24,<0.27"
 aiokafka = "^0.7.2"
 aio-pika = ">=6.8,<9.0"
 hypothesis = "^6.53.0"
 
+
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py39"]
 line-length = 88
 color = true
 
 exclude = '''
@@ -91,16 +89,29 @@
 '''
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
 py_version = 39
 line_length = 88
 
-known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
-sections = ["FUTURE", "TYPING", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
+known_typing = [
+  "typing",
+  "types",
+  "typing_extensions",
+  "mypy",
+  "mypy_extensions",
+]
+sections = [
+  "FUTURE",
+  "TYPING",
+  "STDLIB",
+  "THIRDPARTY",
+  "FIRSTPARTY",
+  "LOCALFOLDER",
+]
 include_trailing_comma = true
 profile = "black"
 multi_line_output = 3
 indent = 4
 color_output = true
 
 [tool.mypy]
@@ -126,20 +137,33 @@
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 
-
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
-norecursedirs =["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
-doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
+norecursedirs = [
+  "hooks",
+  "*.egg",
+  ".eggs",
+  "dist",
+  "build",
+  "docs",
+  ".tox",
+  ".git",
+  "__pycache__",
+]
+doctest_optionflags = [
+  "NUMBER",
+  "NORMALIZE_WHITESPACE",
+  "IGNORE_EXCEPTION_DETAIL",
+]
 asyncio_mode = "auto"
 # Extra options:
 addopts = [
   "--strict-markers",
   "--tb=short",
   "--doctest-modules",
   "--doctest-continue-on-failure",
```

### Comparing `rhubarb-py-1.7.0/rhubarb/__init__.py` & `rhubarb_py-1.8.0/rhubarb/__init__.py`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/rhubarb/_core.py` & `rhubarb_py-1.8.0/rhubarb/_core.py`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/rhubarb/backends/base.py` & `rhubarb_py-1.8.0/rhubarb/backends/base.py`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/rhubarb/backends/kafka.py` & `rhubarb_py-1.8.0/rhubarb/backends/kafka.py`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/rhubarb/backends/memory.py` & `rhubarb_py-1.8.0/rhubarb/backends/memory.py`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/rhubarb/backends/postgres.py` & `rhubarb_py-1.8.0/rhubarb/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/rhubarb/backends/rabbitmq.py` & `rhubarb_py-1.8.0/rhubarb/backends/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/rhubarb/backends/redis.py` & `rhubarb_py-1.8.0/rhubarb/backends/redis.py`

 * *Files identical despite different names*

### Comparing `rhubarb-py-1.7.0/setup.py` & `rhubarb_py-1.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,208 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rhubarb-py
+Version: 1.8.0
+Summary: Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API
+Home-page: https://github.com/mopeyjellyfish/rhubarb
+License: MIT
+Author: mopeyjellyfish
+Author-email: dev@davidhall.tech
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: kafka
+Provides-Extra: postgres
+Provides-Extra: rabbitmq
+Provides-Extra: redis
+Requires-Dist: aio-pika (>=6.8,<9.0) ; extra == "rabbitmq"
+Requires-Dist: aiokafka (>=0.7.2,<0.8.0) ; extra == "kafka"
+Requires-Dist: anyio (>=3.4.0,<4.0.0)
+Requires-Dist: asyncpg (>=0.24,<0.27) ; extra == "postgres"
+Requires-Dist: redis (>=4.3.4,<5.0.0) ; extra == "redis"
+Project-URL: Repository, https://github.com/mopeyjellyfish/rhubarb
+Description-Content-Type: text/markdown
+
+# Rhubarb
+
+<div align="center">
+
+[![Build status](https://github.com/mopeyjellyfish/rhubarb/workflows/build/badge.svg?branch=main&event=push)](https://github.com/mopeyjellyfish/rhubarb/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/rhubarb-py.svg)](https://pypi.org/project/rhubarb-py)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/mopeyjellyfish/rhubarb/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+[![codecov](https://codecov.io/gh/mopeyjellyfish/rhubarb/branch/main/graph/badge.svg?token=E8F5LMKDBK)](https://codecov.io/gh/mopeyjellyfish/rhubarb)
+[![Documentation Status](https://readthedocs.org/projects/rhubarb-py/badge/?version=latest)](https://rhubarb-py.readthedocs.io/en/latest/?badge=latest)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/mopeyjellyfish/rhubarb/blob/master/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/mopeyjellyfish/rhubarb/releases)
+[![License](https://img.shields.io/github/license/mopeyjellyfish/rhubarb)](https://github.com/mopeyjellyfish/rhubarb/blob/master/LICENSE)
+
+Rhubarb is a library that simplifies realtime streaming of events for a number of backends in to a single API. Currently supports [`Postgres`](https://github.com/MagicStack/asyncpg), [`kafka`](https://github.com/aio-libs/aiokafka), [`RabbitMQ`](https://github.com/mosquito/aio-pika), [`redis`](https://github.com/aio-libs/aioredis-py) as well as an internal memory backend useful for testing.
+
+</div>
+
+## Installation
+
+There are a number of backends that can be used with Rhubarb:
+
+| Kafka | Postgres | Redis | RabbitMQ |
+| --------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |--------------------------------------------------------------------------------- |
+| <p align="center"><img src="./README_assets/kafka.png" width="60" height="100"/></p>    | <p align="center"><img src="./README_assets/postgres.png" width="100" height="100" /></p> | <p align="center"><img src="./README_assets/redis.png" width="100" height="80"/></p> | <p align="center"><img src="./README_assets/rabbitmq.jpg" width="100" height="100" /></p> |
+| `pip install rhubarb-py[kafka]` | `pip install rhubarb-py[postgres]` | `pip install rhubarb-py[redis]` | `pip install rhubarb-py[rabbitmq]` |
+
+## Backends
+
+- `Rhubarb("redis://localhost:6379/0")`
+- `Rhubarb("kafka://localhost:9092")`
+- `Rhubarb("postgres://postgres:postgres@localhost:5432/rhubarb")`
+- `Rhubarb("amqp://guest:guest@localhost/")`
+- `Rhubarb("memory://")`
+
+## Quick start
+
+### Simple event consumer
+
+```python
+async with Rhubarb("redis://localhost:6379/0") as events:
+    async with events.subscribe(channel="CHATROOM") as subscriber:
+        async for event in subscriber:
+            await websocket.send_text(event.message)
+```
+
+### Simple event producer
+
+```python
+async with Rhubarb("redis://localhost:6379/0") as events:
+    await events.publish("test message")
+```
+
+### History retrieval
+
+```python
+async with Rhubarb("redis://localhost:6379/0") as events: 
+    async with events.subscribe(channel="CHATROOM", history=10) as subscriber: # read the last 10 events published to the channel
+        async for event in subscriber:
+            await websocket.send_text(event.message)
+```
+
+### Custom serializer & deserializer
+
+```python
+async with Rhubarb("redis://localhost:6379/0", serializer=json.dumps, deserializer=json.loads) as events:
+    async with events.subscribe(channel="CHATROOM", history=10) as subscriber: # read the last 10 events published to the channel
+        async for event in subscriber:
+            await websocket.send_text(event.message)
+```
+
+### Group subscribing (at-most-once processing)
+
+```python
+async with Rhubarb("redis://localhost:6379/0", serializer=json.dumps, deserializer=json.loads) as events:
+    async with events.subscribe(
+        "TEST-GROUP-CHANNEL", group_name="TEST_GROUP", consumer_name="sub_1"
+    ) as subscriber_1:
+        async for event in subscriber:
+            await process_job(event)
+```
+
+## Example
+
+A minimal working example can be found in [example](https://github.com/mopeyjellyfish/rhubarb/blob/main/example/app.py) directory.
+
+```python
+import os
+
+from starlette.applications import Starlette
+from starlette.concurrency import run_until_first_complete
+from starlette.responses import HTMLResponse
+from starlette.routing import Route, WebSocketRoute
+
+from rhubarb import Rhubarb
+
+URL = os.environ.get("URL", "redis://localhost:6379/0")
+
+events = Rhubarb(URL)
+
+html = """
+<!DOCTYPE html>
+<html>
+    <head>
+        <title>Chat</title>
+    </head>
+    <body>
+        <h1>WebSocket Chat</h1>
+        <form action="" onsubmit="sendMessage(event)">
+            <input type="text" id="messageText" autocomplete="off"/>
+            <button>Send</button>
+        </form>
+        <ul id='messages'>
+        </ul>
+        <script>
+            var ws = new WebSocket("ws://localhost:8000/ws");
+            ws.onmessage = function(event) {
+                var messages = document.getElementById('messages')
+                var message = document.createElement('li')
+                var content = document.createTextNode(event.data)
+                message.appendChild(content)
+                messages.appendChild(message)
+            };
+            function sendMessage(event) {
+                var input = document.getElementById("messageText")
+                ws.send(input.value)
+                input.value = ''
+                event.preventDefault()
+            }
+        </script>
+    </body>
+</html>
+"""
+
+
+async def homepage(_):
+    return HTMLResponse(html)
+
+
+async def room_consumer(websocket):
+    async for message in websocket.iter_text():
+        await events.publish(channel="chatroom", message=message)
+
+
+async def room_producer(websocket):
+    async with events.subscribe(channel="chatroom") as subscriber:
+        async for event in subscriber:
+            await websocket.send_text(event.message)
+
+
+async def ws(websocket):
+    await websocket.accept()
+    await run_until_first_complete(
+        (room_consumer, {"websocket": websocket}),
+        (room_producer, {"websocket": websocket}),
+    )
+
+
+routes = [
+    Route("/", homepage),
+    WebSocketRoute("/ws", ws, name="chatroom_ws"),
+]
+
+
+app = Starlette(
+    routes=routes,
+    on_startup=[events.connect],
+    on_shutdown=[events.disconnect],
+)
+```
 
-packages = \
-['rhubarb', 'rhubarb.backends']
+## 🛡 License
 
-package_data = \
-{'': ['*']}
+[![License](https://img.shields.io/github/license/mopeyjellyfish/rhubarb)](https://github.com/mopeyjellyfish/rhubarb/blob/master/LICENSE)
 
-install_requires = \
-['anyio>=3.4.0,<4.0.0']
-
-extras_require = \
-{':extra == "kafka"': ['aiokafka>=0.7.2,<0.8.0'],
- ':extra == "postgres"': ['asyncpg>=0.24,<0.27'],
- ':extra == "rabbitmq"': ['aio-pika>=6.8,<9.0'],
- ':extra == "redis"': ['redis==4.3.4']}
-
-setup_kwargs = {
-    'name': 'rhubarb-py',
-    'version': '1.7.0',
-    'description': 'Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API',
-    'long_description': '# Rhubarb\n\n<div align="center">\n\n[![Build status](https://github.com/mopeyjellyfish/rhubarb/workflows/build/badge.svg?branch=main&event=push)](https://github.com/mopeyjellyfish/rhubarb/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/rhubarb-py.svg)](https://pypi.org/project/rhubarb-py)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/mopeyjellyfish/rhubarb/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n[![codecov](https://codecov.io/gh/mopeyjellyfish/rhubarb/branch/main/graph/badge.svg?token=E8F5LMKDBK)](https://codecov.io/gh/mopeyjellyfish/rhubarb)\n[![Documentation Status](https://readthedocs.org/projects/rhubarb-py/badge/?version=latest)](https://rhubarb-py.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/mopeyjellyfish/rhubarb/blob/master/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/mopeyjellyfish/rhubarb/releases)\n[![License](https://img.shields.io/github/license/mopeyjellyfish/rhubarb)](https://github.com/mopeyjellyfish/rhubarb/blob/master/LICENSE)\n\nRhubarb is a library that simplifies realtime streaming of events for a number of backends in to a single API. Currently supports [`Postgres`](https://github.com/MagicStack/asyncpg), [`kafka`](https://github.com/aio-libs/aiokafka), [`RabbitMQ`](https://github.com/mosquito/aio-pika), [`redis`](https://github.com/aio-libs/aioredis-py) as well as an internal memory backend useful for testing.\n\n</div>\n\n## Installation\n\nThere are a number of backends that can be used with Rhubarb:\n\n| Kafka | Postgres | Redis | RabbitMQ |\n| --------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |--------------------------------------------------------------------------------- |\n| <p align="center"><img src="./README_assets/kafka.png" width="60" height="100"/></p>    | <p align="center"><img src="./README_assets/postgres.png" width="100" height="100" /></p> | <p align="center"><img src="./README_assets/redis.png" width="100" height="80"/></p> | <p align="center"><img src="./README_assets/rabbitmq.jpg" width="100" height="100" /></p> |\n| `pip install rhubarb-py[kafka]` | `pip install rhubarb-py[postgres]` | `pip install rhubarb-py[redis]` | `pip install rhubarb-py[rabbitmq]` |\n\n## Backends\n\n- `Rhubarb("redis://localhost:6379/0")`\n- `Rhubarb("kafka://localhost:9092")`\n- `Rhubarb("postgres://postgres:postgres@localhost:5432/rhubarb")`\n- `Rhubarb("amqp://guest:guest@localhost/")`\n- `Rhubarb("memory://")`\n\n## Quick start\n\n### Simple event consumer\n\n```python\nasync with Rhubarb("redis://localhost:6379/0") as events:\n    async with events.subscribe(channel="CHATROOM") as subscriber:\n        async for event in subscriber:\n            await websocket.send_text(event.message)\n```\n\n### Simple event producer\n\n```python\nasync with Rhubarb("redis://localhost:6379/0") as events:\n    await events.publish("test message")\n```\n\n### History retrieval\n\n```python\nasync with Rhubarb("redis://localhost:6379/0") as events: \n    async with events.subscribe(channel="CHATROOM", history=10) as subscriber: # read the last 10 events published to the channel\n        async for event in subscriber:\n            await websocket.send_text(event.message)\n```\n\n### Custom serializer & deserializer\n\n```python\nasync with Rhubarb("redis://localhost:6379/0", serializer=json.dumps, deserializer=json.loads) as events:\n    async with events.subscribe(channel="CHATROOM", history=10) as subscriber: # read the last 10 events published to the channel\n        async for event in subscriber:\n            await websocket.send_text(event.message)\n```\n\n### Group subscribing (at-most-once processing)\n\n```python\nasync with Rhubarb("redis://localhost:6379/0", serializer=json.dumps, deserializer=json.loads) as events:\n    async with events.subscribe(\n        "TEST-GROUP-CHANNEL", group_name="TEST_GROUP", consumer_name="sub_1"\n    ) as subscriber_1:\n        async for event in subscriber:\n            await process_job(event)\n```\n\n## Example\n\nA minimal working example can be found in [example](https://github.com/mopeyjellyfish/rhubarb/blob/main/example/app.py) directory.\n\n```python\nimport os\n\nfrom starlette.applications import Starlette\nfrom starlette.concurrency import run_until_first_complete\nfrom starlette.responses import HTMLResponse\nfrom starlette.routing import Route, WebSocketRoute\n\nfrom rhubarb import Rhubarb\n\nURL = os.environ.get("URL", "redis://localhost:6379/0")\n\nevents = Rhubarb(URL)\n\nhtml = """\n<!DOCTYPE html>\n<html>\n    <head>\n        <title>Chat</title>\n    </head>\n    <body>\n        <h1>WebSocket Chat</h1>\n        <form action="" onsubmit="sendMessage(event)">\n            <input type="text" id="messageText" autocomplete="off"/>\n            <button>Send</button>\n        </form>\n        <ul id=\'messages\'>\n        </ul>\n        <script>\n            var ws = new WebSocket("ws://localhost:8000/ws");\n            ws.onmessage = function(event) {\n                var messages = document.getElementById(\'messages\')\n                var message = document.createElement(\'li\')\n                var content = document.createTextNode(event.data)\n                message.appendChild(content)\n                messages.appendChild(message)\n            };\n            function sendMessage(event) {\n                var input = document.getElementById("messageText")\n                ws.send(input.value)\n                input.value = \'\'\n                event.preventDefault()\n            }\n        </script>\n    </body>\n</html>\n"""\n\n\nasync def homepage(_):\n    return HTMLResponse(html)\n\n\nasync def room_consumer(websocket):\n    async for message in websocket.iter_text():\n        await events.publish(channel="chatroom", message=message)\n\n\nasync def room_producer(websocket):\n    async with events.subscribe(channel="chatroom") as subscriber:\n        async for event in subscriber:\n            await websocket.send_text(event.message)\n\n\nasync def ws(websocket):\n    await websocket.accept()\n    await run_until_first_complete(\n        (room_consumer, {"websocket": websocket}),\n        (room_producer, {"websocket": websocket}),\n    )\n\n\nroutes = [\n    Route("/", homepage),\n    WebSocketRoute("/ws", ws, name="chatroom_ws"),\n]\n\n\napp = Starlette(\n    routes=routes,\n    on_startup=[events.connect],\n    on_shutdown=[events.disconnect],\n)\n```\n\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/mopeyjellyfish/rhubarb)](https://github.com/mopeyjellyfish/rhubarb/blob/master/LICENSE)\n\nThis project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/mopeyjellyfish/rhubarb/blob/master/LICENSE) for more details.\n',
-    'author': 'mopeyjellyfish',
-    'author_email': 'dev@davidhall.tech',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mopeyjellyfish/rhubarb',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
-}
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/mopeyjellyfish/rhubarb/blob/master/LICENSE) for more details.
 
-
-setup(**setup_kwargs)
```

