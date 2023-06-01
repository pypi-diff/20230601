# Comparing `tmp/logprep-6.3.0.tar.gz` & `tmp/logprep-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logprep-6.3.0.tar", last modified: Mon May 22 10:47:03 2023, max compression
+gzip compressed data, was "logprep-6.4.0.tar", last modified: Thu Jun  1 10:39:40 2023, max compression
```

## Comparing `logprep-6.3.0.tar` & `logprep-6.4.0.tar`

### file list

```diff
@@ -1,536 +1,536 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.664559 logprep-6.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-22 10:46:57.000000 logprep-6.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 10:46:57.000000 logprep-6.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-05-22 10:47:03.664559 logprep-6.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-05-22 10:46:57.000000 logprep-6.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.664559 logprep-6.3.0/logprep/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-22 10:47:03.664559 logprep-6.3.0/logprep/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/confluent_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/confluent_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/confluent_kafka/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/confluent_kafka/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/console/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/dummy/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/dummy/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/elasticsearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/file/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/http/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/json/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/jsonl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/jsonl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/jsonl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/jsonl/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/opensearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/s3/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/factory_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/filter/expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/filter/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/filter/expression/filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/filter/lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/rule_tree/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/rule_tree/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/rule_tree/rule_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/metrics/metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/metrics/metric_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/base/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/calculator/fourFn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/calculator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/calculator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/concatenator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/concatenator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/datetime_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/datetime_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/deleter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/deleter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dissector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dissector/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_label_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_label_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dropper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dropper/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/field_manager/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/field_manager/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_adder/mysql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_adder/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_adder/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/geoip_enricher/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/geoip_enricher/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/grokker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/grokker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/hyperscan_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/hyperscan_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/ip_informer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/ip_informer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/key_checker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/key_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/key_checker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/key_checker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/labeler/labeling_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/labeler/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/labeler/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/list_comparison/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/list_comparison/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/normalizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/normalizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pre_detector/ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pre_detector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pre_detector/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pseudonymizer/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pseudonymizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pseudonymizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/requester/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/requester/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/selective_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/selective_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/string_splitter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/string_splitter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/template_replacer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/template_replacer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamp_differ/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamp_differ/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamper/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.640559 logprep-6.3.0/logprep/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/aggregating_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.640559 logprep-6.3.0/logprep/util/auto_rule_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/auto_rule_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/auto_rule_tester/auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/getter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.640559 logprep-6.3.0/logprep/util/grok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/grok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.616558 logprep-6.3.0/logprep/util/grok/patterns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.640559 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/aws
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bind
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/exim
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/java
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/maven
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/rails
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/redis
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/squid
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/zeek
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/logprep/util/grok/patterns/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/aws
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/bind
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/exim
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/java
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/maven
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/mcollective-patterns
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/rails
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/redis
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/squid
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/json_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/multiprocessing_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/pipeline_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/pre_detector_rule_matching_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.620558 logprep-6.3.0/logprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 10:46:57.000000 logprep-6.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-22 10:47:03.664559 logprep-6.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-22 10:46:57.000000 logprep-6.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_config_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_full_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_multiple_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_pre_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_wineventlog_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_wineventlog_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_wineventlog_pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/ci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/ci/runner-image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/ci/runner-image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/ci/runner-image/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/ci/runner-image/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/ci/runner-image/scripts/compare_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/ConfigurationForTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/FilledTempFile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/ruledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/testdata/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/testdata/unit/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/unit/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/unit/clusterer/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_confluent_kafka_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_confluent_kafka_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_confluent_kafka_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_dummy_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_dummy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_elasticsearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_file_input_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_file_input_not_tailing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_file_input_start_at_end_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_jsonl_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_jsonl_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_opensearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_s3_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/exceptions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/exceptions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/exceptions/processor/test_processing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/filter/test_filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/filter/test_lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/rule_tree/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    27846 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/rule_tree/test_rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/rule_tree/test_rule_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/test_pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/metrics/test_metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/metrics/test_metric_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_amides_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/calculator/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/calculator/test_calculator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/concatenator/test_concatenator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/concatenator/test_concatenator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/deleter/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/deleter/test_deleter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dissector/test_dissector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dissector/test_dissector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dropper/test_dropper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dropper/test_dropper_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18589 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/field_manager/test_field_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/field_manager/test_field_manager_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_adder/test_generic_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/grokker/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/grokker/test_grokker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/grokker/test_grokker_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/ip_informer/test_ip_informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/labeler/test_labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/labeler/test_labeler_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/labeler/test_labeling_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/list_comparison/test_list_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/normalizer/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/normalizer/test_normalizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pre_detector/test_ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pre_detector/test_pre_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pseudonymizer/test_encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/requester/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/requester/test_requester_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/string_splitter/test_string_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/template_replacer/test_template_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/test_processor_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/test_processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamper/test_timestamper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamper/test_timestamper_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/test_run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.664559 logprep-6.3.0/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_helper_add_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/tests_json_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.664559 logprep-6.3.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/util/testhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-05-22 10:46:57.000000 logprep-6.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.572381 logprep-6.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-01 10:39:35.000000 logprep-6.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-01 10:39:35.000000 logprep-6.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-06-01 10:39:40.572381 logprep-6.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-06-01 10:39:35.000000 logprep-6.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.572381 logprep-6.4.0/logprep/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 10:39:40.572381 logprep-6.4.0/logprep/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/abc/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/abc/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/abc/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/abc/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/abc/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/abc/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/confluent_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:35.000000 logprep-6.4.0/logprep/connector/confluent_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/confluent_kafka/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/confluent_kafka/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/console/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/dummy/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/dummy/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/elasticsearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/file/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/http/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/json/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/jsonl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/jsonl/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/opensearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/connector/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/connector/s3/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/factory_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/filter/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/filter/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/filter/expression/filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/filter/lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/framework/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/framework/pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/framework/rule_tree/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/framework/rule_tree/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/framework/rule_tree/rule_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/metrics/metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/metrics/metric_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/amides/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/amides/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/amides/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/amides/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/amides/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/base/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/calculator/fourFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/calculator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/calculator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/clusterer/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/clusterer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/clusterer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/clusterer/signature_calculation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/clusterer/signature_calculation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/clusterer/signature_calculation/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/concatenator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/concatenator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/datetime_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/datetime_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/deleter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/deleter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/dissector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/dissector/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/domain_label_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/domain_label_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.544381 logprep-6.4.0/logprep/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/domain_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/domain_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/dropper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/dropper/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/field_manager/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/field_manager/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/generic_adder/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/generic_adder/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/generic_adder/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/generic_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/generic_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/geoip_enricher/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/geoip_enricher/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/grokker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/grokker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/hyperscan_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/hyperscan_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/ip_informer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/ip_informer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/key_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/key_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/key_checker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/key_checker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/labeler/labeling_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/labeler/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/labeler/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/list_comparison/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/list_comparison/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/normalizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/normalizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/pre_detector/ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/pre_detector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/pre_detector/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/pseudonymizer/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/pseudonymizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/pseudonymizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.548381 logprep-6.4.0/logprep/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/requester/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/requester/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.552381 logprep-6.4.0/logprep/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/selective_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/selective_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.552381 logprep-6.4.0/logprep/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/string_splitter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/string_splitter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.552381 logprep-6.4.0/logprep/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/template_replacer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/template_replacer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.552381 logprep-6.4.0/logprep/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/timestamp_differ/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/timestamp_differ/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.552381 logprep-6.4.0/logprep/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/timestamper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/processor/timestamper/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.552381 logprep-6.4.0/logprep/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/aggregating_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.552381 logprep-6.4.0/logprep/util/auto_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/auto_rule_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/auto_rule_tester/auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.552381 logprep-6.4.0/logprep/util/grok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/grok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.536381 logprep-6.4.0/logprep/util/grok/patterns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.556381 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/maven
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/zeek
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.556381 logprep-6.4.0/logprep/util/grok/patterns/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/maven
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/mcollective-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok/patterns/legacy/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/json_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/multiprocessing_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/pipeline_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/pre_detector_rule_matching_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-01 10:39:36.000000 logprep-6.4.0/logprep/util/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.540381 logprep-6.4.0/logprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-06-01 10:39:40.000000 logprep-6.4.0/logprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-01 10:39:40.000000 logprep-6.4.0/logprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:39:40.000000 logprep-6.4.0/logprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 10:39:40.000000 logprep-6.4.0/logprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-01 10:39:40.000000 logprep-6.4.0/logprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 10:39:40.000000 logprep-6.4.0/logprep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-01 10:39:36.000000 logprep-6.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 10:39:40.572381 logprep-6.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-01 10:39:36.000000 logprep-6.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.556381 logprep-6.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_config_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_full_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_multiple_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_pre_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_wineventlog_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_wineventlog_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/test_wineventlog_pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/acceptance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/ci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/ci/runner-image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/ci/runner-image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/ci/runner-image/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/ci/runner-image/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/ci/runner-image/scripts/compare_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/testdata/ConfigurationForTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/testdata/FilledTempFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/testdata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/testdata/ruledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/testdata/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/testdata/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/testdata/unit/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/testdata/unit/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/testdata/unit/clusterer/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/unit/component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/unit/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_confluent_kafka_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_confluent_kafka_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_confluent_kafka_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_dummy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_dummy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_elasticsearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_file_input_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_file_input_not_tailing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_file_input_start_at_end_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_jsonl_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_jsonl_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_opensearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/connector/test_s3_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/unit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/unit/exceptions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/exceptions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/exceptions/processor/test_processing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/unit/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22087 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/filter/test_filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/filter/test_lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.560381 logprep-6.4.0/tests/unit/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/framework/rule_tree/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27846 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/framework/rule_tree/test_rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/framework/rule_tree/test_rule_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/framework/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/framework/test_pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/metrics/test_metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/metrics/test_metric_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/amides/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/amides/test_amides_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/amides/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/amides/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/amides/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/calculator/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/calculator/test_calculator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/clusterer/test_clusterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/clusterer/test_clusterer_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/concatenator/test_concatenator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/concatenator/test_concatenator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/deleter/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/deleter/test_deleter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/dissector/test_dissector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/dissector/test_dissector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.564381 logprep-6.4.0/tests/unit/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/dropper/test_dropper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/dropper/test_dropper_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/field_manager/test_field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/field_manager/test_field_manager_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/generic_adder/test_generic_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/grokker/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/grokker/test_grokker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/grokker/test_grokker_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/ip_informer/test_ip_informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/labeler/test_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/labeler/test_labeler_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/labeler/test_labeling_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/list_comparison/test_list_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/normalizer/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/normalizer/test_normalizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/pre_detector/test_ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/pre_detector/test_pre_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/pseudonymizer/test_encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/requester/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/requester/test_requester_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.568381 logprep-6.4.0/tests/unit/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/string_splitter/test_string_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.572381 logprep-6.4.0/tests/unit/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/template_replacer/test_template_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/test_processor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/test_processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.572381 logprep-6.4.0/tests/unit/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.572381 logprep-6.4.0/tests/unit/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/timestamper/test_timestamper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/processor/timestamper/test_timestamper_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/test_run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.572381 logprep-6.4.0/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_helper_add_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/unit/util/tests_json_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:40.572381 logprep-6.4.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-01 10:39:36.000000 logprep-6.4.0/tests/util/testhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-06-01 10:39:36.000000 logprep-6.4.0/versioneer.py
```

### Comparing `logprep-6.3.0/LICENSE` & `logprep-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/PKG-INFO` & `logprep-6.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.3.0
+Version: 6.4.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.3.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.4.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.3.0/README.md` & `logprep-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/abc/component.py` & `logprep-6.4.0/logprep/abc/component.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/abc/connector.py` & `logprep-6.4.0/logprep/abc/connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/abc/getter.py` & `logprep-6.4.0/logprep/abc/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/abc/input.py` & `logprep-6.4.0/logprep/abc/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/abc/output.py` & `logprep-6.4.0/logprep/abc/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/abc/processor.py` & `logprep-6.4.0/logprep/abc/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/configuration.py` & `logprep-6.4.0/logprep/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/confluent_kafka/input.py` & `logprep-6.4.0/logprep/connector/confluent_kafka/input.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from functools import cached_property, partial
 from logging import Logger
 from socket import getfqdn
 from typing import Any, List, Optional, Tuple, Union
 
 import msgspec
 from attrs import define, field, validators
-from confluent_kafka import Consumer, KafkaException
+from confluent_kafka import Consumer, KafkaException, TopicPartition
 
 from logprep.abc.input import CriticalInputError, Input
 from logprep.abc.output import FatalOutputError
 from logprep.util.validators import dict_with_keys_validator
 
 
 class ConfluentKafkaInput(Input):
@@ -274,15 +274,25 @@
         Should be called by output connectors if they are finished processing a batch of records.
         This is only used if automatic offest storing is disabled in the kafka input.
         The last valid record for each partition is be used by this method to update all offsets.
         """
         if not self._config.enable_auto_offset_store:
             if self._last_valid_records:
                 for last_valid_records in self._last_valid_records.values():
-                    self._consumer.store_offsets(message=last_valid_records)
+                    try:
+                        self._consumer.store_offsets(message=last_valid_records)
+                    except KafkaException:
+                        topic = self._consumer.list_topics(topic=self._config.topic)
+                        partition_keys = list(topic.topics[self._config.topic].partitions.keys())
+                        partitions = [
+                            TopicPartition(self._config.topic, partition)
+                            for partition in partition_keys
+                        ]
+                        self._consumer.assign(partitions)
+                        self._consumer.store_offsets(message=last_valid_records)
 
     def setup(self):
         super().setup()
         try:
             _ = self._consumer
         except (KafkaException, ValueError) as error:
             raise FatalOutputError(self, str(error)) from error
```

### Comparing `logprep-6.3.0/logprep/connector/confluent_kafka/output.py` & `logprep-6.4.0/logprep/connector/confluent_kafka/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/console/output.py` & `logprep-6.4.0/logprep/connector/console/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/dummy/input.py` & `logprep-6.4.0/logprep/connector/dummy/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/dummy/output.py` & `logprep-6.4.0/logprep/connector/dummy/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/elasticsearch/output.py` & `logprep-6.4.0/logprep/connector/elasticsearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/file/input.py` & `logprep-6.4.0/logprep/connector/file/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/http/input.py` & `logprep-6.4.0/logprep/connector/http/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/json/input.py` & `logprep-6.4.0/logprep/connector/json/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/jsonl/input.py` & `logprep-6.4.0/logprep/connector/jsonl/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/jsonl/output.py` & `logprep-6.4.0/logprep/connector/jsonl/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/opensearch/output.py` & `logprep-6.4.0/logprep/connector/opensearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/connector/s3/output.py` & `logprep-6.4.0/logprep/connector/s3/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/factory.py` & `logprep-6.4.0/logprep/factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/factory_error.py` & `logprep-6.4.0/logprep/factory_error.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/filter/expression/filter_expression.py` & `logprep-6.4.0/logprep/filter/expression/filter_expression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module contains all filter expressions used for matching rules."""
 
-from typing import List, Any
 import re
-from itertools import chain, zip_longest
 from abc import ABC, abstractmethod
+from itertools import chain, zip_longest
+from typing import List, Any
 
 
 class FilterExpressionError(BaseException):
     """Base class for FilterExpression related exceptions."""
 
 
 class KeyDoesNotExistError(FilterExpressionError):
@@ -96,14 +96,20 @@
         -------
         str
             Returns dotted string.
 
         """
         return ".".join([str(i) for i in key_list])
 
+    def get_lucene_filter(self):
+        """Returns a filter string that is partially lucene complete. As lucene does not support
+        regex the corresponding regex field is left as a value inside the lucene filter such that
+        the end user can decide for themselves what they want to do with this information"""
+        return str(self)
+
 
 class Always(FilterExpression):
     """Filter expression that can be set to match always or never."""
 
     def __init__(self, value: Any):
         self._value = value
 
@@ -111,24 +117,32 @@
         if self._value:
             return "TRUE"
         return "FALSE"
 
     def does_match(self, document: dict):
         return self._value
 
+    def get_lucene_filter(self):
+        if self._value:
+            return "*"
+        return ""
+
 
 class Not(FilterExpression):
     """Filter expression that negates a match."""
 
     def __init__(self, expression: FilterExpression):
         self.expression = expression
 
     def __repr__(self) -> str:
         return f"NOT({str(self.expression)})"
 
+    def get_lucene_filter(self):
+        return f"NOT ({self.expression.get_lucene_filter()})"
+
     def does_match(self, document: dict) -> bool:
         return not self.expression.matches(document)
 
 
 class CompoundFilterExpression(FilterExpression):
     """Base class of filter expressions that combine other filter expressions."""
 
@@ -141,38 +155,47 @@
 
 class And(CompoundFilterExpression):
     """Compound filter expression that is a logical conjunction."""
 
     def __repr__(self) -> str:
         return f'AND({", ".join([str(i) for i in self.expressions])})'
 
+    def get_lucene_filter(self):
+        return f'({" AND ".join([exp.get_lucene_filter() for exp in self.expressions])})'
+
     def does_match(self, document: dict) -> bool:
         return all((expression.matches(document) for expression in self.expressions))
 
 
 class Or(CompoundFilterExpression):
     """Compound filter expression that is a logical disjunction."""
 
     def __repr__(self) -> str:
         return f'OR({", ".join([str(i) for i in self.expressions])})'
 
+    def get_lucene_filter(self):
+        return f'({" OR ".join([exp.get_lucene_filter() for exp in self.expressions])})'
+
     def does_match(self, document: dict) -> bool:
         return any((expression.matches(document) for expression in self.expressions))
 
 
 class KeyValueBasedFilterExpression(FilterExpression):
     """Base class of filter expressions that match a certain value on a given key."""
 
     def __init__(self, key: List[str], expected_value: Any):
         self.key = key
         self._expected_value = expected_value
 
     def __repr__(self) -> str:
         return f"{self.as_dotted_string(self.key)}:{str(self._expected_value)}"
 
+    def get_lucene_filter(self):
+        return str(self)
+
     def does_match(self, document):
         raise NotImplementedError
 
 
 class StringFilterExpression(KeyValueBasedFilterExpression):
     """Key value filter expression that matches for a string."""
 
@@ -182,14 +205,17 @@
         if isinstance(value, list):
             return self._expected_value in value
         return str(value) == self._expected_value
 
     def __repr__(self) -> str:
         return f'{self.as_dotted_string(self.key)}:"{str(self._expected_value)}"'
 
+    def get_lucene_filter(self):
+        return str(self)
+
 
 class WildcardStringFilterExpression(KeyValueBasedFilterExpression):
     """Key value filter expression that matches for a string with wildcard support."""
 
     flags = 0
 
     wc = re.compile(r"((?:\\)*\*)")
@@ -326,24 +352,30 @@
     def does_match(self, document: dict) -> bool:
         value = self._get_value(self.key, document)
 
         if isinstance(value, list):
             return any(filter(self._matcher.match, value))
         return self._matcher.match(str(value)) is not None
 
+    def get_lucene_filter(self):
+        return str(self)
+
 
 class Exists(FilterExpression):
     """Filter expression that returns true if a given field exists."""
 
     def __init__(self, value: list):
         self.split_field = value
 
     def __repr__(self) -> str:
         return f'"{self.as_dotted_string(self.split_field)}"'
 
+    def get_lucene_filter(self):
+        return f"{self}: *"
+
     def does_match(self, document: dict) -> bool:
         if not self.split_field:
             return False
 
         try:
             current = document
             for sub_field in self.split_field:
```

### Comparing `logprep-6.3.0/logprep/filter/lucene_filter.py` & `logprep-6.4.0/logprep/filter/lucene_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Filter
 ======
 
 The filters are based on the Lucene query language, but contain some additional enhancements.
 It is possible to filter for keys and values in log messages.
 **Dot notation** is used to access subfields in log messages.
 A filter for :code:`{'field': {'subfield': 'value'}}` can be specified by
-:code:`field.subfield': 'value`.
+:code:`field.subfield': 'value'`.
 
 If a key without a value is given it is filtered for the existence of the key.
 The existence of a specific field can therefore be checked by a key without a value.
 The filter :code:`filter: field.subfield` would match for every value :code:`subfield` in
 :code:`{'field': {'subfield': 'value'}}`.
 The special key :code:`*` can be used to always match on any input.
 Thus, the filter :code:`filter: *` would match any input document.
@@ -28,15 +28,15 @@
     :caption: Example
 
     { "filter": "ip_address: 192.168.0.1" }
 
 It is possible to use filters with field names that contain white spaces or use special symbols
 of the Lucene syntax. However, this has to be escaped.
 The filter :code:`filter: 'field.a subfield(test): value'` must be escaped as
-:code:`filter: 'field.a\ subfield\(test\): value'`.
+:code:`filter: 'field.a\\\ subfield\(test\): value'`.
 Other references to this field do not require such escaping.
 This is *only* necessary for the filter.
 It is necessary to escape twice if the file is in the JSON format - once for
 the filter itself and once for JSON.
 
 Operators
 ---------
@@ -76,19 +76,20 @@
     :linenos:
     :caption: Example
 
     filter: 'ip_address: "192\.168\.0\..*"'
     regex_fields:
     - ip_address
 """
-# pylint: enable=anomalous-backslash-in-string
-from typing import List, Union, Optional
 import re
 from itertools import chain, zip_longest
 
+# pylint: enable=anomalous-backslash-in-string
+from typing import List, Union, Optional
+
 import luqum
 from luqum.parser import parser, ParseSyntaxError, IllegalCharacterError
 from luqum.tree import OrOperation, AndOperation, Group, FieldGroup, SearchField, Phrase, Word, Not
 
 from logprep.filter.expression.filter_expression import (
     Or,
     And,
```

### Comparing `logprep-6.3.0/logprep/framework/pipeline.py` & `logprep-6.4.0/logprep/framework/pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/framework/pipeline_manager.py` & `logprep-6.4.0/logprep/framework/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/framework/rule_tree/node.py` & `logprep-6.4.0/logprep/framework/rule_tree/node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/framework/rule_tree/rule_parser.py` & `logprep-6.4.0/logprep/framework/rule_tree/rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/framework/rule_tree/rule_tree.py` & `logprep-6.4.0/logprep/framework/rule_tree/rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/metrics/metric.py` & `logprep-6.4.0/logprep/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/metrics/metric_exposer.py` & `logprep-6.4.0/logprep/metrics/metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/metrics/metric_targets.py` & `logprep-6.4.0/logprep/metrics/metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/amides/detection.py` & `logprep-6.4.0/logprep/processor/amides/detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/amides/features.py` & `logprep-6.4.0/logprep/processor/amides/features.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/amides/normalize.py` & `logprep-6.4.0/logprep/processor/amides/normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/amides/processor.py` & `logprep-6.4.0/logprep/processor/amides/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/amides/rule.py` & `logprep-6.4.0/logprep/processor/amides/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/base/exceptions.py` & `logprep-6.4.0/logprep/processor/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/base/rule.py` & `logprep-6.4.0/logprep/processor/base/rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 .. WARNING::
    The dotted field notation is available in all processors, the use of indices to access list
    elements is though not available in the :code:`Clusterer`, :code:`Labeler` and the
    :code:`Pseudonymizer`.
 """
 
 import json
+from functools import cached_property
 from os.path import basename, splitext
 from typing import Dict, List, Optional, Set
 
 from attrs import define, field, validators
 from ruamel.yaml import YAML
 
 from logprep.filter.expression.filter_expression import FilterExpression
@@ -243,14 +244,18 @@
     def tests(self) -> list:
         return self._config.tests
 
     @property
     def failure_tags(self):
         return self._config.tag_on_failure
 
+    @cached_property
+    def lucene_filter(self):
+        return self.filter.get_lucene_filter()
+
     # pylint: enable=C0111
 
     @classmethod
     def create_rules_from_target(cls, path: str) -> list:
         """Create a rule from a file."""
         content = GetterFactory.from_string(path).get()
         try:
```

### Comparing `logprep-6.3.0/logprep/processor/calculator/fourFn.py` & `logprep-6.4.0/logprep/processor/calculator/fourFn.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/calculator/processor.py` & `logprep-6.4.0/logprep/processor/calculator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/calculator/rule.py` & `logprep-6.4.0/logprep/processor/calculator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/clusterer/processor.py` & `logprep-6.4.0/logprep/processor/clusterer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/clusterer/rule.py` & `logprep-6.4.0/logprep/processor/clusterer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/clusterer/signature_calculation/signature_phase.py` & `logprep-6.4.0/logprep/processor/clusterer/signature_calculation/signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/concatenator/processor.py` & `logprep-6.4.0/logprep/processor/concatenator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/concatenator/rule.py` & `logprep-6.4.0/logprep/processor/concatenator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/datetime_extractor/processor.py` & `logprep-6.4.0/logprep/processor/datetime_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/datetime_extractor/rule.py` & `logprep-6.4.0/logprep/processor/datetime_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/deleter/processor.py` & `logprep-6.4.0/logprep/processor/deleter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/deleter/rule.py` & `logprep-6.4.0/logprep/processor/deleter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/dissector/processor.py` & `logprep-6.4.0/logprep/processor/dissector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/dissector/rule.py` & `logprep-6.4.0/logprep/processor/dissector/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/domain_label_extractor/processor.py` & `logprep-6.4.0/logprep/processor/domain_label_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/domain_label_extractor/rule.py` & `logprep-6.4.0/logprep/processor/domain_label_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/domain_resolver/processor.py` & `logprep-6.4.0/logprep/processor/domain_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/domain_resolver/rule.py` & `logprep-6.4.0/logprep/processor/domain_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/dropper/processor.py` & `logprep-6.4.0/logprep/processor/dropper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/dropper/rule.py` & `logprep-6.4.0/logprep/processor/dropper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/field_manager/processor.py` & `logprep-6.4.0/logprep/processor/field_manager/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         self._write_to_single_target(args, extend_target_list, overwrite_target, rule)
 
     def _apply_mapping(self, event, rule, rule_args):
         source_fields, _, mapping, _, _ = rule_args
         source_fields, targets = list(zip(*mapping.items()))
         source_field_values = self._get_field_values(event, mapping.keys())
         self._handle_missing_fields(event, rule, source_fields, source_field_values)
+        if not any(source_field_values):
+            return
         source_field_values, targets = self._filter_missing_fields(source_field_values, targets)
         self._write_to_multiple_targets(event, targets, source_field_values, rule, rule_args)
         if rule.delete_source_fields:
             for dotted_field in source_fields:
                 pop_dotted_field_value(event, dotted_field)
 
     def _write_to_multiple_targets(self, event, target_fields, field_values, rule, rule_args):
```

### Comparing `logprep-6.3.0/logprep/processor/field_manager/rule.py` & `logprep-6.4.0/logprep/processor/field_manager/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/generic_adder/mysql_connector.py` & `logprep-6.4.0/logprep/processor/generic_adder/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/generic_adder/processor.py` & `logprep-6.4.0/logprep/processor/generic_adder/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/generic_adder/rule.py` & `logprep-6.4.0/logprep/processor/generic_adder/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/generic_resolver/processor.py` & `logprep-6.4.0/logprep/processor/generic_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/generic_resolver/rule.py` & `logprep-6.4.0/logprep/processor/generic_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/geoip_enricher/processor.py` & `logprep-6.4.0/logprep/processor/geoip_enricher/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/geoip_enricher/rule.py` & `logprep-6.4.0/logprep/processor/geoip_enricher/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/grokker/processor.py` & `logprep-6.4.0/logprep/processor/grokker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/grokker/rule.py` & `logprep-6.4.0/logprep/processor/grokker/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,15 +111,16 @@
         """A mapping from source fields to a grok pattern.
         Dotted field notation is possible in key and in the grok pattern.
         Additionally logstash field notation is possible in grok pattern.
         The value can be a list of search patterns or a single search pattern.
         Lists of search pattern will be checked in the order of the list until the first matching
         pattern.
         It is possible to use `oniguruma` regex pattern with or without grok patterns in the
-        patterns part.
+        patterns part. When defining an `oniguruma` there is a limitation of three nested
+        parentheses inside the pattern. Applying more nested parentheses is not possible.  
         Logstashs ecs conform grok patterns are used to resolve the here used grok patterns.
         """
         patterns: dict = field(
             validator=[
                 validators.instance_of(dict),
                 validators.deep_mapping(
                     key_validator=validators.instance_of(str),
@@ -140,22 +141,28 @@
 
     def _set_convert_actions(self):
         pass
 
     def set_mapping_actions(self, custom_patterns_dir: str = None) -> None:
         """sets the mapping actions"""
         custom_patterns_dir = "" if custom_patterns_dir is None else custom_patterns_dir
-        self.actions = {
-            dotted_field: Grok(
-                pattern,
-                custom_patterns=self._config.patterns,
-                custom_patterns_dir=custom_patterns_dir,
+
+        try:
+            self.actions = {
+                dotted_field: Grok(
+                    pattern,
+                    custom_patterns=self._config.patterns,
+                    custom_patterns_dir=custom_patterns_dir,
+                )
+                for dotted_field, pattern in self._config.mapping.items()
+            }
+        except re.error as error:
+            raise InvalidRuleDefinitionError(
+                f"The resolved grok pattern '{error.pattern}' is not valid"
             )
-            for dotted_field, pattern in self._config.mapping.items()
-        }
 
         # to ensure no string splitting is done during processing for target fields:
         for _, grok in self.actions.items():
             target_fields = list(grok.field_mapper.values())
             if not target_fields:
                 raise InvalidRuleDefinitionError("no target fields defined")
             for target_field in target_fields:
```

### Comparing `logprep-6.3.0/logprep/processor/hyperscan_resolver/processor.py` & `logprep-6.4.0/logprep/processor/hyperscan_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/hyperscan_resolver/rule.py` & `logprep-6.4.0/logprep/processor/hyperscan_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/ip_informer/processor.py` & `logprep-6.4.0/logprep/processor/ip_informer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/ip_informer/rule.py` & `logprep-6.4.0/logprep/processor/ip_informer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/key_checker/processor.py` & `logprep-6.4.0/logprep/processor/key_checker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/key_checker/rule.py` & `logprep-6.4.0/logprep/processor/key_checker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/labeler/labeling_schema.py` & `logprep-6.4.0/logprep/processor/labeler/labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/labeler/processor.py` & `logprep-6.4.0/logprep/processor/labeler/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/labeler/rule.py` & `logprep-6.4.0/logprep/processor/labeler/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/list_comparison/processor.py` & `logprep-6.4.0/logprep/processor/list_comparison/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/list_comparison/rule.py` & `logprep-6.4.0/logprep/processor/list_comparison/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/normalizer/processor.py` & `logprep-6.4.0/logprep/processor/normalizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/normalizer/rule.py` & `logprep-6.4.0/logprep/processor/normalizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/pre_detector/ip_alerter.py` & `logprep-6.4.0/logprep/processor/pre_detector/ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/pre_detector/processor.py` & `logprep-6.4.0/logprep/processor/pre_detector/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,13 +134,14 @@
             self._event["pre_detection_id"] = str(uuid4())
 
         detection_results.append(self._generate_detection_result(rule))
 
     def _generate_detection_result(self, rule: PreDetectorRule):
         detection_result = rule.detection_data
         detection_result["rule_filter"] = rule.filter_str
+        detection_result["lucene_filter"] = rule.lucene_filter
         detection_result["description"] = rule.description
         detection_result["pre_detection_id"] = self._event["pre_detection_id"]
         if "host" in self._event and "name" in self._event["host"]:
             detection_result["host"] = {"name": self._event["host"]["name"]}
 
         return detection_result
```

### Comparing `logprep-6.3.0/logprep/processor/pre_detector/rule.py` & `logprep-6.4.0/logprep/processor/pre_detector/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/processor_strategy.py` & `logprep-6.4.0/logprep/processor/processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/pseudonymizer/encrypter.py` & `logprep-6.4.0/logprep/processor/pseudonymizer/encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/pseudonymizer/processor.py` & `logprep-6.4.0/logprep/processor/pseudonymizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/pseudonymizer/rule.py` & `logprep-6.4.0/logprep/processor/pseudonymizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/requester/processor.py` & `logprep-6.4.0/logprep/processor/requester/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/requester/rule.py` & `logprep-6.4.0/logprep/processor/requester/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/selective_extractor/processor.py` & `logprep-6.4.0/logprep/processor/selective_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/selective_extractor/rule.py` & `logprep-6.4.0/logprep/processor/selective_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/string_splitter/processor.py` & `logprep-6.4.0/logprep/processor/string_splitter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/string_splitter/rule.py` & `logprep-6.4.0/logprep/processor/string_splitter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/template_replacer/processor.py` & `logprep-6.4.0/logprep/processor/template_replacer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/template_replacer/rule.py` & `logprep-6.4.0/logprep/processor/template_replacer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/timestamp_differ/processor.py` & `logprep-6.4.0/logprep/processor/timestamp_differ/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/timestamp_differ/rule.py` & `logprep-6.4.0/logprep/processor/timestamp_differ/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/timestamper/processor.py` & `logprep-6.4.0/logprep/processor/timestamper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/processor/timestamper/rule.py` & `logprep-6.4.0/logprep/processor/timestamper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/registry.py` & `logprep-6.4.0/logprep/registry.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/run_logprep.py` & `logprep-6.4.0/logprep/run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/runner.py` & `logprep-6.4.0/logprep/runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/aggregating_logger.py` & `logprep-6.4.0/logprep/util/aggregating_logger.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py` & `logprep-6.4.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/auto_rule_tester/auto_rule_tester.py` & `logprep-6.4.0/logprep/util/auto_rule_tester/auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py` & `logprep-6.4.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/cache.py` & `logprep-6.4.0/logprep/util/cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/configuration.py` & `logprep-6.4.0/logprep/util/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/decorators.py` & `logprep-6.4.0/logprep/util/decorators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/getter.py` & `logprep-6.4.0/logprep/util/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/grok.py` & `logprep-6.4.0/logprep/util/grok/grok.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,32 +19,36 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import re
+import string
 import sys
 from hashlib import md5
 from itertools import chain
 from pathlib import Path
+from re import error
 
+import numpy as np
 import pkg_resources
 from attrs import define, field, validators
 
 if sys.version_info.minor < 11:
     # because needed possessive quantifiers and atomic grouping
     # added to re module in python 3.11
     import regex as re  # pylint: disable=shadowed-import
 
 DEFAULT_PATTERNS_DIRS = [pkg_resources.resource_filename(__name__, "patterns/ecs-v1")]
 
 LOGSTASH_NOTATION = r"(([^\[\]\{\}\.:]*)?(\[[^\[\]\{\}\.:]*\])*)"
 GROK = r"%\{" + rf"([A-Z0-9_]*)(:({LOGSTASH_NOTATION}))?(:(int|float))?" + r"\}"
-ONIGURUMA = r"\(\?\<(.*)\>(.*)\)"
+ONIGURUMA = r"\(\?<([^()]*)>\(?(([^()]*|\(([^()]*|\([^()]*\))*\))*)\)?\)"
+NON_RESOLVED_ONIGURUMA = r"\(\?<[^md5].*>"
 INT_FLOAT = {"int": int, "float": float}
 
 
 @define(slots=True)
 class Grok:
     """Grok object"""
 
@@ -88,23 +92,23 @@
         if self.fullmatch:
             match_obj = [regex_pattern.fullmatch(text) for regex_pattern in self.regex_obj]
         else:
             match_obj = [regex_pattern.search(text) for regex_pattern in self.regex_obj]
 
         match_obj = [match for match in match_obj if match is not None]
         matches = [match.groupdict() for match in match_obj]
+        if not matches:
+            return {}
+        first_match = matches[0]
         if self.type_mapper:
-            matches = list(map(self._map_types, matches))
-        # deduplicate matches
-        matches = [dict(tup) for tup in {tuple(match.items()) for match in matches}]
-        return {
-            self.field_mapper[field_hash]: value
-            for match in matches
-            for field_hash, value in match.items()
-        }
+            for key, match in first_match.items():
+                type_ = INT_FLOAT.get(self.type_mapper.get(key))
+                if type_ is not None and match is not None:
+                    first_match[key] = type_(match)
+        return {self.field_mapper[field_hash]: value for field_hash, value in first_match.items()}
 
     def _map_types(self, matches):
         for key, match in matches.items():
             type_ = INT_FLOAT.get(self.type_mapper.get(key))
             if type_ is not None and match is not None:
                 matches[key] = type_(match)
         return matches
@@ -136,25 +140,33 @@
             raise ValueError(f"grok pattern '{name}' not found")
         if fields is None:
             return pattern.regex_str
         type_str = match.group(8)
         dundered_fields = self._to_dundered_field(fields)
         dotted_fields = self._to_dotted_field(dundered_fields)
         fields_hash = f"md5{md5(fields.encode()).hexdigest()}"  # nosemgrep
+        if fields_hash in self.field_mapper:
+            fields_hash += (
+                f"_{''.join(np.random.choice(list(string.ascii_letters), size=10, replace=True))}"
+            )
         if type_str is not None:
             self.type_mapper |= {fields_hash: type_str}
         self.field_mapper |= {fields_hash: dotted_fields}
         return rf"(?P<{fields_hash}>" rf"{pattern.regex_str})"
 
     def _resolve_oniguruma(self, match: re.Match) -> str:
         fields = match.group(1)
         pattern = match.group(2)
         dundered_fields = self._to_dundered_field(fields)
         dotted_fields = self._to_dotted_field(dundered_fields)
         fields_hash = f"md5{md5(fields.encode()).hexdigest()}"  # nosemgrep
+        if fields_hash in self.field_mapper:
+            fields_hash += (
+                f"_{''.join(np.random.choice(list(string.ascii_letters), size=10, replace=True))}"
+            )
         self.field_mapper |= {fields_hash: dotted_fields}
         return rf"(?P<{fields_hash}>" rf"{pattern})"
 
     def _load_search_pattern(self):
         py_regex_pattern = self.pattern
         if isinstance(py_regex_pattern, list):
             self.regex_obj = list(map(self._compile_pattern, py_regex_pattern))
@@ -172,14 +184,17 @@
         while re.search(Grok.grok_pattern, py_regex_pattern):
             py_regex_pattern = re.sub(
                 Grok.grok_pattern,
                 self._resolve_grok,
                 py_regex_pattern,
                 count=1,
             )
+        # Enforce error to be consistent between python versions 3.9 and 3.11
+        if re.match(NON_RESOLVED_ONIGURUMA, py_regex_pattern):
+            raise error("Not valid oniguruma pattern", pattern=py_regex_pattern)
         return re.compile(py_regex_pattern)
 
 
 def _reload_patterns(patterns_dirs):
     """ """
     patterns_dirs = [Path(directory) for directory in patterns_dirs]
     patterns_dirs += chain(*[list(directory.rglob("**/*")) for directory in patterns_dirs])
```

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/aws` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bacula` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bind` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/bind`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bro` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/exim` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/firewalls` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/grok-patterns` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/haproxy` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/httpd` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/java` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/java`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/junos` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/linux-syslog` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/mongodb` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/nagios` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/rails` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/squid` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/squid`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/zeek` & `logprep-6.4.0/logprep/util/grok/patterns/ecs-v1/zeek`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/aws` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/bacula` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/bro` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/exim` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/firewalls` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/grok-patterns` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/haproxy` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/httpd` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/java` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/java`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/junos` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/linux-syslog` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/mongodb` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/nagios` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok/patterns/legacy/rails` & `logprep-6.4.0/logprep/util/grok/patterns/legacy/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/grok_pattern_loader.py` & `logprep-6.4.0/logprep/util/grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/hasher.py` & `logprep-6.4.0/logprep/util/hasher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/helper.py` & `logprep-6.4.0/logprep/util/helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/json_handling.py` & `logprep-6.4.0/logprep/util/json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/log_aggregator.py` & `logprep-6.4.0/logprep/util/log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/multiprocessing_log_handler.py` & `logprep-6.4.0/logprep/util/multiprocessing_log_handler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/pipeline_profiler.py` & `logprep-6.4.0/logprep/util/pipeline_profiler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/pre_detector_rule_matching_tester.py` & `logprep-6.4.0/logprep/util/pre_detector_rule_matching_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/processor_generator.py` & `logprep-6.4.0/logprep/util/processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/prometheus_exporter.py` & `logprep-6.4.0/logprep/util/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/rule_dry_runner.py` & `logprep-6.4.0/logprep/util/rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/schema_and_rule_checker.py` & `logprep-6.4.0/logprep/util/schema_and_rule_checker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/time.py` & `logprep-6.4.0/logprep/util/time.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/time_measurement.py` & `logprep-6.4.0/logprep/util/time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep/util/validators.py` & `logprep-6.4.0/logprep/util/validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/logprep.egg-info/PKG-INFO` & `logprep-6.4.0/logprep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.3.0
+Version: 6.4.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.3.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.4.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.3.0/logprep.egg-info/SOURCES.txt` & `logprep-6.4.0/logprep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/setup.py` & `logprep-6.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_amides.py` & `logprep-6.4.0/tests/acceptance/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_config_refresh.py` & `logprep-6.4.0/tests/acceptance/test_config_refresh.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_file_input.py` & `logprep-6.4.0/tests/acceptance/test_file_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_full_configuration.py` & `logprep-6.4.0/tests/acceptance/test_full_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_http_input.py` & `logprep-6.4.0/tests/acceptance/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_multiple_outputs.py` & `logprep-6.4.0/tests/acceptance/test_multiple_outputs.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_pre_detection.py` & `logprep-6.4.0/tests/acceptance/test_pre_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,36 +35,36 @@
             {"@timestamp":"2019-08-02T09:46:20.000Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"event":{"kind":"event","code":6005,"created":"2019-08-02T09:55:11.996Z"},"ecs":{"version":"1.0.0"},"host":{"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1","architecture":"x86","os":{"version":"6.1","family":"windows","name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows"},"name":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"},"log":{"level":"information"},"message":"The Event log service was started.","winlog":{"provider_name":"EventLog","task":"","channel":"System","event_data":{"Binary":"E30708000500020009002E00140057010000000000000000"},"event_id":6005,"computer_name":"abcdefg1234","keywords":["Classic"],"record_id":11571,"api":"wineventlog"}},
             {"@timestamp":"2019-08-02T09:46:20.000Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"event":{"kind":"event","code":6005,"created":"2019-08-02T09:55:11.996Z"},"ecs":{"version":"1.0.0"},"host":{"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1","architecture":"x86","os":{"version":"6.1","family":"windows","name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows"},"name":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"},"log":{"level":"information"},"message":"The Event log service was started.","winlog":{"provider_name":"EventLog","task":"","channel":"System","event_data":{"Binary":"E30708000500020009002E00140057010000000000000000"},"event_id":6005,"computer_name":"abcdefg1234","keywords":["Classic"],"record_id":11571,"api":"wineventlog"}},
             None
         ),
         (
             {"@timestamp":"2019-07-30T14:38:16.352Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"event":{"code":7036,"created":"2019-08-02T09:55:11.996Z","kind":"event"},"agent":{"version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0"},"ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","hostname":"CLIENT1","architecture":"x86","os":{"name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4"},"log":{"level":"information"},"message":"The Software Protection service entered the stopped state.","winlog":{"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","event_id":1234,"task":"","api":"wineventlog","event_data":{"Binary":"7300700070007300760063002F0031000000","param1":"Software Protection","param2":"stopped"},"keywords":["Classic"],"provider_name":"Service Control Manager","record_id":11580,"channel":"System","computer_name":"abcdefg1234","process":{"thread":{"id":2808},"pid":436}}},
             {"@timestamp":"2019-07-30T14:38:16.352Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"event":{"code":7036,"created":"2019-08-02T09:55:11.996Z","kind":"event"},"agent":{"version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0"},"ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","hostname":"CLIENT1","architecture":"x86","os":{"name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4"},"log":{"level":"information"},"message":"The Software Protection service entered the stopped state.","winlog":{"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","event_id":1234,"task":"","api":"wineventlog","event_data":{"Binary":"7300700070007300760063002F0031000000","param1":"Software Protection","param2":"stopped"},"keywords":["Classic"],"provider_name":"Service Control Manager","record_id":11580,"channel":"System","computer_name":"abcdefg1234","process":{"thread":{"id":2808},"pid":436}}},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "1cf39644-a632-4c42-a7b4-2896c4efffb5", "host": {"name": "CLIENT1"}, "@timestamp": "2019-07-30T14:38:16.352Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', 'lucene_filter': 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "1cf39644-a632-4c42-a7b4-2896c4efffb5", "host": {"name": "CLIENT1"}, "@timestamp": "2019-07-30T14:38:16.352Z"}}]
         ),
         (
             {"@timestamp":"2019-08-02T09:46:41.906Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"host":{"name":"CLIENT1","os":{"name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1","architecture":"x86"},"agent":{"hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9"},"ecs":{"version":"1.0.0"},"winlog":{"channel":"System","provider_name":"Service Control Manager","record_id":11627,"event_id":1234,"api":"wineventlog","keywords":["Classic"],"computer_name":"abcdefg1234","process":{"pid":440,"thread":{"id":524}},"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","event_data":{"param1":"Wazuh","param2":"running","Binary":"4F0073007300650063005300760063002F0034000000"},"task":""},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:11.998Z"},"log":{"level":"information"},"message":"The Wazuh service entered the running state."},
             {"@timestamp":"2019-08-02T09:46:41.906Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"host":{"name":"CLIENT1","os":{"name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1","architecture":"x86"},"agent":{"hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9"},"ecs":{"version":"1.0.0"},"winlog":{"channel":"System","provider_name":"Service Control Manager","record_id":11627,"event_id":1234,"api":"wineventlog","keywords":["Classic"],"computer_name":"abcdefg1234","process":{"pid":440,"thread":{"id":524}},"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","event_data":{"param1":"Wazuh","param2":"running","Binary":"4F0073007300650063005300760063002F0034000000"},"task":""},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:11.998Z"},"log":{"level":"information"},"message":"The Wazuh service entered the running state."},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "08d1aa6f-f508-464e-a13d-0b5da46b5bcc", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:46:41.906Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', 'lucene_filter': 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "08d1aa6f-f508-464e-a13d-0b5da46b5bcc", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:46:41.906Z"}}]
         ),
         (
             {"@timestamp":"2019-08-02T09:46:54.583Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"provider_name":"Service Control Manager","computer_name":"abcdefg1234","provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","process":{"pid":440,"thread":{"id":1792}},"event_data":{"param1":"Portable Device Enumerator Service","param2":"running","Binary":"57005000440042007500730045006E0075006D002F0034000000"},"channel":"System","record_id":11638,"task":"","api":"wineventlog","event_id":1234,"keywords":["Classic"]},"event":{"code":7036,"created":"2019-08-02T09:55:11.999Z","kind":"event"},"agent":{"ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat"},"ecs":{"version":"1.0.0"},"host":{"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","name":"CLIENT1","hostname":"CLIENT1","architecture":"x86","os":{"platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0"}},"log":{"level":"information"},"message":"The Portable Device Enumerator Service service entered the running state."},
             {"@timestamp":"2019-08-02T09:46:54.583Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"provider_name":"Service Control Manager","computer_name":"abcdefg1234","provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","process":{"pid":440,"thread":{"id":1792}},"event_data":{"param1":"Portable Device Enumerator Service","param2":"running","Binary":"57005000440042007500730045006E0075006D002F0034000000"},"channel":"System","record_id":11638,"task":"","api":"wineventlog","event_id":1234,"keywords":["Classic"]},"event":{"code":7036,"created":"2019-08-02T09:55:11.999Z","kind":"event"},"agent":{"ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat"},"ecs":{"version":"1.0.0"},"host":{"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","name":"CLIENT1","hostname":"CLIENT1","architecture":"x86","os":{"platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0"}},"log":{"level":"information"},"message":"The Portable Device Enumerator Service service entered the running state."},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "06d12743-01f0-4793-8a31-3815cfa31fc3", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:46:54.583Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', 'lucene_filter': 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "06d12743-01f0-4793-8a31-3815cfa31fc3", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:46:54.583Z"}}]
         ),
         (
             {"@timestamp":"2019-08-02T09:54:57.125Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"computer_name":"abcdefg1234","event_id":123,"record_id":11714,"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","channel":"System","task":"","api":"wineventlog","event_data":{"param2":"running","Binary":"41007500640069006F007300720076002F0034000000","param1":"Windows Audio"},"provider_name":"Service Control Manager 2","keywords":["Classic"],"process":{"pid":440,"thread":{"id":528}}},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:12.091Z"},"log":{"level":"information"},"message":"The Windows Audio service entered the running state.","ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","architecture":"x86","os":{"kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"}},
             {"@timestamp":"2019-08-02T09:54:57.125Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"computer_name":"abcdefg1234","event_id":123,"record_id":11714,"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","channel":"System","task":"","api":"wineventlog","event_data":{"param2":"running","Binary":"41007500640069006F007300720076002F0034000000","param1":"Windows Audio"},"provider_name":"Service Control Manager 2","keywords":["Classic"],"process":{"pid":440,"thread":{"id":528}}},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:12.091Z"},"log":{"level":"information"},"message":"The Windows Audio service entered the running state.","ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","architecture":"x86","os":{"kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"}},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_TWO_ID", "title": "RULE_TWO", "severity": "critical", "mitre": ["mitre2", "mitre3"], "case_condition": "directly", "rule_filter": 'winlog.event_id:"123"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_TWO_ID", "title": "RULE_TWO", "severity": "critical", "mitre": ["mitre2", "mitre3"], "case_condition": "directly", "rule_filter": 'winlog.event_id:"123"', 'lucene_filter': 'winlog.event_id:"123"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}}]
         ),
         (
             {"@timestamp":"2019-08-02T09:54:57.125Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"computer_name":"abcdefg1234","event_id":123,"record_id":11714,"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","channel":"System","task":"","api":"wineventlog","event_data":{"param2":"running","Binary":"41007500640069006F007300720076002F0034000000","param1":"Windows Audio"},"provider_name":"Service Control Manager","keywords":["Classic"],"process":{"pid":440,"thread":{"id":528}}},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:12.091Z"},"log":{"level":"information"},"message":"The Windows Audio service entered the running state.","ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","architecture":"x86","os":{"kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"}},
             {"@timestamp":"2019-08-02T09:54:57.125Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"computer_name":"abcdefg1234","event_id":123,"record_id":11714,"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","channel":"System","task":"","api":"wineventlog","event_data":{"param2":"running","Binary":"41007500640069006F007300720076002F0034000000","param1":"Windows Audio"},"provider_name":"Service Control Manager","keywords":["Classic"],"process":{"pid":440,"thread":{"id":528}}},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:12.091Z"},"log":{"level":"information"},"message":"The Windows Audio service entered the running state.","ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","architecture":"x86","os":{"kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"}},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}},
-             {"pre_detector_topic": {"description": "", "id": "RULE_TWO_ID", "title": "RULE_TWO", "severity": "critical", "mitre": ["mitre2", "mitre3"], "case_condition": "directly", "rule_filter": 'winlog.event_id:"123"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', 'lucene_filter': 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}},
+             {"pre_detector_topic": {"description": "", "id": "RULE_TWO_ID", "title": "RULE_TWO", "severity": "critical", "mitre": ["mitre2", "mitre3"], "case_condition": "directly", "rule_filter": 'winlog.event_id:"123"', 'lucene_filter': 'winlog.event_id:"123"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}}]
         ),
     ],
 )
 # fmt: on
 def test_events_pre_detected_correctly(
     tmp_path, input_event, expected_output_event, expected_extra_output
 ):
```

### Comparing `logprep-6.3.0/tests/acceptance/test_preprocessing.py` & `logprep-6.4.0/tests/acceptance/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py` & `logprep-6.4.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_wineventlog_normalization.py` & `logprep-6.4.0/tests/acceptance/test_wineventlog_normalization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_wineventlog_processing.py` & `logprep-6.4.0/tests/acceptance/test_wineventlog_processing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/test_wineventlog_pseudonymization.py` & `logprep-6.4.0/tests/acceptance/test_wineventlog_pseudonymization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/acceptance/util.py` & `logprep-6.4.0/tests/acceptance/util.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/ci/runner-image/scripts/compare_json.py` & `logprep-6.4.0/tests/ci/runner-image/scripts/compare_json.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/testdata/ConfigurationForTest.py` & `logprep-6.4.0/tests/testdata/ConfigurationForTest.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/testdata/FilledTempFile.py` & `logprep-6.4.0/tests/testdata/FilledTempFile.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/testdata/metadata.py` & `logprep-6.4.0/tests/testdata/metadata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/testdata/ruledata.py` & `logprep-6.4.0/tests/testdata/ruledata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/testdata/unit/clusterer/test_data.py` & `logprep-6.4.0/tests/testdata/unit/clusterer/test_data.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/component/base.py` & `logprep-6.4.0/tests/unit/component/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/base.py` & `logprep-6.4.0/tests/unit/connector/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_confluent_kafka_common.py` & `logprep-6.4.0/tests/unit/connector/test_confluent_kafka_common.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_confluent_kafka_input.py` & `logprep-6.4.0/tests/unit/connector/test_confluent_kafka_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_confluent_kafka_output.py` & `logprep-6.4.0/tests/unit/connector/test_confluent_kafka_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_console_output.py` & `logprep-6.4.0/tests/unit/connector/test_console_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_dummy_input.py` & `logprep-6.4.0/tests/unit/connector/test_dummy_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_dummy_output.py` & `logprep-6.4.0/tests/unit/connector/test_dummy_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_elasticsearch_output.py` & `logprep-6.4.0/tests/unit/connector/test_elasticsearch_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_file_input_default_config.py` & `logprep-6.4.0/tests/unit/connector/test_file_input_default_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_file_input_not_tailing_config.py` & `logprep-6.4.0/tests/unit/connector/test_file_input_not_tailing_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_file_input_start_at_end_config.py` & `logprep-6.4.0/tests/unit/connector/test_file_input_start_at_end_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_http_input.py` & `logprep-6.4.0/tests/unit/connector/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_json_input.py` & `logprep-6.4.0/tests/unit/connector/test_json_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_jsonl_input.py` & `logprep-6.4.0/tests/unit/connector/test_jsonl_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_jsonl_output.py` & `logprep-6.4.0/tests/unit/connector/test_jsonl_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_opensearch_output.py` & `logprep-6.4.0/tests/unit/connector/test_opensearch_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/connector/test_s3_output.py` & `logprep-6.4.0/tests/unit/connector/test_s3_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/exceptions/processor/test_processing_warning.py` & `logprep-6.4.0/tests/unit/exceptions/processor/test_processing_warning.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/filter/test_filter_expression.py` & `logprep-6.4.0/tests/unit/filter/test_filter_expression.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     FloatRangeFilterExpression,
     FloatFilterExpression,
     Always,
     WildcardStringFilterExpression,
     SigmaFilterExpression,
     Exists,
 )
+from logprep.filter.lucene_filter import LuceneFilter
 
 
 class TestFilterExpression:
     def test_get_value_fails_for_missing_key(self):
         with pytest.raises(KeyDoesNotExistError):
             FilterExpression._get_value(["some", "key"], {})
 
@@ -517,7 +518,62 @@
             (r'te\\"st', r'^te\\\\"st$'),
             (r'te\\"st"', r'^te\\\\"st"$'),
         ],
     )
     def test_escaped_expected(self, filter_expression, expected_expression):
         _filter = SigmaFilterExpression(["key1", "key2"], filter_expression)
         assert _filter.escaped_expected == expected_expression
+
+
+class TestLuceneRepresentation:
+    @pytest.mark.parametrize(
+        "logprep_filter_language, special_fields, expected_lucene_filter_query",
+        [
+            ("exist_field", None, '"exist_field": *'),
+            ("key: value", None, 'key:"value"'),
+            ("dotted.key: value", None, 'dotted.key:"value"'),
+            ("*", None, "*"),
+            ("NOT key", None, 'NOT ("key": *)'),
+            ("NOT key: value", None, 'NOT (key:"value")'),
+            ("key: value1 AND keyy: value2", None, '(key:"value1" AND keyy:"value2")'),
+            (
+                "key: value1 AND keyy: value2 AND keyyy: value3",
+                None,
+                '(key:"value1" AND keyy:"value2" AND keyyy:"value3")',
+            ),
+            ("key: value1 OR key: value2", None, '(key:"value1" OR key:"value2")'),
+            (
+                "key: value1 AND keyy: value2 OR keyyy: value3",
+                None,
+                '((key:"value1" AND keyy:"value2") OR keyyy:"value3")',
+            ),
+            (
+                "key: value1 AND (keyy: value2 OR keyyy: value3)",
+                None,
+                '(key:"value1" AND (keyy:"value2" OR keyyy:"value3"))',
+            ),
+            (
+                "key: value1 AND (keyy: value2 OR NOT keyyy: value3)",
+                None,
+                '(key:"value1" AND (keyy:"value2" OR NOT (keyyy:"value3")))',
+            ),
+            ("key: val*", None, 'key:"val*"'),
+            ("key: 1", None, 'key:"1"'),
+            ("key: 1.0", None, 'key:"1.0"'),
+            (r"key: field\[\d\].*", {"regex_fields": ["key"]}, r"key:r/^field\[\d\].*$/"),
+            (
+                r"nonRegexKey: something AND key: field\[\d\].*",
+                {"regex_fields": ["key"]},
+                r'(nonRegexKey:"something" AND key:r/^field\[\d\].*$/)',
+            ),
+        ],
+    )
+    def test_convert_filter_to_best_closest_lucene_language(
+        self, logprep_filter_language, special_fields, expected_lucene_filter_query
+    ):
+        filter_expression = LuceneFilter.create(
+            logprep_filter_language, special_fields=special_fields
+        )
+        lucene_filter = filter_expression.get_lucene_filter()
+        assert (
+            lucene_filter == expected_lucene_filter_query
+        ), f"Expected: '{expected_lucene_filter_query}', but got: '{lucene_filter}'"
```

### Comparing `logprep-6.3.0/tests/unit/filter/test_lucene_filter.py` & `logprep-6.4.0/tests/unit/filter/test_lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/framework/rule_tree/test_node.py` & `logprep-6.4.0/tests/unit/framework/rule_tree/test_node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/framework/rule_tree/test_rule_parser.py` & `logprep-6.4.0/tests/unit/framework/rule_tree/test_rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/framework/rule_tree/test_rule_tree.py` & `logprep-6.4.0/tests/unit/framework/rule_tree/test_rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/framework/test_pipeline.py` & `logprep-6.4.0/tests/unit/framework/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/framework/test_pipeline_manager.py` & `logprep-6.4.0/tests/unit/framework/test_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/metrics/test_metric_exposer.py` & `logprep-6.4.0/tests/unit/metrics/test_metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/metrics/test_metric_targets.py` & `logprep-6.4.0/tests/unit/metrics/test_metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/metrics/test_metrics.py` & `logprep-6.4.0/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/amides/test_amides.py` & `logprep-6.4.0/tests/unit/processor/amides/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/amides/test_amides_rule.py` & `logprep-6.4.0/tests/unit/processor/amides/test_amides_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/amides/test_detection.py` & `logprep-6.4.0/tests/unit/processor/amides/test_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/amides/test_normalize.py` & `logprep-6.4.0/tests/unit/processor/amides/test_normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/amides/test_tokenizer.py` & `logprep-6.4.0/tests/unit/processor/amides/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/base.py` & `logprep-6.4.0/tests/unit/processor/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/calculator/test_calculator.py` & `logprep-6.4.0/tests/unit/processor/calculator/test_calculator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/calculator/test_calculator_rule.py` & `logprep-6.4.0/tests/unit/processor/calculator/test_calculator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer.py` & `logprep-6.4.0/tests/unit/processor/clusterer/test_clusterer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer_rule.py` & `logprep-6.4.0/tests/unit/processor/clusterer/test_clusterer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py` & `logprep-6.4.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/concatenator/test_concatenator.py` & `logprep-6.4.0/tests/unit/processor/concatenator/test_concatenator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/concatenator/test_concatenator_rule.py` & `logprep-6.4.0/tests/unit/processor/concatenator/test_concatenator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py` & `logprep-6.4.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py` & `logprep-6.4.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/deleter/test_deleter.py` & `logprep-6.4.0/tests/unit/processor/deleter/test_deleter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/deleter/test_deleter_rule.py` & `logprep-6.4.0/tests/unit/processor/deleter/test_deleter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/dissector/test_dissector.py` & `logprep-6.4.0/tests/unit/processor/dissector/test_dissector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/dissector/test_dissector_rule.py` & `logprep-6.4.0/tests/unit/processor/dissector/test_dissector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py` & `logprep-6.4.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py` & `logprep-6.4.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/domain_resolver/test_domain_resolver.py` & `logprep-6.4.0/tests/unit/processor/domain_resolver/test_domain_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py` & `logprep-6.4.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/dropper/test_dropper.py` & `logprep-6.4.0/tests/unit/processor/dropper/test_dropper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/dropper/test_dropper_rule.py` & `logprep-6.4.0/tests/unit/processor/dropper/test_dropper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/field_manager/test_field_manager.py` & `logprep-6.4.0/tests/unit/processor/field_manager/test_field_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,14 +467,26 @@
             "one": 1,
             "two": 2,
             "three": "exists",
             "tags": ["_field_manager_failure"],
         },
         ".*FieldExistsWarning.*",
     ),
+    (
+        "tries to move multiple fields to multiple target fields but none exists",
+        {
+            "filter": "no-mapped-field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+            },
+        },
+        {"no-mapped-field": "exists"},
+        {"no-mapped-field": "exists", "tags": ["_field_manager_missing_field_warning"]},
+        ".*ProcessingWarning.*",
+    ),
 ]  # testcase, rule, event, expected, error
 
 
 class TestFieldManager(BaseProcessorTestCase):
     CONFIG: dict = {
         "type": "field_manager",
         "specific_rules": ["tests/testdata/unit/field_manager/specific_rules"],
```

### Comparing `logprep-6.3.0/tests/unit/processor/field_manager/test_field_manager_rule.py` & `logprep-6.4.0/tests/unit/processor/field_manager/test_field_manager_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/generic_adder/test_generic_adder.py` & `logprep-6.4.0/tests/unit/processor/generic_adder/test_generic_adder.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py` & `logprep-6.4.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/generic_resolver/test_generic_resolver.py` & `logprep-6.4.0/tests/unit/processor/generic_resolver/test_generic_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py` & `logprep-6.4.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py` & `logprep-6.4.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py` & `logprep-6.4.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/grokker/test_grok.py` & `logprep-6.4.0/tests/unit/processor/grokker/test_grok.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/grokker/test_grokker.py` & `logprep-6.4.0/tests/unit/processor/grokker/test_grokker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
+# pylint: disable=line-too-long
 import logging
 import re
 from copy import deepcopy
 from unittest import mock
 
 import pytest
 
@@ -108,15 +109,15 @@
         {
             "filter": "winlog.event_id: 123456789",
             "grokker": {
                 "mapping": {
                     "winlog.event_data.normalize me!": [
                         "%{IP:some_ip_1} %{NUMBER:port_1:int} foo",
                         "%{IP:some_ip_2} %{NUMBER:port_2:int} bar",
-                        "%{IP:some_ip_2} %{NUMBER:port_2:int} bar",
+                        "%{IP:some_ip_3} %{NUMBER:port_3:int} bar",
                     ]
                 }
             },
         },
         {
             "winlog": {
                 "api": "wineventlog",
@@ -238,14 +239,51 @@
         {
             "filter": "message",
             "grokker": {"mapping": {"message": "this is the (?<userfield>[A-Za-z0-9]+)"}},
         },
         {"message": "this is the MyUser586"},
         {"message": "this is the MyUser586", "userfield": "MyUser586"},
     ),
+    (
+        "oniguruma with nested parentheses (3 levels supported)",
+        {
+            "filter": "message",
+            "grokker": {
+                "mapping": {
+                    "message": "^(?<timestamp>%{DAY}%{SPACE}%{MONTH}%{SPACE}%{MONTHDAY}%{SPACE}%{TIME}%{SPACE}%{YEAR})%{SPACE}%{GREEDYDATA:[remains]}$",
+                    "remains": "(?<action>(SEND%{SPACE}INFO)%{SPACE}(?<info>BAL)%{GREEDYDATA:rest}",
+                }
+            },
+        },
+        {"message": "Wed Dec 7 13:14:13 2005 SEND INFO BAL/4"},
+        {
+            "message": "Wed Dec 7 13:14:13 2005 SEND INFO BAL/4",
+            "timestamp": "Wed Dec 7 13:14:13 2005",
+            "action": "SEND INFO",
+            "info": "BAL",
+            "rest": "/4",
+            "remains": "SEND INFO BAL/4",
+        },
+    ),
+    (
+        "two oniguruma with same target names, applies only the last target",
+        {
+            "filter": "message",
+            "grokker": {
+                "mapping": {
+                    "message": "^(?<action>%{NUMBER})%{SPACE}(?<action>%{NUMBER})%{SPACE}(?<action>%{NUMBER})%{SPACE}(?<action>%{NUMBER})$",
+                }
+            },
+        },
+        {"message": "13 37 21 42"},
+        {
+            "message": "13 37 21 42",
+            "action": "42",
+        },
+    ),
 ]
 
 failure_test_cases = [
     (
         "only field does not exist",
         {"filter": "message", "grokker": {"mapping": {"unknown": "this is the %{USER:userfield}"}}},
         {"message": "this is the MyUser586"},
```

### Comparing `logprep-6.3.0/tests/unit/processor/grokker/test_grokker_rule.py` & `logprep-6.4.0/tests/unit/processor/grokker/test_grokker_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,14 +208,38 @@
                 {
                     "filter": "message",
                     "grokker": {"mapping": {"message": "(?P<groupname>)"}},
                 },
                 ValueError,
                 "must match regex",
             ),
+            (
+                {
+                    "filter": "message",
+                    "grokker": {
+                        "mapping": {
+                            "message": "(?<group>(TOO(%{SPACE}(M(AN)Y)%{SPACE})PARENTHESES))"
+                        }
+                    },
+                },
+                InvalidRuleDefinitionError,
+                r"The resolved grok pattern.*is not valid",
+            ),
+            (
+                {
+                    "filter": "message",
+                    "grokker": {
+                        "mapping": {
+                            "message": "(?<group>(NOT-TOO(%{SPACE}(MANY)%{SPACE})PARENTHESES))"
+                        }
+                    },
+                },
+                None,
+                None,
+            ),
         ],
     )
     def test_create_from_dict_validates_config(self, rule, error, message):
         if error:
             with pytest.raises(error, match=message):
                 rule = GrokkerRule._create_from_dict(rule)
                 rule.set_mapping_actions()
```

### Comparing `logprep-6.3.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py` & `logprep-6.4.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py` & `logprep-6.4.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/ip_informer/test_ip_informer.py` & `logprep-6.4.0/tests/unit/processor/ip_informer/test_ip_informer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py` & `logprep-6.4.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/labeler/test_labeler.py` & `logprep-6.4.0/tests/unit/processor/labeler/test_labeler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/labeler/test_labeler_rule.py` & `logprep-6.4.0/tests/unit/processor/labeler/test_labeler_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/labeler/test_labeling_schema.py` & `logprep-6.4.0/tests/unit/processor/labeler/test_labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/list_comparison/test_list_comparison.py` & `logprep-6.4.0/tests/unit/processor/list_comparison/test_list_comparison.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py` & `logprep-6.4.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/normalizer/test_normalizer.py` & `logprep-6.4.0/tests/unit/processor/normalizer/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/normalizer/test_normalizer_rule.py` & `logprep-6.4.0/tests/unit/processor/normalizer/test_normalizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/pre_detector/test_ip_alerter.py` & `logprep-6.4.0/tests/unit/processor/pre_detector/test_ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/pre_detector/test_pre_detector.py` & `logprep-6.4.0/tests/unit/processor/pre_detector/test_pre_detector.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                     "id": "RULE_ONE_ID",
                     "title": "RULE_ONE",
                     "severity": "critical",
                     "mitre": ["attack.test1", "attack.test2"],
                     "case_condition": "directly",
                     "description": "Test rule one",
                     "rule_filter": 'AND(winlog.event_id:"123", winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
+                    "lucene_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
@@ -54,14 +55,15 @@
                     "title": "RULE_ONE",
                     "severity": "critical",
                     "mitre": ["attack.test1", "attack.test2"],
                     "case_condition": "directly",
                     "host": {"name": "Test hostname"},
                     "description": "Test rule one",
                     "rule_filter": 'AND(winlog.event_id:"123", winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
+                    "lucene_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
@@ -77,14 +79,15 @@
                     "id": "RULE_ONE_ID",
                     "title": "RULE_ONE",
                     "severity": "critical",
                     "mitre": ["attack.test1", "attack.test2"],
                     "case_condition": "directly",
                     "description": "Test rule one",
                     "rule_filter": 'AND(winlog.event_id:"123", winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
+                    "lucene_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
 
         document["pre_detection_id"] = "11fdfc1f-8e00-476e-b88f-753d92af989c"
         detection_results = self.object.process(document)
@@ -105,14 +108,16 @@
                     "mitre": [],
                     "case_condition": "directly",
                     "description": "Test rule two",
                     "rule_filter": 'AND(tags:"test", '
                     'process.program:"test", '
                     'OR(message:"test1*xyz", '
                     'message:"test2*xyz"))',
+                    "lucene_filter": '(tags:"test" AND process.program:"test" AND '
+                    '(message:"test1*xyz" OR message:"test2*xyz"))',
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
@@ -131,14 +136,16 @@
                     "mitre": [],
                     "case_condition": "directly",
                     "description": "Test rule three",
                     "rule_filter": 'AND(tags:"test2", '
                     'process.program:"test", '
                     'OR(message:"test1*xyz", '
                     'message:"test2?xyz"))',
+                    "lucene_filter": '(tags:"test2" AND process.program:"test" AND '
+                    '(message:"test1*xyz" OR message:"test2?xyz"))',
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
@@ -152,23 +159,25 @@
             [
                 {
                     "case_condition": "directly",
                     "id": "RULE_ONE_ID",
                     "mitre": ["attack.test1", "attack.test2"],
                     "description": "Test two rules one",
                     "rule_filter": '"first_match"',
+                    "lucene_filter": '"first_match": *',
                     "severity": "critical",
                     "title": "RULE_ONE",
                 },
                 {
                     "case_condition": "directly",
                     "id": "RULE_TWO_ID",
                     "mitre": ["attack.test2", "attack.test4"],
                     "description": "Test two rules two",
                     "rule_filter": '"second_match"',
+                    "lucene_filter": '"second_match": *',
                     "severity": "suspicious",
                     "title": "RULE_TWO",
                 },
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
@@ -252,14 +261,15 @@
                     "id": "RULE_TWO_ID",
                     "title": "RULE_TWO",
                     "severity": "critical",
                     "mitre": [],
                     "case_condition": "directly",
                     "description": "Test rule two",
                     "rule_filter": 'AND(tags:"test", process.program:"test", OR(message:"test1*xyz", message:"test2*xyz"))',  # pylint: disable=line-too-long
+                    "lucene_filter": '(tags:"test" AND process.program:"test" AND (message:"test1*xyz" OR message:"test2*xyz"))',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
@@ -275,14 +285,15 @@
                     "id": "RULE_TWO_ID",
                     "title": "RULE_TWO",
                     "severity": "critical",
                     "mitre": [],
                     "case_condition": "directly",
                     "description": "Test rule two",
                     "rule_filter": 'AND(tags:"test", process.program:"test", OR(message:"test1*xyz", message:"test2*xyz"))',  # pylint: disable=line-too-long
+                    "lucene_filter": '(tags:"test" AND process.program:"test" AND (message:"test1*xyz" OR message:"test2*xyz"))',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
```

### Comparing `logprep-6.3.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py` & `logprep-6.4.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/pseudonymizer/test_encrypter.py` & `logprep-6.4.0/tests/unit/processor/pseudonymizer/test_encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py` & `logprep-6.4.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py` & `logprep-6.4.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/requester/test_requester.py` & `logprep-6.4.0/tests/unit/processor/requester/test_requester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/requester/test_requester_rule.py` & `logprep-6.4.0/tests/unit/processor/requester/test_requester_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/selective_extractor/test_selective_extractor.py` & `logprep-6.4.0/tests/unit/processor/selective_extractor/test_selective_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py` & `logprep-6.4.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/string_splitter/test_string_splitter.py` & `logprep-6.4.0/tests/unit/processor/string_splitter/test_string_splitter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py` & `logprep-6.4.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/template_replacer/test_template_replacer.py` & `logprep-6.4.0/tests/unit/processor/template_replacer/test_template_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/test_processor_rule.py` & `logprep-6.4.0/tests/unit/processor/test_processor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/test_processor_strategy.py` & `logprep-6.4.0/tests/unit/processor/test_processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py` & `logprep-6.4.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py` & `logprep-6.4.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/timestamper/test_timestamper.py` & `logprep-6.4.0/tests/unit/processor/timestamper/test_timestamper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/processor/timestamper/test_timestamper_rule.py` & `logprep-6.4.0/tests/unit/processor/timestamper/test_timestamper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/test_configuration.py` & `logprep-6.4.0/tests/unit/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/test_factory.py` & `logprep-6.4.0/tests/unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/test_run_logprep.py` & `logprep-6.4.0/tests/unit/test_run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/test_runner.py` & `logprep-6.4.0/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_auto_rule_corpus_tester.py` & `logprep-6.4.0/tests/unit/util/test_auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_auto_rule_tester.py` & `logprep-6.4.0/tests/unit/util/test_auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_cache.py` & `logprep-6.4.0/tests/unit/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_configuration.py` & `logprep-6.4.0/tests/unit/util/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_getter.py` & `logprep-6.4.0/tests/unit/util/test_getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_grok_pattern_loader.py` & `logprep-6.4.0/tests/unit/util/test_grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_helper.py` & `logprep-6.4.0/tests/unit/util/test_helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_helper_add_field.py` & `logprep-6.4.0/tests/unit/util/test_helper_add_field.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_log_aggregator.py` & `logprep-6.4.0/tests/unit/util/test_log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_processor_generator.py` & `logprep-6.4.0/tests/unit/util/test_processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_prometheus_exporter.py` & `logprep-6.4.0/tests/unit/util/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_rule_dry_runner.py` & `logprep-6.4.0/tests/unit/util/test_rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_time.py` & `logprep-6.4.0/tests/unit/util/test_time.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_time_measurement.py` & `logprep-6.4.0/tests/unit/util/test_time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/test_validators.py` & `logprep-6.4.0/tests/unit/util/test_validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/unit/util/tests_json_handling.py` & `logprep-6.4.0/tests/unit/util/tests_json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/tests/util/testhelpers.py` & `logprep-6.4.0/tests/util/testhelpers.py`

 * *Files identical despite different names*

### Comparing `logprep-6.3.0/versioneer.py` & `logprep-6.4.0/versioneer.py`

 * *Files identical despite different names*

