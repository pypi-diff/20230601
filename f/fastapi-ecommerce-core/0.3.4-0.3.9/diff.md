# Comparing `tmp/fastapi_ecommerce_core-0.3.4.tar.gz` & `tmp/fastapi_ecommerce_core-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_core-0.3.4.tar", last modified: Wed May 24 16:13:45 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_core-0.3.9.tar", last modified: Thu Jun  1 19:40:30 2023, max compression
```

## Comparing `fastapi_ecommerce_core-0.3.4.tar` & `fastapi_ecommerce_core-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 16:13:45.142780 fastapi_ecommerce_core-0.3.4/
--rw-rw-rw-   0        0        0     1077 2023-05-01 04:19:18.000000 fastapi_ecommerce_core-0.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0      331 2023-05-24 16:13:45.142780 fastapi_ecommerce_core-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      479 2023-05-24 15:32:56.000000 fastapi_ecommerce_core-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 16:13:45.132637 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core/
-drwxrwxrwx   0        0        0        0 2023-05-24 16:13:45.142780 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core/logger/
--rw-rw-rw-   0        0        0        0 2023-05-01 04:19:18.000000 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core/logger/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-05-22 21:06:05.000000 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core/logger/configure.py
--rw-rw-rw-   0        0        0     2651 2023-05-22 21:06:05.000000 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:13:45.142780 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core.egg-info/
--rw-rw-rw-   0        0        0      331 2023-05-24 16:13:45.000000 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-24 16:13:45.000000 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 16:13:45.000000 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-24 16:13:45.000000 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-24 16:13:45.000000 fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-24 16:13:45.142780 fastapi_ecommerce_core-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-05-24 16:11:00.000000 fastapi_ecommerce_core-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:40:30.144057 fastapi_ecommerce_core-0.3.9/
+-rw-rw-rw-   0        0        0     1061 2023-06-01 11:52:40.000000 fastapi_ecommerce_core-0.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      331 2023-06-01 19:40:30.144057 fastapi_ecommerce_core-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-01 11:52:40.000000 fastapi_ecommerce_core-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 19:40:30.112406 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core/
+drwxrwxrwx   0        0        0        0 2023-06-01 19:40:30.144057 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core/logger/
+-rw-rw-rw-   0        0        0        0 2023-06-01 11:52:40.000000 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core/logger/__init__.py
+-rw-rw-rw-   0        0        0     1462 2023-06-01 11:52:40.000000 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core/logger/configure.py
+-rw-rw-rw-   0        0        0     2583 2023-06-01 11:52:40.000000 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:40:30.139541 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core.egg-info/
+-rw-rw-rw-   0        0        0      331 2023-06-01 19:40:30.000000 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-06-01 19:40:30.000000 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:40:30.000000 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-01 19:40:30.000000 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-01 19:40:30.000000 fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-01 19:40:30.144057 fastapi_ecommerce_core-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-06-01 19:40:28.000000 fastapi_ecommerce_core-0.3.9/setup.py
```

### Comparing `fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core/logger/configure.py` & `fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core/logger/configure.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import logging
-import sys
-
-from loguru import logger
-
-
-class InterceptHandler(logging.Handler):
-    def emit(self, record: logging.LogRecord):
-        try:
-            level = logger.level(record.levelname).name
-        except ValueError:
-            level = record.levelno
-        frame, depth = logging.currentframe(), 2
-        while frame.f_code.co_filename == logging.__file__:
-            frame = frame.f_back
-            depth += 1
-        logger.opt(depth=depth, exception=record.exc_info).log(
-            level, record.getMessage()
-        )
-
-
-def configure_logging(logging_level: int, access_log_path: str) -> None:
-    loggers = [
-        logging.getLogger(name)
-        for name in logging.root.manager.loggerDict
-        if name.startswith("uvicorn") or name.startswith("gunicorn")
-    ]
-    for lg in loggers:
-        lg.handlers = []
-    intercept_handler = InterceptHandler()
-    logging.getLogger("uvicorn").handlers = [intercept_handler]
-    logging.getLogger("gunicorn").handlers = [intercept_handler]
-    logger.configure(
-        handlers=[
-            {
-                "sink": sys.stdout,
-                "level": logging_level,
-            },
-        ],
-    )
-    logger.add(
-        access_log_path,
-        serialize=True,
-        level=logging_level,
-        enqueue=True,
-        backtrace=True,
-        diagnose=True,
-        encoding="UTF-8",
-        rotation="256 MB",
-        retention="7 days",
-        compression="zip",
-    )
+import logging
+import sys
+
+from loguru import logger
+
+
+class InterceptHandler(logging.Handler):
+    def emit(self, record: logging.LogRecord):
+        try:
+            level = logger.level(record.levelname).name
+        except ValueError:
+            level = record.levelno
+        frame, depth = logging.currentframe(), 2
+        while frame.f_code.co_filename == logging.__file__:
+            frame = frame.f_back
+            depth += 1
+        logger.opt(depth=depth, exception=record.exc_info).log(
+            level, record.getMessage()
+        )
+
+
+def configure_logging(logging_level: int, access_log_path: str) -> None:
+    loggers = [
+        logging.getLogger(name)
+        for name in logging.root.manager.loggerDict
+        if name.startswith("uvicorn") or name.startswith("gunicorn")
+    ]
+    for lg in loggers:
+        lg.handlers = []
+    intercept_handler = InterceptHandler()
+    logging.getLogger("uvicorn").handlers = [intercept_handler]
+    logging.getLogger("gunicorn").handlers = [intercept_handler]
+    logger.configure(
+        handlers=[
+            {
+                "sink": sys.stdout,
+                "level": logging_level,
+            },
+        ],
+    )
+    logger.add(
+        access_log_path,
+        serialize=True,
+        level=logging_level,
+        enqueue=True,
+        backtrace=True,
+        diagnose=True,
+        encoding="UTF-8",
+        rotation="256 MB",
+        retention="7 days",
+        compression="zip",
+    )
```

### Comparing `fastapi_ecommerce_core-0.3.4/fastapi_ecommerce_core/logger/middleware.py` & `fastapi_ecommerce_core-0.3.9/fastapi_ecommerce_core/logger/middleware.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import json
-import time
-from typing import Callable
-
-from loguru import logger
-from starlette import status
-from starlette.concurrency import iterate_in_threadpool
-from starlette.middleware.base import StreamingResponse
-from starlette.requests import Request
-from starlette.responses import Response, JSONResponse
-from starlette.routing import Match
-
-
-class LoguruLoggingMiddleware:
-    async def __call__(self, request: Request, call_next: Callable):
-        try:
-            await self.log_before_response(request)
-            st = time.time()
-            response = await call_next(request)
-            elapsed = f"{time.time() - st:0.10f} sec"
-            response.headers.append("X-Response-Time", elapsed)
-        except Exception as e:
-            response = JSONResponse(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-                content={"detail": f"{e.__class__.__name__} - {e.args}"},
-                media_type="application/json",
-            )
-            if request.app.debug:
-                logger.exception(e)
-                return await self.log_after_response(request, response)
-        return response
-
-    @staticmethod
-    def log_format(request: Request):
-        return f"{request.client.host}:{request.client.port} - {request.method} {request.url}"
-
-    async def log_before_response(self, request: Request):
-        msg = (
-            f"{request.client.host}:{request.client.port} - "
-            f"{request.method} {request.url}"
-        )
-        if request.app.debug:
-            headers = []
-            for route in request.app.router.routes:
-                match, scope = route.matches(request)
-                if match == Match.FULL:
-                    for name, value in scope["path_params"].items():
-                        headers.append(f"{name}: {value}")
-            if len(headers) > 0:
-                logger.info(f"- Params: {headers}")
-        logger.info(self.log_format(request))
-        return request
-
-    @staticmethod
-    async def log_after_response(
-        request: Request, response: Response | StreamingResponse
-    ):
-        msg = "response to prev request: "
-        if isinstance(response, StreamingResponse):
-            response_body = [
-                section async for section in response.body_iterator
-            ]
-            response.body_iterator = iterate_in_threadpool(iter(response_body))
-            msg += f"{response_body[0].decode()}"
-        elif isinstance(response, Response):
-            msg += f"{json.loads(response.body)}"
-        logger.info(msg)
-        return response
+import json
+import time
+from typing import Callable
+
+from loguru import logger
+from starlette import status
+from starlette.concurrency import iterate_in_threadpool
+from starlette.middleware.base import StreamingResponse
+from starlette.requests import Request
+from starlette.responses import Response, JSONResponse
+from starlette.routing import Match
+
+
+class LoguruLoggingMiddleware:
+    async def __call__(self, request: Request, call_next: Callable):
+        try:
+            await self.log_before_response(request)
+            st = time.time()
+            response = await call_next(request)
+            elapsed = f"{time.time() - st:0.10f} sec"
+            response.headers.append("X-Response-Time", elapsed)
+        except Exception as e:
+            response = JSONResponse(
+                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+                content={"detail": f"{e.__class__.__name__} - {e.args}"},
+                media_type="application/json",
+            )
+            if request.app.debug:
+                logger.exception(e)
+                return await self.log_after_response(request, response)
+        return response
+
+    @staticmethod
+    def log_format(request: Request):
+        return f"{request.client.host}:{request.client.port} - {request.method} {request.url}"
+
+    async def log_before_response(self, request: Request):
+        msg = (
+            f"{request.client.host}:{request.client.port} - "
+            f"{request.method} {request.url}"
+        )
+        if request.app.debug:
+            headers = []
+            for route in request.app.router.routes:
+                match, scope = route.matches(request)
+                if match == Match.FULL:
+                    for name, value in scope["path_params"].items():
+                        headers.append(f"{name}: {value}")
+            if len(headers) > 0:
+                logger.info(f"- Params: {headers}")
+        logger.info(self.log_format(request))
+        return request
+
+    @staticmethod
+    async def log_after_response(
+        request: Request, response: Response | StreamingResponse
+    ):
+        msg = "response to prev request: "
+        if isinstance(response, StreamingResponse):
+            response_body = [
+                section async for section in response.body_iterator
+            ]
+            response.body_iterator = iterate_in_threadpool(iter(response_body))
+            msg += f"{response_body[0].decode()}"
+        elif isinstance(response, Response):
+            msg += f"{json.loads(response.body)}"
+        logger.info(msg)
+        return response
```

