# Comparing `tmp/rlogging-1.1.4.tar.gz` & `tmp/rlogging-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlogging-1.1.4.tar", max compression
+gzip compressed data, was "rlogging-1.1.5.tar", max compression
```

## Comparing `rlogging-1.1.4.tar` & `rlogging-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1399 2023-06-01 21:18:55.176675 rlogging-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1465 2023-06-01 21:18:55.176675 rlogging-1.1.4/readme.md
--rw-r--r--   0        0        0       78 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/__init__.py
--rw-r--r--   0        0        0     3176 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/adapters.py
--rw-r--r--   0        0        0      125 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/filters.py
--rw-r--r--   0        0        0     2150 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/formatters.py
--rw-r--r--   0        0        0      990 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/handlers.py
--rw-r--r--   0        0        0        0 2023-06-01 21:29:41.201532 rlogging-1.1.4/rlogging/integration/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 21:29:41.201532 rlogging-1.1.4/rlogging/integration/aiogram/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 21:29:41.201532 rlogging-1.1.4/rlogging/integration/django/__init__.py
--rw-r--r--   0        0        0      727 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/integration/django/adapters.py
--rw-r--r--   0        0        0      125 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/integration/django/admin.py
--rw-r--r--   0        0        0      215 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/integration/django/apps.py
--rw-r--r--   0        0        0        0 2023-06-01 21:29:41.201532 rlogging-1.1.4/rlogging/integration/django/handlers.py
--rw-r--r--   0        0        0     1483 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/integration/django/middleware.py
--rw-r--r--   0        0        0       72 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/integration/django/models.py
--rw-r--r--   0        0        0     2019 2023-06-01 21:18:55.176675 rlogging-1.1.4/rlogging/integration/django/signals.py
--rw-r--r--   0        0        0        0 2023-06-01 21:29:41.201532 rlogging-1.1.4/rlogging/integration/fastapi/__init__.py
--rw-r--r--   0        0        0       50 2023-06-01 21:18:55.184675 rlogging-1.1.4/rlogging/namespaces.py
--rw-r--r--   0        0        0     1542 2023-06-01 21:18:55.184675 rlogging-1.1.4/rlogging/utils.py
--rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 rlogging-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1399 2023-06-01 21:18:55.176675 rlogging-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1465 2023-06-01 21:18:55.176675 rlogging-1.1.5/readme.md
+-rw-r--r--   0        0        0       78 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/__init__.py
+-rw-r--r--   0        0        0     3176 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/adapters.py
+-rw-r--r--   0        0        0      125 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/filters.py
+-rw-r--r--   0        0        0     2150 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/formatters.py
+-rw-r--r--   0        0        0      990 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/aiogram/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/django/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/adapters.py
+-rw-r--r--   0        0        0      125 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/admin.py
+-rw-r--r--   0        0        0      215 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/apps.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/django/handlers.py
+-rw-r--r--   0        0        0     1483 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/middleware.py
+-rw-r--r--   0        0        0       72 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/models.py
+-rw-r--r--   0        0        0     2019 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/signals.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/fastapi/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-01 21:18:55.184675 rlogging-1.1.5/rlogging/namespaces.py
+-rw-r--r--   0        0        0     1542 2023-06-01 21:18:55.184675 rlogging-1.1.5/rlogging/utils.py
+-rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 rlogging-1.1.5/PKG-INFO
```

### Comparing `rlogging-1.1.4/pyproject.toml` & `rlogging-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/readme.md` & `rlogging-1.1.5/readme.md`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/rlogging/adapters.py` & `rlogging-1.1.5/rlogging/adapters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/rlogging/formatters.py` & `rlogging-1.1.5/rlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/rlogging/handlers.py` & `rlogging-1.1.5/rlogging/handlers.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/rlogging/integration/django/adapters.py` & `rlogging-1.1.5/rlogging/integration/django/adapters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/rlogging/integration/django/middleware.py` & `rlogging-1.1.5/rlogging/integration/django/middleware.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/rlogging/integration/django/signals.py` & `rlogging-1.1.5/rlogging/integration/django/signals.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/rlogging/utils.py` & `rlogging-1.1.5/rlogging/utils.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.4/PKG-INFO` & `rlogging-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlogging
-Version: 1.1.4
+Version: 1.1.5
 Summary: 
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

