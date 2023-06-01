# Comparing `tmp/metaflow-2.9.2.tar.gz` & `tmp/metaflow-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-2.9.2.tar", last modified: Mon May 22 17:27:09 2023, max compression
+gzip compressed data, was "metaflow-2.9.3.tar", last modified: Thu Jun  1 19:08:09 2023, max compression
```

## Comparing `metaflow-2.9.2.tar` & `metaflow-2.9.3.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-22 17:26:56.000000 metaflow-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 17:26:56.000000 metaflow-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-22 17:27:09.194964 metaflow-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-22 17:26:56.000000 metaflow-2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.162963 metaflow-2.9.2/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.162963 metaflow-2.9.2/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33396 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18629 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31438 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)   103837 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.178964 metaflow-2.9.2/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.178964 metaflow-2.9.2/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.178964 metaflow-2.9.2/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.158963 metaflow-2.9.2/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.162963 metaflow-2.9.2/metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 17:27:09.194964 metaflow-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-22 17:26:56.000000 metaflow-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-01 19:07:53.000000 metaflow-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 19:07:53.000000 metaflow-2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-01 19:08:09.183644 metaflow-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-01 19:07:53.000000 metaflow-2.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.147644 metaflow-2.9.3/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.147644 metaflow-2.9.3/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.151644 metaflow-2.9.3/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.151644 metaflow-2.9.3/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.151644 metaflow-2.9.3/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.151644 metaflow-2.9.3/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.155644 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.155644 metaflow-2.9.3/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.155644 metaflow-2.9.3/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33396 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.155644 metaflow-2.9.3/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.155644 metaflow-2.9.3/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49461 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.159644 metaflow-2.9.3/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.159644 metaflow-2.9.3/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.159644 metaflow-2.9.3/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.163644 metaflow-2.9.3/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31438 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.163644 metaflow-2.9.3/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.163644 metaflow-2.9.3/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.163644 metaflow-2.9.3/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104651 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.163644 metaflow-2.9.3/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.163644 metaflow-2.9.3/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.167644 metaflow-2.9.3/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.167644 metaflow-2.9.3/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.167644 metaflow-2.9.3/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.167644 metaflow-2.9.3/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.171644 metaflow-2.9.3/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.171644 metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.171644 metaflow-2.9.3/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.171644 metaflow-2.9.3/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.171644 metaflow-2.9.3/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.175644 metaflow-2.9.3/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.175644 metaflow-2.9.3/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.175644 metaflow-2.9.3/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.175644 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.175644 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.175644 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.179644 metaflow-2.9.3/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.179644 metaflow-2.9.3/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.179644 metaflow-2.9.3/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19933 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.179644 metaflow-2.9.3/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.179644 metaflow-2.9.3/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.179644 metaflow-2.9.3/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.139644 metaflow-2.9.3/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.179644 metaflow-2.9.3/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.183644 metaflow-2.9.3/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-01 19:07:53.000000 metaflow-2.9.3/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:08:09.147644 metaflow-2.9.3/metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-01 19:08:09.000000 metaflow-2.9.3/metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-01 19:08:09.000000 metaflow-2.9.3/metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:08:09.000000 metaflow-2.9.3/metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 19:08:09.000000 metaflow-2.9.3/metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 19:08:09.000000 metaflow-2.9.3/metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 19:08:09.000000 metaflow-2.9.3/metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 19:08:09.187644 metaflow-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-01 19:07:53.000000 metaflow-2.9.3/setup.py
```

### Comparing `metaflow-2.9.2/LICENSE` & `metaflow-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/README.md` & `metaflow-2.9.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,94 @@
+Metadata-Version: 2.1
+Name: metaflow
+Version: 2.9.3
+Summary: Metaflow: More Data Science, Less Engineering
+Author: Metaflow Developers
+Author-email: help@metaflow.org
+License: Apache Software License
+Project-URL: Source, https://github.com/Netflix/metaflow
+Project-URL: Issues, https://github.com/Netflix/metaflow/issues
+Project-URL: Documentation, https://docs.metaflow.org
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![Metaflow_Logo_Horizontal_FullColor_Ribbon_Dark_RGB](https://user-images.githubusercontent.com/763451/89453116-96a57e00-d713-11ea-9fa6-82b29d4d6eff.png)
 
 # Metaflow
 
 Metaflow is a human-friendly library that helps scientists and engineers build and manage real-life data science projects. Metaflow was [originally developed at Netflix](https://netflixtechblog.com/open-sourcing-metaflow-a-human-centric-framework-for-data-science-fa72e04a5d9) to boost productivity of data scientists who work on a wide variety of projects from classical statistics to state-of-the-art deep learning.
 
 For more information, see [Metaflow's website](https://metaflow.org) and [documentation](https://docs.metaflow.org).
 
 ## From prototype to production (and back)
 
 Metaflow provides a simple, friendly API that covers foundational needs of ML, AI, and data science projects:
 <img src="./docs/prototype-to-prod.png" width="800px">
 
-1. Rapid local prototyping, support for notebooks, and built-in experiment tracking and versioning.
-2. Horizontal and vertical scalability to the cloud, utilizing both CPUs and GPUs, and fast data access.
-3. One-click deployments to highly available production orchestrators.
+1. [Rapid local prototyping](https://docs.metaflow.org/metaflow/basics), [support for notebooks](https://docs.metaflow.org/metaflow/visualizing-results), and [built-in experiment tracking and versioning](https://docs.metaflow.org/metaflow/client).
+2. [Horizontal and vertical scalability to the cloud](https://docs.metaflow.org/scaling/remote-tasks/introduction), utilizing both CPUs and GPUs, and [fast data access](https://docs.metaflow.org/scaling/data).
+3. [Managing dependencies](https://docs.metaflow.org/scaling/dependencies) and [one-click deployments to highly available production orchestrators](https://docs.metaflow.org/production/introduction).
 
 
 ## Getting started
 
-Getting up and running is easy. If you don't know where to start, click the link to get started in your [Metaflow sandbox](https://outerbounds.com/sandbox), where you can run code and explore Metaflow in seconds.
+Getting up and running is easy. If you don't know where to start, [Metaflow sandbox](https://outerbounds.com/sandbox) will have you running and exploring Metaflow in seconds.
 
 ### Installing Metaflow in your Python environment
 
-To install Metaflow into your local environment, you can install from [PyPi](https://pypi.org/project/metaflow/):
+To install Metaflow in your local environment, you can install from [PyPi](https://pypi.org/project/metaflow/):
 
 ```sh
 pip install metaflow
 ```
-Alternatively, you can install from [Conda](https://anaconda.org/conda-forge/metaflow):
+Alternatively, you can also install from [conda-forge](https://anaconda.org/conda-forge/metaflow):
 
 ```sh
 conda install -c conda-forge metaflow
 ```
+If you are eager to try out Metaflow in practice, you can start with the [tutorial](https://docs.metaflow.org/getting-started/tutorials). After the tutorial, you can learn more about how Metaflow works [here](https://docs.metaflow.org/metaflow/basics).
+
+### Deploying infrastructure for Metaflow in your cloud
+<img src="./docs/multicloud.png" width="800px">
+
 
-## Resources
+While you can get started with Metaflow easily on your laptop, the main benefits of Metaflow lie in its ability to [scale out to external compute clusters](https://docs.metaflow.org/scaling/remote-tasks/introduction) 
+and to [deploy to production-grade workflow orchestrators](https://docs.metaflow.org/production/introduction). To benefit from these features, follow this [guide](https://outerbounds.com/engineering/welcome/) to 
+configure Metaflow and the infrastructure behind it appropriately.
 
-### [Slack](http://slack.outerbounds.co/)
-An active community of data scientists and ML engineers discussing the ins-and-outs of applied machine learning. Get answers to your MLOps questions in minutes.
+## [Resources](https://docs.metaflow.org/introduction/metaflow-resources)
+
+### [Slack Community](http://slack.outerbounds.co/)
+An active [community](http://slack.outerbounds.co/) of thousands of data scientists and ML engineers discussing the ins-and-outs of applied machine learning.
 
 ### [Tutorials](https://outerbounds.com/docs/tutorials-index/)
-Demonstrations of Metaflow in real-world data science contexts. Beginner tutorials are linked below, and the budding Metaflow power user can find more advanced content by exploring [here](https://outerbounds.com/docs/tutorials-index/).
 - [Introduction to Metaflow](https://outerbounds.com/docs/intro-tutorial-overview/)
 - [Natural Language Processing with Metaflow](https://outerbounds.com/docs/nlp-tutorial-overview/)
 - [Computer Vision with Metaflow](https://outerbounds.com/docs/cv-tutorial-overview/)
 - [Recommender Systems with Metaflow](https://outerbounds.com/docs/recsys-tutorial-overview/)
+- And more advanced content [here](https://outerbounds.com/docs/tutorials-index/)
 
 ### [Generative AI and LLM use cases](https://outerbounds.com/blog/?category=Foundation%20Models)
+- [Infrastructure Stack for Large Language Models](https://outerbounds.com/blog/llm-infrastructure-stack/)
 - [Parallelizing Stable Diffusion for Production Use Cases](https://outerbounds.com/blog/parallelizing-stable-diffusion-production-use-cases/)
 - [Whisper with Metaflow on Kubernetes](https://outerbounds.com/blog/whisper-kubernetes/)
 - [Training a Large Language Model With Metaflow, Featuring Dolly](https://outerbounds.com/blog/train-dolly-metaflow/)
 
-### [Guides for data scientists](https://outerbounds.com/docs/data-science-welcome/)
-Short posts written to unblock data scientists without breaking their focus. Check [here](https://outerbounds.com/docs/data-science-welcome/) for answers to common Metaflow questions written in a Stack Overflow Q&A style.
-
-### Case studies and best practices
-
-This section is a sample of Metaflow content that will not be updated at high frequency. To find the latest Metaflow case studies and best practices, head over to the [Outerbounds blog](https://outerbounds.com/blog/).
-
-| Post title | Patterns | Complimentary tools |
-| ---------- | -------- | ----- |
-| [Fast Data: Loading Tables From S3 At Lightning Speed](https://outerbounds.com/blog/metaflow-fast-data/) | Optimizing I/O for data transfer in ML systems | Apache Arrow |
-| [Case Study: MLOps for FinTech using Metaflow](https://outerbounds.com/blog/mlops-fin-tech/) | Versioning, CI/CD, and Why Metaflow? | Snowflake, TensorFlow, MLFlow, Optuna, Arize |
-| [Scaling Media ML at Netflix](https://netflixtechblog.com/scaling-media-machine-learning-at-netflix-f19b400243) | Feature store, Multi-GPU, Model Serving, Vector Search | Ray |
-| [Better Airflow with Metaflow](https://outerbounds.com/blog/better-airflow-with-metaflow/) | ML Orchestration, Data Engineering Workflows | Airflow |
-| [Accelerating ML at CNN](https://medium.com/cnn-digital/accelerating-ml-within-cnn-983f6b7bd2eb) | ML experimentation platform | AWS Batch, Terraform | 
-| [Developing Safe and Reliable ML products at 23andMe](https://medium.com/23andme-engineering/machine-learning-eeee69d40736) | Privacy, compliance, data security, and testing ML systems | MLFlow, Jenkins, AWS Fargate |
-| [Case Study: MLOps for NLP-powered Media Intelligence using Metaflow](https://outerbounds.com/blog/mlops-media-intelligence/) | Testing, optimizing, and deploying ML workflows | HuggingFace, Neptune, Gradio, PyTorch, ONNX |
-| [Machine Learning with the Modern Data Stack: A Case Study](https://outerbounds.com/blog/modern-data-stack-mlops/) | End-to-end ML with Python and SQL | dbt, Snowflake, CometML, Sagemaker | 
-
-### [Metaflow Deployment Guides](https://outerbounds.com/engineering/welcome/)
-<img src="./docs/multicloud.png" width="800px">
-
-To set up and operate the full stack of ML/data science infrastructure for Metaflow on your own infrastructure, see these [guides for engineers](https://outerbounds.com/engineering/welcome/). This link will help you navigate the decision for deploying Metaflow in your organization's cloud accounts. 
-
-If you are looking for a managed Metaflow offering, see the [Outerbounds platform](https://outerbounds.com/platform/).
-
-### [Effective Data Science Infrastructure: How to make data scientists productive](https://www.manning.com/books/effective-data-science-infrastructure)
-A book about data science infrastructure, with many Metaflow tales included! You can find all code examples in [this repository](https://github.com/outerbounds/dsbook). 
-
-### Get in touch
+## Get in touch
 There are several ways to get in touch with us:
-- [Slack](http://slack.outerbounds.co/)
-- Open an issue at: https://github.com/Netflix/metaflow 
+- [Slack Community](http://slack.outerbounds.co/)
+- [Github Issues](https://github.com/Netflix/metaflow/issues)
 
 ## Contributing
-
 We welcome contributions to Metaflow. Please see our [contribution guide](https://docs.metaflow.org/introduction/contributing-to-metaflow) for more details.
```

### Comparing `metaflow-2.9.2/metaflow/R.py` & `metaflow-2.9.3/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/__init__.py` & `metaflow-2.9.3/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/__init__.py` & `metaflow-2.9.3/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/_bashcomplete.py` & `metaflow-2.9.3/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/_compat.py` & `metaflow-2.9.3/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/_termui_impl.py` & `metaflow-2.9.3/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/_textwrap.py` & `metaflow-2.9.3/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/_unicodefun.py` & `metaflow-2.9.3/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/_winconsole.py` & `metaflow-2.9.3/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/core.py` & `metaflow-2.9.3/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/decorators.py` & `metaflow-2.9.3/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/exceptions.py` & `metaflow-2.9.3/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/formatting.py` & `metaflow-2.9.3/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/globals.py` & `metaflow-2.9.3/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/parser.py` & `metaflow-2.9.3/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/termui.py` & `metaflow-2.9.3/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/testing.py` & `metaflow-2.9.3/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/types.py` & `metaflow-2.9.3/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/click/utils.py` & `metaflow-2.9.3/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `metaflow-2.9.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `metaflow-2.9.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_5/zipp.py` & `metaflow-2.9.3/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/typing_extensions.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/_vendor/v3_6/zipp.py` & `metaflow-2.9.3/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/cli.py` & `metaflow-2.9.3/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/cli_args.py` & `metaflow-2.9.3/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/client/core.py` & `metaflow-2.9.3/metaflow/client/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/client/filecache.py` & `metaflow-2.9.3/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/cmd/configure_cmd.py` & `metaflow-2.9.3/metaflow/cmd/configure_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/cmd/main_cli.py` & `metaflow-2.9.3/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/cmd/tutorials_cmd.py` & `metaflow-2.9.3/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/cmd_with_io.py` & `metaflow-2.9.3/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/current.py` & `metaflow-2.9.3/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/datastore/content_addressed_store.py` & `metaflow-2.9.3/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/datastore/datastore_set.py` & `metaflow-2.9.3/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/datastore/datastore_storage.py` & `metaflow-2.9.3/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/datastore/flow_datastore.py` & `metaflow-2.9.3/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/datastore/task_datastore.py` & `metaflow-2.9.3/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/debug.py` & `metaflow-2.9.3/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/decorators.py` & `metaflow-2.9.3/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/event_logger.py` & `metaflow-2.9.3/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/events.py` & `metaflow-2.9.3/metaflow/events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/exception.py` & `metaflow-2.9.3/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/extension_support/__init__.py` & `metaflow-2.9.3/metaflow/extension_support/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,27 +380,32 @@
     meta_to_pkg = defaultdict(list)
 
     # 1st step: look for distributions (the common case)
     for dist in metadata.distributions():
         if any(
             [pkg == EXT_PKG for pkg in (dist.read_text("top_level.txt") or "").split()]
         ):
+            # In all cases (whether duplicate package or not), we remove the package
+            # from the list of locations to look in.
+            # This is not 100% accurate because it is possible that at the same
+            # location there is a package and a non-package, but this is extremely
+            # unlikely so we are going to ignore this case.
+            dist_root = dist.locate_file(EXT_PKG).as_posix()
+            all_paths.discard(dist_root)
+
             if dist.metadata["Name"] in mf_ext_packages:
                 _ext_debug(
                     "Ignoring duplicate package '%s' (duplicate paths in sys.path? (%s))"
                     % (dist.metadata["Name"], str(sys.path))
                 )
                 continue
-            _ext_debug("Found extension package '%s'..." % dist.metadata["Name"])
-
-            # Remove the path from the paths to search. This is not 100% accurate because
-            # it is possible that at that same location there is a package and a non-package,
-            # but it is exceedingly unlikely, so we are going to ignore this.
-            dist_root = dist.locate_file(EXT_PKG).as_posix()
-            all_paths.discard(dist_root)
+            _ext_debug(
+                "Found extension package '%s' at '%s'..."
+                % (dist.metadata["Name"], dist_root)
+            )
 
             files_to_include = []
             meta_module = None
 
             # At this point, we check to see what extension points this package
             # contributes to. This is to enable multiple namespace packages to contribute
             # to the same extension point (for example, you may have multiple packages
```

### Comparing `metaflow-2.9.2/metaflow/extension_support/cmd.py` & `metaflow-2.9.3/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/extension_support/integrations.py` & `metaflow-2.9.3/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/extension_support/plugins.py` & `metaflow-2.9.3/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/flowspec.py` & `metaflow-2.9.3/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/graph.py` & `metaflow-2.9.3/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/includefile.py` & `metaflow-2.9.3/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/integrations.py` & `metaflow-2.9.3/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/lint.py` & `metaflow-2.9.3/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/metadata/heartbeat.py` & `metaflow-2.9.3/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/metadata/metadata.py` & `metaflow-2.9.3/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/metadata/util.py` & `metaflow-2.9.3/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/metaflow_config.py` & `metaflow-2.9.3/metaflow/metaflow_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,16 @@
 # Default node selectors to use by K8S jobs created by Metaflow - foo=bar,baz=bab
 KUBERNETES_NODE_SELECTOR = from_conf("KUBERNETES_NODE_SELECTOR", "")
 KUBERNETES_TOLERATIONS = from_conf("KUBERNETES_TOLERATIONS", "")
 KUBERNETES_PERSISTENT_VOLUME_CLAIMS = from_conf(
     "KUBERNETES_PERSISTENT_VOLUME_CLAIMS", ""
 )
 KUBERNETES_SECRETS = from_conf("KUBERNETES_SECRETS", "")
+# Default labels for kubernetes pods
+KUBERNETES_LABELS = from_conf("KUBERNETES_LABELS", "")
 # Default GPU vendor to use by K8S jobs created by Metaflow (supports nvidia, amd)
 KUBERNETES_GPU_VENDOR = from_conf("KUBERNETES_GPU_VENDOR", "nvidia")
 # Default container image for K8S
 KUBERNETES_CONTAINER_IMAGE = from_conf(
     "KUBERNETES_CONTAINER_IMAGE", DEFAULT_CONTAINER_IMAGE
 )
 # Image pull policy for container images
```

### Comparing `metaflow-2.9.2/metaflow/metaflow_config_funcs.py` & `metaflow-2.9.3/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/metaflow_environment.py` & `metaflow-2.9.3/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/metaflow_version.py` & `metaflow-2.9.3/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/mflog/__init__.py` & `metaflow-2.9.3/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/mflog/mflog.py` & `metaflow-2.9.3/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/mflog/save_logs.py` & `metaflow-2.9.3/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/mflog/save_logs_periodically.py` & `metaflow-2.9.3/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/mflog/tee.py` & `metaflow-2.9.3/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/monitor.py` & `metaflow-2.9.3/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/multicore_utils.py` & `metaflow-2.9.3/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/package.py` & `metaflow-2.9.3/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/parameters.py` & `metaflow-2.9.3/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/__init__.py` & `metaflow-2.9.3/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/airflow/airflow.py` & `metaflow-2.9.3/metaflow/plugins/airflow/airflow.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/airflow/airflow_cli.py` & `metaflow-2.9.3/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/airflow/airflow_decorator.py` & `metaflow-2.9.3/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/airflow/airflow_utils.py` & `metaflow-2.9.3/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/airflow/plumbing/set_parameters.py` & `metaflow-2.9.3/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/airflow/sensors/base_sensor.py` & `metaflow-2.9.3/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `metaflow-2.9.3/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/airflow/sensors/s3_sensor.py` & `metaflow-2.9.3/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/argo/argo_client.py` & `metaflow-2.9.3/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/argo/argo_events.py` & `metaflow-2.9.3/metaflow/plugins/argo/argo_events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/argo/argo_workflows.py` & `metaflow-2.9.3/metaflow/plugins/argo/argo_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,24 +26,29 @@
     DATASTORE_SYSROOT_AZURE,
     DATASTORE_SYSROOT_GS,
     DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
     DEFAULT_METADATA,
     DEFAULT_SECRETS_BACKEND_TYPE,
     KUBERNETES_FETCH_EC2_METADATA,
+    KUBERNETES_LABELS,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
     KUBERNETES_SECRETS,
     S3_ENDPOINT_URL,
     SERVICE_HEADERS,
     SERVICE_INTERNAL_URL,
 )
 from metaflow.mflog import BASH_SAVE_LOGS, bash_capture_logs, export_mflog_env_vars
 from metaflow.parameters import deploy_time_eval
+from metaflow.plugins.kubernetes.kubernetes import (
+    parse_kube_keyvalue_list,
+    validate_kube_labels,
+)
 from metaflow.util import (
     compress_list,
     dict_to_cli_options,
     to_bytes,
     to_camelcase,
     to_unicode,
 )
@@ -142,14 +147,15 @@
         self.notify_on_success = notify_on_success
         self.notify_slack_webhook_url = notify_slack_webhook_url
 
         self.parameters = self._process_parameters()
         self.triggers, self.trigger_options = self._process_triggers()
         self._schedule, self._timezone = self._get_schedule()
 
+        self.kubernetes_labels = self._get_kubernetes_labels()
         self._workflow_template = self._compile_workflow_template()
         self._sensor = self._compile_sensor()
 
     def __str__(self):
         return str(self._workflow_template)
 
     def deploy(self):
@@ -197,14 +203,27 @@
         try:
             return ArgoClient(namespace=KUBERNETES_NAMESPACE).trigger_workflow_template(
                 name, parameters
             )
         except Exception as e:
             raise ArgoWorkflowsException(str(e))
 
+    @staticmethod
+    def _get_kubernetes_labels():
+        """
+        Get Kubernetes labels from environment variable.
+        Parses the string into a dict and validates that values adhere to Kubernetes restrictions.
+        """
+        if not KUBERNETES_LABELS:
+            return {}
+        env_labels = KUBERNETES_LABELS.split(",")
+        env_labels = parse_kube_keyvalue_list(env_labels, False)
+        validate_kube_labels(env_labels)
+        return env_labels
+
     def _get_schedule(self):
         schedule = self.flow._flow_decorators.get("schedule")
         if schedule:
             # Remove the field "Year" if it exists
             schedule = schedule[0]
             return " ".join(schedule.schedule.split()[:5]), schedule.timezone
         return None, None
@@ -553,14 +572,15 @@
                 )
                 # Set common pod metadata.
                 .pod_metadata(
                     Metadata()
                     .label("app.kubernetes.io/name", "metaflow-task")
                     .label("app.kubernetes.io/part-of", "metaflow")
                     .annotations(annotations)
+                    .labels(self.kubernetes_labels)
                 )
                 # Set the entrypoint to flow name
                 .entrypoint(self.flow.name)
                 # Set exit hook handlers if notifications are enabled
                 .hooks(
                     {
                         **(
@@ -1168,14 +1188,15 @@
                     "tmpfs-ephemeral-volume",
                     medium="Memory",
                     size_limit=tmpfs_size if tmpfs_enabled else 0,
                 )
                 .pvc_volumes(resources.get("persistent_volume_claims"))
                 # Set node selectors
                 .node_selectors(resources.get("node_selector"))
+                # Set tolerations
                 .tolerations(resources.get("tolerations"))
                 # Set container
                 .container(
                     # TODO: Unify the logic with kubernetes.py
                     # Important note - Unfortunately, V1Container uses snakecase while
                     # Argo Workflows uses camel. For most of the attributes, both cases
                     # are indistinguishable, but unfortunately, not for all - (
@@ -1446,14 +1467,15 @@
             .metadata(
                 # Sensor metadata.
                 ObjectMeta()
                 .name(self.name.replace(".", "-"))
                 .namespace(KUBERNETES_NAMESPACE)
                 .label("app.kubernetes.io/name", "metaflow-sensor")
                 .label("app.kubernetes.io/part-of", "metaflow")
+                .labels(self.kubernetes_labels)
                 .annotations(annotations)
             )
             .spec(
                 SensorSpec().template(
                     # Sensor template.
                     SensorTemplate()
                     .metadata(
@@ -1731,15 +1753,15 @@
     def label(self, key, value):
         self.payload["labels"][key] = str(value)
         return self
 
     def labels(self, labels):
         if "labels" not in self.payload:
             self.payload["labels"] = {}
-        self.payload["labels"].update(labels)
+        self.payload["labels"].update(labels or {})
         return self
 
     def name(self, name):
         self.payload["name"] = name
         return self
 
     def namespace(self, namespace):
@@ -1848,15 +1870,15 @@
     def label(self, key, value):
         self.payload["labels"][key] = str(value)
         return self
 
     def labels(self, labels):
         if "labels" not in self.payload:
             self.payload["labels"] = {}
-        self.payload["labels"].update(labels)
+        self.payload["labels"].update(labels or {})
         return self
 
     def labels_from(self, labels_from):
         # Only available in workflow_metadata
         # https://github.com/argoproj/argo-workflows/blob/master/examples/label-value-from-workflow.yaml
         if "labelsFrom" not in self.payload:
             self.payload["labelsFrom"] = {}
```

### Comparing `metaflow-2.9.2/metaflow/plugins/argo/argo_workflows_cli.py` & `metaflow-2.9.3/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/argo/argo_workflows_decorator.py` & `metaflow-2.9.3/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/argo/process_input_paths.py` & `metaflow-2.9.3/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/aws_client.py` & `metaflow-2.9.3/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/aws_utils.py` & `metaflow-2.9.3/metaflow/plugins/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/batch/batch.py` & `metaflow-2.9.3/metaflow/plugins/aws/batch/batch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/batch/batch_cli.py` & `metaflow-2.9.3/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/batch/batch_client.py` & `metaflow-2.9.3/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/batch/batch_decorator.py` & `metaflow-2.9.3/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `metaflow-2.9.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/production_token.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_client.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `metaflow-2.9.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/azure/azure_tail.py` & `metaflow-2.9.3/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/azure/azure_utils.py` & `metaflow-2.9.3/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/azure/blob_service_client_factory.py` & `metaflow-2.9.3/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/azure/includefile_support.py` & `metaflow-2.9.3/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_cli.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_client.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_datastore.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_decorator.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/__init__.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/base.html` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/basic.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/bundle.css` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/card.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/main.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/components.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/main.js` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/renderer_tools.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_modules/test_cards.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/card_resolver.py` & `metaflow-2.9.3/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/component_serializer.py` & `metaflow-2.9.3/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/cards/exception.py` & `metaflow-2.9.3/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/catch_decorator.py` & `metaflow-2.9.3/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/conda/__init__.py` & `metaflow-2.9.3/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/conda/batch_bootstrap.py` & `metaflow-2.9.3/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/conda/conda.py` & `metaflow-2.9.3/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/conda/conda_environment.py` & `metaflow-2.9.3/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/conda/conda_flow_decorator.py` & `metaflow-2.9.3/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/conda/conda_step_decorator.py` & `metaflow-2.9.3/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datastores/azure_storage.py` & `metaflow-2.9.3/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datastores/gs_storage.py` & `metaflow-2.9.3/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datastores/local_storage.py` & `metaflow-2.9.3/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datastores/s3_storage.py` & `metaflow-2.9.3/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datatools/__init__.py` & `metaflow-2.9.3/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datatools/local.py` & `metaflow-2.9.3/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datatools/s3/s3.py` & `metaflow-2.9.3/metaflow/plugins/datatools/s3/s3.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datatools/s3/s3op.py` & `metaflow-2.9.3/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datatools/s3/s3tail.py` & `metaflow-2.9.3/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/datatools/s3/s3util.py` & `metaflow-2.9.3/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/debug_logger.py` & `metaflow-2.9.3/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/debug_monitor.py` & `metaflow-2.9.3/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/__init__.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/client.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,20 +81,25 @@
         )
 
         # Read override configuration
         # We can't just import the "overrides" module because that does not
         # distinguish it from other modules named "overrides" (either a third party
         # lib -- there is one -- or just other escaped modules). We therefore load
         # a fuller path to distinguish them from one another.
+        # We insert in sys.path a prefix that doesn't go up past metaflow/metaflow_extensions
+        # because overrides may import other modules and we want to make sure we
+        # don't "leak" things from the outside environment.
         pkg_components = []
         prefix, last_basename = os.path.split(config_dir)
-        while last_basename not in ("metaflow", "metaflow_extensions"):
+        while True:
             pkg_components.append(last_basename)
-            prefix, last_basename = os.path.split(prefix)
-        pkg_components.append(last_basename)
+            possible_prefix, last_basename = os.path.split(prefix)
+            if last_basename in ("metaflow", "metaflow_extensions"):
+                break
+            prefix = possible_prefix
 
         try:
             sys.path.insert(0, prefix)
             override_module = importlib.import_module(
                 ".overrides", package=".".join(reversed(pkg_components))
             )
             override_values = override_module.__dict__.values()
```

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/client_modules.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/communication/bytestream.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/communication/channel.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/communication/utils.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/consts.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/data_transferer.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/exception_transferer.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/override_decorators.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/server.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/stub.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/env_escape/utils.py` & `metaflow-2.9.3/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/environment_decorator.py` & `metaflow-2.9.3/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/events_decorator.py` & `metaflow-2.9.3/metaflow/plugins/events_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/frameworks/pytorch.py` & `metaflow-2.9.3/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/gcp/gs_storage_client_factory.py` & `metaflow-2.9.3/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/gcp/gs_tail.py` & `metaflow-2.9.3/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/gcp/gs_utils.py` & `metaflow-2.9.3/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/gcp/includefile_support.py` & `metaflow-2.9.3/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes.py` & `metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 import math
 import os
+import re
 import shlex
 import time
+from typing import Dict, List, Optional
 
 from metaflow import current, util
 from metaflow.exception import MetaflowException
 from metaflow.metaflow_config import (
     ARGO_EVENTS_EVENT,
     ARGO_EVENTS_EVENT_BUS,
     ARGO_EVENTS_EVENT_SOURCE,
@@ -21,14 +23,15 @@
     DATASTORE_SYSROOT_GS,
     DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
     DEFAULT_AWS_CLIENT_PROVIDER,
     DEFAULT_METADATA,
     DEFAULT_SECRETS_BACKEND_TYPE,
     KUBERNETES_FETCH_EC2_METADATA,
+    KUBERNETES_LABELS,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
     S3_ENDPOINT_URL,
     SERVICE_HEADERS,
     SERVICE_INTERNAL_URL,
 )
 from metaflow.mflog import (
     BASH_SAVE_LOGS,
@@ -159,14 +162,15 @@
         tmpfs_tempdir=None,
         tmpfs_size=None,
         tmpfs_path=None,
         run_time_limit=None,
         env=None,
         persistent_volume_claims=None,
         tolerations=None,
+        labels=None,
     ):
         if env is None:
             env = {}
 
         job = (
             KubernetesClient()
             .job(
@@ -192,14 +196,15 @@
                 gpu=gpu,
                 gpu_vendor=gpu_vendor,
                 timeout_in_seconds=run_time_limit,
                 # Retries are handled by Metaflow runtime
                 retries=0,
                 step_name=step_name,
                 tolerations=tolerations,
+                labels=self._get_labels(labels),
                 use_tmpfs=use_tmpfs,
                 tmpfs_tempdir=tmpfs_tempdir,
                 tmpfs_size=tmpfs_size,
                 tmpfs_path=tmpfs_path,
                 persistent_volume_claims=persistent_volume_claims,
             )
             .environment_variable("METAFLOW_CODE_SHA", code_package_sha)
@@ -390,7 +395,64 @@
 
         exit_code, _ = self._job.reason
         echo(
             "Task finished with exit code %s." % exit_code,
             "stderr",
             job_id=self._job.id,
         )
+
+    @staticmethod
+    def _get_labels(extra_labels=None):
+        if extra_labels is None:
+            extra_labels = {}
+        env_labels = KUBERNETES_LABELS.split(",") if KUBERNETES_LABELS else []
+        env_labels = parse_kube_keyvalue_list(env_labels, False)
+        labels = {**env_labels, **extra_labels}
+        validate_kube_labels(labels)
+        return labels
+
+
+def validate_kube_labels(
+    labels: Optional[Dict[str, Optional[str]]],
+) -> bool:
+    """Validate label values.
+
+    This validates the kubernetes label values.  It does not validate the keys.
+    Ideally, keys should be static and also the validation rules for keys are
+    more complex than those for values.  For full validation rules, see:
+
+    https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#syntax-and-character-set
+    """
+
+    def validate_label(s: Optional[str]):
+        regex_match = r"^(([A-Za-z0-9][-A-Za-z0-9_.]{0,61})?[A-Za-z0-9])?$"
+        if not s:
+            # allow empty label
+            return True
+        if not re.search(regex_match, s):
+            raise KubernetesException(
+                'Invalid value: "%s"\n'
+                "A valid label must be an empty string or one that\n"
+                "  - Consist of alphanumeric, '-', '_' or '.' characters\n"
+                "  - Begins and ends with an alphanumeric character\n"
+                "  - Is at most 63 characters" % s
+            )
+        return True
+
+    return all([validate_label(v) for v in labels.values()]) if labels else True
+
+
+def parse_kube_keyvalue_list(items: List[str], requires_both: bool = True):
+    try:
+        ret = {}
+        for item_str in items:
+            item = item_str.split("=", 1)
+            if requires_both:
+                item[1]  # raise IndexError
+            if str(item[0]) in ret:
+                raise KubernetesException("Duplicate key found: %s" % str(item[0]))
+            ret[str(item[0])] = str(item[1]) if len(item) > 1 else None
+        return ret
+    except KubernetesException as e:
+        raise e
+    except (AttributeError, IndexError):
+        raise KubernetesException("Unable to parse kubernetes list: %s" % items)
```

### Comparing `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_cli.py` & `metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import sys
 import time
 import traceback
 
-from metaflow import util, JSONTypeClass
+from metaflow import JSONTypeClass, util
 from metaflow._vendor import click
 from metaflow.exception import METAFLOW_EXIT_DISALLOW_RETRY, CommandException
 from metaflow.metadata.util import sync_local_metadata_from_datastore
-from metaflow.metaflow_config import DATASTORE_LOCAL_DIR
+from metaflow.metaflow_config import DATASTORE_LOCAL_DIR, KUBERNETES_LABELS
 from metaflow.mflog import TASK_LOG_SOURCE
 
-from .kubernetes import Kubernetes, KubernetesKilledException
+from .kubernetes import Kubernetes, KubernetesKilledException, parse_kube_keyvalue_list
 from .kubernetes_decorator import KubernetesDecorator
 
 
 @click.group()
 def cli():
     pass
 
@@ -191,15 +191,15 @@
         task_id=kwargs["task_id"],
         attempt=int(retry_count),
     )
     stdout_location = ds.get_log_location(TASK_LOG_SOURCE, "stdout")
     stderr_location = ds.get_log_location(TASK_LOG_SOURCE, "stderr")
 
     # `node_selector` is a tuple of strings, convert it to a dictionary
-    node_selector = KubernetesDecorator.parse_node_selector(node_selector)
+    node_selector = parse_kube_keyvalue_list(node_selector)
 
     def _sync_metadata():
         if ctx.obj.metadata.TYPE == "local":
             sync_local_metadata_from_datastore(
                 DATASTORE_LOCAL_DIR,
                 ctx.obj.flow_datastore.get_task_datastore(
                     kwargs["run_id"], step_name, kwargs["task_id"]
```

### Comparing `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_client.py` & `metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,31 +8,29 @@
 from metaflow.exception import MetaflowException
 from metaflow.metadata import MetaDatum
 from metaflow.metadata.util import sync_local_metadata_to_datastore
 from metaflow.metaflow_config import (
     DATASTORE_LOCAL_DIR,
     KUBERNETES_CONTAINER_IMAGE,
     KUBERNETES_CONTAINER_REGISTRY,
+    KUBERNETES_FETCH_EC2_METADATA,
     KUBERNETES_IMAGE_PULL_POLICY,
     KUBERNETES_GPU_VENDOR,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
+    KUBERNETES_PERSISTENT_VOLUME_CLAIMS,
     KUBERNETES_TOLERATIONS,
     KUBERNETES_SERVICE_ACCOUNT,
-    KUBERNETES_SECRETS,
-    KUBERNETES_FETCH_EC2_METADATA,
-    KUBERNETES_PERSISTENT_VOLUME_CLAIMS,
 )
 from metaflow.plugins.resources_decorator import ResourcesDecorator
 from metaflow.plugins.timeout_decorator import get_run_time_limit_for_task
 from metaflow.sidecar import Sidecar
 
 from ..aws.aws_utils import get_docker_registry, get_ec2_instance_metadata
-
-from .kubernetes import KubernetesException
+from .kubernetes import KubernetesException, parse_kube_keyvalue_list
 
 try:
     unicode
 except NameError:
     unicode = str
     basestring = str
 
@@ -74,14 +72,17 @@
         sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
     tmpfs_size: int, optional
         The value for the size (in MiB) of the tmpfs mount for this step.
         This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
         memory allocated for this step.
     tmpfs_path: string, optional
         Path to tmpfs mount for this step. Defaults to /metaflow_temp.
+    persistent_volume_claims: Dict[str, str], optional
+        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
+        volumes to the path to which the volume is to be mounted, e.g., { "pvc-name": "/path/to/mount/on" }.
     """
 
     name = "kubernetes"
     defaults = {
         "cpu": "1",
         "memory": "4096",
         "disk": "10240",
@@ -125,15 +126,15 @@
             self.attributes["persistent_volume_claims"] = json.loads(
                 KUBERNETES_PERSISTENT_VOLUME_CLAIMS
             )
         if not self.attributes["image_pull_policy"] and KUBERNETES_IMAGE_PULL_POLICY:
             self.attributes["image_pull_policy"] = KUBERNETES_IMAGE_PULL_POLICY
 
         if isinstance(self.attributes["node_selector"], str):
-            self.attributes["node_selector"] = self.parse_node_selector(
+            self.attributes["node_selector"] = parse_kube_keyvalue_list(
                 self.attributes["node_selector"].split(",")
             )
 
         if self.attributes["tolerations"]:
             try:
                 from kubernetes.client import V1Toleration
 
@@ -322,18 +323,19 @@
             cli_args.command_args.append(self.package_url)
 
             # --namespace is used to specify Metaflow namespace (a different
             # concept from k8s namespace).
             for k, v in self.attributes.items():
                 if k == "namespace":
                     cli_args.command_options["k8s_namespace"] = v
-                elif k == "node_selector" and v:
-                    cli_args.command_options[k] = ",".join(
-                        ["=".join([key, str(val)]) for key, val in v.items()]
-                    )
+                elif k in {"node_selector"} and v:
+                    cli_args.command_options[k] = [
+                        "=".join([key, str(val)]) if val else key
+                        for key, val in v.items()
+                    ]
                 elif k in ["tolerations", "persistent_volume_claims"]:
                     cli_args.command_options[k] = json.dumps(v)
                 else:
                     cli_args.command_options[k] = v
             cli_args.command_options["run-time-limit"] = self.run_time_limit
             cli_args.entrypoint[0] = sys.executable
 
@@ -437,19 +439,7 @@
 
     @classmethod
     def _save_package_once(cls, flow_datastore, package):
         if cls.package_url is None:
             cls.package_url, cls.package_sha = flow_datastore.save_data(
                 [package.blob], len_hint=1
             )[0]
-
-    @staticmethod
-    def parse_node_selector(node_selector: list):
-        try:
-            return {
-                str(k.split("=", 1)[0]): str(k.split("=", 1)[1])
-                for k in node_selector or []
-            }
-        except (AttributeError, IndexError):
-            raise KubernetesException(
-                "Unable to parse node_selector: %s" % node_selector
-            )
```

### Comparing `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_job.py` & `metaflow-2.9.3/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/metadata/local.py` & `metaflow-2.9.3/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/metadata/service.py` & `metaflow-2.9.3/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/package_cli.py` & `metaflow-2.9.3/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/parallel_decorator.py` & `metaflow-2.9.3/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/project_decorator.py` & `metaflow-2.9.3/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/resources_decorator.py` & `metaflow-2.9.3/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/retry_decorator.py` & `metaflow-2.9.3/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/secrets/secrets_decorator.py` & `metaflow-2.9.3/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/storage_executor.py` & `metaflow-2.9.3/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/tag_cli.py` & `metaflow-2.9.3/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/test_unbounded_foreach_decorator.py` & `metaflow-2.9.3/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/plugins/timeout_decorator.py` & `metaflow-2.9.3/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/procpoll.py` & `metaflow-2.9.3/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/pylint_wrapper.py` & `metaflow-2.9.3/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/runtime.py` & `metaflow-2.9.3/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/sidecar/sidecar.py` & `metaflow-2.9.3/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/sidecar/sidecar_messages.py` & `metaflow-2.9.3/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/sidecar/sidecar_subprocess.py` & `metaflow-2.9.3/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/sidecar/sidecar_worker.py` & `metaflow-2.9.3/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tagging_util.py` & `metaflow-2.9.3/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/task.py` & `metaflow-2.9.3/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/00-helloworld/helloworld.py` & `metaflow-2.9.3/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/01-playlist/README.md` & `metaflow-2.9.3/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/01-playlist/movies.csv` & `metaflow-2.9.3/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/01-playlist/playlist.ipynb` & `metaflow-2.9.3/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/01-playlist/playlist.py` & `metaflow-2.9.3/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/02-statistics/README.md` & `metaflow-2.9.3/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/02-statistics/movies.csv` & `metaflow-2.9.3/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/02-statistics/stats.ipynb` & `metaflow-2.9.3/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/02-statistics/stats.py` & `metaflow-2.9.3/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/README.md` & `metaflow-2.9.3/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/playlist.py` & `metaflow-2.9.3/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/README.md` & `metaflow-2.9.3/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/playlist.py` & `metaflow-2.9.3/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/README.md` & `metaflow-2.9.3/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `metaflow-2.9.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `metaflow-2.9.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/README.md` & `metaflow-2.9.3/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `metaflow-2.9.3/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/07-worldview/worldview.ipynb` & `metaflow-2.9.3/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/08-autopilot/README.md` & `metaflow-2.9.3/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `metaflow-2.9.3/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/util.py` & `metaflow-2.9.3/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow/vendor.py` & `metaflow-2.9.3/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/metaflow.egg-info/SOURCES.txt` & `metaflow-2.9.3/metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.2/setup.py` & `metaflow-2.9.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.9.2"
+version = "2.9.3"
 
 setup(
     include_package_data=True,
     name="metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

