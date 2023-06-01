# Comparing `tmp/etos_lib-2.1.0.tar.gz` & `tmp/etos_lib-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/etos_lib-2.1.0.tar", last modified: Thu Jan 20 08:41:05 2022, max compression
+gzip compressed data, was "etos_lib-2.2.0.tar", last modified: Thu Jun  1 07:05:41 2023, max compression
```

## Comparing `etos_lib-2.1.0.tar` & `etos_lib-2.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.650151 etos_lib-2.1.0/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2020-10-07 11:22:57.000000 etos_lib-2.1.0/.coveragerc
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.642151 etos_lib-2.1.0/.github/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.642151 etos_lib-2.1.0/.github/workflows/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2021-10-29 10:11:43.000000 etos_lib-2.1.0/.github/workflows/main.yml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      536 2021-10-29 10:11:43.000000 etos_lib-2.1.0/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2020-10-07 11:22:57.000000 etos_lib-2.1.0/AUTHORS.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2020-12-16 05:35:39.000000 etos_lib-2.1.0/CODEOWNERS
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2020-10-07 11:22:57.000000 etos_lib-2.1.0/LICENSE.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1565 2022-01-20 08:41:05.650151 etos_lib-2.1.0/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2020-12-16 05:35:39.000000 etos_lib-2.1.0/README.rst
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.646151 etos_lib-2.1.0/docs/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/Makefile
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.646151 etos_lib-2.1.0/docs/_static/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/_static/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/authors.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/changelog.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     9179 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/conf.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/index.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/license.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/readme.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2020-10-07 11:22:57.000000 etos_lib-2.1.0/docs/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      177 2022-01-20 06:30:24.000000 etos_lib-2.1.0/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1473 2022-01-20 08:41:05.650151 etos_lib-2.1.0/setup.cfg
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2020-10-07 11:22:57.000000 etos_lib-2.1.0/setup.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.642151 etos_lib-2.1.0/src/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.646151 etos_lib-2.1.0/src/etos_lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2020-10-07 11:22:57.000000 etos_lib-2.1.0/src/etos_lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5386 2021-10-13 09:45:08.000000 etos_lib-2.1.0/src/etos_lib/etos.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.646151 etos_lib-2.1.0/src/etos_lib/graphql/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2020-10-07 11:22:57.000000 etos_lib-2.1.0/src/etos_lib/graphql/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2692 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/graphql/query_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.646151 etos_lib-2.1.0/src/etos_lib/kubernetes/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2020-10-07 11:22:57.000000 etos_lib-2.1.0/src/etos_lib/kubernetes/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3355 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/kubernetes/base.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3294 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/kubernetes/jobs.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.650151 etos_lib-2.1.0/src/etos_lib/lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2020-10-07 11:22:57.000000 etos_lib-2.1.0/src/etos_lib/lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2152 2020-10-07 11:22:57.000000 etos_lib-2.1.0/src/etos_lib/lib/auth.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3999 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/lib/config.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2020-10-07 11:22:57.000000 etos_lib-2.1.0/src/etos_lib/lib/database.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5140 2021-10-29 10:30:11.000000 etos_lib-2.1.0/src/etos_lib/lib/debug.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    15853 2022-01-20 06:29:24.000000 etos_lib-2.1.0/src/etos_lib/lib/events.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2020-10-07 11:22:57.000000 etos_lib-2.1.0/src/etos_lib/lib/exceptions.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      809 2022-01-20 06:29:58.000000 etos_lib-2.1.0/src/etos_lib/lib/feature_flags.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4331 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/lib/http.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/lib/monitor.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2632 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/lib/secrets.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/lib/utils.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.650151 etos_lib-2.1.0/src/etos_lib/logging/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2020-12-16 09:06:15.000000 etos_lib-2.1.0/src/etos_lib/logging/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2021-01-11 09:55:23.000000 etos_lib-2.1.0/src/etos_lib/logging/default_config.yaml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2021-01-11 11:40:00.000000 etos_lib-2.1.0/src/etos_lib/logging/filter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/logging/formatter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5506 2021-10-29 10:11:43.000000 etos_lib-2.1.0/src/etos_lib/logging/logger.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.646151 etos_lib-2.1.0/src/etos_lib.egg-info/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1565 2022-01-20 08:41:05.000000 etos_lib-2.1.0/src/etos_lib.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1290 2022-01-20 08:41:05.000000 etos_lib-2.1.0/src/etos_lib.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2022-01-20 08:41:05.000000 etos_lib-2.1.0/src/etos_lib.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2020-12-16 09:45:22.000000 etos_lib-2.1.0/src/etos_lib.egg-info/not-zip-safe
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      185 2022-01-20 08:41:05.000000 etos_lib-2.1.0/src/etos_lib.egg-info/requires.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2022-01-20 08:41:05.000000 etos_lib-2.1.0/src/etos_lib.egg-info/top_level.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2020-10-07 11:22:57.000000 etos_lib-2.1.0/test-requirements.txt
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2022-01-20 08:41:05.650151 etos_lib-2.1.0/tests/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2020-10-07 11:22:57.000000 etos_lib-2.1.0/tests/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2020-10-07 11:22:57.000000 etos_lib-2.1.0/tests/conftest.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2020-10-07 11:22:57.000000 etos_lib-2.1.0/tox.ini
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.230867 etos_lib-2.2.0/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2023-03-09 08:23:58.000000 etos_lib-2.2.0/.coveragerc
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.222868 etos_lib-2.2.0/.github/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/.github/workflows/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-03-09 08:23:58.000000 etos_lib-2.2.0/.github/workflows/main.yml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      536 2023-06-01 07:05:22.000000 etos_lib-2.2.0/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-03-09 08:23:58.000000 etos_lib-2.2.0/AUTHORS.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-03-09 08:23:58.000000 etos_lib-2.2.0/CODEOWNERS
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-03-09 08:23:58.000000 etos_lib-2.2.0/LICENSE.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-01 07:05:41.230867 etos_lib-2.2.0/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2023-03-09 08:23:58.000000 etos_lib-2.2.0/README.rst
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/docs/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/Makefile
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/docs/_static/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/_static/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/authors.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/changelog.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     9175 2023-05-31 11:37:56.000000 etos_lib-2.2.0/docs/conf.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/index.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/license.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/readme.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      177 2023-06-01 07:05:22.000000 etos_lib-2.2.0/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1473 2023-06-01 07:05:41.230867 etos_lib-2.2.0/setup.cfg
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2023-03-09 08:23:58.000000 etos_lib-2.2.0/setup.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.222868 etos_lib-2.2.0/src/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     5386 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/etos.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib/graphql/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/graphql/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2692 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/graphql/query_handler.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib/kubernetes/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/kubernetes/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3355 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/kubernetes/base.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3292 2023-05-31 11:37:56.000000 etos_lib-2.2.0/src/etos_lib/kubernetes/jobs.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib/lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2152 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/auth.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4200 2023-06-01 07:05:22.000000 etos_lib-2.2.0/src/etos_lib/lib/config.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/database.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     5143 2023-05-31 11:37:56.000000 etos_lib-2.2.0/src/etos_lib/lib/debug.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    15885 2023-05-31 11:37:56.000000 etos_lib-2.2.0/src/etos_lib/lib/events.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/exceptions.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      810 2023-05-31 11:37:56.000000 etos_lib-2.2.0/src/etos_lib/lib/feature_flags.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4331 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/http.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/monitor.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2632 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/secrets.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/utils.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.230867 etos_lib-2.2.0/src/etos_lib/logging/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/logging/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2023-05-26 11:19:01.000000 etos_lib-2.2.0/src/etos_lib/logging/default_config.yaml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/logging/filter.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/logging/formatter.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     5506 2023-06-01 07:05:22.000000 etos_lib-2.2.0/src/etos_lib/logging/logger.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib.egg-info/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1290 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-05-26 11:39:50.000000 etos_lib-2.2.0/src/etos_lib.egg-info/not-zip-safe
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      185 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/requires.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2023-03-09 08:23:58.000000 etos_lib-2.2.0/test-requirements.txt
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.230867 etos_lib-2.2.0/tests/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2023-03-09 08:23:58.000000 etos_lib-2.2.0/tests/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2023-03-09 08:23:58.000000 etos_lib-2.2.0/tests/conftest.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2023-03-09 08:23:58.000000 etos_lib-2.2.0/tox.ini
```

### Comparing `etos_lib-2.1.0/.coveragerc` & `etos_lib-2.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/.github/workflows/main.yml` & `etos_lib-2.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/.gitignore` & `etos_lib-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/LICENSE.txt` & `etos_lib-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/PKG-INFO` & `etos_lib-2.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: etos_lib
-Version: 2.1.0
+Version: 2.2.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
-Description: ============
-        ETOS Library
-        ============
-        
-        .. image:: https://img.shields.io/badge/Stage-Sandbox-yellow.svg
-          :target: https://github.com/eiffel-community/community/blob/master/PROJECT_LIFECYCLE.md#stage-sandbox
-        
-        ETOS (Eiffel Test Orchestration System) Library
-        
-        
-        Description
-        ===========
-        
-        A collection of common tools and code used throughout the whole ETOS project.
-        
-        
-        Installation
-        ============
-        
-           pip install etos_lib
-        
-        
-        Contribute
-        ==========
-        
-        - Issue Tracker: https://github.com/eiffel-community/etos/issues
-        - Source Code: https://github.com/eiffel-community/etos-library
-        
-        
-        Support
-        =======
-        
-        If you are having issues, please let us know.
-        There is a mailing list at: etos-maintainers@googlegroups.com or just write an Issue.
-        
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.4
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+============
+ETOS Library
+============
+
+.. image:: https://img.shields.io/badge/Stage-Sandbox-yellow.svg
+  :target: https://github.com/eiffel-community/community/blob/master/PROJECT_LIFECYCLE.md#stage-sandbox
+
+ETOS (Eiffel Test Orchestration System) Library
+
+
+Description
+===========
+
+A collection of common tools and code used throughout the whole ETOS project.
+
+
+Installation
+============
+
+   pip install etos_lib
+
+
+Contribute
+==========
+
+- Issue Tracker: https://github.com/eiffel-community/etos/issues
+- Source Code: https://github.com/eiffel-community/etos-library
+
+
+Support
+=======
+
+If you are having issues, please let us know.
+There is a mailing list at: etos-maintainers@googlegroups.com or just write an Issue.
+
+
```

### Comparing `etos_lib-2.1.0/README.rst` & `etos_lib-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/docs/Makefile` & `etos_lib-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/docs/conf.py` & `etos_lib-2.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"etos_lib"
-copyright = u"2020, Axis Communications AB"
+project = "etos_lib"
+copyright = "2020, Axis Communications AB"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = ""  # Is set by calling `setup.py docs`
@@ -237,15 +237,15 @@
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ("index", "user_guide.tex", u"etos_lib Documentation", u"", "manual"),
+    ("index", "user_guide.tex", "etos_lib Documentation", "", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
```

### Comparing `etos_lib-2.1.0/setup.cfg` & `etos_lib-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/setup.py` & `etos_lib-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/__init__.py` & `etos_lib-2.2.0/src/etos_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/etos.py` & `etos_lib-2.2.0/src/etos_lib/etos.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/graphql/__init__.py` & `etos_lib-2.2.0/src/etos_lib/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/graphql/query_handler.py` & `etos_lib-2.2.0/src/etos_lib/graphql/query_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/kubernetes/__init__.py` & `etos_lib-2.2.0/src/etos_lib/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/kubernetes/base.py` & `etos_lib-2.2.0/src/etos_lib/kubernetes/base.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/kubernetes/jobs.py` & `etos_lib-2.2.0/src/etos_lib/kubernetes/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             status = response.status
             if status.active is not None:
                 print(f"Started at: {status.start_time}")
                 break
             time.sleep(1)
         return response
 
-    def wait_for_job_finished(self, job_name, timeout=(3600 * 10)):
+    def wait_for_job_finished(self, job_name, timeout=3600 * 10):
         """Wait for a kubernetes job status to become 'failed' or 'succeeded'.
 
         :param job_name: Name of job to wait for.
         :type job_name: str
         :param timeout: How long, in seconds, to wait for job to start.
                         Default: 10 hours.
         :type timeout: int
```

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/__init__.py` & `etos_lib-2.2.0/src/etos_lib/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/auth.py` & `etos_lib-2.2.0/src/etos_lib/lib/auth.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/config.py` & `etos_lib-2.2.0/src/etos_lib/lib/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ETOS Library config."""
+import json
 from pprint import pprint
 import os
 
 
 class Config:
     """ETOS configuration storage."""
 
@@ -92,17 +93,21 @@
         }
         self.set("rabbitmq", data)
 
     def rabbitmq_subscriber_from_environment(self):
         """Load RabbitMQ subscriber data from environment variables and set in config."""
         if not self.get("rabbitmq"):
             self.rabbitmq_from_environment()
+        queue_params = os.getenv("RABBITMQ_QUEUE_PARAMS")
+        if queue_params is not None:
+            queue_params = json.loads(queue_params)
         data = {
             "queue": os.getenv("RABBITMQ_QUEUE", None),
             "routing_key": os.getenv("RABBITMQ_ROUTING_KEY", "#"),
+            "queue_params": queue_params,
         }
         data.update(**self.get("rabbitmq").copy())
         self.set("rabbitmq_subscriber", data)
 
     def rabbitmq_publisher_from_environment(self):
         """Load RabbitMQ publisher data from environment variables and set in config.
```

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/database.py` & `etos_lib-2.2.0/src/etos_lib/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/debug.py` & `etos_lib-2.2.0/src/etos_lib/lib/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,29 +108,29 @@
         return bool(os.getenv("ETOS_DISABLE_MONITOR_ANNOUNCE", None))
 
     @property
     def environment_provider(self):
         """Environment provider host to use."""
         if os.getenv("ETOS_ENVIRONMENT_PROVIDER") is not None:
             return os.getenv("ETOS_ENVIRONMENT_PROVIDER")
-        raise Exception("ETOS_ENVIRONMENT_PROVIDER environment variable not set!")
+        raise ValueError("ETOS_ENVIRONMENT_PROVIDER environment variable not set!")
 
     @property
     def etos_api(self):
         """ETOS API host to use."""
         if os.getenv("ETOS_API") is not None:
             return os.getenv("ETOS_API")
-        raise Exception("ETOS_API environment variable not set!")
+        raise ValueError("ETOS_API environment variable not set!")
 
     @property
     def graphql_server(self):
         """Graphql server to use."""
         if os.getenv("ETOS_GRAPHQL_SERVER") is not None:
             return os.getenv("ETOS_GRAPHQL_SERVER")
-        raise Exception("ETOS_GRAPHQL_SERVER environment variable not set!")
+        raise ValueError("ETOS_GRAPHQL_SERVER environment variable not set!")
 
     @property
     def database_host(self):
         """Database host."""
         return os.getenv("ETOS_DATABASE_HOST", "localhost")
 
     @property
```

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/events.py` & `etos_lib-2.2.0/src/etos_lib/lib/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,17 @@
         :type optional: dict
         """
         if (
             optional.get("image") is None
             and optional.get("host") is None
             and optional.get("uri") is None
         ):
-            raise Exception("At least one of 'host', 'image' or 'uri' must be provided")
+            raise ValueError(
+                "At least one of 'host', 'image' or 'uri' must be provided"
+            )
         links = links if links is not None else {}
         data = {"name": name}
         data.update(**optional)
         return self.send(EiffelEnvironmentDefinedEvent(), links, data)
 
     def send_test_suite_started(self, name, links=None, **optional):
         """Publish a test suite started event.
@@ -236,15 +238,15 @@
         :type selection_strategy: dict
         :param links: Optional links to add to event.
         :type links: dict
         :param optional: Dictionary of optional data to add.
         :type optional: dict
         """
         if optional.get("batches") is None and optional.get("batchesUri") is None:
-            raise Exception(
+            raise ValueError(
                 "At least one of 'batches' or 'batchesUri' must be provided"
             )
         links = links if links is not None else {}
         data = {"selectionStrategy": selection_strategy}
         data.update(**optional)
         return self.send(EiffelTestExecutionRecipeCollectionCreatedEvent(), links, data)
```

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/exceptions.py` & `etos_lib-2.2.0/src/etos_lib/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/feature_flags.py` & `etos_lib-2.2.0/src/etos_lib/lib/feature_flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ETOS feature flags."""
 
+
 # This is a good thing! pylint:disable=too-few-public-methods
 class FeatureFlags:
     """Feature flags for ETOS."""
```

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/http.py` & `etos_lib-2.2.0/src/etos_lib/lib/http.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/monitor.py` & `etos_lib-2.2.0/src/etos_lib/lib/monitor.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/secrets.py` & `etos_lib-2.2.0/src/etos_lib/lib/secrets.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/lib/utils.py` & `etos_lib-2.2.0/src/etos_lib/lib/utils.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/logging/__init__.py` & `etos_lib-2.2.0/src/etos_lib/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/logging/filter.py` & `etos_lib-2.2.0/src/etos_lib/logging/filter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/logging/formatter.py` & `etos_lib-2.2.0/src/etos_lib/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib/logging/logger.py` & `etos_lib-2.2.0/src/etos_lib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/src/etos_lib.egg-info/SOURCES.txt` & `etos_lib-2.2.0/src/etos_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-2.1.0/tests/__init__.py` & `etos_lib-2.2.0/tests/__init__.py`

 * *Files identical despite different names*

