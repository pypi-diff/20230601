# Comparing `tmp/concurrent_tasks-1.4.1.tar.gz` & `tmp/concurrent_tasks-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concurrent_tasks-1.4.1.tar", max compression
+gzip compressed data, was "concurrent_tasks-1.5.0.tar", max compression
```

## Comparing `concurrent_tasks-1.4.1.tar` & `concurrent_tasks-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-03-10 20:36:05.994155 concurrent_tasks-1.4.1/LICENSE
--rw-r--r--   0        0        0     4616 2023-03-10 20:36:05.994155 concurrent_tasks-1.4.1/README.md
--rw-r--r--   0        0        0      399 2023-03-10 20:36:05.994155 concurrent_tasks-1.4.1/concurrent_tasks/__init__.py
--rw-r--r--   0        0        0     1458 2023-03-10 20:36:05.994155 concurrent_tasks-1.4.1/concurrent_tasks/background.py
--rw-r--r--   0        0        0        0 2023-03-10 20:36:05.994155 concurrent_tasks-1.4.1/concurrent_tasks/py.typed
--rw-r--r--   0        0        0     3097 2023-03-10 20:36:05.994155 concurrent_tasks-1.4.1/concurrent_tasks/restartable.py
--rw-r--r--   0        0        0     4208 2023-03-10 20:36:05.994155 concurrent_tasks-1.4.1/concurrent_tasks/thread_safe_pool.py
--rw-r--r--   0        0        0      228 2023-03-10 20:36:05.998155 concurrent_tasks-1.4.1/concurrent_tasks/threaded_pool/__init__.py
--rw-r--r--   0        0        0     1587 2023-03-10 20:36:05.998155 concurrent_tasks-1.4.1/concurrent_tasks/threaded_pool/aio.py
--rw-r--r--   0        0        0     4527 2023-03-10 20:36:05.998155 concurrent_tasks-1.4.1/concurrent_tasks/threaded_pool/base.py
--rw-r--r--   0        0        0     1529 2023-03-10 20:36:05.998155 concurrent_tasks-1.4.1/concurrent_tasks/threaded_pool/blocking.py
--rw-r--r--   0        0        0      913 2023-03-10 20:36:05.998155 concurrent_tasks-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 concurrent_tasks-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4616 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/README.md
+-rw-r--r--   0        0        0      399 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/__init__.py
+-rw-r--r--   0        0        0     1458 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/background.py
+-rw-r--r--   0        0        0        0 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/py.typed
+-rw-r--r--   0        0        0     3097 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/restartable.py
+-rw-r--r--   0        0        0     4208 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/thread_safe_pool.py
+-rw-r--r--   0        0        0      228 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/threaded_pool/__init__.py
+-rw-r--r--   0        0        0     1696 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/threaded_pool/aio.py
+-rw-r--r--   0        0        0     4655 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/threaded_pool/base.py
+-rw-r--r--   0        0        0     1638 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/concurrent_tasks/threaded_pool/blocking.py
+-rw-r--r--   0        0        0      914 2023-06-01 07:52:01.936349 concurrent_tasks-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 concurrent_tasks-1.5.0/PKG-INFO
```

### Comparing `concurrent_tasks-1.4.1/LICENSE` & `concurrent_tasks-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.4.1/README.md` & `concurrent_tasks-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.4.1/concurrent_tasks/background.py` & `concurrent_tasks-1.5.0/concurrent_tasks/background.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.4.1/concurrent_tasks/restartable.py` & `concurrent_tasks-1.5.0/concurrent_tasks/restartable.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.4.1/concurrent_tasks/thread_safe_pool.py` & `concurrent_tasks-1.5.0/concurrent_tasks/thread_safe_pool.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.4.1/concurrent_tasks/threaded_pool/aio.py` & `concurrent_tasks-1.5.0/concurrent_tasks/threaded_pool/aio.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,23 @@
 
     def __init__(
         self,
         name: Optional[str] = None,
         size: int = 0,
         timeout: Optional[float] = None,
         context_manager: Optional[Union[ContextManager, AsyncContextManager]] = None,
+        daemon: bool = False,
     ):
-        self._base = BaseThreadedTaskPool(name, size, timeout, context_manager)
+        self._base = BaseThreadedTaskPool(
+            name,
+            size,
+            timeout,
+            context_manager,
+            daemon,
+        )
 
     async def __aenter__(self) -> "AsyncThreadedTaskPool":
         self._base.start()
         await asyncio.wrap_future(self._base.post_start())
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
```

### Comparing `concurrent_tasks-1.4.1/concurrent_tasks/threaded_pool/base.py` & `concurrent_tasks-1.5.0/concurrent_tasks/threaded_pool/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,40 +24,46 @@
 
     def __init__(
         self,
         name: Optional[str] = None,
         size: int = 0,
         timeout: Optional[float] = None,
         context_manager: Optional[Union[ContextManager, AsyncContextManager]] = None,
+        daemon: bool = False,
     ):
         self._name = name
 
         self._size = size
         self._timeout = timeout
         self._pool: Optional[ThreadSafeTaskPool] = None
 
         # Context managers.
         self._stack = AsyncExitStack()
         self._context_manager = context_manager
 
         self._thread: Optional[threading.Thread] = None
+        self._daemon = daemon
         # Create an event loop for that thread.
         self._loop: Optional[asyncio.AbstractEventLoop] = None
         # Set when the event loop is running.
         # Cleared when stopping to prevent receiving new tasks.
         self._initialized = threading.Event()
 
     def start(self) -> None:
         """Start the thread and wait for the loop to start running."""
         if self._thread is not None:
             raise RuntimeError(
                 f"{self.__class__.__name__}({self._name}) is already running"
             )
         self._loop = asyncio.new_event_loop()
-        self._thread = threading.Thread(name=self._name, target=self._run_thread)
+        self._thread = threading.Thread(
+            name=self._name,
+            target=self._run_thread,
+            daemon=self._daemon,
+        )
         self._thread.start()
         self._initialized.wait()
 
     async def _post_start(self) -> None:
         """Enter context managers in this tread's event loop."""
         if self._context_manager:
             try:
```

### Comparing `concurrent_tasks-1.4.1/concurrent_tasks/threaded_pool/blocking.py` & `concurrent_tasks-1.5.0/concurrent_tasks/threaded_pool/blocking.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,23 @@
 
     def __init__(
         self,
         name: Optional[str] = None,
         size: int = 0,
         timeout: Optional[float] = None,
         context_manager: Optional[Union[ContextManager, AsyncContextManager]] = None,
+        daemon: bool = False,
     ):
-        self._base = BaseThreadedTaskPool(name, size, timeout, context_manager)
+        self._base = BaseThreadedTaskPool(
+            name,
+            size,
+            timeout,
+            context_manager,
+            daemon,
+        )
 
     def __enter__(self) -> "BlockingThreadedTaskPool":
         self._base.start()
         self._base.post_start().result()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
```

### Comparing `concurrent_tasks-1.4.1/pyproject.toml` & `concurrent_tasks-1.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "concurrent_tasks"
-version = "1.4.1"
+version = "1.5.0"
 description = "Tools to run asyncio tasks concurrently."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/asyncio-concurrent-tasks"
 include = ["concurrent_tasks/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
 [tool.poetry.group.test.dependencies]
-pytest = "==7.2.2"
-pytest-asyncio = "==0.20.3"
+pytest = "==7.3.1"
+pytest-asyncio = "==0.21.0"
 pytest-mock = "==3.10.0"
-ruff = "==0.0.254"
-mypy = "==1.1.1"
-black = "==23.1.0"
-pre-commit = "==3.1.1"
+ruff = "==0.0.265"
+mypy = "==1.2.0"
+black = "==23.3.0"
+pre-commit = "==3.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
@@ -32,9 +32,10 @@
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.ruff]
 select = ["A", "B", "E", "F", "I", "PT"]
 ignore = ["E501"]
+
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `concurrent_tasks-1.4.1/PKG-INFO` & `concurrent_tasks-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concurrent-tasks
-Version: 1.4.1
+Version: 1.5.0
 Summary: Tools to run asyncio tasks concurrently.
 Home-page: https://github.com/gpajot/asyncio-concurrent-tasks
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

