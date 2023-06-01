# Comparing `tmp/th2_data_services_lwdp-2.0.3.0.dev5145692687.tar.gz` & `tmp/th2_data_services_lwdp-2.0.3.0.dev5145827351.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.0.3.0.dev5145692687.tar", last modified: Thu Jun  1 14:40:05 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.0.3.0.dev5145827351.tar", last modified: Thu Jun  1 14:53:17 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687.tar` & `th2_data_services_lwdp-2.0.3.0.dev5145827351.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-01 14:39:45.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    40637 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    13515 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-01 14:36:11.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-01 14:40:05.000000 th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-01 14:52:50.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42064 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13925 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-01 14:49:36.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-01 14:53:16.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-06-01 14:53:17.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 14:53:16.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-01 14:53:16.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-01 14:53:16.000000 th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/PKG-INFO` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.0.3.0.dev5145692687
+Version: 2.0.3.0.dev5145827351
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/README.md` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/setup.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,20 +230,15 @@
             return [api.get_url_get_message_aliases(book_id=self._book_id)]
         else:
             return [
                 api.get_url_get_message_aliases(
                     self._book_id, self._start_timestamp, self._end_timestamp
                 )
             ]
-
-    def _stream_chunk_data(self, sse_events_stream):
-        for chunk in sse_events_stream:
-            for event in chunk:
-                yield event
-
+        
     def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
         """Parses SSEEvents Into Data Object.
 
         Args:
             data_source: HTTPDataSource
 
         Returns:
@@ -251,39 +246,75 @@
         """
         sse_events_stream = partial(self._sse_events_stream, data_source)
         data = Data(sse_events_stream).map_stream(self._sse_handler).use_cache(self._cache)
         data.metadata["urls"] = self._get_urls(data_source)
         return data
 
 
-class GetMessageGroups(IHTTPCommand):
+class GetMessageGroups(SSEHandlerClassBase):
     """A Class-Command for request to lw-data-provider.
 
     It retrieves a list of message groups in book.
 
     Returns:
         dict: List[str].
     """
 
-    def __init__(self, book_id: str):
-        """GetMessageGroups constructor.
+    def __init__(
+        self,
+        book_id: str,
+        start_timestamp: datetime = None,
+        end_timestamp: datetime = None,
+        buffer_limit: int = DEFAULT_BUFFER_LIMIT,
+        cache: bool = False,
+    ) -> None:
+        """GetMessageGroups Constructor.
+
+        If start_timestamp and end_timestamp are not provided, it returns all aliases.
 
         Args:
-            book_id: Name of book to search in.
+            book_id (str): Book ID.
+            start_timestamp (datetime): Start Timestamp.
+            end_timestamp (datetime): End Timestamp.
+            cache (Optional, bool): Cache Status. Defaults To `False`.
+            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
-        super().__init__()
+        super().__init__(cache, buffer_limit=buffer_limit)
+        if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
+            self._all_results = True
+        else:
+            _check_datetime(start_timestamp)
+            _check_datetime(end_timestamp)
+            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            self._all_results = False
         self._book_id = book_id
 
-    def handle(self, data_source: HTTPDataSource) -> List[str]:  # noqa: D102
-        api: HTTPAPI = data_source.source_api
-        url = api.get_url_get_message_groups(self._book_id)
-
-        # LOG         logger.info(url)
+    def _get_urls(self, data_source: HTTPDataSource):
+        api = data_source.source_api
+        if self._all_results:
+            return [api.get_url_get_message_groups(book_id=self._book_id)]
+        else:
+            return [
+                api.get_url_get_message_groups(
+                    self._book_id, self._start_timestamp, self._end_timestamp
+                )
+            ]
 
-        return api.execute_request(url).json()
+    def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
+        """Parses SSEEvents Into Data Object.
+        Args:
+            data_source: HTTPDataSource
+        Returns:
+             Data
+        """
+        sse_events_stream = partial(self._sse_events_stream, data_source)
+        data = Data(sse_events_stream).map_stream(self._sse_handler).use_cache(self._cache)
+        data.metadata["urls"] = self._get_urls(data_source)
+        return data
 
 
 class GetBooks(IHTTPCommand):
     """A Class-Command for request to lw-data-provider.
 
     It retrieves a list of books from provider.
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,33 @@
             "endTimestamp": end_timestamp,
             "chunkedSize": chunked_size,
         }
 
         url += "&".join(f"{k}={v}" for k, v in kwargs.items() if v is not None)
         return self.__encode_url(url)
 
-    def get_url_get_message_groups(self, book_id: str) -> str:
-        """REST-API `book/{bookID}/message/groups` call returns a list of message groups in book named bookID."""
-        return self.__encode_url(f"{self._url}/book/{book_id}/message/groups")
+    def get_url_get_message_groups(
+        self,
+        book_id: str,
+        start_timestamp: int = None,
+        end_timestamp: int = None,
+        chunked_size: int = None,
+    ) -> str:
+        """REST-API `book/{bookID}/message/groups/sse` call creates an sse channel of message groups in book named bookID."""
+        url = f"{self._url}/book/{book_id}/message/groups/sse?"
 
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "chunkedSize": chunked_size,
+        }
+
+        url += "&".join(f"{k}={v}" for k, v in kwargs.items() if v is not None)
+        return self.__encode_url(url)
+    
     def get_url_find_event_by_id(self, event_id: str) -> str:
         """REST-API `event` call returns a single event with the specified id."""
         return self.__encode_url(f"{self._url}/event/{event_id}")
 
     def get_url_find_message_by_id(self, message_id: str, only_raw: bool = False) -> str:
         """REST-API `message` call returns a single      message with the specified id."""
         return self.__encode_url(f"{self._url}/message/{message_id}?onlyRaw={only_raw}")
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services/data_source/lwdp/utils/misc.py` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services/data_source/lwdp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.0.3.0.dev5145692687
+Version: 2.0.3.0.dev5145827351
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5145692687/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.0.3.0.dev5145827351/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

