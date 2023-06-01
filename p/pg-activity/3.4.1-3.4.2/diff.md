# Comparing `tmp/pg-activity-3.4.1.tar.gz` & `tmp/pg-activity-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg-activity-3.4.1.tar", last modified: Tue May 30 07:20:56 2023, max compression
+gzip compressed data, was "pg-activity-3.4.2.tar", last modified: Thu Jun  1 13:26:25 2023, max compression
```

## Comparing `pg-activity-3.4.1.tar` & `pg-activity-3.4.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.130953 pg-activity-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 07:20:42.000000 pg-activity-3.4.1/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 07:20:42.000000 pg-activity-3.4.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 07:20:42.000000 pg-activity-3.4.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-30 07:20:42.000000 pg-activity-3.4.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-30 07:20:42.000000 pg-activity-3.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    13753 2023-05-30 07:20:42.000000 pg-activity-3.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-30 07:20:42.000000 pg-activity-3.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 07:20:42.000000 pg-activity-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-30 07:20:56.130953 pg-activity-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-30 07:20:42.000000 pg-activity-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-30 07:20:42.000000 pg-activity-3.4.1/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.102953 pg-activity-3.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.110953 pg-activity-3.4.1/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/imgs/logo-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/imgs/logo-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/imgs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   337072 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/imgs/screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.114953 pg-activity-3.4.1/docs/man/
--rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/man/build-man.sh
--rw-r--r--   0 runner    (1001) docker     (123)    27465 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/man/pg_activity.1
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/man/pg_activity.pod
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-30 07:20:42.000000 pg-activity-3.4.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.114953 pg-activity-3.4.1/pg_activity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.118953 pg-activity-3.4.1/pgactivity/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/activities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11203 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/pg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.130953 pg-activity-3.4.1/pgactivity/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/disable_log_min_duration_sample.sql
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/disable_log_min_duration_statement.sql
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/do_pg_cancel_backend.sql
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/do_pg_terminate_backend.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_blocking_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_blocking_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_blocking_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_data_directory.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_100000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_110000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_130000.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pga_inet_addresses.sql
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_replication_slots_post_140000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090400.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_100000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_110000.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_temporary_files_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_090500.sql
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_120000.sql
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_version.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_waiting_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_waiting_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_wal_receivers_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_wal_senders_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/reset_statement_timeout.sql
--rw-r--r--   0 runner    (1001) docker     (123)    30898 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19014 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 07:20:56.130953 pg-activity-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 07:20:42.000000 pg-activity-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.130953 pg-activity-3.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.130953 pg-activity-3.4.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    62239 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/data/local-processes-input.json
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_scroll.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    40923 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_ui.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    24193 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_views.txt
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_widgets.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.761099 pg-activity-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 13:26:06.000000 pg-activity-3.4.2/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 13:26:06.000000 pg-activity-3.4.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 13:26:06.000000 pg-activity-3.4.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-01 13:26:06.000000 pg-activity-3.4.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-01 13:26:06.000000 pg-activity-3.4.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-06-01 13:26:06.000000 pg-activity-3.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-01 13:26:06.000000 pg-activity-3.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-01 13:26:06.000000 pg-activity-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-06-01 13:26:25.761099 pg-activity-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-06-01 13:26:06.000000 pg-activity-3.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-01 13:26:06.000000 pg-activity-3.4.2/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.741098 pg-activity-3.4.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.745098 pg-activity-3.4.2/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-06-01 13:26:06.000000 pg-activity-3.4.2/docs/imgs/logo-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-01 13:26:06.000000 pg-activity-3.4.2/docs/imgs/logo-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-01 13:26:06.000000 pg-activity-3.4.2/docs/imgs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   337072 2023-06-01 13:26:06.000000 pg-activity-3.4.2/docs/imgs/screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.745098 pg-activity-3.4.2/docs/man/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-06-01 13:26:06.000000 pg-activity-3.4.2/docs/man/build-man.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    27465 2023-06-01 13:26:06.000000 pg-activity-3.4.2/docs/man/pg_activity.1
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-06-01 13:26:06.000000 pg-activity-3.4.2/docs/man/pg_activity.pod
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-01 13:26:06.000000 pg-activity-3.4.2/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.745098 pg-activity-3.4.2/pg_activity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-06-01 13:26:25.000000 pg-activity-3.4.2/pg_activity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-01 13:26:25.000000 pg-activity-3.4.2/pg_activity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:26:25.000000 pg-activity-3.4.2/pg_activity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 13:26:25.000000 pg-activity-3.4.2/pg_activity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-01 13:26:25.000000 pg-activity-3.4.2/pg_activity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 13:26:25.000000 pg-activity-3.4.2/pg_activity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.749099 pg-activity-3.4.2/pgactivity/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/activities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11203 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/pg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.757099 pg-activity-3.4.2/pgactivity/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/disable_log_min_duration_sample.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/disable_log_min_duration_statement.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/do_pg_cancel_backend.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/do_pg_terminate_backend.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_blocking_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_blocking_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_blocking_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_data_directory.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_pg_activity_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_100000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_110000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_130000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_pga_inet_addresses.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_replication_slots_post_140000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_server_info_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_server_info_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_server_info_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_server_info_post_090400.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_server_info_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_server_info_post_100000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_server_info_post_110000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_temporary_files_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_temporary_files_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_temporary_files_post_090500.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_temporary_files_post_120000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_version.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_waiting_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_waiting_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_wal_receivers_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/get_wal_senders_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/queries/reset_statement_timeout.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    30898 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19014 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pgactivity/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 13:26:06.000000 pg-activity-3.4.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:26:25.761099 pg-activity-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:26:06.000000 pg-activity-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.761099 pg-activity-3.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:26:25.761099 pg-activity-3.4.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    62239 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/data/local-processes-input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_scroll.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40923 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_ui.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24193 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_views.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tests/test_widgets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-01 13:26:06.000000 pg-activity-3.4.2/tox.ini
```

### Comparing `pg-activity-3.4.1/AUTHORS.md` & `pg-activity-3.4.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/CHANGELOG.md` & `pg-activity-3.4.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Change log
 
+## pg\_activity 3.4.2 - 2023-06-01
+
+### Fixed
+
+* Fix package installation by not installing `tests` and `docs` directories
+  (#378).
+
 ## pg\_activity 3.4.1 - 2023-05-30
 
 ### Fixed
 
 * Add more compatibility for old attr versions (#376).
 
 ## pg\_activity 3.4.0 - 2023-05-15
```

### Comparing `pg-activity-3.4.1/LICENSE.txt` & `pg-activity-3.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/PKG-INFO` & `pg-activity-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-activity
-Version: 3.4.1
+Version: 3.4.2
 Summary: Command line tool for PostgreSQL server activity monitoring.
 Author-email: Julien Tachoires <julmon@gmail.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>, Denis Laxalde <denis.laxalde@dalibo.com>, Dalibo <contact@dalibo.com>
 Maintainer-email: Denis Laxalde <denis.laxalde@dalibo.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>
 License: PostgreSQL
 Project-URL: Bug Tracker, https://github.com/dalibo/pg_activity/issues/
 Project-URL: Changelog, https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/dalibo/pg_activity
```

### Comparing `pg-activity-3.4.1/README.md` & `pg-activity-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/RELEASE.md` & `pg-activity-3.4.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/docs/imgs/logo-horizontal.png` & `pg-activity-3.4.2/docs/imgs/logo-horizontal.png`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/docs/imgs/logo-horizontal.svg` & `pg-activity-3.4.2/docs/imgs/logo-horizontal.svg`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/docs/imgs/logo.svg` & `pg-activity-3.4.2/docs/imgs/logo.svg`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/docs/imgs/screenshot.png` & `pg-activity-3.4.2/docs/imgs/screenshot.png`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/docs/man/pg_activity.1` & `pg-activity-3.4.2/docs/man/pg_activity.1`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 .    ds ae ae
 .    ds Ae AE
 .\}
 .rm #[ #] #H #V #F C
 .\" ========================================================================
 .\"
 .IX Title "PG_ACTIVITY 1"
-.TH PG_ACTIVITY 1 "2023-05-30" "pg_activity 3.4.1" "Command line tool for PostgreSQL server activity monitoring."
+.TH PG_ACTIVITY 1 "2023-06-01" "pg_activity 3.4.2" "Command line tool for PostgreSQL server activity monitoring."
 .\" For nroff, turn off justification.  Always turn off hyphenation; it makes
 .\" way too many mistakes in technical documents.
 .if n .ad l
 .nh
 .SH "NAME"
 pg_activity \- Realtime PostgreSQL database server monitoring tool
 .SH "SYNOPSIS"
```

### Comparing `pg-activity-3.4.1/docs/man/pg_activity.pod` & `pg-activity-3.4.2/docs/man/pg_activity.pod`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pg_activity.egg-info/PKG-INFO` & `pg-activity-3.4.2/pg_activity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-activity
-Version: 3.4.1
+Version: 3.4.2
 Summary: Command line tool for PostgreSQL server activity monitoring.
 Author-email: Julien Tachoires <julmon@gmail.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>, Denis Laxalde <denis.laxalde@dalibo.com>, Dalibo <contact@dalibo.com>
 Maintainer-email: Denis Laxalde <denis.laxalde@dalibo.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>
 License: PostgreSQL
 Project-URL: Bug Tracker, https://github.com/dalibo/pg_activity/issues/
 Project-URL: Changelog, https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/dalibo/pg_activity
```

### Comparing `pg-activity-3.4.1/pg_activity.egg-info/SOURCES.txt` & `pg-activity-3.4.2/pg_activity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/activities.py` & `pg-activity-3.4.2/pgactivity/activities.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/cli.py` & `pg-activity-3.4.2/pgactivity/cli.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/colors.py` & `pg-activity-3.4.2/pgactivity/colors.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/compat.py` & `pg-activity-3.4.2/pgactivity/compat.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/config.py` & `pg-activity-3.4.2/pgactivity/config.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/data.py` & `pg-activity-3.4.2/pgactivity/data.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/handlers.py` & `pg-activity-3.4.2/pgactivity/handlers.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/keys.py` & `pg-activity-3.4.2/pgactivity/keys.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/pg.py` & `pg-activity-3.4.2/pgactivity/pg.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_blocking_oldest.sql` & `pg-activity-3.4.2/pgactivity/queries/get_blocking_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_blocking_post_090200.sql` & `pg-activity-3.4.2/pgactivity/queries/get_blocking_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_blocking_post_090600.sql` & `pg-activity-3.4.2/pgactivity/queries/get_blocking_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_oldest.sql` & `pg-activity-3.4.2/pgactivity/queries/get_pg_activity_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_090200.sql` & `pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_090600.sql` & `pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_100000.sql` & `pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_100000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_110000.sql` & `pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_110000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_130000.sql` & `pg-activity-3.4.2/pgactivity/queries/get_pg_activity_post_130000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_server_info_oldest.sql` & `pg-activity-3.4.2/pgactivity/queries/get_server_info_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090100.sql` & `pg-activity-3.4.2/pgactivity/queries/get_server_info_post_090100.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090200.sql` & `pg-activity-3.4.2/pgactivity/queries/get_server_info_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090400.sql` & `pg-activity-3.4.2/pgactivity/queries/get_server_info_post_090400.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090600.sql` & `pg-activity-3.4.2/pgactivity/queries/get_server_info_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_100000.sql` & `pg-activity-3.4.2/pgactivity/queries/get_server_info_post_100000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_110000.sql` & `pg-activity-3.4.2/pgactivity/queries/get_server_info_post_110000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_temporary_files_oldest.sql` & `pg-activity-3.4.2/pgactivity/queries/get_temporary_files_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_090100.sql` & `pg-activity-3.4.2/pgactivity/queries/get_temporary_files_post_090100.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_090500.sql` & `pg-activity-3.4.2/pgactivity/queries/get_temporary_files_post_090500.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_waiting_oldest.sql` & `pg-activity-3.4.2/pgactivity/queries/get_waiting_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/queries/get_waiting_post_090200.sql` & `pg-activity-3.4.2/pgactivity/queries/get_waiting_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/types.py` & `pg-activity-3.4.2/pgactivity/types.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/ui.py` & `pg-activity-3.4.2/pgactivity/ui.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/utils.py` & `pg-activity-3.4.2/pgactivity/utils.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/views.py` & `pg-activity-3.4.2/pgactivity/views.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pgactivity/widgets.py` & `pg-activity-3.4.2/pgactivity/widgets.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/pyproject.toml` & `pg-activity-3.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 Changelog = "https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md"
 Homepage = "https://github.com/dalibo/pg_activity"
 "Source code" = "https://github.com/dalibo/pg_activity/"
 
 [tool.setuptools.dynamic]
 version = { attr = "pgactivity.__version__" }
 
-[tool.setuptools.packages.find]
-where = ["."]
+[tool.setuptools]
+packages = ["pgactivity"]
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
 exclude = '''
 (
   /(
```

### Comparing `pg-activity-3.4.1/tests/conftest.py` & `pg-activity-3.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/data/local-processes-input.json` & `pg-activity-3.4.2/tests/data/local-processes-input.json`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/test_activities.py` & `pg-activity-3.4.2/tests/test_activities.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/test_config.py` & `pg-activity-3.4.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/test_data.py` & `pg-activity-3.4.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/test_scroll.txt` & `pg-activity-3.4.2/tests/test_scroll.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/test_ui.txt` & `pg-activity-3.4.2/tests/test_ui.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/test_views.py` & `pg-activity-3.4.2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/test_views.txt` & `pg-activity-3.4.2/tests/test_views.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tests/test_widgets.txt` & `pg-activity-3.4.2/tests/test_widgets.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.1/tox.ini` & `pg-activity-3.4.2/tox.ini`

 * *Files identical despite different names*

