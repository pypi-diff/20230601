# Comparing `tmp/sqlargon-0.0.4.tar.gz` & `tmp/sqlargon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlargon-0.0.4.tar", max compression
+gzip compressed data, was "sqlargon-0.0.5.tar", max compression
```

## Comparing `sqlargon-0.0.4.tar` & `sqlargon-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-04-15 19:35:30.078581 sqlargon-0.0.4/LICENSE
--rw-r--r--   0        0        0     3277 2023-04-15 19:35:30.078581 sqlargon-0.0.4/README.md
--rw-r--r--   0        0        0     1559 2023-04-15 19:35:30.082581 sqlargon-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      454 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/__init__.py
--rw-r--r--   0        0        0       22 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/_version.py
--rw-r--r--   0        0        0     3404 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/db.py
--rw-r--r--   0        0        0        0 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/dialects/__init__.py
--rw-r--r--   0        0        0      206 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/dialects/postgres.py
--rw-r--r--   0        0        0      243 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/dialects/sqlite.py
--rw-r--r--   0        0        0     6243 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/function_elements.py
--rw-r--r--   0        0        0        0 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/integrations/__init__.py
--rw-r--r--   0        0        0      858 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/integrations/fastapi.py
--rw-r--r--   0        0        0     1315 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/mixins.py
--rw-r--r--   0        0        0      913 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/orm.py
--rw-r--r--   0        0        0        0 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/py.typed
--rw-r--r--   0        0        0     7358 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/repository.py
--rw-r--r--   0        0        0      803 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/settings.py
--rw-r--r--   0        0        0     3033 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/types.py
--rw-r--r--   0        0        0      255 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/util.py
--rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 sqlargon-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 09:18:34.980474 sqlargon-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3264 2023-06-01 09:18:34.980474 sqlargon-0.0.5/README.md
+-rw-r--r--   0        0        0     1558 2023-06-01 09:18:34.988474 sqlargon-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      454 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/_version.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/contrib/__init__.py
+-rw-r--r--   0        0        0      986 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/contrib/fastapi.py
+-rw-r--r--   0        0        0     3417 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/db.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/dialects/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/dialects/postgres.py
+-rw-r--r--   0        0        0      243 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/dialects/sqlite.py
+-rw-r--r--   0        0        0     6243 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/function_elements.py
+-rw-r--r--   0        0        0     1315 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/mixins.py
+-rw-r--r--   0        0        0      913 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/orm.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/py.typed
+-rw-r--r--   0        0        0     7358 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/repository.py
+-rw-r--r--   0        0        0      803 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/settings.py
+-rw-r--r--   0        0        0     3033 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/types.py
+-rw-r--r--   0        0        0      484 2023-06-01 09:18:34.988474 sqlargon-0.0.5/sqlargon/util.py
+-rw-r--r--   0        0        0     3913 1970-01-01 00:00:00.000000 sqlargon-0.0.5/PKG-INFO
```

### Comparing `sqlargon-0.0.4/LICENSE` & `sqlargon-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.4/README.md` & `sqlargon-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 
 *Wrapper around SQLAlchemy async session, core and Postgres native features*
 
 ---
-Version: 0.0.4
+Version: 0.0.5
 
 Documentation: https://performancemedia.github.io/sqlargon/
 
 Repository: https://github.com/performancemedia/sqlargon
 
 ---
 
@@ -80,30 +80,30 @@
 ```
 
 ## Sessions
 
 Manager object needs `sqlalchemy.ext.asyncio.AsyncSession`, but it's possible
 to provide the session object by yourself, by subclassing Manager class e.g.
 
-
 ```python
 from fastapi import Depends
 from sqlargon import Database
-from sqlargon.integrations.fastapi import FastapiRepositoryProvider
+from sqlargon.contrib.fastapi import FastapiRepositoryProvider
 
 db = Database(url="sqlite+aiosqlite:///:memory:")
 di = FastapiRepositoryProvider(db)
 
 
 class UserRepository(Repository[User]):
     ...
-        
+
 
 from fastapi import FastAPI
 
 app = FastAPI()
 
+
 @app.get("/users")
 async def get_users(user_repository: UserRepository = Depends(di[UserRepository])):
     return await user_repository.all()
 
 ```
```

### Comparing `sqlargon-0.0.4/pyproject.toml` & `sqlargon-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "sqlargon"
-version = "0.0.4"
+version = "0.0.5"
 description = "SQLAlchemy utils for Postgres and Sqlite"
 readme = "README.md"
 authors = [
     "Radzim Kowalow <radzim.kowalow@performance-media.pl>"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 alembic = "^1.10.2"
 asyncpg = "^0.27.0"
-aiosqlite = "^0.18.0"
+aiosqlite = "^0.19.0"
 sqlalchemy = "^2.0.8"
-orjson = "^3.8.9"
-pydantic = "^1.10.7"
+pydantic = ">=1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.2"
 pytest-cov = "^4.0.0"
 flake8 = "^6.0.0"
 mypy = "^0.961"
 black = "^22.3.0"
 isort = "^5.10.1"
 tox = "^3.25.0"
 bandit = "^1.7.4"
 python-semantic-release = "^7.33.2"
 greenlet = "^2.0.2"
 fastapi = "^0.95.0"
+orjson = "^3.8.14"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.2.1"
 mkdocs-autorefs = "^0.4.1"
 mkdocs-gen-files = "^0.4.0"
 mkdocstrings-python = "^0.8.2"
```

### Comparing `sqlargon-0.0.4/sqlargon/db.py` & `sqlargon-0.0.5/sqlargon/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sqlalchemy.pool import AsyncAdaptedQueuePool, Pool
 
 from .repository import SQLAlchemyModelRepository
 from .settings import DatabaseSettings
 from .util import json_dumps, json_loads
 
 
-def configure_repository_class(dialect):
+def configure_repository_class(dialect: str) -> None:
     if dialect == "postgresql":
         from .dialects.postgres import configure_postgres_dialect
 
         configure_postgres_dialect(SQLAlchemyModelRepository)
 
     elif dialect == "sqlite":
         from .dialects.sqlite import configure_sqlite_dialect
```

### Comparing `sqlargon-0.0.4/sqlargon/function_elements.py` & `sqlargon-0.0.5/sqlargon/function_elements.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.4/sqlargon/integrations/fastapi.py` & `sqlargon-0.0.5/sqlargon/contrib/fastapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-from typing import Callable, Dict, Generic, Type, TypeVar
+from typing import Callable, Dict, Type
 
 from fastapi import Depends
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from ..db import Database
 from ..repository import SQLAlchemyModelRepository
 
-R = TypeVar("R", bound=SQLAlchemyModelRepository)
 
-
-class FastapiRepositoryProvider(Generic[R]):
+class FastapiRepositoryProvider:
     def __init__(self, db: Database):
         self.db = db
-        self._wrappers: Dict[Type[R], Callable[[AsyncSession], R]] = {}
-
-    def __getitem__(self, item: Type[R]) -> Callable[[AsyncSession], R]:
+        self._wrappers: Dict[
+            Type[SQLAlchemyModelRepository],
+            Callable[[AsyncSession], SQLAlchemyModelRepository],
+        ] = {}
+
+    def __getitem__(
+        self, item: Type[SQLAlchemyModelRepository]
+    ) -> Callable[[AsyncSession], SQLAlchemyModelRepository]:
         if not issubclass(item, SQLAlchemyModelRepository):
             raise KeyError
 
         if item not in self._wrappers:
 
-            def wrapped(session: AsyncSession = Depends(self.db.session_factory)) -> R:
+            def wrapped(
+                session: AsyncSession = Depends(self.db.session_factory),
+            ) -> SQLAlchemyModelRepository:
                 return item(session=session)
 
             self._wrappers[item] = wrapped
 
-        return self._wrappers[item]
+        return Depends(self._wrappers[item])
```

### Comparing `sqlargon-0.0.4/sqlargon/mixins.py` & `sqlargon-0.0.5/sqlargon/mixins.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.4/sqlargon/orm.py` & `sqlargon-0.0.5/sqlargon/orm.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.4/sqlargon/repository.py` & `sqlargon-0.0.5/sqlargon/repository.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.4/sqlargon/settings.py` & `sqlargon-0.0.5/sqlargon/settings.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.4/sqlargon/types.py` & `sqlargon-0.0.5/sqlargon/types.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.4/PKG-INFO` & `sqlargon-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: sqlargon
-Version: 0.0.4
+Version: 0.0.5
 Summary: SQLAlchemy utils for Postgres and Sqlite
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiosqlite (>=0.18.0,<0.19.0)
+Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: alembic (>=1.10.2,<2.0.0)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
-Requires-Dist: orjson (>=3.8.9,<4.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=1.0)
 Requires-Dist: sqlalchemy (>=2.0.8,<3.0.0)
 Description-Content-Type: text/markdown
 
 # SQLArgon
 
 ![CI](https://github.com/performancemedia/sqlargon/workflows/CI/badge.svg)
 ![Build](https://github.com/performancemedia/sqlargon/workflows/Publish/badge.svg)
@@ -29,15 +28,15 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 
 *Wrapper around SQLAlchemy async session, core and Postgres native features*
 
 ---
-Version: 0.0.4
+Version: 0.0.5
 
 Documentation: https://performancemedia.github.io/sqlargon/
 
 Repository: https://github.com/performancemedia/sqlargon
 
 ---
 
@@ -99,31 +98,31 @@
 ```
 
 ## Sessions
 
 Manager object needs `sqlalchemy.ext.asyncio.AsyncSession`, but it's possible
 to provide the session object by yourself, by subclassing Manager class e.g.
 
-
 ```python
 from fastapi import Depends
 from sqlargon import Database
-from sqlargon.integrations.fastapi import FastapiRepositoryProvider
+from sqlargon.contrib.fastapi import FastapiRepositoryProvider
 
 db = Database(url="sqlite+aiosqlite:///:memory:")
 di = FastapiRepositoryProvider(db)
 
 
 class UserRepository(Repository[User]):
     ...
-        
+
 
 from fastapi import FastAPI
 
 app = FastAPI()
 
+
 @app.get("/users")
 async def get_users(user_repository: UserRepository = Depends(di[UserRepository])):
     return await user_repository.all()
 
 ```
```

