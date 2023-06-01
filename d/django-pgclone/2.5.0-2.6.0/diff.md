# Comparing `tmp/django_pgclone-2.5.0.tar.gz` & `tmp/django_pgclone-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgclone-2.5.0.tar", max compression
+gzip compressed data, was "django_pgclone-2.6.0.tar", max compression
```

## Comparing `django_pgclone-2.5.0.tar` & `django_pgclone-2.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1456 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/LICENSE
--rw-r--r--   0        0        0     2372 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/README.rst
--rw-r--r--   0        0        0      196 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/__init__.py
--rw-r--r--   0        0        0     2342 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/copy_cmd.py
--rw-r--r--   0        0        0     4894 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/db.py
--rw-r--r--   0        0        0     3487 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/dump_cmd.py
--rw-r--r--   0        0        0      438 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/exceptions.py
--rw-r--r--   0        0        0     2169 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/logging.py
--rw-r--r--   0        0        0     3521 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/ls_cmd.py
--rw-r--r--   0        0        0        0 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/management/commands/__init__.py
--rw-r--r--   0        0        0     7145 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/management/commands/pgclone.py
--rw-r--r--   0        0        0     2483 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/options.py
--rw-r--r--   0        0        0     8429 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/restore_cmd.py
--rw-r--r--   0        0        0     1559 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/run.py
--rw-r--r--   0        0        0     2048 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/settings.py
--rw-r--r--   0        0        0     3505 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/storage.py
--rw-r--r--   0        0        0      152 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/version.py
--rw-r--r--   0        0        0     2333 2023-05-23 18:06:54.895585 django_pgclone-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 django_pgclone-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/LICENSE
+-rw-r--r--   0        0        0     2372 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/README.rst
+-rw-r--r--   0        0        0      196 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/__init__.py
+-rw-r--r--   0        0        0     2304 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/copy_cmd.py
+-rw-r--r--   0        0        0     5946 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/db.py
+-rw-r--r--   0        0        0     3487 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/dump_cmd.py
+-rw-r--r--   0        0        0      438 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/exceptions.py
+-rw-r--r--   0        0        0     2169 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/logging.py
+-rw-r--r--   0        0        0     3521 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/ls_cmd.py
+-rw-r--r--   0        0        0        0 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/management/commands/__init__.py
+-rw-r--r--   0        0        0     7145 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/management/commands/pgclone.py
+-rw-r--r--   0        0        0     2483 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/options.py
+-rw-r--r--   0        0        0     8350 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/restore_cmd.py
+-rw-r--r--   0        0        0     1559 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/run.py
+-rw-r--r--   0        0        0     2220 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/settings.py
+-rw-r--r--   0        0        0     3505 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/storage.py
+-rw-r--r--   0        0        0      152 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/version.py
+-rw-r--r--   0        0        0     2333 2023-06-01 01:55:05.744856 django_pgclone-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 django_pgclone-2.6.0/PKG-INFO
```

### Comparing `django_pgclone-2.5.0/LICENSE` & `django_pgclone-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/README.rst` & `django_pgclone-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/pgclone/copy_cmd.py` & `django_pgclone-2.6.0/pgclone/copy_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,19 +24,15 @@
     target_db = db.make(target_db_name, using=database, check=False)
 
     if source_db == target_db:  # pragma: no cover
         raise exceptions.RuntimeError("Target database cannot be the same as source database.")
 
     logging.success_msg("Creating copy")
     db.drop(target_db, using=database)
-    copy_db_sql = f"""
-        CREATE DATABASE "{target_db['NAME']}"
-            WITH TEMPLATE
-        "{source_db['NAME']}"
-    """
+    copy_db_sql = f'CREATE DATABASE "{target_db["NAME"]}" WITH TEMPLATE "{source_db["NAME"]}"'
     db.kill_connections(source_db, using=database)
     db.psql(copy_db_sql, using=database)
 
     logging.success_msg(f'Successfully copied database "{database}" to "{dump_key}"')
 
     return dump_key
```

### Comparing `django_pgclone-2.5.0/pgclone/db.py` & `django_pgclone-2.6.0/pgclone/db.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import contextlib
 import copy
 import functools
 import shlex
+import tempfile
+import textwrap
 
 from django.conf import settings as django_settings
 from django.db import connections, DEFAULT_DB_ALIAS
 from django.db.utils import load_backend
 
 from pgclone import exceptions, run, settings
 
@@ -105,29 +107,56 @@
     """Convert a database dictionary config to a url"""
     return shlex.quote(
         f'postgresql://{db_config["USER"]}:{db_config["PASSWORD"]}'
         f'@{db_config["HOST"]}:{db_config["PORT"]}/{db_config["NAME"]}'
     )
 
 
+def _fmt_psql_sql(sql):
+    """Formats SQL for psql execution"""
+    sql = textwrap.dedent(sql).strip()
+    if not sql.endswith(";"):  # For better debugging output
+        sql += ";"
+
+    if settings.statement_timeout() is not None:
+        sql = f"SET statement_timeout = {settings.statement_timeout()};\n{sql}"
+
+    if settings.lock_timeout() is not None:
+        sql = f"SET lock_timeout = {settings.lock_timeout()};\n{sql}"
+
+    return sql
+
+
 def psql(sql, *, using, ignore_errors=False):
-    """Runs psql -c with properly formatted SQL"""
+    """Runs psql -f with properly formatted SQL.
+
+    Ensures PGCLONE_STATEMENT_TIMEOUT and PGCLONE_LOCK_TIMEOUT are set
+    if those parameters are defined.
+    """
     db_url = url(conn(using=using))
+    sql = _fmt_psql_sql(sql)
 
-    # Format special SQL characters
-    sql = sql.replace("$", "\\$").replace("\n", " ").replace('"', '\\"').strip()
-    return run.shell(f'psql {db_url} -P pager=off -c "{sql};"', ignore_errors=ignore_errors)
+    # psql -c will run all statements in one transaction, which causes errors when using
+    # setting overrides for some commands that cannot be executed in a transaction. In order
+    # to get around this, we use the -f option to read statements from a file. Executing them
+    # this way ensures that the statements are executed in the same session and no transaction
+    with tempfile.NamedTemporaryFile() as tmp_f:
+        tmp_f.write(sql.encode("utf-8"))
+        tmp_f.flush()
+
+        return run.shell(
+            f"psql {db_url} -o /dev/null -a -v ON_ERROR_STOP=1 -P pager=off -f {tmp_f.name}",
+            ignore_errors=ignore_errors,
+        )
 
 
 def kill_connections(database, *, using):
     kill_connections_sql = f"""
-        SELECT pg_terminate_backend(pg_stat_activity.pid)
-        FROM pg_stat_activity
-        WHERE pg_stat_activity.datname = '{database["NAME"]}'
-            AND pid <> pg_backend_pid()
+        SELECT pg_terminate_backend(pg_stat_activity.pid) FROM pg_stat_activity
+            WHERE pg_stat_activity.datname = '{database["NAME"]}' AND pid <> pg_backend_pid()
     """
     psql(kill_connections_sql, using=using)
 
 
 def drop(database, *, using):
     kill_connections(database, using=using)
     drop_sql = f'DROP DATABASE IF EXISTS "{database["NAME"]}"'
```

### Comparing `django_pgclone-2.5.0/pgclone/dump_cmd.py` & `django_pgclone-2.6.0/pgclone/dump_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/pgclone/logging.py` & `django_pgclone-2.6.0/pgclone/logging.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/pgclone/ls_cmd.py` & `django_pgclone-2.6.0/pgclone/ls_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/pgclone/management/commands/pgclone.py` & `django_pgclone-2.6.0/pgclone/management/commands/pgclone.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/pgclone/options.py` & `django_pgclone-2.6.0/pgclone/options.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/pgclone/restore_cmd.py` & `django_pgclone-2.6.0/pgclone/restore_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,44 +146,36 @@
         )
 
     # When in reversible mode, make a special __curr db snapshot.
     # Avoid this if we are restoring the current db
     if reversible and local_restore_db != curr_db:
         logging.success_msg("Creating snapshot for reversible restore")
         db.drop(curr_db, using=database)
-        create_current_db_sql = f"""
-            CREATE DATABASE "{curr_db['NAME']}"
-             WITH TEMPLATE
-            "{temp_db['NAME']}"
-        """
+        create_current_db_sql = (
+            f'CREATE DATABASE "{curr_db["NAME"]}" WITH TEMPLATE "{temp_db["NAME"]}"'
+        )
         db.psql(create_current_db_sql, using=database)
 
     # pre-swap hook step
     with db.route(temp_db):
         for management_command_name in pre_swap_hooks:
             logging.success_msg(f'Running "manage.py {management_command_name}" pre_swap hook')
             run.management(management_command_name)
 
     # swap step
     logging.success_msg("Swapping the restored copy with the primary database")
     db.drop(prev_db, using=database)
     db.kill_connections(restore_db, using=database)
-    alter_db_sql = f"""
-        ALTER DATABASE "{restore_db['NAME']}" RENAME TO
-        "{prev_db['NAME']}"
-    """
+    alter_db_sql = f'ALTER DATABASE "{restore_db["NAME"]}" RENAME TO "{prev_db["NAME"]}"'
     # There's a scenario where the default DB may not exist before running
     # this, so just ignore errors on this command
     db.psql(alter_db_sql, ignore_errors=True, using=database)
 
     db.kill_connections(temp_db, using=database)
-    rename_sql = f"""
-        ALTER DATABASE "{temp_db["NAME"]}"
-        RENAME TO "{restore_db["NAME"]}"
-    """
+    rename_sql = f'ALTER DATABASE "{temp_db["NAME"]}" RENAME TO "{restore_db["NAME"]}"'
     db.psql(rename_sql, using=database)
 
     if not reversible:
         logging.success_msg("Cleaning old pgclone resources")
         db.drop(curr_db, using=database)
         db.drop(prev_db, using=database)
```

### Comparing `django_pgclone-2.5.0/pgclone/run.py` & `django_pgclone-2.6.0/pgclone/run.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/pgclone/settings.py` & `django_pgclone-2.6.0/pgclone/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 from django.conf import settings
 from django.db import DEFAULT_DB_ALIAS
 
 from pgclone import exceptions
 
 
+def statement_timeout():
+    return getattr(settings, "PGCLONE_STATEMENT_TIMEOUT", None)
+
+
+def lock_timeout():
+    return getattr(settings, "PGCLONE_LOCK_TIMEOUT", None)
+
+
 def s3_config():
     return getattr(settings, "PGCLONE_S3_CONFIG", {})
 
 
 def s3_endpoint_url():
     return getattr(settings, "PGCLONE_S3_ENDPOINT_URL", None)
```

### Comparing `django_pgclone-2.5.0/pgclone/storage.py` & `django_pgclone-2.6.0/pgclone/storage.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.5.0/pyproject.toml` & `django_pgclone-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgclone"
 packages = [
   { include = "pgclone" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "2.5.0"
+version = "2.6.0"
 description = "Dump and restore Postgres databases with Django."
 authors = ["Wes Kendall", "Ethan O'Brien"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
```

### Comparing `django_pgclone-2.5.0/PKG-INFO` & `django_pgclone-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgclone
-Version: 2.5.0
+Version: 2.6.0
 Summary: Dump and restore Postgres databases with Django.
 Home-page: https://github.com/Opus10/django-pgclone
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

