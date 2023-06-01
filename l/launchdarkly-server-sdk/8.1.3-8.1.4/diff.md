# Comparing `tmp/launchdarkly-server-sdk-8.1.3.tar.gz` & `tmp/launchdarkly-server-sdk-8.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchdarkly-server-sdk-8.1.3.tar", last modified: Wed May  3 20:06:23 2023, max compression
+gzip compressed data, was "launchdarkly-server-sdk-8.1.4.tar", last modified: Thu Jun  1 19:37:51 2023, max compression
```

## Comparing `launchdarkly-server-sdk-8.1.3.tar` & `launchdarkly-server-sdk-8.1.4.tar`

### file list

```diff
@@ -1,151 +1,152 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.281630 launchdarkly-server-sdk-8.1.3/
--rw-r--r--   0 root         (0) root         (0)      556 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      934 2023-05-03 20:06:23.281630 launchdarkly-server-sdk-8.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4155 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/consul-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/dynamodb-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.253631 launchdarkly-server-sdk-8.1.3/launchdarkly_server_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      934 2023-05-03 20:06:23.000000 launchdarkly-server-sdk-8.1.3/launchdarkly_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4447 2023-05-03 20:06:23.000000 launchdarkly-server-sdk-8.1.3/launchdarkly_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 20:06:23.000000 launchdarkly-server-sdk-8.1.3/launchdarkly_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-05-03 20:06:23.000000 launchdarkly-server-sdk-8.1.3/launchdarkly_server_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 20:06:23.000000 launchdarkly-server-sdk-8.1.3/launchdarkly_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.253631 launchdarkly-server-sdk-8.1.3/ldclient/
--rw-r--r--   0 root         (0) root         (0)     3086 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22613 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/client.py
--rw-r--r--   0 root         (0) root         (0)    22770 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/config.py
--rw-r--r--   0 root         (0) root         (0)    43163 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/context.py
--rw-r--r--   0 root         (0) root         (0)     8450 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/evaluation.py
--rw-r--r--   0 root         (0) root         (0)     8002 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/feature_store.py
--rw-r--r--   0 root         (0) root         (0)     5793 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/feature_store_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.257631 launchdarkly-server-sdk-8.1.3/ldclient/impl/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/big_segments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.257631 launchdarkly-server-sdk-8.1.3/ldclient/impl/datasource/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/datasource/feature_requester.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/datasource/polling.py
--rw-r--r--   0 root         (0) root         (0)     7309 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/datasource/streaming.py
--rw-r--r--   0 root         (0) root         (0)    22768 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/evaluator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.261631 launchdarkly-server-sdk-8.1.3/ldclient/impl/events/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4678 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/events/diagnostics.py
--rw-r--r--   0 root         (0) root         (0)     3893 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/events/event_context_formatter.py
--rw-r--r--   0 root         (0) root         (0)    19731 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/events/event_processor.py
--rw-r--r--   0 root         (0) root         (0)     3384 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/events/event_summarizer.py
--rw-r--r--   0 root         (0) root         (0)     6586 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/events/types.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/fixed_thread_pool.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.261631 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.261631 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/consul/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/consul/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5546 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/consul/consul_feature_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.261631 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/dynamodb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/dynamodb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/dynamodb/dynamodb_big_segment_store.py
--rw-r--r--   0 root         (0) root         (0)     8283 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/dynamodb/dynamodb_feature_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.261631 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/files/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6224 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/files/file_data_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.265631 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/redis/redis_big_segment_store.py
--rw-r--r--   0 root         (0) root         (0)     4023 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/redis/redis_feature_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.265631 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/test_data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/test_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/test_data/test_data_source.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/listeners.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/lru_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.265631 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/attribute_ref.py
--rw-r--r--   0 root         (0) root         (0)     2546 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/clause.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/encoder.py
--rw-r--r--   0 root         (0) root         (0)     4057 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/entity.py
--rw-r--r--   0 root         (0) root         (0)     4958 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/feature_flag.py
--rw-r--r--   0 root         (0) root         (0)     4105 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/segment.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/value_parsing.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/model/variation_or_rollout.py
--rw-r--r--   0 root         (0) root         (0)     4963 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/operators.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/repeating_task.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/retry_delay.py
--rw-r--r--   0 root         (0) root         (0)     1111 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/rwlock.py
--rw-r--r--   0 root         (0) root         (0)     7190 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/sse.py
--rw-r--r--   0 root         (0) root         (0)      655 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/stubs.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/impl/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.265631 launchdarkly-server-sdk-8.1.3/ldclient/integrations/
--rw-r--r--   0 root         (0) root         (0)    14183 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28304 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/integrations/test_data.py
--rw-r--r--   0 root         (0) root         (0)    17386 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/interfaces.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/py.typed
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 20:06:18.000000 launchdarkly-server-sdk-8.1.3/ldclient/version.py
--rw-r--r--   0 root         (0) root         (0)     3017 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/ldclient/versioned_data_kind.py
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/redis-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 20:06:23.281630 launchdarkly-server-sdk-8.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2842 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/setup.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/test-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.269631 launchdarkly-server-sdk-8.1.3/testing/
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7441 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/builders.py
--rw-r--r--   0 root         (0) root         (0)     5136 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/feature_store_test_base.py
--rw-r--r--   0 root         (0) root         (0)     5994 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/http_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.277630 launchdarkly-server-sdk-8.1.3/testing/impl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.277630 launchdarkly-server-sdk-8.1.3/testing/impl/datasource/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5360 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/datasource/test_feature_requester.py
--rw-r--r--   0 root         (0) root         (0)     3316 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/datasource/test_polling_processor.py
--rw-r--r--   0 root         (0) root         (0)    13410 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/datasource/test_streaming.py
--rw-r--r--   0 root         (0) root         (0)     3234 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/evaluator_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.277630 launchdarkly-server-sdk-8.1.3/testing/impl/events/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6606 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/events/test_diagnostics.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/events/test_event_context_formatter.py
--rw-r--r--   0 root         (0) root         (0)     2658 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/events/test_event_factory.py
--rw-r--r--   0 root         (0) root         (0)    21504 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/events/test_event_processor.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/events/test_event_summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_attribute_ref.py
--rw-r--r--   0 root         (0) root         (0)     7183 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_big_segments.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_big_segment.py
--rw-r--r--   0 root         (0) root         (0)     5874 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_bucketing.py
--rw-r--r--   0 root         (0) root         (0)     3295 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_clause.py
--rw-r--r--   0 root         (0) root         (0)     3944 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_prerequisites.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_segment.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_target.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_listeners.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     2115 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_model_decode.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_model_encoder.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_operators.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_repeating_task.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_retry_delay.py
--rw-r--r--   0 root         (0) root         (0)     3062 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/impl/test_sse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:06:23.281630 launchdarkly-server-sdk-8.1.3/testing/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4483 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/integrations/big_segment_store_test_base.py
--rw-r--r--   0 root         (0) root         (0)     4418 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/integrations/persistent_feature_store_test_base.py
--rw-r--r--   0 root         (0) root         (0)      969 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/integrations/test_consul.py
--rw-r--r--   0 root         (0) root         (0)     6374 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/integrations/test_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     3974 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/integrations/test_redis.py
--rw-r--r--   0 root         (0) root         (0)    13935 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/integrations/test_test_data_source.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/mock_components.py
--rw-r--r--   0 root         (0) root         (0)     3092 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/proxy_test_util.py
--rw-r--r--   0 root         (0) root         (0)     4755 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/stub_util.py
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/sync_util.py
--rw-r--r--   0 root         (0) root         (0)     2547 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_config.py
--rw-r--r--   0 root         (0) root         (0)    13278 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_context.py
--rw-r--r--   0 root         (0) root         (0)    12086 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_feature_store_helpers.py
--rw-r--r--   0 root         (0) root         (0)     7624 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_file_data_source.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_flags_state.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_in_memory_feature_store.py
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_init.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_ldclient.py
--rw-r--r--   0 root         (0) root         (0)     7749 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_ldclient_end_to_end.py
--rw-r--r--   0 root         (0) root         (0)    14646 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_ldclient_evaluation.py
--rw-r--r--   0 root         (0) root         (0)    10506 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_ldclient_events.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_ldclient_listeners.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-05-03 20:06:17.000000 launchdarkly-server-sdk-8.1.3/testing/test_ldclient_singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.916992 launchdarkly-server-sdk-8.1.4/
+-rw-r--r--   0 root         (0) root         (0)      556 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      934 2023-06-01 19:37:51.916992 launchdarkly-server-sdk-8.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/consul-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/dynamodb-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.888993 launchdarkly-server-sdk-8.1.4/launchdarkly_server_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      934 2023-06-01 19:37:51.000000 launchdarkly-server-sdk-8.1.4/launchdarkly_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4468 2023-06-01 19:37:51.000000 launchdarkly-server-sdk-8.1.4/launchdarkly_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:37:51.000000 launchdarkly-server-sdk-8.1.4/launchdarkly_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-01 19:37:51.000000 launchdarkly-server-sdk-8.1.4/launchdarkly_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-01 19:37:51.000000 launchdarkly-server-sdk-8.1.4/launchdarkly_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.888993 launchdarkly-server-sdk-8.1.4/ldclient/
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22613 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/client.py
+-rw-r--r--   0 root         (0) root         (0)    22770 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/config.py
+-rw-r--r--   0 root         (0) root         (0)    43163 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/context.py
+-rw-r--r--   0 root         (0) root         (0)     8450 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     8002 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/feature_store.py
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/feature_store_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.892993 launchdarkly-server-sdk-8.1.4/ldclient/impl/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/big_segments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.892993 launchdarkly-server-sdk-8.1.4/ldclient/impl/datasource/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/datasource/feature_requester.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/datasource/polling.py
+-rw-r--r--   0 root         (0) root         (0)     7309 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/datasource/streaming.py
+-rw-r--r--   0 root         (0) root         (0)    22768 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/evaluator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.896993 launchdarkly-server-sdk-8.1.4/ldclient/impl/events/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4678 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/events/diagnostics.py
+-rw-r--r--   0 root         (0) root         (0)     3893 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/events/event_context_formatter.py
+-rw-r--r--   0 root         (0) root         (0)    19731 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/events/event_processor.py
+-rw-r--r--   0 root         (0) root         (0)     3384 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/events/event_summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     6586 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/events/types.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/fixed_thread_pool.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.896993 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.896993 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/consul/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/consul/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5546 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/consul/consul_feature_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.896993 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/dynamodb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/dynamodb/dynamodb_big_segment_store.py
+-rw-r--r--   0 root         (0) root         (0)     8283 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/dynamodb/dynamodb_feature_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.896993 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/files/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/files/file_data_source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.896993 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/redis/redis_big_segment_store.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/redis/redis_feature_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.900993 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/test_data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/test_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/test_data/test_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/listeners.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/lru_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.900993 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/attribute_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/clause.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     4057 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/entity.py
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/feature_flag.py
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/segment.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/value_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/model/variation_or_rollout.py
+-rw-r--r--   0 root         (0) root         (0)     4963 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/operators.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/repeating_task.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/retry_delay.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/rwlock.py
+-rw-r--r--   0 root         (0) root         (0)     7190 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/sse.py
+-rw-r--r--   0 root         (0) root         (0)      655 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/stubs.py
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/impl/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.900993 launchdarkly-server-sdk-8.1.4/ldclient/integrations/
+-rw-r--r--   0 root         (0) root         (0)    14183 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28304 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/integrations/test_data.py
+-rw-r--r--   0 root         (0) root         (0)    17386 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 19:37:47.000000 launchdarkly-server-sdk-8.1.4/ldclient/version.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/ldclient/versioned_data_kind.py
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/redis-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 19:37:51.916992 launchdarkly-server-sdk-8.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/test-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.908993 launchdarkly-server-sdk-8.1.4/testing/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7441 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/builders.py
+-rw-r--r--   0 root         (0) root         (0)     5136 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/feature_store_test_base.py
+-rw-r--r--   0 root         (0) root         (0)     5994 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/http_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.912992 launchdarkly-server-sdk-8.1.4/testing/impl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.912992 launchdarkly-server-sdk-8.1.4/testing/impl/datasource/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5360 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/datasource/test_feature_requester.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/datasource/test_polling_processor.py
+-rw-r--r--   0 root         (0) root         (0)    13410 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/datasource/test_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/evaluator_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.912992 launchdarkly-server-sdk-8.1.4/testing/impl/events/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6606 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/events/test_diagnostics.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/events/test_event_context_formatter.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/events/test_event_factory.py
+-rw-r--r--   0 root         (0) root         (0)    21504 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/events/test_event_processor.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/events/test_event_summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_attribute_ref.py
+-rw-r--r--   0 root         (0) root         (0)     7183 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_big_segments.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_big_segment.py
+-rw-r--r--   0 root         (0) root         (0)     5874 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_bucketing.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_clause.py
+-rw-r--r--   0 root         (0) root         (0)     3944 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_prerequisites.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_segment.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_target.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_listeners.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_model_decode.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_model_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_repeating_task.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_retry_delay.py
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/impl/test_sse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:37:51.916992 launchdarkly-server-sdk-8.1.4/testing/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/integrations/big_segment_store_test_base.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/integrations/persistent_feature_store_test_base.py
+-rw-r--r--   0 root         (0) root         (0)      969 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/integrations/test_consul.py
+-rw-r--r--   0 root         (0) root         (0)     6374 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/integrations/test_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/integrations/test_redis.py
+-rw-r--r--   0 root         (0) root         (0)    13935 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/integrations/test_test_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/mock_components.py
+-rw-r--r--   0 root         (0) root         (0)     3092 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/proxy_test_util.py
+-rw-r--r--   0 root         (0) root         (0)     4755 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/stub_util.py
+-rw-r--r--   0 root         (0) root         (0)      377 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/sync_util.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    13278 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_context.py
+-rw-r--r--   0 root         (0) root         (0)    12086 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_feature_store_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     7624 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_file_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_flags_state.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_in_memory_feature_store.py
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_init.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_ldclient.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_ldclient_end_to_end.py
+-rw-r--r--   0 root         (0) root         (0)    14646 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_ldclient_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)    10506 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_ldclient_events.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_ldclient_listeners.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_ldclient_singleton.py
+-rw-r--r--   0 root         (0) root         (0)      786 2023-06-01 19:37:46.000000 launchdarkly-server-sdk-8.1.4/testing/test_util.py
```

### Comparing `launchdarkly-server-sdk-8.1.3/LICENSE.txt` & `launchdarkly-server-sdk-8.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/PKG-INFO` & `launchdarkly-server-sdk-8.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchdarkly-server-sdk
-Version: 8.1.3
+Version: 8.1.4
 Summary: LaunchDarkly SDK for Python
 Home-page: https://github.com/launchdarkly/python-server-sdk
 Author: LaunchDarkly
 Author-email: team@launchdarkly.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `launchdarkly-server-sdk-8.1.3/README.md` & `launchdarkly-server-sdk-8.1.4/README.md`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/launchdarkly_server_sdk.egg-info/PKG-INFO` & `launchdarkly-server-sdk-8.1.4/launchdarkly_server_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchdarkly-server-sdk
-Version: 8.1.3
+Version: 8.1.4
 Summary: LaunchDarkly SDK for Python
 Home-page: https://github.com/launchdarkly/python-server-sdk
 Author: LaunchDarkly
 Author-email: team@launchdarkly.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `launchdarkly-server-sdk-8.1.3/launchdarkly_server_sdk.egg-info/SOURCES.txt` & `launchdarkly-server-sdk-8.1.4/launchdarkly_server_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 testing/test_init.py
 testing/test_ldclient.py
 testing/test_ldclient_end_to_end.py
 testing/test_ldclient_evaluation.py
 testing/test_ldclient_events.py
 testing/test_ldclient_listeners.py
 testing/test_ldclient_singleton.py
+testing/test_util.py
 testing/impl/__init__.py
 testing/impl/evaluator_util.py
 testing/impl/test_attribute_ref.py
 testing/impl/test_big_segments.py
 testing/impl/test_evaluator.py
 testing/impl/test_evaluator_big_segment.py
 testing/impl/test_evaluator_bucketing.py
```

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/__init__.py` & `launchdarkly-server-sdk-8.1.4/ldclient/__init__.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/client.py` & `launchdarkly-server-sdk-8.1.4/ldclient/client.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/config.py` & `launchdarkly-server-sdk-8.1.4/ldclient/config.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/context.py` & `launchdarkly-server-sdk-8.1.4/ldclient/context.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/evaluation.py` & `launchdarkly-server-sdk-8.1.4/ldclient/evaluation.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/feature_store.py` & `launchdarkly-server-sdk-8.1.4/ldclient/feature_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/feature_store_helpers.py` & `launchdarkly-server-sdk-8.1.4/ldclient/feature_store_helpers.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/big_segments.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/big_segments.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/datasource/feature_requester.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/datasource/feature_requester.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/datasource/polling.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/datasource/polling.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/datasource/streaming.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/datasource/streaming.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/evaluator.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/evaluator.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/events/diagnostics.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/events/diagnostics.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/events/event_context_formatter.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/events/event_context_formatter.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/events/event_processor.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/events/event_processor.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/events/event_summarizer.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/events/event_summarizer.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/events/types.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/events/types.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/fixed_thread_pool.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/fixed_thread_pool.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/http.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/http.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/consul/consul_feature_store.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/consul/consul_feature_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/dynamodb/dynamodb_big_segment_store.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/dynamodb/dynamodb_big_segment_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/dynamodb/dynamodb_feature_store.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/dynamodb/dynamodb_feature_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/files/file_data_source.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/files/file_data_source.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/redis/redis_big_segment_store.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/redis/redis_big_segment_store.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ldclient import log
 from ldclient.interfaces import BigSegmentStore, BigSegmentStoreMetadata
+from ldclient.impl.util import redact_password
 
 from typing import Any, Optional, Dict, Set, cast
 
 have_redis = False
 try:
     import redis
     have_redis = True
@@ -17,15 +18,15 @@
     KEY_USER_EXCLUDE = ':big_segment_exclude:'
 
     def __init__(self, url: str, prefix: Optional[str], redis_opts: Dict[str, Any]):
         if not have_redis:
             raise NotImplementedError("Cannot use Redis Big Segment store because redis package is not installed")
         self._prefix = prefix or 'launchdarkly'
         self._pool = redis.ConnectionPool.from_url(url=url, **redis_opts)
-        log.info("Started RedisBigSegmentStore connected to URL: " + url + " using prefix: " + self._prefix)
+        log.info("Started RedisBigSegmentStore connected to URL: " + redact_password(url) + " using prefix: " + self._prefix)
 
     def get_metadata(self) -> BigSegmentStoreMetadata:
         r = redis.Redis(connection_pool=self._pool)
         value = r.get(self._prefix + self.KEY_LAST_UP_TO_DATE)
         if value is None:
             return BigSegmentStoreMetadata(None)
```

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/redis/redis_feature_store.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/redis/redis_feature_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,27 @@
     have_redis = True
 except ImportError:
     pass
 
 from ldclient import log
 from ldclient.interfaces import DiagnosticDescription, FeatureStoreCore
 from ldclient.versioned_data_kind import FEATURES
+from ldclient.impl.util import redact_password
 
 from typing import Any, Dict
 
 
 class _RedisFeatureStoreCore(DiagnosticDescription, FeatureStoreCore):
     def __init__(self, url, prefix, redis_opts: Dict[str, Any]):
         if not have_redis:
             raise NotImplementedError("Cannot use Redis feature store because redis package is not installed")
         self._prefix = prefix or 'launchdarkly'
         self._pool = redis.ConnectionPool.from_url(url=url, **redis_opts)
         self.test_update_hook = None  # exposed for testing
-        log.info("Started RedisFeatureStore connected to URL: " + url + " using prefix: " + self._prefix)
+        log.info("Started RedisFeatureStore connected to URL: " + redact_password(url) + " using prefix: " + self._prefix)
 
     def _items_key(self, kind):
         return "{0}:{1}".format(self._prefix, kind.namespace)
 
     def init_internal(self, all_data):
         pipe = redis.Redis(connection_pool=self._pool).pipeline()
```

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/integrations/test_data/test_data_source.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/integrations/test_data/test_data_source.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/listeners.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/listeners.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/lru_cache.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/lru_cache.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/model/attribute_ref.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/model/attribute_ref.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/model/clause.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/model/clause.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/model/entity.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/model/entity.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/model/feature_flag.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/model/feature_flag.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/model/segment.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/model/segment.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/model/value_parsing.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/model/value_parsing.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/model/variation_or_rollout.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/model/variation_or_rollout.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/operators.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/operators.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/repeating_task.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/repeating_task.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/retry_delay.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/retry_delay.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/rwlock.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/rwlock.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/sse.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/sse.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/stubs.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/stubs.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/impl/util.py` & `launchdarkly-server-sdk-8.1.4/ldclient/impl/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import re
 import sys
 import time
 
 from typing import Any
 from ldclient.impl.http import _base_headers
+from urllib.parse import urlparse, urlunparse
 
 
 def current_time_millis() -> int:
     return int(time.time() * 1000)
 
 
 log = logging.getLogger('ldclient.util')  # historical logger name
@@ -128,7 +129,21 @@
     for attr in attrs:
         val = attrdict.get(attr)
         if val is not None and not isinstance(val, str):
             if newdict is None:
                 newdict = attrdict.copy()
             newdict[attr] = str(val)
     return attrdict if newdict is None else newdict
+
+def redact_password(url: str) -> str:
+    """
+    Replace any embedded password in the provided URL with 'xxxx'. This is
+    useful for ensuring sensitive information included in a URL isn't logged.
+    """
+    parts = urlparse(url)
+    if parts.password is None:
+        return url
+
+    updated = parts.netloc.replace(parts.password, "xxxx")
+    parts = parts._replace(netloc=updated)
+
+    return urlunparse(parts)
```

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/integrations/__init__.py` & `launchdarkly-server-sdk-8.1.4/ldclient/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/integrations/test_data.py` & `launchdarkly-server-sdk-8.1.4/ldclient/integrations/test_data.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/interfaces.py` & `launchdarkly-server-sdk-8.1.4/ldclient/interfaces.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/ldclient/versioned_data_kind.py` & `launchdarkly-server-sdk-8.1.4/ldclient/versioned_data_kind.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/setup.py` & `launchdarkly-server-sdk-8.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/builders.py` & `launchdarkly-server-sdk-8.1.4/testing/builders.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/feature_store_test_base.py` & `launchdarkly-server-sdk-8.1.4/testing/feature_store_test_base.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/http_util.py` & `launchdarkly-server-sdk-8.1.4/testing/http_util.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/datasource/test_feature_requester.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/datasource/test_feature_requester.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/datasource/test_polling_processor.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/datasource/test_polling_processor.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/datasource/test_streaming.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/datasource/test_streaming.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/evaluator_util.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/evaluator_util.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/events/test_diagnostics.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/events/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/events/test_event_context_formatter.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/events/test_event_context_formatter.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/events/test_event_factory.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/events/test_event_factory.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/events/test_event_processor.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/events/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/events/test_event_summarizer.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/events/test_event_summarizer.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_attribute_ref.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_attribute_ref.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_big_segments.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_big_segments.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_big_segment.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_big_segment.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_bucketing.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_bucketing.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_clause.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_clause.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_prerequisites.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_prerequisites.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_segment.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_segment.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_evaluator_target.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_evaluator_target.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_listeners.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_listeners.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_lru_cache.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_model_decode.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_model_decode.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_operators.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_operators.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_repeating_task.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_repeating_task.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_retry_delay.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_retry_delay.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/impl/test_sse.py` & `launchdarkly-server-sdk-8.1.4/testing/impl/test_sse.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/integrations/big_segment_store_test_base.py` & `launchdarkly-server-sdk-8.1.4/testing/integrations/big_segment_store_test_base.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/integrations/persistent_feature_store_test_base.py` & `launchdarkly-server-sdk-8.1.4/testing/integrations/persistent_feature_store_test_base.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/integrations/test_consul.py` & `launchdarkly-server-sdk-8.1.4/testing/integrations/test_consul.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/integrations/test_dynamodb.py` & `launchdarkly-server-sdk-8.1.4/testing/integrations/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/integrations/test_redis.py` & `launchdarkly-server-sdk-8.1.4/testing/integrations/test_redis.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/integrations/test_test_data_source.py` & `launchdarkly-server-sdk-8.1.4/testing/integrations/test_test_data_source.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/mock_components.py` & `launchdarkly-server-sdk-8.1.4/testing/mock_components.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/proxy_test_util.py` & `launchdarkly-server-sdk-8.1.4/testing/proxy_test_util.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/stub_util.py` & `launchdarkly-server-sdk-8.1.4/testing/stub_util.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_config.py` & `launchdarkly-server-sdk-8.1.4/testing/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,11 +59,14 @@
 
 @pytest.fixture(params = [
     " ",
     "@",
     ":",
     "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789._-a"
 ])
-def application_will_drop_invalid_values(value):
-    application = {"id": value, "version": value}
+def invalid_application_tags(request):
+    return request.param
+
+def test_application_will_drop_invalid_values(invalid_application_tags):
+    application = {"id": invalid_application_tags, "version": invalid_application_tags}
     config = Config(sdk_key = "SDK_KEY", application = application)
     assert config.application == {"id": "", "version": ""}
```

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_context.py` & `launchdarkly-server-sdk-8.1.4/testing/test_context.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_feature_store_helpers.py` & `launchdarkly-server-sdk-8.1.4/testing/test_feature_store_helpers.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_file_data_source.py` & `launchdarkly-server-sdk-8.1.4/testing/test_file_data_source.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_flags_state.py` & `launchdarkly-server-sdk-8.1.4/testing/test_flags_state.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_init.py` & `launchdarkly-server-sdk-8.1.4/testing/test_init.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_ldclient.py` & `launchdarkly-server-sdk-8.1.4/testing/test_ldclient.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_ldclient_end_to_end.py` & `launchdarkly-server-sdk-8.1.4/testing/test_ldclient_end_to_end.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_ldclient_evaluation.py` & `launchdarkly-server-sdk-8.1.4/testing/test_ldclient_evaluation.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_ldclient_events.py` & `launchdarkly-server-sdk-8.1.4/testing/test_ldclient_events.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_ldclient_listeners.py` & `launchdarkly-server-sdk-8.1.4/testing/test_ldclient_listeners.py`

 * *Files identical despite different names*

### Comparing `launchdarkly-server-sdk-8.1.3/testing/test_ldclient_singleton.py` & `launchdarkly-server-sdk-8.1.4/testing/test_ldclient_singleton.py`

 * *Files identical despite different names*

