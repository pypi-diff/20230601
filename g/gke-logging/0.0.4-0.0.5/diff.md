# Comparing `tmp/gke-logging-0.0.4.tar.gz` & `tmp/gke_logging-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gke-logging-0.0.4.tar", max compression
+gzip compressed data, was "gke_logging-0.0.5.tar", max compression
```

## Comparing `gke-logging-0.0.4.tar` & `gke_logging-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1066 2022-02-01 19:47:43.974189 gke-logging-0.0.4/LICENSE
--rw-r--r--   0        0        0     4960 2022-02-01 19:47:43.974189 gke-logging-0.0.4/README.md
--rw-r--r--   0        0        0       67 2022-02-23 19:30:13.286644 gke-logging-0.0.4/gke_logging/__init__.py
--rw-r--r--   0        0        0     6072 2022-02-23 19:28:11.438155 gke-logging-0.0.4/gke_logging/asgi.py
--rw-r--r--   0        0        0     1837 2022-02-01 19:48:13.102257 gke-logging-0.0.4/gke_logging/context.py
--rw-r--r--   0        0        0        0 2022-02-23 19:19:01.012085 gke-logging-0.0.4/gke_logging/py.typed
--rw-r--r--   0        0        0     2729 2022-02-01 19:47:43.974189 gke-logging-0.0.4/gke_logging/pylogging.py
--rw-r--r--   0        0        0     2977 2022-02-23 19:28:11.438155 gke-logging-0.0.4/gke_logging/types.py
--rw-r--r--   0        0        0      532 2022-02-23 19:30:13.286644 gke-logging-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5886 2022-02-23 19:31:43.472802 gke-logging-0.0.4/setup.py
--rw-r--r--   0        0        0     5646 2022-02-23 19:31:43.473299 gke-logging-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-02-01 01:45:52.712912 gke_logging-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4960 2022-02-01 01:34:06.851115 gke_logging-0.0.5/README.md
+-rw-r--r--   0        0        0       67 2023-05-31 23:18:07.116176 gke_logging-0.0.5/gke_logging/__init__.py
+-rw-r--r--   0        0        0     6072 2023-05-31 23:17:46.439290 gke_logging-0.0.5/gke_logging/asgi.py
+-rw-r--r--   0        0        0     1837 2022-02-08 19:54:43.214704 gke_logging-0.0.5/gke_logging/context.py
+-rw-r--r--   0        0        0        0 2023-05-31 23:17:46.439290 gke_logging-0.0.5/gke_logging/py.typed
+-rw-r--r--   0        0        0     2729 2022-02-01 01:45:52.712912 gke_logging-0.0.5/gke_logging/pylogging.py
+-rw-r--r--   0        0        0     2977 2023-05-31 23:17:46.439290 gke_logging-0.0.5/gke_logging/types.py
+-rw-r--r--   0        0        0      537 2023-05-31 23:18:07.116176 gke_logging-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5694 1970-01-01 00:00:00.000000 gke_logging-0.0.5/PKG-INFO
```

### Comparing `gke-logging-0.0.4/LICENSE` & `gke_logging-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gke-logging-0.0.4/README.md` & `gke_logging-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gke-logging-0.0.4/gke_logging/asgi.py` & `gke_logging-0.0.5/gke_logging/asgi.py`

 * *Files identical despite different names*

### Comparing `gke-logging-0.0.4/gke_logging/context.py` & `gke_logging-0.0.5/gke_logging/context.py`

 * *Files identical despite different names*

### Comparing `gke-logging-0.0.4/gke_logging/pylogging.py` & `gke_logging-0.0.5/gke_logging/pylogging.py`

 * *Files identical despite different names*

### Comparing `gke-logging-0.0.4/gke_logging/types.py` & `gke_logging-0.0.5/gke_logging/types.py`

 * *Files identical despite different names*

### Comparing `gke-logging-0.0.4/pyproject.toml` & `gke_logging-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "gke-logging"
-version = "0.0.4"
+version = "0.0.5"
 description = "Utilities for interacting with logging facilities in GKE workloads"
 readme = "README.md"
 authors = ["Station A <oss@stationa.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = "^1.9.0"
-starlette = {version = "^0.18.0", optional = true}
+starlette = {version = ">=0.18,<0.28", optional = true}
 
 [tool.poetry.extras]
 asgi = ["starlette"]
 
 [tool.poetry.dev-dependencies]
 black = "21.12b0"
 mypy = "^0.931"
```

### Comparing `gke-logging-0.0.4/setup.py` & `gke_logging-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,195 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gke-logging
+Version: 0.0.5
+Summary: Utilities for interacting with logging facilities in GKE workloads
+License: MIT
+Author: Station A
+Author-email: oss@stationa.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: asgi
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: starlette (>=0.18,<0.28) ; extra == "asgi"
+Description-Content-Type: text/markdown
 
-packages = \
-['gke_logging']
+# gke-logging
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/gke-logging.svg)](https://badge.fury.io/py/gke-logging)
 
-install_requires = \
-['pydantic>=1.9.0,<2.0.0']
-
-extras_require = \
-{'asgi': ['starlette>=0.18.0,<0.19.0']}
-
-setup_kwargs = {
-    'name': 'gke-logging',
-    'version': '0.0.4',
-    'description': 'Utilities for interacting with logging facilities in GKE workloads',
-    'long_description': '# gke-logging\n\n[![PyPI version](https://badge.fury.io/py/gke-logging.svg)](https://badge.fury.io/py/gke-logging)\n\nUtilities for interacting with logging facilities in GKE workloads\n\n## Installation\n\n### Requirements\n\n- Python 3.7+\n- [Poetry](https://python-poetry.org/) (for development only)\n\n### Install from PyPI (recommended)\n\n```\npip install gke-logging\n```\n\n### Installing from Github\n\n```\npip install git+https://github.com/StationA/gke-logging.git#egg=gke-logging\n```\n\n### Installing from source\n\n```\ngit clone https://github.com/StationA/gke-logging.git\ncd gke-logging\npoetry install\n```\n\n## Usage\n\n### `gke_logging.GKELoggingFormatter`\n\nOne of the core components is the `GKELoggingFormatter`, which is an implementation of the built-in\n`logging.Formatter` protocol that translates a `logging.LogRecord` into a JSON format that GKE\'s\nlogging infrastructure can understand. At a minimum, this enables any software running on GKE to\nintegrate structured logging simply by applying this formatter for your loggers, e.g.:\n\n```python\nimport logging\n\nfrom gke_logging import GKELoggingFormatter\n\n\nLOGGER = logging.getLogger(__name__)\nh = logging.StreamHandler()\nh.setFormatter(GKELoggingFormatter())\nLOGGER.addHandler(h)\nLOGGER.setLevel(logging.INFO)\n\n\n# ...\n\nLOGGER.info("Look at me! I can haz GKE structured logging!")\n# Prints out: {"time": "2022-01-13T23:22:26.336686+00:00", "severity": "INFO", "message": "Look at me! I can haz GKE structured logging!", "logging.googleapis.com/sourceLocation": {"file": "test_log.py", "line": "14", "function": "<module>"}, "logging.googleapis.com/labels": {}}\n```\n\nFurthermore, this formatter allows you to set app-level metadata to be sent along with each log\nmessage, which is useful in order to better organize collected log data:\n\n```python\n# ...\nh.setFormatter(\n    GKELoggingFormatter(default_labels=dict(app_id="my-cool-app", version="0.1.0"))\n)\n# ...\n```\n\nAlso the formatter also allows you to add HTTP metadata to any logs that occur during the course of\na request. This enhances logs that are emitted during request-handling logic in APIs with additional\ndata. This functionality is primarily utilized in the included `GKELoggingMiddleware` in order to\nprovide basic access logs.\n\n### `gke_logging.asgi.GKELoggingMiddleware`\n\n`gke_logging.asgi.GKELoggingMiddleware` is an ASGI middleware that emits basic access logs in\n"common log format", with a default behavior that integrates with the `GKELoggingFormatter` to write\nthe access logs in a format that GKE\'s logging infrastructure better understands. By implementing\nper the ASGI spec, this means it can work with any ASGI-compatible server, including FastAPI,\nstarlette, and ASGI implementations:\n\n```python\nfrom fastapi import FastAPI\nfrom gke_logging.asgi import GKELoggingMiddleware\n\napp = FastAPI()\napp.add_middleware(GKELoggingMiddleware)\n\n@app.get("/")\ndef get_it() -> str:\n    return "OK"\n```\n\nAdditionally, because this middleware integrates with `gke_logging.context` bindings, it enables any\nlogger used during the course of handling a request to emit logs that also contain request-time\ndata, e.g. request URL, user-agent, response latency, etc.\n\n```python\nimport logging\n\nfrom fastapi import FastAPI\nfrom gke_logging import GKELoggingFormatter\nfrom gke_logging.asgi import GKELoggingMiddleware\n\napp = FastAPI()\napp.add_middleware(GKELoggingMiddleware)\n\n\nroot_logger = logging.getLogger()\nh = logging.StreamHandler()\nh.setFormatter(GKELoggingFormatter())\nroot_logger.setLevel(logging.INFO)\nroot_logger.addHandler(h)\n\n\n@app.get("/")\ndef get_it() -> str:\n    # Any log records created during request-handling will be enriched with other HTTP request data\n    root_logger.info("TEST")\n    return "OK"\n```\n\n### `gke_logging.context`\n\nIn order to control additional metadata labels for log records that correspond to one logical\noperation, e.g. an HTTP request, a batch job operation, etc., you should use the helper functions\nexported in `gke_logging.context`:\n\n```python\nimport logging\n\nfrom contextvars import copy_context\n\nfrom gke_logging import GKELoggingFormatter\nfrom gke_logging.context import set_labels\n\n\nLOGGER = logging.getLogger(__name__)\nh = logging.StreamHandler()\nh.setFormatter(GKELoggingFormatter())\nLOGGER.addHandler(h)\nLOGGER.setLevel(logging.INFO)\n\n# ...\n\n\ndef run_job(job_id: str):\n    set_labels(job_id=job_id)\n    LOGGER.info("TEST")\n\n\nctx = copy_context()\nfor i in range(10):\n    ctx.run(run_job, f"{i + 1}")\n```\n\nBecause `ContextVar`s bind natively to Python\'s `asyncio`, you can use these same helper\nfunctions within asynchronous tasks in a similar fashion.\n\n### Additional examples\n\nAdditional usage examples can be found in [examples/](examples/)\n\n## Contributing\n\nWhen contributing to this repository, please follow the steps below:\n\n1. Fork the repository\n1. Submit your patch in one commit, or a series of well-defined commits\n1. Submit your pull request and make sure you reference the issue you are addressing\n',
-    'author': 'Station A',
-    'author_email': 'oss@stationa.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+Utilities for interacting with logging facilities in GKE workloads
 
+## Installation
+
+### Requirements
+
+- Python 3.7+
+- [Poetry](https://python-poetry.org/) (for development only)
+
+### Install from PyPI (recommended)
+
+```
+pip install gke-logging
+```
+
+### Installing from Github
+
+```
+pip install git+https://github.com/StationA/gke-logging.git#egg=gke-logging
+```
+
+### Installing from source
+
+```
+git clone https://github.com/StationA/gke-logging.git
+cd gke-logging
+poetry install
+```
+
+## Usage
+
+### `gke_logging.GKELoggingFormatter`
+
+One of the core components is the `GKELoggingFormatter`, which is an implementation of the built-in
+`logging.Formatter` protocol that translates a `logging.LogRecord` into a JSON format that GKE's
+logging infrastructure can understand. At a minimum, this enables any software running on GKE to
+integrate structured logging simply by applying this formatter for your loggers, e.g.:
+
+```python
+import logging
+
+from gke_logging import GKELoggingFormatter
+
+
+LOGGER = logging.getLogger(__name__)
+h = logging.StreamHandler()
+h.setFormatter(GKELoggingFormatter())
+LOGGER.addHandler(h)
+LOGGER.setLevel(logging.INFO)
+
+
+# ...
+
+LOGGER.info("Look at me! I can haz GKE structured logging!")
+# Prints out: {"time": "2022-01-13T23:22:26.336686+00:00", "severity": "INFO", "message": "Look at me! I can haz GKE structured logging!", "logging.googleapis.com/sourceLocation": {"file": "test_log.py", "line": "14", "function": "<module>"}, "logging.googleapis.com/labels": {}}
+```
+
+Furthermore, this formatter allows you to set app-level metadata to be sent along with each log
+message, which is useful in order to better organize collected log data:
+
+```python
+# ...
+h.setFormatter(
+    GKELoggingFormatter(default_labels=dict(app_id="my-cool-app", version="0.1.0"))
+)
+# ...
+```
+
+Also the formatter also allows you to add HTTP metadata to any logs that occur during the course of
+a request. This enhances logs that are emitted during request-handling logic in APIs with additional
+data. This functionality is primarily utilized in the included `GKELoggingMiddleware` in order to
+provide basic access logs.
+
+### `gke_logging.asgi.GKELoggingMiddleware`
+
+`gke_logging.asgi.GKELoggingMiddleware` is an ASGI middleware that emits basic access logs in
+"common log format", with a default behavior that integrates with the `GKELoggingFormatter` to write
+the access logs in a format that GKE's logging infrastructure better understands. By implementing
+per the ASGI spec, this means it can work with any ASGI-compatible server, including FastAPI,
+starlette, and ASGI implementations:
+
+```python
+from fastapi import FastAPI
+from gke_logging.asgi import GKELoggingMiddleware
+
+app = FastAPI()
+app.add_middleware(GKELoggingMiddleware)
+
+@app.get("/")
+def get_it() -> str:
+    return "OK"
+```
+
+Additionally, because this middleware integrates with `gke_logging.context` bindings, it enables any
+logger used during the course of handling a request to emit logs that also contain request-time
+data, e.g. request URL, user-agent, response latency, etc.
+
+```python
+import logging
+
+from fastapi import FastAPI
+from gke_logging import GKELoggingFormatter
+from gke_logging.asgi import GKELoggingMiddleware
+
+app = FastAPI()
+app.add_middleware(GKELoggingMiddleware)
+
+
+root_logger = logging.getLogger()
+h = logging.StreamHandler()
+h.setFormatter(GKELoggingFormatter())
+root_logger.setLevel(logging.INFO)
+root_logger.addHandler(h)
+
+
+@app.get("/")
+def get_it() -> str:
+    # Any log records created during request-handling will be enriched with other HTTP request data
+    root_logger.info("TEST")
+    return "OK"
+```
+
+### `gke_logging.context`
+
+In order to control additional metadata labels for log records that correspond to one logical
+operation, e.g. an HTTP request, a batch job operation, etc., you should use the helper functions
+exported in `gke_logging.context`:
+
+```python
+import logging
+
+from contextvars import copy_context
+
+from gke_logging import GKELoggingFormatter
+from gke_logging.context import set_labels
+
+
+LOGGER = logging.getLogger(__name__)
+h = logging.StreamHandler()
+h.setFormatter(GKELoggingFormatter())
+LOGGER.addHandler(h)
+LOGGER.setLevel(logging.INFO)
+
+# ...
+
+
+def run_job(job_id: str):
+    set_labels(job_id=job_id)
+    LOGGER.info("TEST")
+
+
+ctx = copy_context()
+for i in range(10):
+    ctx.run(run_job, f"{i + 1}")
+```
+
+Because `ContextVar`s bind natively to Python's `asyncio`, you can use these same helper
+functions within asynchronous tasks in a similar fashion.
+
+### Additional examples
+
+Additional usage examples can be found in [examples/](examples/)
+
+## Contributing
+
+When contributing to this repository, please follow the steps below:
+
+1. Fork the repository
+1. Submit your patch in one commit, or a series of well-defined commits
+1. Submit your pull request and make sure you reference the issue you are addressing
 
-setup(**setup_kwargs)
```

