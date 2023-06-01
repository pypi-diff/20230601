# Comparing `tmp/dagster-graphql-1.3.6.tar.gz` & `tmp/dagster-graphql-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.6.tar", last modified: Thu May 25 17:23:41 2023, max compression
+gzip compressed data, was "dagster-graphql-1.3.7.tar", last modified: Thu Jun  1 18:22:47 2023, max compression
```

## Comparing `dagster-graphql-1.3.6.tar` & `dagster-graphql-1.3.7.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.969202 dagster-graphql-1.3.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-25 17:23:41.969202 dagster-graphql-1.3.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.885201 dagster-graphql-1.3.6/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7442 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.889201 dagster-graphql-1.3.6/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17835 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.905202 dagster-graphql-1.3.6/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18592 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.909201 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11457 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8885 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4586 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7270 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25777 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12470 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    14972 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)     9554 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    21120 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8078 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.937202 dagster-graphql-1.3.6/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40571 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     4705 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16767 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18061 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16323 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10983 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28430 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.941202 dagster-graphql-1.3.6/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20983 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17622 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.957202 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11062 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39668 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.965202 dagster-graphql-1.3.6/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    25389 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    37776 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.965202 dagster-graphql-1.3.6/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8306 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29569 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.965202 dagster-graphql-1.3.6/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6364 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.889201 dagster-graphql-1.3.6/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4286 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-25 17:23:41.969202 dagster-graphql-1.3.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.821929 dagster-graphql-1.3.7/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-01 18:22:47.821929 dagster-graphql-1.3.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.749929 dagster-graphql-1.3.7/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.753929 dagster-graphql-1.3.7/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17963 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.769929 dagster-graphql-1.3.7/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.773929 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11422 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7270 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25777 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12470 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.801929 dagster-graphql-1.3.7/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40571 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     6280 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16867 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16323 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28430 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.801929 dagster-graphql-1.3.7/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.813929 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39668 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.817929 dagster-graphql-1.3.7/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    25389 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    37798 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.821929 dagster-graphql-1.3.7/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8306 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.821929 dagster-graphql-1.3.7/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6364 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.749929 dagster-graphql-1.3.7/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-01 18:22:47.825929 dagster-graphql-1.3.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/setup.py
```

### Comparing `dagster-graphql-1.3.6/LICENSE` & `dagster-graphql-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/PKG-INFO` & `dagster-graphql-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.6
+Version: 1.3.7
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/__init__.py` & `dagster-graphql-1.3.7/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/cli.py` & `dagster-graphql-1.3.7/dagster_graphql/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Mapping, Optional
 from urllib.parse import urljoin, urlparse
 
 import click
 import dagster._check as check
 import dagster._seven as seven
 import requests
+from dagster._cli.utils import get_instance_for_cli, get_temporary_instance_for_cli
 from dagster._cli.workspace import workspace_target_argument
 from dagster._cli.workspace.cli_target import (
     WORKSPACE_TARGET_WARNING,
     get_workspace_process_context_from_kwargs,
 )
-from dagster._core.instance import DagsterInstance
 from dagster._core.workspace.context import WorkspaceProcessContext
 from dagster._utils import DEFAULT_WORKSPACE_YAML_FILENAME
 from dagster._utils.log import get_stack_trace_array
 
 from .client.query import LAUNCH_PIPELINE_EXECUTION_MUTATION
 from .schema import create_schema
 from .version import __version__
@@ -193,15 +193,15 @@
         )
 
     if remote:
         res = execute_query_against_remote(remote, query, variables)
         print(res)  # noqa: T201
     else:
         with (
-            DagsterInstance.local_temp() if ephemeral_instance else DagsterInstance.get()
+            get_temporary_instance_for_cli() if ephemeral_instance else get_instance_for_cli()
         ) as instance:
             with get_workspace_process_context_from_kwargs(
                 instance, version=__version__, read_only=False, kwargs=kwargs
             ) as workspace_process_context:
                 execute_query_from_cli(
                     workspace_process_context,
                     query,
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/client/client.py` & `dagster-graphql-1.3.7/dagster_graphql/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from itertools import chain
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Union
 
 import dagster._check as check
 import requests.exceptions
 from dagster import DagsterRunStatus
 from dagster._annotations import public
+from dagster._core.definitions.run_config import RunConfig, convert_config_input
 from dagster._core.definitions.utils import validate_tags
 from dagster._utils.backcompat import experimental_class_warning
 from gql import Client, gql
 from gql.transport import Transport
 from gql.transport.requests import RequestsHTTPTransport
 
 from .client_queries import (
@@ -113,27 +114,27 @@
             raise DagsterGraphQLClientError(repo_connection_status, query_res["message"])
 
     def _core_submit_execution(
         self,
         pipeline_name: str,
         repository_location_name: Optional[str] = None,
         repository_name: Optional[str] = None,
-        run_config: Optional[Mapping[str, Any]] = None,
+        run_config: Optional[Union[RunConfig, Mapping[str, Any]]] = None,
         mode: str = "default",
         preset: Optional[str] = None,
         tags: Optional[Mapping[str, str]] = None,
         op_selection: Optional[Sequence[str]] = None,
         is_using_job_op_graph_apis: Optional[bool] = False,
     ):
         check.opt_str_param(repository_location_name, "repository_location_name")
         check.opt_str_param(repository_name, "repository_name")
         check.str_param(pipeline_name, "pipeline_name")
         check.opt_str_param(mode, "mode")
         check.opt_str_param(preset, "preset")
-        run_config = check.opt_mapping_param(run_config, "run_config")
+        run_config = check.opt_mapping_param(convert_config_input(run_config), "run_config")
 
         # The following invariant will never fail when a job is executed
         check.invariant(
             (mode is not None and run_config is not None) or preset is not None,
             (
                 "Either a mode and run_config or a preset must be specified in order to "
                 f"submit the pipeline {pipeline_name} for execution"
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.3.7/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/client/query.py` & `dagster-graphql-1.3.7/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/client/utils.py` & `dagster-graphql-1.3.7/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/events.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # re-exports
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey
 from dagster._core.events import EngineEventData
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.captured_log_manager import CapturedLogManager
 from dagster._core.storage.compute_log_manager import ComputeIOType, ComputeLogFileData
-from dagster._core.storage.dagster_run import DagsterRunStatus
+from dagster._core.storage.dagster_run import CANCELABLE_RUN_STATUSES
 from dagster._core.workspace.permissions import Permissions
 from dagster._utils.error import serializable_error_info_from_exc_info
 from starlette.concurrency import (
     run_in_threadpool,  # can provide this indirectly if we dont want starlette dep in dagster-graphql
 )
 
 if TYPE_CHECKING:
@@ -102,15 +102,15 @@
     if location_name:
         assert_permission_for_location(
             graphene_info, Permissions.TERMINATE_PIPELINE_EXECUTION, location_name
         )
     else:
         assert_permission(graphene_info, Permissions.TERMINATE_PIPELINE_EXECUTION)
 
-    can_cancel_run = run.status == DagsterRunStatus.STARTED or run.status == DagsterRunStatus.QUEUED
+    can_cancel_run = run.status in CANCELABLE_RUN_STATUSES
 
     valid_status = not run.is_finished and (force_mark_as_canceled or can_cancel_run)
 
     if not valid_status:
         return GrapheneTerminateRunFailure(
             run=graphene_run,
             message="Run {run_id} could not be terminated due to having status {status}.".format(
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/backfill.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,32 @@
         GrapheneCancelBackfillSuccess,
         GrapheneLaunchBackfillSuccess,
         GrapheneResumeBackfillSuccess,
     )
     from ...schema.errors import GraphenePartitionSetNotFoundError
 
 
+def _assert_permission_for_asset_graph(
+    graphene_info: "ResolveInfo", asset_graph: ExternalAssetGraph, permission: str
+) -> None:
+    location_names = set(
+        repo_handle.code_location_origin.location_name
+        for repo_handle in asset_graph.repository_handles_by_key.values()
+    )
+
+    if not location_names:
+        assert_permission(
+            graphene_info,
+            permission,
+        )
+    else:
+        for location_name in location_names:
+            assert_permission_for_location(graphene_info, permission, location_name)
+
+
 def create_and_launch_partition_backfill(
     graphene_info: "ResolveInfo",
     backfill_params: BackfillParams,
 ) -> Union["GrapheneLaunchBackfillSuccess", "GraphenePartitionSetNotFoundError"]:
     from ...schema.backfill import GrapheneLaunchBackfillSuccess
     from ...schema.errors import GraphenePartitionSetNotFoundError
 
@@ -132,31 +150,18 @@
                 "forceSynchronousSubmission is not supported for pure asset backfills"
             )
 
         if backfill_params.get("fromFailure"):
             raise DagsterError("fromFailure is not supported for pure asset backfills")
 
         asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
-
-        location_names = set(
-            repo_handle.code_location_origin.location_name
-            for repo_handle in asset_graph.repository_handles_by_key.values()
+        _assert_permission_for_asset_graph(
+            graphene_info, asset_graph, Permissions.LAUNCH_PARTITION_BACKFILL
         )
 
-        if not location_names:
-            assert_permission(
-                graphene_info,
-                Permissions.LAUNCH_PARTITION_BACKFILL,
-            )
-        else:
-            for location_name in location_names:
-                assert_permission_for_location(
-                    graphene_info, Permissions.LAUNCH_PARTITION_BACKFILL, location_name
-                )
-
         backfill = PartitionBackfill.from_asset_partitions(
             asset_graph=asset_graph,
             backfill_id=backfill_id,
             tags=tags,
             backfill_timestamp=backfill_timestamp,
             asset_selection=asset_selection,
             partition_names=backfill_params.get("partitionNames"),
@@ -179,21 +184,33 @@
 ) -> "GrapheneCancelBackfillSuccess":
     from ...schema.backfill import GrapheneCancelBackfillSuccess
 
     backfill = graphene_info.context.instance.get_backfill(backfill_id)
     if not backfill:
         check.failed(f"No backfill found for id: {backfill_id}")
 
-    partition_set_origin = check.not_none(backfill.partition_set_origin)
-    location_name = partition_set_origin.selector.location_name
-    assert_permission_for_location(
-        graphene_info, Permissions.CANCEL_PARTITION_BACKFILL, location_name
-    )
+    if backfill.serialized_asset_backfill_data:
+        asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
+        _assert_permission_for_asset_graph(
+            graphene_info, asset_graph, Permissions.CANCEL_PARTITION_BACKFILL
+        )
+        graphene_info.context.instance.update_backfill(
+            backfill.with_status(BulkActionStatus.CANCELING)
+        )
+
+    else:
+        partition_set_origin = check.not_none(backfill.partition_set_origin)
+        location_name = partition_set_origin.selector.location_name
+        assert_permission_for_location(
+            graphene_info, Permissions.CANCEL_PARTITION_BACKFILL, location_name
+        )
+        graphene_info.context.instance.update_backfill(
+            backfill.with_status(BulkActionStatus.CANCELED)
+        )
 
-    graphene_info.context.instance.update_backfill(backfill.with_status(BulkActionStatus.CANCELED))
     return GrapheneCancelBackfillSuccess(backfill_id=backfill_id)
 
 
 def resume_partition_backfill(
     graphene_info: "ResolveInfo", backfill_id: str
 ) -> "GrapheneResumeBackfillSuccess":
     from ...schema.backfill import GrapheneResumeBackfillSuccess
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/external.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.3.7/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.auto_materialize_condition import (
     AutoMaterializeCondition,
     AutoMaterializeDecisionType,
     DownstreamFreshnessAutoMaterializeCondition,
     FreshnessAutoMaterializeCondition,
+    MaxMaterializationsExceededAutoMaterializeCondition,
     MissingAutoMaterializeCondition,
     ParentMaterializedAutoMaterializeCondition,
     ParentOutdatedAutoMaterializeCondition,
 )
 from dagster._core.definitions.partition import SerializedPartitionsSubset
 from dagster._core.scheduler.instigation import AutoMaterializeAssetEvaluationRecord
 
+from dagster_graphql.schema.errors import GrapheneError
+
 from .util import non_null_list
 
 GrapheneAutoMaterializeDecisionType = graphene.Enum.from_enum(AutoMaterializeDecisionType)
 
 
 class GrapheneAutoMaterializeConditionWithDecisionType(graphene.Interface):
     decisionType = graphene.NonNull(GrapheneAutoMaterializeDecisionType)
@@ -52,23 +55,30 @@
 
 class GrapheneParentOutdatedAutoMaterializeCondition(graphene.ObjectType):
     class Meta:
         name = "ParentOutdatedAutoMaterializeCondition"
         interfaces = (GrapheneAutoMaterializeConditionWithDecisionType,)
 
 
+class GrapheneMaxMaterializationsExceededAutoMaterializeCondition(graphene.ObjectType):
+    class Meta:
+        name = "MaxMaterializationsExceededAutoMaterializeCondition"
+        interfaces = (GrapheneAutoMaterializeConditionWithDecisionType,)
+
+
 class GrapheneAutoMaterializeCondition(graphene.Union):
     class Meta:
         name = "AutoMaterializeCondition"
         types = (
             GrapheneFreshnessAutoMaterializeCondition,
             GrapheneDownstreamFreshnessAutoMaterializeCondition,
             GrapheneParentMaterializedAutoMaterializeCondition,
             GrapheneMissingAutoMaterializeCondition,
             GrapheneParentOutdatedAutoMaterializeCondition,
+            GrapheneMaxMaterializationsExceededAutoMaterializeCondition,
         )
 
 
 def create_graphene_auto_materialize_condition(
     condition_tuple: Tuple[AutoMaterializeCondition, Optional[SerializedPartitionsSubset]]
 ):
     condition, _ = condition_tuple
@@ -82,14 +92,18 @@
         return GrapheneParentMaterializedAutoMaterializeCondition(
             decisionType=condition.decision_type
         )
     elif isinstance(condition, MissingAutoMaterializeCondition):
         return GrapheneMissingAutoMaterializeCondition(decisionType=condition.decision_type)
     elif isinstance(condition, ParentOutdatedAutoMaterializeCondition):
         return GrapheneParentOutdatedAutoMaterializeCondition(decisionType=condition.decision_type)
+    elif isinstance(condition, MaxMaterializationsExceededAutoMaterializeCondition):
+        return GrapheneMaxMaterializationsExceededAutoMaterializeCondition(
+            decisionType=condition.decision_type
+        )
     else:
         check.failed(f"Unexpected condition type {type(condition)}")
 
 
 class GrapheneAutoMaterializeAssetEvaluationRecord(graphene.ObjectType):
     id = graphene.NonNull(graphene.ID)
     evaluationId = graphene.NonNull(graphene.Int)
@@ -111,7 +125,34 @@
             numDiscarded=record.evaluation.num_discarded,
             conditions=[
                 create_graphene_auto_materialize_condition(c)
                 for c in record.evaluation.partition_subsets_by_condition
             ],
             timestamp=record.timestamp,
         )
+
+
+class GrapheneAutoMaterializeAssetEvaluationRecords(graphene.ObjectType):
+    records = non_null_list(GrapheneAutoMaterializeAssetEvaluationRecord)
+
+    class Meta:
+        name = "AutoMaterializeAssetEvaluationRecords"
+
+    def __init__(self, records: List[AutoMaterializeAssetEvaluationRecord]):
+        super().__init__(records=records)
+
+
+class GrapheneAutoMaterializeAssetEvaluationNeedsMigrationError(graphene.ObjectType):
+    message = graphene.NonNull(graphene.String)
+
+    class Meta:
+        interfaces = (GrapheneError,)
+        name = "AutoMaterializeAssetEvaluationNeedsMigrationError"
+
+
+class GrapheneAutoMaterializeAssetEvaluationRecordsOrError(graphene.Union):
+    class Meta:
+        types = (
+            GrapheneAutoMaterializeAssetEvaluationRecords,
+            GrapheneAutoMaterializeAssetEvaluationNeedsMigrationError,
+        )
+        name = "AutoMaterializeAssetEvaluationRecordsOrError"
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,18 +4,20 @@
     AutoMaterializePolicy,
     AutoMaterializePolicyType,
 )
 
 
 class GrapheneAutoMaterializePolicy(graphene.ObjectType):
     policyType = graphene.NonNull(graphene.Enum.from_enum(AutoMaterializePolicyType))
+    maxMaterializationsPerMinute = graphene.Int()
 
     class Meta:
         name = "AutoMaterializePolicy"
 
     def __init__(self, auto_materialize_policy: AutoMaterializePolicy):
         auto_materialize_policy = check.inst_param(
             auto_materialize_policy, "auto_materialize_policy", AutoMaterializePolicy
         )
         super().__init__(
             policyType=auto_materialize_policy.policy_type,
+            maxMaterializationsPerMinute=auto_materialize_policy.max_materializations_per_minute,
         )
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 
 
 class GrapheneBulkActionStatus(graphene.Enum):
     REQUESTED = "REQUESTED"
     COMPLETED = "COMPLETED"
     FAILED = "FAILED"
     CANCELED = "CANCELED"
+    CANCELING = "CANCELING"
 
     class Meta:
         name = "BulkActionStatus"
 
 
 class GrapheneAssetBackfillData(graphene.ObjectType):
     class Meta:
@@ -149,15 +150,15 @@
         limit=graphene.Int(),
     )
     unfinishedRuns = graphene.Field(
         non_null_list("dagster_graphql.schema.pipelines.pipeline.GrapheneRun"),
         limit=graphene.Int(),
     )
     error = graphene.Field(GraphenePythonError)
-    partitionStatuses = graphene.NonNull(
+    partitionStatuses = graphene.Field(
         "dagster_graphql.schema.partition_sets.GraphenePartitionStatuses"
     )
     partitionStatusCounts = non_null_list(
         "dagster_graphql.schema.partition_sets.GraphenePartitionStatusCounts"
     )
     isAssetBackfill = graphene.NonNull(graphene.Boolean)
     assetBackfillData = graphene.Field(GrapheneAssetBackfillData)
@@ -272,14 +273,17 @@
 
         return GraphenePartitionSet(
             external_repository_handle=partition_set.repository_handle,
             external_partition_set=partition_set,
         )
 
     def resolve_partitionStatuses(self, graphene_info: ResolveInfo):
+        if self._backfill_job.is_asset_backfill:
+            return None
+
         partition_set_origin = self._backfill_job.partition_set_origin
         partition_set_name = (
             partition_set_origin.partition_set_name if partition_set_origin else None
         )
         partition_run_data = self._get_partition_run_data(graphene_info)
         return partition_statuses_from_run_partition_data(
             partition_set_name,
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/errors.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/execution.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/external.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/instance.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/resources.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/roots/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from dagster_graphql.implementation.fetch_auto_materialize_asset_evaluations import (
     fetch_auto_materialize_asset_evaluations,
 )
 from dagster_graphql.implementation.fetch_env_vars import get_utilized_env_vars_or_error
 from dagster_graphql.implementation.fetch_logs import get_captured_log_metadata
 from dagster_graphql.implementation.fetch_runs import get_assets_latest_info
 from dagster_graphql.schema.auto_materialize_asset_evaluations import (
-    GrapheneAutoMaterializeAssetEvaluationRecord,
+    GrapheneAutoMaterializeAssetEvaluationRecordsOrError,
 )
 from dagster_graphql.schema.env_vars import GrapheneEnvVarWithConsumersListOrError
 
 from ...implementation.external import (
     fetch_location_statuses,
     fetch_repositories,
     fetch_repository,
@@ -465,16 +465,16 @@
     )
 
     test = graphene.Field(
         GrapheneTestFields,
         description="Provides fields for testing behavior",
     )
 
-    autoMaterializeAssetEvaluations = graphene.Field(
-        non_null_list(GrapheneAutoMaterializeAssetEvaluationRecord),
+    autoMaterializeAssetEvaluationsOrError = graphene.Field(
+        GrapheneAutoMaterializeAssetEvaluationRecordsOrError,
         assetKey=graphene.Argument(GrapheneAssetKeyInput),
         limit=graphene.Argument(graphene.NonNull(graphene.Int)),
         cursor=graphene.Argument(graphene.String),
         description="Retrieve the auto materialization evaluation records for all assets.",
     )
 
     @capture_error
@@ -983,17 +983,17 @@
 
     def resolve_shouldShowNux(self, graphene_info):
         return graphene_info.context.instance.nux_enabled and not get_has_seen_nux()
 
     def resolve_test(self, _):
         return GrapheneTestFields()
 
-    def resolve_autoMaterializeAssetEvaluations(
+    def resolve_autoMaterializeAssetEvaluationsOrError(
         self,
         graphene_info: ResolveInfo,
         assetKey: GrapheneAssetKeyInput,
         limit: int,
-        cursor: Optional[str],
+        cursor: Optional[str] = None,
     ):
         return fetch_auto_materialize_asset_evaluations(
             instance=graphene_info.context.instance, asset_key=assetKey, cursor=cursor, limit=limit
         )
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/runs.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/solids.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/table.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/tags.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/schema/util.py` & `dagster-graphql-1.3.7/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql/test/utils.py` & `dagster-graphql-1.3.7/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.3.7/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.6
+Version: 1.3.7
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.6/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.3.7/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.6/setup.py` & `dagster-graphql-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.3.6",
+        "dagster==1.3.7",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
         "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
```

