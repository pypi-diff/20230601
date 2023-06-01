# Comparing `tmp/br-ci-sdk-0.0.2.tar.gz` & `tmp/br-ci-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "br-ci-sdk-0.0.2.tar", last modified: Thu Jun  1 10:09:25 2023, max compression
+gzip compressed data, was "br-ci-sdk-0.0.3.tar", last modified: Thu Jun  1 10:56:47 2023, max compression
```

## Comparing `br-ci-sdk-0.0.2.tar` & `br-ci-sdk-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,94 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2302 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1868 2023-05-31 08:38:01.000000 br-ci-sdk-0.0.2/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.243923 br-ci-sdk-0.0.2/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1534 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2251 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1295 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2302 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      676 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       39 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       75 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/requires.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       34 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        8 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3923 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)    10941 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3359 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/repo.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      527 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1360 2023-06-01 10:09:18.000000 br-ci-sdk-0.0.2/setup.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1304 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/xml_utils.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.498300 br-ci-sdk-0.0.3/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       10 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/MANIFEST.in
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2302 2023-06-01 10:56:47.498300 br-ci-sdk-0.0.3/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1868 2023-05-31 08:38:01.000000 br-ci-sdk-0.0.3/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/br_ci_sdk.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2302 2023-06-01 10:56:47.000000 br-ci-sdk-0.0.3/br_ci_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2442 2023-06-01 10:56:47.000000 br-ci-sdk-0.0.3/br_ci_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-06-01 10:56:47.000000 br-ci-sdk-0.0.3/br_ci_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       44 2023-06-01 10:56:47.000000 br-ci-sdk-0.0.3/br_ci_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       75 2023-06-01 10:56:47.000000 br-ci-sdk-0.0.3/br_ci_sdk.egg-info/requires.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        5 2023-06-01 10:56:47.000000 br-ci-sdk-0.0.3/br_ci_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/brci/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      340 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/.env
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      341 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/.perf.test.env
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/Dockerfile-online-compile
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/brci/__pycache__/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      139 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      963 2023-06-01 10:53:11.000000 br-ci-sdk-0.0.3/brci/__pycache__/createPod.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2722 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/__pycache__/main.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3223 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/__pycache__/run.cpython-39.pyc
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/brci/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/apis/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/brci/apis/__pycache__/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      147 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/apis/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1653 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/apis/__pycache__/build.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1868 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/apis/__pycache__/client.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4351 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/apis/__pycache__/pdu.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2120 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/apis/__pycache__/perf.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1447 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/apis/__pycache__/pr.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1534 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2251 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1295 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/apis/pr.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2341 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/bm_supa_perf_cur_test.csv
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      167 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/bm_supa_perf_cur_test2.csv
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      661 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/compare.conf.template
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/brci/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/config/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/brci/config/__pycache__/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      467 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/config/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      672 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/config/__pycache__/develop.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/config/prod.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      751 2023-06-01 10:52:45.000000 br-ci-sdk-0.0.3/brci/createPod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/brci/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        8 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/handles/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.494300 br-ci-sdk-0.0.3/brci/handles/__pycache__/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      150 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/handles/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3837 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/handles/__pycache__/build.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3207 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/handles/__pycache__/pdu.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7999 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/handles/__pycache__/perf.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1624 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/handles/__pycache__/pr.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2630 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/handles/__pycache__/repo.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3923 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)    10941 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/handles/pr.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3359 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/handles/repo.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2831 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/report03.csv
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       74 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/requirements.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4367 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/run.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.498300 br-ci-sdk-0.0.3/brci/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/schemas/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.498300 br-ci-sdk-0.0.3/brci/schemas/__pycache__/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      150 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/schemas/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1016 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/schemas/__pycache__/jenkins.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1080 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/schemas/__pycache__/pull_request.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      484 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/schemas/__pycache__/pull_request_job.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      389 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/schemas/__pycache__/test_case.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      527 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/schemas/test_case.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1727 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/temp_last.csv
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      550 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/test_hander_perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      355 2023-06-01 10:48:41.000000 br-ci-sdk-0.0.3/brci/test_pod.yml
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.498300 br-ci-sdk-0.0.3/brci/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/utils/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:56:47.498300 br-ci-sdk-0.0.3/brci/utils/__pycache__/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      148 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/utils/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1623 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/utils/__pycache__/csv_utils.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1049 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/utils/__pycache__/file_utils.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      618 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/utils/__pycache__/json_utils.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      300 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/utils/__pycache__/pd_utils.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      834 2023-06-01 10:48:48.000000 br-ci-sdk-0.0.3/brci/utils/__pycache__/xml_utils.cpython-39.pyc
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1304 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-06-01 10:44:13.000000 br-ci-sdk-0.0.3/brci/utils/xml_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-06-01 10:56:47.498300 br-ci-sdk-0.0.3/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1370 2023-06-01 10:56:34.000000 br-ci-sdk-0.0.3/setup.py
```

### Comparing `br-ci-sdk-0.0.2/PKG-INFO` & `br-ci-sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: br-ci-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `br-ci-sdk-0.0.2/README.md` & `br-ci-sdk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/apis/build.py` & `br-ci-sdk-0.0.3/brci/apis/build.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/apis/client.py` & `br-ci-sdk-0.0.3/brci/apis/client.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/apis/pdu.py` & `br-ci-sdk-0.0.3/brci/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/apis/perf.py` & `br-ci-sdk-0.0.3/brci/apis/perf.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/apis/pr.py` & `br-ci-sdk-0.0.3/brci/apis/pr.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/br_ci_sdk.egg-info/PKG-INFO` & `br-ci-sdk-0.0.3/br_ci_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: br-ci-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `br-ci-sdk-0.0.2/handles/build.py` & `br-ci-sdk-0.0.3/brci/handles/build.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/handles/pdu.py` & `br-ci-sdk-0.0.3/brci/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/handles/perf.py` & `br-ci-sdk-0.0.3/brci/handles/perf.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/handles/pr.py` & `br-ci-sdk-0.0.3/brci/handles/pr.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/handles/repo.py` & `br-ci-sdk-0.0.3/brci/handles/repo.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/schemas/jenkins.py` & `br-ci-sdk-0.0.3/brci/schemas/jenkins.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/schemas/pull_request.py` & `br-ci-sdk-0.0.3/brci/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/setup.py` & `br-ci-sdk-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import os
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 
 def _process_requirements():
-    packages = open('./requirements.txt').read().strip().split('\n')
+    packages = open('./brci/requirements.txt').read().strip().split('\n')
     requires = []
     for pkg in packages:
         if pkg.startswith('git+ssh'):
             return_code = os.system('pip install {}'.format(pkg))
             assert return_code == 0, 'error, status_code is: {}, exit!'.format(return_code)
         else:
             requires.append(pkg)
     return requires
 
 
 setuptools.setup(
     name="br-ci-sdk", 
-    version="0.0.2",    
+    version="0.0.3",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
@@ -38,11 +38,11 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6', 
     install_requires=_process_requirements(),
     include_package_data=True,
         entry_points={
         'console_scripts': [
-            'brci-cmd = run:main',
+            'brci-cmd = brci.run:main',
         ],
         }
 )
```

### Comparing `br-ci-sdk-0.0.2/utils/csv_utils.py` & `br-ci-sdk-0.0.3/brci/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.2/utils/xml_utils.py` & `br-ci-sdk-0.0.3/brci/utils/xml_utils.py`

 * *Files identical despite different names*

