# Comparing `tmp/google-cloud-functions-1.8.3.tar.gz` & `tmp/google-cloud-functions-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-functions-1.8.3.tar", last modified: Mon Oct 10 16:24:13 2022, max compression
+gzip compressed data, was "google-cloud-functions-1.9.0.tar", last modified: Thu Dec 15 16:58:08 2022, max compression
```

## Comparing `google-cloud-functions-1.8.3.tar` & `google-cloud-functions-1.9.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.019746 google-cloud-functions-1.8.3/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4426 2022-10-10 16:24:13.019746 google-cloud-functions-1.8.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3687 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.007748 google-cloud-functions-1.8.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.007748 google-cloud-functions-1.8.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.007748 google-cloud-functions-1.8.3/google/cloud/functions/
--rw-rw-r--   0 root         (0)     1003     2165 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions/__init__.py
--rw-rw-r--   0 root         (0)     1003       83 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.007748 google-cloud-functions-1.8.3/google/cloud/functions_v1/
--rw-rw-r--   0 root         (0)     1003     1982 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3316 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       83 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.011747 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.011747 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/
--rw-rw-r--   0 root         (0)     1003      797 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62781 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72375 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/client.py
--rw-rw-r--   0 root         (0)     1003     5756 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.011747 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/
--rw-rw-r--   0 root         (0)     1003     1264 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12698 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26282 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26860 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.011747 google-cloud-functions-1.8.3/google/cloud/functions_v1/types/
--rw-rw-r--   0 root         (0)     1003     1773 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    36568 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/types/functions.py
--rw-rw-r--   0 root         (0)     1003     3237 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v1/types/operations.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.011747 google-cloud-functions-1.8.3/google/cloud/functions_v2/
--rw-rw-r--   0 root         (0)     1003     2043 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     2548 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       83 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.011747 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.015746 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/
--rw-rw-r--   0 root         (0)     1003      773 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    65707 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    79873 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/client.py
--rw-rw-r--   0 root         (0)     1003     5746 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.015746 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11370 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28694 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29200 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.015746 google-cloud-functions-1.8.3/google/cloud/functions_v2/types/
--rw-rw-r--   0 root         (0)     1003     1884 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    42881 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/google/cloud/functions_v2/types/functions.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.015746 google-cloud-functions-1.8.3/google_cloud_functions.egg-info/
--rw-r--r--   0 root         (0)     1003     4426 2022-10-10 16:24:12.000000 google-cloud-functions-1.8.3/google_cloud_functions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2471 2022-10-10 16:24:12.000000 google-cloud-functions-1.8.3/google_cloud_functions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:24:12.000000 google-cloud-functions-1.8.3/google_cloud_functions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:24:12.000000 google-cloud-functions-1.8.3/google_cloud_functions.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:24:12.000000 google-cloud-functions-1.8.3/google_cloud_functions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      269 2022-10-10 16:24:12.000000 google-cloud-functions-1.8.3/google_cloud_functions.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:24:12.000000 google-cloud-functions-1.8.3/google_cloud_functions.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.015746 google-cloud-functions-1.8.3/scripts/
--rw-rw-r--   0 root         (0)     1003     6510 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/scripts/fixup_functions_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:24:13.019746 google-cloud-functions-1.8.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2359 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.015746 google-cloud-functions-1.8.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.015746 google-cloud-functions-1.8.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.015746 google-cloud-functions-1.8.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.019746 google-cloud-functions-1.8.3/tests/unit/gapic/functions_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/tests/unit/gapic/functions_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   145005 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/tests/unit/gapic/functions_v1/test_cloud_functions_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:13.019746 google-cloud-functions-1.8.3/tests/unit/gapic/functions_v2/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/tests/unit/gapic/functions_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   161523 2022-10-10 16:21:03.000000 google-cloud-functions-1.8.3/tests/unit/gapic/functions_v2/test_function_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.119019 google-cloud-functions-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4558 2022-12-15 16:58:08.119019 google-cloud-functions-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3687 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.107017 google-cloud-functions-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.107017 google-cloud-functions-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.107017 google-cloud-functions-1.9.0/google/cloud/functions/
+-rw-rw-r--   0 root         (0)     1003     2277 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.111017 google-cloud-functions-1.9.0/google/cloud/functions_v1/
+-rw-rw-r--   0 root         (0)     1003     2094 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3316 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.111017 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.111017 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/
+-rw-rw-r--   0 root         (0)     1003      797 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    63415 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    73013 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5756 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.111017 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1264 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12577 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26382 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26947 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.111017 google-cloud-functions-1.9.0/google/cloud/functions_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1773 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37451 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/types/functions.py
+-rw-rw-r--   0 root         (0)     1003     3369 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v1/types/operations.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.111017 google-cloud-functions-1.9.0/google/cloud/functions_v2/
+-rw-rw-r--   0 root         (0)     1003     2155 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2548 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.111017 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.115018 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/
+-rw-rw-r--   0 root         (0)     1003      773 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    66463 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    80663 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5746 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.115018 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11249 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28794 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29287 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.115018 google-cloud-functions-1.9.0/google/cloud/functions_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1884 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44248 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/google/cloud/functions_v2/types/functions.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.115018 google-cloud-functions-1.9.0/google_cloud_functions.egg-info/
+-rw-r--r--   0 root         (0)     1003     4558 2022-12-15 16:58:08.000000 google-cloud-functions-1.9.0/google_cloud_functions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2558 2022-12-15 16:58:08.000000 google-cloud-functions-1.9.0/google_cloud_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 16:58:08.000000 google-cloud-functions-1.9.0/google_cloud_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-15 16:58:08.000000 google-cloud-functions-1.9.0/google_cloud_functions.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 16:58:08.000000 google-cloud-functions-1.9.0/google_cloud_functions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      294 2022-12-15 16:58:08.000000 google-cloud-functions-1.9.0/google_cloud_functions.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-15 16:58:08.000000 google-cloud-functions-1.9.0/google_cloud_functions.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-15 16:58:08.119019 google-cloud-functions-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2917 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.115018 google-cloud-functions-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.115018 google-cloud-functions-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.119019 google-cloud-functions-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.119019 google-cloud-functions-1.9.0/tests/unit/gapic/functions_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/tests/unit/gapic/functions_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   145059 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/tests/unit/gapic/functions_v1/test_cloud_functions_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 16:58:08.119019 google-cloud-functions-1.9.0/tests/unit/gapic/functions_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/tests/unit/gapic/functions_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   161577 2022-12-15 16:54:49.000000 google-cloud-functions-1.9.0/tests/unit/gapic/functions_v2/test_function_service.py
```

### Comparing `google-cloud-functions-1.8.3/LICENSE` & `google-cloud-functions-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/MANIFEST.in` & `google-cloud-functions-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/PKG-INFO` & `google-cloud-functions-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: google-cloud-functions
-Version: 1.8.3
+Version: 1.9.0
+Summary: Google Cloud Functions API client library
 Home-page: https://github.com/googleapis/python-functions
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Cloud Functions API
 =====================================
 
 |stable| |pypi| |versions|
```

### Comparing `google-cloud-functions-1.8.3/README.rst` & `google-cloud-functions-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.functions import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.cloud.functions_v1.services.cloud_functions_service.async_client import (
     CloudFunctionsServiceAsyncClient,
 )
 from google.cloud.functions_v1.services.cloud_functions_service.client import (
     CloudFunctionsServiceClient,
 )
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-from .services.cloud_functions_service import (
-    CloudFunctionsServiceAsyncClient,
-    CloudFunctionsServiceClient,
-)
-from .types.functions import (
+from .functions import (
     CallFunctionRequest,
     CallFunctionResponse,
     CloudFunction,
     CloudFunctionStatus,
     CreateFunctionRequest,
     DeleteFunctionRequest,
     EventTrigger,
@@ -36,35 +31,33 @@
     ListFunctionsRequest,
     ListFunctionsResponse,
     SecretEnvVar,
     SecretVolume,
     SourceRepository,
     UpdateFunctionRequest,
 )
-from .types.operations import OperationMetadataV1, OperationType
+from .operations import OperationMetadataV1, OperationType
 
 __all__ = (
-    "CloudFunctionsServiceAsyncClient",
     "CallFunctionRequest",
     "CallFunctionResponse",
     "CloudFunction",
-    "CloudFunctionStatus",
-    "CloudFunctionsServiceClient",
     "CreateFunctionRequest",
     "DeleteFunctionRequest",
     "EventTrigger",
     "FailurePolicy",
     "GenerateDownloadUrlRequest",
     "GenerateDownloadUrlResponse",
     "GenerateUploadUrlRequest",
     "GenerateUploadUrlResponse",
     "GetFunctionRequest",
     "HttpsTrigger",
     "ListFunctionsRequest",
     "ListFunctionsResponse",
-    "OperationMetadataV1",
-    "OperationType",
     "SecretEnvVar",
     "SecretVolume",
     "SourceRepository",
     "UpdateFunctionRequest",
+    "CloudFunctionStatus",
+    "OperationMetadataV1",
+    "OperationType",
 )
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/gapic_metadata.json` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/async_client.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.functions_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
@@ -178,17 +189,17 @@
         type(CloudFunctionsServiceClient).get_transport_class,
         type(CloudFunctionsServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, CloudFunctionsServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the cloud functions service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -224,18 +235,18 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def list_functions(
         self,
-        request: Union[functions.ListFunctionsRequest, dict] = None,
+        request: Optional[Union[functions.ListFunctionsRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFunctionsAsyncPager:
         r"""Returns a list of functions that belong to the
         requested project.
 
         .. code-block:: python
 
@@ -260,15 +271,15 @@
                 page_result = client.list_functions(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.functions_v1.types.ListFunctionsRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v1.types.ListFunctionsRequest, dict]]):
                 The request object. Request for the `ListFunctions`
                 method.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -326,19 +337,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_function(
         self,
-        request: Union[functions.GetFunctionRequest, dict] = None,
+        request: Optional[Union[functions.GetFunctionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.CloudFunction:
         r"""Returns a function with the given name from the
         requested project.
 
         .. code-block:: python
 
@@ -363,15 +374,15 @@
                 # Make the request
                 response = await client.get_function(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v1.types.GetFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v1.types.GetFunctionRequest, dict]]):
                 The request object. Request for the `GetFunction`
                 method.
             name (:class:`str`):
                 Required. The name of the function
                 which details should be obtained.
 
                 This corresponds to the ``name`` field
@@ -441,20 +452,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def create_function(
         self,
-        request: Union[functions.CreateFunctionRequest, dict] = None,
+        request: Optional[Union[functions.CreateFunctionRequest, dict]] = None,
         *,
-        location: str = None,
-        function: functions.CloudFunction = None,
+        location: Optional[str] = None,
+        function: Optional[functions.CloudFunction] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Creates a new function. If a function with the given name
         already exists in the specified project, the long running
         operation will return ``ALREADY_EXISTS`` error.
 
         .. code-block:: python
@@ -482,21 +493,21 @@
                 )
 
                 # Make the request
                 operation = client.create_function(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v1.types.CreateFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v1.types.CreateFunctionRequest, dict]]):
                 The request object. Request for the `CreateFunction`
                 method.
             location (:class:`str`):
                 Required. The project and location in which the function
                 should be created, specified in the format
                 ``projects/*/locations/*``
 
@@ -573,19 +584,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_function(
         self,
-        request: Union[functions.UpdateFunctionRequest, dict] = None,
+        request: Optional[Union[functions.UpdateFunctionRequest, dict]] = None,
         *,
-        function: functions.CloudFunction = None,
+        function: Optional[functions.CloudFunction] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Updates existing function.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -610,21 +621,21 @@
                 )
 
                 # Make the request
                 operation = client.update_function(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v1.types.UpdateFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v1.types.UpdateFunctionRequest, dict]]):
                 The request object. Request for the `UpdateFunction`
                 method.
             function (:class:`google.cloud.functions_v1.types.CloudFunction`):
                 Required. New version of the
                 function.
 
                 This corresponds to the ``function`` field
@@ -705,19 +716,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_function(
         self,
-        request: Union[functions.DeleteFunctionRequest, dict] = None,
+        request: Optional[Union[functions.DeleteFunctionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a function with the given name from the
         specified project. If the given function is used by some
         trigger, the trigger will be updated to remove this
         function.
 
@@ -742,21 +753,21 @@
                 )
 
                 # Make the request
                 operation = client.delete_function(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v1.types.DeleteFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v1.types.DeleteFunctionRequest, dict]]):
                 The request object. Request for the `DeleteFunction`
                 method.
             name (:class:`str`):
                 Required. The name of the function
                 which should be deleted.
 
                 This corresponds to the ``name`` field
@@ -842,20 +853,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def call_function(
         self,
-        request: Union[functions.CallFunctionRequest, dict] = None,
+        request: Optional[Union[functions.CallFunctionRequest, dict]] = None,
         *,
-        name: str = None,
-        data: str = None,
+        name: Optional[str] = None,
+        data: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.CallFunctionResponse:
         r"""Synchronously invokes a deployed Cloud Function. To be used for
         testing purposes as very limited traffic is allowed. For more
         information on the actual limits, refer to `Rate
         Limits <https://cloud.google.com/functions/quotas#rate_limits>`__.
 
@@ -883,15 +894,15 @@
                 # Make the request
                 response = await client.call_function(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v1.types.CallFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v1.types.CallFunctionRequest, dict]]):
                 The request object. Request for the `CallFunction`
                 method.
             name (:class:`str`):
                 Required. The name of the function to
                 be called.
 
                 This corresponds to the ``name`` field
@@ -956,18 +967,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def generate_upload_url(
         self,
-        request: Union[functions.GenerateUploadUrlRequest, dict] = None,
+        request: Optional[Union[functions.GenerateUploadUrlRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.GenerateUploadUrlResponse:
         r"""Returns a signed URL for uploading a function source code. For
         more information about the signed URL usage see:
         https://cloud.google.com/storage/docs/access-control/signed-urls.
         Once the function source code upload is complete, the used
         signed URL should be provided in CreateFunction or
@@ -1017,15 +1028,15 @@
                 # Make the request
                 response = await client.generate_upload_url(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v1.types.GenerateUploadUrlRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v1.types.GenerateUploadUrlRequest, dict]]):
                 The request object. Request of `GenerateSourceUploadUrl`
                 method.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -1060,18 +1071,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def generate_download_url(
         self,
-        request: Union[functions.GenerateDownloadUrlRequest, dict] = None,
+        request: Optional[Union[functions.GenerateDownloadUrlRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.GenerateDownloadUrlResponse:
         r"""Returns a signed URL for downloading deployed
         function source code. The URL is only valid for a
         limited period and should be used within minutes after
         generation.
         For more information about the signed URL usage see:
@@ -1099,15 +1110,15 @@
                 # Make the request
                 response = await client.generate_download_url(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v1.types.GenerateDownloadUrlRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v1.types.GenerateDownloadUrlRequest, dict]]):
                 The request object. Request of `GenerateDownloadUrl`
                 method.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -1142,18 +1153,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def set_iam_policy(
         self,
-        request: Union[iam_policy_pb2.SetIamPolicyRequest, dict] = None,
+        request: Optional[Union[iam_policy_pb2.SetIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the IAM access control policy on the specified
         function. Replaces any existing policy.
 
         .. code-block:: python
 
@@ -1179,15 +1190,15 @@
                 # Make the request
                 response = await client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
+            request (Optional[Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]]):
                 The request object. Request message for `SetIamPolicy`
                 method.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -1286,18 +1297,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_iam_policy(
         self,
-        request: Union[iam_policy_pb2.GetIamPolicyRequest, dict] = None,
+        request: Optional[Union[iam_policy_pb2.GetIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the IAM access control policy for a function.
         Returns an empty policy if the function exists and does
         not have a policy set.
 
         .. code-block:: python
@@ -1324,15 +1335,15 @@
                 # Make the request
                 response = await client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
+            request (Optional[Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]]):
                 The request object. Request message for `GetIamPolicy`
                 method.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -1431,18 +1442,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def test_iam_permissions(
         self,
-        request: Union[iam_policy_pb2.TestIamPermissionsRequest, dict] = None,
+        request: Optional[Union[iam_policy_pb2.TestIamPermissionsRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Tests the specified permissions against the IAM access control
         policy for a function. If the function does not exist, this will
         return an empty set of permissions, not a NOT_FOUND error.
 
         .. code-block:: python
@@ -1470,15 +1481,15 @@
                 # Make the request
                 response = await client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
+            request (Optional[Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]]):
                 The request object. Request message for
                 `TestIamPermissions` method.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -1521,18 +1532,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-functions",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("CloudFunctionsServiceAsyncClient",)
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/client.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.functions_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
@@ -62,15 +74,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[CloudFunctionsServiceTransport]]
     _transport_registry["grpc"] = CloudFunctionsServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = CloudFunctionsServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[CloudFunctionsServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -387,30 +399,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, CloudFunctionsServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, CloudFunctionsServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the cloud functions service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, CloudFunctionsServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -432,14 +444,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -484,18 +497,18 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def list_functions(
         self,
-        request: Union[functions.ListFunctionsRequest, dict] = None,
+        request: Optional[Union[functions.ListFunctionsRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFunctionsPager:
         r"""Returns a list of functions that belong to the
         requested project.
 
         .. code-block:: python
 
@@ -577,19 +590,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_function(
         self,
-        request: Union[functions.GetFunctionRequest, dict] = None,
+        request: Optional[Union[functions.GetFunctionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.CloudFunction:
         r"""Returns a function with the given name from the
         requested project.
 
         .. code-block:: python
 
@@ -682,20 +695,20 @@
         )
 
         # Done; return the response.
         return response
 
     def create_function(
         self,
-        request: Union[functions.CreateFunctionRequest, dict] = None,
+        request: Optional[Union[functions.CreateFunctionRequest, dict]] = None,
         *,
-        location: str = None,
-        function: functions.CloudFunction = None,
+        location: Optional[str] = None,
+        function: Optional[functions.CloudFunction] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Creates a new function. If a function with the given name
         already exists in the specified project, the long running
         operation will return ``ALREADY_EXISTS`` error.
 
         .. code-block:: python
@@ -814,19 +827,19 @@
         )
 
         # Done; return the response.
         return response
 
     def update_function(
         self,
-        request: Union[functions.UpdateFunctionRequest, dict] = None,
+        request: Optional[Union[functions.UpdateFunctionRequest, dict]] = None,
         *,
-        function: functions.CloudFunction = None,
+        function: Optional[functions.CloudFunction] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Updates existing function.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -936,19 +949,19 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_function(
         self,
-        request: Union[functions.DeleteFunctionRequest, dict] = None,
+        request: Optional[Union[functions.DeleteFunctionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a function with the given name from the
         specified project. If the given function is used by some
         trigger, the trigger will be updated to remove this
         function.
 
@@ -1063,20 +1076,20 @@
         )
 
         # Done; return the response.
         return response
 
     def call_function(
         self,
-        request: Union[functions.CallFunctionRequest, dict] = None,
+        request: Optional[Union[functions.CallFunctionRequest, dict]] = None,
         *,
-        name: str = None,
-        data: str = None,
+        name: Optional[str] = None,
+        data: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.CallFunctionResponse:
         r"""Synchronously invokes a deployed Cloud Function. To be used for
         testing purposes as very limited traffic is allowed. For more
         information on the actual limits, refer to `Rate
         Limits <https://cloud.google.com/functions/quotas#rate_limits>`__.
 
@@ -1177,18 +1190,18 @@
         )
 
         # Done; return the response.
         return response
 
     def generate_upload_url(
         self,
-        request: Union[functions.GenerateUploadUrlRequest, dict] = None,
+        request: Optional[Union[functions.GenerateUploadUrlRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.GenerateUploadUrlResponse:
         r"""Returns a signed URL for uploading a function source code. For
         more information about the signed URL usage see:
         https://cloud.google.com/storage/docs/access-control/signed-urls.
         Once the function source code upload is complete, the used
         signed URL should be provided in CreateFunction or
@@ -1282,18 +1295,18 @@
         )
 
         # Done; return the response.
         return response
 
     def generate_download_url(
         self,
-        request: Union[functions.GenerateDownloadUrlRequest, dict] = None,
+        request: Optional[Union[functions.GenerateDownloadUrlRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.GenerateDownloadUrlResponse:
         r"""Returns a signed URL for downloading deployed
         function source code. The URL is only valid for a
         limited period and should be used within minutes after
         generation.
         For more information about the signed URL usage see:
@@ -1365,18 +1378,18 @@
         )
 
         # Done; return the response.
         return response
 
     def set_iam_policy(
         self,
-        request: Union[iam_policy_pb2.SetIamPolicyRequest, dict] = None,
+        request: Optional[Union[iam_policy_pb2.SetIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the IAM access control policy on the specified
         function. Replaces any existing policy.
 
         .. code-block:: python
 
@@ -1508,18 +1521,18 @@
         )
 
         # Done; return the response.
         return response
 
     def get_iam_policy(
         self,
-        request: Union[iam_policy_pb2.GetIamPolicyRequest, dict] = None,
+        request: Optional[Union[iam_policy_pb2.GetIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the IAM access control policy for a function.
         Returns an empty policy if the function exists and does
         not have a policy set.
 
         .. code-block:: python
@@ -1652,18 +1665,18 @@
         )
 
         # Done; return the response.
         return response
 
     def test_iam_permissions(
         self,
-        request: Union[iam_policy_pb2.TestIamPermissionsRequest, dict] = None,
+        request: Optional[Union[iam_policy_pb2.TestIamPermissionsRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Tests the specified permissions against the IAM access control
         policy for a function. If the function does not exist, this will
         return an empty set of permissions, not a NOT_FOUND error.
 
         .. code-block:: python
@@ -1748,18 +1761,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-functions",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("CloudFunctionsServiceClient",)
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/pagers.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/base.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,40 +22,35 @@
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.functions_v1 import gapic_version as package_version
 from google.cloud.functions_v1.types import functions
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-functions",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class CloudFunctionsServiceTransport(abc.ABC):
     """Abstract transport class for CloudFunctionsService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "cloudfunctions.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/grpc.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "cloudfunctions.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -181,16 +181,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "cloudfunctions.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/services/cloud_functions_service/transports/grpc_asyncio.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/services/cloud_functions_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "cloudfunctions.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -91,23 +91,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "cloudfunctions.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/types/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .functions import (
+from google.cloud.functions import gapic_version as package_version
+
+__version__ = package_version.__version__
+
+
+from .services.cloud_functions_service import (
+    CloudFunctionsServiceAsyncClient,
+    CloudFunctionsServiceClient,
+)
+from .types.functions import (
     CallFunctionRequest,
     CallFunctionResponse,
     CloudFunction,
     CloudFunctionStatus,
     CreateFunctionRequest,
     DeleteFunctionRequest,
     EventTrigger,
@@ -31,33 +40,35 @@
     ListFunctionsRequest,
     ListFunctionsResponse,
     SecretEnvVar,
     SecretVolume,
     SourceRepository,
     UpdateFunctionRequest,
 )
-from .operations import OperationMetadataV1, OperationType
+from .types.operations import OperationMetadataV1, OperationType
 
 __all__ = (
+    "CloudFunctionsServiceAsyncClient",
     "CallFunctionRequest",
     "CallFunctionResponse",
     "CloudFunction",
+    "CloudFunctionStatus",
+    "CloudFunctionsServiceClient",
     "CreateFunctionRequest",
     "DeleteFunctionRequest",
     "EventTrigger",
     "FailurePolicy",
     "GenerateDownloadUrlRequest",
     "GenerateDownloadUrlResponse",
     "GenerateUploadUrlRequest",
     "GenerateUploadUrlResponse",
     "GetFunctionRequest",
     "HttpsTrigger",
     "ListFunctionsRequest",
     "ListFunctionsResponse",
+    "OperationMetadataV1",
+    "OperationType",
     "SecretEnvVar",
     "SecretVolume",
     "SourceRepository",
     "UpdateFunctionRequest",
-    "CloudFunctionStatus",
-    "OperationMetadataV1",
-    "OperationType",
 )
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/types/functions.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/types/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.functions.v1",
@@ -136,20 +138,20 @@
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The last update timestamp of a
             Cloud Function.
         version_id (int):
             Output only. The version identifier of the
             Cloud Function. Each deployment attempt results
             in a new version of a function being created.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Labels associated with this Cloud Function.
-        environment_variables (Mapping[str, str]):
+        environment_variables (MutableMapping[str, str]):
             Environment variables that shall be available
             during function execution.
-        build_environment_variables (Mapping[str, str]):
+        build_environment_variables (MutableMapping[str, str]):
             Build environment variables that shall be
             available during build time.
         network (str):
             The VPC Network that this cloud function can connect to. It
             can be either the fully-qualified URI, or the short name of
             the network resource. If the short network name is used, the
             network must belong to the same project. Otherwise, it must
@@ -249,17 +251,17 @@
         build_id (str):
             Output only. The Cloud Build ID of the latest
             successful deployment of the function.
         build_name (str):
             Output only. The Cloud Build Name of the function
             deployment.
             ``projects/<project-number>/locations/<region>/builds/<build-id>``.
-        secret_environment_variables (Sequence[google.cloud.functions_v1.types.SecretEnvVar]):
+        secret_environment_variables (MutableSequence[google.cloud.functions_v1.types.SecretEnvVar]):
             Secret environment variables configuration.
-        secret_volumes (Sequence[google.cloud.functions_v1.types.SecretVolume]):
+        secret_volumes (MutableSequence[google.cloud.functions_v1.types.SecretVolume]):
             Secret volumes configuration.
         source_token (str):
             Input only. An identifier for Firebase
             function sources. Disclaimer: This field is only
             supported for Firebase function deployments.
         docker_repository (str):
             User managed repository created in Artifact Registry
@@ -311,161 +313,161 @@
 
     class DockerRegistry(proto.Enum):
         r"""Docker Registry to use for storing function Docker images."""
         DOCKER_REGISTRY_UNSPECIFIED = 0
         CONTAINER_REGISTRY = 1
         ARTIFACT_REGISTRY = 2
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    source_archive_url = proto.Field(
+    source_archive_url: str = proto.Field(
         proto.STRING,
         number=3,
         oneof="source_code",
     )
-    source_repository = proto.Field(
+    source_repository: "SourceRepository" = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="source_code",
         message="SourceRepository",
     )
-    source_upload_url = proto.Field(
+    source_upload_url: str = proto.Field(
         proto.STRING,
         number=16,
         oneof="source_code",
     )
-    https_trigger = proto.Field(
+    https_trigger: "HttpsTrigger" = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="trigger",
         message="HttpsTrigger",
     )
-    event_trigger = proto.Field(
+    event_trigger: "EventTrigger" = proto.Field(
         proto.MESSAGE,
         number=6,
         oneof="trigger",
         message="EventTrigger",
     )
-    status = proto.Field(
+    status: "CloudFunctionStatus" = proto.Field(
         proto.ENUM,
         number=7,
         enum="CloudFunctionStatus",
     )
-    entry_point = proto.Field(
+    entry_point: str = proto.Field(
         proto.STRING,
         number=8,
     )
-    runtime = proto.Field(
+    runtime: str = proto.Field(
         proto.STRING,
         number=19,
     )
-    timeout = proto.Field(
+    timeout: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=9,
         message=duration_pb2.Duration,
     )
-    available_memory_mb = proto.Field(
+    available_memory_mb: int = proto.Field(
         proto.INT32,
         number=10,
     )
-    service_account_email = proto.Field(
+    service_account_email: str = proto.Field(
         proto.STRING,
         number=11,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=12,
         message=timestamp_pb2.Timestamp,
     )
-    version_id = proto.Field(
+    version_id: int = proto.Field(
         proto.INT64,
         number=14,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=15,
     )
-    environment_variables = proto.MapField(
+    environment_variables: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=17,
     )
-    build_environment_variables = proto.MapField(
+    build_environment_variables: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=28,
     )
-    network = proto.Field(
+    network: str = proto.Field(
         proto.STRING,
         number=18,
     )
-    max_instances = proto.Field(
+    max_instances: int = proto.Field(
         proto.INT32,
         number=20,
     )
-    min_instances = proto.Field(
+    min_instances: int = proto.Field(
         proto.INT32,
         number=32,
     )
-    vpc_connector = proto.Field(
+    vpc_connector: str = proto.Field(
         proto.STRING,
         number=22,
     )
-    vpc_connector_egress_settings = proto.Field(
+    vpc_connector_egress_settings: VpcConnectorEgressSettings = proto.Field(
         proto.ENUM,
         number=23,
         enum=VpcConnectorEgressSettings,
     )
-    ingress_settings = proto.Field(
+    ingress_settings: IngressSettings = proto.Field(
         proto.ENUM,
         number=24,
         enum=IngressSettings,
     )
-    kms_key_name = proto.Field(
+    kms_key_name: str = proto.Field(
         proto.STRING,
         number=25,
     )
-    build_worker_pool = proto.Field(
+    build_worker_pool: str = proto.Field(
         proto.STRING,
         number=26,
     )
-    build_id = proto.Field(
+    build_id: str = proto.Field(
         proto.STRING,
         number=27,
     )
-    build_name = proto.Field(
+    build_name: str = proto.Field(
         proto.STRING,
         number=33,
     )
-    secret_environment_variables = proto.RepeatedField(
+    secret_environment_variables: MutableSequence["SecretEnvVar"] = proto.RepeatedField(
         proto.MESSAGE,
         number=29,
         message="SecretEnvVar",
     )
-    secret_volumes = proto.RepeatedField(
+    secret_volumes: MutableSequence["SecretVolume"] = proto.RepeatedField(
         proto.MESSAGE,
         number=30,
         message="SecretVolume",
     )
-    source_token = proto.Field(
+    source_token: str = proto.Field(
         proto.STRING,
         number=31,
     )
-    docker_repository = proto.Field(
+    docker_repository: str = proto.Field(
         proto.STRING,
         number=34,
     )
-    docker_registry = proto.Field(
+    docker_registry: DockerRegistry = proto.Field(
         proto.ENUM,
         number=35,
         enum=DockerRegistry,
     )
 
 
 class SourceRepository(proto.Message):
@@ -491,19 +493,19 @@
         deployed_url (str):
             Output only. The URL pointing to the hosted
             repository where the function were defined at
             the time of deployment. It always points to a
             specific commit in the format described above.
     """
 
-    url = proto.Field(
+    url: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    deployed_url = proto.Field(
+    deployed_url: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class HttpsTrigger(proto.Message):
     r"""Describes HttpsTrigger, could be used to connect web hooks to
@@ -524,19 +526,19 @@
 
         If unspecified, SECURE_OPTIONAL will be used.
         """
         SECURITY_LEVEL_UNSPECIFIED = 0
         SECURE_ALWAYS = 1
         SECURE_OPTIONAL = 2
 
-    url = proto.Field(
+    url: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    security_level = proto.Field(
+    security_level: SecurityLevel = proto.Field(
         proto.ENUM,
         number=2,
         enum=SecurityLevel,
     )
 
 
 class EventTrigger(proto.Message):
@@ -588,27 +590,27 @@
             the API will be used. For example,
             ``storage.googleapis.com`` is the default for all event
             types in the ``google.storage`` namespace.
         failure_policy (google.cloud.functions_v1.types.FailurePolicy):
             Specifies policy for failed executions.
     """
 
-    event_type = proto.Field(
+    event_type: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    resource = proto.Field(
+    resource: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    service = proto.Field(
+    service: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    failure_policy = proto.Field(
+    failure_policy: "FailurePolicy" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="FailurePolicy",
     )
 
 
 class FailurePolicy(proto.Message):
@@ -632,15 +634,15 @@
         failure. A function execution will be retried on any failure. A
         failed execution will be retried up to 7 days with an
         exponential backoff (capped at 10 seconds).
         Retried execution is charged as any other execution.
 
         """
 
-    retry = proto.Field(
+    retry: Retry = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="action",
         message=Retry,
     )
 
 
@@ -666,27 +668,27 @@
             Version of the secret (version number or the
             string 'latest'). It is recommended to use a
             numeric version for secret environment variables
             as any updates to the secret value is not
             reflected until new instances start.
     """
 
-    key = proto.Field(
+    key: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    project_id = proto.Field(
+    project_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    secret = proto.Field(
+    secret: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    version = proto.Field(
+    version: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class SecretVolume(proto.Message):
     r"""Configuration for a secret volume. It has the information
@@ -713,15 +715,15 @@
             project that contains the secret. If not set, it
             will be populated with the function's project
             assuming that the secret exists in the same
             project as of the function.
         secret (str):
             Name of the secret in secret manager (not the
             full resource name).
-        versions (Sequence[google.cloud.functions_v1.types.SecretVolume.SecretVersion]):
+        versions (MutableSequence[google.cloud.functions_v1.types.SecretVolume.SecretVersion]):
             List of secret versions to mount for this secret. If empty,
             the ``latest`` version of the secret will be made available
             in a file named after the secret under the mount point.
     """
 
     class SecretVersion(proto.Message):
         r"""Configuration for a single version.
@@ -736,36 +738,36 @@
                 Relative path of the file under the mount path where the
                 secret value for this version will be fetched and made
                 available. For example, setting the mount_path as
                 '/etc/secrets' and path as ``/secret_foo`` would mount the
                 secret value file at ``/etc/secrets/secret_foo``.
         """
 
-        version = proto.Field(
+        version: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        path = proto.Field(
+        path: str = proto.Field(
             proto.STRING,
             number=2,
         )
 
-    mount_path = proto.Field(
+    mount_path: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    project_id = proto.Field(
+    project_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    secret = proto.Field(
+    secret: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    versions = proto.RepeatedField(
+    versions: MutableSequence[SecretVersion] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message=SecretVersion,
     )
 
 
 class CreateFunctionRequest(proto.Message):
@@ -776,19 +778,19 @@
             Required. The project and location in which the function
             should be created, specified in the format
             ``projects/*/locations/*``
         function (google.cloud.functions_v1.types.CloudFunction):
             Required. Function to be created.
     """
 
-    location = proto.Field(
+    location: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    function = proto.Field(
+    function: "CloudFunction" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="CloudFunction",
     )
 
 
 class UpdateFunctionRequest(proto.Message):
@@ -798,20 +800,20 @@
         function (google.cloud.functions_v1.types.CloudFunction):
             Required. New version of the function.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. The list of fields in ``CloudFunction`` that have
             to be updated.
     """
 
-    function = proto.Field(
+    function: "CloudFunction" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="CloudFunction",
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class GetFunctionRequest(proto.Message):
@@ -819,15 +821,15 @@
 
     Attributes:
         name (str):
             Required. The name of the function which
             details should be obtained.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListFunctionsRequest(proto.Message):
     r"""Request for the ``ListFunctions`` method.
@@ -847,74 +849,74 @@
         page_token (str):
             The value returned by the last ``ListFunctionsResponse``;
             indicates that this is a continuation of a prior
             ``ListFunctions`` call, and that the system should return
             the next page of data.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ListFunctionsResponse(proto.Message):
     r"""Response for the ``ListFunctions`` method.
 
     Attributes:
-        functions (Sequence[google.cloud.functions_v1.types.CloudFunction]):
+        functions (MutableSequence[google.cloud.functions_v1.types.CloudFunction]):
             The functions that match the request.
         next_page_token (str):
             If not empty, indicates that there may be more functions
             that match the request; this value should be passed in a new
             [google.cloud.functions.v1.ListFunctionsRequest][google.cloud.functions.v1.ListFunctionsRequest]
             to get more functions.
-        unreachable (Sequence[str]):
+        unreachable (MutableSequence[str]):
             Locations that could not be reached. The
             response does not include any functions from
             these locations.
     """
 
     @property
     def raw_page(self):
         return self
 
-    functions = proto.RepeatedField(
+    functions: MutableSequence["CloudFunction"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="CloudFunction",
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    unreachable = proto.RepeatedField(
+    unreachable: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
 
 
 class DeleteFunctionRequest(proto.Message):
     r"""Request for the ``DeleteFunction`` method.
 
     Attributes:
         name (str):
             Required. The name of the function which
             should be deleted.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class CallFunctionRequest(proto.Message):
     r"""Request for the ``CallFunction`` method.
@@ -923,19 +925,19 @@
         name (str):
             Required. The name of the function to be
             called.
         data (str):
             Required. Input to be passed to the function.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    data = proto.Field(
+    data: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class CallFunctionResponse(proto.Message):
     r"""Response of ``CallFunction`` method.
@@ -949,23 +951,23 @@
             function does not return a result through
             context.
         error (str):
             Either system or user-function generated
             error. Set if execution was not successful.
     """
 
-    execution_id = proto.Field(
+    execution_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    result = proto.Field(
+    result: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    error = proto.Field(
+    error: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class GenerateUploadUrlRequest(proto.Message):
     r"""Request of ``GenerateSourceUploadUrl`` method.
@@ -994,19 +996,19 @@
             Encrypter/Decrypter
             (roles/cloudkms.cryptoKeyEncrypterDecrypter)' on the
             Key/KeyRing/Project/Organization (least access preferred).
             GCF will delegate access to the Google Storage service
             account in the internal project.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    kms_key_name = proto.Field(
+    kms_key_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class GenerateUploadUrlResponse(proto.Message):
     r"""Response of ``GenerateSourceUploadUrl`` method.
@@ -1015,15 +1017,15 @@
         upload_url (str):
             The generated Google Cloud Storage signed URL
             that should be used for a function source code
             upload. The uploaded file should be a zip
             archive which contains a function.
     """
 
-    upload_url = proto.Field(
+    upload_url: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class GenerateDownloadUrlRequest(proto.Message):
     r"""Request of ``GenerateDownloadUrl`` method.
@@ -1034,19 +1036,19 @@
             Google Cloud Storage signed URL should be
             generated.
         version_id (int):
             The optional version of function. If not set,
             default, current version is used.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    version_id = proto.Field(
+    version_id: int = proto.Field(
         proto.UINT64,
         number=2,
     )
 
 
 class GenerateDownloadUrlResponse(proto.Message):
     r"""Response of ``GenerateDownloadUrl`` method.
@@ -1054,14 +1056,14 @@
     Attributes:
         download_url (str):
             The generated Google Cloud Storage signed URL
             that should be used for function source code
             download.
     """
 
-    download_url = proto.Field(
+    download_url: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v1/types/operations.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v1/types/operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import any_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.functions.v1",
     manifest={
@@ -62,45 +64,45 @@
             Firebase function deployments.
         build_name (str):
             The Cloud Build Name of the function deployment. This field
             is only populated for Create and Update operations.
             ``projects/<project-number>/locations/<region>/builds/<build-id>``.
     """
 
-    target = proto.Field(
+    target: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    type_ = proto.Field(
+    type_: "OperationType" = proto.Field(
         proto.ENUM,
         number=2,
         enum="OperationType",
     )
-    request = proto.Field(
+    request: any_pb2.Any = proto.Field(
         proto.MESSAGE,
         number=3,
         message=any_pb2.Any,
     )
-    version_id = proto.Field(
+    version_id: int = proto.Field(
         proto.INT64,
         number=4,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
-    build_id = proto.Field(
+    build_id: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    source_token = proto.Field(
+    source_token: str = proto.Field(
         proto.STRING,
         number=7,
     )
-    build_name = proto.Field(
+    build_name: str = proto.Field(
         proto.STRING,
         number=8,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.functions import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.function_service import FunctionServiceAsyncClient, FunctionServiceClient
 from .types.functions import (
     BuildConfig,
     CreateFunctionRequest,
     DeleteFunctionRequest,
     Environment,
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/gapic_metadata.json` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/async_client.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.functions_v2 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
@@ -187,17 +198,17 @@
     get_transport_class = functools.partial(
         type(FunctionServiceClient).get_transport_class, type(FunctionServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, FunctionServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the function service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -233,19 +244,19 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def get_function(
         self,
-        request: Union[functions.GetFunctionRequest, dict] = None,
+        request: Optional[Union[functions.GetFunctionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.Function:
         r"""Returns a function with the given name from the
         requested project.
 
         .. code-block:: python
 
@@ -270,15 +281,15 @@
                 # Make the request
                 response = await client.get_function(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v2.types.GetFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v2.types.GetFunctionRequest, dict]]):
                 The request object. Request for the `GetFunction`
                 method.
             name (:class:`str`):
                 Required. The name of the function
                 which details should be obtained.
 
                 This corresponds to the ``name`` field
@@ -338,19 +349,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_functions(
         self,
-        request: Union[functions.ListFunctionsRequest, dict] = None,
+        request: Optional[Union[functions.ListFunctionsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFunctionsAsyncPager:
         r"""Returns a list of functions that belong to the
         requested project.
 
         .. code-block:: python
 
@@ -376,15 +387,15 @@
                 page_result = client.list_functions(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.functions_v2.types.ListFunctionsRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v2.types.ListFunctionsRequest, dict]]):
                 The request object. Request for the `ListFunctions`
                 method.
             parent (:class:`str`):
                 Required. The project and location from which the
                 function should be listed, specified in the format
                 ``projects/*/locations/*`` If you want to list functions
                 in all locations, use "-" in place of a location. When
@@ -459,21 +470,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def create_function(
         self,
-        request: Union[functions.CreateFunctionRequest, dict] = None,
+        request: Optional[Union[functions.CreateFunctionRequest, dict]] = None,
         *,
-        parent: str = None,
-        function: functions.Function = None,
-        function_id: str = None,
+        parent: Optional[str] = None,
+        function: Optional[functions.Function] = None,
+        function_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Creates a new function. If a function with the given name
         already exists in the specified project, the long running
         operation will return ``ALREADY_EXISTS`` error.
 
         .. code-block:: python
@@ -497,21 +508,21 @@
                 )
 
                 # Make the request
                 operation = client.create_function(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v2.types.CreateFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v2.types.CreateFunctionRequest, dict]]):
                 The request object. Request for the `CreateFunction`
                 method.
             parent (:class:`str`):
                 Required. The project and location in which the function
                 should be created, specified in the format
                 ``projects/*/locations/*``
 
@@ -600,20 +611,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_function(
         self,
-        request: Union[functions.UpdateFunctionRequest, dict] = None,
+        request: Optional[Union[functions.UpdateFunctionRequest, dict]] = None,
         *,
-        function: functions.Function = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        function: Optional[functions.Function] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Updates existing function.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -634,21 +645,21 @@
                 )
 
                 # Make the request
                 operation = client.update_function(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v2.types.UpdateFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v2.types.UpdateFunctionRequest, dict]]):
                 The request object. Request for the `UpdateFunction`
                 method.
             function (:class:`google.cloud.functions_v2.types.Function`):
                 Required. New version of the
                 function.
 
                 This corresponds to the ``function`` field
@@ -730,19 +741,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_function(
         self,
-        request: Union[functions.DeleteFunctionRequest, dict] = None,
+        request: Optional[Union[functions.DeleteFunctionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a function with the given name from the
         specified project. If the given function is used by some
         trigger, the trigger will be updated to remove this
         function.
 
@@ -767,21 +778,21 @@
                 )
 
                 # Make the request
                 operation = client.delete_function(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v2.types.DeleteFunctionRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v2.types.DeleteFunctionRequest, dict]]):
                 The request object. Request for the `DeleteFunction`
                 method.
             name (:class:`str`):
                 Required. The name of the function
                 which should be deleted.
 
                 This corresponds to the ``name`` field
@@ -857,18 +868,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def generate_upload_url(
         self,
-        request: Union[functions.GenerateUploadUrlRequest, dict] = None,
+        request: Optional[Union[functions.GenerateUploadUrlRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.GenerateUploadUrlResponse:
         r"""Returns a signed URL for uploading a function source code. For
         more information about the signed URL usage see:
         https://cloud.google.com/storage/docs/access-control/signed-urls.
         Once the function source code upload is complete, the used
         signed URL should be provided in CreateFunction or
@@ -917,15 +928,15 @@
                 # Make the request
                 response = await client.generate_upload_url(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v2.types.GenerateUploadUrlRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v2.types.GenerateUploadUrlRequest, dict]]):
                 The request object. Request of `GenerateSourceUploadUrl`
                 method.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -960,18 +971,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def generate_download_url(
         self,
-        request: Union[functions.GenerateDownloadUrlRequest, dict] = None,
+        request: Optional[Union[functions.GenerateDownloadUrlRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.GenerateDownloadUrlResponse:
         r"""Returns a signed URL for downloading deployed
         function source code. The URL is only valid for a
         limited period and should be used within 30 minutes of
         generation.
         For more information about the signed URL usage see:
@@ -1000,15 +1011,15 @@
                 # Make the request
                 response = await client.generate_download_url(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v2.types.GenerateDownloadUrlRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v2.types.GenerateDownloadUrlRequest, dict]]):
                 The request object. Request of `GenerateDownloadUrl`
                 method.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -1043,19 +1054,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_runtimes(
         self,
-        request: Union[functions.ListRuntimesRequest, dict] = None,
+        request: Optional[Union[functions.ListRuntimesRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.ListRuntimesResponse:
         r"""Returns a list of runtimes that are supported for the
         requested project.
 
         .. code-block:: python
 
@@ -1080,15 +1091,15 @@
                 # Make the request
                 response = await client.list_runtimes(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.functions_v2.types.ListRuntimesRequest, dict]):
+            request (Optional[Union[google.cloud.functions_v2.types.ListRuntimesRequest, dict]]):
                 The request object. Request for the `ListRuntimes`
                 method.
             parent (:class:`str`):
                 Required. The project and location from which the
                 runtimes should be listed, specified in the format
                 ``projects/*/locations/*``
 
@@ -1145,18 +1156,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_operations(
         self,
-        request: operations_pb2.ListOperationsRequest = None,
+        request: Optional[operations_pb2.ListOperationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operations_pb2.ListOperationsResponse:
         r"""Lists operations that match the specified filter in the request.
 
         Args:
             request (:class:`~.operations_pb2.ListOperationsRequest`):
                 The request object. Request message for
@@ -1199,18 +1210,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_operation(
         self,
-        request: operations_pb2.GetOperationRequest = None,
+        request: Optional[operations_pb2.GetOperationRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operations_pb2.Operation:
         r"""Gets the latest state of a long-running operation.
 
         Args:
             request (:class:`~.operations_pb2.GetOperationRequest`):
                 The request object. Request message for
@@ -1253,18 +1264,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def set_iam_policy(
         self,
-        request: iam_policy_pb2.SetIamPolicyRequest = None,
+        request: Optional[iam_policy_pb2.SetIamPolicyRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the IAM access control policy on the specified function.
 
         Replaces any existing policy.
 
         Args:
@@ -1373,18 +1384,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_iam_policy(
         self,
-        request: iam_policy_pb2.GetIamPolicyRequest = None,
+        request: Optional[iam_policy_pb2.GetIamPolicyRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the IAM access control policy for a function.
 
         Returns an empty policy if the function exists and does not have a
         policy set.
 
@@ -1494,18 +1505,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def test_iam_permissions(
         self,
-        request: iam_policy_pb2.TestIamPermissionsRequest = None,
+        request: Optional[iam_policy_pb2.TestIamPermissionsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Tests the specified IAM permissions against the IAM access control
             policy for a function.
 
         If the function does not exist, this will return an empty set
         of permissions, not a NOT_FOUND error.
@@ -1553,18 +1564,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_locations(
         self,
-        request: locations_pb2.ListLocationsRequest = None,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> locations_pb2.ListLocationsResponse:
         r"""Lists information about the supported locations for this service.
 
         Args:
             request (:class:`~.location_pb2.ListLocationsRequest`):
                 The request object. Request message for
@@ -1612,18 +1623,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-functions",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("FunctionServiceAsyncClient",)
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/client.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.functions_v2 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
@@ -64,15 +76,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[FunctionServiceTransport]]
     _transport_registry["grpc"] = FunctionServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = FunctionServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[FunctionServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -520,30 +532,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, FunctionServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, FunctionServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the function service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, FunctionServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -565,14 +577,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -617,19 +630,19 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def get_function(
         self,
-        request: Union[functions.GetFunctionRequest, dict] = None,
+        request: Optional[Union[functions.GetFunctionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.Function:
         r"""Returns a function with the given name from the
         requested project.
 
         .. code-block:: python
 
@@ -722,19 +735,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_functions(
         self,
-        request: Union[functions.ListFunctionsRequest, dict] = None,
+        request: Optional[Union[functions.ListFunctionsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFunctionsPager:
         r"""Returns a list of functions that belong to the
         requested project.
 
         .. code-block:: python
 
@@ -843,21 +856,21 @@
         )
 
         # Done; return the response.
         return response
 
     def create_function(
         self,
-        request: Union[functions.CreateFunctionRequest, dict] = None,
+        request: Optional[Union[functions.CreateFunctionRequest, dict]] = None,
         *,
-        parent: str = None,
-        function: functions.Function = None,
-        function_id: str = None,
+        parent: Optional[str] = None,
+        function: Optional[functions.Function] = None,
+        function_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Creates a new function. If a function with the given name
         already exists in the specified project, the long running
         operation will return ``ALREADY_EXISTS`` error.
 
         .. code-block:: python
@@ -984,20 +997,20 @@
         )
 
         # Done; return the response.
         return response
 
     def update_function(
         self,
-        request: Union[functions.UpdateFunctionRequest, dict] = None,
+        request: Optional[Union[functions.UpdateFunctionRequest, dict]] = None,
         *,
-        function: functions.Function = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        function: Optional[functions.Function] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Updates existing function.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1114,19 +1127,19 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_function(
         self,
-        request: Union[functions.DeleteFunctionRequest, dict] = None,
+        request: Optional[Union[functions.DeleteFunctionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a function with the given name from the
         specified project. If the given function is used by some
         trigger, the trigger will be updated to remove this
         function.
 
@@ -1241,18 +1254,18 @@
         )
 
         # Done; return the response.
         return response
 
     def generate_upload_url(
         self,
-        request: Union[functions.GenerateUploadUrlRequest, dict] = None,
+        request: Optional[Union[functions.GenerateUploadUrlRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.GenerateUploadUrlResponse:
         r"""Returns a signed URL for uploading a function source code. For
         more information about the signed URL usage see:
         https://cloud.google.com/storage/docs/access-control/signed-urls.
         Once the function source code upload is complete, the used
         signed URL should be provided in CreateFunction or
@@ -1345,18 +1358,18 @@
         )
 
         # Done; return the response.
         return response
 
     def generate_download_url(
         self,
-        request: Union[functions.GenerateDownloadUrlRequest, dict] = None,
+        request: Optional[Union[functions.GenerateDownloadUrlRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.GenerateDownloadUrlResponse:
         r"""Returns a signed URL for downloading deployed
         function source code. The URL is only valid for a
         limited period and should be used within 30 minutes of
         generation.
         For more information about the signed URL usage see:
@@ -1429,19 +1442,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_runtimes(
         self,
-        request: Union[functions.ListRuntimesRequest, dict] = None,
+        request: Optional[Union[functions.ListRuntimesRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> functions.ListRuntimesResponse:
         r"""Returns a list of runtimes that are supported for the
         requested project.
 
         .. code-block:: python
 
@@ -1544,18 +1557,18 @@
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
     def list_operations(
         self,
-        request: operations_pb2.ListOperationsRequest = None,
+        request: Optional[operations_pb2.ListOperationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operations_pb2.ListOperationsResponse:
         r"""Lists operations that match the specified filter in the request.
 
         Args:
             request (:class:`~.operations_pb2.ListOperationsRequest`):
                 The request object. Request message for
@@ -1598,18 +1611,18 @@
         )
 
         # Done; return the response.
         return response
 
     def get_operation(
         self,
-        request: operations_pb2.GetOperationRequest = None,
+        request: Optional[operations_pb2.GetOperationRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operations_pb2.Operation:
         r"""Gets the latest state of a long-running operation.
 
         Args:
             request (:class:`~.operations_pb2.GetOperationRequest`):
                 The request object. Request message for
@@ -1652,18 +1665,18 @@
         )
 
         # Done; return the response.
         return response
 
     def set_iam_policy(
         self,
-        request: iam_policy_pb2.SetIamPolicyRequest = None,
+        request: Optional[iam_policy_pb2.SetIamPolicyRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the IAM access control policy on the specified function.
 
         Replaces any existing policy.
 
         Args:
@@ -1772,18 +1785,18 @@
         )
 
         # Done; return the response.
         return response
 
     def get_iam_policy(
         self,
-        request: iam_policy_pb2.GetIamPolicyRequest = None,
+        request: Optional[iam_policy_pb2.GetIamPolicyRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the IAM access control policy for a function.
 
         Returns an empty policy if the function exists and does not have a
         policy set.
 
@@ -1893,18 +1906,18 @@
         )
 
         # Done; return the response.
         return response
 
     def test_iam_permissions(
         self,
-        request: iam_policy_pb2.TestIamPermissionsRequest = None,
+        request: Optional[iam_policy_pb2.TestIamPermissionsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Tests the specified IAM permissions against the IAM access control
             policy for a function.
 
         If the function does not exist, this will return an empty set
         of permissions, not a NOT_FOUND error.
@@ -1952,18 +1965,18 @@
         )
 
         # Done; return the response.
         return response
 
     def list_locations(
         self,
-        request: locations_pb2.ListLocationsRequest = None,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> locations_pb2.ListLocationsResponse:
         r"""Lists information about the supported locations for this service.
 
         Args:
             request (:class:`~.location_pb2.ListLocationsRequest`):
                 The request object. Request message for
@@ -2005,18 +2018,13 @@
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-functions",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("FunctionServiceClient",)
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/pagers.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/base.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,40 +23,35 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.functions_v2 import gapic_version as package_version
 from google.cloud.functions_v2.types import functions
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-functions",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class FunctionServiceTransport(abc.ABC):
     """Abstract transport class for FunctionService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "cloudfunctions.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/grpc.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,22 +51,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "cloudfunctions.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -186,16 +186,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "cloudfunctions.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/services/function_service/transports/grpc_asyncio.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/services/function_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "cloudfunctions.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -96,23 +96,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "cloudfunctions.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/types/__init__.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/google/cloud/functions_v2/types/functions.py` & `google-cloud-functions-1.9.0/google/cloud/functions_v2/types/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import any_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.functions.v2",
@@ -86,74 +88,74 @@
             Functions that fires events in response to a
             condition in another service.
         state (google.cloud.functions_v2.types.Function.State):
             Output only. State of the function.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The last update timestamp of a
             Cloud Function.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Labels associated with this Cloud Function.
-        state_messages (Sequence[google.cloud.functions_v2.types.StateMessage]):
+        state_messages (MutableSequence[google.cloud.functions_v2.types.StateMessage]):
             Output only. State Messages for this Cloud
             Function.
     """
 
     class State(proto.Enum):
         r"""Describes the current state of the function."""
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         FAILED = 2
         DEPLOYING = 3
         DELETING = 4
         UNKNOWN = 5
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    environment = proto.Field(
+    environment: "Environment" = proto.Field(
         proto.ENUM,
         number=10,
         enum="Environment",
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    build_config = proto.Field(
+    build_config: "BuildConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="BuildConfig",
     )
-    service_config = proto.Field(
+    service_config: "ServiceConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ServiceConfig",
     )
-    event_trigger = proto.Field(
+    event_trigger: "EventTrigger" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="EventTrigger",
     )
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=6,
         enum=State,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=8,
     )
-    state_messages = proto.RepeatedField(
+    state_messages: MutableSequence["StateMessage"] = proto.RepeatedField(
         proto.MESSAGE,
         number=9,
         message="StateMessage",
     )
 
 
 class StateMessage(proto.Message):
@@ -172,24 +174,24 @@
     class Severity(proto.Enum):
         r"""Severity of the state message."""
         SEVERITY_UNSPECIFIED = 0
         ERROR = 1
         WARNING = 2
         INFO = 3
 
-    severity = proto.Field(
+    severity: Severity = proto.Field(
         proto.ENUM,
         number=1,
         enum=Severity,
     )
-    type_ = proto.Field(
+    type_: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    message = proto.Field(
+    message: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class StorageSource(proto.Message):
     r"""Location of the source in an archive file in Google Cloud
@@ -207,23 +209,23 @@
             containing source to build.
         generation (int):
             Google Cloud Storage generation for the
             object. If the generation is omitted, the latest
             generation will be used.
     """
 
-    bucket = proto.Field(
+    bucket: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    object_ = proto.Field(
+    object_: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    generation = proto.Field(
+    generation: int = proto.Field(
         proto.INT64,
         number=3,
     )
 
 
 class RepoSource(proto.Message):
     r"""Location of the source in a Google Cloud Source Repository.
@@ -269,42 +271,42 @@
             that step's execution. eg. helloworld (no leading slash
             allowed)
         invert_regex (bool):
             Only trigger a build if the revision regex
             does NOT match the revision regex.
     """
 
-    branch_name = proto.Field(
+    branch_name: str = proto.Field(
         proto.STRING,
         number=3,
         oneof="revision",
     )
-    tag_name = proto.Field(
+    tag_name: str = proto.Field(
         proto.STRING,
         number=4,
         oneof="revision",
     )
-    commit_sha = proto.Field(
+    commit_sha: str = proto.Field(
         proto.STRING,
         number=5,
         oneof="revision",
     )
-    project_id = proto.Field(
+    project_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    repo_name = proto.Field(
+    repo_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    dir_ = proto.Field(
+    dir_: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    invert_regex = proto.Field(
+    invert_regex: bool = proto.Field(
         proto.BOOL,
         number=7,
     )
 
 
 class Source(proto.Message):
     r"""The location of the function source code.
@@ -325,21 +327,21 @@
         repo_source (google.cloud.functions_v2.types.RepoSource):
             If provided, get the source from this
             location in a Cloud Source Repository.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    storage_source = proto.Field(
+    storage_source: "StorageSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="StorageSource",
     )
-    repo_source = proto.Field(
+    repo_source: "RepoSource" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="source",
         message="RepoSource",
     )
 
 
@@ -352,20 +354,20 @@
             A copy of the build's ``source.storage_source``, if exists,
             with any generations resolved.
         resolved_repo_source (google.cloud.functions_v2.types.RepoSource):
             A copy of the build's ``source.repo_source``, if exists,
             with any revisions resolved.
     """
 
-    resolved_storage_source = proto.Field(
+    resolved_storage_source: "StorageSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="StorageSource",
     )
-    resolved_repo_source = proto.Field(
+    resolved_repo_source: "RepoSource" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="RepoSource",
     )
 
 
 class BuildConfig(proto.Message):
@@ -404,15 +406,15 @@
             {workerPool} is the short name of the worker pool.
 
             If the project id is not the same as the function, then the
             Cloud Functions Service Agent
             (service-<project_number>@gcf-admin-robot.iam.gserviceaccount.com)
             must be granted the role Cloud Build Custom Workers Builder
             (roles/cloudbuild.customworkers.builder) in the project.
-        environment_variables (Mapping[str, str]):
+        environment_variables (MutableMapping[str, str]):
             User-provided build-time environment
             variables for the function
         docker_repository (str):
             Optional. User managed repository created in Artifact
             Registry optionally with a customer managed encryption key.
             This is the repository to which the function docker image
             will be pushed after it is built by Cloud Build. If
@@ -423,46 +425,46 @@
             ``projects/{project}/locations/{location}/repositories/{repository}``.
 
             Cross-project repositories are not supported. Cross-location
             repositories are not supported. Repository format must be
             'DOCKER'.
     """
 
-    build = proto.Field(
+    build: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    runtime = proto.Field(
+    runtime: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    entry_point = proto.Field(
+    entry_point: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    source = proto.Field(
+    source: "Source" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="Source",
     )
-    source_provenance = proto.Field(
+    source_provenance: "SourceProvenance" = proto.Field(
         proto.MESSAGE,
         number=8,
         message="SourceProvenance",
     )
-    worker_pool = proto.Field(
+    worker_pool: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    environment_variables = proto.MapField(
+    environment_variables: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
-    docker_repository = proto.Field(
+    docker_repository: str = proto.Field(
         proto.STRING,
         number=7,
     )
 
 
 class ServiceConfig(proto.Message):
     r"""Describes the Service being deployed.
@@ -482,15 +484,15 @@
             The amount of memory available for a
             function. Defaults to 256M. Supported units are
             k, M, G, Mi, Gi. If no unit is supplied the
             value is interpreted as bytes.
             See
             https://github.com/kubernetes/kubernetes/blob/master/staging/src/k8s.io/apimachinery/pkg/api/resource/quantity.go
             a full description.
-        environment_variables (Mapping[str, str]):
+        environment_variables (MutableMapping[str, str]):
             Environment variables that shall be available
             during function execution.
         max_instance_count (int):
             The limit on the maximum number of function instances that
             may coexist at a given time.
 
             In some cases, such as rapid traffic surges, Cloud Functions
@@ -536,17 +538,17 @@
             Whether 100% of traffic is routed to the
             latest revision. On CreateFunction and
             UpdateFunction, when set to true, the revision
             being deployed will serve 100% of traffic,
             ignoring any traffic split settings, if any. On
             GetFunction, true will be returned if the latest
             revision is serving 100% of traffic.
-        secret_environment_variables (Sequence[google.cloud.functions_v2.types.SecretEnvVar]):
+        secret_environment_variables (MutableSequence[google.cloud.functions_v2.types.SecretEnvVar]):
             Secret environment variables configuration.
-        secret_volumes (Sequence[google.cloud.functions_v2.types.SecretVolume]):
+        secret_volumes (MutableSequence[google.cloud.functions_v2.types.SecretVolume]):
             Secret volumes configuration.
         revision (str):
             Output only. The name of service revision.
     """
 
     class VpcConnectorEgressSettings(proto.Enum):
         r"""Available egress settings.
@@ -566,76 +568,76 @@
         If unspecified, ALLOW_ALL will be used.
         """
         INGRESS_SETTINGS_UNSPECIFIED = 0
         ALLOW_ALL = 1
         ALLOW_INTERNAL_ONLY = 2
         ALLOW_INTERNAL_AND_GCLB = 3
 
-    service = proto.Field(
+    service: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    timeout_seconds = proto.Field(
+    timeout_seconds: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    available_memory = proto.Field(
+    available_memory: str = proto.Field(
         proto.STRING,
         number=13,
     )
-    environment_variables = proto.MapField(
+    environment_variables: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=4,
     )
-    max_instance_count = proto.Field(
+    max_instance_count: int = proto.Field(
         proto.INT32,
         number=5,
     )
-    min_instance_count = proto.Field(
+    min_instance_count: int = proto.Field(
         proto.INT32,
         number=12,
     )
-    vpc_connector = proto.Field(
+    vpc_connector: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    vpc_connector_egress_settings = proto.Field(
+    vpc_connector_egress_settings: VpcConnectorEgressSettings = proto.Field(
         proto.ENUM,
         number=7,
         enum=VpcConnectorEgressSettings,
     )
-    ingress_settings = proto.Field(
+    ingress_settings: IngressSettings = proto.Field(
         proto.ENUM,
         number=8,
         enum=IngressSettings,
     )
-    uri = proto.Field(
+    uri: str = proto.Field(
         proto.STRING,
         number=9,
     )
-    service_account_email = proto.Field(
+    service_account_email: str = proto.Field(
         proto.STRING,
         number=10,
     )
-    all_traffic_on_latest_revision = proto.Field(
+    all_traffic_on_latest_revision: bool = proto.Field(
         proto.BOOL,
         number=16,
     )
-    secret_environment_variables = proto.RepeatedField(
+    secret_environment_variables: MutableSequence["SecretEnvVar"] = proto.RepeatedField(
         proto.MESSAGE,
         number=17,
         message="SecretEnvVar",
     )
-    secret_volumes = proto.RepeatedField(
+    secret_volumes: MutableSequence["SecretVolume"] = proto.RepeatedField(
         proto.MESSAGE,
         number=19,
         message="SecretVolume",
     )
-    revision = proto.Field(
+    revision: str = proto.Field(
         proto.STRING,
         number=18,
     )
 
 
 class SecretEnvVar(proto.Message):
     r"""Configuration for a secret environment variable. It has the
@@ -658,27 +660,27 @@
             Version of the secret (version number or the
             string 'latest'). It is recommended to use a
             numeric version for secret environment variables
             as any updates to the secret value is not
             reflected until new instances start.
     """
 
-    key = proto.Field(
+    key: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    project_id = proto.Field(
+    project_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    secret = proto.Field(
+    secret: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    version = proto.Field(
+    version: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class SecretVolume(proto.Message):
     r"""Configuration for a secret volume. It has the information
@@ -699,15 +701,15 @@
             but can also be the project ID) of the project
             that contains the secret. If not set, it is
             assumed that the secret is in the same project
             as the function.
         secret (str):
             Name of the secret in secret manager (not the
             full resource name).
-        versions (Sequence[google.cloud.functions_v2.types.SecretVolume.SecretVersion]):
+        versions (MutableSequence[google.cloud.functions_v2.types.SecretVolume.SecretVersion]):
             List of secret versions to mount for this secret. If empty,
             the ``latest`` version of the secret will be made available
             in a file named after the secret under the mount point.
     """
 
     class SecretVersion(proto.Message):
         r"""Configuration for a single version.
@@ -722,36 +724,36 @@
                 Relative path of the file under the mount path where the
                 secret value for this version will be fetched and made
                 available. For example, setting the mount_path as
                 '/etc/secrets' and path as ``secret_foo`` would mount the
                 secret value file at ``/etc/secrets/secret_foo``.
         """
 
-        version = proto.Field(
+        version: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        path = proto.Field(
+        path: str = proto.Field(
             proto.STRING,
             number=2,
         )
 
-    mount_path = proto.Field(
+    mount_path: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    project_id = proto.Field(
+    project_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    secret = proto.Field(
+    secret: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    versions = proto.RepeatedField(
+    versions: MutableSequence[SecretVersion] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message=SecretVersion,
     )
 
 
 class EventTrigger(proto.Message):
@@ -770,15 +772,15 @@
             function, a different region or multi-region, or
             the global region. If not provided, defaults to
             the same region as the function.
         event_type (str):
             Required. The type of event to observe. For example:
             ``google.cloud.audit.log.v1.written`` or
             ``google.cloud.pubsub.topic.v1.messagePublished``.
-        event_filters (Sequence[google.cloud.functions_v2.types.EventFilter]):
+        event_filters (MutableSequence[google.cloud.functions_v2.types.EventFilter]):
             Criteria used to filter events.
         pubsub_topic (str):
             Optional. The name of a Pub/Sub topic in the same project
             that will be used as the transport topic for the event
             delivery. Format: ``projects/{project}/topics/{topic}``.
 
             This is only valid for events of type
@@ -805,45 +807,45 @@
         r"""Describes the retry policy in case of function's execution
         failure. Retried execution is charged as any other execution.
         """
         RETRY_POLICY_UNSPECIFIED = 0
         RETRY_POLICY_DO_NOT_RETRY = 1
         RETRY_POLICY_RETRY = 2
 
-    trigger = proto.Field(
+    trigger: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    trigger_region = proto.Field(
+    trigger_region: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    event_type = proto.Field(
+    event_type: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    event_filters = proto.RepeatedField(
+    event_filters: MutableSequence["EventFilter"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="EventFilter",
     )
-    pubsub_topic = proto.Field(
+    pubsub_topic: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    service_account_email = proto.Field(
+    service_account_email: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    retry_policy = proto.Field(
+    retry_policy: RetryPolicy = proto.Field(
         proto.ENUM,
         number=7,
         enum=RetryPolicy,
     )
-    channel = proto.Field(
+    channel: str = proto.Field(
         proto.STRING,
         number=8,
     )
 
 
 class EventFilter(proto.Message):
     r"""Filters events based on exact matches on the CloudEvents
@@ -858,38 +860,38 @@
         operator (str):
             Optional. The operator used for matching the events with the
             value of the filter. If not specified, only events that have
             an exact key-value pair specified in the filter are matched.
             The only allowed value is ``match-path-pattern``.
     """
 
-    attribute = proto.Field(
+    attribute: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    value = proto.Field(
+    value: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    operator = proto.Field(
+    operator: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class GetFunctionRequest(proto.Message):
     r"""Request for the ``GetFunction`` method.
 
     Attributes:
         name (str):
             Required. The name of the function which
             details should be obtained.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListFunctionsRequest(proto.Message):
     r"""Request for the ``ListFunctions`` method.
@@ -919,66 +921,66 @@
         order_by (str):
             The sorting order of the resources returned.
             Value should be a comma separated list of
             fields. The default sorting oder is ascending.
             See https://google.aip.dev/132#ordering.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    order_by = proto.Field(
+    order_by: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class ListFunctionsResponse(proto.Message):
     r"""Response for the ``ListFunctions`` method.
 
     Attributes:
-        functions (Sequence[google.cloud.functions_v2.types.Function]):
+        functions (MutableSequence[google.cloud.functions_v2.types.Function]):
             The functions that match the request.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
-        unreachable (Sequence[str]):
+        unreachable (MutableSequence[str]):
             Locations that could not be reached. The
             response does not include any functions from
             these locations.
     """
 
     @property
     def raw_page(self):
         return self
 
-    functions = proto.RepeatedField(
+    functions: MutableSequence["Function"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Function",
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    unreachable = proto.RepeatedField(
+    unreachable: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
 
 
 class CreateFunctionRequest(proto.Message):
     r"""Request for the ``CreateFunction`` method.
@@ -994,24 +996,24 @@
             The ID to use for the function, which will become the final
             component of the function's resource name.
 
             This value should be 4-63 characters, and valid characters
             are /[a-z][0-9]-/.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    function = proto.Field(
+    function: "Function" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="Function",
     )
-    function_id = proto.Field(
+    function_id: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class UpdateFunctionRequest(proto.Message):
     r"""Request for the ``UpdateFunction`` method.
@@ -1021,20 +1023,20 @@
             Required. New version of the function.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to be updated.
             If no field mask is provided, all provided
             fields in the request will be updated.
     """
 
-    function = proto.Field(
+    function: "Function" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Function",
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class DeleteFunctionRequest(proto.Message):
@@ -1042,15 +1044,15 @@
 
     Attributes:
         name (str):
             Required. The name of the function which
             should be deleted.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class GenerateUploadUrlRequest(proto.Message):
     r"""Request of ``GenerateSourceUploadUrl`` method.
@@ -1058,15 +1060,15 @@
     Attributes:
         parent (str):
             Required. The project and location in which the Google Cloud
             Storage signed URL should be generated, specified in the
             format ``projects/*/locations/*``.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class GenerateUploadUrlResponse(proto.Message):
     r"""Response of ``GenerateSourceUploadUrl`` method.
@@ -1086,19 +1088,19 @@
             CreateFunction and UpdateFunction.
 
             Generation defaults to 0, as Cloud Storage provides a new
             generation only upon uploading a new object or version of an
             object.
     """
 
-    upload_url = proto.Field(
+    upload_url: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    storage_source = proto.Field(
+    storage_source: "StorageSource" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="StorageSource",
     )
 
 
 class GenerateDownloadUrlRequest(proto.Message):
@@ -1107,15 +1109,15 @@
     Attributes:
         name (str):
             Required. The name of function for which
             source code Google Cloud Storage signed URL
             should be generated.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class GenerateDownloadUrlResponse(proto.Message):
     r"""Response of ``GenerateDownloadUrl`` method.
@@ -1123,15 +1125,15 @@
     Attributes:
         download_url (str):
             The generated Google Cloud Storage signed URL
             that should be used for function source code
             download.
     """
 
-    download_url = proto.Field(
+    download_url: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListRuntimesRequest(proto.Message):
     r"""Request for the ``ListRuntimes`` method.
@@ -1143,29 +1145,29 @@
             ``projects/*/locations/*``
         filter (str):
             The filter for Runtimes that match the filter
             expression, following the syntax outlined in
             https://google.aip.dev/160.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class ListRuntimesResponse(proto.Message):
     r"""Response for the ``ListRuntimes`` method.
 
     Attributes:
-        runtimes (Sequence[google.cloud.functions_v2.types.ListRuntimesResponse.Runtime]):
+        runtimes (MutableSequence[google.cloud.functions_v2.types.ListRuntimesResponse.Runtime]):
             The runtimes that match the request.
     """
 
     class RuntimeStage(proto.Enum):
         r"""The various stages that a runtime can be in."""
         RUNTIME_STAGE_UNSPECIFIED = 0
         DEVELOPMENT = 1
@@ -1185,45 +1187,45 @@
                 'nodejs12', etc.
             display_name (str):
                 The user facing name, eg 'Go 1.13', 'Node.js
                 12', etc.
             stage (google.cloud.functions_v2.types.ListRuntimesResponse.RuntimeStage):
                 The stage of life this runtime is in, e.g.,
                 BETA, GA, etc.
-            warnings (Sequence[str]):
+            warnings (MutableSequence[str]):
                 Warning messages, e.g., a deprecation
                 warning.
             environment (google.cloud.functions_v2.types.Environment):
                 The environment for the runtime.
         """
 
-        name = proto.Field(
+        name: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        display_name = proto.Field(
+        display_name: str = proto.Field(
             proto.STRING,
             number=5,
         )
-        stage = proto.Field(
+        stage: "ListRuntimesResponse.RuntimeStage" = proto.Field(
             proto.ENUM,
             number=2,
             enum="ListRuntimesResponse.RuntimeStage",
         )
-        warnings = proto.RepeatedField(
+        warnings: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=3,
         )
-        environment = proto.Field(
+        environment: "Environment" = proto.Field(
             proto.ENUM,
             number=4,
             enum="Environment",
         )
 
-    runtimes = proto.RepeatedField(
+    runtimes: MutableSequence[Runtime] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=Runtime,
     )
 
 
 class OperationMetadata(proto.Message):
@@ -1249,54 +1251,54 @@
             [google.rpc.Status.code][google.rpc.Status.code] of 1,
             corresponding to ``Code.CANCELLED``.
         api_version (str):
             API version used to start the operation.
         request_resource (google.protobuf.any_pb2.Any):
             The original request that started the
             operation.
-        stages (Sequence[google.cloud.functions_v2.types.Stage]):
+        stages (MutableSequence[google.cloud.functions_v2.types.Stage]):
             Mechanism for reporting in-progress stages
     """
 
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=1,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         message=timestamp_pb2.Timestamp,
     )
-    target = proto.Field(
+    target: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    verb = proto.Field(
+    verb: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    status_detail = proto.Field(
+    status_detail: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    cancel_requested = proto.Field(
+    cancel_requested: bool = proto.Field(
         proto.BOOL,
         number=6,
     )
-    api_version = proto.Field(
+    api_version: str = proto.Field(
         proto.STRING,
         number=7,
     )
-    request_resource = proto.Field(
+    request_resource: any_pb2.Any = proto.Field(
         proto.MESSAGE,
         number=8,
         message=any_pb2.Any,
     )
-    stages = proto.RepeatedField(
+    stages: MutableSequence["Stage"] = proto.RepeatedField(
         proto.MESSAGE,
         number=9,
         message="Stage",
     )
 
 
 class Stage(proto.Message):
@@ -1310,15 +1312,15 @@
             Message describing the Stage
         state (google.cloud.functions_v2.types.Stage.State):
             Current state of the Stage
         resource (str):
             Resource of the Stage
         resource_uri (str):
             Link to the current Stage resource
-        state_messages (Sequence[google.cloud.functions_v2.types.StateMessage]):
+        state_messages (MutableSequence[google.cloud.functions_v2.types.StateMessage]):
             State messages from the current Stage.
     """
 
     class Name(proto.Enum):
         r"""Possible names for a Stage"""
         NAME_UNSPECIFIED = 0
         ARTIFACT_REGISTRY = 1
@@ -1331,37 +1333,37 @@
     class State(proto.Enum):
         r"""Possible states for a Stage"""
         STATE_UNSPECIFIED = 0
         NOT_STARTED = 1
         IN_PROGRESS = 2
         COMPLETE = 3
 
-    name = proto.Field(
+    name: Name = proto.Field(
         proto.ENUM,
         number=1,
         enum=Name,
     )
-    message = proto.Field(
+    message: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=3,
         enum=State,
     )
-    resource = proto.Field(
+    resource: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    resource_uri = proto.Field(
+    resource_uri: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    state_messages = proto.RepeatedField(
+    state_messages: MutableSequence["StateMessage"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="StateMessage",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-functions-1.8.3/google_cloud_functions.egg-info/PKG-INFO` & `google-cloud-functions-1.9.0/google_cloud_functions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: google-cloud-functions
-Version: 1.8.3
+Version: 1.9.0
+Summary: Google Cloud Functions API client library
 Home-page: https://github.com/googleapis/python-functions
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Cloud Functions API
 =====================================
 
 |stable| |pypi| |versions|
```

### Comparing `google-cloud-functions-1.8.3/google_cloud_functions.egg-info/SOURCES.txt` & `google-cloud-functions-1.9.0/google_cloud_functions.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/cloud/functions/__init__.py
+google/cloud/functions/gapic_version.py
 google/cloud/functions/py.typed
 google/cloud/functions_v1/__init__.py
 google/cloud/functions_v1/gapic_metadata.json
+google/cloud/functions_v1/gapic_version.py
 google/cloud/functions_v1/py.typed
 google/cloud/functions_v1/services/__init__.py
 google/cloud/functions_v1/services/cloud_functions_service/__init__.py
 google/cloud/functions_v1/services/cloud_functions_service/async_client.py
 google/cloud/functions_v1/services/cloud_functions_service/client.py
 google/cloud/functions_v1/services/cloud_functions_service/pagers.py
 google/cloud/functions_v1/services/cloud_functions_service/transports/__init__.py
@@ -18,14 +20,15 @@
 google/cloud/functions_v1/services/cloud_functions_service/transports/grpc.py
 google/cloud/functions_v1/services/cloud_functions_service/transports/grpc_asyncio.py
 google/cloud/functions_v1/types/__init__.py
 google/cloud/functions_v1/types/functions.py
 google/cloud/functions_v1/types/operations.py
 google/cloud/functions_v2/__init__.py
 google/cloud/functions_v2/gapic_metadata.json
+google/cloud/functions_v2/gapic_version.py
 google/cloud/functions_v2/py.typed
 google/cloud/functions_v2/services/__init__.py
 google/cloud/functions_v2/services/function_service/__init__.py
 google/cloud/functions_v2/services/function_service/async_client.py
 google/cloud/functions_v2/services/function_service/client.py
 google/cloud/functions_v2/services/function_service/pagers.py
 google/cloud/functions_v2/services/function_service/transports/__init__.py
@@ -37,15 +40,14 @@
 google_cloud_functions.egg-info/PKG-INFO
 google_cloud_functions.egg-info/SOURCES.txt
 google_cloud_functions.egg-info/dependency_links.txt
 google_cloud_functions.egg-info/namespace_packages.txt
 google_cloud_functions.egg-info/not-zip-safe
 google_cloud_functions.egg-info/requires.txt
 google_cloud_functions.egg-info/top_level.txt
-scripts/fixup_functions_v1_keywords.py
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/functions_v1/__init__.py
 tests/unit/gapic/functions_v1/test_cloud_functions_service.py
 tests/unit/gapic/functions_v2/__init__.py
 tests/unit/gapic/functions_v2/test_function_service.py
```

### Comparing `google-cloud-functions-1.8.3/setup.py` & `google-cloud-functions-1.9.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,91 @@
 # -*- coding: utf-8 -*-
-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import io
 import os
 
 import setuptools  # type: ignore
 
-version = "1.8.3"
+package_root = os.path.abspath(os.path.dirname(__file__))
+
+name = "google-cloud-functions"
+
+
+description = "Google Cloud Functions API client library"
+
+version = {}
+with open(os.path.join(package_root, "google/cloud/functions/gapic_version.py")) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+if version[0] == "0":
+    release_status = "Development Status :: 4 - Beta"
+else:
+    release_status = "Development Status :: 5 - Production/Stable"
+
+dependencies = [
+    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
+    "proto-plus >= 1.22.0, <2.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
+    "grpc-google-iam-v1 >= 0.12.4, < 1.0.0dev",
+]
+url = "https://github.com/googleapis/python-functions"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
+packages = [
+    package
+    for package in setuptools.PEP420PackageFinder.find()
+    if package.startswith("google")
+]
+
+namespaces = ["google"]
+if "google.cloud" in packages:
+    namespaces.append("google.cloud")
 
 setuptools.setup(
-    name="google-cloud-functions",
+    name=name,
     version=version,
+    description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-functions",
-    packages=[
-        package
-        for package in setuptools.PEP420PackageFinder.find()
-        if package.startswith("google")
-    ],
-    namespace_packages=("google", "google.cloud"),
-    platforms="Posix; MacOS X; Windows",
-    include_package_data=True,
-    install_requires=(
-        "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
-        "proto-plus >= 1.22.0, <2.0.0dev",
-        "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
-        "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
-    ),
-    python_requires=">=3.7",
-    scripts=[
-        "scripts/fixup_functions_v1_keywords.py",
-    ],
+    url=url,
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        release_status,
         "Intended Audience :: Developers",
-        "Operating System :: OS Independent",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Operating System :: OS Independent",
         "Topic :: Internet",
-        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+    platforms="Posix; MacOS X; Windows",
+    packages=packages,
+    python_requires=">=3.7",
+    namespace_packages=namespaces,
+    install_requires=dependencies,
+    include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-functions-1.8.3/tests/__init__.py` & `google-cloud-functions-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/tests/unit/__init__.py` & `google-cloud-functions-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/tests/unit/gapic/__init__.py` & `google-cloud-functions-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/tests/unit/gapic/functions_v1/__init__.py` & `google-cloud-functions-1.9.0/tests/unit/gapic/functions_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/tests/unit/gapic/functions_v1/test_cloud_functions_service.py` & `google-cloud-functions-1.9.0/tests/unit/gapic/functions_v1/test_cloud_functions_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from google.auth.exceptions import MutualTLSChannelError
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import options_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account
 from google.protobuf import duration_pb2  # type: ignore
+from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.type import expr_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
```

### Comparing `google-cloud-functions-1.8.3/tests/unit/gapic/functions_v2/__init__.py` & `google-cloud-functions-1.9.0/tests/unit/gapic/functions_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-functions-1.8.3/tests/unit/gapic/functions_v2/test_function_service.py` & `google-cloud-functions-1.9.0/tests/unit/gapic/functions_v2/test_function_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.location import locations_pb2
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import options_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account
+from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
```

