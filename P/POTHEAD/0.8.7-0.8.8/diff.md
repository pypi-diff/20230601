# Comparing `tmp/POTHEAD-0.8.7.tar.gz` & `tmp/POTHEAD-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "POTHEAD-0.8.7.tar", last modified: Thu May 25 16:40:09 2023, max compression
+gzip compressed data, was "POTHEAD-0.8.8.tar", last modified: Thu Jun  1 08:16:53 2023, max compression
```

## Comparing `POTHEAD-0.8.7.tar` & `POTHEAD-0.8.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-25 16:40:09.137863 POTHEAD-0.8.7/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.7/LICENSE
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-05-25 16:40:09.137863 POTHEAD-0.8.7/PKG-INFO
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-25 16:40:09.133863 POTHEAD-0.8.7/POTHEAD.egg-info/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/PKG-INFO
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/SOURCES.txt
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       76 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/requires.txt
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-05-25 16:40:09.000000 POTHEAD-0.8.7/POTHEAD.egg-info/top_level.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.7/README.md
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-25 16:40:09.137863 POTHEAD-0.8.7/pothead/
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.7/pothead/__init__.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.7/pothead/cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.7/pothead/gating.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8198 2023-05-25 14:08:42.000000 POTHEAD-0.8.7/pothead/oob_response.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.7/pothead/resource_balancer.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.7/pothead/server.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    11308 2023-05-25 14:00:40.000000 POTHEAD-0.8.7/pothead/subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.7/pothead/test_cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.7/pothead/test_resource_balancer.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    14323 2023-05-25 16:38:51.000000 POTHEAD-0.8.7/pothead/test_subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     9156 2023-04-24 20:03:18.000000 POTHEAD-0.8.7/pothead/test_worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1173 2023-02-09 14:53:08.000000 POTHEAD-0.8.7/pothead/util.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    14570 2023-04-24 20:03:05.000000 POTHEAD-0.8.7/pothead/worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.7/pothead/wsgi_typing.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-05-25 16:40:09.137863 POTHEAD-0.8.7/setup.cfg
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      876 2023-05-25 16:39:27.000000 POTHEAD-0.8.7/setup.py
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-01 08:16:53.876469 POTHEAD-0.8.8/
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.8/LICENSE
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-06-01 08:16:53.876469 POTHEAD-0.8.8/PKG-INFO
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-01 08:16:53.872469 POTHEAD-0.8.8/POTHEAD.egg-info/
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/PKG-INFO
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/SOURCES.txt
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       76 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/requires.txt
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/top_level.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.8/README.md
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-01 08:16:53.876469 POTHEAD-0.8.8/pothead/
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.8/pothead/__init__.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.8/pothead/cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.8/pothead/gating.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8196 2023-05-31 15:04:17.000000 POTHEAD-0.8.8/pothead/oob_response.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.8/pothead/resource_balancer.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.8/pothead/server.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    11721 2023-06-01 07:59:46.000000 POTHEAD-0.8.8/pothead/subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.8/pothead/test_cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.8/pothead/test_resource_balancer.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    15931 2023-06-01 07:59:46.000000 POTHEAD-0.8.8/pothead/test_subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    10257 2023-05-31 15:30:55.000000 POTHEAD-0.8.8/pothead/test_worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1173 2023-02-09 14:53:08.000000 POTHEAD-0.8.8/pothead/util.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    17037 2023-06-01 07:59:46.000000 POTHEAD-0.8.8/pothead/worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.8/pothead/wsgi_typing.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-06-01 08:16:53.876469 POTHEAD-0.8.8/setup.cfg
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      876 2023-06-01 08:10:50.000000 POTHEAD-0.8.8/setup.py
```

### Comparing `POTHEAD-0.8.7/LICENSE` & `POTHEAD-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/PKG-INFO` & `POTHEAD-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.7
+Version: 0.8.8
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `POTHEAD-0.8.7/POTHEAD.egg-info/PKG-INFO` & `POTHEAD-0.8.8/POTHEAD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.7
+Version: 0.8.8
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `POTHEAD-0.8.7/POTHEAD.egg-info/SOURCES.txt` & `POTHEAD-0.8.8/POTHEAD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/README.md` & `POTHEAD-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/pothead/cgroups.py` & `POTHEAD-0.8.8/pothead/cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/pothead/gating.py` & `POTHEAD-0.8.8/pothead/gating.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/pothead/oob_response.py` & `POTHEAD-0.8.8/pothead/oob_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def pop(self, key) -> Optional[Any]:
         with self._lock:
             return self._dict.pop(key, (None, None))[1]
 
     def close(self):
         self._shutdown = True
         with self._lock:
-            for (expires_at, job) in self._dict.values():
+            for expires_at, job in self._dict.values():
                 if hasattr(job, "close"):
                     job.close()
             self._dict.clear()
 
     def wait_for_clear(self):
         while True:
             with self._lock:
```

### Comparing `POTHEAD-0.8.7/pothead/resource_balancer.py` & `POTHEAD-0.8.8/pothead/resource_balancer.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/pothead/server.py` & `POTHEAD-0.8.8/pothead/server.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/pothead/subprocess_middleware.py` & `POTHEAD-0.8.8/pothead/subprocess_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     WriteCallable,
     WsgiApplication,
 )
 
 # So that exception tracebacks can be moved across process boundaries
 pickling_support.install()
 
+INTERRUPTIBLE_INTERVAL_S = 0.5
+
 
 class MsgStartResponse(NamedTuple):
     """
     Sent when the wrapped WSGI app has invoked the `start_response` callback.
     """
 
     http_status: str
@@ -93,22 +95,29 @@
 
 
 def do_nothing_warmup():
     pass
 
 
 class SubprocessMiddleware:
-    def __init__(self, logger: Logger, wrapped_app: WsgiApplication):
+    def __init__(
+        self,
+        logger: Logger,
+        wrapped_app: WsgiApplication,
+        *,
+        process_name: str = "WSGI request subprocess",
+    ):
         """
         wrapped_app: WsgiApplication
             The underlying WSGI app, which will have each of its requests called
             in a separate subprocess.
         """
         self.logger = logger
         self.wrapped_app = wrapped_app
+        self.process_name = process_name
 
         # Use a forkserver with the app's module preloaded, to make the
         # spawning of subprocesses for each request faster.
         self.forkserver_context = multiprocessing.get_context("forkserver")
         preload_module_names = [wrapped_app.__module__]
         self.forkserver_context.set_forkserver_preload(preload_module_names)
 
@@ -153,15 +162,15 @@
             args=(self.logger, environ, wsgi_input_writer),
         )
 
         # Setup up the subprocess for running the wrapped WSGI app
         (msg_reader, msg_writer) = self.forkserver_context.Pipe(duplex=False)
         subprocess = self.forkserver_context.Process(
             target=subprocess_main,
-            name="WSGI request subprocess",
+            name=self.process_name,
             args=(
                 self.wrapped_app,
                 new_environ,
                 msg_writer,
                 wsgi_input_reader,
                 reset_cpu_reservation is not None,
             ),
@@ -174,15 +183,20 @@
             # once the subprocess closes its instance, the connection will be
             # completely closed and recv() and similar methods will indicate EOF.
             msg_writer.close()
             wsgi_input_reader.close()
 
             while True:
                 try:
-                    msg = msg_reader.recv()
+                    if msg_reader.poll(INTERRUPTIBLE_INTERVAL_S):
+                        msg = msg_reader.recv()
+                    else:
+                        # Yield an empty chunk, allowing worker.py to abort the request
+                        yield b""
+                        continue
                 except EOFError:
                     # This should not normally happen even if the wrapped app raises
                     # an exception during processing, and likely indicates that the
                     # subprocess died from receiving a signal.
                     raise Exception("Failed to read from WSGI request subprocess!")
 
                 if isinstance(msg, MsgStartResponse):
```

### Comparing `POTHEAD-0.8.7/pothead/test_cgroups.py` & `POTHEAD-0.8.8/pothead/test_cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/pothead/test_resource_balancer.py` & `POTHEAD-0.8.8/pothead/test_resource_balancer.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/pothead/test_subprocess_middleware.py` & `POTHEAD-0.8.8/pothead/test_subprocess_middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 import os
 import subprocess
 from logging import getLogger
-from psutil import Process
+from uuid import uuid4
+from psutil import Process, process_iter
 from threading import Thread
 import pytest
 import signal
 import sys
 import time
 import timeout_decorator
 import traceback
@@ -108,14 +109,18 @@
 
             a_function_in_the_wrapped_app_callstack()
         elif request.path == "/test_wrapped_app_dies_from_signal":
             os.kill(os.getpid(), signal.SIGKILL)
         elif request.path == "/test_globals_not_reinitialized_for_each_request":
             start_response("200 OK", [], None)
             yield f"TEST_GLOBAL_VAR: {TEST_GLOBAL_VAR}".encode("utf-8")
+        elif request.path == "/hang_forever":
+            start_response("200 OK", [], None)
+            while True:
+                time.sleep(60)
         elif request.path in [
             "/test_successful_subprocess_is_shut_down",
             "/test_failing_subprocess_is_shut_down",
         ]:
 
             def sleep_forever():
                 while True:
@@ -350,7 +355,47 @@
                         print(
                             f"Leaked subprocess: {leaked_subprocess} ({leaked_subprocess.cmdline()})"
                         )
                     p.terminate()
 
                 if leaked_subprocess:
                     assert False, f"Subprocess was leaked: {leaked_subprocess}"
+
+    def test_middleware_provides_interruption_points(
+        self,
+    ) -> Optional[Exception]:
+        from . import subprocess_middleware as mw
+
+        orig_INTERRUPTIBLE_INTERVAL_S = mw.INTERRUPTIBLE_INTERVAL_S
+        mw.INTERRUPTIBLE_INTERVAL_S = 0.05
+
+        try:
+            client = Client(SubprocessMiddleware(LOGGER, wrapped_app))
+
+            response = client.post("/hang_forever", data=b"")
+
+            assert response.status == "200 OK"
+            assert (
+                next(response.response) == b""
+            )  # Even though the app is now hung, we expect the middleware to yield empty responses after a timeout
+            assert next(response.response) == b""  # And keep yielding
+        finally:
+            mw.INTERRUPTIBLE_INTERVAL_S = orig_INTERRUPTIBLE_INTERVAL_S
+
+    def test_closed_response_kills_subprocess(
+        self,
+    ) -> Optional[Exception]:
+        worker_name = str(uuid4())
+        client = Client(
+            SubprocessMiddleware(LOGGER, wrapped_app, process_name=worker_name)
+        )
+
+        response = client.post("/hang_forever", data=b"")
+
+        assert response.status == "200 OK"
+        response.response.close()
+
+        for _ in range(10):
+            if not any(filter(lambda p: worker_name in p.name(), process_iter())):
+                return
+            time.sleep(0.1)
+        raise AssertionError("Process left hanging after request-cancellation")
```

### Comparing `POTHEAD-0.8.7/pothead/test_worker.py` & `POTHEAD-0.8.8/pothead/test_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,51 @@
 
 from pothead.gating import wait_for_idle_cpus  # noqa: E402 override environ first
 
 from .util import ObjectProxy  # noqa: E402
 from .worker import LoadBalancer, Server  # noqa: E402
 
 
-def demo_app(environ, start_response):
-    path = environ.get("PATH_INFO")
-    if path == "/":
-        start_response("200 OK", ())
-        yield b"Hello World!"
-    elif path == "/crash":
-        raise Exception("Nope nope nope")
-    elif path == "/slow_loris":
-        sleep(0.05)
-        start_response("200 OK", ())
-        for byte in b"This might take a while...":
-            sleep(0.1)
-            yield byte
-    else:
-        start_response("404 Not Found", ())
+class Flag:
+    def __init__(self) -> None:
+        self.v = False
+
+    def set(self):
+        self.v = True
+
+    def is_set(self) -> bool:
+        return self.v
+
+
+def make_demo_app(is_terminated: Flag):
+    def demo_app(environ, start_response):
+        path = environ.get("PATH_INFO")
+        try:
+            if path == "/":
+                start_response("200 OK", ())
+                yield b"Hello World!"
+            elif path == "/crash":
+                raise Exception("Nope nope nope")
+            elif path == "/slow_loris":
+                sleep(0.05)
+                start_response("200 OK", ())
+                for byte in b"This might take a while...":
+                    sleep(0.1)
+                    yield byte
+            elif path == "/hang_forever":
+                start_response("200 OK", ())
+                while True:
+                    yield b""
+                    sleep(0.01)
+            else:
+                start_response("404 Not Found", ())
+        finally:
+            is_terminated.set()
+
+    return demo_app
 
 
 class WorkerConnection:
     def __init__(self, sock: socket):
         self.sock = sock
 
     def send_request(self, path="/"):
@@ -83,23 +105,21 @@
 
     return MockBalancer
 
 
 class WorkerTest(TestCase):
     def test_load_balancing(self):
         broker_a, broker_b = (DummyBroker() for _ in range(2))
-        app = ObjectProxy(demo_app)
+        app = ObjectProxy(make_demo_app(Flag()))
         app.wait_for_slot = wait_for_idle_cpus(0, max_concurrent=10)
 
         worker = Server(
             ("", 0),
             app,
             load_balancer=mock_balancer(map(DummyBroker.addr, (broker_a, broker_b))),
-            oob_cleanup_interval_seconds=OOB_CLEANUP_INTERVAL_SECONDS,
-            oob_item_expiry_seconds=OOB_ITEM_EXPIRY_SECONDS,
         )
         Thread(target=worker.poll_loop, daemon=True).start()
 
         connection_a = broker_a.accept(0.1)
         connection_b = broker_b.accept(0.1)
 
         assert broker_a.accept(0.2) is None
@@ -107,14 +127,37 @@
 
         connection_b.send_request()
         assert broker_b.accept(0.2) is not None
 
         connection_a.send_request()
         assert broker_a.accept(0.2) is not None
 
+    def test_cancel_hung_request(self):
+        broker = DummyBroker()
+        request_finished = Flag()
+
+        app = ObjectProxy(make_demo_app(request_finished))
+        app.wait_for_slot = wait_for_idle_cpus(0, max_concurrent=10)
+
+        server = Server(
+            ("", 0),
+            app,
+            load_balancer=mock_balancer([broker.addr()]),
+        )
+        Thread(target=server.poll_loop, daemon=True).start()
+        connection = broker.accept(0.1)
+
+        connection.send_request("/hang_forever")
+        sleep(0.1)
+        connection.disconnect()
+
+        sleep(0.1)
+
+        assert request_finished.is_set()
+
 
 class WaitForFirstSlot:
     def __init__(self, callbacks):
         self.counter = 0
         self.callbacks = callbacks
 
     def __call__(self, halt):
@@ -134,15 +177,15 @@
         caplog.set_level(INFO)
         self.caplog = caplog
 
     def setUp(self):
         broker = DummyBroker()
         self.callbacks = MagicMock()
 
-        app = ObjectProxy(demo_app)
+        app = ObjectProxy(make_demo_app(Flag()))
         app.wait_for_slot = WaitForFirstSlot(self.callbacks)
 
         self.server = Server(
             ("", 0),
             app,
             load_balancer=mock_balancer([broker.addr()]),
             redirect_port=0,
```

### Comparing `POTHEAD-0.8.7/pothead/util.py` & `POTHEAD-0.8.8/pothead/util.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/pothead/worker.py` & `POTHEAD-0.8.8/pothead/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 #!/usr/bin/env python3
 
+from errno import EAGAIN
 from http import HTTPStatus
 from logging import getLogger
 from signal import SIGTERM, signal
 from socket import (
     AF_INET,
     IPPROTO_TCP,
+    MSG_DONTWAIT,
+    MSG_PEEK,
     SHUT_RDWR,
     SO_KEEPALIVE,
     SOCK_STREAM,
     SOL_SOCKET,
     TCP_KEEPCNT,
     TCP_KEEPIDLE,
     TCP_KEEPINTVL,
     getaddrinfo,
     socket,
+    error as SocketError,
 )
 from threading import Condition, Thread, Timer
 from time import monotonic, sleep
 from typing import Dict, Optional, Set
 from uuid import uuid4
 from wsgiref import simple_server
 
 from werkzeug.serving import WSGIRequestHandler, BaseWSGIServer, make_server
 
 from .gating import wait_for_idle_cpus
 from .oob_response import OutOfBandResponder
 from .resource_balancer import BoundedResourceBalancer, ResourceLoan
 from .subprocess_middleware import SubprocessMiddleware
 from .util import ObjectProxy, ThreadsTracker
+from .wsgi_typing import (
+    WsgiApplication,
+)
 
 LOGGER = getLogger("pothead.worker")
 BROKER_CONNECT_RETRY_INTERVAL = 2
 
 
 class DeferrableCleanup:
     def __init__(self, f):
@@ -77,23 +84,70 @@
     ):
         self.cb_request_received = cb_request_received
         self.env = None
         self.request_id = None
         self.request_received_at = None
 
         with DeferrableCleanup(cb_processing_done) as c:
-            if isinstance(server.app, OutOfBandResponder):
-                app = server.app
-                server = ObjectProxy(server)
-                server.app = lambda environ, start_response: app(
-                    environ, start_response, c.assume
-                )
+            app = server.app
+            if isinstance(app, OutOfBandResponder):
+                app = self._oob_wrapped_app(app, c.assume)
+
+            app = self._socket_checking_app(app)
 
+            server = ObjectProxy(server)
+            server.app = app
             super().__init__(socket, address, server)
 
+    def _socket_checking_app(self, app) -> WsgiApplication:
+        def application(environ, start_response):
+            response_started = [False]
+
+            def wrapped_start_response(*args, **kwargs):
+                response_started[0] = True
+                return start_response(*args, **kwargs)
+
+            for chunk in app(environ, wrapped_start_response):
+                if len(chunk) == 0:
+                    # Non-empty chunks will fail by themselves when sending to client.
+                    # Empty chunks OTOH, will give us a chance to abort if client is no longer connected
+
+                    try:
+                        if len(self.request.recv(1, MSG_DONTWAIT | MSG_PEEK)) == 0:
+                            # recv() returns empty slice if client shutdown it's writing side
+                            #
+                            # Considering "closed for reading" as a sign of abandoned request is not supported by the
+                            # HTTP specification, (https://datatracker.ietf.org/doc/html/rfc9112#section-9.6).
+                            # However, it _is_ the default behavior of hyper, and we can probably get away with it
+                            # https://docs.rs/hyper/0.14.26/hyper/server/struct.Builder.html#method.http1_half_close
+                            raise ConnectionError(
+                                "Connection closed during response from server"
+                            )
+                    except SocketError as e:
+                        if e.errno != EAGAIN:
+                            raise ConnectionError(
+                                "Connection closed during response from server"
+                            ) from e
+                # By allowing empty chunks to be yielded before `start_response`, we enable early abort. But, werkzeug
+                # doesn't support even empty chunks to be yielded before `start_response` is called, so we suppress
+                # those
+                if not response_started[0] and len(chunk) == 0:
+                    continue
+
+                yield chunk
+
+        return application
+
+    @staticmethod
+    def _oob_wrapped_app(app, assume_cleanup) -> WsgiApplication:
+        def application(environ, start_response):
+            return app(environ, start_response, assume_cleanup)
+
+        return application
+
     def handle_one_request(self):
         try:
             # Handler may be used for several requests, so we must reset
             # environment overrides each time
             self.env = None
             super().handle_one_request()
         finally:
```

### Comparing `POTHEAD-0.8.7/pothead/wsgi_typing.py` & `POTHEAD-0.8.8/pothead/wsgi_typing.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.7/setup.py` & `POTHEAD-0.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 test_deps = ["aiohttp", "werkzeug", "tblib", "timeout-decorator"]
 
 setuptools.setup(
     name="POTHEAD",
-    version="0.8.7",
+    version="0.8.8",
     author="Ulrik Mikaelsson",
     author_email="ulrik.mikaelsson@gmail.com",
     description="A reverse-http proxy implementation for non-concurrent requests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/rawler/pothead",
     packages=setuptools.find_packages(),
```

