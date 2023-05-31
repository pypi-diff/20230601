# Comparing `tmp/rick-db-1.1.2.tar.gz` & `tmp/rick-db-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rick-db-1.1.2.tar", last modified: Sun May 21 18:30:57 2023, max compression
+gzip compressed data, was "rick-db-1.2.0.tar", last modified: Wed May 31 22:54:34 2023, max compression
```

## Comparing `rick-db-1.1.2.tar` & `rick-db-1.2.0.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 18:30:36.000000 rick-db-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-21 18:30:57.715435 rick-db-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-21 18:30:36.000000 rick-db-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/conn/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/conn/pg/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/pg/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/conn/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/sqlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/dbgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/profiler/profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/util/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/util/pg/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/pginfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/util/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/sqlite/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/sqlite/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:30:57.715435 rick-db-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-21 18:30:36.000000 rick-db-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/tests/conn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/tests/conn/pg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/pg/test_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/tests/conn/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/sqlite/test_sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/dbgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/tests/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_dialects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)    36045 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_pgsql_dbgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_pgsql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_sqlite_dbgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_sqlite_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/tests/util/pg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/test_pginfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/tests/util/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/sqlite/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/sqlite/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 22:54:14.000000 rick-db-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-31 22:54:34.775360 rick-db-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-31 22:54:14.000000 rick-db-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.767360 rick-db-1.2.0/rick_db/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/commands/dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/commands/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/cli/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/conn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/conn/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/conn/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/conn/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/conn/pg/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/conn/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/conn/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/conn/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/dbgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/profiler/profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/sql/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/sql/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/sql/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/sql/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49904 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/sql/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/sql/sql_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/sql/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/util/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/pg/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/pg/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/pg/pginfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/pg/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.771360 rick-db-1.2.0/rick_db/util/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/sqlite/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/util/sqlite/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 22:54:14.000000 rick-db-1.2.0/rick_db/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.767360 rick-db-1.2.0/rick_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-31 22:54:34.000000 rick-db-1.2.0/rick_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-31 22:54:34.000000 rick-db-1.2.0/rick_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:54:34.000000 rick-db-1.2.0/rick_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 22:54:34.000000 rick-db-1.2.0/rick_db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:54:34.000000 rick-db-1.2.0/rick_db.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 22:54:34.000000 rick-db-1.2.0/rick_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 22:54:34.000000 rick-db-1.2.0/rick_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:54:34.775360 rick-db-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-31 22:54:14.000000 rick-db-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/tests/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/conn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/tests/conn/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/conn/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/conn/pg/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/tests/conn/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/conn/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/conn/sqlite/test_sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/dbgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/tests/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/sql/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/sql/test_dialects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/sql/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38909 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/sql/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/sql/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/sql/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/test_pgsql_dbgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/test_pgsql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/test_sqlite_dbgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/test_sqlite_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/tests/util/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/pg/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/pg/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/pg/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/pg/test_pginfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:34.775360 rick-db-1.2.0/tests/util/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/sqlite/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-31 22:54:14.000000 rick-db-1.2.0/tests/util/sqlite/test_migrations.py
```

### Comparing `rick-db-1.1.2/LICENSE` & `rick-db-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/PKG-INFO` & `rick-db-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rick-db
-Version: 1.1.2
+Version: 1.2.0
 Summary: SQL database layer
 Home-page: https://git.oddbit.org/OddBit/rick_db
 Author: Joao Pinheiro
 Author-email: 
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,16 +18,17 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-rick_db - Simple SQL database layer
---
+# rick_db - Simple SQL database layer
+
+
 [![Tests](https://github.com/oddbit-project/rick_db/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick_db/actions)
 [![pypi](https://img.shields.io/pypi/v/rick_db.svg)](https://pypi.org/project/rick_db/)
 [![license](https://img.shields.io/pypi/l/rick-db.svg)](https://git.oddbit.org/OddBit/rick_db/src/branch/master/LICENSE)
 
 rick_db is a simple SQL database layer for Python3. It includes connection management, Object Mapper, Query Builder,
 and a Repository pattern implementation. It is **not** an ORM, and it's not meant to replace one. 
 
@@ -59,110 +60,119 @@
 
 ```python
 from rick_db import fieldmapper, Repository
 from rick_db.conn.pg import PgConnection
 from rick_db.sql import Select, Literal
 
 
-@fieldmapper(tablename='publisher', pk='id_publisher')
+@fieldmapper(tablename="publisher", pk="id_publisher")
 class Publisher:
-    id = 'id_publisher'
-    name = 'name'
+    id = "id_publisher"
+    name = "name"
 
 
-@fieldmapper(tablename='book', pk='id_book')
+@fieldmapper(tablename="book", pk="id_book")
 class Book:
-    id = 'id_book'
-    title = 'title'
-    total_pages = 'total_pages'
-    rating = 'rating'
-    isbn = 'isbn'
-    published = 'published_date'
-    fk_publisher = 'fk_publisher'
+    id = "id_book"
+    title = "title"
+    total_pages = "total_pages"
+    rating = "rating"
+    isbn = "isbn"
+    published = "published_date"
+    fk_publisher = "fk_publisher"
 
 
-@fieldmapper(tablename='author', pk='id_author')
+@fieldmapper(tablename="author", pk="id_author")
 class Author:
-    id = 'id_author'
-    first_name = 'first_name'
-    middle_name = 'middle_name'
-    last_name = 'last_name'
+    id = "id_author"
+    first_name = "first_name"
+    middle_name = "middle_name"
+    last_name = "last_name"
 
 
-@fieldmapper(tablename='book_author', pk='id_book_author')
+@fieldmapper(tablename="book_author", pk="id_book_author")
 class BookAuthor:
-    id = 'id_book_author'
-    fk_book = 'fk_book'
-    fk_author = 'fk_author'
+    id = "id_book_author"
+    fk_book = "fk_book"
+    fk_author = "fk_author"
 
 
 class AuthorRepository(Repository):
-
     def __init__(self, db):
         super().__init__(db, Author)
 
     def calc_avg_rating(self, id_author: int):
         """
         Calculate average rating for a given author
         :param id_author: author id
         :return: average rating, if any
         """
-        
+
         # generated query:
-        # SELECT avg(rating) AS "rating" FROM "book" INNER JOIN "book_author" ON 
+        # SELECT avg(rating) AS "rating" FROM "book" INNER JOIN "book_author" ON
         # "book"."id_book"="book_author"."fk_book" WHERE ("fk_author" = %s)
-        qry = Select(self._dialect). \
-            from_(Book, {Literal("avg({})".format(Book.rating)): 'rating'}). \
-            join(BookAuthor, BookAuthor.fk_book, Book, Book.id). \
-            where(BookAuthor.fk_author, '=', id_author)
-        
+        qry = (
+            Select(self._dialect)
+            .from_(Book, {Literal("avg({})".format(Book.rating)): "rating"})
+            .join(BookAuthor, BookAuthor.fk_book, Book, Book.id)
+            .where(BookAuthor.fk_author, "=", id_author)
+        )
+
         # retrieve result as list of type Book (to get the rating field)
         rset = self.fetch(qry, cls=Book)
         if len(rset) > 0:
             return rset.pop(0).rating
         return 0
 
     def books(self, id_author: int) -> list[Book]:
         """
         Retrieve all books for the given author
         :return: list[Book]
         """
-        
-        qry = Select(self._dialect). \
-            from_(Book). \
-            join(BookAuthor, BookAuthor.fk_book, Book, Book.id). \
-            where(BookAuthor.fk_author, '=', id_author)
+
+        qry = (
+            Select(self._dialect)
+            .from_(Book)
+            .join(BookAuthor, BookAuthor.fk_book, Book, Book.id)
+            .where(BookAuthor.fk_author, "=", id_author)
+        )
 
         return self.fetch(qry, cls=Book)
 
 
 def dump_author_rating(repo: AuthorRepository):
     for author in repo.fetch_all():
-        
         # calculate average
         rating = repo.calc_avg_rating(author.id)
-        
+
         # print book list
-        print("Books by {firstname} {lastname}:".format(firstname=author.first_name, lastname=author.last_name))
+        print(
+            "Books by {firstname} {lastname}:".format(
+                firstname=author.first_name, lastname=author.last_name
+            )
+        )
         for book in repo.books(author.id):
             print(book.title)
-        
-        # print average rating           
-        print("Average rating for {firstname} {lastname} is {rating}".
-              format(firstname=author.first_name, lastname=author.last_name, rating=rating))
 
-        
-if __name__ == '__main__':
+        # print average rating
+        print(
+            "Average rating for {firstname} {lastname} is {rating}".format(
+                firstname=author.first_name, lastname=author.last_name, rating=rating
+            )
+        )
+
+
+if __name__ == "__main__":
     db_cfg = {
-        'dbname': "rickdb-bookstore",
-        'user': "rickdb_user",
-        'password': "rickdb_pass",
-        'host': "localhost",
-        'port': 5432,
-        'sslmode': 'require'        
+        "dbname": "rickdb-bookstore",
+        "user": "rickdb_user",
+        "password": "rickdb_pass",
+        "host": "localhost",
+        "port": 5432,
+        "sslmode": "require",
     }
 
     conn = PgConnection(**db_cfg)
     repo = AuthorRepository(conn)
     dump_author_rating(repo)
 ```
```

### Comparing `rick-db-1.1.2/README.md` & `rick-db-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-rick_db - Simple SQL database layer
---
+# rick_db - Simple SQL database layer
+
+
 [![Tests](https://github.com/oddbit-project/rick_db/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick_db/actions)
 [![pypi](https://img.shields.io/pypi/v/rick_db.svg)](https://pypi.org/project/rick_db/)
 [![license](https://img.shields.io/pypi/l/rick-db.svg)](https://git.oddbit.org/OddBit/rick_db/src/branch/master/LICENSE)
 
 rick_db is a simple SQL database layer for Python3. It includes connection management, Object Mapper, Query Builder,
 and a Repository pattern implementation. It is **not** an ORM, and it's not meant to replace one. 
 
@@ -35,110 +36,119 @@
 
 ```python
 from rick_db import fieldmapper, Repository
 from rick_db.conn.pg import PgConnection
 from rick_db.sql import Select, Literal
 
 
-@fieldmapper(tablename='publisher', pk='id_publisher')
+@fieldmapper(tablename="publisher", pk="id_publisher")
 class Publisher:
-    id = 'id_publisher'
-    name = 'name'
+    id = "id_publisher"
+    name = "name"
 
 
-@fieldmapper(tablename='book', pk='id_book')
+@fieldmapper(tablename="book", pk="id_book")
 class Book:
-    id = 'id_book'
-    title = 'title'
-    total_pages = 'total_pages'
-    rating = 'rating'
-    isbn = 'isbn'
-    published = 'published_date'
-    fk_publisher = 'fk_publisher'
+    id = "id_book"
+    title = "title"
+    total_pages = "total_pages"
+    rating = "rating"
+    isbn = "isbn"
+    published = "published_date"
+    fk_publisher = "fk_publisher"
 
 
-@fieldmapper(tablename='author', pk='id_author')
+@fieldmapper(tablename="author", pk="id_author")
 class Author:
-    id = 'id_author'
-    first_name = 'first_name'
-    middle_name = 'middle_name'
-    last_name = 'last_name'
+    id = "id_author"
+    first_name = "first_name"
+    middle_name = "middle_name"
+    last_name = "last_name"
 
 
-@fieldmapper(tablename='book_author', pk='id_book_author')
+@fieldmapper(tablename="book_author", pk="id_book_author")
 class BookAuthor:
-    id = 'id_book_author'
-    fk_book = 'fk_book'
-    fk_author = 'fk_author'
+    id = "id_book_author"
+    fk_book = "fk_book"
+    fk_author = "fk_author"
 
 
 class AuthorRepository(Repository):
-
     def __init__(self, db):
         super().__init__(db, Author)
 
     def calc_avg_rating(self, id_author: int):
         """
         Calculate average rating for a given author
         :param id_author: author id
         :return: average rating, if any
         """
-        
+
         # generated query:
-        # SELECT avg(rating) AS "rating" FROM "book" INNER JOIN "book_author" ON 
+        # SELECT avg(rating) AS "rating" FROM "book" INNER JOIN "book_author" ON
         # "book"."id_book"="book_author"."fk_book" WHERE ("fk_author" = %s)
-        qry = Select(self._dialect). \
-            from_(Book, {Literal("avg({})".format(Book.rating)): 'rating'}). \
-            join(BookAuthor, BookAuthor.fk_book, Book, Book.id). \
-            where(BookAuthor.fk_author, '=', id_author)
-        
+        qry = (
+            Select(self._dialect)
+            .from_(Book, {Literal("avg({})".format(Book.rating)): "rating"})
+            .join(BookAuthor, BookAuthor.fk_book, Book, Book.id)
+            .where(BookAuthor.fk_author, "=", id_author)
+        )
+
         # retrieve result as list of type Book (to get the rating field)
         rset = self.fetch(qry, cls=Book)
         if len(rset) > 0:
             return rset.pop(0).rating
         return 0
 
     def books(self, id_author: int) -> list[Book]:
         """
         Retrieve all books for the given author
         :return: list[Book]
         """
-        
-        qry = Select(self._dialect). \
-            from_(Book). \
-            join(BookAuthor, BookAuthor.fk_book, Book, Book.id). \
-            where(BookAuthor.fk_author, '=', id_author)
+
+        qry = (
+            Select(self._dialect)
+            .from_(Book)
+            .join(BookAuthor, BookAuthor.fk_book, Book, Book.id)
+            .where(BookAuthor.fk_author, "=", id_author)
+        )
 
         return self.fetch(qry, cls=Book)
 
 
 def dump_author_rating(repo: AuthorRepository):
     for author in repo.fetch_all():
-        
         # calculate average
         rating = repo.calc_avg_rating(author.id)
-        
+
         # print book list
-        print("Books by {firstname} {lastname}:".format(firstname=author.first_name, lastname=author.last_name))
+        print(
+            "Books by {firstname} {lastname}:".format(
+                firstname=author.first_name, lastname=author.last_name
+            )
+        )
         for book in repo.books(author.id):
             print(book.title)
-        
-        # print average rating           
-        print("Average rating for {firstname} {lastname} is {rating}".
-              format(firstname=author.first_name, lastname=author.last_name, rating=rating))
 
-        
-if __name__ == '__main__':
+        # print average rating
+        print(
+            "Average rating for {firstname} {lastname} is {rating}".format(
+                firstname=author.first_name, lastname=author.last_name, rating=rating
+            )
+        )
+
+
+if __name__ == "__main__":
     db_cfg = {
-        'dbname': "rickdb-bookstore",
-        'user': "rickdb_user",
-        'password': "rickdb_pass",
-        'host': "localhost",
-        'port': 5432,
-        'sslmode': 'require'        
+        "dbname": "rickdb-bookstore",
+        "user": "rickdb_user",
+        "password": "rickdb_pass",
+        "host": "localhost",
+        "port": 5432,
+        "sslmode": "require",
     }
 
     conn = PgConnection(**db_cfg)
     repo = AuthorRepository(conn)
     dump_author_rating(repo)
 ```
```

### Comparing `rick-db-1.1.2/rick_db/cache.py` & `rick-db-1.2.0/rick_db/cache.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/commands/check.py` & `rick-db-1.2.0/rick_db/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/commands/dto.py` & `rick-db-1.2.0/rick_db/cli/commands/dto.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/commands/flatten.py` & `rick-db-1.2.0/rick_db/cli/commands/flatten.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/commands/help.py` & `rick-db-1.2.0/rick_db/cli/commands/help.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/commands/init.py` & `rick-db-1.2.0/rick_db/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/commands/list.py` & `rick-db-1.2.0/rick_db/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/commands/migrate.py` & `rick-db-1.2.0/rick_db/cli/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/config.py` & `rick-db-1.2.0/rick_db/cli/config.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/cli/manage.py` & `rick-db-1.2.0/rick_db/cli/manage.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/conn/connection.py` & `rick-db-1.2.0/rick_db/conn/connection.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/conn/pg/postgres.py` & `rick-db-1.2.0/rick_db/conn/pg/postgres.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/conn/sqlite/sqlite.py` & `rick-db-1.2.0/rick_db/conn/sqlite/sqlite.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/dbgrid.py` & `rick-db-1.2.0/rick_db/dbgrid.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/mapper.py` & `rick-db-1.2.0/rick_db/mapper.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/profiler/profilers.py` & `rick-db-1.2.0/rick_db/profiler/profilers.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/repository.py` & `rick-db-1.2.0/rick_db/repository.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/sql/common.py` & `rick-db-1.2.0/rick_db/sql/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         return self._literal
 
 
 class Sql:
     DISTINCT = "distinct"
     COLUMNS = "columns"
     FROM = "from"
+    LATERAL = "lateral"
     UNION = "union"
     WHERE = "where"
     GROUP = "group"
     HAVING = "having"
     ORDER = "order"
     LIMIT_OFFSET = "limitoffset"
     FOR_UPDATE = "forupdate"
@@ -31,14 +32,17 @@
     JOIN = "JOIN"
     INNER_JOIN = "INNER JOIN"
     LEFT_JOIN = "LEFT JOIN"
     RIGHT_JOIN = "RIGHT JOIN"
     FULL_JOIN = "FULL JOIN"
     CROSS_JOIN = "CROSS JOIN"
     NATURAL_JOIN = "NATURAL JOIN"
+    INNER_JOIN_LATERAL = "INNER JOIN LATERAL"
+    LEFT_JOIN_LATERAL = "LEFT JOIN LATERAL"
+    SQL_LATERAL = "LATERAL"
 
     SQL_WILDCARD = "*"
     SQL_SELECT = "SELECT"
     SQL_UNION = "UNION"
     SQL_UNION_ALL = "UNION ALL"
     SQL_FROM = "FROM"
     SQL_WHERE = "WHERE"
@@ -61,11 +65,15 @@
     SQL_LIST_DELIMITER_LEFT = "("
     SQL_LIST_DELIMITER_RIGHT = ")"
     SQL_ALL = "ALL"
     SQL_DELETE = "DELETE FROM"
     SQL_CASCADE = "CASCADE"
     SQL_UPDATE = "UPDATE"
     SQL_SET = "SET"
+    SQL_WITH = "WITH"
+    SQL_NOT_MATERIALIZED = "NOT MATERIALIZED"
+    SQL_RECURSIVE = "RECURSIVE"
 
 
 class SqlStatement:
-    pass
+    def assemble(self) -> tuple:
+        pass
```

### Comparing `rick-db-1.1.2/rick_db/sql/delete.py` & `rick-db-1.2.0/rick_db/sql/delete.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/sql/dialect.py` & `rick-db-1.2.0/rick_db/sql/dialect.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/sql/insert.py` & `rick-db-1.2.0/rick_db/sql/insert.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/sql/select.py` & `rick-db-1.2.0/rick_db/sql/select.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SQL Query Builder
 #
 # Notes:
 # The Select() implementation is heavily inspired from the Zend_Db_Select approach. You can check the
 # Zend_Db_Select code and licensing at https://github.com/zendframework/zf1/blob/master/library/Zend/Db/Select.php
 
 import collections
+from typing import Union
 
 from .common import SqlStatement, Sql, Literal, SqlError
 from .dialect import SqlDialect, DefaultSqlDialect
 from ..mapper import ATTR_TABLE, ATTR_SCHEMA
 
 
 class Select(SqlStatement):
@@ -30,14 +31,16 @@
     _valid_joins = [
         Sql.INNER_JOIN,
         Sql.LEFT_JOIN,
         Sql.RIGHT_JOIN,
         Sql.FULL_JOIN,
         Sql.CROSS_JOIN,
         Sql.NATURAL_JOIN,
+        Sql.INNER_JOIN_LATERAL,
+        Sql.LEFT_JOIN_LATERAL,
     ]
     _valid_unions = [Sql.SQL_UNION, Sql.SQL_UNION_ALL]
     _valid_order = [Sql.SQL_ASC, Sql.SQL_DESC]
 
     def __init__(self, dialect: SqlDialect = None):
         """
         Constructor
@@ -160,14 +163,31 @@
             .from({class_or_object: "bar"}, ["field1"])  # SELECT "bar"."field1" FROM "<object_table_name>" AS "bar"
         """
         if cols is None or (type(cols) in (list, tuple) and len(cols) == 0):
             cols = Sql.SQL_WILDCARD
 
         return self._join(Sql.FROM, table, None, None, None, None, cols, schema, None)
 
+    def lateral(self, subquery: SqlStatement, alias: str, cols=None):
+        """
+        Adds a LATERAL clause
+        :param subquery: LATERAL subquery expression
+        :param alias: subquery alias
+        :param cols: optional columns to be selected
+        :return: self
+
+        Example:
+            .lateral(Select().from_("users"), "u")  # SELECT
+        """
+        if cols is None or (type(cols) in (list, tuple) and len(cols) == 0):
+            cols = Sql.SQL_WILDCARD
+        return self._join(
+            Sql.LATERAL, {subquery: alias}, None, None, None, None, cols, None, None
+        )
+
     def limit(self, limit: int, offset: int = None):
         """
         LIMIT clause
         :param limit: LIMIT value
         :param offset: OFFSET value
         :return: self
 
@@ -705,14 +725,70 @@
             expr_field,
             operator,
             cols,
             schema,
             expr_schema,
         )
 
+    def join_inner_lateral(
+        self, subquery: Union[SqlStatement, Literal], alias: str, join_expr: Literal
+    ):
+        """
+        Performs a INNER JOIN LATERAL
+        See join() for more information
+
+        :param subquery: subquery
+        :param alias: alias for subquery
+        :param join_expr: Literal for ON clause
+
+        :return: self
+
+        Examples:
+            .join_inner_lateral(Select().from_('product').limit(3), 'prod', Literal('true'))
+        """
+        return self._join(
+            Sql.INNER_JOIN_LATERAL,
+            {subquery: alias},
+            join_expr,
+            None,
+            None,
+            None,
+            None,
+            None,
+            None,
+        )
+
+    def join_left_lateral(
+        self, subquery: Union[SqlStatement, Literal], alias: str, join_expr: Literal
+    ):
+        """
+        Performs a LEFT JOIN LATERAL
+        See join() for more information
+
+        :param subquery: subquery
+        :param alias: alias for subquery
+        :param join_expr: Literal for ON clause
+
+        :return: self
+
+        Examples:
+            .join_left_lateral(Select().from_('product').limit(3), 'prod', Literal('true'))
+        """
+        return self._join(
+            Sql.LEFT_JOIN_LATERAL,
+            {subquery: alias},
+            join_expr,
+            None,
+            None,
+            None,
+            None,
+            None,
+            None,
+        )
+
     def join_cross(self, table, cols=None, schema=None):
         """
         Performs a CROSS JOIN
         See join() for more information
 
         :param table: table to perform join
         :param cols: columns to be selected from the joined table
@@ -856,15 +932,18 @@
         :param from_field: existing table field
         :param operator: operator to use on join_table.expr_or_field <operator> from_table.from_field
         :param cols: columns to select from table schema
         :param schema: joined table schema
         :param from_schema: source table schema
         :return:
         """
-        if join_type not in self._valid_joins and join_type != Sql.FROM:
+        if join_type not in self._valid_joins and join_type not in (
+            Sql.FROM,
+            Sql.LATERAL,
+        ):
             raise SqlError(f"_join(): invalid join type {join_type}")
 
         if len(self._parts_union) > 0:
             raise SqlError("_join(): invalid use of table with union")
 
         # join table
         join_table, alias, schema = self._parse_table_def(join_table, schema)
@@ -929,21 +1008,20 @@
             "tableName": join_table,
             "joinCondition": expression,
             "schema": schema,
         }
 
         # always alias wildcard tables
         has_alias = False
-        if join_type == Sql.FROM:
+        if join_type in (Sql.FROM, Sql.LATERAL):
             has_alias = (join_table != alias) or str(cols) == "*"
         else:
             # in joins, cols are always prefixed by alias
             if cols is not None:
                 has_alias = True
-
         self._add_columns(alias, cols, has_alias)
         return self
 
     def _parse_table_def(self, table, schema):
         """
         Parse a table definition from a parameter
 
@@ -1072,29 +1150,49 @@
         """
         Renders FROM and JOIN clauses
         :return: string
         """
         parts = [Sql.SQL_FROM]
         from_parts = {}
         join_parts = {}
+        lateral_parts = {}
         for alias, details in self._parts_from.items():
             if details["joinType"] == Sql.FROM:
                 from_parts[alias] = details
+            elif details["joinType"] == Sql.LATERAL:
+                lateral_parts[alias] = details
             else:
                 join_parts[alias] = details
 
         # FROM clause
         names = []
         for alias, details in from_parts.items():
             tbl_alias = None
             if alias != details["tableName"]:
                 tbl_alias = alias
             names.append(
                 self._dialect.table(details["tableName"], tbl_alias, details["schema"])
             )
+
+        # LATERAL clause
+        if len(lateral_parts) > 0:
+            for alias, details in lateral_parts.items():
+                tbl_alias = None
+                if alias != details["tableName"]:
+                    tbl_alias = alias
+                names.append(
+                    " ".join(
+                        [
+                            Sql.SQL_LATERAL,
+                            self._dialect.table(details["tableName"], tbl_alias),
+                        ]
+                    )
+                )
+
+        # build FROM, LATERAL
         parts.append(", ".join(names))
 
         # JOIN clauses
         names = []
         for alias, details in join_parts.items():
             stmt = []
             tbl_alias = None
@@ -1187,27 +1285,24 @@
             if isinstance(expr, collections.abc.Mapping):
                 for field, _order in expr.items():
                     stmt.append(self._dialect.field(field))
                     if _order is None:
                         stmt.append(order)
                     else:
                         stmt.append(_order)
+                    parts.append(" ".join(stmt))
             elif isinstance(expr, (list, tuple)):
                 for field in expr:
-                    stmt.append(self._dialect.field(field))
-                    stmt.append(order)
+                    parts.append(" ".join([self._dialect.field(field), order]))
             elif isinstance(expr, Literal):
-                stmt.append(str(expr))
-                stmt.append(order)
+                parts.append(" ".join([str(expr), order]))
             elif isinstance(expr, str):
-                stmt.append(self._dialect.field(expr))
-                stmt.append(order)
+                parts.append(" ".join([self._dialect.field(expr), order]))
             else:
                 raise SqlError("order(): invalid field type: %s" % str(type(expr)))
-            parts.append(" ".join(stmt))
 
         return " ".join([Sql.SQL_ORDER_BY, ",".join(parts)])
 
     def _render_where(self):
         """
         Renders WHERE clause
```

### Comparing `rick-db-1.1.2/rick_db/sql/update.py` & `rick-db-1.2.0/rick_db/sql/update.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/console.py` & `rick-db-1.2.0/rick_db/util/console.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/metadata.py` & `rick-db-1.2.0/rick_db/util/metadata.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/migrations.py` & `rick-db-1.2.0/rick_db/util/migrations.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/pg/metadata.py` & `rick-db-1.2.0/rick_db/util/pg/metadata.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/pg/migrations.py` & `rick-db-1.2.0/rick_db/util/pg/migrations.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/pg/pginfo.py` & `rick-db-1.2.0/rick_db/util/pg/pginfo.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/pg/records.py` & `rick-db-1.2.0/rick_db/util/pg/records.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/sqlite/metadata.py` & `rick-db-1.2.0/rick_db/util/sqlite/metadata.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db/util/sqlite/migrations.py` & `rick-db-1.2.0/rick_db/util/sqlite/migrations.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/rick_db.egg-info/PKG-INFO` & `rick-db-1.2.0/rick_db.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rick-db
-Version: 1.1.2
+Version: 1.2.0
 Summary: SQL database layer
 Home-page: https://git.oddbit.org/OddBit/rick_db
 Author: Joao Pinheiro
 Author-email: 
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,16 +18,17 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-rick_db - Simple SQL database layer
---
+# rick_db - Simple SQL database layer
+
+
 [![Tests](https://github.com/oddbit-project/rick_db/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick_db/actions)
 [![pypi](https://img.shields.io/pypi/v/rick_db.svg)](https://pypi.org/project/rick_db/)
 [![license](https://img.shields.io/pypi/l/rick-db.svg)](https://git.oddbit.org/OddBit/rick_db/src/branch/master/LICENSE)
 
 rick_db is a simple SQL database layer for Python3. It includes connection management, Object Mapper, Query Builder,
 and a Repository pattern implementation. It is **not** an ORM, and it's not meant to replace one. 
 
@@ -59,110 +60,119 @@
 
 ```python
 from rick_db import fieldmapper, Repository
 from rick_db.conn.pg import PgConnection
 from rick_db.sql import Select, Literal
 
 
-@fieldmapper(tablename='publisher', pk='id_publisher')
+@fieldmapper(tablename="publisher", pk="id_publisher")
 class Publisher:
-    id = 'id_publisher'
-    name = 'name'
+    id = "id_publisher"
+    name = "name"
 
 
-@fieldmapper(tablename='book', pk='id_book')
+@fieldmapper(tablename="book", pk="id_book")
 class Book:
-    id = 'id_book'
-    title = 'title'
-    total_pages = 'total_pages'
-    rating = 'rating'
-    isbn = 'isbn'
-    published = 'published_date'
-    fk_publisher = 'fk_publisher'
+    id = "id_book"
+    title = "title"
+    total_pages = "total_pages"
+    rating = "rating"
+    isbn = "isbn"
+    published = "published_date"
+    fk_publisher = "fk_publisher"
 
 
-@fieldmapper(tablename='author', pk='id_author')
+@fieldmapper(tablename="author", pk="id_author")
 class Author:
-    id = 'id_author'
-    first_name = 'first_name'
-    middle_name = 'middle_name'
-    last_name = 'last_name'
+    id = "id_author"
+    first_name = "first_name"
+    middle_name = "middle_name"
+    last_name = "last_name"
 
 
-@fieldmapper(tablename='book_author', pk='id_book_author')
+@fieldmapper(tablename="book_author", pk="id_book_author")
 class BookAuthor:
-    id = 'id_book_author'
-    fk_book = 'fk_book'
-    fk_author = 'fk_author'
+    id = "id_book_author"
+    fk_book = "fk_book"
+    fk_author = "fk_author"
 
 
 class AuthorRepository(Repository):
-
     def __init__(self, db):
         super().__init__(db, Author)
 
     def calc_avg_rating(self, id_author: int):
         """
         Calculate average rating for a given author
         :param id_author: author id
         :return: average rating, if any
         """
-        
+
         # generated query:
-        # SELECT avg(rating) AS "rating" FROM "book" INNER JOIN "book_author" ON 
+        # SELECT avg(rating) AS "rating" FROM "book" INNER JOIN "book_author" ON
         # "book"."id_book"="book_author"."fk_book" WHERE ("fk_author" = %s)
-        qry = Select(self._dialect). \
-            from_(Book, {Literal("avg({})".format(Book.rating)): 'rating'}). \
-            join(BookAuthor, BookAuthor.fk_book, Book, Book.id). \
-            where(BookAuthor.fk_author, '=', id_author)
-        
+        qry = (
+            Select(self._dialect)
+            .from_(Book, {Literal("avg({})".format(Book.rating)): "rating"})
+            .join(BookAuthor, BookAuthor.fk_book, Book, Book.id)
+            .where(BookAuthor.fk_author, "=", id_author)
+        )
+
         # retrieve result as list of type Book (to get the rating field)
         rset = self.fetch(qry, cls=Book)
         if len(rset) > 0:
             return rset.pop(0).rating
         return 0
 
     def books(self, id_author: int) -> list[Book]:
         """
         Retrieve all books for the given author
         :return: list[Book]
         """
-        
-        qry = Select(self._dialect). \
-            from_(Book). \
-            join(BookAuthor, BookAuthor.fk_book, Book, Book.id). \
-            where(BookAuthor.fk_author, '=', id_author)
+
+        qry = (
+            Select(self._dialect)
+            .from_(Book)
+            .join(BookAuthor, BookAuthor.fk_book, Book, Book.id)
+            .where(BookAuthor.fk_author, "=", id_author)
+        )
 
         return self.fetch(qry, cls=Book)
 
 
 def dump_author_rating(repo: AuthorRepository):
     for author in repo.fetch_all():
-        
         # calculate average
         rating = repo.calc_avg_rating(author.id)
-        
+
         # print book list
-        print("Books by {firstname} {lastname}:".format(firstname=author.first_name, lastname=author.last_name))
+        print(
+            "Books by {firstname} {lastname}:".format(
+                firstname=author.first_name, lastname=author.last_name
+            )
+        )
         for book in repo.books(author.id):
             print(book.title)
-        
-        # print average rating           
-        print("Average rating for {firstname} {lastname} is {rating}".
-              format(firstname=author.first_name, lastname=author.last_name, rating=rating))
 
-        
-if __name__ == '__main__':
+        # print average rating
+        print(
+            "Average rating for {firstname} {lastname} is {rating}".format(
+                firstname=author.first_name, lastname=author.last_name, rating=rating
+            )
+        )
+
+
+if __name__ == "__main__":
     db_cfg = {
-        'dbname': "rickdb-bookstore",
-        'user': "rickdb_user",
-        'password': "rickdb_pass",
-        'host': "localhost",
-        'port': 5432,
-        'sslmode': 'require'        
+        "dbname": "rickdb-bookstore",
+        "user": "rickdb_user",
+        "password": "rickdb_pass",
+        "host": "localhost",
+        "port": 5432,
+        "sslmode": "require",
     }
 
     conn = PgConnection(**db_cfg)
     repo = AuthorRepository(conn)
     dump_author_rating(repo)
 ```
```

### Comparing `rick-db-1.1.2/rick_db.egg-info/SOURCES.txt` & `rick-db-1.2.0/rick_db.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 rick_db/profiler/profilers.py
 rick_db/sql/__init__.py
 rick_db/sql/common.py
 rick_db/sql/delete.py
 rick_db/sql/dialect.py
 rick_db/sql/insert.py
 rick_db/sql/select.py
+rick_db/sql/sql_with.py
 rick_db/sql/update.py
 rick_db/util/__init__.py
 rick_db/util/console.py
 rick_db/util/metadata.py
 rick_db/util/migrations.py
 rick_db/util/pg/__init__.py
 rick_db/util/pg/metadata.py
@@ -69,14 +70,15 @@
 tests/conn/sqlite/test_sqlite3.py
 tests/sql/__init__.py
 tests/sql/test_delete.py
 tests/sql/test_dialects.py
 tests/sql/test_insert.py
 tests/sql/test_select.py
 tests/sql/test_update.py
+tests/sql/test_with.py
 tests/util/__init__.py
 tests/util/migrations.py
 tests/util/pg/__init__.py
 tests/util/pg/common.py
 tests/util/pg/test_metadata.py
 tests/util/pg/test_migrations.py
 tests/util/pg/test_pginfo.py
```

### Comparing `rick-db-1.1.2/setup.py` & `rick-db-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/conn/pg/test_postgres.py` & `rick-db-1.2.0/tests/conn/pg/test_postgres.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/conn/sqlite/test_sqlite3.py` & `rick-db-1.2.0/tests/conn/sqlite/test_sqlite3.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/dbgrid.py` & `rick-db-1.2.0/tests/dbgrid.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/repository.py` & `rick-db-1.2.0/tests/repository.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/sql/test_delete.py` & `rick-db-1.2.0/tests/sql/test_delete.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/sql/test_dialects.py` & `rick-db-1.2.0/tests/sql/test_dialects.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/sql/test_insert.py` & `rick-db-1.2.0/tests/sql/test_insert.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/sql/test_select.py` & `rick-db-1.2.0/tests/sql/test_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 from rick_db import fieldmapper
-from rick_db.sql import Select, SqlError, Literal, PgSqlDialect
+from rick_db.sql import Select, SqlError, Literal, PgSqlDialect, Sql
 
 TABLE_NAME = "test_table"
 
 
 @fieldmapper(tablename="test_table")
 class SomeTable:
     field = "field"
@@ -375,23 +375,23 @@
 
 
 @pytest.mark.parametrize(
     "join_table, expr_or_field, expr_table, expr_field, operator, cols, schema, join_schema, result",
     join_noalias_cases,
 )
 def test_noalias_join(
-    join_table,
-    expr_or_field,
-    expr_table,
-    expr_field,
-    operator,
-    cols,
-    schema,
-    join_schema,
-    result,
+        join_table,
+        expr_or_field,
+        expr_table,
+        expr_field,
+        operator,
+        cols,
+        schema,
+        join_schema,
+        result,
 ):
     sql, _ = (
         Select()
         .from_(TABLE_NAME, "*")
         .join(
             join_table,
             expr_or_field,
@@ -408,23 +408,23 @@
 
 
 @pytest.mark.parametrize(
     "join_table, expr_or_field, expr_table, expr_field, operator, cols, schema, join_schema, result",
     join_alias_cases,
 )
 def test_alias_join(
-    join_table,
-    expr_or_field,
-    expr_table,
-    expr_field,
-    operator,
-    cols,
-    schema,
-    join_schema,
-    result,
+        join_table,
+        expr_or_field,
+        expr_table,
+        expr_field,
+        operator,
+        cols,
+        schema,
+        join_schema,
+        result,
 ):
     sql, _ = (
         Select()
         .from_({TABLE_NAME: "t1"}, "*")
         .join(
             join_table,
             expr_or_field,
@@ -441,23 +441,23 @@
 
 
 @pytest.mark.parametrize(
     "join_table, expr_or_field, expr_table, expr_field, operator, cols, schema, join_schema, result",
     join_noalias_cases,
 )
 def test_noalias_join_left(
-    join_table,
-    expr_or_field,
-    expr_table,
-    expr_field,
-    operator,
-    cols,
-    schema,
-    join_schema,
-    result,
+        join_table,
+        expr_or_field,
+        expr_table,
+        expr_field,
+        operator,
+        cols,
+        schema,
+        join_schema,
+        result,
 ):
     result = result.replace("INNER", "LEFT")
     sql, _ = (
         Select()
         .from_(TABLE_NAME, "*")
         .join_left(
             join_table,
@@ -475,23 +475,23 @@
 
 
 @pytest.mark.parametrize(
     "join_table, expr_or_field, expr_table, expr_field, operator, cols, schema, join_schema, result",
     join_alias_cases,
 )
 def test_alias_join_left(
-    join_table,
-    expr_or_field,
-    expr_table,
-    expr_field,
-    operator,
-    cols,
-    schema,
-    join_schema,
-    result,
+        join_table,
+        expr_or_field,
+        expr_table,
+        expr_field,
+        operator,
+        cols,
+        schema,
+        join_schema,
+        result,
 ):
     result = result.replace("INNER", "LEFT")
     sql, _ = (
         Select()
         .from_({TABLE_NAME: "t1"}, "*")
         .join_left(
             join_table,
@@ -509,23 +509,23 @@
 
 
 @pytest.mark.parametrize(
     "join_table, expr_or_field, expr_table, expr_field, operator, cols, schema, join_schema, result",
     join_noalias_cases,
 )
 def test_noalias_join_right(
-    join_table,
-    expr_or_field,
-    expr_table,
-    expr_field,
-    operator,
-    cols,
-    schema,
-    join_schema,
-    result,
+        join_table,
+        expr_or_field,
+        expr_table,
+        expr_field,
+        operator,
+        cols,
+        schema,
+        join_schema,
+        result,
 ):
     result = result.replace("INNER", "RIGHT")
     sql, _ = (
         Select()
         .from_(TABLE_NAME, "*")
         .join_right(
             join_table,
@@ -543,23 +543,23 @@
 
 
 @pytest.mark.parametrize(
     "join_table, expr_or_field, expr_table, expr_field, operator, cols, schema, join_schema, result",
     join_alias_cases,
 )
 def test_alias_join_right(
-    join_table,
-    expr_or_field,
-    expr_table,
-    expr_field,
-    operator,
-    cols,
-    schema,
-    join_schema,
-    result,
+        join_table,
+        expr_or_field,
+        expr_table,
+        expr_field,
+        operator,
+        cols,
+        schema,
+        join_schema,
+        result,
 ):
     result = result.replace("INNER", "RIGHT")
     sql, _ = (
         Select()
         .from_({TABLE_NAME: "t1"}, "*")
         .join_right(
             join_table,
@@ -577,23 +577,23 @@
 
 
 @pytest.mark.parametrize(
     "join_table, expr_or_field, expr_table, expr_field, operator, cols, schema, join_schema, result",
     join_noalias_cases,
 )
 def test_noalias_join_full(
-    join_table,
-    expr_or_field,
-    expr_table,
-    expr_field,
-    operator,
-    cols,
-    schema,
-    join_schema,
-    result,
+        join_table,
+        expr_or_field,
+        expr_table,
+        expr_field,
+        operator,
+        cols,
+        schema,
+        join_schema,
+        result,
 ):
     result = result.replace("INNER", "FULL")
     sql, _ = (
         Select()
         .from_(TABLE_NAME, "*")
         .join_full(
             join_table,
@@ -611,23 +611,23 @@
 
 
 @pytest.mark.parametrize(
     "join_table, expr_or_field, expr_table, expr_field, operator, cols, schema, join_schema, result",
     join_alias_cases,
 )
 def test_alias_join_full(
-    join_table,
-    expr_or_field,
-    expr_table,
-    expr_field,
-    operator,
-    cols,
-    schema,
-    join_schema,
-    result,
+        join_table,
+        expr_or_field,
+        expr_table,
+        expr_field,
+        operator,
+        cols,
+        schema,
+        join_schema,
+        result,
 ):
     result = result.replace("INNER", "FULL")
     sql, _ = (
         Select()
         .from_({TABLE_NAME: "t1"}, "*")
         .join_full(
             join_table,
@@ -1116,16 +1116,16 @@
         [
             Select(PgSqlDialect()).from_(SomeTable),
             Select(PgSqlDialect()).from_(SchemaTestTable),
         ]
     )
     sql, _ = qry_union.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" UNION SELECT "other_table".* FROM "public"."other_table"'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" UNION SELECT "other_table".* FROM "public"."other_table"'
     )
 
 
 # Select:where_and() -----------------------------------------------------------------------------------------------
 
 
 def test_where_and():
@@ -1137,16 +1137,16 @@
         .where("field1", "=", 1)
         .where("field2", "=", 2)
         .where_end()
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) )'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) )'
     )
     assert values == [1, 2]
 
     # AND group and parameter
     qry = (
         Select(PgSqlDialect())
         .from_(SomeTable)
@@ -1155,17 +1155,17 @@
         .where("field1", "=", 1)
         .where("field2", "=", 2)
         .where_end()
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ("field3" = %s) AND ( ("field1" = %s) AND ("field2" '
-        "= %s) )"
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ("field3" = %s) AND ( ("field1" = %s) AND ("field2" '
+               "= %s) )"
     )
     assert values == [3, 1, 2]
 
     # AND group and two parameters
     qry = (
         Select(PgSqlDialect())
         .from_(SomeTable)
@@ -1175,17 +1175,17 @@
         .where("field2", "=", 2)
         .where_end()
         .where("field4", "=", 4)
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ("field3" = %s) AND ( ("field1" = %s) AND ("field2" '
-        '= %s) ) AND ("field4" = %s)'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ("field3" = %s) AND ( ("field1" = %s) AND ("field2" '
+               '= %s) ) AND ("field4" = %s)'
     )
     assert values == [3, 1, 2, 4]
 
     # nested AND group
     qry = (
         Select(PgSqlDialect())
         .from_(SomeTable)
@@ -1198,17 +1198,17 @@
         .where("field4", "=", 4)
         .where_end()
         .where("field5", "=", 5)
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ( ("field2" = %s) OR ("field3" '
-        '= %s) ) AND ("field4" = %s) ) AND ("field5" = %s)'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ( ("field2" = %s) OR ("field3" '
+               '= %s) ) AND ("field4" = %s) ) AND ("field5" = %s)'
     )
     assert values == [1, 2, 3, 4, 5]
 
     # Two AND groups
     qry = (
         Select(PgSqlDialect())
         .from_(SomeTable)
@@ -1220,17 +1220,17 @@
         .where("field3", "=", 3)
         .orwhere("field4", "=", 4)
         .where_end()
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) ) AND ( ('
-        '"field3" = %s) OR ("field4" = %s) )'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) ) AND ( ('
+               '"field3" = %s) OR ("field4" = %s) )'
     )
     assert values == [1, 2, 3, 4]
 
 
 def test_where_or():
     # test with OR group in the beginning
     qry = (
@@ -1240,16 +1240,16 @@
         .where("field1", "=", 1)
         .where("field2", "=", 2)
         .where_end()
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) )'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) )'
     )
     assert values == [1, 2]
 
     # OR group and parameter
     qry = (
         Select(PgSqlDialect())
         .from_(SomeTable)
@@ -1258,17 +1258,17 @@
         .where("field1", "=", 1)
         .where("field2", "=", 2)
         .where_end()
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ("field3" = %s) OR ( ("field1" = %s) AND ("field2" = '
-        "%s) )"
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ("field3" = %s) OR ( ("field1" = %s) AND ("field2" = '
+               "%s) )"
     )
     assert values == [3, 1, 2]
 
     # OR group and two parameters
     qry = (
         Select(PgSqlDialect())
         .from_(SomeTable)
@@ -1278,17 +1278,17 @@
         .where("field2", "=", 2)
         .where_end()
         .where("field4", "=", 4)
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ("field3" = %s) OR ( ("field1" = %s) AND ("field2" = '
-        '%s) ) AND ("field4" = %s)'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ("field3" = %s) OR ( ("field1" = %s) AND ("field2" = '
+               '%s) ) AND ("field4" = %s)'
     )
     assert values == [3, 1, 2, 4]
 
     # nested OR group
     qry = (
         Select(PgSqlDialect())
         .from_(SomeTable)
@@ -1301,17 +1301,17 @@
         .where("field4", "=", 4)
         .where_end()
         .where("field5", "=", 5)
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) OR ( ("field2" = %s) OR ("field3" '
-        '= %s) ) AND ("field4" = %s) ) AND ("field5" = %s)'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) OR ( ("field2" = %s) OR ("field3" '
+               '= %s) ) AND ("field4" = %s) ) AND ("field5" = %s)'
     )
     assert values == [1, 2, 3, 4, 5]
 
     # Two OR groups
     qry = (
         Select(PgSqlDialect())
         .from_(SomeTable)
@@ -1323,17 +1323,17 @@
         .where("field3", "=", 3)
         .orwhere("field4", "=", 4)
         .where_end()
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) ) OR ( ('
-        '"field3" = %s) OR ("field4" = %s) )'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) ) OR ( ('
+               '"field3" = %s) OR ("field4" = %s) )'
     )
     assert values == [1, 2, 3, 4]
 
 
 def test_where_and_or():
     # test with both AND and OR groups
     qry = (
@@ -1347,12 +1347,91 @@
         .where("field3", "=", 3)
         .where("field4", "=", 4)
         .where_end()
     )
 
     sql, values = qry.assemble()
     assert (
-        sql
-        == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) ) OR ( ('
-        '"field3" = %s) AND ("field4" = %s) )'
+            sql
+            == 'SELECT "test_table".* FROM "test_table" WHERE ( ("field1" = %s) AND ("field2" = %s) ) OR ( ('
+               '"field3" = %s) AND ("field4" = %s) )'
     )
     assert values == [1, 2, 3, 4]
+
+
+# Select:join_left_lateral() --------------------------------------------------------------------------------------------
+
+join_lateral = [
+    [
+        {"t_wishlist": "w"},
+        Select(PgSqlDialect()).from_({"t_product": "p"}).where("price", "<", "desired_price").order("price",
+                                                                                                    Sql.SQL_DESC).limit(
+            3),
+        "x",
+        Literal("true"),
+        'SELECT "w".* FROM "t_wishlist" AS "w" LEFT JOIN LATERAL (SELECT "p".* FROM "t_product" AS "p" WHERE ("price" < %s) ORDER BY "price" DESC LIMIT 3) AS "x" ON (true)',
+    ],
+]
+
+from_lateral = [
+    [
+        {"t_wishlist": "w"},
+        Select(PgSqlDialect()).from_({"t_product": "p"}).where("price", "<", "desired_price").order("price",
+                                                                                                    Sql.SQL_DESC).limit(3),
+        "x",
+        'SELECT "w".*,"x".* FROM "t_wishlist" AS "w", LATERAL (SELECT "p".* FROM "t_product" AS "p" WHERE ("price" < %s) ORDER BY "price" DESC LIMIT 3) AS "x"'
+    ]
+]
+
+
+@pytest.mark.parametrize("table, subquery, alias, join_expr,result", join_lateral)
+def test_join_left_lateral(
+        table,
+        subquery,
+        alias,
+        join_expr,
+        result,
+):
+    sql, _ = (
+        Select()
+        .from_(table)
+        .join_left_lateral(subquery, alias, join_expr)
+        .assemble()
+    )
+    assert sql == result
+
+# Select:join_inner_lateral() ------------------------------------------------------------------------------------------
+
+@pytest.mark.parametrize("table, subquery, alias, join_expr,result", join_lateral)
+def test_join_inner_lateral(
+        table,
+        subquery,
+        alias,
+        join_expr,
+        result,
+):
+    result = result.replace("LEFT", "INNER")
+    sql, _ = (
+        Select()
+        .from_(table)
+        .join_inner_lateral(subquery, alias, join_expr)
+        .assemble()
+    )
+    assert sql == result
+
+
+# Select:lateral() ------------------------------------------------------------------------------------------
+
+@pytest.mark.parametrize("table, subquery, alias, result", from_lateral)
+def test_from_lateral(
+        table,
+        subquery,
+        alias,
+        result,
+):
+    sql, _ = (
+        Select()
+        .from_(table)
+        .lateral(subquery, alias)
+        .assemble()
+    )
+    assert sql == result
```

### Comparing `rick-db-1.1.2/tests/sql/test_update.py` & `rick-db-1.2.0/tests/sql/test_update.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/test_pgsql_dbgrid.py` & `rick-db-1.2.0/tests/test_pgsql_dbgrid.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/test_pgsql_repository.py` & `rick-db-1.2.0/tests/test_pgsql_repository.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/test_record.py` & `rick-db-1.2.0/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/test_sqlite_dbgrid.py` & `rick-db-1.2.0/tests/test_sqlite_dbgrid.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/test_sqlite_repository.py` & `rick-db-1.2.0/tests/test_sqlite_repository.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/util/migrations.py` & `rick-db-1.2.0/tests/util/migrations.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/util/pg/common.py` & `rick-db-1.2.0/tests/util/pg/common.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/util/pg/test_metadata.py` & `rick-db-1.2.0/tests/util/pg/test_metadata.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/util/pg/test_pginfo.py` & `rick-db-1.2.0/tests/util/pg/test_pginfo.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/util/sqlite/test_metadata.py` & `rick-db-1.2.0/tests/util/sqlite/test_metadata.py`

 * *Files identical despite different names*

### Comparing `rick-db-1.1.2/tests/util/sqlite/test_migrations.py` & `rick-db-1.2.0/tests/util/sqlite/test_migrations.py`

 * *Files identical despite different names*

