# Comparing `tmp/fastapi_views-0.0.4.tar.gz` & `tmp/fastapi_views-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_views-0.0.4.tar", max compression
+gzip compressed data, was "fastapi_views-0.0.5.tar", max compression
```

## Comparing `fastapi_views-0.0.4.tar` & `fastapi_views-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-05-22 09:02:02.788504 fastapi_views-0.0.4/LICENSE
--rw-r--r--   0        0        0     2159 2023-05-22 09:02:02.788504 fastapi_views-0.0.4/README.md
--rw-r--r--   0        0        0      760 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/__init__.py
--rw-r--r--   0        0        0       22 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/_version.py
--rw-r--r--   0        0        0     1320 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/config.py
--rw-r--r--   0        0        0     1421 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/enum.py
--rw-r--r--   0        0        0      479 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/__init__.py
--rw-r--r--   0        0        0      449 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/exceptions.py
--rw-r--r--   0        0        0     1238 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/handlers.py
--rw-r--r--   0        0        0     1811 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/models.py
--rw-r--r--   0        0        0      986 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/utils.py
--rw-r--r--   0        0        0     2001 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/healthcheck.py
--rw-r--r--   0        0        0     1795 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/models.py
--rw-r--r--   0        0        0      331 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/openapi.py
--rw-r--r--   0        0        0      663 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/prometheus.py
--rw-r--r--   0        0        0        0 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/py.typed
--rw-r--r--   0        0        0      413 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/response.py
--rw-r--r--   0        0        0     1338 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/routers.py
--rw-r--r--   0        0        0     2051 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/settings.py
--rw-r--r--   0        0        0     1121 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/types.py
--rw-r--r--   0        0        0      881 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/utils.py
--rw-r--r--   0        0        0      263 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/__init__.py
--rw-r--r--   0        0        0    18045 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/api.py
--rw-r--r--   0        0        0     2126 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/functools.py
--rw-r--r--   0        0        0    13755 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/generics.py
--rw-r--r--   0        0        0     1837 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/mixins.py
--rw-r--r--   0        0        0     4355 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/viewsets.py
--rw-r--r--   0        0        0     1629 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 fastapi_views-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2159 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/README.md
+-rw-r--r--   0        0        0      760 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/_version.py
+-rw-r--r--   0        0        0     1577 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/config.py
+-rw-r--r--   0        0        0     1421 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/enum.py
+-rw-r--r--   0        0        0      479 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/errors/__init__.py
+-rw-r--r--   0        0        0      449 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/errors/exceptions.py
+-rw-r--r--   0        0        0     1238 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/errors/handlers.py
+-rw-r--r--   0        0        0     1811 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/errors/models.py
+-rw-r--r--   0        0        0      986 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/errors/utils.py
+-rw-r--r--   0        0        0     2001 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/healthcheck.py
+-rw-r--r--   0        0        0     1795 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/models.py
+-rw-r--r--   0        0        0      331 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/openapi.py
+-rw-r--r--   0        0        0      663 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/prometheus.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/py.typed
+-rw-r--r--   0        0        0      413 2023-06-01 10:06:26.006691 fastapi_views-0.0.5/fastapi_views/response.py
+-rw-r--r--   0        0        0     1338 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/routers.py
+-rw-r--r--   0        0        0     2051 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/settings.py
+-rw-r--r--   0        0        0     1121 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/types.py
+-rw-r--r--   0        0        0      881 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/utils.py
+-rw-r--r--   0        0        0      263 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/views/__init__.py
+-rw-r--r--   0        0        0    18045 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/views/api.py
+-rw-r--r--   0        0        0     2126 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/views/functools.py
+-rw-r--r--   0        0        0    13755 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/views/generics.py
+-rw-r--r--   0        0        0     1837 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/views/mixins.py
+-rw-r--r--   0        0        0     4355 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/fastapi_views/views/viewsets.py
+-rw-r--r--   0        0        0     1786 2023-06-01 10:06:26.010691 fastapi_views-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 fastapi_views-0.0.5/PKG-INFO
```

### Comparing `fastapi_views-0.0.4/LICENSE` & `fastapi_views-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/README.md` & `fastapi_views-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ![Mypy](https://img.shields.io/badge/mypy-checked-blue)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 *FastAPI Class Views and utilities*
 
 ---
-Version: 0.0.4
+Version: 0.0.5
 
 Documentation: https://performancemedia.github.io/fastapi-views/
 
 Repository: https://github.com/performancemedia/fastapi-views
 
 ---
```

### Comparing `fastapi_views-0.0.4/fastapi_views/__init__.py` & `fastapi_views-0.0.5/fastapi_views/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/config.py` & `fastapi_views-0.0.5/fastapi_views/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,28 @@
 
 from .errors import ServiceUnavailableAPIError, add_error_handlers
 from .healthcheck import HealthCheck
 from .openapi import simplify_operation_ids
 from .prometheus import add_prometheus_middleware
 from .settings import APISettings
 
+try:
+    from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
+
+except ImportError:
+    FastAPIInstrumentor = None
+
 
 def configure_app(
     app: FastAPI,
     enable_error_handlers: bool = True,
     healthcheck: HealthCheck | None = None,
     enable_prometheus_middleware: bool = True,
     simplify_openapi_ids: bool = True,
+    **tracing_opts,
 ):
     if enable_error_handlers:
         add_error_handlers(app)
     if healthcheck:
         app.add_api_route(
             methods=["GET"],
             path=healthcheck.endpoint,
@@ -27,14 +34,17 @@
             responses={503: {"model": ServiceUnavailableAPIError}},
         )
     if enable_prometheus_middleware:
         add_prometheus_middleware(app)
     if simplify_openapi_ids:
         simplify_operation_ids(app)
 
+    if FastAPIInstrumentor is not None:
+        FastAPIInstrumentor.instrument_app(app, **tracing_opts)
+
 
 def create_fastapi_app(settings: APISettings, **kwargs) -> FastAPI:
     app = FastAPI(**settings.fastapi_kwargs, **kwargs)
     configure_app(app, **settings.config_kwargs)
     return app
```

### Comparing `fastapi_views-0.0.4/fastapi_views/enum.py` & `fastapi_views-0.0.5/fastapi_views/enum.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/errors/handlers.py` & `fastapi_views-0.0.5/fastapi_views/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/errors/models.py` & `fastapi_views-0.0.5/fastapi_views/errors/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/errors/utils.py` & `fastapi_views-0.0.5/fastapi_views/errors/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/healthcheck.py` & `fastapi_views-0.0.5/fastapi_views/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/models.py` & `fastapi_views-0.0.5/fastapi_views/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/prometheus.py` & `fastapi_views-0.0.5/fastapi_views/prometheus.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/routers.py` & `fastapi_views-0.0.5/fastapi_views/routers.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/settings.py` & `fastapi_views-0.0.5/fastapi_views/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/types.py` & `fastapi_views-0.0.5/fastapi_views/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/utils.py` & `fastapi_views-0.0.5/fastapi_views/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/views/api.py` & `fastapi_views-0.0.5/fastapi_views/views/api.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/views/functools.py` & `fastapi_views-0.0.5/fastapi_views/views/functools.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/views/generics.py` & `fastapi_views-0.0.5/fastapi_views/views/generics.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/views/mixins.py` & `fastapi_views-0.0.5/fastapi_views/views/mixins.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/fastapi_views/views/viewsets.py` & `fastapi_views-0.0.5/fastapi_views/views/viewsets.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.4/pyproject.toml` & `fastapi_views-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "fastapi-views"
-version = "0.0.4"
+version = "0.0.5"
 description = "FastAPI Class Views and utilities"
 authors = ["Radzim Kowalow <radzim.kowalow@performance-media.pl>"]
 readme = "README.md"
 packages = [{include = "fastapi_views"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 fastapi = "^0.95.0"
 orjson = ">=3.2.1,<=3.8.9"
 uvicorn = "^0.22.0"
 uvloop = "^0.17.0"
 starlette-exporter = "^0.16"
+opentelemetry-instrumentation-fastapi = {version = "^0.39b0", optional = true}
 
-
+[tool.poetry.extras]
+opentelemetry = ["opentelemetry-instrumentation-fastapi"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.2"
 pytest-cov = "^4.0.0"
 black = "^22.3.0"
 flake8 = "^6.0.0"
```

### Comparing `fastapi_views-0.0.4/PKG-INFO` & `fastapi_views-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: fastapi-views
-Version: 0.0.4
+Version: 0.0.5
 Summary: FastAPI Class Views and utilities
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: opentelemetry
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.39b0,<0.40) ; extra == "opentelemetry"
 Requires-Dist: orjson (>=3.2.1,<=3.8.9)
 Requires-Dist: starlette-exporter (>=0.16,<0.17)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Description-Content-Type: text/markdown
 
 # fastapi-views
@@ -27,15 +29,15 @@
 ![Mypy](https://img.shields.io/badge/mypy-checked-blue)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 *FastAPI Class Views and utilities*
 
 ---
-Version: 0.0.4
+Version: 0.0.5
 
 Documentation: https://performancemedia.github.io/fastapi-views/
 
 Repository: https://github.com/performancemedia/fastapi-views
 
 ---
```

