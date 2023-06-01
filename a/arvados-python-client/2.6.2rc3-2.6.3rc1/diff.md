# Comparing `tmp/arvados-python-client-2.6.2rc3.tar.gz` & `tmp/arvados-python-client-2.6.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-python-client-2.6.2rc3.tar", last modified: Mon May  1 21:19:59 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-python-client-2.6.3rc1.tar", last modified: Thu Jun  1 21:38:11 2023, max compression
```

## Comparing `arvados-python-client-2.6.2rc3.tar` & `arvados-python-client-2.6.3rc1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2088 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6450 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/_normalize_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3492 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/_pycurlhelper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/_ranges.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17005 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    49239 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    76777 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/collection.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados/commands/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2125 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/_util.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    31921 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/arv_copy.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18701 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/federation_migrate.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13261 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23760 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3357 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11841 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/migrate19.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57541 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/run.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4765 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1629 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/config.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      896 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/diskcache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12489 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/http_to_keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    61777 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8472 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2635 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3750 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/timer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19413 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/vocabulary.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2032 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      343 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-copy
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-federation-migrate
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-get
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-keepdocker
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-ls
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-migrate-docker19
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-normalize
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-put
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-ws
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2141 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10182 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/arvados_testutil.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/keepstub.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/manifest_examples.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/tests/performance/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/performance/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/performance/performance_profiler.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/performance/test_a_sample.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    38152 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/run_test_server.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/slow_test.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18619 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_copy.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8686 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_normalize.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43464 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_benchmark_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77435 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18037 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    82578 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_keep_client.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_keep_locator.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2425 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_retry_job_helpers.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_sdk.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11619 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7865 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2088 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6450 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/_normalize_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3492 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/_pycurlhelper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/_ranges.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17498 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    49239 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    76741 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/collection.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados/commands/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2127 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/_util.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    32047 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/arv_copy.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18836 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/federation_migrate.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13287 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23786 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3383 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11841 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/migrate19.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57567 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/run.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1629 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/config.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      896 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/diskcache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12489 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/http_to_keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    61779 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8235 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2635 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3751 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/timer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19413 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2032 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      343 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-copy
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-federation-migrate
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-get
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-keepdocker
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-ls
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-migrate-docker19
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-normalize
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-put
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-ws
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2141 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10197 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/arvados_testutil.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/keepstub.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/manifest_examples.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/tests/performance/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/performance/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/performance/performance_profiler.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/performance/test_a_sample.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    38152 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/run_test_server.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/slow_test.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21197 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_copy.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8686 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_normalize.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43528 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_benchmark_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77433 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18037 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_http.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    83499 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_keep_client.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_keep_locator.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2440 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_retry_job_helpers.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_sdk.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11337 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7865 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_vocabulary.py
```

### Comparing `arvados-python-client-2.6.2rc3/LICENSE-2.0.txt` & `arvados-python-client-2.6.3rc1/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/PKG-INFO` & `arvados-python-client-2.6.3rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.6.2rc3
+Version: 2.6.3rc1
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.6.2rc3/README.rst` & `arvados-python-client-2.6.3rc1/README.rst`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/__init__.py` & `arvados-python-client-2.6.3rc1/arvados/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/_normalize_stream.py` & `arvados-python-client-2.6.3rc1/arvados/_normalize_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/_pycurlhelper.py` & `arvados-python-client-2.6.3rc1/arvados/_pycurlhelper.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/_ranges.py` & `arvados-python-client-2.6.3rc1/arvados/_ranges.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/api.py` & `arvados-python-client-2.6.3rc1/arvados/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,27 +23,37 @@
 import socket
 import ssl
 import sys
 import time
 import types
 
 import apiclient
+import apiclient.http
 from apiclient import discovery as apiclient_discovery
 from apiclient import errors as apiclient_errors
 from . import config
 from . import errors
+from . import retry
 from . import util
 from . import cache
 
 _logger = logging.getLogger('arvados.api')
 
 MAX_IDLE_CONNECTION_DURATION = 30
-RETRY_DELAY_INITIAL = 2
-RETRY_DELAY_BACKOFF = 2
-RETRY_COUNT = 2
+
+# These constants supported our own retry logic that we've since removed in
+# favor of using googleapiclient's num_retries. They're kept here purely for
+# API compatibility, but set to 0 to indicate no retries happen.
+RETRY_DELAY_INITIAL = 0
+RETRY_DELAY_BACKOFF = 0
+RETRY_COUNT = 0
+
+# An unused HTTP 5xx status code to request a retry internally.
+# See _intercept_http_request. This should not be user-visible.
+_RETRY_4XX_STATUS = 545
 
 if sys.version_info >= (3,):
     httplib2.SSLHandshakeError = None
 
 class OrderedJsonModel(apiclient.model.JsonModel):
     """Model class for JSON that preserves the contents' order.
 
@@ -60,84 +70,80 @@
         content = content.decode('utf-8')
         body = json.loads(content, object_pairs_hook=collections.OrderedDict)
         if self._data_wrapper and isinstance(body, dict) and 'data' in body:
             body = body['data']
         return body
 
 
+_orig_retry_request = apiclient.http._retry_request
+def _retry_request(http, num_retries, *args, **kwargs):
+    try:
+        num_retries = max(num_retries, http.num_retries)
+    except AttributeError:
+        # `http` client object does not have a `num_retries` attribute.
+        # It apparently hasn't gone through _patch_http_request, possibly
+        # because this isn't an Arvados API client. Pass through to
+        # avoid interfering with other Google API clients.
+        return _orig_retry_request(http, num_retries, *args, **kwargs)
+    response, body = _orig_retry_request(http, num_retries, *args, **kwargs)
+    # If _intercept_http_request ran out of retries for a 4xx response,
+    # restore the original status code.
+    if response.status == _RETRY_4XX_STATUS:
+        response.status = int(response['status'])
+    return (response, body)
+apiclient.http._retry_request = _retry_request
+
 def _intercept_http_request(self, uri, method="GET", headers={}, **kwargs):
     if not headers.get('X-Request-Id'):
         headers['X-Request-Id'] = self._request_id()
     try:
         if (self.max_request_size and
             kwargs.get('body') and
             self.max_request_size < len(kwargs['body'])):
             raise apiclient_errors.MediaUploadSizeError("Request size %i bytes exceeds published limit of %i bytes" % (len(kwargs['body']), self.max_request_size))
 
         headers['Authorization'] = 'OAuth2 %s' % self.arvados_api_token
 
-        retryable = method in [
-            'DELETE', 'GET', 'HEAD', 'OPTIONS', 'PUT']
-        retry_count = self._retry_count if retryable else 0
-
-        if (not retryable and
-            time.time() - self._last_request_time > self._max_keepalive_idle):
+        if (time.time() - self._last_request_time) > self._max_keepalive_idle:
             # High probability of failure due to connection atrophy. Make
             # sure this request [re]opens a new connection by closing and
             # forgetting all cached connections first.
             for conn in self.connections.values():
                 conn.close()
             self.connections.clear()
 
-        delay = self._retry_delay_initial
-        for _ in range(retry_count):
-            self._last_request_time = time.time()
-            try:
-                return self.orig_http_request(uri, method, headers=headers, **kwargs)
-            except http.client.HTTPException:
-                _logger.debug("[%s] Retrying API request in %d s after HTTP error",
-                              headers['X-Request-Id'], delay, exc_info=True)
-            except ssl.SSLCertVerificationError as e:
-                raise ssl.SSLCertVerificationError(e.args[0], "Could not connect to %s\n%s\nPossible causes: remote SSL/TLS certificate expired, or was issued by an untrusted certificate authority." % (uri, e)) from None
-            except socket.error:
-                # This is the one case where httplib2 doesn't close the
-                # underlying connection first.  Close all open
-                # connections, expecting this object only has the one
-                # connection to the API server.  This is safe because
-                # httplib2 reopens connections when needed.
-                _logger.debug("[%s] Retrying API request in %d s after socket error",
-                              headers['X-Request-Id'], delay, exc_info=True)
-                for conn in self.connections.values():
-                    conn.close()
-
-            time.sleep(delay)
-            delay = delay * self._retry_delay_backoff
-
         self._last_request_time = time.time()
-        return self.orig_http_request(uri, method, headers=headers, **kwargs)
+        try:
+            response, body = self.orig_http_request(uri, method, headers=headers, **kwargs)
+        except ssl.SSLCertVerificationError as e:
+            raise ssl.SSLCertVerificationError(e.args[0], "Could not connect to %s\n%s\nPossible causes: remote SSL/TLS certificate expired, or was issued by an untrusted certificate authority." % (uri, e)) from None
+        # googleapiclient only retries 403, 429, and 5xx status codes.
+        # If we got another 4xx status that we want to retry, convert it into
+        # 5xx so googleapiclient handles it the way we want.
+        if response.status in retry._HTTP_CAN_RETRY and response.status < 500:
+            response.status = _RETRY_4XX_STATUS
+        return (response, body)
     except Exception as e:
         # Prepend "[request_id] " to the error message, which we
         # assume is the first string argument passed to the exception
         # constructor.
         for i in range(len(e.args or ())):
             if type(e.args[i]) == type(""):
                 e.args = e.args[:i] + ("[{}] {}".format(headers['X-Request-Id'], e.args[i]),) + e.args[i+1:]
                 raise type(e)(*e.args)
         raise
 
-def _patch_http_request(http, api_token):
+def _patch_http_request(http, api_token, num_retries):
     http.arvados_api_token = api_token
     http.max_request_size = 0
+    http.num_retries = num_retries
     http.orig_http_request = http.request
     http.request = types.MethodType(_intercept_http_request, http)
     http._last_request_time = 0
     http._max_keepalive_idle = MAX_IDLE_CONNECTION_DURATION
-    http._retry_delay_initial = RETRY_DELAY_INITIAL
-    http._retry_delay_backoff = RETRY_DELAY_BACKOFF
-    http._retry_count = RETRY_COUNT
     http._request_id = util.new_request_id
     return http
 
 def _close_connections(self):
     for conn in self._http.connections.values():
         conn.close()
 
@@ -178,14 +184,15 @@
         version,
         discoveryServiceUrl,
         token,
         *,
         cache=True,
         http=None,
         insecure=False,
+        num_retries=10,
         request_id=None,
         timeout=5*60,
         **kwargs,
 ):
     """Build an Arvados API client
 
     This function returns a `googleapiclient.discovery.Resource` object
@@ -215,14 +222,18 @@
     : The HTTP client object the API client object will use to make requests.
       If not provided, this function will build its own to use. Either way, the
       object will be patched as part of the build process.
 
     insecure: bool
     : If true, ignore SSL certificate validation errors. Default `False`.
 
+    num_retries: int
+    : The number of times to retry each API request if it encounters a
+      temporary failure. Default 10.
+
     request_id: str | None
     : Default `X-Request-Id` header value for outgoing requests that
       don't already provide one. If `None` or omitted, generate a random
       ID. When retrying failed requests, the same ID is used on all
       attempts.
 
     timeout: int
@@ -235,21 +246,22 @@
         http = httplib2.Http(
             ca_certs=util.ca_certs_path(),
             cache=http_cache('discovery') if cache else None,
             disable_ssl_certificate_validation=bool(insecure),
         )
     if http.timeout is None:
         http.timeout = timeout
-    http = _patch_http_request(http, token)
+    http = _patch_http_request(http, token, num_retries)
 
     svc = apiclient_discovery.build(
         'arvados', version,
         cache_discovery=False,
         discoveryServiceUrl=discoveryServiceUrl,
         http=http,
+        num_retries=num_retries,
         **kwargs,
     )
     svc.api_token = token
     svc.insecure = insecure
     svc.request_id = request_id
     svc.config = lambda: util.get_config_once(svc)
     svc.vocabulary = lambda: util.get_vocabulary_once(svc)
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/arvfile.py` & `arvados-python-client-2.6.3rc1/arvados/arvfile.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/cache.py` & `arvados-python-client-2.6.3rc1/arvados/cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/collection.py` & `arvados-python-client-2.6.3rc1/arvados/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1252,15 +1252,15 @@
     initialization, or using `save_new`) to use `save` or `update`
 
     """
 
     def __init__(self, manifest_locator_or_text=None,
                  api_client=None,
                  keep_client=None,
-                 num_retries=None,
+                 num_retries=10,
                  parent=None,
                  apiconfig=None,
                  block_manager=None,
                  replication_desired=None,
                  storage_classes_desired=None,
                  put_threads=None,
                  get_threads=None):
@@ -1320,15 +1320,15 @@
         self.get_threads = get_threads
 
         if apiconfig:
             self._config = apiconfig
         else:
             self._config = config.settings()
 
-        self.num_retries = num_retries if num_retries is not None else 0
+        self.num_retries = num_retries
         self._manifest_locator = None
         self._manifest_text = None
         self._portable_data_hash = None
         self._api_response = None
         self._past_versions = set()
 
         self.lock = threading.RLock()
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/_util.py` & `arvados-python-client-2.6.3rc1/arvados/commands/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 def _pos_int(s):
     num = int(s)
     if num < 0:
         raise ValueError("can't accept negative value: %s" % (num,))
     return num
 
 retry_opt = argparse.ArgumentParser(add_help=False)
-retry_opt.add_argument('--retries', type=_pos_int, default=3, help="""
+retry_opt.add_argument('--retries', type=_pos_int, default=10, help="""
 Maximum number of times to retry server requests that encounter temporary
-failures (e.g., server down).  Default 3.""")
+failures (e.g., server down).  Default 10.""")
 
 def _ignore_error(error):
     return None
 
 def _raise_error(error):
     raise error
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/arv_copy.py` & `arvados-python-client-2.6.3rc1/arvados/commands/arv_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,16 @@
     else:
         logger.setLevel(logging.INFO)
 
     if not args.source_arvados:
         args.source_arvados = args.object_uuid[:5]
 
     # Create API clients for the source and destination instances
-    src_arv = api_for_instance(args.source_arvados)
-    dst_arv = api_for_instance(args.destination_arvados)
+    src_arv = api_for_instance(args.source_arvados, args.retries)
+    dst_arv = api_for_instance(args.destination_arvados, args.retries)
 
     if not args.project_uuid:
         args.project_uuid = dst_arv.users().current().execute(num_retries=args.retries)["uuid"]
 
     # Identify the kind of object we have been given, and begin copying.
     t = uuid_type(src_arv, args.object_uuid)
     if t == 'Collection':
@@ -183,15 +183,15 @@
 #     If instance_name contains a slash, it is presumed to be a path
 #     (either local or absolute) to a file with Arvados configuration
 #     settings.
 #
 #     Otherwise, it is presumed to be the name of a file in
 #     $HOME/.config/arvados/instance_name.conf
 #
-def api_for_instance(instance_name):
+def api_for_instance(instance_name, num_retries):
     if not instance_name:
         # Use environment
         return arvados.api('v1', model=OrderedJsonModel())
 
     if '/' in instance_name:
         config_file = instance_name
     else:
@@ -210,15 +210,17 @@
         api_is_insecure = (
             cfg.get('ARVADOS_API_HOST_INSECURE', '').lower() in set(
                 ['1', 't', 'true', 'y', 'yes']))
         client = arvados.api('v1',
                              host=cfg['ARVADOS_API_HOST'],
                              token=cfg['ARVADOS_API_TOKEN'],
                              insecure=api_is_insecure,
-                             model=OrderedJsonModel())
+                             model=OrderedJsonModel(),
+                             num_retries=num_retries,
+                             )
     else:
         abort('need ARVADOS_API_HOST and ARVADOS_API_TOKEN for {}'.format(instance_name))
     return client
 
 # Check if git is available
 def check_git_availability():
     try:
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/federation_migrate.py` & `arvados-python-client-2.6.3rc1/arvados/commands/federation_migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import argparse
 import hmac
 import urllib.parse
 import os
 import hashlib
 import re
 from arvados._version import __version__
+from . import _util as arv_cmd
 
 EMAIL=0
 USERNAME=1
 UUID=2
 HOMECLUSTER=3
 
 def connect_clusters(args):
@@ -39,18 +40,18 @@
         with open(args.tokens, "rt") as f:
             for r in csv.reader(f):
                 if len(r) != 2:
                     continue
                 host = r[0]
                 token = r[1]
                 print("Contacting %s" % (host))
-                arv = arvados.api(host=host, token=token, cache=False)
+                arv = arvados.api(host=host, token=token, cache=False, num_retries=args.retries)
                 clusters[arv._rootDesc["uuidPrefix"]] = arv
     else:
-        arv = arvados.api(cache=False)
+        arv = arvados.api(cache=False, num_retries=args.retries)
         rh = arv._rootDesc["remoteHosts"]
         tok = arv.api_client_authorizations().current().execute()
         token = "v2/%s/%s" % (tok["uuid"], tok["api_token"])
 
         for k,v in rh.items():
             arv = arvados.api(host=v, token=token, cache=False, insecure=os.environ.get("ARVADOS_API_HOST_INSECURE"))
             clusters[k] = arv
@@ -322,15 +323,18 @@
             target_owner, rsc_name, rsc_type = name_collision.groups()
             print("(%s) Cannot migrate to %s because both origin and target users have a %s named '%s'. Please rename the conflicting items or use --data-into-subproject to migrate all users' data into a special subproject." % (email, target_owner, rsc_type[:-1], rsc_name))
         else:
             print("(%s) Skipping user migration because of error: %s" % (email, e))
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Migrate users to federated identity, see https://doc.arvados.org/admin/merge-remote-account.html')
+    parser = argparse.ArgumentParser(
+        description='Migrate users to federated identity, see https://doc.arvados.org/admin/merge-remote-account.html',
+        parents=[arv_cmd.retry_opt],
+    )
     parser.add_argument(
         '--version', action='version', version="%s %s" % (sys.argv[0], __version__),
         help='Print version and exit.')
     parser.add_argument('--tokens', type=str, metavar='FILE', required=False, help="Read tokens from FILE. Not needed when using LoginCluster.")
     parser.add_argument('--data-into-subproject', action="store_true", help="Migrate user's data into a separate subproject. This can be used to avoid name collisions from within an account.")
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument('--report', type=str, metavar='FILE', help="Generate report .csv file listing users by email address and their associated Arvados accounts.")
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/get.py` & `arvados-python-client-2.6.3rc1/arvados/commands/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
     args = parse_arguments(arguments, stdout, stderr)
     logger.setLevel(logging.WARNING - 10 * args.v)
 
     request_id = arvados.util.new_request_id()
     logger.info('X-Request-Id: '+request_id)
 
-    api_client = arvados.api('v1', request_id=request_id)
+    api_client = arvados.api('v1', request_id=request_id, num_retries=args.retries)
 
     r = re.search(r'^(.*?)(/.*)?$', args.locator)
     col_loc = r.group(1)
     get_prefix = r.group(2)
     if args.r and not get_prefix:
         get_prefix = os.sep
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/keepdocker.py` & `arvados-python-client-2.6.3rc1/arvados/commands/keepdocker.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         filters=[['uuid', '=', uuid]],
         select=['portable_data_hash'],
     ).execute()['items'][0]['portable_data_hash']
 
 def main(arguments=None, stdout=sys.stdout, install_sig_handlers=True, api=None):
     args = arg_parser.parse_args(arguments)
     if api is None:
-        api = arvados.api('v1')
+        api = arvados.api('v1', num_retries=args.retries)
 
     if args.image is None or args.image == 'images':
         fmt = "{:30}  {:10}  {:12}  {:29}  {:20}\n"
         stdout.write(fmt.format("REPOSITORY", "TAG", "IMAGE ID", "COLLECTION", "CREATED"))
         try:
             for i, j in list_images_in_arv(api, args.retries):
                 stdout.write(fmt.format(j["repo"], j["tag"], j["dockerhash"][0:12], i, j["timestamp"].strftime("%c")))
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/ls.py` & `arvados-python-client-2.6.3rc1/arvados/commands/ls.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def name_formatter(coll_file):
     return "{}/{}".format(coll_file.stream_name, coll_file.name)
 
 def main(args, stdout, stderr, api_client=None, logger=None):
     args = parse_args(args)
 
     if api_client is None:
-        api_client = arvados.api('v1')
+        api_client = arvados.api('v1', num_retries=args.retries)
 
     if logger is None:
         logger = logging.getLogger('arvados.arv-ls')
 
     try:
         r = re.search(r'^(.*?)(/.*)?$', args.locator)
         collection = r.group(1)
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/migrate19.py` & `arvados-python-client-2.6.3rc1/arvados/commands/migrate19.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/put.py` & `arvados-python-client-2.6.3rc1/arvados/commands/put.py`

 * *Files 0% similar despite different names*

```diff
@@ -1132,15 +1132,15 @@
 
     request_id = arvados.util.new_request_id()
 
     formatter = ArvPutLogFormatter(request_id)
     logging.getLogger('arvados').handlers[0].setFormatter(formatter)
 
     if api_client is None:
-        api_client = arvados.api('v1', request_id=request_id)
+        api_client = arvados.api('v1', request_id=request_id, num_retries=args.retries)
 
     if install_sig_handlers:
         arv_cmd.install_signal_handlers()
 
     # Trash arguments validation
     trash_at = None
     if args.trash_at is not None:
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/run.py` & `arvados-python-client-2.6.3rc1/arvados/commands/run.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/commands/ws.py` & `arvados-python-client-2.6.3rc1/arvados/commands/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import sys
 import logging
 import argparse
 import arvados
 import json
 from arvados.events import subscribe
 from arvados._version import __version__
+from . import _util as arv_cmd
 import signal
 
 def main(arguments=None):
     logger = logging.getLogger('arvados.arv-ws')
 
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(parents=[arv_cmd.retry_opt])
     parser.add_argument('--version', action='version',
                         version="%s %s" % (sys.argv[0], __version__),
                         help='Print version and exit.')
     parser.add_argument('-u', '--uuid', type=str, default="", help="Filter events on object_uuid")
     parser.add_argument('-f', '--filters', type=str, default="", help="Arvados query filter to apply to log events (JSON encoded)")
     parser.add_argument('-s', '--start-time', type=str, default="", help="Arvados query filter to fetch log events created at or after this time. This will be server time in UTC. Allowed format: YYYY-MM-DD or YYYY-MM-DD hh:mm:ss")
     parser.add_argument('-i', '--id', type=int, default=None, help="Start from given log id.")
@@ -52,15 +53,15 @@
         if known_component_jobs != pipeline_jobs:
             new_filters = [['object_uuid', 'in', [args.pipeline] + list(pipeline_jobs)]]
             ws.subscribe(new_filters)
             ws.unsubscribe(filters)
             filters = new_filters
             known_component_jobs = pipeline_jobs
 
-    api = arvados.api('v1')
+    api = arvados.api('v1', num_retries=args.retries)
 
     if args.uuid:
         filters += [ ['object_uuid', '=', args.uuid] ]
 
     if args.filters:
         filters += json.loads(args.filters)
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/config.py` & `arvados-python-client-2.6.3rc1/arvados/config.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/crunch.py` & `arvados-python-client-2.6.3rc1/arvados/crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/diskcache.py` & `arvados-python-client-2.6.3rc1/arvados/diskcache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/errors.py` & `arvados-python-client-2.6.3rc1/arvados/errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/events.py` & `arvados-python-client-2.6.3rc1/arvados/events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/http_to_keep.py` & `arvados-python-client-2.6.3rc1/arvados/http_to_keep.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/keep.py` & `arvados-python-client-2.6.3rc1/arvados/keep.py`

 * *Files 0% similar despite different names*

```diff
@@ -831,15 +831,15 @@
 
             return result['body'].strip(), replicas_stored, classes_confirmed
 
 
     def __init__(self, api_client=None, proxy=None,
                  timeout=DEFAULT_TIMEOUT, proxy_timeout=DEFAULT_PROXY_TIMEOUT,
                  api_token=None, local_store=None, block_cache=None,
-                 num_retries=0, session=None):
+                 num_retries=10, session=None):
         """Initialize a new KeepClient.
 
         Arguments:
         :api_client:
           The API client to use to find Keep services.  If not
           provided, KeepClient will build one from available Arvados
           configuration.
@@ -884,15 +884,15 @@
           environment variable.  If you want to ensure KeepClient does not
           use local storage, pass in an empty string.  This is primarily
           intended to mock a server for testing.
 
         :num_retries:
           The default number of times to retry failed requests.
           This will be used as the default num_retries value when get() and
-          put() are called.  Default 0.
+          put() are called.  Default 10.
         """
         self.lock = threading.Lock()
         if proxy is None:
             if config.get('ARVADOS_KEEP_SERVICES'):
                 proxy = config.get('ARVADOS_KEEP_SERVICES')
             else:
                 proxy = config.get('ARVADOS_KEEP_PROXY')
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/retry.py` & `arvados-python-client-2.6.3rc1/arvados/retry.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import time
 
 from collections import deque
 
 import arvados.errors
 
 _HTTP_SUCCESSES = set(range(200, 300))
-_HTTP_CAN_RETRY = set([408, 409, 422, 423, 500, 502, 503, 504])
+_HTTP_CAN_RETRY = set([408, 409, 423, 500, 502, 503, 504])
 
 class RetryLoop(object):
     """Coordinate limited retries of code.
 
     `RetryLoop` coordinates a loop that runs until it records a
     successful result or tries too many times, whichever comes first.
     Typical use looks like:
@@ -196,18 +196,14 @@
     failure, and `False` otherwise.  You can use this as the
     `success_check` for a `RetryLoop` that queries the Arvados API server.
     Specifically:
 
     * Any 2xx result returns `True`.
 
     * A select few status codes, or any malformed responses, return `None`.
-      422 Unprocessable Entity is in this category.  This may not meet the
-      letter of the HTTP specification, but the Arvados API server will
-      use it for various server-side problems like database connection
-      errors.
 
     * Everything else returns `False`.  Note that this includes 1xx and
       3xx status codes.  They don't indicate success, and you can't
       retry those requests verbatim.
 
     Arguments:
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/safeapi.py` & `arvados-python-client-2.6.3rc1/arvados/safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/stream.py` & `arvados-python-client-2.6.3rc1/arvados/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from arvados.keep import *
 from . import config
 from . import errors
 from ._normalize_stream import normalize_stream
 
 class StreamReader(object):
     def __init__(self, tokens, keep=None, debug=False, _empty=False,
-                 num_retries=0):
+                 num_retries=10):
         self._stream_name = None
         self._data_locators = []
         self._files = collections.OrderedDict()
         self._keep = keep
         self.num_retries = num_retries
 
         streamoffset = 0
```

### Comparing `arvados-python-client-2.6.2rc3/arvados/timer.py` & `arvados-python-client-2.6.3rc1/arvados/timer.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/util.py` & `arvados-python-client-2.6.3rc1/arvados/util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados/vocabulary.py` & `arvados-python-client-2.6.3rc1/arvados/vocabulary.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/PKG-INFO` & `arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.6.2rc3
+Version: 2.6.3rc1
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/SOURCES.txt` & `arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/arvados_version.py` & `arvados-python-client-2.6.3rc1/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/bin/arv-normalize` & `arvados-python-client-2.6.3rc1/bin/arv-normalize`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/setup.py` & `arvados-python-client-2.6.3rc1/setup.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/arvados_testutil.py` & `arvados-python-client-2.6.3rc1/tests/arvados_testutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,18 @@
 
 def mock_responses(body, *codes, **headers):
     if not isinstance(body, bytes) and hasattr(body, 'encode'):
         body = body.encode()
     return mock.patch('httplib2.Http.request', side_effect=queue_with((
         (fake_httplib2_response(code, **headers), body) for code in codes)))
 
-def mock_api_responses(api_client, body, codes, headers={}):
+def mock_api_responses(api_client, body, codes, headers={}, method='request'):
     if not isinstance(body, bytes) and hasattr(body, 'encode'):
         body = body.encode()
-    return mock.patch.object(api_client._http, 'request', side_effect=queue_with((
+    return mock.patch.object(api_client._http, method, side_effect=queue_with((
         (fake_httplib2_response(code, **headers), body) for code in codes)))
 
 def str_keep_locator(s):
     return '{}+{}'.format(hashlib.md5(s if isinstance(s, bytes) else s.encode()).hexdigest(), len(s))
 
 @contextlib.contextmanager
 def redirected_streams(stdout=None, stderr=None):
```

### Comparing `arvados-python-client-2.6.2rc3/tests/keepstub.py` & `arvados-python-client-2.6.3rc1/tests/keepstub.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/manifest_examples.py` & `arvados-python-client-2.6.3rc1/tests/manifest_examples.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/performance/performance_profiler.py` & `arvados-python-client-2.6.3rc1/tests/performance/performance_profiler.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/run_test_server.py` & `arvados-python-client-2.6.3rc1/tests/run_test_server.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_api.py` & `arvados-python-client-2.6.3rc1/tests/test_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,46 +3,46 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import absolute_import
 from builtins import str
 from builtins import range
 import arvados
 import collections
+import contextlib
 import httplib2
 import itertools
 import json
 import mimetypes
 import os
 import socket
 import string
+import sys
 import unittest
 import urllib.parse as urlparse
 
 import mock
 from . import run_test_server
 
 from apiclient import errors as apiclient_errors
 from apiclient import http as apiclient_http
 from arvados.api import (
     api_client,
     normalize_api_kwargs,
     api_kwargs_from_config,
     OrderedJsonModel,
-    RETRY_DELAY_INITIAL,
-    RETRY_DELAY_BACKOFF,
-    RETRY_COUNT,
 )
-from .arvados_testutil import fake_httplib2_response, queue_with
+from .arvados_testutil import fake_httplib2_response, mock_api_responses, queue_with
 
 if not mimetypes.inited:
     mimetypes.init()
 
 class ArvadosApiTest(run_test_server.TestCaseWithServers):
     MAIN_SERVER = {}
     ERROR_HEADERS = {'Content-Type': mimetypes.types_map['.json']}
+    RETRIED_4XX = frozenset([408, 409, 423])
 
     def api_error_response(self, code, *errors):
         return (fake_httplib2_response(code, **self.ERROR_HEADERS),
                 json.dumps({'errors': errors,
                             'error_token': '1234567890+12345678'}).encode())
 
     def _config_from_environ(self):
@@ -146,14 +146,65 @@
             "Default timeout value should be 300")
 
     def test_custom_request_timeout(self):
         api = arvados.api('v1', timeout=1234)
         self.assertEqual(api._http.timeout, 1234,
             "Requested timeout value was 1234")
 
+    def test_4xx_retried(self):
+        client = arvados.api('v1')
+        for code in self.RETRIED_4XX:
+            name = f'retried #{code}'
+            with self.subTest(name), mock.patch('time.sleep'):
+                expected = {'username': name}
+                with mock_api_responses(
+                        client,
+                        json.dumps(expected),
+                        [code, code, 200],
+                        self.ERROR_HEADERS,
+                        'orig_http_request',
+                ):
+                    actual = client.users().current().execute()
+                self.assertEqual(actual, expected)
+
+    def test_4xx_not_retried(self):
+        client = arvados.api('v1', num_retries=3)
+        # Note that googleapiclient does retry 403 *if* the response JSON
+        # includes flags that say the request was denied by rate limiting.
+        # An empty JSON response like we use here should not be retried.
+        for code in [400, 401, 403, 404, 422]:
+            with self.subTest(f'error {code}'), mock.patch('time.sleep'):
+                with mock_api_responses(
+                        client,
+                        b'{}',
+                        [code, 200],
+                        self.ERROR_HEADERS,
+                        'orig_http_request',
+                ), self.assertRaises(arvados.errors.ApiError) as exc_check:
+                    client.users().current().execute()
+                response = exc_check.exception.args[0]
+                self.assertEqual(response.status, code)
+                self.assertEqual(response.get('status'), str(code))
+
+    def test_4xx_raised_after_retry_exhaustion(self):
+        client = arvados.api('v1', num_retries=1)
+        for code in self.RETRIED_4XX:
+            with self.subTest(f'failed {code}'), mock.patch('time.sleep'):
+                with mock_api_responses(
+                        client,
+                        b'{}',
+                        [code, code, code, 200],
+                        self.ERROR_HEADERS,
+                        'orig_http_request',
+                ), self.assertRaises(arvados.errors.ApiError) as exc_check:
+                    client.users().current().execute()
+                response = exc_check.exception.args[0]
+                self.assertEqual(response.status, code)
+                self.assertEqual(response.get('status'), str(code))
+
     def test_ordered_json_model(self):
         mock_responses = {
             'arvados.humans.get': (
                 None,
                 json.dumps(collections.OrderedDict(
                     (c, int(c, 16)) for c in string.hexdigits
                 )).encode(),
@@ -337,79 +388,97 @@
             with self.subTest(f"api_client fails with {arg_index}={arg_value!r}"), \
                  self.assertRaises(apiclient_errors.UnknownApiNameOrVersion):
                 args = list(all_args)
                 args[arg_index] = arg_value
                 api_client(*args, insecure=True)
 
 
-class RetryREST(unittest.TestCase):
+class ConstructNumRetriesTestCase(unittest.TestCase):
+    @staticmethod
+    def _fake_retry_request(http, num_retries, req_type, sleep, rand, uri, method, *args, **kwargs):
+        return http.request(uri, method, *args, **kwargs)
+
+    @contextlib.contextmanager
+    def patch_retry(self):
+        # We have this dedicated context manager that goes through `sys.modules`
+        # instead of just using `mock.patch` because of the unfortunate
+        # `arvados.api` name collision.
+        orig_func = sys.modules['arvados.api']._orig_retry_request
+        expect_name = 'googleapiclient.http._retry_request'
+        self.assertEqual(
+            '{0.__module__}.{0.__name__}'.format(orig_func), expect_name,
+            f"test setup problem: {expect_name} not at arvados.api._orig_retry_request",
+        )
+        retry_mock = mock.Mock(wraps=self._fake_retry_request)
+        sys.modules['arvados.api']._orig_retry_request = retry_mock
+        try:
+            yield retry_mock
+        finally:
+            sys.modules['arvados.api']._orig_retry_request = orig_func
+
+    def _iter_num_retries(self, retry_mock):
+        for call in retry_mock.call_args_list:
+            try:
+                yield call.args[1]
+            except IndexError:
+                yield call.kwargs['num_retries']
+
+    def test_default_num_retries(self):
+        with self.patch_retry() as retry_mock:
+            client = arvados.api('v1')
+        actual = set(self._iter_num_retries(retry_mock))
+        self.assertEqual(len(actual), 1)
+        self.assertTrue(actual.pop() > 6, "num_retries lower than expected")
+
+    def _test_calls(self, init_arg, call_args, expected):
+        with self.patch_retry() as retry_mock:
+            client = arvados.api('v1', num_retries=init_arg)
+            for num_retries in call_args:
+                client.users().current().execute(num_retries=num_retries)
+        actual = self._iter_num_retries(retry_mock)
+        # The constructor makes two requests with its num_retries argument:
+        # one for the discovery document, and one for the config.
+        self.assertEqual(next(actual, None), init_arg)
+        self.assertEqual(next(actual, None), init_arg)
+        self.assertEqual(list(actual), expected)
+
+    def test_discovery_num_retries(self):
+        for num_retries in [0, 5, 55]:
+            with self.subTest(f"num_retries={num_retries}"):
+                self._test_calls(num_retries, [], [])
+
+    def test_num_retries_called_le_init(self):
+        for n in [6, 10]:
+            with self.subTest(f"init_arg={n}"):
+                call_args = [n - 4, n - 2, n]
+                expected = [n] * 3
+                self._test_calls(n, call_args, expected)
+
+    def test_num_retries_called_ge_init(self):
+        for n in [0, 10]:
+            with self.subTest(f"init_arg={n}"):
+                call_args = [n, n + 4, n + 8]
+                self._test_calls(n, call_args, call_args)
+
+    def test_num_retries_called_mixed(self):
+        self._test_calls(5, [2, 6, 4, 8], [5, 6, 5, 8])
+
+
+class PreCloseSocketTestCase(unittest.TestCase):
     def setUp(self):
         self.api = arvados.api('v1')
         self.assertTrue(hasattr(self.api._http, 'orig_http_request'),
                         "test doesn't know how to intercept HTTP requests")
         self.mock_response = {'user': 'person'}
         self.request_success = (fake_httplib2_response(200),
                                 json.dumps(self.mock_response))
         self.api._http.orig_http_request = mock.MagicMock()
         # All requests succeed by default. Tests override as needed.
         self.api._http.orig_http_request.return_value = self.request_success
 
-    @mock.patch('time.sleep')
-    def test_socket_error_retry_get(self, sleep):
-        self.api._http.orig_http_request.side_effect = (
-            socket.error('mock error'),
-            self.request_success,
-        )
-        self.assertEqual(self.api.users().current().execute(),
-                         self.mock_response)
-        self.assertGreater(self.api._http.orig_http_request.call_count, 1,
-                           "client got the right response without retrying")
-        self.assertEqual(sleep.call_args_list,
-                         [mock.call(RETRY_DELAY_INITIAL)])
-
-    @mock.patch('time.sleep')
-    def test_same_automatic_request_id_on_retry(self, sleep):
-        self.api._http.orig_http_request.side_effect = (
-            socket.error('mock error'),
-            self.request_success,
-        )
-        self.api.users().current().execute()
-        calls = self.api._http.orig_http_request.call_args_list
-        self.assertEqual(len(calls), 2)
-        self.assertEqual(
-            calls[0][1]['headers']['X-Request-Id'],
-            calls[1][1]['headers']['X-Request-Id'])
-        self.assertRegex(calls[0][1]['headers']['X-Request-Id'], r'^req-[a-z0-9]{20}$')
-
-    @mock.patch('time.sleep')
-    def test_provided_request_id_on_retry(self, sleep):
-        self.api.request_id='fake-request-id'
-        self.api._http.orig_http_request.side_effect = (
-            socket.error('mock error'),
-            self.request_success,
-        )
-        self.api.users().current().execute()
-        calls = self.api._http.orig_http_request.call_args_list
-        self.assertEqual(len(calls), 2)
-        for call in calls:
-            self.assertEqual(call[1]['headers']['X-Request-Id'], 'fake-request-id')
-
-    @mock.patch('time.sleep')
-    def test_socket_error_retry_delay(self, sleep):
-        self.api._http.orig_http_request.side_effect = socket.error('mock')
-        self.api._http._retry_count = 3
-        with self.assertRaises(socket.error):
-            self.api.users().current().execute()
-        self.assertEqual(self.api._http.orig_http_request.call_count, 4)
-        self.assertEqual(sleep.call_args_list, [
-            mock.call(RETRY_DELAY_INITIAL),
-            mock.call(RETRY_DELAY_INITIAL * RETRY_DELAY_BACKOFF),
-            mock.call(RETRY_DELAY_INITIAL * RETRY_DELAY_BACKOFF**2),
-        ])
-
     @mock.patch('time.time', side_effect=[i*2**20 for i in range(99)])
     def test_close_old_connections_non_retryable(self, sleep):
         self._test_connection_close(expect=1)
 
     @mock.patch('time.time', side_effect=itertools.count())
     def test_no_close_fresh_connections_non_retryable(self, sleep):
         self._test_connection_close(expect=0)
@@ -425,22 +494,10 @@
         self.api.users().create(body={}).execute()
         mock_conns = {str(i): mock.MagicMock() for i in range(2)}
         self.api._http.connections = mock_conns.copy()
         self.api.users().create(body={}).execute()
         for c in mock_conns.values():
             self.assertEqual(c.close.call_count, expect)
 
-    @mock.patch('time.sleep')
-    def test_socket_error_no_retry_post(self, sleep):
-        self.api._http.orig_http_request.side_effect = (
-            socket.error('mock error'),
-            self.request_success,
-        )
-        with self.assertRaises(socket.error):
-            self.api.users().create(body={}).execute()
-        self.assertEqual(self.api._http.orig_http_request.call_count, 1,
-                         "client should try non-retryable method exactly once")
-        self.assertEqual(sleep.call_args_list, [])
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arvados-python-client-2.6.2rc3/tests/test_arv_copy.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_arv_get.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_arv_keepdocker.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_arv_ls.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_arv_normalize.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_normalize.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_arv_put.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_arv_ws.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_arvfile.py` & `arvados-python-client-2.6.3rc1/tests/test_arvfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,30 +410,30 @@
 
             self.assertEqual(c.manifest_text(), ". 7f614da9329cd3aebf59b91aadc30bf0+67108864 781e5e245d69b566979b86e28d23f2c7+10 0:67108864:count.txt 0:67108864:count.txt 0:2:count.txt 67108864:10:count.txt\n")
 
     def test_sparse_write3(self):
         keep = ArvadosFileWriterTestCase.MockKeep({})
         api = ArvadosFileWriterTestCase.MockApi({}, {})
         for r in [[0, 1, 2, 3, 4], [4, 3, 2, 1, 0], [3, 2, 0, 4, 1]]:
-            with Collection() as c:
+            with Collection(api_client=api, keep_client=keep) as c:
                 writer = c.open("count.txt", "rb+")
                 self.assertEqual(writer.size(), 0)
 
                 for i in r:
                     w = ("%s" % i) * 10
                     writer.seek(i*10)
                     writer.write(w.encode())
                 writer.seek(0)
                 self.assertEqual(writer.read(), b"00000000001111111111222222222233333333334444444444")
 
     def test_sparse_write4(self):
         keep = ArvadosFileWriterTestCase.MockKeep({})
         api = ArvadosFileWriterTestCase.MockApi({}, {})
         for r in [[0, 1, 2, 4], [4, 2, 1, 0], [2, 0, 4, 1]]:
-            with Collection() as c:
+            with Collection(api_client=api, keep_client=keep) as c:
                 writer = c.open("count.txt", "rb+")
                 self.assertEqual(writer.size(), 0)
 
                 for i in r:
                     w = ("%s" % i) * 10
                     writer.seek(i*10)
                     writer.write(w.encode())
```

### Comparing `arvados-python-client-2.6.2rc3/tests/test_benchmark_collections.py` & `arvados-python-client-2.6.3rc1/tests/test_benchmark_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_cache.py` & `arvados-python-client-2.6.3rc1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_collections.py` & `arvados-python-client-2.6.3rc1/tests/test_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,19 +534,19 @@
         self._mock_api_call(api_mock.collections().get, code, body)
 
     def api_client_mock(self, status=200):
         client = super(CollectionReaderTestCase, self).api_client_mock()
         self.mock_get_collection(client, status, 'foo_file')
         return client
 
-    def test_init_no_default_retries(self):
+    def test_init_default_retries(self):
         client = self.api_client_mock(200)
         reader = arvados.CollectionReader(self.DEFAULT_UUID, api_client=client)
         reader.manifest_text()
-        client.collections().get().execute.assert_called_with(num_retries=0)
+        client.collections().get().execute.assert_called_with(num_retries=10)
 
     def test_uuid_init_success(self):
         client = self.api_client_mock(200)
         reader = arvados.CollectionReader(self.DEFAULT_UUID, api_client=client,
                                           num_retries=3)
         self.assertEqual(self.DEFAULT_COLLECTION['manifest_text'],
                          reader.manifest_text())
```

### Comparing `arvados-python-client-2.6.2rc3/tests/test_crunch.py` & `arvados-python-client-2.6.3rc1/tests/test_crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_errors.py` & `arvados-python-client-2.6.3rc1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_events.py` & `arvados-python-client-2.6.3rc1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_http.py` & `arvados-python-client-2.6.3rc1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_keep_client.py` & `arvados-python-client-2.6.3rc1/tests/test_keep_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     def test_recognize_proxy_services_in_controller_response(self):
         keep_client = arvados.KeepClient(api_client=self.mock_keep_services(
             service_type='proxy', service_host='localhost', service_port=9, count=1),
                                          block_cache=self.make_block_cache(self.disk_cache))
         try:
             # this will fail, but it ensures we get the service
             # discovery response
-            keep_client.put('baz2')
+            keep_client.put('baz2', num_retries=0)
         except:
             pass
         self.assertTrue(keep_client.using_proxy)
 
     def test_insecure_disables_tls_verify(self):
         api_client = self.mock_keep_services(count=1)
         force_timeout = socket.timeout("timed out")
@@ -334,15 +334,19 @@
     # whether pycurl actually exhibits the expected timeout behavior
     # -- those tests are in the KeepClientTimeout test class.
 
     def test_get_timeout(self):
         api_client = self.mock_keep_services(count=1)
         force_timeout = socket.timeout("timed out")
         with tutil.mock_keep_responses(force_timeout, 0) as mock:
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             with self.assertRaises(arvados.errors.KeepReadError):
                 keep_client.get('ffffffffffffffffffffffffffffffff')
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.CONNECTTIMEOUT_MS),
                 int(arvados.KeepClient.DEFAULT_TIMEOUT[0]*1000))
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.LOW_SPEED_TIME),
@@ -351,15 +355,19 @@
                 mock.responses[0].getopt(pycurl.LOW_SPEED_LIMIT),
                 int(arvados.KeepClient.DEFAULT_TIMEOUT[2]))
 
     def test_put_timeout(self):
         api_client = self.mock_keep_services(count=1)
         force_timeout = socket.timeout("timed out")
         with tutil.mock_keep_responses(force_timeout, 0) as mock:
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             with self.assertRaises(arvados.errors.KeepWriteError):
                 keep_client.put(b'foo')
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.CONNECTTIMEOUT_MS),
                 int(arvados.KeepClient.DEFAULT_TIMEOUT[0]*1000))
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.LOW_SPEED_TIME),
@@ -368,15 +376,19 @@
                 mock.responses[0].getopt(pycurl.LOW_SPEED_LIMIT),
                 int(arvados.KeepClient.DEFAULT_TIMEOUT[2]))
 
     def test_head_timeout(self):
         api_client = self.mock_keep_services(count=1)
         force_timeout = socket.timeout("timed out")
         with tutil.mock_keep_responses(force_timeout, 0) as mock:
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             with self.assertRaises(arvados.errors.KeepReadError):
                 keep_client.head('ffffffffffffffffffffffffffffffff')
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.CONNECTTIMEOUT_MS),
                 int(arvados.KeepClient.DEFAULT_TIMEOUT[0]*1000))
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.LOW_SPEED_TIME),
@@ -385,15 +397,19 @@
                 mock.responses[0].getopt(pycurl.LOW_SPEED_LIMIT),
                 None)
 
     def test_proxy_get_timeout(self):
         api_client = self.mock_keep_services(service_type='proxy', count=1)
         force_timeout = socket.timeout("timed out")
         with tutil.mock_keep_responses(force_timeout, 0) as mock:
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             with self.assertRaises(arvados.errors.KeepReadError):
                 keep_client.get('ffffffffffffffffffffffffffffffff')
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.CONNECTTIMEOUT_MS),
                 int(arvados.KeepClient.DEFAULT_PROXY_TIMEOUT[0]*1000))
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.LOW_SPEED_TIME),
@@ -402,15 +418,19 @@
                 mock.responses[0].getopt(pycurl.LOW_SPEED_LIMIT),
                 int(arvados.KeepClient.DEFAULT_PROXY_TIMEOUT[2]))
 
     def test_proxy_head_timeout(self):
         api_client = self.mock_keep_services(service_type='proxy', count=1)
         force_timeout = socket.timeout("timed out")
         with tutil.mock_keep_responses(force_timeout, 0) as mock:
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             with self.assertRaises(arvados.errors.KeepReadError):
                 keep_client.head('ffffffffffffffffffffffffffffffff')
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.CONNECTTIMEOUT_MS),
                 int(arvados.KeepClient.DEFAULT_PROXY_TIMEOUT[0]*1000))
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.LOW_SPEED_TIME),
@@ -420,15 +440,18 @@
                 None)
 
     def test_proxy_put_timeout(self):
         self.disk_cache_dir = None
         api_client = self.mock_keep_services(service_type='proxy', count=1)
         force_timeout = socket.timeout("timed out")
         with tutil.mock_keep_responses(force_timeout, 0) as mock:
-            keep_client = arvados.KeepClient(api_client=api_client)
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                num_retries=0,
+            )
             with self.assertRaises(arvados.errors.KeepWriteError):
                 keep_client.put('foo')
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.CONNECTTIMEOUT_MS),
                 int(arvados.KeepClient.DEFAULT_PROXY_TIMEOUT[0]*1000))
             self.assertEqual(
                 mock.responses[0].getopt(pycurl.LOW_SPEED_TIME),
@@ -437,15 +460,19 @@
                 mock.responses[0].getopt(pycurl.LOW_SPEED_LIMIT),
                 int(arvados.KeepClient.DEFAULT_PROXY_TIMEOUT[2]))
 
     def check_no_services_error(self, verb, exc_class):
         api_client = mock.MagicMock(name='api_client')
         api_client.keep_services().accessible().execute.side_effect = (
             arvados.errors.ApiError)
-        keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+        keep_client = arvados.KeepClient(
+            api_client=api_client,
+            block_cache=self.make_block_cache(self.disk_cache),
+            num_retries=0,
+        )
         with self.assertRaises(exc_class) as err_check:
             getattr(keep_client, verb)('d41d8cd98f00b204e9800998ecf8427e+0')
         self.assertEqual(0, len(err_check.exception.request_errors()))
 
     def test_get_error_with_no_services(self):
         self.check_no_services_error('get', arvados.errors.KeepReadError)
 
@@ -457,15 +484,19 @@
 
     def check_errors_from_last_retry(self, verb, exc_class):
         api_client = self.mock_keep_services(count=2)
         req_mock = tutil.mock_keep_responses(
             "retry error reporting test", 500, 500, 500, 500, 500, 500, 502, 502)
         with req_mock, tutil.skip_sleep, \
                 self.assertRaises(exc_class) as err_check:
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             getattr(keep_client, verb)('d41d8cd98f00b204e9800998ecf8427e+0',
                                        num_retries=3)
         self.assertEqual([502, 502], [
                 getattr(error, 'status_code', None)
                 for error in err_check.exception.request_errors().values()])
         self.assertRegex(str(err_check.exception), r'failed to (read|write) .* after 4 attempts')
 
@@ -480,55 +511,75 @@
 
     def test_put_error_does_not_include_successful_puts(self):
         data = 'partial failure test'
         data_loc = tutil.str_keep_locator(data)
         api_client = self.mock_keep_services(count=3)
         with tutil.mock_keep_responses(data_loc, 200, 500, 500) as req_mock, \
                 self.assertRaises(arvados.errors.KeepWriteError) as exc_check:
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             keep_client.put(data)
         self.assertEqual(2, len(exc_check.exception.request_errors()))
 
     def test_proxy_put_with_no_writable_services(self):
         data = 'test with no writable services'
         data_loc = tutil.str_keep_locator(data)
         api_client = self.mock_keep_services(service_type='proxy', read_only=True, count=1)
         with tutil.mock_keep_responses(data_loc, 200, 500, 500) as req_mock, \
                 self.assertRaises(arvados.errors.KeepWriteError) as exc_check:
-          keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
-          keep_client.put(data)
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
+            keep_client.put(data)
         self.assertEqual(True, ("no Keep services available" in str(exc_check.exception)))
         self.assertEqual(0, len(exc_check.exception.request_errors()))
 
     def test_oddball_service_get(self):
         body = b'oddball service get'
         api_client = self.mock_keep_services(service_type='fancynewblobstore')
         with tutil.mock_keep_responses(body, 200):
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             actual = keep_client.get(tutil.str_keep_locator(body))
         self.assertEqual(body, actual)
 
     def test_oddball_service_put(self):
         body = b'oddball service put'
         pdh = tutil.str_keep_locator(body)
         api_client = self.mock_keep_services(service_type='fancynewblobstore')
         with tutil.mock_keep_responses(pdh, 200):
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             actual = keep_client.put(body, copies=1)
         self.assertEqual(pdh, actual)
 
     def test_oddball_service_writer_count(self):
         body = b'oddball service writer count'
         pdh = tutil.str_keep_locator(body)
         api_client = self.mock_keep_services(service_type='fancynewblobstore',
                                              count=4)
         headers = {'x-keep-replicas-stored': 3}
         with tutil.mock_keep_responses(pdh, 200, 418, 418, 418,
                                        **headers) as req_mock:
-            keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
+            keep_client = arvados.KeepClient(
+                api_client=api_client,
+                block_cache=self.make_block_cache(self.disk_cache),
+                num_retries=0,
+            )
             actual = keep_client.put(body, copies=2)
         self.assertEqual(pdh, actual)
         self.assertEqual(1, req_mock.call_count)
 
 @tutil.skip_sleep
 @parameterized.parameterized_class([{"disk_cache": True}, {"disk_cache": False}])
 class KeepClientCacheTestCase(unittest.TestCase, tutil.ApiClientMock, DiskCacheBase):
@@ -634,15 +685,15 @@
 
     def test_partial_storage_classes_put(self):
         headers = {
             'x-keep-replicas-stored': 1,
             'x-keep-storage-classes-confirmed': 'foo=1'}
         with tutil.mock_keep_responses(self.locator, 200, 503, **headers) as mock:
             with self.assertRaises(arvados.errors.KeepWriteError):
-                self.keep_client.put(self.data, copies=1, classes=['foo', 'bar'])
+                self.keep_client.put(self.data, copies=1, classes=['foo', 'bar'], num_retries=0)
             # 1st request, both classes pending
             req1_headers = mock.responses[0].getopt(pycurl.HTTPHEADER)
             self.assertIn('X-Keep-Storage-Classes: bar, foo', req1_headers)
             # 2nd try, 'foo' class already satisfied
             req2_headers = mock.responses[1].getopt(pycurl.HTTPHEADER)
             self.assertIn('X-Keep-Storage-Classes: bar', req2_headers)
 
@@ -685,15 +736,15 @@
         for w_copies, w_classes, c_copies, c_classes, return_code in cases:
             headers = {'x-keep-replicas-stored': c_copies}
             if c_classes is not None:
                 headers.update({'x-keep-storage-classes-confirmed': c_classes})
             with tutil.mock_keep_responses(self.locator, return_code, return_code, **headers):
                 case_desc = 'wanted_copies={}, wanted_classes="{}", confirmed_copies={}, confirmed_classes="{}"'.format(w_copies, ', '.join(w_classes), c_copies, c_classes)
                 with self.assertRaises(arvados.errors.KeepWriteError, msg=case_desc):
-                    self.keep_client.put(self.data, copies=w_copies, classes=w_classes)
+                    self.keep_client.put(self.data, copies=w_copies, classes=w_classes, num_retries=0)
 
 @tutil.skip_sleep
 @parameterized.parameterized_class([{"disk_cache": True}, {"disk_cache": False}])
 class KeepXRequestIdTestCase(unittest.TestCase, tutil.ApiClientMock, DiskCacheBase):
     disk_cache = False
 
     def setUp(self):
@@ -1246,18 +1297,14 @@
         with self.TEST_PATCHER(self.DEFAULT_EXPECT, 500, 200):
             self.check_success(num_retries=3)
 
     def test_exception_then_success(self):
         with self.TEST_PATCHER(self.DEFAULT_EXPECT, Exception('mock err'), 200):
             self.check_success(num_retries=3)
 
-    def test_no_default_retry(self):
-        with self.TEST_PATCHER(self.DEFAULT_EXPECT, 500, 200):
-            self.check_exception()
-
     def test_no_retry_after_permanent_error(self):
         with self.TEST_PATCHER(self.DEFAULT_EXPECT, 403, 200):
             self.check_exception(num_retries=3)
 
     def test_error_after_retries_exhausted(self):
         with self.TEST_PATCHER(self.DEFAULT_EXPECT, 500, 500, 200):
             err = self.check_exception(num_retries=1)
@@ -1289,15 +1336,15 @@
             self.check_exception(arvados.errors.NotFoundError, num_retries=3)
 
     def test_general_exception_with_mixed_errors(self):
         # get should raise a NotFoundError if no server returns the block,
         # and a high threshold of servers report that it's not found.
         # This test rigs up 50/50 disagreement between two servers, and
         # checks that it does not become a NotFoundError.
-        client = self.new_client()
+        client = self.new_client(num_retries=0)
         with tutil.mock_keep_responses(self.DEFAULT_EXPECT, 404, 500):
             with self.assertRaises(arvados.errors.KeepReadError) as exc_check:
                 client.get(self.HINTED_LOCATOR)
             self.assertNotIsInstance(
                 exc_check.exception, arvados.errors.NotFoundError,
                 "mixed errors raised NotFoundError")
 
@@ -1337,15 +1384,15 @@
             self.check_exception(arvados.errors.NotFoundError, num_retries=3)
 
     def test_general_exception_with_mixed_errors(self):
         # head should raise a NotFoundError if no server returns the block,
         # and a high threshold of servers report that it's not found.
         # This test rigs up 50/50 disagreement between two servers, and
         # checks that it does not become a NotFoundError.
-        client = self.new_client()
+        client = self.new_client(num_retries=0)
         with tutil.mock_keep_responses(self.DEFAULT_EXPECT, 404, 500):
             with self.assertRaises(arvados.errors.KeepReadError) as exc_check:
                 client.head(self.HINTED_LOCATOR)
             self.assertNotIsInstance(
                 exc_check.exception, arvados.errors.NotFoundError,
                 "mixed errors raised NotFoundError")
```

### Comparing `arvados-python-client-2.6.2rc3/tests/test_keep_locator.py` & `arvados-python-client-2.6.3rc1/tests/test_keep_locator.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_retry.py` & `arvados-python-client-2.6.3rc1/tests/test_retry.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,22 +170,22 @@
     check_is = check('assertIs')
     check_is_not = check('assertIsNot')
 
     def test_obvious_successes(self):
         self.check_is(True, *list(range(200, 207)))
 
     def test_obvious_stops(self):
-        self.check_is(False, 424, 426, 428, 431,
+        self.check_is(False, 422, 424, 426, 428, 431,
                       *list(range(400, 408)) + list(range(410, 420)))
 
     def test_obvious_retries(self):
         self.check_is(None, 500, 502, 503, 504)
 
     def test_4xx_retries(self):
-        self.check_is(None, 408, 409, 422, 423)
+        self.check_is(None, 408, 409, 423)
 
     def test_5xx_failures(self):
         self.check_is(False, 501, *list(range(505, 512)))
 
     def test_1xx_not_retried(self):
         self.check_is_not(None, 100, 101)
```

### Comparing `arvados-python-client-2.6.2rc3/tests/test_retry_job_helpers.py` & `arvados-python-client-2.6.3rc1/tests/test_retry_job_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     @classmethod
     def setUpClass(cls):
         run_test_server.run()
 
     def setUp(self):
         # Patch arvados.api() to return our mock API, so we can mock
         # its http requests.
-        self.api_client = arvados.api('v1', cache=False)
+        self.api_client = arvados.api('v1', cache=False, num_retries=0)
         self.api_patch = mock.patch('arvados.api', return_value=self.api_client)
         self.api_patch.start()
 
     def tearDown(self):
         self.api_patch.stop()
 
     def run_method(self):
```

### Comparing `arvados-python-client-2.6.2rc3/tests/test_safeapi.py` & `arvados-python-client-2.6.3rc1/tests/test_safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_sdk.py` & `arvados-python-client-2.6.3rc1/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_stream.py` & `arvados-python-client-2.6.3rc1/tests/test_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,21 +220,14 @@
     @tutil.skip_sleep
     def test_success_without_retries(self):
         with tutil.mock_keep_responses('bar', 200):
             reader = self.reader_for('bar_file')
             self.assertEqual(b'bar', self.read_for_test(reader, 3))
 
     @tutil.skip_sleep
-    def test_read_no_default_retry(self):
-        with tutil.mock_keep_responses('', 500):
-            reader = self.reader_for('user_agreement')
-            with self.assertRaises(arvados.errors.KeepReadError):
-                self.read_for_test(reader, 10)
-
-    @tutil.skip_sleep
     def test_read_with_instance_retries(self):
         with tutil.mock_keep_responses('foo', 500, 200):
             reader = self.reader_for('foo_file', num_retries=3)
             self.assertEqual(b'foo', self.read_for_test(reader, 3))
 
     @tutil.skip_sleep
     def test_read_with_method_retries(self):
```

### Comparing `arvados-python-client-2.6.2rc3/tests/test_util.py` & `arvados-python-client-2.6.3rc1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc3/tests/test_vocabulary.py` & `arvados-python-client-2.6.3rc1/tests/test_vocabulary.py`

 * *Files identical despite different names*

