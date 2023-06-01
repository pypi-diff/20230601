# Comparing `tmp/kbcstorage-0.5.0.tar.gz` & `tmp/kbcstorage-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbcstorage-0.5.0.tar", last modified: Thu Mar  9 13:36:21 2023, max compression
+gzip compressed data, was "kbcstorage-0.7.2.tar", last modified: Thu Jun  1 17:19:12 2023, max compression
```

## Comparing `kbcstorage-0.5.0.tar` & `kbcstorage-0.7.2.tar`

### file list

```diff
@@ -1,53 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      347 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/kbcstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23904 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/kbcstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/bucket_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/job_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/table_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/workspace_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.500666 kbcstorage-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.env.template
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.476666 kbcstorage-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.480666 kbcstorage-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-01 17:19:12.496666 kbcstorage-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.484666 kbcstorage-0.7.2/kbcstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23903 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.488666 kbcstorage-0.7.2/kbcstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:19:12.500666 kbcstorage-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.488666 kbcstorage-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/base_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.492666 kbcstorage-0.7.2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_workspaces_abs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.496666 kbcstorage-0.7.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/branches_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/bucket_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/component_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/configuration_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/job_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/table_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/token_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/workspace_responses.py
```

### Comparing `kbcstorage-0.5.0/LICENSE` & `kbcstorage-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/PKG-INFO` & `kbcstorage-0.7.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,27 @@
-Metadata-Version: 2.1
-Name: kbcstorage
-Version: 0.5.0
-Home-page: https://github.com/keboola/sapi-python-client
-Download-URL: https://github.com/keboola/sapi-python-client
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.txt
-
 [![Build Status](https://travis-ci.org/keboola/sapi-python-client.svg?branch=master)](https://travis-ci.org/keboola/sapi-python-client)
 
 # Python client for the Keboola Storage API
 Client for using [Keboola Connection Storage API](http://docs.keboola.apiary.io/). This API client provides client methods to get data from KBC and store data in KBC. The endpoints 
 for working with buckets, tables and workspaces are covered.
 
 ## Install
 
-`$ pip3 install git+https://github.com/keboola/sapi-python-client.git`
+```bash
+pip install kbcstorage
+```
 
 or 
 
 ```bash
-$ git clone https://github.com/keboola/sapi-python-client.git && cd sapi-python-client
-$ python setup.py install
+pip install git+https://github.com/keboola/sapi-python-client.git
 ```
 
 ## Client Class Usage
-```
+```python
 from kbcstorage.client import Client
 
 client = Client('https://connection.keboola.com', 'your-token')
 
 # get table data into local file
 client.tables.export_to_file(table_id='in.c-demo.some-table', path_name='/data/')
 
@@ -45,15 +36,15 @@
 
 # get table info
 client.tables.detail('in.c-demo.some-table')
 
 ```
 
 ## Endpoint Classes Usage 
-```
+```python
 from kbcstorage.tables import Tables
 from kbcstorage.buckets import Buckets
 
 tables = Tables('https://connection.keboola.com', 'your-token')
 
 # get table data into local file
 tables.export_to_file(table_id='in.c-demo.some-table', path_name='/data/')
@@ -69,40 +60,33 @@
 buckets.list_tables('in.c-demo')
 
 # get table info
 tables.detail('in.c-demo.some-table')
 
 ```
 
-## Docker image
-Docker image with pre-installed library is also available, run it via:
-
-```
-docker run -i -t quay.io/keboola/sapi-python-client
-```
-
 ## Tests
-
-```bash
-$ git clone https://github.com/keboola/sapi-python-client.git && cd sapi-python-client
-$ python setup.py test
-```
-
-or 
+Create `.env` file according to the `.env.template` file and run the tests with:
 
 ```bash
 $ docker-compose run --rm -e KBC_TEST_TOKEN -e KBC_TEST_API_URL sapi-python-client -m unittest discover
 ```
 
 ## Contribution Guide
 The client is far from supporting the entire API, all contributions are very welcome. New API endpoints should 
-be implemeneted in their own class extending `Endpoint`. Naming conventions should follow existing naming conventions
-or those of the [API](http://docs.keboola.apiary.io/#). If the method contains some processing of the request or response, consult the corresponing [PHP implementation](https://github.com/keboola/storage-api-php-client) for reference. New code should be covered by tests.
-
-Note that if you submit a PR from your own forked repository, the automated functional tests will fail. This is limitation of [Travis](https://docs.travis-ci.com/user/pull-requests/#Pull-Requests-and-Security-Restrictions). Either run the tests locally (set `KBC_TEST_TOKEN` (your token to test project) and `KBC_TEST_API_URL` (https://connection.keboola.com) variables) or ask for access. In case, you need a project for local testing, feel free to [ask for one](https://developers.keboola.com/#development-project).
+be implemented in their own class extending `Endpoint`. Naming conventions should follow existing naming conventions
+or those of the [API](http://docs.keboola.apiary.io/#). If the method contains some processing of the request or 
+response, consult the corresponding [PHP implementation](https://github.com/keboola/storage-api-php-client) for 
+reference. New code should be covered by tests.
+
+Note that if you submit a PR from your own forked repository, the automated functional tests will fail. 
+This is expected for security reasons, please do send the PR anyway. 
+Either run the tests locally (set `KBC_TEST_TOKEN` (your token to test project) and 
+`KBC_TEST_API_URL` (https://connection.keboola.com) variables) or ask for access. In case, you need a 
+project for local testing, feel free to [ask for one](https://developers.keboola.com/#development-project).
 
 The recommended workflow for making a pull request is:
 
 ```bash
 git clone https://github.com/keboola/sapi-python-client.git
 git checkout master
 git pull
```

### Comparing `kbcstorage-0.5.0/kbcstorage/base.py` & `kbcstorage-0.7.2/kbcstorage/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,14 @@
             path_component (str): The section of the path specific to the
                 endpoint. eg. "buckets"
             token (str): A key for the Storage API. Can be found in the storage
                 console.
         """
         if not root_url:
             raise ValueError("Root URL is required.")
-        if not path_component:
-            raise ValueError("Path component is required.")
         if not token:
             raise ValueError("Token is required.")
         self.root_url = root_url
         self.base_url = '{}/v2/storage/{}'.format(root_url.strip('/'),
                                                   path_component.strip('/'))
         self.token = token
         self._auth_header = {'X-StorageApi-Token': self.token,
```

### Comparing `kbcstorage-0.5.0/kbcstorage/buckets.py` & `kbcstorage-0.7.2/kbcstorage/buckets.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/kbcstorage/client.py` & `kbcstorage-0.7.2/kbcstorage/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 """"
 Entry point for the Storage API client.
 """
-
+from kbcstorage.branches import Branches
 from kbcstorage.buckets import Buckets
+from kbcstorage.components import Components
+from kbcstorage.configurations import Configurations
+from kbcstorage.tokens import Tokens
 from kbcstorage.workspaces import Workspaces
 from kbcstorage.jobs import Jobs
 from kbcstorage.tables import Tables
 from kbcstorage.files import Files
 
 
 class Client:
     """
     Storage API Client.
     """
 
-    def __init__(self, api_domain, token):
+    def __init__(self, api_domain, token, branch_id='default'):
         """
         Initialise a client.
 
         Args:
             api_domain (str): The domain on which the API sits. eg.
                 "https://connection.keboola.com".
             token (str): A storage API key.
+            branch_id (str): The ID of branch to use, use 'default' to work without branch (in main).
         """
-        self.root_url = api_domain
+        self.root_url = api_domain.rstrip("/")
         self._token = token
+        self._branch_id = branch_id
 
         self.buckets = Buckets(self.root_url, self.token)
         self.files = Files(self.root_url, self.token)
         self.jobs = Jobs(self.root_url, self.token)
         self.tables = Tables(self.root_url, self.token)
         self.workspaces = Workspaces(self.root_url, self.token)
+        self.components = Components(self.root_url, self.token, self.branch_id)
+        self.configurations = Configurations(self.root_url, self.token, self.branch_id)
+        self.tokens = Tokens(self.root_url, self.token)
+        self.branches = Branches(self.root_url, self.token)
 
     @property
     def token(self):
         return self._token
+
+    @property
+    def branch_id(self):
+        return self._branch_id
```

### Comparing `kbcstorage-0.5.0/kbcstorage/files.py` & `kbcstorage-0.7.2/kbcstorage/files.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/kbcstorage/jobs.py` & `kbcstorage-0.7.2/kbcstorage/jobs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/kbcstorage/tables.py` & `kbcstorage-0.7.2/kbcstorage/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from kbcstorage.base import Endpoint
 from kbcstorage.files import Files
 from kbcstorage.jobs import Jobs
 
 
 class Tables(Endpoint):
     """
-    Buckets Endpoint
+    Tables Endpoint
     """
     def __init__(self, root_url, token):
         """
         Create a Tables endpoint.
 
         Args:
             root_url (:obj:`str`): The base url for the API.
```

### Comparing `kbcstorage-0.5.0/kbcstorage/workspaces.py` & `kbcstorage-0.7.2/kbcstorage/workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/kbcstorage.egg-info/SOURCES.txt` & `kbcstorage-0.7.2/kbcstorage.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 .codeclimate.yml
+.dockerignore
+.env.template
 .flake8
 .gitattributes
 .gitignore
 Dockerfile
 LICENSE
-LICENSE.txt
 README.md
-deploy.sh
 docker-compose.yml
-setup.py
+pyproject.toml
 .github/workflows/push.yml
 kbcstorage/__init__.py
 kbcstorage/base.py
+kbcstorage/branches.py
 kbcstorage/buckets.py
 kbcstorage/client.py
+kbcstorage/components.py
+kbcstorage/configurations.py
 kbcstorage/files.py
 kbcstorage/jobs.py
 kbcstorage/tables.py
+kbcstorage/tokens.py
 kbcstorage/workspaces.py
 kbcstorage.egg-info/PKG-INFO
 kbcstorage.egg-info/SOURCES.txt
 kbcstorage.egg-info/dependency_links.txt
 kbcstorage.egg-info/requires.txt
 kbcstorage.egg-info/top_level.txt
 tests/__init__.py
+tests/base_test_case.py
 tests/functional/__init__.py
 tests/functional/test_base.py
+tests/functional/test_branches.py
 tests/functional/test_buckets.py
 tests/functional/test_client.py
+tests/functional/test_components.py
+tests/functional/test_configurations.py
 tests/functional/test_files.py
 tests/functional/test_tables.py
+tests/functional/test_tokens.py
 tests/functional/test_workspaces.py
+tests/functional/test_workspaces_abs.py
 tests/mocks/__init__.py
+tests/mocks/branches_responses.py
 tests/mocks/bucket_responses.py
+tests/mocks/component_responses.py
+tests/mocks/configuration_responses.py
 tests/mocks/job_responses.py
 tests/mocks/table_responses.py
+tests/mocks/test_branches.py
 tests/mocks/test_buckets.py
 tests/mocks/test_client.py
+tests/mocks/test_components.py
+tests/mocks/test_configurations.py
 tests/mocks/test_jobs.py
 tests/mocks/test_tables.py
+tests/mocks/test_tokens.py
 tests/mocks/test_workspaces.py
+tests/mocks/token_responses.py
 tests/mocks/workspace_responses.py
```

### Comparing `kbcstorage-0.5.0/tests/functional/test_base.py` & `kbcstorage-0.7.2/tests/functional/test_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import unittest
 import os
 from requests import HTTPError
 from kbcstorage.base import Endpoint
+from tests.base_test_case import BaseTestCase
 
 
-class TestEndpoint(unittest.TestCase):
+class TestEndpoint(BaseTestCase):
     """
     Test Endpoint functionality.
     """
     def setUp(self):
         self.root = os.getenv('KBC_TEST_API_URL')
         self.token = 'some-token'
 
@@ -80,28 +80,23 @@
             endpoint._delete('{}/not-a-url'.format(endpoint.base_url))
 
     def test_custom_headers(self):
         """
         Passing custom headers to Endpoint._get()
         """
         endpoint = Endpoint(self.root, '/', self.token)
-        resp = endpoint._get_raw(self.root, headers={'x-foo': 'bar'})
+        resp = endpoint._get_raw(self.root + '/v2/storage', headers={'x-foo': 'bar'})
         request_headers = resp.request.headers
         with self.subTest():
             self.assertIn('x-foo', request_headers)
         with self.subTest():
             self.assertIn('X-StorageApi-Token', request_headers)
         with self.subTest():
             self.assertEqual('bar', request_headers['x-foo'])
 
     def test_missing_url(self):
         with self.assertRaisesRegex(ValueError, "Root URL is required."):
             Endpoint(None, '', None)
 
-    def test_missing_part(self):
-        with self.assertRaisesRegex(ValueError,
-                                    "Path component is required."):
-            Endpoint('https://connection.keboola.com/', '', None)
-
     def test_missing_token(self):
         with self.assertRaisesRegex(ValueError, "Token is required."):
             Endpoint('https://connection.keboola.com/', 'tables', None)
```

### Comparing `kbcstorage-0.5.0/tests/functional/test_buckets.py` & `kbcstorage-0.7.2/tests/functional/test_buckets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import csv
 import os
 import tempfile
-import unittest
 import warnings
-
 from requests import exceptions
 from kbcstorage.buckets import Buckets
 from kbcstorage.tables import Tables
+from tests.base_test_case import BaseTestCase
 
 
-class TestBuckets(unittest.TestCase):
+class TestEndpoint(BaseTestCase):
     def setUp(self):
         self.buckets = Buckets(os.getenv('KBC_TEST_API_URL'),
                                os.getenv('KBC_TEST_TOKEN'))
         try:
             self.buckets.delete('in.c-py-test-buckets', force=True)
         except exceptions.HTTPError as e:
             if e.response.status_code != 404:
```

### Comparing `kbcstorage-0.5.0/tests/functional/test_client.py` & `kbcstorage-0.7.2/tests/functional/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import csv
 import os
 import tempfile
-import unittest
 import warnings
-
 from requests import exceptions
 from kbcstorage.client import Client
+from tests.base_test_case import BaseTestCase
 
 
-class TestClient(unittest.TestCase):
+class TestEndpoint(BaseTestCase):
     def setUp(self):
         self.client = Client(os.getenv('KBC_TEST_API_URL'),
                              os.getenv('KBC_TEST_TOKEN'))
         try:
             self.client.buckets.delete('in.c-py-test-client', force=True)
         except exceptions.HTTPError as e:
             if e.response.status_code != 404:
```

### Comparing `kbcstorage-0.5.0/tests/functional/test_files.py` & `kbcstorage-0.7.2/tests/functional/test_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import csv
 import os
-import unittest
 import tempfile
 import warnings
 import time
 from requests import exceptions
-
 from kbcstorage.buckets import Buckets
 from kbcstorage.files import Files
 from kbcstorage.tables import Tables
+from tests.base_test_case import BaseTestCase
 
 
-class TestFiles(unittest.TestCase):
+class TestEndpoint(BaseTestCase):
     def setUp(self):
         # timeout for files from previous tests to appear
         time.sleep(1)
         self.files = Files(os.getenv('KBC_TEST_API_URL'),
                            os.getenv('KBC_TEST_TOKEN'))
         files = self.files.list(tags=['py-test'])
         for file in files:
```

### Comparing `kbcstorage-0.5.0/tests/functional/test_tables.py` & `kbcstorage-0.7.2/tests/functional/test_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
-import unittest
 import tempfile
 import csv
 import warnings
 from requests import exceptions
 from kbcstorage.tables import Tables
 from kbcstorage.buckets import Buckets
+from tests.base_test_case import BaseTestCase
 
 
-class TestTables(unittest.TestCase):
+class TestEndpoint(BaseTestCase):
     def setUp(self):
         self.tables = Tables(os.getenv('KBC_TEST_API_URL'),
                              os.getenv('KBC_TEST_TOKEN'))
         self.buckets = Buckets(os.getenv('KBC_TEST_API_URL'),
                                os.getenv('KBC_TEST_TOKEN'))
         try:
             self.buckets.delete('in.c-py-test-tables', force=True)
```

### Comparing `kbcstorage-0.5.0/tests/mocks/bucket_responses.py` & `kbcstorage-0.7.2/tests/mocks/bucket_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/tests/mocks/job_responses.py` & `kbcstorage-0.7.2/tests/mocks/job_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/tests/mocks/table_responses.py` & `kbcstorage-0.7.2/tests/mocks/table_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/tests/mocks/test_buckets.py` & `kbcstorage-0.7.2/tests/mocks/test_buckets.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/tests/mocks/test_jobs.py` & `kbcstorage-0.7.2/tests/mocks/test_jobs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/tests/mocks/test_tables.py` & `kbcstorage-0.7.2/tests/mocks/test_tables.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.5.0/tests/mocks/test_workspaces.py` & `kbcstorage-0.7.2/tests/mocks/test_workspaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Asses basic functionality of the Workspace endpoint.
 """
 import unittest
-
 import responses
 from requests import HTTPError
 
 from kbcstorage.workspaces import Workspaces
 
 from .workspace_responses import (list_response, detail_response,
                                   load_tables_response, create_response,
```

### Comparing `kbcstorage-0.5.0/tests/mocks/workspace_responses.py` & `kbcstorage-0.7.2/tests/mocks/workspace_responses.py`

 * *Files identical despite different names*

