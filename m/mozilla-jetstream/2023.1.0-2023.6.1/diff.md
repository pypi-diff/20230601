# Comparing `tmp/mozilla-jetstream-2023.1.0.tar.gz` & `tmp/mozilla-jetstream-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-jetstream-2023.1.0.tar", last modified: Wed Jan 25 22:44:04 2023, max compression
+gzip compressed data, was "mozilla-jetstream-2023.6.1.tar", last modified: Thu Jun  1 17:51:03 2023, max compression
```

## Comparing `mozilla-jetstream-2023.1.0.tar` & `mozilla-jetstream-2023.6.1.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.872232 mozilla-jetstream-2023.1.0/
--rw-r--r--   0 root         (0) root         (0)    16725 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1189 2023-01-25 22:44:04.872232 mozilla-jetstream-2023.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      853 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.864232 mozilla-jetstream-2023.1.0/jetstream/
--rw-r--r--   0 root         (0) root         (0)      100 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25885 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/analysis.py
--rw-r--r--   0 root         (0) root         (0)     8134 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/argo.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/bigquery_client.py
--rw-r--r--   0 root         (0) root         (0)    28037 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/cli.py
--rw-r--r--   0 root         (0) root         (0)    10261 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.864232 mozilla-jetstream-2023.1.0/jetstream/diagnostics/
--rw-r--r--   0 root         (0) root         (0)     6642 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/diagnostics/resource_profiling_plugin.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/diagnostics/task_monitoring_plugin.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/dryrun.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/errors.py
--rw-r--r--   0 root         (0) root         (0)     8083 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/experimenter.py
--rw-r--r--   0 root         (0) root         (0)     8486 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/export_json.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/exposure_signal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.864232 mozilla-jetstream-2023.1.0/jetstream/logging/
--rw-r--r--   0 root         (0) root         (0)     1421 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/logging/bigquery_log_handler.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/metadata.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/metric.py
--rw-r--r--   0 root         (0) root         (0)     3135 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/platform.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/segment.py
--rw-r--r--   0 root         (0) root         (0)    26899 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/statistics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.868232 mozilla-jetstream-2023.1.0/jetstream/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7857 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.868232 mozilla-jetstream-2023.1.0/jetstream/tests/data/
--rw-r--r--   0 root         (0) root         (0)     5091 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/Metadata_v1.0.json
--rw-r--r--   0 root         (0) root         (0)     7055 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/NimbusExperiment_v1.0.json
--rw-r--r--   0 root         (0) root         (0)     2983 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/Statistics_v1.0.json
--rw-r--r--   0 root         (0) root         (0)     2069 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/default_metrics.toml
--rw-r--r--   0 root         (0) root         (0)   732445 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/probe_data.json.gz
--rw-r--r--   0 root         (0) root         (0)     1591 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/test_clients_daily.ndjson
--rw-r--r--   0 root         (0) root         (0)     2818 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/test_clients_last_seen.ndjson
--rw-r--r--   0 root         (0) root         (0)     1351 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/test_events.ndjson
--rw-r--r--   0 root         (0) root         (0)    10925 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/wine.data
--rw-r--r--   0 root         (0) root         (0)     3036 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/data/wine.names
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.868232 mozilla-jetstream-2023.1.0/jetstream/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/integration/conftest.py
--rw-r--r--   0 root         (0) root         (0)    25701 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/integration/test_analysis_integration.py
--rw-r--r--   0 root         (0) root         (0)     7903 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     3717 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/integration/test_logging_integration.py
--rw-r--r--   0 root         (0) root         (0)    13572 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_argo.py
--rw-r--r--   0 root         (0) root         (0)    18048 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     5823 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    20799 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_experimenter.py
--rw-r--r--   0 root         (0) root         (0)     6078 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)    12938 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_metadata.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     2833 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_pretreatment.py
--rw-r--r--   0 root         (0) root         (0)    10984 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/tests/test_statistics.py
--rw-r--r--   0 root         (0) root         (0)     1372 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.868232 mozilla-jetstream-2023.1.0/jetstream/workflows/
--rw-r--r--   0 root         (0) root         (0)     3915 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/jetstream/workflows/run.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 22:44:04.868232 mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-01-25 22:44:04.000000 mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2026 2023-01-25 22:44:04.000000 mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 22:44:04.000000 mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-01-25 22:44:04.000000 mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      466 2023-01-25 22:44:04.000000 mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-25 22:44:04.000000 mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      528 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/platform_config.toml
--rw-r--r--   0 root         (0) root         (0)       85 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2023-01-25 22:44:04.872232 mozilla-jetstream-2023.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2152 2023-01-25 22:43:57.000000 mozilla-jetstream-2023.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.468599 mozilla-jetstream-2023.6.1/
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-06-01 17:51:03.468599 mozilla-jetstream-2023.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      853 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.456599 mozilla-jetstream-2023.6.1/jetstream/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28758 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     8255 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/argo.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/bigquery_client.py
+-rw-r--r--   0 root         (0) root         (0)    44798 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/cli.py
+-rw-r--r--   0 root         (0) root         (0)    10221 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.456599 mozilla-jetstream-2023.6.1/jetstream/diagnostics/
+-rw-r--r--   0 root         (0) root         (0)     6642 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/diagnostics/resource_profiling_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/diagnostics/task_monitoring_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/dryrun.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9175 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/experimenter.py
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/export_json.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/exposure_signal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.456599 mozilla-jetstream-2023.6.1/jetstream/logging/
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/logging/bigquery_log_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/platform.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/preview.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/segment.py
+-rw-r--r--   0 root         (0) root         (0)    27108 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.460599 mozilla-jetstream-2023.6.1/jetstream/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.464599 mozilla-jetstream-2023.6.1/jetstream/tests/data/
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/Metadata_v1.0.json
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/NimbusExperiment_v1.0.json
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/Statistics_v1.0.json
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/default_metrics.toml
+-rw-r--r--   0 root         (0) root         (0)   732445 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/probe_data.json.gz
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/test_clients_daily.ndjson
+-rw-r--r--   0 root         (0) root         (0)     2818 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/test_clients_last_seen.ndjson
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/test_events.ndjson
+-rw-r--r--   0 root         (0) root         (0)    10925 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/wine.data
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/data/wine.names
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.464599 mozilla-jetstream-2023.6.1/jetstream/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/integration/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    25935 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/integration/test_analysis_integration.py
+-rw-r--r--   0 root         (0) root         (0)     7903 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/integration/test_logging_integration.py
+-rw-r--r--   0 root         (0) root         (0)    15220 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_argo.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_bigquery_client.py
+-rw-r--r--   0 root         (0) root         (0)    18925 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     5837 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    20883 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_experimenter.py
+-rw-r--r--   0 root         (0) root         (0)     6078 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)    12952 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_pretreatment.py
+-rw-r--r--   0 root         (0) root         (0)    10984 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/tests/test_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.464599 mozilla-jetstream-2023.6.1/jetstream/workflows/
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/jetstream/workflows/run.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:51:03.468599 mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-06-01 17:51:03.000000 mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-06-01 17:51:03.000000 mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 17:51:03.000000 mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-01 17:51:03.000000 mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      466 2023-06-01 17:51:03.000000 mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-01 17:51:03.000000 mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      528 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/platform_config.toml
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-01 17:51:03.468599 mozilla-jetstream-2023.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-01 17:50:54.000000 mozilla-jetstream-2023.6.1/setup.py
```

### Comparing `mozilla-jetstream-2023.1.0/LICENSE` & `mozilla-jetstream-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/PKG-INFO` & `mozilla-jetstream-2023.6.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mozilla-jetstream
-Version: 2023.1.0
+Version: 2023.6.1
 Summary: Runs a thing that analyzes experiments
 Home-page: https://github.com/mozilla/jetstream
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 [![CircleCI](https://circleci.com/gh/mozilla/jetstream/tree/main.svg?style=shield)](https://circleci.com/gh/mozilla/jetstream/tree/main)
 
 # jetstream
```

### Comparing `mozilla-jetstream-2023.1.0/README.md` & `mozilla-jetstream-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/analysis.py` & `mozilla-jetstream-2023.6.1/jetstream/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import re
 from datetime import datetime, timedelta
+from pathlib import Path
 from textwrap import dedent
 from typing import Any, Dict, List, Optional
 
 import attr
 import dask
 import google
 import mozanalysis
@@ -40,27 +41,35 @@
 
 from . import bq_normalize_name
 
 logger = logging.getLogger(__name__)
 
 DASK_DASHBOARD_ADDRESS = "127.0.0.1:8782"
 DASK_N_PROCESSES = int(os.getenv("JETSTREAM_PROCESSES", 0)) or None  # Defaults to number of CPUs
+COST_PER_BYTE = 1 / 1024 / 1024 / 1024 / 1024 * 5
 
 _dask_cluster = None
 
 
 @attr.s(auto_attribs=True)
 class Analysis:
     """Wrapper for analysing experiments."""
 
     project: str
     dataset: str
     config: AnalysisConfiguration
     log_config: Optional[LogConfiguration] = None
     start_time: Optional[datetime] = None
+    analysis_periods: List[AnalysisPeriod] = [
+        AnalysisPeriod.DAY,
+        AnalysisPeriod.WEEK,
+        AnalysisPeriod.DAYS_28,
+        AnalysisPeriod.OVERALL,
+    ]
+    sql_output_dir: Optional[str] = None
 
     @property
     def bigquery(self):
         return BigQueryClient(project=self.project, dataset=self.dataset)
 
     def _get_timelimits_if_ready(
         self, period: AnalysisPeriod, current_date: datetime
@@ -135,14 +144,20 @@
         return TimeLimits.for_single_analysis_window(
             last_date_full_data=prior_date_str,
             analysis_start_days=0,
             analysis_length_dates=analysis_length_dates,
             **time_limits_args,
         )
 
+    def _write_sql_output(self, destination: str, sql: str):
+        """Write SQL query to local file named after `destination`."""
+        if self.sql_output_dir:
+            Path(self.sql_output_dir).mkdir(parents=True, exist_ok=True)
+            (Path(self.sql_output_dir) / destination).write_text(sql)
+
     def _table_name(
         self, window_period: str, window_index: int, analysis_basis: Optional[AnalysisBasis] = None
     ) -> str:
         """
         Returns the Bigquery table name for statistics and metrics result tables.
 
         Tables names are based on analysis period, analysis window and optionally analysis basis.
@@ -252,32 +267,37 @@
                 metrics,
                 last_window_limits,
                 enrollments_table_name,
                 analysis_basis,
                 exposure_signal,
             )
 
-            self.bigquery.execute(metrics_sql, res_table_name)
+            results = self.bigquery.execute(metrics_sql, res_table_name)
+            logger.info(
+                f"Metric query cost: {results.total_bytes_billed * COST_PER_BYTE}",
+            )
+            self._write_sql_output(res_table_name, metrics_sql)
             self._publish_view(period, analysis_basis=analysis_basis.value)
 
         return res_table_name
 
     @dask.delayed
     def calculate_statistics(
         self,
         metric: metric.Summary,
         segment_data: DataFrame,
         segment: str,
         analysis_basis: AnalysisBasis,
+        analysis_length_dates: int,
     ) -> StatisticResultCollection:
         """
         Run statistics on metric.
         """
         return (
-            Summary.from_config(metric)
+            Summary.from_config(metric, analysis_length_dates)
             .run(segment_data, self.config.experiment, analysis_basis, segment)
             .set_segment(segment)
             .set_analysis_basis(analysis_basis)
         )
 
     @dask.delayed
     def counts(
@@ -363,14 +383,17 @@
         if (
             current_date
             and self.config.experiment.end_date
             and self.config.experiment.end_date < current_date
         ):
             raise errors.EndedException(self.config.experiment.normandy_slug)
 
+        if self.config.experiment.is_rollout:
+            raise errors.RolloutSkipException(self.config.experiment.normandy_slug)
+
         return True
 
     def _app_id_to_bigquery_dataset(self, app_id: str) -> str:
         return re.sub(r"[^a-zA-Z0-9]", "_", app_id).lower()
 
     def validate(self) -> None:
         self.check_runnable()
@@ -431,14 +454,19 @@
             PLATFORM_CONFIGS[self.config.experiment.app_name].enrollments_query_type,
             self.config.experiment.enrollment_query,
             None,
             exposure_signal,
             segments,
         )
 
+        self._write_sql_output(
+            f"enrollments_{bq_normalize_name(self.config.experiment.normandy_slug)}",
+            enrollments_sql,
+        )
+
         dry_run_query(enrollments_sql)
         print(f"Dry running enrollments query for {self.config.experiment.normandy_slug}:")
         print(enrollments_sql)
 
         metrics_sql = exp.build_metrics_query(
             metrics, limits, "enrollments_table", AnalysisBasis.ENROLLMENTS
         )
@@ -462,14 +490,18 @@
                     DATE('2020-01-01') AS enrollment_date,
                     DATE('2020-01-01') AS exposure_date,
                     1 AS num_enrollment_events,
                     1 AS num_exposure_events
             ), analysis_windows AS (""",
         )
 
+        self._write_sql_output(
+            f"metrics_{bq_normalize_name(self.config.experiment.normandy_slug)}", metrics_sql
+        )
+
         dry_run_query(metrics_sql)
         print(f"Dry running metrics query for {self.config.experiment.normandy_slug}:")
         print(metrics_sql)
 
     @dask.delayed
     def save_statistics(
         self,
@@ -504,14 +536,27 @@
             self.config.experiment.normandy_slug,
             self.start_time,
         )
 
         self.check_runnable(current_date)
         assert self.config.experiment.start_date is not None  # for mypy
 
+        # make sure enrollment is actually ended (and enrollment is not manually overridden)
+        if (
+            hasattr(self.config.experiment, "is_enrollment_paused")
+            and self.config.experiment.is_enrollment_paused is False
+        ) and (
+            self.config.experiment.proposed_enrollment
+            == self.config.experiment.experiment.proposed_enrollment
+            and self.config.experiment.enrollment_end_date
+            == self.config.experiment.experiment.enrollment_end_date
+            and self.config.experiment.experiment_spec.enrollment_period is None
+        ):
+            raise errors.EnrollmentNotCompleteException(self.config.experiment.normandy_slug)
+
         self.ensure_enrollments(current_date)
 
         # set up dask
         _dask_cluster = _dask_cluster or LocalCluster(
             dashboard_address=DASK_DASHBOARD_ADDRESS,
             processes=True,
             threads_per_worker=1,
@@ -543,14 +588,18 @@
             #     experiment=self.config.experiment.normandy_slug,
             # )
             # _dask_cluster.scheduler.add_plugin(task_monitoring_plugin)
 
         table_to_dataframe = dask.delayed(self.bigquery.table_to_dataframe)
 
         for period in self.config.metrics:
+            if period not in self.analysis_periods:
+                logger.info(f"Skipping {period};")
+                continue
+
             segment_results = []
             time_limits = self._get_timelimits_if_ready(period, current_date)
 
             if time_limits is None:
                 logger.info(
                     "Skipping %s (%s); not ready [START: %s]",
                     self.config.experiment.normandy_slug,
@@ -604,19 +653,26 @@
                     for m in self.config.metrics[period]:
                         if (
                             m.metric.analysis_bases != analysis_basis
                             and analysis_basis not in m.metric.analysis_bases
                         ):
                             continue
 
+                        analysis_length_dates = 1
+                        if period.value == AnalysisPeriod.OVERALL:
+                            analysis_length_dates = time_limits.analysis_length_dates
+                        elif period.value == AnalysisPeriod.WEEK:
+                            analysis_length_dates = 7
+
                         segment_results += self.calculate_statistics(
                             m,
                             segment_data,
                             segment,
                             analysis_basis,
+                            analysis_length_dates,
                         ).to_dict()["data"]
 
                     segment_results += self.counts(segment_data, segment, analysis_basis).to_dict()[
                         "data"
                     ]
 
             results.append(
@@ -626,31 +682,16 @@
                     self._table_name(period.value, len(time_limits.analysis_windows)),
                 )
             )
 
         result_futures = client.compute(results)
         client.gather(result_futures)  # block until futures have finished
 
-    def ensure_enrollments(self, current_date: datetime) -> None:
-        """Ensure that enrollment tables for experiment are up-to-date or re-create."""
-        time_limits = self._get_timelimits_if_ready(AnalysisPeriod.DAY, current_date)
-
-        if time_limits is None:
-            logger.info(
-                "Skipping enrollments for %s; not ready", self.config.experiment.normandy_slug
-            )
-            return
-
-        if self.config.experiment.start_date is None:
-            raise errors.NoStartDateException(self.config.experiment.normandy_slug)
-
-        normalized_slug = bq_normalize_name(self.config.experiment.normandy_slug)
-        enrollments_table = f"enrollments_{normalized_slug}"
-
-        logger.info(f"Create {enrollments_table}")
+    def enrollments_query(self, time_limits: TimeLimits) -> str:
+        """Returns the enrollments SQL query."""
         exp = mozanalysis.experiment.Experiment(
             experiment_slug=self.config.experiment.normandy_slug,
             start_date=self.config.experiment.start_date.strftime("%Y-%m-%d"),
             app_id=self._app_id_to_bigquery_dataset(self.config.experiment.app_id),
         )
 
         exposure_signal = None
@@ -660,24 +701,47 @@
             )
             exposure_signal = exposure_signal.to_mozanalysis_exposure_signal(time_limits)
 
         segments = []
         for segment in self.config.experiment.segments:
             segments.append(Segment.from_segment_config(segment).to_mozanalysis_segment())
 
-        enrollments_sql = exp.build_enrollments_query(
+        return exp.build_enrollments_query(
             time_limits,
             PLATFORM_CONFIGS[self.config.experiment.app_name].enrollments_query_type,
             self.config.experiment.enrollment_query,
             None,
             exposure_signal,
             segments,
         )
 
+    def ensure_enrollments(self, current_date: datetime) -> None:
+        """Ensure that enrollment tables for experiment are up-to-date or re-create."""
+        time_limits = self._get_timelimits_if_ready(AnalysisPeriod.DAY, current_date)
+
+        if time_limits is None:
+            logger.info(
+                "Skipping enrollments for %s; not ready", self.config.experiment.normandy_slug
+            )
+            return
+
+        if self.config.experiment.start_date is None:
+            raise errors.NoStartDateException(self.config.experiment.normandy_slug)
+
+        normalized_slug = bq_normalize_name(self.config.experiment.normandy_slug)
+        enrollments_table = f"enrollments_{normalized_slug}"
+
+        logger.info(f"Create {enrollments_table}")
+        enrollments_sql = self.enrollments_query(time_limits=time_limits)
+
         try:
-            self.bigquery.execute(
+            self._write_sql_output(enrollments_table, enrollments_sql)
+            results = self.bigquery.execute(
                 enrollments_sql,
                 enrollments_table,
                 google.cloud.bigquery.job.WriteDisposition.WRITE_EMPTY,
             )
+            logger.info(
+                "Enrollment query cost: " + f"{results.total_bytes_billed * COST_PER_BYTE}",
+            )
         except Conflict:
             pass
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/argo.py` & `mozilla-jetstream-2023.6.1/jetstream/argo.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,21 +61,24 @@
     if monitor_status:
         finished = False
 
         logger.info("Argo workflow is running")
         # link to logs
         logger.info(
             "To connect to Argo dashboard forward port by running: "
-            + f"gcloud container clusters get-credentials jetstream --zone {zone} "
-            + f"--project {project_id} && "
-            + "kubectl port-forward --namespace argo $(kubectl get pod --namespace argo "
-            + "--selector='app=argo-server' --output jsonpath='{.items[0].metadata.name}') "
-            + "8080:2746"
+            + f"gcloud container clusters get-credentials jetstream --region={zone} && "
+            + "kubectl -n argo exec $(kubectl get pod -n argo -l 'app=argo-server' "
+            + "-o jsonpath='{.items[0].metadata.name}') -- argo auth token \n\n"
+            + "Copy the Bearer token.\n"
+        )
+        logger.info("kubectl -n argo port-forward svc/argo-server 2746:2746 \n")
+        logger.info(
+            "The dashboard can be accessed via 127.0.0.1:2746. "
+            + "Use the Bearer token for authentication."
         )
-        logger.info("The dashboard can be accessed via 127.0.0.1:8080")
 
         while not finished:
             workflow = api.get_workflow(
                 workflow["metadata"]["namespace"], workflow["metadata"]["name"]
             )
 
             if (
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/bigquery_client.py` & `mozilla-jetstream-2023.6.1/jetstream/bigquery_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 import time
-from typing import Any, Dict, Iterable, Mapping, Optional
+from typing import Any, Dict, Iterable, List, Mapping, Optional
 
 import attr
 import google.cloud.bigquery
 import google.cloud.bigquery.client
 import google.cloud.bigquery.dataset
 import google.cloud.bigquery.job
 import google.cloud.bigquery.table
@@ -61,15 +61,15 @@
         )
 
     def execute(
         self,
         query: str,
         destination_table: Optional[str] = None,
         write_disposition: Optional[google.cloud.bigquery.job.WriteDisposition] = None,
-    ) -> None:
+    ) -> google.cloud.bigquery.job.QueryJob:
         dataset = google.cloud.bigquery.dataset.DatasetReference.from_string(
             self.dataset,
             default_project=self.project,
         )
         kwargs: Dict[str, Any] = {}
         if destination_table:
             kwargs["destination"] = dataset.table(destination_table)
@@ -86,14 +86,16 @@
         if destination_table:
             # add a label with the current timestamp to the table
             self.add_labels_to_table(
                 destination_table,
                 {"last_updated": self._current_timestamp_label()},
             )
 
+        return job
+
     def tables_matching_regex(self, regex: str):
         """Returns a list of tables with names matching the specified pattern."""
         table_name_re = re.compile(regex)
         existing_tables = self.client.list_tables(self.dataset)
         return [table.table_id for table in existing_tables if table_name_re.match(table.table_id)]
 
     def touch_tables(self, normandy_slug: str):
@@ -108,7 +110,27 @@
         timestamp = self._current_timestamp_label()
         for table in tables:
             self.add_labels_to_table(table, {"last_updated": timestamp})
 
     def delete_table(self, table_id: str) -> None:
         """Delete the table."""
         self.client.delete_table(table_id, not_found_ok=True)
+
+    def delete_experiment_tables(
+        self, slug: str, analysis_periods: List[AnalysisPeriod], delete_enrollments: bool = False
+    ):
+        """Delete all tables associated with the specified experiment slug."""
+        normalized_slug = bq_normalize_name(slug)
+        analysis_periods_re = "|".join([p.value for p in analysis_periods])
+
+        existing_tables = self.tables_matching_regex(
+            f"^{normalized_slug}_.+_({analysis_periods_re}).*$"
+        )
+        existing_tables += self.tables_matching_regex(
+            f"^statistics_{normalized_slug}_({analysis_periods_re}).*$"
+        )
+
+        if delete_enrollments:
+            existing_tables += self.tables_matching_regex(f"^enrollments_{normalized_slug}$")
+
+        for existing_table in existing_tables:
+            self.delete_table(f"{self.project}.{self.dataset}.{existing_table}")
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/config.py` & `mozilla-jetstream-2023.6.1/jetstream/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 )
 from metric_config_parser.data_source import DataSource
 from metric_config_parser.experiment import Experiment
 from pytz import UTC
 
 from . import bq_normalize_name
 
-DEFAULT_CONFIG_REPO = "https://github.com/mozilla/jetstream-config"
 METRIC_HUB_REPO = "https://github.com/mozilla/metric-hub"
+CONFIGS = "https://github.com/mozilla/metric-hub/tree/main/jetstream"
 
 
 class _ConfigLoader:
     """
     Loads config files from an external repository.
 
     Config objects are converted into jetstream native types.
@@ -53,17 +53,15 @@
     @property
     def configs(self) -> ConfigCollection:
         configs = getattr(self, "_configs", None)
         if configs:
             return configs
 
         if self.config_collection is None:
-            self.config_collection = ConfigCollection.from_github_repos(
-                [METRIC_HUB_REPO, DEFAULT_CONFIG_REPO]
-            )
+            self.config_collection = ConfigCollection.from_github_repos([METRIC_HUB_REPO, CONFIGS])
         self._configs = self.config_collection
         return self._configs
 
     def with_configs_from(
         self, repo_urls: Optional[List[str]], is_private: bool = False
     ) -> "_ConfigLoader":
         """Load configs from another repository and merge with default configs."""
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/diagnostics/resource_profiling_plugin.py` & `mozilla-jetstream-2023.6.1/jetstream/diagnostics/resource_profiling_plugin.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/diagnostics/task_monitoring_plugin.py` & `mozilla-jetstream-2023.6.1/jetstream/diagnostics/task_monitoring_plugin.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/dryrun.py` & `mozilla-jetstream-2023.6.1/jetstream/dryrun.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/errors.py` & `mozilla-jetstream-2023.6.1/jetstream/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,25 @@
     """Exception thrown when an experiment is invalid."""
 
     def __init__(self, message):
         super().__init__(message)
 
 
 class NoSlugException(ValidationException):
-    def __init__(self, message="Experiment has no slug"):
+    def __init__(self, message="Experiment has no slug."):
         super().__init__(message)
 
 
 class NoEnrollmentPeriodException(ValidationException):
-    def __init__(self, normandy_slug, message="Experiment has no enrollment period"):
+    def __init__(self, normandy_slug, message="Experiment has no enrollment period."):
+        super().__init__(f"{normandy_slug} -> {message}")
+
+
+class EnrollmentNotCompleteException(ValidationException):
+    def __init__(self, normandy_slug, message="Experiment has not finished enrollment."):
         super().__init__(f"{normandy_slug} -> {message}")
 
 
 class NoStartDateException(ValidationException):
     def __init__(self, normandy_slug, message="Experiment has no start date."):
         super().__init__(f"{normandy_slug} -> {message}")
 
@@ -36,14 +41,19 @@
 
 
 class ExplicitSkipException(ValidationException):
     def __init__(self, normandy_slug, message="Experiment is configured with skip=true."):
         super().__init__(f"{normandy_slug} -> {message}")
 
 
+class RolloutSkipException(ValidationException):
+    def __init__(self, normandy_slug, message="Experiment is a rollout and will not be analyzed."):
+        super().__init__(f"{normandy_slug} -> {message}")
+
+
 class InvalidConfigurationException(Exception):
     """Exception thrown when experiment configuration is invalid."""
 
     def __init__(self, message):
         super().__init__(message)
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/experimenter.py` & `mozilla-jetstream-2023.6.1/jetstream/experimenter.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,14 +97,16 @@
     endDate: Optional[dt.datetime]
     proposedEnrollment: int
     referenceBranch: Optional[str]
     _appName: Optional[str] = None
     _appId: Optional[str] = None
     outcomes: Optional[List[Outcome]] = None
     enrollmentEndDate: Optional[dt.datetime] = None
+    isEnrollmentPaused: Optional[bool] = None
+    isRollout: bool = False
 
     @property
     def appName(self) -> str:
         return self._appName or "firefox_desktop"
 
     @property
     def appId(self) -> str:
@@ -149,32 +151,41 @@
             is_high_population=False,
             app_name=self.appName,
             app_id=self.appId,
             outcomes=[o.slug for o in self.outcomes] if self.outcomes else [],
             enrollment_end_date=pytz.utc.localize(self.enrollmentEndDate)
             if self.enrollmentEndDate
             else None,
+            is_enrollment_paused=bool(self.isEnrollmentPaused),
+            is_rollout=self.isRollout,
         )
 
 
 @attr.s(auto_attribs=True)
 class ExperimentCollection:
     experiments: List[experiment.Experiment] = attr.Factory(list)
 
     MAX_RETRIES = 3
     EXPERIMENTER_API_URL_V1 = "https://experimenter.services.mozilla.com/api/v1/experiments/"
 
     # for nimbus experiments
     EXPERIMENTER_API_URL_V6 = "https://experimenter.services.mozilla.com/api/v6/experiments/"
 
+    # experiments that are in draft state
+    EXPERIMENTER_API_URL_V6_DRAFTS = (
+        "https://experimenter.services.mozilla.com/api/v6/draft-experiments/"
+    )
+
     # user agent sent to the Experimenter API
     USER_AGENT = "jetstream"
 
     @classmethod
-    def from_experimenter(cls, session: requests.Session = None) -> "ExperimentCollection":
+    def from_experimenter(
+        cls, session: requests.Session = None, with_draft_experiments=False
+    ) -> "ExperimentCollection":
         session = session or requests.Session()
         legacy_experiments_json = retry_get(
             session, cls.EXPERIMENTER_API_URL_V1, cls.MAX_RETRIES, cls.USER_AGENT
         )
         legacy_experiments = []
 
         for legacy_experiment in legacy_experiments_json:
@@ -197,15 +208,31 @@
             try:
                 nimbus_experiments.append(ExperimentV6.from_dict(nimbus_experiment).to_experiment())
             except Exception as e:
                 logger.exception(
                     str(e), exc_info=e, extra={"experiment": nimbus_experiment["slug"]}
                 )
 
-        return cls(nimbus_experiments + legacy_experiments)
+        draft_experiments = []
+        if with_draft_experiments:
+            # draft experiments are mainly used to compute previews
+            draft_experiments_json = retry_get(
+                session, cls.EXPERIMENTER_API_URL_V6_DRAFTS, cls.MAX_RETRIES, cls.USER_AGENT
+            )
+
+            for draft_experiment in draft_experiments_json:
+                try:
+                    draft_experiments.append(
+                        ExperimentV6.from_dict(draft_experiment).to_experiment()
+                    )
+                except Exception as e:
+                    print(f"Error converting draft experiment {draft_experiment['slug']}")
+                    print(str(e))
+
+        return cls(nimbus_experiments + legacy_experiments + draft_experiments)
 
     def of_type(self, type_or_types: Union[str, Iterable[str]]) -> "ExperimentCollection":
         if isinstance(type_or_types, str):
             type_or_types = (type_or_types,)
         cls = type(self)
         return cls([ex for ex in self.experiments if ex.type in type_or_types])
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/export_json.py` & `mozilla-jetstream-2023.6.1/jetstream/export_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from datetime import datetime, timedelta
 from typing import Callable, Dict, Optional
 
 import cattr
 import google.cloud.bigquery as bigquery
 import google.cloud.storage as storage
 import smart_open
+from google.cloud.exceptions import BadRequest
 from metric_config_parser.metric import AnalysisPeriod
 
 from jetstream import bq_normalize_name
 from jetstream.logging import LogConfiguration
 
 logger = logging.getLogger(__name__)
 
 EXPERIMENT_LOG_PATH = "errors"
+SKIP_ERROR_TYPES = ["EndedException", "EnrollmentNotCompleteException"]
 
 
 def _get_statistics_tables_last_modified(
     client: bigquery.Client, bq_dataset: str, experiment_slug: Optional[str]
 ) -> Dict[str, datetime]:
     """Returns statistics table names and their last modified timestamp as datetime object."""
     experiment_table = "%"
@@ -57,23 +59,32 @@
     dataset_id: str,
     table: str,
     bucket: str,
     target_path: str,
     storage_client: storage.Client,
 ):
     """Export a single table or view to GCS as JSON."""
-    # since views cannot get exported directly, write data into a temporary table
-    job = client.query(
-        f"""
-        SELECT *
-        FROM {dataset_id}.{table}
-    """
-    )
-
-    job.result()
+    try:
+        # since views cannot get exported directly, write data into a temporary table
+        job = client.query(
+            f"""
+            SELECT *
+            FROM {dataset_id}.{table}
+        """
+        )
+
+        job.result()
+    except BadRequest as e:
+        if "does not match any table" in e.message:
+            logger.error(
+                f"google.cloud.exceptions.BadRequest: {e.args[0]}. Skipping query and export..."
+            )
+            return
+        else:
+            raise e
 
     # add a random string to the identifier to prevent collision errors if there
     # happen to be multiple instances running that export data for the same experiment
     tmp = "".join(random.choices(string.ascii_lowercase, k=8))
     destination_uri = f"gs://{bucket}/{target_path}/{table}-{tmp}.ndjson"
     dataset_ref = bigquery.DatasetReference(project_id, job.destination.dataset_id)
     table_ref = dataset_ref.table(job.destination.table_id)
@@ -163,14 +174,17 @@
         FROM {dataset}.{table}
         WHERE experiment = '{experiment_slug}'
     """
     if min_timestamp is not None:
         floored_timestamp = min_timestamp.replace(second=0, microsecond=0)
         query_text += f" AND timestamp >= TIMESTAMP('{floored_timestamp}')"
 
+    for exception_type in SKIP_ERROR_TYPES:
+        query_text += f" AND exception_type != '{exception_type}'"
+
     query_text += " ORDER BY timestamp ASC"
 
     results = client.query(query_text).result()
 
     # convert results to JSON
     records = [dict(row) for row in results]
     converter = cattr.GenConverter()
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/exposure_signal.py` & `mozilla-jetstream-2023.6.1/jetstream/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/logging/__init__.py` & `mozilla-jetstream-2023.6.1/jetstream/logging/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,28 @@
     log_project_id: Optional[str]
     log_dataset_id: Optional[str]
     log_table_id: Optional[str]
     task_profiling_log_table_id: Optional[str]
     task_monitoring_log_table_id: Optional[str]
     log_to_bigquery: bool = False
     capacity: int = 50
+    log_level: int = logging.WARNING
 
     def setup_logger(self, client=None):
         logging.basicConfig(
             level=logging.INFO,
             format="%(levelname)s:%(asctime)s:%(name)s:%(message)s",
         )
         logger = logging.getLogger()
 
         if self.log_to_bigquery:
             bigquery_handler = BigQueryLogHandler(
                 self.log_project_id, self.log_dataset_id, self.log_table_id, client, self.capacity
             )
-            bigquery_handler.setLevel(logging.WARNING)
+            bigquery_handler.setLevel(self.log_level)
             logger.addHandler(bigquery_handler)
 
 
 class LogPlugin(WorkerPlugin):
     """
     Dask worker plugin for initializing the logger.
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/logging/bigquery_log_handler.py` & `mozilla-jetstream-2023.6.1/jetstream/logging/bigquery_log_handler.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/metadata.py` & `mozilla-jetstream-2023.6.1/jetstream/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import attr
 import cattr
 import google.cloud.storage as storage
 from metric_config_parser.analysis import AnalysisConfiguration
 
 from jetstream import bq_normalize_name
-from jetstream.config import DEFAULT_CONFIG_REPO, ConfigLoader
+from jetstream.config import METRIC_HUB_REPO, ConfigLoader
 from jetstream.statistics import StatisticResult
 
 logger = logging.getLogger(__name__)
 
 
 @attr.s(auto_attribs=True)
 class MetricsMetadata:
@@ -109,15 +109,18 @@
                 and config.experiment.start_date != config.experiment.experiment.start_date
                 else None,
                 enrollment_period=config.experiment.enrollment_period
                 if config.experiment.enrollment_period
                 != config.experiment.experiment.proposed_enrollment
                 else None,
                 skip=config.experiment.skip,
-                url=DEFAULT_CONFIG_REPO + "/blob/main/" + config.experiment.normandy_slug + ".toml",
+                url=METRIC_HUB_REPO
+                + "/blob/main/jetstream/"
+                + config.experiment.normandy_slug
+                + ".toml",
             )
 
         return cls(
             metrics=metrics_metadata,
             outcomes=outcomes_metadata,
             external_config=external_config,
             analysis_start_time=analysis_start_time,
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/metric.py` & `mozilla-jetstream-2023.6.1/jetstream/metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/platform.py` & `mozilla-jetstream-2023.6.1/jetstream/platform.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/pre_treatment.py` & `mozilla-jetstream-2023.6.1/jetstream/pre_treatment.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 @attr.s(auto_attribs=True)
 class PreTreatment(ABC):
     """
     Represents an abstract pre-treatment step applied to data before
     calculating statistics.
     """
 
+    analysis_period_length: int = attr.ib(kw_only=True, default=1)
+
     @classmethod
     def name(cls):
         """Return snake-cased name of the statistic."""
         return re.sub(r"(?<!^)(?=[A-Z])", "_", cls.__name__).lower()
 
     @abstractmethod
     def apply(self, df: DataFrame, col: str) -> DataFrame:
@@ -90,14 +92,25 @@
 
     def apply(self, df: DataFrame, col: str) -> DataFrame:
         mask = df[col] < self.threshold
         return df.loc[mask, :]
 
 
 @attr.s(auto_attribs=True)
+class NormalizeOverAnalysisPeriod(PreTreatment):
+    """Normalizes the row values over a given analysis period (number of days)."""
+
+    analysis_period_length: int = 1
+
+    def apply(self, df: DataFrame, col: str) -> DataFrame:
+        df[col] = df[col] / self.analysis_period_length
+        return df
+
+
+@attr.s(auto_attribs=True)
 class Log(PreTreatment):
     base: Optional[float] = 10.0
 
     def apply(self, df: DataFrame, col: str) -> DataFrame:
         # Silence divide-by-zero and domain warnings
         with np.errstate(divide="ignore", invalid="ignore"):
             result = np.log(df[col])
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/segment.py` & `mozilla-jetstream-2023.6.1/jetstream/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/statistics.py` & `mozilla-jetstream-2023.6.1/jetstream/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,17 @@
     """Represents a metric with a statistical treatment."""
 
     metric: Metric
     statistic: "Statistic"
     pre_treatments: List[PreTreatment] = attr.Factory(list)
 
     @classmethod
-    def from_config(cls, summary_config: parser_metric.Summary) -> "Summary":
+    def from_config(
+        cls, summary_config: parser_metric.Summary, analysis_period_length: Optional[int]
+    ) -> "Summary":
         """Create a Jetstream-native Summary representation."""
         metric = Metric.from_metric_config(summary_config.metric)
 
         found = False
         for statistic in Statistic.__subclasses__():
             if statistic.name() == summary_config.statistic.name:
                 found = True
@@ -63,14 +65,17 @@
         for pre_treatment_conf in summary_config.pre_treatments:
             found = False
             for pre_treatment in PreTreatment.__subclasses__():
                 if isabstract(pre_treatment):
                     continue
                 if pre_treatment.name() == pre_treatment_conf.name:
                     found = True
+                    # inject analysis_period_length from experiment
+                    pre_treatment.analysis_period_length = analysis_period_length or 1
+
                     pre_treatments.append(pre_treatment.from_dict(pre_treatment_conf.args))
 
             if not found:
                 raise ValueError(f"Could not find pre-treatment {pre_treatment_conf.name}.")
 
         return cls(
             metric=metric,
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/conftest.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,14 +127,46 @@
             normandy_slug="normandy-test-slug",
             reference_branch=None,
             is_high_population=True,
             outcomes=["parameterised_distinct_by_branch_config"],
             app_name="firefox_desktop",
             app_id="firefox-desktop",
         ),
+        Experiment(
+            experimenter_slug=None,
+            type="pref",
+            status="Live",
+            start_date=dt.datetime(2019, 12, 1, tzinfo=pytz.utc),
+            end_date=None,
+            proposed_enrollment=7,
+            branches=[],
+            normandy_slug="normandy-test-slug",
+            reference_branch=None,
+            is_high_population=False,
+            app_name="firefox_desktop",
+            app_id="firefox-desktop",
+            enrollment_end_date=dt.datetime(2019, 12, 8, tzinfo=pytz.utc),
+            is_enrollment_paused=False,
+        ),
+        Experiment(
+            experimenter_slug=None,
+            type="pref",
+            status="Live",
+            start_date=dt.datetime(2019, 12, 1, tzinfo=pytz.utc),
+            end_date=None,
+            proposed_enrollment=7,
+            branches=[],
+            normandy_slug="normandy-test-slug",
+            reference_branch=None,
+            is_high_population=False,
+            app_name="firefox_desktop",
+            app_id="firefox-desktop",
+            enrollment_end_date=dt.datetime(2019, 12, 8, tzinfo=pytz.utc),
+            is_enrollment_paused=True,
+        ),
     ]
 
 
 @pytest.fixture
 def fenix_experiments():
     return [
         Experiment(
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/Metadata_v1.0.json` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/Metadata_v1.0.json`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/NimbusExperiment_v1.0.json` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/NimbusExperiment_v1.0.json`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/Statistics_v1.0.json` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/Statistics_v1.0.json`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/default_metrics.toml` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/default_metrics.toml`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/probe_data.json.gz` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/probe_data.json.gz`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/test_clients_daily.ndjson` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/test_clients_daily.ndjson`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/test_clients_last_seen.ndjson` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/test_clients_last_seen.ndjson`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/test_events.ndjson` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/test_events.ndjson`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 {"submission_date": "2020-04-02", "client_id": "aaaa", "event_category": "normandy", "event_method": "enroll", "event_string_value": "test-experiment", "event_map_values": [{"key": "branch", "value": "branch1"}]}
 {"submission_date": "2020-04-03", "client_id": "bbbb", "event_category": "normandy", "event_method": "enroll", "event_string_value": "test-experiment", "event_map_values": [{"key": "branch", "value": "branch2"}]}
-{"submission_date": "2020-04-02", "client_id": "aaaa", "event_category": "normandy", "event_method": "exposure", "event_string_value": "test-experiment", "event_map_values": [{"key": "branch", "value": "branch1"}]}
-{"submission_date": "2020-04-03", "client_id": "bbbb", "event_category": "normandy", "event_method": "exposure", "event_string_value": "test-experiment", "event_map_values": [{"key": "branch", "value": "branch2"}]}
+{"submission_date": "2020-04-02", "client_id": "aaaa", "event_category": "normandy", "event_method": "exposure", "event_string_value": "test-experiment", "event_map_values": [{"key": "branchSlug", "value": "branch1"}]}
+{"submission_date": "2020-04-03", "client_id": "bbbb", "event_category": "normandy", "event_method": "expose", "event_string_value": "test-experiment", "event_map_values": [{"key": "branchSlug", "value": "branch2"}]}
 {"submission_date": "2020-04-03", "client_id": "bbbb", "event_category": "foo"}
 {"submission_date": "2020-04-03", "client_id": "cccc", "event_category": "foo", "event_method": "enroll", "event_string_value": "test-experiment", "event_map_values": [{"key": "branch", "value": "branch1"}]}
 {"submission_date": "2020-04-03", "client_id": "dddd", "event_category": "foo", "event_method": "enroll", "event_string_value": "test-experiment", "event_map_values": [{"key": "branch", "value": "branch2"}]}
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/wine.data` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/wine.data`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/data/wine.names` & `mozilla-jetstream-2023.6.1/jetstream/tests/data/wine.names`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/integration/conftest.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/integration/test_analysis_integration.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/integration/test_analysis_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         experiment = Experiment(
             experimenter_slug="test-experiment",
             type="rollout",
             status="Live",
             start_date=dt.datetime(2020, 3, 30, tzinfo=pytz.utc),
             end_date=dt.datetime(2020, 6, 1, tzinfo=pytz.utc),
             proposed_enrollment=7,
+            is_enrollment_paused=True,
             branches=[Branch(slug="branch1", ratio=0.5), Branch(slug="branch2", ratio=0.5)],
             reference_branch="branch2",
             normandy_slug="test-experiment",
             is_high_population=False,
             app_name="firefox_desktop",
             app_id="firefox-desktop",
         )
@@ -193,14 +194,15 @@
         experiment = Experiment(
             experimenter_slug="test-experiment",
             type="rollout",
             status="Live",
             start_date=dt.datetime(2020, 3, 30, tzinfo=pytz.utc),
             end_date=dt.datetime(2020, 6, 1, tzinfo=pytz.utc),
             proposed_enrollment=7,
+            is_enrollment_paused=True,
             branches=[Branch(slug="branch1", ratio=0.5), Branch(slug="branch2", ratio=0.5)],
             reference_branch="branch2",
             normandy_slug="test-experiment",
             is_high_population=False,
             app_name="firefox_desktop",
             app_id="firefox-desktop",
         )
@@ -294,14 +296,15 @@
         experiment = Experiment(
             experimenter_slug="test-experiment-2",
             type="rollout",
             status="Live",
             start_date=dt.datetime(2020, 3, 30, tzinfo=pytz.utc),
             end_date=dt.datetime(2020, 6, 1, tzinfo=pytz.utc),
             proposed_enrollment=7,
+            is_enrollment_paused=True,
             branches=[Branch(slug="a", ratio=0.5), Branch(slug="b", ratio=0.5)],
             reference_branch="a",
             normandy_slug="test-experiment-2",
             is_high_population=False,
             app_name="firefox_desktop",
             app_id="firefox-desktop",
         )
@@ -360,14 +363,15 @@
         experiment = Experiment(
             experimenter_slug="test-experiment",
             type="rollout",
             status="Live",
             start_date=dt.datetime(2020, 3, 30, tzinfo=pytz.utc),
             end_date=dt.datetime(2020, 6, 1, tzinfo=pytz.utc),
             proposed_enrollment=7,
+            is_enrollment_paused=True,
             branches=[Branch(slug="branch1", ratio=0.5), Branch(slug="branch2", ratio=0.5)],
             reference_branch="branch2",
             normandy_slug="test-experiment",
             is_high_population=False,
             app_name="firefox_desktop",
             app_id="firefox-desktop",
         )
@@ -512,14 +516,15 @@
         experiment = Experiment(
             experimenter_slug="test-experiment",
             type="rollout",
             status="Live",
             start_date=dt.datetime(2020, 3, 30, tzinfo=pytz.utc),
             end_date=dt.datetime(2020, 6, 1, tzinfo=pytz.utc),
             proposed_enrollment=7,
+            is_enrollment_paused=True,
             branches=[Branch(slug="branch1", ratio=0.5), Branch(slug="branch2", ratio=0.5)],
             reference_branch="branch2",
             normandy_slug="test-experiment",
             is_high_population=False,
             app_name="firefox_desktop",
             app_id="firefox-desktop",
         )
@@ -634,14 +639,15 @@
         experiment = Experiment(
             experimenter_slug="test-experiment",
             type="rollout",
             status="Live",
             start_date=dt.datetime(2020, 3, 30, tzinfo=pytz.utc),
             end_date=dt.datetime(2020, 6, 1, tzinfo=pytz.utc),
             proposed_enrollment=7,
+            is_enrollment_paused=True,
             branches=[Branch(slug="branch1", ratio=0.5), Branch(slug="branch2", ratio=0.5)],
             reference_branch="branch2",
             normandy_slug="test-experiment",
             is_high_population=False,
             app_name="firefox_desktop",
             app_id="firefox-desktop",
         )
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/integration/test_config_integration.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/integration/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/integration/test_logging_integration.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/integration/test_logging_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_analysis.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from metric_config_parser.analysis import AnalysisSpec
 from metric_config_parser.metric import AnalysisBasis, AnalysisPeriod
 
 import jetstream.analysis
 from jetstream.analysis import Analysis
 from jetstream.config import ConfigLoader
 from jetstream.errors import (
+    EnrollmentNotCompleteException,
     ExplicitSkipException,
     HighPopulationException,
     NoEnrollmentPeriodException,
 )
 from jetstream.experimenter import ExperimentV1
 
 
@@ -274,14 +275,60 @@
     configured = spec.resolve(experiments[0], ConfigLoader.configs)
     with pytest.raises(ExplicitSkipException):
         Analysis("test", "test", configured).run(
             current_date=dt.datetime(2020, 1, 1, tzinfo=pytz.utc), dry_run=True
         )
 
 
+def test_skip_while_enrolling(experiments):
+    config = AnalysisSpec().resolve(experiments[8], ConfigLoader.configs)
+    with pytest.raises(EnrollmentNotCompleteException):
+        Analysis("test", "test", config).run(
+            current_date=dt.datetime(2020, 1, 1, tzinfo=pytz.utc), dry_run=True
+        )
+
+
+def test_custom_override_skips_enrollment_paused_check(experiments, monkeypatch):
+    conf = dedent(
+        """
+        [experiment]
+        enrollment_period = 7
+        """
+    )
+    spec = AnalysisSpec.from_dict(toml.loads(conf))
+    config = spec.resolve(experiments[8], ConfigLoader.configs)
+    m = Mock()
+    m.return_value = None
+    monkeypatch.setattr("jetstream.analysis.Analysis._get_timelimits_if_ready", m)
+    # no errors expected
+    Analysis("test", "test", config).run(
+        current_date=dt.datetime(2020, 1, 1, tzinfo=pytz.utc), dry_run=True
+    )
+
+
+def test_validation_working_while_enrolling(experiments):
+    config = AnalysisSpec().resolve(experiments[8], ConfigLoader.configs)
+    assert experiments[8].is_enrollment_paused is False
+    try:
+        Analysis("test", "test", config).validate()
+    except Exception as e:
+        assert False, f"Raised {e}"
+
+
+def test_run_when_enrolling_complete(experiments, monkeypatch):
+    config = AnalysisSpec().resolve(experiments[9], ConfigLoader.configs)
+    m = Mock()
+    m.return_value = None
+    monkeypatch.setattr("jetstream.analysis.Analysis._get_timelimits_if_ready", m)
+    # no errors expected
+    Analysis("test", "test", config).run(
+        current_date=dt.datetime(2020, 1, 1, tzinfo=pytz.utc), dry_run=True
+    )
+
+
 def test_fenix_experiments_use_right_datasets(fenix_experiments, monkeypatch):
     for experiment in fenix_experiments:
         called = 0
 
         def dry_run_query(query):
             nonlocal called
             called = called + 1
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_argo.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_argo.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_cli.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import attr
 import pytest
 import toml
 from click.testing import CliRunner
 from metric_config_parser.analysis import AnalysisSpec
 from metric_config_parser.config import Config, ConfigCollection
 from metric_config_parser.experiment import Branch, Experiment
+from metric_config_parser.metric import AnalysisPeriod
 from pytz import UTC
 
 from jetstream import cli, experimenter
 from jetstream.config import ConfigLoader, _ConfigLoader
 
 
 @pytest.fixture(name="cli_experiments")
@@ -455,47 +456,70 @@
             analysis_class=fake_analysis,
             experiment_getter=lambda: cli_experiments,
             config_getter=ConfigLoader,
         )
         config = spec.resolve(experiment, ConfigLoader.configs)
         run_date = dt.datetime(2020, 10, 31, tzinfo=UTC)
         strategy.execute([(config, run_date)])
-        fake_analysis.assert_called_once_with("spam", "eggs", config, None)
+        fake_analysis.assert_called_once_with(
+            "spam",
+            "eggs",
+            config,
+            None,
+            None,
+            [
+                AnalysisPeriod.DAY,
+                AnalysisPeriod.WEEK,
+                AnalysisPeriod.DAYS_28,
+                AnalysisPeriod.OVERALL,
+            ],
+            None,
+        )
         fake_analysis().run.assert_called_once_with(run_date)
 
 
 class TestArgoExecutorStrategy:
     def test_simple_workflow(self, cli_experiments):
         experiment = cli_experiments.experiments[0]
         spec = AnalysisSpec.default_for_experiment(experiment, ConfigLoader.configs)
         config = spec.resolve(experiment, ConfigLoader.configs)
 
         with mock.patch("jetstream.cli.submit_workflow") as submit_workflow_mock:
             strategy = cli.ArgoExecutorStrategy(
-                "spam",
-                "eggs",
-                "bucket",
-                "zone",
-                "cluster_id",
-                False,
-                None,
-                None,
-                lambda: cli_experiments,
+                project_id="spam",
+                dataset_id="eggs",
+                bucket="bucket",
+                zone="zone",
+                cluster_id="cluster_id",
+                monitor_status=False,
+                cluster_ip=None,
+                cluster_cert=None,
+                experiment_getter=lambda: cli_experiments,
+                analysis_periods=[
+                    AnalysisPeriod.DAY,
+                    AnalysisPeriod.WEEK,
+                    AnalysisPeriod.DAYS_28,
+                    AnalysisPeriod.OVERALL,
+                ],
             )
             run_date = dt.datetime(2020, 10, 31, tzinfo=UTC)
             strategy.execute([(config, run_date)])
 
             submit_workflow_mock.assert_called_once_with(
                 project_id="spam",
                 zone="zone",
                 cluster_id="cluster_id",
                 workflow_file=strategy.RUN_WORKFLOW,
                 parameters={
                     "experiments": [{"slug": "my_cool_experiment", "dates": ["2020-10-31"]}],
                     "project_id": "spam",
                     "dataset_id": "eggs",
                     "bucket": "bucket",
+                    "analysis_periods_day": "day",
+                    "analysis_periods_week": "week",
+                    "analysis_periods_days28": "days28",
+                    "analysis_periods_overall": "overall",
                 },
                 monitor_status=False,
                 cluster_ip=None,
                 cluster_cert=None,
             )
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_config.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         configs_collection = ConfigLoader
         assert configs_collection.configs is not None
         assert len(configs_collection.configs.configs) > 0
 
     def test_configs_from(self):
         loader = _ConfigLoader()
         configs_collection = loader.with_configs_from(
-            ["https://github.com/mozilla/jetstream-config"]
+            ["https://github.com/mozilla/metric-hub/tree/main/jetstream"]
         )
         assert configs_collection.configs is not None
         assert len(configs_collection.configs.configs) == len(loader.configs.configs)
 
     def test_spec_for_experiment(self):
         experiment = ConfigLoader.configs.configs[0].slug
         assert ConfigLoader.spec_for_experiment(experiment) is not None
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_experimenter.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_experimenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,26 +540,28 @@
     experiment_v6 = ExperimentV6(
         slug="test_slug",
         startDate=dt.datetime(2019, 1, 1),
         endDate=dt.datetime(2019, 1, 10),
         proposedEnrollment=14,
         branches=[Branch(slug="control", ratio=2), Branch(slug="treatment", ratio=1)],
         referenceBranch="control",
+        isEnrollmentPaused=True,
     )
 
     experiment = experiment_v6.to_experiment()
 
     assert experiment.experimenter_slug is None
     assert experiment.normandy_slug == "test_slug"
     assert experiment.status == "Complete"
     assert experiment.type == "v6"
     assert len(experiment.branches) == 2
     assert experiment.reference_branch == "control"
     assert experiment.is_high_population is False
     assert experiment.outcomes == []
+    assert experiment.is_enrollment_paused is True
 
 
 def test_fixture_validates():
     schema = json.loads((Path(__file__).parent / "data/NimbusExperiment_v1.0.json").read_text())
     experiments = json.loads(EXPERIMENTER_FIXTURE_V6)
     [jsonschema.validate(e, schema) for e in experiments if e["slug"]]
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_exposure_signal.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_metadata.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import jsonschema
 import requests
 import toml
 from metric_config_parser.analysis import AnalysisSpec
 from metric_config_parser.config import Outcome
 from metric_config_parser.outcome import OutcomeSpec
 
-from jetstream.config import DEFAULT_CONFIG_REPO, ConfigLoader, _ConfigLoader
+from jetstream.config import METRIC_HUB_REPO, ConfigLoader, _ConfigLoader
 from jetstream.metadata import ExperimentMetadata, export_metadata
 from jetstream.statistics import StatisticResult
 
 
 @patch.object(requests.Session, "get")
 def test_metadata_from_config(mock_get, experiments):
     config_str = dedent(
@@ -73,15 +73,16 @@
 
     spec = AnalysisSpec.from_dict(toml.loads(config_str))
     config = spec.resolve(experiments[4], ConfigLoader.configs)
     metadata = ExperimentMetadata.from_config(config)
 
     assert metadata.external_config.reference_branch == "a"
     assert (
-        metadata.external_config.url == DEFAULT_CONFIG_REPO + "/blob/main/normandy-test-slug.toml"
+        metadata.external_config.url
+        == METRIC_HUB_REPO + "/blob/main/jetstream/normandy-test-slug.toml"
     )
 
     config_str = dedent(
         """
         [metrics]
         weekly = ["view_about_logins"]
 
@@ -261,15 +262,15 @@
             "external_config": {
                 "end_date": "2021-07-01",
                 "enrollment_period": null,
                 "reference_branch": null,
                 "skip": false,
                 "start_date": null,
                 "url": """
-        + '"https://github.com/mozilla/jetstream-config/blob/main/normandy-test-slug.toml"'
+        + '"https://github.com/mozilla/metric-hub/blob/main/jetstream/normandy-test-slug.toml"'
         + r"""},
             "analysis_start_time": """
         + f'"{mock_analysis_start}"'
         + """,
             "schema_version":"""
         + str(StatisticResult.SCHEMA_VERSION)
         + """
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_metric.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_pretreatment.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_pretreatment.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,7 +70,15 @@
         pt = pre_treatment.ZeroFill()
         pd.testing.assert_frame_equal(example_data, pt.apply(example_data, "a"))
         example_data.loc[1, "a"] = np.nan
         example_data.loc[1, "b"] = np.nan
         ex1 = pt.apply(example_data, "a")
         assert ex1.loc[1, "a"] == 0
         assert np.isnan(ex1.loc[1, "b"])
+
+    def test_normalize_analysis_perioby_d(self, example_data):
+        pt = pre_treatment.NormalizeOverAnalysisPeriod(analysis_period_length=10)
+        ex1 = pt.apply(example_data, "a")
+        assert ex1.loc[0, "a"] == 1 / 10
+        assert ex1.loc[0, "b"] == 2
+        assert ex1.loc[2, "a"] == 1 / 2
+        assert ex1.loc[2, "b"] == 7
```

### Comparing `mozilla-jetstream-2023.1.0/jetstream/tests/test_statistics.py` & `mozilla-jetstream-2023.6.1/jetstream/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/util.py` & `mozilla-jetstream-2023.6.1/jetstream/util.py`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/jetstream/workflows/run.yaml` & `mozilla-jetstream-2023.6.1/jetstream/workflows/run.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 apiVersion: argoproj.io/v1alpha1
 kind: Workflow
 metadata:
   generateName: jetstream-
 spec:
   entrypoint: jetstream
+  ttlStrategy:
+    secondsAfterSuccess: 432000 # delete workflows automatically after 5 days
   arguments:
     parameters:
     - name: experiments  # set dynamically when worklfow gets deployed
     - name: project_id
     - name: dataset_id
     - name: bucket
+    - name: analysis_periods_day
+    - name: analysis_periods_week
+    - name: analysis_periods_days28
+    - name: analysis_periods_overall
   templates:
   - name: jetstream
     parallelism: 5  # run up to 5 containers in parallel at the same time
     inputs:
       parameters:
         - name: experiments
     steps:
@@ -68,20 +74,24 @@
     inputs:
       parameters:
       - name: date
       - name: slug
     container:
       image: gcr.io/moz-fx-data-experiments/jetstream:latest
       command: [
-        jetstream, --log_to_bigquery, run, 
-        "--date={{inputs.parameters.date}}", 
-        "--experiment_slug={{inputs.parameters.slug}}", 
+        jetstream, --log_to_bigquery, run,
+        "--date={{inputs.parameters.date}}",
+        "--experiment_slug={{inputs.parameters.slug}}",
         "--dataset_id={{workflow.parameters.dataset_id}}", 
         "--project_id={{workflow.parameters.project_id}}",
-        "--bucket={{workflow.parameters.bucket}}"
+        "--bucket={{workflow.parameters.bucket}}", 
+        "--analysis_periods={{workflow.parameters.analysis_periods_day}}",
+        "--analysis_periods={{workflow.parameters.analysis_periods_week}}",
+        "--analysis_periods={{workflow.parameters.analysis_periods_days28}}",
+        "--analysis_periods={{workflow.parameters.analysis_periods_overall}}"
       ]
       resources:
         requests:
           memory: 10Gi   # make sure there is at least 10Gb of memory available for the task
         limits:
           cpu: 4  # limit to 4 cores
     retryStrategy:
```

### Comparing `mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/PKG-INFO` & `mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mozilla-jetstream
-Version: 2023.1.0
+Version: 2023.6.1
 Summary: Runs a thing that analyzes experiments
 Home-page: https://github.com/mozilla/jetstream
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 [![CircleCI](https://circleci.com/gh/mozilla/jetstream/tree/main.svg?style=shield)](https://circleci.com/gh/mozilla/jetstream/tree/main)
 
 # jetstream
```

### Comparing `mozilla-jetstream-2023.1.0/mozilla_jetstream.egg-info/SOURCES.txt` & `mozilla-jetstream-2023.6.1/mozilla_jetstream.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 jetstream/experimenter.py
 jetstream/export_json.py
 jetstream/exposure_signal.py
 jetstream/metadata.py
 jetstream/metric.py
 jetstream/platform.py
 jetstream/pre_treatment.py
+jetstream/preview.py
 jetstream/segment.py
 jetstream/statistics.py
 jetstream/util.py
 jetstream/../platform_config.toml
 jetstream/../pyproject.toml
 jetstream/diagnostics/resource_profiling_plugin.py
 jetstream/diagnostics/task_monitoring_plugin.py
 jetstream/logging/__init__.py
 jetstream/logging/bigquery_log_handler.py
 jetstream/tests/__init__.py
 jetstream/tests/conftest.py
 jetstream/tests/test_analysis.py
 jetstream/tests/test_argo.py
+jetstream/tests/test_bigquery_client.py
 jetstream/tests/test_cli.py
 jetstream/tests/test_config.py
 jetstream/tests/test_experimenter.py
 jetstream/tests/test_exposure_signal.py
 jetstream/tests/test_metadata.py
 jetstream/tests/test_metric.py
 jetstream/tests/test_pretreatment.py
```

### Comparing `mozilla-jetstream-2023.1.0/platform_config.toml` & `mozilla-jetstream-2023.6.1/platform_config.toml`

 * *Files identical despite different names*

### Comparing `mozilla-jetstream-2023.1.0/setup.py` & `mozilla-jetstream-2023.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         "toml",
     ],
     include_package_data=True,
     tests_require=test_dependencies,
     extras_require=extras,
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
-    python_requires=">=3.6",
+    python_requires=">=3.10",
     entry_points="""
         [console_scripts]
         pensieve=jetstream.cli:cli
         jetstream=jetstream.cli:cli
     """,
     # This project does not issue releases, so this number is not meaningful
     # and should not need to change.
-    version="2023.1.0",
+    version="2023.6.1",
 )
```

