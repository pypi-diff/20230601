# Comparing `tmp/httpx-sse-0.3.0.tar.gz` & `tmp/httpx-sse-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx-sse-0.3.0.tar", last modified: Thu Apr 27 20:24:20 2023, max compression
+gzip compressed data, was "httpx-sse-0.3.1.tar", last modified: Thu Jun  1 20:25:25 2023, max compression
```

## Comparing `httpx-sse-0.3.0.tar` & `httpx-sse-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      142 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (123)      883 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/CHANGELOG.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1072 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      565 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/Makefile
--rw-r--r--   0 vsts      (1001) docker     (123)     8500 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6829 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.640906 httpx-sse-0.3.0/ci/
--rw-r--r--   0 vsts      (1001) docker     (123)      893 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/ci/azure-pipelines.yml
--rw-r--r--   0 vsts      (1001) docker     (123)     1025 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      204 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      320 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.640906 httpx-sse-0.3.0/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/src/httpx_sse/
--rw-r--r--   0 vsts      (1001) docker     (123)      282 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2157 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1748 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/_decoders.py
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/src/httpx_sse.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     8500 2023-04-27 20:24:20.000000 httpx-sse-0.3.0/src/httpx_sse.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      564 2023-04-27 20:24:20.000000 httpx-sse-0.3.0/src/httpx_sse.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-27 20:24:20.000000 httpx-sse-0.3.0/src/httpx_sse.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-27 20:24:20.000000 httpx-sse-0.3.0/src/httpx_sse.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2383 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1280 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_asgi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6687 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_event_source.py
--rw-r--r--   0 vsts      (1001) docker     (123)      131 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_models.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 20:25:25.037266 httpx-sse-0.3.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      142 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/CHANGELOG.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1072 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      486 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (123)     8641 2023-06-01 20:25:25.037266 httpx-sse-0.3.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     6829 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 20:25:25.033266 httpx-sse-0.3.1/ci/
+-rw-r--r--   0 vsts      (1001) docker     (123)      893 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/ci/azure-pipelines.yml
+-rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      184 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-01 20:25:25.037266 httpx-sse-0.3.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 20:25:25.033266 httpx-sse-0.3.1/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 20:25:25.033266 httpx-sse-0.3.1/src/httpx_sse/
+-rw-r--r--   0 vsts      (1001) docker     (123)      282 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/src/httpx_sse/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2157 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/src/httpx_sse/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1748 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/src/httpx_sse/_decoders.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/src/httpx_sse/_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1221 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/src/httpx_sse/_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/src/httpx_sse/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 20:25:25.037266 httpx-sse-0.3.1/src/httpx_sse.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8641 2023-06-01 20:25:25.000000 httpx-sse-0.3.1/src/httpx_sse.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      564 2023-06-01 20:25:25.000000 httpx-sse-0.3.1/src/httpx_sse.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-01 20:25:25.000000 httpx-sse-0.3.1/src/httpx_sse.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-06-01 20:25:25.000000 httpx-sse-0.3.1/src/httpx_sse.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 20:25:25.037266 httpx-sse-0.3.1/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2383 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/tests/test_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1280 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/tests/test_asgi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6687 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/tests/test_event_source.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      131 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      838 2023-06-01 20:24:47.000000 httpx-sse-0.3.1/tests/test_models.py
```

### Comparing `httpx-sse-0.3.0/CHANGELOG.md` & `httpx-sse-0.3.1/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## 0.3.1 - 2023-06-01
+
+### Added
+
+* Add `__repr__()` for `ServerSentEvent` model, which may help with debugging and other tasks. (Pull #16)
+
 ## 0.3.0 - 2023-04-27
 
 ### Changed
 
 * Raising an `SSEError` if the response content type is not `text/event-stream` is now performed as part of `iter_sse()` / `aiter_sse()`, instead of `connect_sse()` / `aconnect_sse()`. This allows inspecting the response before iterating on server-sent events, such as checking for error responses. (Pull #12)
 
 ## 0.2.0 - 2023-03-27
```

### Comparing `httpx-sse-0.3.0/LICENSE` & `httpx-sse-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/PKG-INFO` & `httpx-sse-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-sse
-Version: 0.3.0
+Version: 0.3.1
 Summary: Consume Server-Sent Event (SSE) messages with HTTPX.
 Author-email: Florimond Manca <florimond.manca@protonmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/florimondmanca/httpx-sse
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -276,14 +276,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## 0.3.1 - 2023-06-01
+
+### Added
+
+* Add `__repr__()` for `ServerSentEvent` model, which may help with debugging and other tasks. (Pull #16)
+
 ## 0.3.0 - 2023-04-27
 
 ### Changed
 
 * Raising an `SSEError` if the response content type is not `text/event-stream` is now performed as part of `iter_sse()` / `aiter_sse()`, instead of `connect_sse()` / `aconnect_sse()`. This allows inspecting the response before iterating on server-sent events, such as checking for error responses. (Pull #12)
 
 ## 0.2.0 - 2023-03-27
```

### Comparing `httpx-sse-0.3.0/README.md` & `httpx-sse-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/ci/azure-pipelines.yml` & `httpx-sse-0.3.1/ci/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/pyproject.toml` & `httpx-sse-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -26,7 +26,12 @@
 
 [project.urls]
 "Homepage" = "https://github.com/florimondmanca/httpx-sse"
 
 [tool.setuptools.dynamic]
 version = { attr = "httpx_sse.__version__" }
 readme = { file = ["README.md", "CHANGELOG.md"], content-type = "text/markdown" }
+
+[tool.ruff]
+select = ["E", "F", "I"]
+line-length = 88
+src = ["src"]
```

### Comparing `httpx-sse-0.3.0/src/httpx_sse/_api.py` & `httpx-sse-0.3.1/src/httpx_sse/_api.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/src/httpx_sse/_decoders.py` & `httpx-sse-0.3.1/src/httpx_sse/_decoders.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/src/httpx_sse.egg-info/PKG-INFO` & `httpx-sse-0.3.1/src/httpx_sse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-sse
-Version: 0.3.0
+Version: 0.3.1
 Summary: Consume Server-Sent Event (SSE) messages with HTTPX.
 Author-email: Florimond Manca <florimond.manca@protonmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/florimondmanca/httpx-sse
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -276,14 +276,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## 0.3.1 - 2023-06-01
+
+### Added
+
+* Add `__repr__()` for `ServerSentEvent` model, which may help with debugging and other tasks. (Pull #16)
+
 ## 0.3.0 - 2023-04-27
 
 ### Changed
 
 * Raising an `SSEError` if the response content type is not `text/event-stream` is now performed as part of `iter_sse()` / `aiter_sse()`, instead of `connect_sse()` / `aconnect_sse()`. This allows inspecting the response before iterating on server-sent events, such as checking for error responses. (Pull #12)
 
 ## 0.2.0 - 2023-03-27
```

### Comparing `httpx-sse-0.3.0/src/httpx_sse.egg-info/SOURCES.txt` & `httpx-sse-0.3.1/src/httpx_sse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/tests/test_api.py` & `httpx-sse-0.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/tests/test_asgi.py` & `httpx-sse-0.3.1/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/tests/test_event_source.py` & `httpx-sse-0.3.1/tests/test_event_source.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.3.0/tests/test_models.py` & `httpx-sse-0.3.1/tests/test_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,7 +21,15 @@
         sse.json()
 
     sse = ServerSentEvent(data='{"key": "value"}')
     assert sse.json() == {"key": "value"}
 
     sse = ServerSentEvent(data='["item1", "item2"]')
     assert sse.json() == ["item1", "item2"]
+
+
+def test_sse_repr() -> None:
+    sse = ServerSentEvent()
+    assert repr(sse) == "ServerSentEvent(event='message')"
+
+    sse = ServerSentEvent(data="data", retry=3, id="id", event="event")
+    assert repr(sse) == "ServerSentEvent(event='event', data='data', id='id', retry=3)"
```

