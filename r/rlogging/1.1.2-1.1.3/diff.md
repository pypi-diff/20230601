# Comparing `tmp/rlogging-1.1.2.tar.gz` & `tmp/rlogging-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlogging-1.1.2.tar", max compression
+gzip compressed data, was "rlogging-1.1.3.tar", max compression
```

## Comparing `rlogging-1.1.2.tar` & `rlogging-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1393 2023-05-31 06:47:27.811892 rlogging-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      456 2023-05-31 06:47:27.811892 rlogging-1.1.2/readme.md
--rw-r--r--   0        0        0       65 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/__init__.py
--rw-r--r--   0        0        0     3208 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/adapters.py
--rw-r--r--   0        0        0      270 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/filters.py
--rw-r--r--   0        0        0     2339 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/formatters.py
--rw-r--r--   0        0        0      945 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/handlers.py
--rw-r--r--   0        0        0        0 2023-05-31 06:47:27.951892 rlogging-1.1.2/rlogging/integration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:47:27.959892 rlogging-1.1.2/rlogging/integration/aiogram/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:47:27.959892 rlogging-1.1.2/rlogging/integration/django/__init__.py
--rw-r--r--   0        0        0      740 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/adapters.py
--rw-r--r--   0        0        0      125 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/admin.py
--rw-r--r--   0        0        0      271 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/apps.py
--rw-r--r--   0        0        0        0 2023-05-31 06:47:27.959892 rlogging-1.1.2/rlogging/integration/django/handlers.py
--rw-r--r--   0        0        0     1483 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/middleware.py
--rw-r--r--   0        0        0       72 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/models.py
--rw-r--r--   0        0        0     2019 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/signals.py
--rw-r--r--   0        0        0        0 2023-05-31 06:47:27.959892 rlogging-1.1.2/rlogging/integration/fastapi/__init__.py
--rw-r--r--   0        0        0       50 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/namespaces.py
--rw-r--r--   0        0        0     1509 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/utils.py
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 rlogging-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1399 2023-06-01 21:18:35.680770 rlogging-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1465 2023-06-01 21:18:35.680770 rlogging-1.1.3/readme.md
+-rw-r--r--   0        0        0       78 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/__init__.py
+-rw-r--r--   0        0        0     3176 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/adapters.py
+-rw-r--r--   0        0        0      125 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/filters.py
+-rw-r--r--   0        0        0     2150 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/formatters.py
+-rw-r--r--   0        0        0      990 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:22:58.427494 rlogging-1.1.3/rlogging/integration/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:22:58.431494 rlogging-1.1.3/rlogging/integration/aiogram/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:22:58.431494 rlogging-1.1.3/rlogging/integration/django/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/integration/django/adapters.py
+-rw-r--r--   0        0        0      125 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/integration/django/admin.py
+-rw-r--r--   0        0        0      215 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/integration/django/apps.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:22:58.431494 rlogging-1.1.3/rlogging/integration/django/handlers.py
+-rw-r--r--   0        0        0     1483 2023-06-01 21:18:35.680770 rlogging-1.1.3/rlogging/integration/django/middleware.py
+-rw-r--r--   0        0        0       72 2023-06-01 21:18:35.684770 rlogging-1.1.3/rlogging/integration/django/models.py
+-rw-r--r--   0        0        0     2019 2023-06-01 21:18:35.684770 rlogging-1.1.3/rlogging/integration/django/signals.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:22:58.431494 rlogging-1.1.3/rlogging/integration/fastapi/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-01 21:18:35.684770 rlogging-1.1.3/rlogging/namespaces.py
+-rw-r--r--   0        0        0     1542 2023-06-01 21:18:35.684770 rlogging-1.1.3/rlogging/utils.py
+-rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 rlogging-1.1.3/PKG-INFO
```

### Comparing `rlogging-1.1.2/pyproject.toml` & `rlogging-1.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -15,35 +15,37 @@
 repository = "https://gitlab.com/rocshers/python/rlogging"
 source = "https://gitlab.com/rocshers/python/rlogging.git"
 documentation = "https://gitlab.com/rocshers/python/rlogging/-/blob/release/readme.md"
 changelog = "https://gitlab.com/rocshers/python/rlogging/-/releases"
 issues = "https://gitlab.com/rocshers/python/rlogging/-/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
-django = "^4.1.7"
-black = "^23.1.0"
-ruff = "^0.0.257"
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+ruff = "^0.0.260"
+black = "^23.3.0"
 isort = "^5.12.0"
+pre-commit = "^3.2.2"
+mypy = "^1.2.0"
+django = "^4.1.7"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 120
 
 [tool.isort]
 profile = "black"
 line_length = 120
 
 [tool.ruff]
-# select = ["A", "B", "C", "D", "E", "F", "I", "UP"]
 select = ["A", "B", "C", "E", "F", "I", "UP"]
-# fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
-fixable = ["A"]
+fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
 ignore = ["UP004", "D100", "D101", "D102", "D103", "D104", "D107", "D400", "D415"]
 line-length = 120
 target-version = "py37"
 
 [tool.ruff.mccabe]
 max-complexity = 10
```

### Comparing `rlogging-1.1.2/rlogging/adapters.py` & `rlogging-1.1.3/rlogging/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import inspect
 import logging
 import sys
 import uuid
-from inspect import FrameInfo
 from types import FrameType
 from typing import Any
 
 
-class RsLoggerAdapter(logging.LoggerAdapter):
+class RLoggerAdapter(logging.LoggerAdapter):
     """Путь логирования
 
     Создание логов, через флоу позволяет обоготить их
 
     """
 
     flow_id: uuid.UUID
@@ -53,15 +52,15 @@
 
         if extra := self.get_class_info():
             self._extra_update(kwargs, extra)
 
         return msg, kwargs
 
 
-class AppLoggerAdapter(RsLoggerAdapter):
+class AppLoggerAdapter(RLoggerAdapter):
     def queries(self, queries: list, *args, **kwargs):
         kwargs.setdefault('stacklevel', 4)
         self.info(f'processing queries: {len(queries)}', **kwargs)
 
 
 class HttpLoggerAdapter(AppLoggerAdapter):
     """Флоу для логирования веб запросов/ответов"""
```

### Comparing `rlogging-1.1.2/rlogging/formatters.py` & `rlogging-1.1.3/rlogging/formatters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 import json
 import logging
 
 from rlogging import utils
 
 
-class RsFormatter(logging.Formatter):
+class RFormatter(logging.Formatter):
     """Кастомный форматер модуля"""
 
-    def enrichment(self, record: logging.LogRecord):
-        pass
 
-    def format(self, record: logging.LogRecord):
-        return super().format(record)
-
-
-class JsonFormatter(RsFormatter):
+class JsonFormatter(RFormatter):
     """Форматер в json"""
 
     DEFAULT_EXCLUDE_FIELDS = {
         'msecs',
         'relativeCreated',
         'filename',
         'exc_info',
@@ -58,15 +52,14 @@
 
         if self.exclude_fields:
             return {k: v for k, v in record_data.items() if k not in self.exclude_fields}
 
         return record_data
 
     def format(self, record: logging.LogRecord):
-        self.enrichment(record)
         record_data = self.get_data_from_record(record)
         return self.json_serializer(record_data, default=self.json_default, cls=self.json_cls)
 
 
 class ElkFormatter(JsonFormatter):
     def get_data_from_record(self, record: logging.LogRecord) -> dict:
         return utils.flatten_dict(super().get_data_from_record(record))
```

### Comparing `rlogging-1.1.2/rlogging/handlers.py` & `rlogging-1.1.3/rlogging/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import time
 from logging import FileHandler
 
 
 class DailyFileHandler(FileHandler):
+    """why not TimedRotatingFileHandler?"""
+
     DATE_FORMAT = '%Y-%m-%d'
 
     _origin_filename__name: str
     _origin_filename__ext: str
 
     def __init__(self, filename, *args, **kwargs):
         root, ext = os.path.splitext(os.path.abspath(os.fspath(filename)))
```

### Comparing `rlogging-1.1.2/rlogging/integration/django/adapters.py` & `rlogging-1.1.3/rlogging/integration/django/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.core.handlers.wsgi import WSGIRequest
-from django.http import HttpRequest, HttpResponse
+from django.http import HttpResponse
 
 from rlogging import HttpLoggerAdapter
 
 
 class DjangoLoggerAdapter(HttpLoggerAdapter):
     def request(self, request: WSGIRequest, *args, **kwargs):
         kwargs.setdefault('stacklevel', 5)
```

### Comparing `rlogging-1.1.2/rlogging/integration/django/middleware.py` & `rlogging-1.1.3/rlogging/integration/django/middleware.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.2/rlogging/integration/django/signals.py` & `rlogging-1.1.3/rlogging/integration/django/signals.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.2/rlogging/utils.py` & `rlogging-1.1.3/rlogging/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 
     if isinstance(obj, (datetime.date, datetime.time, datetime.datetime)):
         return obj.isoformat()
 
     if isinstance(obj, uuid.UUID):
         return str(obj)
 
+    if isinstance(obj, BaseException):
+        return ''.join(traceback.format_exception(obj)).strip()
+
     if isinstance(obj, types.TracebackType):
         return ''.join(traceback.format_tb(obj)).strip()
 
-    if isinstance(obj, Exception):
-        return f'Exception: {obj}'
-
     return str(obj)
 
 
 def flatten_dict(dict_data: dict, parent_key: str = '', sep: str = '.'):
     """
     Рекурсивно преобразует вложенный словарь в одномерный словарь
     с объединенными ключами разных уровней через точку.
     """
 
     items = []
     for k, v in dict_data.items():
-        new_key = f"{parent_key}{sep}{k}" if parent_key else k
+        new_key = f'{parent_key}{sep}{k}' if parent_key else k
         if isinstance(v, dict):
             items.extend(flatten_dict(v, new_key, sep=sep).items())
         else:
             items.append((new_key, v))
     return dict(items)
```

