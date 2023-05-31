# Comparing `tmp/postgres_lock-0.1.0.tar.gz` & `tmp/postgres_lock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres_lock-0.1.0.tar", max compression
+gzip compressed data, was "postgres_lock-0.1.1.tar", max compression
```

## Comparing `postgres_lock-0.1.0.tar` & `postgres_lock-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1496 2023-05-30 13:15:35.574393 postgres_lock-0.1.0/LICENSE
--rw-r--r--   0        0        0     2972 2023-05-31 21:00:50.824114 postgres_lock-0.1.0/README.md
--rw-r--r--   0        0        0      107 2023-05-31 14:20:25.432460 postgres_lock-0.1.0/postgres_lock/__init__.py
--rw-r--r--   0        0        0     1708 2023-05-31 15:47:45.539175 postgres_lock-0.1.0/postgres_lock/asyncpg.py
--rw-r--r--   0        0        0      355 2023-05-31 14:47:42.602709 postgres_lock-0.1.0/postgres_lock/errors.py
--rw-r--r--   0        0        0     8485 2023-05-31 20:27:01.047229 postgres_lock-0.1.0/postgres_lock/lock.py
--rw-r--r--   0        0        0     1796 2023-05-31 14:47:42.602709 postgres_lock-0.1.0/postgres_lock/psycopg2.py
--rw-r--r--   0        0        0     2198 2023-05-31 14:47:42.602709 postgres_lock-0.1.0/postgres_lock/psycopg3.py
--rw-r--r--   0        0        0     2094 2023-05-31 20:08:55.316117 postgres_lock-0.1.0/postgres_lock/sqlalchemy.py
--rw-r--r--   0        0        0      421 2023-05-30 21:34:31.696622 postgres_lock-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 postgres_lock-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-05-30 13:15:35.574393 postgres_lock-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3015 2023-05-31 23:45:03.742762 postgres_lock-0.1.1/README.md
+-rw-r--r--   0        0        0      107 2023-05-31 14:20:25.432460 postgres_lock-0.1.1/postgres_lock/__init__.py
+-rw-r--r--   0        0        0     1708 2023-05-31 15:47:45.539175 postgres_lock-0.1.1/postgres_lock/asyncpg.py
+-rw-r--r--   0        0        0      354 2023-05-31 22:29:05.371623 postgres_lock-0.1.1/postgres_lock/errors.py
+-rw-r--r--   0        0        0     8570 2023-05-31 23:33:28.102639 postgres_lock-0.1.1/postgres_lock/lock.py
+-rw-r--r--   0        0        0     1796 2023-05-31 14:47:42.602709 postgres_lock-0.1.1/postgres_lock/psycopg2.py
+-rw-r--r--   0        0        0     2198 2023-05-31 14:47:42.602709 postgres_lock-0.1.1/postgres_lock/psycopg3.py
+-rw-r--r--   0        0        0     2094 2023-05-31 20:08:55.316117 postgres_lock-0.1.1/postgres_lock/sqlalchemy.py
+-rw-r--r--   0        0        0      542 2023-05-31 23:46:13.084356 postgres_lock-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3804 1970-01-01 00:00:00.000000 postgres_lock-0.1.1/PKG-INFO
```

### Comparing `postgres_lock-0.1.0/LICENSE` & `postgres_lock-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.0/README.md` & `postgres_lock-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Lock mechanism implemented with Postgres advisory locks.
 
 Easily implement distributed database locking.
 
 ### Install
 
 ```sh
-python3 -m pip install postgres_lock
+pip install postgres-lock
 ```
 
 ### Supported database interfaces
 
 - **asyncpg**
   - asynchronous
 - **psycopg2**
@@ -139,7 +139,12 @@
 
 # create and use lock
 with Lock(conn, "shared-identifier", interface="asyncpg"):
     print("Acquired lock!")
 
     # do something here
 ```
+
+### Changelog
+
+- **0.1.1**
+  - Key can be str or int
```

### Comparing `postgres_lock-0.1.0/postgres_lock/asyncpg.py` & `postgres_lock-0.1.1/postgres_lock/asyncpg.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.0/postgres_lock/lock.py` & `postgres_lock-0.1.1/postgres_lock/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,44 +24,44 @@
         - asyncpg
             - asynchronous
         - psycopg2
             - synchronous
         - psycopg3
             - asynchronous
             - synchronous
-        - sqlalchemy 1 & 2 (can use any underlying database interface)
+        - sqlalchemy (supports version 1 & 2; can use any underlying database interface)
             - asynchronous
             - synchronous
 
     Lock scopes:
         - session: only a single session can hold the lock
-        - transaction: only a single transaction can hold the lock
+        - transaction: only a single transaction within a single session can hold the lock
 
     Modes:
         - blocked: do not return until the lock is acquired
         - nonblocking: return immediately with or without the lock being acquired
 
     Sharing (locks can or cannot be reacquired from the same scope)
     """
 
     conn: Any
     interface: str
-    key: str
+    key: str | int
     lock_id: int
     scope: str
     shared: bool
 
     blocking_lock_func: str
     nonblocking_lock_func: str
     unlock_func: str
 
     def __init__(
         self,
         conn: Any,
-        key: str,
+        key: str | int,
         interface: Literal[
             "auto",
             "asyncpg",
             "psycopg2",
             "psycopg3",
             "sqlalchemy",
         ] = "auto",
@@ -69,24 +69,26 @@
         shared: bool = False,
     ):
         """
         Create a new Lock instance.
 
         Parameters:
             conn (object): Database connection.
-            key (str): Unique lock key.
+            key (str|int): Unique lock key.
             interface (str): Database interface.
             scope (str): Lock scope.
             shared (bool): Use a shared lock.
         """
         self.conn = conn
         self.interface = interface
         self.impl = self._load_impl()
         self.key = key
-        self.lock_id = str(int(hashlib.sha1(key.encode("utf-8")).hexdigest(), 16))[:18]
+        self.lock_id = str(int(hashlib.sha1(str(key).encode("utf-8")).hexdigest(), 16))[
+            :18
+        ]
         self.scope = scope
         self._locked = False
         self._ref_count = 0
         self._shared = shared
 
         infix = "_xact"
         suffix = ""
```

### Comparing `postgres_lock-0.1.0/postgres_lock/psycopg2.py` & `postgres_lock-0.1.1/postgres_lock/psycopg2.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.0/postgres_lock/psycopg3.py` & `postgres_lock-0.1.1/postgres_lock/psycopg3.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.0/postgres_lock/sqlalchemy.py` & `postgres_lock-0.1.1/postgres_lock/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.0/PKG-INFO` & `postgres_lock-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: postgres-lock
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lock mechanism implemented with Postgres advisory locks.
+Home-page: https://github.com/seankerr/py-postgres-lock
 License: BSD-3-Clause
+Keywords: postgres,postgresql,distributed,lock
 Author: Sean Kerr
 Author-email: sean@code-box.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/seankerr/py-postgres-lock
 Description-Content-Type: text/markdown
 
 ## postgres-lock
 
 Lock mechanism implemented with Postgres advisory locks.
 
 Easily implement distributed database locking.
 
 ### Install
 
 ```sh
-python3 -m pip install postgres_lock
+pip install postgres-lock
 ```
 
 ### Supported database interfaces
 
 - **asyncpg**
   - asynchronous
 - **psycopg2**
@@ -157,7 +160,12 @@
 # create and use lock
 with Lock(conn, "shared-identifier", interface="asyncpg"):
     print("Acquired lock!")
 
     # do something here
 ```
 
+### Changelog
+
+- **0.1.1**
+  - Key can be str or int
+
```

