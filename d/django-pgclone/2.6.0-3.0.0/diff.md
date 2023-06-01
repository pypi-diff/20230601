# Comparing `tmp/django_pgclone-2.6.0.tar.gz` & `tmp/django_pgclone-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgclone-2.6.0.tar", max compression
+gzip compressed data, was "django_pgclone-3.0.0.tar", max compression
```

## Comparing `django_pgclone-2.6.0.tar` & `django_pgclone-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1456 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/LICENSE
--rw-r--r--   0        0        0     2372 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/README.rst
--rw-r--r--   0        0        0      196 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/__init__.py
--rw-r--r--   0        0        0     2304 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/copy_cmd.py
--rw-r--r--   0        0        0     5946 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/db.py
--rw-r--r--   0        0        0     3487 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/dump_cmd.py
--rw-r--r--   0        0        0      438 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/exceptions.py
--rw-r--r--   0        0        0     2169 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/logging.py
--rw-r--r--   0        0        0     3521 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/ls_cmd.py
--rw-r--r--   0        0        0        0 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/management/commands/__init__.py
--rw-r--r--   0        0        0     7145 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/management/commands/pgclone.py
--rw-r--r--   0        0        0     2483 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/options.py
--rw-r--r--   0        0        0     8350 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/restore_cmd.py
--rw-r--r--   0        0        0     1559 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/run.py
--rw-r--r--   0        0        0     2220 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/settings.py
--rw-r--r--   0        0        0     3505 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/storage.py
--rw-r--r--   0        0        0      152 2023-06-01 01:54:24.096981 django_pgclone-2.6.0/pgclone/version.py
--rw-r--r--   0        0        0     2333 2023-06-01 01:55:05.744856 django_pgclone-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 django_pgclone-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2372 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/README.rst
+-rw-r--r--   0        0        0      196 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/__init__.py
+-rw-r--r--   0        0        0     2159 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/copy_cmd.py
+-rw-r--r--   0        0        0     6054 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/db.py
+-rw-r--r--   0        0        0     3487 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/dump_cmd.py
+-rw-r--r--   0        0        0      438 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/exceptions.py
+-rw-r--r--   0        0        0     2169 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/logging.py
+-rw-r--r--   0        0        0     3521 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/ls_cmd.py
+-rw-r--r--   0        0        0        0 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/management/commands/__init__.py
+-rw-r--r--   0        0        0     7201 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/management/commands/pgclone.py
+-rw-r--r--   0        0        0     2483 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/options.py
+-rw-r--r--   0        0        0     9404 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/restore_cmd.py
+-rw-r--r--   0        0        0     1559 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/run.py
+-rw-r--r--   0        0        0     2220 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/settings.py
+-rw-r--r--   0        0        0     3505 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/storage.py
+-rw-r--r--   0        0        0      152 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/version.py
+-rw-r--r--   0        0        0     2333 2023-06-01 20:40:42.926421 django_pgclone-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 django_pgclone-3.0.0/PKG-INFO
```

### Comparing `django_pgclone-2.6.0/LICENSE` & `django_pgclone-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/README.rst` & `django_pgclone-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/pgclone/copy_cmd.py` & `django_pgclone-3.0.0/pgclone/copy_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,53 +6,48 @@
     Copy implementation
     """
     if not settings.allow_copy():  # pragma: no cover
         raise exceptions.RuntimeError("Copy not allowed.")
 
     source_db = db.conf(using=database)
 
-    if not dump_key or dump_key == ":current":
-        dump_key = ":current"
-        target_db_name = f'{source_db["NAME"]}__curr'
-    elif dump_key == ":previous":
-        target_db_name = f'{source_db["NAME"]}__prev'
-    else:
-        if not dump_key.startswith(":"):  # pragma: no cover
-            raise RuntimeError('Copy target must start with ":"')
-
-        target_db_name = dump_key[1:]
+    if not dump_key.startswith(":"):  # pragma: no cover
+        raise exceptions.ValueError('Copy target must start with ":"')
+    elif dump_key in (":pre", ":post"):  # pragma: no cover
+        raise exceptions.ValueError(
+            ":pre and :post are reserved names. Please use a different copy target name."
+        )
 
+    target_db_name = dump_key[1:]
     target_db = db.make(target_db_name, using=database, check=False)
 
     if source_db == target_db:  # pragma: no cover
         raise exceptions.RuntimeError("Target database cannot be the same as source database.")
 
     logging.success_msg("Creating copy")
     db.drop(target_db, using=database)
     copy_db_sql = f'CREATE DATABASE "{target_db["NAME"]}" WITH TEMPLATE "{source_db["NAME"]}"'
-    db.kill_connections(source_db, using=database)
-    db.psql(copy_db_sql, using=database)
+    db.psql(copy_db_sql, using=database, kill_connections=source_db)
 
     logging.success_msg(f'Successfully copied database "{database}" to "{dump_key}"')
 
     return dump_key
 
 
-def copy(dump_key=None, *, database=None, config=None):
+def copy(dump_key, *, database=None, config=None):
     """
     Copies a database using ``CREATE DATABASE <dump_key> TEMPLATE <database>``.
 
     Note that we use dump keys with the same syntax that ``dump`` and ``restore``
     commands take. Since ``copy`` only works with local database copies, this
     means the dump keys are always the database name prefixed with ``:``.
 
     Args:
-        dump_key (str, default=None): A name to use for the copy. Must be prefixed
+        dump_key (str): A name to use for the copy. Must be prefixed
             with ``:`` and only consist of valid database name characters.
-            If ``None``, ``:{database}__curr`` is used as the key.
         database (str, default=None): The database to copy.
         config (str, default=None): The configuration name
             from ``settings.PGCLONE_CONFIGS``.
 
     Returns:
         str: The dump key that was copied.
     """
```

### Comparing `django_pgclone-2.6.0/pgclone/db.py` & `django_pgclone-3.0.0/pgclone/db.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,20 +122,31 @@
 
     if settings.lock_timeout() is not None:
         sql = f"SET lock_timeout = {settings.lock_timeout()};\n{sql}"
 
     return sql
 
 
-def psql(sql, *, using, ignore_errors=False):
+def _kill_connections(database, *, using):
+    kill_connections_sql = f"""
+        SELECT pg_terminate_backend(pg_stat_activity.pid) FROM pg_stat_activity
+            WHERE pg_stat_activity.datname = '{database["NAME"]}' AND pid <> pg_backend_pid()
+    """
+    psql(kill_connections_sql, using=using)
+
+
+def psql(sql, *, using, ignore_errors=False, kill_connections=None):
     """Runs psql -f with properly formatted SQL.
 
     Ensures PGCLONE_STATEMENT_TIMEOUT and PGCLONE_LOCK_TIMEOUT are set
     if those parameters are defined.
     """
+    if kill_connections:
+        _kill_connections(kill_connections, using=using)
+
     db_url = url(conn(using=using))
     sql = _fmt_psql_sql(sql)
 
     # psql -c will run all statements in one transaction, which causes errors when using
     # setting overrides for some commands that cannot be executed in a transaction. In order
     # to get around this, we use the -f option to read statements from a file. Executing them
     # this way ensures that the statements are executed in the same session and no transaction
@@ -145,19 +156,11 @@
 
         return run.shell(
             f"psql {db_url} -o /dev/null -a -v ON_ERROR_STOP=1 -P pager=off -f {tmp_f.name}",
             ignore_errors=ignore_errors,
         )
 
 
-def kill_connections(database, *, using):
-    kill_connections_sql = f"""
-        SELECT pg_terminate_backend(pg_stat_activity.pid) FROM pg_stat_activity
-            WHERE pg_stat_activity.datname = '{database["NAME"]}' AND pid <> pg_backend_pid()
-    """
-    psql(kill_connections_sql, using=using)
-
-
 def drop(database, *, using):
-    kill_connections(database, using=using)
+    _kill_connections(database, using=using)
     drop_sql = f'DROP DATABASE IF EXISTS "{database["NAME"]}"'
     psql(drop_sql, using=using)
```

### Comparing `django_pgclone-2.6.0/pgclone/dump_cmd.py` & `django_pgclone-3.0.0/pgclone/dump_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/pgclone/logging.py` & `django_pgclone-3.0.0/pgclone/logging.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/pgclone/ls_cmd.py` & `django_pgclone-3.0.0/pgclone/ls_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/pgclone/management/commands/pgclone.py` & `django_pgclone-3.0.0/pgclone/management/commands/pgclone.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             ),
         )
         parser.add_argument(
             "-r",
             "--reversible",
             default=None,  # Use None so that configs/settings can be used as defaults
             action="store_true",
-            help="Keep current and previous database copies available for reversion.",
+            help="Keep pre/post restore database copies available for reversion.",
         )
         parser.add_argument(
             "-d",
             "--database",
             help="Restore to this database.",
         )
         parser.add_argument(
@@ -181,19 +181,22 @@
             storage_location=options["storage_location"],
             config=options["config"],
         )
 
 
 class CopyCommand(BaseSubcommand):
     def add_arguments(self, parser):
-        parser.add_argument("dump_key", nargs="?", help="The local dump key to copy to.")
+        parser.add_argument(
+            "dump_key",
+            help="The database target in the format of a local dump key, e.g. ':db_backup'",
+        )
         parser.add_argument(
             "-d",
             "--database",
-            help="Restore to this database.",
+            help="Copy this database.",
         )
         parser.add_argument(
             "-c",
             "--config",
             help="Use this configuration to supply default option values.",
         )
```

### Comparing `django_pgclone-2.6.0/pgclone/options.py` & `django_pgclone-3.0.0/pgclone/options.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/pgclone/restore_cmd.py` & `django_pgclone-3.0.0/pgclone/restore_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,40 +28,39 @@
         cursor.execute("SHOW search_path;")
         search_path = cursor.fetchone()[0]
 
     set_search_path_sql = f'ALTER DATABASE "{database["NAME"]}" SET search_path to {search_path}'
     db.psql(set_search_path_sql, using=using)
 
 
-def _local_restore(dump_key, *, temp_db, curr_db, prev_db, using):
+def _local_restore(dump_key, *, temp_db, post_db, pre_db, using):
     """
     Performs a restore using a local database
     """
-    if dump_key == ":current":
-        local_restore_db = curr_db
-    elif dump_key == ":previous":
-        local_restore_db = prev_db
+    if dump_key == ":post":
+        local_restore_db = post_db
+    elif dump_key == ":pre":
+        local_restore_db = pre_db
     else:
         local_restore_db = db.make(dump_key[1:], using=using)
 
     if not _db_exists(local_restore_db, using=using):
         raise exceptions.RuntimeError(
             f'Local database "{local_restore_db["NAME"]}" does not exist.'
             ' Use "pgclone ls --local" to see local database keys.'
         )
 
     # Perform the local restore process. It is completely valid to
     # try to restore the temp_db, so do nothing if this database
     # is provided by the user
     if local_restore_db != temp_db:  # pragma: no branch
         db.drop(temp_db, using=using)
-        create_temp_sql = f"""
-            CREATE DATABASE "{temp_db["NAME"]}"
-            TEMPLATE "{local_restore_db["NAME"]}"
-        """
+        create_temp_sql = (
+            f'CREATE DATABASE "{temp_db["NAME"]}" WITH TEMPLATE "{local_restore_db["NAME"]}"'
+        )
         db.psql(create_temp_sql, using=using)
 
     _set_search_path(temp_db, using=using)
 
     return dump_key
 
 
@@ -113,75 +112,91 @@
     if not dump_key:
         raise exceptions.ValueError("Must provide a dump key or prefix to restore.")
 
     # Restore works in the following steps with the following databases:
     # 1. Create the temp_db database to perform the restore without
     #    affecting the restore_db
     # 2. Call pg_restore on temp_db
-    # 3. Apply any pre_swap_hooks to temp_db
-    # 4. Terminate all connections on restore_db so that we
+    # 3. If using --reversible, create the post_db restore copy of temp_db
+    # 4. Apply any pre_swap_hooks to temp_db
+    # 5. Terminate all connections on restore_db so that we
     #    can swap in the temp_db
-    # 4. Rename restore_db to prev_db
-    # 5. Rename temp_db to restore_db
-    # 6. Delete prev_db
+    # 6. Rename restore_db to swap_db
+    # 7. Rename temp_db to restore_db
+    # 8. Delete swap_db and post/pre_db if not using --reversible OR
+    #    rename swap_db to pre_db if using --reversible
     #
     # Database variable names below reflect this process.
 
     restore_db = db.conf(using=database)
+    # The DB in which a restore happens behind the scenes. Pre-swap hooks
+    # are applied to it
     temp_db = db.make(restore_db["NAME"] + "__temp", using=database)
-    prev_db = db.make(restore_db["NAME"] + "__prev", using=database)
-    curr_db = db.make(restore_db["NAME"] + "__curr", using=database)
-    local_restore_db = None
+    # A temporary DB to use for the swap step. Helps us do a quick rename of
+    # DBs.
+    swap_db = db.make(restore_db["NAME"] + "__swap", using=database)
+    # These two DBs are only for reversible restores
+    pre_db = db.make(restore_db["NAME"] + "__pre", using=database)
+    post_db = db.make(restore_db["NAME"] + "__post", using=database)
+    is_local_restore = dump_key.startswith(":")
 
-    if dump_key.startswith(":"):
+    if is_local_restore:
         dump_key = _local_restore(
             dump_key,
             temp_db=temp_db,
-            curr_db=curr_db,
-            prev_db=prev_db,
+            post_db=post_db,
+            pre_db=pre_db,
             using=database,
         )
     else:
         dump_key = _remote_restore(
             dump_key, temp_db=temp_db, using=database, storage_location=storage_location
         )
 
-    # When in reversible mode, make a special __curr db snapshot.
-    # Avoid this if we are restoring the current db
-    if reversible and local_restore_db != curr_db:
-        logging.success_msg("Creating snapshot for reversible restore")
-        db.drop(curr_db, using=database)
-        create_current_db_sql = (
-            f'CREATE DATABASE "{curr_db["NAME"]}" WITH TEMPLATE "{temp_db["NAME"]}"'
+    # When in reversible mode, make a special __post db snapshot.
+    # Note that reversible mode is a noop for local restores.
+    if reversible and not is_local_restore:
+        logging.success_msg("Creating 'post' snapshot for reversible restore")
+        db.drop(post_db, using=database)
+        create_post_db_sql = (
+            f'CREATE DATABASE "{post_db["NAME"]}" WITH TEMPLATE "{temp_db["NAME"]}"'
         )
-        db.psql(create_current_db_sql, using=database)
+        db.psql(create_post_db_sql, using=database)
 
     # pre-swap hook step
     with db.route(temp_db):
         for management_command_name in pre_swap_hooks:
             logging.success_msg(f'Running "manage.py {management_command_name}" pre_swap hook')
             run.management(management_command_name)
 
     # swap step
     logging.success_msg("Swapping the restored copy with the primary database")
-    db.drop(prev_db, using=database)
-    db.kill_connections(restore_db, using=database)
-    alter_db_sql = f'ALTER DATABASE "{restore_db["NAME"]}" RENAME TO "{prev_db["NAME"]}"'
-    # There's a scenario where the default DB may not exist before running
+    db.drop(swap_db, using=database)
+    alter_db_sql = f'ALTER DATABASE "{restore_db["NAME"]}" RENAME TO "{swap_db["NAME"]}"'
+    # There's a scenario where the restore DB may not exist before running
     # this, so just ignore errors on this command
-    db.psql(alter_db_sql, ignore_errors=True, using=database)
+    db.psql(alter_db_sql, ignore_errors=True, using=database, kill_connections=restore_db)
 
-    db.kill_connections(temp_db, using=database)
     rename_sql = f'ALTER DATABASE "{temp_db["NAME"]}" RENAME TO "{restore_db["NAME"]}"'
-    db.psql(rename_sql, using=database)
+    db.psql(rename_sql, using=database, kill_connections=temp_db)
 
-    if not reversible:
-        logging.success_msg("Cleaning old pgclone resources")
-        db.drop(curr_db, using=database)
-        db.drop(prev_db, using=database)
+    # If we're doing a reversible remote restore, keep the swap DB around as the prev DB
+    if reversible and not is_local_restore:
+        logging.success_msg("Creating 'pre' snapshot for reversible restore")
+        db.drop(pre_db, using=database)
+        rename_sql = f'ALTER DATABASE "{swap_db["NAME"]}" RENAME TO "{pre_db["NAME"]}"'
+        db.psql(rename_sql, using=database, kill_connections=swap_db)
+    else:
+        logging.success_msg("Cleaning pgclone resources")
+        db.drop(swap_db, using=database)
+        if not reversible and not is_local_restore:
+            # If we did a non-reversible remote restore, remove any previous restore
+            # points from reversible restores
+            db.drop(post_db, using=database)
+            db.drop(pre_db, using=database)
 
     logging.success_msg(f'Successfully restored dump "{dump_key}" to database "{database}"')
 
     return dump_key
 
 
 def restore(
```

### Comparing `django_pgclone-2.6.0/pgclone/run.py` & `django_pgclone-3.0.0/pgclone/run.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/pgclone/settings.py` & `django_pgclone-3.0.0/pgclone/settings.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/pgclone/storage.py` & `django_pgclone-3.0.0/pgclone/storage.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.6.0/pyproject.toml` & `django_pgclone-3.0.0/pyproject.toml`

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
-version = "2.6.0"
+version = "3.0.0"
 description = "Dump and restore Postgres databases with Django."
 authors = ["Wes Kendall", "Ethan O'Brien"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
```

### Comparing `django_pgclone-2.6.0/PKG-INFO` & `django_pgclone-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgclone
-Version: 2.6.0
+Version: 3.0.0
 Summary: Dump and restore Postgres databases with Django.
 Home-page: https://github.com/Opus10/django-pgclone
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

