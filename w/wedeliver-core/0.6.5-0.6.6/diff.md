# Comparing `tmp/wedeliver_core-0.6.5.tar.gz` & `tmp/wedeliver_core-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core/dist/.tmp-oxucl5hi/wedeliver_core-0.6.5.tar", last modified: Thu Jun  1 12:10:28 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core/dist/.tmp-6wnxhemk/wedeliver_core-0.6.6.tar", last modified: Thu Jun  1 12:19:56 2023, max compression
```

## Comparing `wedeliver_core-0.6.5.tar` & `wedeliver_core-0.6.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core/
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1561 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3991 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2068 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3700 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4725 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      367 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    11642 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-06-01 12:10:17.000000 wedeliver_core-0.6.5/wedeliver_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-01 12:10:28.000000 wedeliver_core-0.6.5/wedeliver_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3991 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2068 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3700 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4725 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      367 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11642 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-06-01 12:19:47.000000 wedeliver_core-0.6.6/wedeliver_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-01 12:19:56.000000 wedeliver_core-0.6.6/wedeliver_core.egg-info/top_level.txt
```

### Comparing `wedeliver_core-0.6.5/PKG-INFO` & `wedeliver_core-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver_core
-Version: 0.6.5
+Version: 0.6.6
 Summary: weDeliverCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core-0.6.5/setup.py` & `wedeliver_core-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
 ]
 
 setup(
     name='wedeliver_core',
-    version='0.6.5',
+    version='0.6.6',
     description='weDeliverCore package',
     long_description="""# Markdown supported!\n\n* weDeliverCore\n* List of features\n""",
     long_description_content_type='text/markdown',
     url='https://www.wedeliverapp.com/',
     author='Eyad Farra',
     author_email='info@wedeliverapp.com',
     license='MIT',
```

### Comparing `wedeliver_core-0.6.5/wedeliver_core/__init__.py` & `wedeliver_core-0.6.6/wedeliver_core/__init__.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/app_decorators/app_entry.py` & `wedeliver_core-0.6.6/wedeliver_core/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/app_decorators/handle_auth.py` & `wedeliver_core-0.6.6/wedeliver_core/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/app_decorators/handle_exceptions.py` & `wedeliver_core-0.6.6/wedeliver_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/app_decorators/handle_response.py` & `wedeliver_core-0.6.6/wedeliver_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/app_decorators/serializer.py` & `wedeliver_core-0.6.6/wedeliver_core/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/base.py` & `wedeliver_core-0.6.6/wedeliver_core/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,13 +37,13 @@
     @route("/fetch_relational_data", methods=["POST"], require_auth=False)
     def _fetch_relational_data_service(validated_data):
         """
         Swagger definition
         """
         user_data_key = '__user_auth_data__'
         if validated_data.get(user_data_key) is not None:
-            from thrivve_core.helpers.auth import Auth
+            from wedeliver_core.helpers.auth import Auth
             Auth.set_user(validated_data.get(user_data_key))
 
         validated_data.pop(user_data_key)
 
         return fetch_relational_data(**validated_data)
```

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/acl_enum.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/get_file_url.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/amazon/get_s3_client.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/atomic_transactions.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/atomic_transactions_v2.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/auth.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/config.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/database/base_model.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/database/log_model.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/enums.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/exceptions.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/fetch_relational_data.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/filters.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/format_exception.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/get_embedded_function.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/kafka_producer.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/log_config.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/micro_fetcher.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/micro_fetcher.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/notification_center.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/notification_center.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/search_function.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/service_config.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/sql.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/time.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/time.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/topics.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/topics.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/validate_mobile_number.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core/helpers/validate_parameters.py` & `wedeliver_core-0.6.6/wedeliver_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core-0.6.5/wedeliver_core.egg-info/PKG-INFO` & `wedeliver_core-0.6.6/wedeliver_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver-core
-Version: 0.6.5
+Version: 0.6.6
 Summary: weDeliverCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core-0.6.5/wedeliver_core.egg-info/SOURCES.txt` & `wedeliver_core-0.6.6/wedeliver_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

