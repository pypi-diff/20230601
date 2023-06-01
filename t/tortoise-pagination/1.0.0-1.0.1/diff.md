# Comparing `tmp/tortoise_pagination-1.0.0.tar.gz` & `tmp/tortoise_pagination-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_pagination-1.0.0.tar", max compression
+gzip compressed data, was "tortoise_pagination-1.0.1.tar", max compression
```

## Comparing `tortoise_pagination-1.0.0.tar` & `tortoise_pagination-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,5 @@
--rw-r--r--   0        0        0      750 2023-06-01 17:24:11.761126 tortoise_pagination-1.0.0/README.md
--rw-r--r--   0        0        0      532 2023-06-01 17:09:36.872840 tortoise_pagination-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        1 2023-06-01 17:09:27.039386 tortoise_pagination-1.0.0/tortoise_pagination/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-06-01 17:09:27.039386 tortoise_pagination-1.0.0/tortoise_pagination/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2023-06-01 17:09:27.046053 tortoise_pagination-1.0.0/tortoise_pagination/.ruff_cache/content/4fdb0d2cbbe7c301
--rw-r--r--   0        0        0       55 2023-06-01 17:17:33.284615 tortoise_pagination-1.0.0/tortoise_pagination/__init__.py
--rw-r--r--   0        0        0     1656 2023-06-01 17:18:51.902773 tortoise_pagination-1.0.0/tortoise_pagination/pagination.py
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 tortoise_pagination-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-06-01 17:28:02.913992 tortoise_pagination-1.0.1/README.md
+-rw-r--r--   0        0        0      532 2023-06-01 19:17:19.109120 tortoise_pagination-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-06-01 17:17:33.284615 tortoise_pagination-1.0.1/tortoise_pagination/__init__.py
+-rw-r--r--   0        0        0     1656 2023-06-01 17:18:51.902773 tortoise_pagination-1.0.1/tortoise_pagination/pagination.py
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 tortoise_pagination-1.0.1/PKG-INFO
```

### Comparing `tortoise_pagination-1.0.0/README.md` & `tortoise_pagination-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Usage
 Supposing in `myapp.schema` you have a pydantic `BaseModel` to represent your model
 
 ```python
 from fastapi import Depends
-from tortoise_pagination improt Pagination, Page
+from tortoise_pagination import Pagination, Page
 
 from myapp.main import app
 from myapp.models import MyModel
 from myapp.schema import MySchema
 
 
 @app.get('/mymodel')
```

### Comparing `tortoise_pagination-1.0.0/pyproject.toml` & `tortoise_pagination-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tortoise-pagination"
-version = "1.0.0"
+version = "1.0.1"
 description = "Pagination for Tortoise-ORM on FastAPI"
 authors = ["Sebastien Nicolet <snicolet95@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tortoise_pagination"}]
 
 [tool.poetry.dependencies]
```

### Comparing `tortoise_pagination-1.0.0/tortoise_pagination/pagination.py` & `tortoise_pagination-1.0.1/tortoise_pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `tortoise_pagination-1.0.0/PKG-INFO` & `tortoise_pagination-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-pagination
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pagination for Tortoise-ORM on FastAPI
 License: MIT
 Author: Sebastien Nicolet
 Author-email: snicolet95@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 
 # Usage
 Supposing in `myapp.schema` you have a pydantic `BaseModel` to represent your model
 
 ```python
 from fastapi import Depends
-from tortoise_pagination improt Pagination, Page
+from tortoise_pagination import Pagination, Page
 
 from myapp.main import app
 from myapp.models import MyModel
 from myapp.schema import MySchema
 
 
 @app.get('/mymodel')
```

