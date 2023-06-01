# Comparing `tmp/etos_lib-2.2.0.tar.gz` & `tmp/etos_lib-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_lib-2.2.0.tar", last modified: Thu Jun  1 07:05:41 2023, max compression
+gzip compressed data, was "etos_lib-3.0.0.tar", last modified: Thu Jun  1 07:09:10 2023, max compression
```

## Comparing `etos_lib-2.2.0.tar` & `etos_lib-3.0.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.230867 etos_lib-2.2.0/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2023-03-09 08:23:58.000000 etos_lib-2.2.0/.coveragerc
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.222868 etos_lib-2.2.0/.github/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/.github/workflows/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-03-09 08:23:58.000000 etos_lib-2.2.0/.github/workflows/main.yml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      536 2023-06-01 07:05:22.000000 etos_lib-2.2.0/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-03-09 08:23:58.000000 etos_lib-2.2.0/AUTHORS.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-03-09 08:23:58.000000 etos_lib-2.2.0/CODEOWNERS
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-03-09 08:23:58.000000 etos_lib-2.2.0/LICENSE.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-01 07:05:41.230867 etos_lib-2.2.0/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2023-03-09 08:23:58.000000 etos_lib-2.2.0/README.rst
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/docs/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/Makefile
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/docs/_static/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/_static/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/authors.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/changelog.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     9175 2023-05-31 11:37:56.000000 etos_lib-2.2.0/docs/conf.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/index.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/license.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/readme.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:58.000000 etos_lib-2.2.0/docs/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      177 2023-06-01 07:05:22.000000 etos_lib-2.2.0/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1473 2023-06-01 07:05:41.230867 etos_lib-2.2.0/setup.cfg
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2023-03-09 08:23:58.000000 etos_lib-2.2.0/setup.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.222868 etos_lib-2.2.0/src/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5386 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/etos.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib/graphql/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/graphql/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2692 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/graphql/query_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib/kubernetes/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/kubernetes/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3355 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/kubernetes/base.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3292 2023-05-31 11:37:56.000000 etos_lib-2.2.0/src/etos_lib/kubernetes/jobs.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib/lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2152 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/auth.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4200 2023-06-01 07:05:22.000000 etos_lib-2.2.0/src/etos_lib/lib/config.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/database.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5143 2023-05-31 11:37:56.000000 etos_lib-2.2.0/src/etos_lib/lib/debug.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    15885 2023-05-31 11:37:56.000000 etos_lib-2.2.0/src/etos_lib/lib/events.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/exceptions.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      810 2023-05-31 11:37:56.000000 etos_lib-2.2.0/src/etos_lib/lib/feature_flags.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4331 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/http.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/monitor.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2632 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/secrets.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/lib/utils.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.230867 etos_lib-2.2.0/src/etos_lib/logging/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/logging/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2023-05-26 11:19:01.000000 etos_lib-2.2.0/src/etos_lib/logging/default_config.yaml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/logging/filter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2023-03-09 08:23:58.000000 etos_lib-2.2.0/src/etos_lib/logging/formatter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5506 2023-06-01 07:05:22.000000 etos_lib-2.2.0/src/etos_lib/logging/logger.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.226868 etos_lib-2.2.0/src/etos_lib.egg-info/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1290 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-05-26 11:39:50.000000 etos_lib-2.2.0/src/etos_lib.egg-info/not-zip-safe
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      185 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/requires.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2023-06-01 07:05:41.000000 etos_lib-2.2.0/src/etos_lib.egg-info/top_level.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2023-03-09 08:23:58.000000 etos_lib-2.2.0/test-requirements.txt
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:05:41.230867 etos_lib-2.2.0/tests/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2023-03-09 08:23:58.000000 etos_lib-2.2.0/tests/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2023-03-09 08:23:58.000000 etos_lib-2.2.0/tests/conftest.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2023-03-09 08:23:58.000000 etos_lib-2.2.0/tox.ini
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2023-03-09 08:23:58.000000 etos_lib-3.0.0/.coveragerc
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/.github/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/.github/workflows/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-03-09 08:23:58.000000 etos_lib-3.0.0/.github/workflows/main.yml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      542 2023-06-01 07:09:02.000000 etos_lib-3.0.0/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-03-09 08:23:58.000000 etos_lib-3.0.0/AUTHORS.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-03-09 08:23:58.000000 etos_lib-3.0.0/CODEOWNERS
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-03-09 08:23:58.000000 etos_lib-3.0.0/LICENSE.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-01 07:09:10.410018 etos_lib-3.0.0/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2023-03-09 08:23:58.000000 etos_lib-3.0.0/README.rst
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/docs/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/Makefile
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/docs/_static/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/_static/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/authors.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/changelog.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     9175 2023-05-31 11:37:56.000000 etos_lib-3.0.0/docs/conf.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/index.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/license.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/readme.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      177 2023-06-01 07:09:02.000000 etos_lib-3.0.0/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1473 2023-06-01 07:09:10.414018 etos_lib-3.0.0/setup.cfg
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2023-03-09 08:23:58.000000 etos_lib-3.0.0/setup.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     5386 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/etos.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/graphql/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/graphql/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2692 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/graphql/query_handler.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/kubernetes/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/kubernetes/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3355 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/kubernetes/base.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3292 2023-05-31 11:37:56.000000 etos_lib-3.0.0/src/etos_lib/kubernetes/jobs.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2152 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/auth.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4814 2023-06-01 07:09:02.000000 etos_lib-3.0.0/src/etos_lib/lib/config.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/database.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     5143 2023-05-31 11:37:56.000000 etos_lib-3.0.0/src/etos_lib/lib/debug.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    15885 2023-05-31 11:37:56.000000 etos_lib-3.0.0/src/etos_lib/lib/events.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/exceptions.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      810 2023-05-31 11:37:56.000000 etos_lib-3.0.0/src/etos_lib/lib/feature_flags.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4331 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/http.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/monitor.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2632 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/secrets.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/utils.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/logging/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/logging/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2023-05-26 11:19:01.000000 etos_lib-3.0.0/src/etos_lib/logging/default_config.yaml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/logging/filter.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/logging/formatter.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1967 2023-06-01 07:09:02.000000 etos_lib-3.0.0/src/etos_lib/logging/log_publisher.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     6817 2023-06-01 07:09:02.000000 etos_lib-3.0.0/src/etos_lib/logging/logger.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2331 2023-06-01 07:09:02.000000 etos_lib-3.0.0/src/etos_lib/logging/rabbitmq_handler.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib.egg-info/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1369 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-05-26 11:39:50.000000 etos_lib-3.0.0/src/etos_lib.egg-info/not-zip-safe
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      185 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/requires.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2023-03-09 08:23:58.000000 etos_lib-3.0.0/test-requirements.txt
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/tests/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2023-03-09 08:23:58.000000 etos_lib-3.0.0/tests/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2023-03-09 08:23:58.000000 etos_lib-3.0.0/tests/conftest.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2023-03-09 08:23:58.000000 etos_lib-3.0.0/tox.ini
```

### Comparing `etos_lib-2.2.0/.coveragerc` & `etos_lib-3.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/.github/workflows/main.yml` & `etos_lib-3.0.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/.gitignore` & `etos_lib-3.0.0/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 *.log
 *.pot
 __pycache__/*
 .cache/*
 .*.swp
 */.ipynb_checkpoints/*
 .DS_Store
+.tags
 
 # Project files
 .ropeproject
 .project
 .pydevproject
 .settings
 .idea
```

### Comparing `etos_lib-2.2.0/LICENSE.txt` & `etos_lib-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/PKG-INFO` & `etos_lib-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_lib
-Version: 2.2.0
+Version: 3.0.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_lib-2.2.0/README.rst` & `etos_lib-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/docs/Makefile` & `etos_lib-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/docs/conf.py` & `etos_lib-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/setup.cfg` & `etos_lib-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	graphql-core==2.2.1
 	gql==0.1.0
 	cryptography==3.1
 	redis==3.5.3
-	eiffellib[rabbitmq]==2.3.0
+	eiffellib[rabbitmq]==2.4.1
 	pydantic==1.6
 	requests==2.24.0
 	kubernetes==7.0.1
 	python-box==5.2.0
 python_requires = >=3.4
 
 [options.packages.find]
```

### Comparing `etos_lib-2.2.0/setup.py` & `etos_lib-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/__init__.py` & `etos_lib-3.0.0/src/etos_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/etos.py` & `etos_lib-3.0.0/src/etos_lib/etos.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/graphql/__init__.py` & `etos_lib-3.0.0/src/etos_lib/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/graphql/query_handler.py` & `etos_lib-3.0.0/src/etos_lib/graphql/query_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/kubernetes/__init__.py` & `etos_lib-3.0.0/src/etos_lib/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/kubernetes/base.py` & `etos_lib-3.0.0/src/etos_lib/kubernetes/base.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/kubernetes/jobs.py` & `etos_lib-3.0.0/src/etos_lib/kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/__init__.py` & `etos_lib-3.0.0/src/etos_lib/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/auth.py` & `etos_lib-3.0.0/src/etos_lib/lib/auth.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/config.py` & `etos_lib-3.0.0/src/etos_lib/lib/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020-2021 Axis Communications AB.
+# Copyright Axis Communications AB.
 #
 # For a full list of individual contributors, please see the commit history.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -75,14 +75,27 @@
         return self.config.get("rabbitmq_publisher")
 
     @property
     def rabbitmq_subscriber(self):
         """Rabbitmq Subscriber data."""
         return self.config.get("rabbitmq_subscriber")
 
+    def etos_rabbitmq_publisher_data(self):
+        """Get RabbitMQ parameters for the ETOS rabbitmq service."""
+        ssl = os.getenv("ETOS_RABBITMQ_SSL", "true") == "true"
+        return {
+            "host": os.getenv("ETOS_RABBITMQ_HOST", "127.0.0.1"),
+            "exchange": os.getenv("ETOS_RABBITMQ_EXCHANGE", "etos"),
+            "username": os.getenv("ETOS_RABBITMQ_USERNAME", None),
+            "password": os.getenv("ETOS_RABBITMQ_PASSWORD", None),
+            "port": int(os.getenv("ETOS_RABBITMQ_PORT", "5672")),
+            "vhost": os.getenv("ETOS_RABBITMQ_VHOST", None),
+            "ssl": ssl,
+        }
+
     def rabbitmq_from_environment(self):
         """Load RabbitMQ data from environment variables."""
         ssl = os.getenv("RABBITMQ_SSL", "true") == "true"
         data = {
             "host": os.getenv("RABBITMQ_HOST", "127.0.0.1"),
             "exchange": os.getenv("RABBITMQ_EXCHANGE", "eiffel"),
             "username": os.getenv("RABBITMQ_USERNAME", None),
```

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/database.py` & `etos_lib-3.0.0/src/etos_lib/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/debug.py` & `etos_lib-3.0.0/src/etos_lib/lib/debug.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/events.py` & `etos_lib-3.0.0/src/etos_lib/lib/events.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/exceptions.py` & `etos_lib-3.0.0/src/etos_lib/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/feature_flags.py` & `etos_lib-3.0.0/src/etos_lib/lib/feature_flags.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/http.py` & `etos_lib-3.0.0/src/etos_lib/lib/http.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/monitor.py` & `etos_lib-3.0.0/src/etos_lib/lib/monitor.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/secrets.py` & `etos_lib-3.0.0/src/etos_lib/lib/secrets.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/lib/utils.py` & `etos_lib-3.0.0/src/etos_lib/lib/utils.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/logging/__init__.py` & `etos_lib-3.0.0/src/etos_lib/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/logging/filter.py` & `etos_lib-3.0.0/src/etos_lib/logging/filter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/logging/formatter.py` & `etos_lib-3.0.0/src/etos_lib/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-2.2.0/src/etos_lib/logging/logger.py` & `etos_lib-3.0.0/src/etos_lib/logging/logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020-2021 Axis Communications AB.
+# Copyright Axis Communications AB.
 #
 # For a full list of individual contributors, please see the commit history.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -25,21 +25,25 @@
     setup_logging("myApp", "1.0.0", "production")
     logger = logging.getLogger(__name__)
     logger.info("Hello!")
     >>> [2020-12-16 10:35:00][cb7c8cd9-40a6-4ecc-8321-a1eae6beae35] INFO: Hello!
 
 """
 import sys
+import atexit
 from pathlib import Path
 import threading
 import logging
 import logging.config
 from box import Box
 from etos_lib.logging.filter import EtosFilter
 from etos_lib.logging.formatter import EtosLogFormatter
+from etos_lib.logging.rabbitmq_handler import RabbitMQHandler
+from etos_lib.logging.log_publisher import RabbitMQLogPublisher
+from etos_lib.lib.config import Config
 from etos_lib.lib.debug import Debug
 
 DEFAULT_CONFIG = Path(__file__).parent.joinpath("default_config.yaml")
 DEFAULT_LOG_PATH = Debug().default_log_path
 
 FORMAT_CONFIG = threading.local()
 
@@ -112,14 +116,45 @@
     stream_handler = logging.StreamHandler(sys.stdout)
     stream_handler.setFormatter(logging.Formatter(logformat, datefmt=dateformat))
     stream_handler.setLevel(loglevel)
     stream_handler.addFilter(log_filter)
     root_logger.addHandler(stream_handler)
 
 
+def setup_rabbitmq_logging(log_filter):
+    """Set up rabbitmq logging.
+
+    :param log_filter: Logfilter to add to stream handler.
+    :type log_filter: :obj:`EtosFilter`
+    """
+    loglevel = logging.DEBUG
+
+    root_logger = logging.getLogger()
+
+    # These have to be removed as they create a loop.
+    # They will still work with the other handlers.
+    logging.getLogger("pika").propagate = False
+    logging.getLogger("rabbitmq_publisher").propagate = False
+    logging.getLogger("base_rabbitmq").propagate = False
+
+    rabbitmq = RabbitMQLogPublisher(
+        **Config().etos_rabbitmq_publisher_data(), routing_key=None
+    )
+    if not Debug().disable_sending_events:
+        rabbitmq.start()
+    atexit.register(close_rabbit, rabbitmq)
+
+    rabbit_handler = RabbitMQHandler(rabbitmq)
+    rabbit_handler.setFormatter(EtosLogFormatter())
+    rabbit_handler.setLevel(loglevel)
+    rabbit_handler.addFilter(log_filter)
+
+    root_logger.addHandler(rabbit_handler)
+
+
 def setup_logging(application, version, environment, config_file=DEFAULT_CONFIG):
     """Set up basic logging.
 
     :param application: Name of application to setup logging for.
     :type application: str
     :param version: Version of application to setup logging for.
     :type version: str
@@ -143,7 +178,14 @@
     root_logger.setLevel(logging.DEBUG)
     root_logger.propagate = 0
 
     if logging_config.get("stream"):
         setup_stream_logging(logging_config.get("stream"), log_filter)
     if logging_config.get("file"):
         setup_file_logging(logging_config.get("file"), log_filter)
+    setup_rabbitmq_logging(log_filter)
+
+
+def close_rabbit(rabbit):
+    """Close down a rabbitmq connection."""
+    rabbit.wait_for_unpublished_events()
+    rabbit.close()
```

### Comparing `etos_lib-2.2.0/src/etos_lib.egg-info/PKG-INFO` & `etos_lib-3.0.0/src/etos_lib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos-lib
-Version: 2.2.0
+Version: 3.0.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_lib-2.2.0/src/etos_lib.egg-info/SOURCES.txt` & `etos_lib-3.0.0/src/etos_lib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -44,10 +44,12 @@
 src/etos_lib/lib/monitor.py
 src/etos_lib/lib/secrets.py
 src/etos_lib/lib/utils.py
 src/etos_lib/logging/__init__.py
 src/etos_lib/logging/default_config.yaml
 src/etos_lib/logging/filter.py
 src/etos_lib/logging/formatter.py
+src/etos_lib/logging/log_publisher.py
 src/etos_lib/logging/logger.py
+src/etos_lib/logging/rabbitmq_handler.py
 tests/__init__.py
 tests/conftest.py
```

### Comparing `etos_lib-2.2.0/tests/__init__.py` & `etos_lib-3.0.0/tests/__init__.py`

 * *Files identical despite different names*

