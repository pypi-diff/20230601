# Comparing `tmp/dagster-1.3.6.tar.gz` & `tmp/dagster-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.3.6.tar", last modified: Thu May 25 17:17:08 2023, max compression
+gzip compressed data, was "dagster-1.3.7.tar", last modified: Thu Jun  1 18:15:21 2023, max compression
```

## Comparing `dagster-1.3.6.tar` & `dagster-1.3.7.tar`

### file list

```diff
@@ -1,628 +1,629 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.351283 dagster-1.3.6/
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-25 17:16:49.000000 dagster-1.3.6/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:49.000000 dagster-1.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-25 17:16:49.000000 dagster-1.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-05-25 17:17:08.351283 dagster-1.3.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-05-25 17:16:49.000000 dagster-1.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.287283 dagster-1.3.6/dagster/
--rw-r--r--   0 root         (0) root         (0)    26157 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.287283 dagster-1.3.6/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2882 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.291283 dagster-1.3.6/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.291283 dagster-1.3.6/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27241 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    29822 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5135 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19909 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.291283 dagster-1.3.6/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28391 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.295283 dagster-1.3.6/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15864 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    19601 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16880 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.295283 dagster-1.3.6/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    71109 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17162 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.295283 dagster-1.3.6/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13645 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.295283 dagster-1.3.6/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.303283 dagster-1.3.6/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7626 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30229 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3816 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36842 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    58294 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    18474 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    64821 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24005 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/auto_materialize_condition.py
--rw-r--r--   0 root         (0) root         (0)     5297 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16105 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45671 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20795 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    17905 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.307283 dagster-1.3.6/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43205 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10676 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14396 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8656 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     6591 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    20546 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39988 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    31576 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21013 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10548 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16195 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44740 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22898 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    51157 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    20308 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.307283 dagster-1.3.6/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    32319 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    56090 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11927 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    22629 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19256 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7509 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    18908 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    39032 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47274 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27231 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.307283 dagster-1.3.6/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    18856 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    17401 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    16917 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    16162 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    24105 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15824 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    38400 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    37556 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10837 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    46882 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    14148 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    12374 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    76525 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15645 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    25453 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6241 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.307283 dagster-1.3.6/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    64981 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7783 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.311283 dagster-1.3.6/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38315 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    30249 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14476 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.311283 dagster-1.3.6/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21992 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9369 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    26845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27417 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    33974 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    44193 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18501 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5149 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5426 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14451 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23031 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12550 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16270 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27355 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10000 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    37831 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    57790 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19280 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15667 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14328 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2789 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33518 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    32089 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    70934 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    12283 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19051 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3610 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   104144 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12808 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24318 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6808 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17249 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11030 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    21903 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18247 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2815 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12099 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16654 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4495 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14452 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.323283 dagster-1.3.6/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.323283 dagster-1.3.6/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.331283 dagster-1.3.6/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.331283 dagster-1.3.6/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8736 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9545 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    23596 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11640 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.331283 dagster-1.3.6/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14381 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3630 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    78441 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.331283 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7408 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18950 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13217 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    27079 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23189 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15454 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46394 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6358 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    22541 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13981 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    14855 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27932 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    19369 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35761 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     4003 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    27515 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3952 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5246 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4399 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17838 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10032 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39799 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.283283 dagster-1.3.6/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29251 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39700 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18451 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    21967 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5551 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    12415 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    51587 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26559 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34303 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    37613 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.351283 dagster-1.3.6/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23319 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8741 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    24259 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    12340 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.351283 dagster-1.3.6/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    10412 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    28864 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.351283 dagster-1.3.6/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.287283 dagster-1.3.6/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25163 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1317 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-25 17:17:08.355284 dagster-1.3.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6509 2023-05-25 17:16:50.000000 dagster-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.218557 dagster-1.3.7/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-01 18:14:54.000000 dagster-1.3.7/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-01 18:14:54.000000 dagster-1.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-01 18:14:54.000000 dagster-1.3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-06-01 18:15:21.218557 dagster-1.3.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-06-01 18:14:54.000000 dagster-1.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.066558 dagster-1.3.7/dagster/
+-rw-r--r--   0 root         (0) root         (0)    26213 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.070558 dagster-1.3.7/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.070558 dagster-1.3.7/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.070558 dagster-1.3.7/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27021 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8263 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5867 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    29907 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5129 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19958 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15707 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.070558 dagster-1.3.7/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28391 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.082558 dagster-1.3.7/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15864 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    19601 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    16880 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.082558 dagster-1.3.7/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    71109 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.090558 dagster-1.3.7/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.090558 dagster-1.3.7/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.114558 dagster-1.3.7/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30229 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    36842 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    58554 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    18474 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    64846 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24005 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/auto_materialize_condition.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16105 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45671 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10845 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20795 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    18695 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.118558 dagster-1.3.7/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43205 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10676 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17845 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14396 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8656 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     7085 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    21205 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39988 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31576 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21013 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16195 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44740 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22898 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    51157 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20308 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.118558 dagster-1.3.7/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32319 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    56090 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20758 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    22629 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19256 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    39032 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47274 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27231 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.122558 dagster-1.3.7/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    18856 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    17401 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    16917 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    16162 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    24105 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    38400 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    37556 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10837 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    46882 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    15391 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    76525 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15645 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    25453 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6241 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.126558 dagster-1.3.7/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    64981 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7783 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.130558 dagster-1.3.7/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38315 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    36589 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14710 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.134558 dagster-1.3.7/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21992 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9369 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    26845 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27349 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    33974 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    44193 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18501 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14451 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.138558 dagster-1.3.7/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23031 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12550 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16270 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27355 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10000 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    37831 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    57790 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19280 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.138558 dagster-1.3.7/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15667 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.138558 dagster-1.3.7/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14328 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.138558 dagster-1.3.7/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.142558 dagster-1.3.7/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33518 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    32089 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    70934 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19051 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.142558 dagster-1.3.7/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   104144 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12808 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24084 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6808 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17249 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11030 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    21903 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18247 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.150558 dagster-1.3.7/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16654 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14452 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.158558 dagster-1.3.7/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.158558 dagster-1.3.7/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.178557 dagster-1.3.7/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.178557 dagster-1.3.7/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    24055 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14381 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3630 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)    78441 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7408 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    18950 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13217 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    27079 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23189 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15454 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46394 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    22541 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13981 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    14855 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27932 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    19369 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.190558 dagster-1.3.7/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.190558 dagster-1.3.7/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    27515 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6111 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4447 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17838 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/monitoring/monitoring_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39799 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.066558 dagster-1.3.7/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.202558 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.202558 dagster-1.3.7/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.202558 dagster-1.3.7/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29251 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39700 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18451 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    21967 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.202558 dagster-1.3.7/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    51761 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26559 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34303 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    37613 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.214558 dagster-1.3.7/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23319 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8732 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    24259 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9813 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    12340 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.214558 dagster-1.3.7/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    10412 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    28864 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.214558 dagster-1.3.7/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.066558 dagster-1.3.7/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25185 2023-06-01 18:15:21.000000 dagster-1.3.7/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-01 18:15:21.218557 dagster-1.3.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-06-01 18:14:54.000000 dagster-1.3.7/setup.py
```

### Comparing `dagster-1.3.6/COPYING` & `dagster-1.3.7/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/LICENSE` & `dagster-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/PKG-INFO` & `dagster-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.6
+Version: 1.3.7
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.6/README.md` & `dagster-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/__init__.py` & `dagster-1.3.7/dagster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 )
 from dagster._core.definitions.composition import PendingNodeInvocation as PendingNodeInvocation
 from dagster._core.definitions.config import ConfigMapping as ConfigMapping
 from dagster._core.definitions.configurable import configured as configured
 from dagster._core.definitions.data_version import (
     DataProvenance as DataProvenance,
     DataVersion as DataVersion,
+    DataVersionsByPartition as DataVersionsByPartition,
 )
 from dagster._core.definitions.decorators.asset_decorator import (
     asset as asset,
     graph_asset as graph_asset,
     graph_multi_asset as graph_multi_asset,
     multi_asset as multi_asset,
 )
```

### Comparing `dagster-1.3.6/dagster/_annotations.py` & `dagster-1.3.7/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/get_server_id.py` & `dagster-1.3.7/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/list_repositories.py` & `dagster-1.3.7/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/notebook_data.py` & `dagster-1.3.7/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.7/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/snapshot_job.py` & `dagster-1.3.7/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/snapshot_partition.py` & `dagster-1.3.7/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/snapshot_repository.py` & `dagster-1.3.7/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/snapshot_schedule.py` & `dagster-1.3.7/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_api/snapshot_sensor.py` & `dagster-1.3.7/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_check/README.md` & `dagster-1.3.7/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_check/__init__.py` & `dagster-1.3.7/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_cli/__init__.py` & `dagster-1.3.7/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_cli/api.py` & `dagster-1.3.7/dagster/_cli/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 from dagster._grpc.types import ExecuteRunArgs, ExecuteStepArgs, ResumeRunArgs
 from dagster._serdes import deserialize_value, serialize_value
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.hosted_user_process import recon_job_from_origin
 from dagster._utils.interrupts import capture_interrupts, setup_interrupt_handlers
 from dagster._utils.log import configure_loggers
 
+from .utils import get_instance_for_cli
+
 
 @click.group(name="api", hidden=True)
 def api_cli():
     """[INTERNAL] These commands are intended to support internal use cases. Users should generally
     not invoke these commands interactively.
     """
 
@@ -56,19 +58,15 @@
     ),
 )
 @click.argument("input_json", type=click.STRING)
 def execute_run_command(input_json):
     with capture_interrupts():
         args = deserialize_value(input_json, ExecuteRunArgs)
 
-        with (
-            DagsterInstance.from_ref(args.instance_ref)
-            if args.instance_ref
-            else DagsterInstance.get()
-        ) as instance:
+        with get_instance_for_cli(instance_ref=args.instance_ref) as instance:
             buffer = []
 
             def send_to_buffer(event):
                 buffer.append(serialize_value(event))
 
             return_code = _execute_run_command_body(
                 args.run_id,
@@ -161,19 +159,15 @@
     ),
 )
 @click.argument("input_json", type=click.STRING)
 def resume_run_command(input_json):
     with capture_interrupts():
         args = deserialize_value(input_json, ResumeRunArgs)
 
-        with (
-            DagsterInstance.from_ref(args.instance_ref)
-            if args.instance_ref
-            else DagsterInstance.get()
-        ) as instance:
+        with get_instance_for_cli(instance_ref=args.instance_ref) as instance:
             buffer = []
 
             def send_to_buffer(event):
                 buffer.append(serialize_value(event))
 
             return_code = _resume_run_command_body(
                 args.run_id,
@@ -337,19 +331,15 @@
         )
 
         if compressed_input_json:
             input_json = zlib.decompress(base64.b64decode(compressed_input_json.encode())).decode()
 
         args = deserialize_value(input_json, ExecuteStepArgs)
 
-        with (
-            DagsterInstance.from_ref(args.instance_ref)
-            if args.instance_ref
-            else DagsterInstance.get()
-        ) as instance:
+        with get_instance_for_cli(instance_ref=args.instance_ref) as instance:
             dagster_run = instance.get_run_by_id(args.run_id)
 
             buff = []
 
             for event in _execute_step_command_body(
                 args,
                 instance,
```

### Comparing `dagster-1.3.6/dagster/_cli/asset.py` & `dagster-1.3.7/dagster/_cli/asset.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,29 +16,31 @@
 from dagster._core.telemetry import telemetry_wrapper
 from dagster._utils.hosted_user_process import (
     recon_job_from_origin,
     recon_repository_from_origin,
 )
 from dagster._utils.interrupts import capture_interrupts
 
-from .utils import get_instance_for_service
+from .utils import get_instance_for_cli, get_possibly_temporary_instance_for_cli
 
 
 @click.group(name="asset")
 def asset_cli():
     """Commands for working with Dagster assets."""
 
 
 @asset_cli.command(name="materialize", help="Execute a run to materialize a selection of assets")
 @python_origin_target_argument
 @click.option("--select", help="Asset selection to target", required=True)
 @click.option("--partition", help="Asset partition to target", required=False)
 def asset_materialize_command(**kwargs):
     with capture_interrupts():
-        with get_instance_for_service("``dagster asset materialize``") as instance:
+        with get_possibly_temporary_instance_for_cli(
+            "``dagster asset materialize``",
+        ) as instance:
             execute_materialize_command(instance, kwargs)
 
 
 @telemetry_wrapper
 def execute_materialize_command(instance: DagsterInstance, kwargs: Mapping[str, str]) -> None:
     repository_origin = get_repository_python_origin_from_kwargs(kwargs)
 
@@ -129,15 +131,15 @@
         )
 
     if cli_args.get("all") and len(key) > 0:
         raise click.UsageError("Error, cannot use more than one of: asset key, `--all`.")
 
     noprompt = cli_args.get("noprompt")
 
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         if len(key) > 0:
             asset_keys = [AssetKey.from_db_string(key_string) for key_string in key]
             prompt = (
                 "Are you sure you want to remove the asset key indexes for these keys from the"
                 " event logs? Type DELETE"
             )
         else:
@@ -181,15 +183,15 @@
         )
 
     if cli_args.get("all") and len(key) > 0:
         raise click.UsageError("Error, cannot use more than one of: asset key, `--all`.")
 
     noprompt = cli_args.get("noprompt")
 
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         if instance.can_cache_asset_status_data() is False:
             raise click.UsageError(
                 "Error, the instance does not support caching asset status. Wiping the cache is not"
                 " supported."
             )
 
         if len(key) > 0:
```

### Comparing `dagster-1.3.6/dagster/_cli/code_server.py` & `dagster-1.3.7/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_cli/config_scaffolder.py` & `dagster-1.3.7/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_cli/debug.py` & `dagster-1.3.7/dagster/_cli/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from gzip import GzipFile
 from typing import List, Tuple
 
 import click
 from tqdm import tqdm
 
-from dagster import DagsterInstance
 from dagster._core.debug import DebugRunPayload
 from dagster._core.storage.dagster_run import DagsterRunStatus, RunsFilter
 from dagster._serdes import deserialize_value
 
+from .utils import get_instance_for_cli
+
 
 def _recent_failed_runs_text(instance):
     lines = []
     runs = instance.get_runs(
         limit=5,
         filters=RunsFilter(statuses=[DagsterRunStatus.FAILURE, DagsterRunStatus.CANCELED]),
     )
@@ -45,15 +46,15 @@
 @debug_cli.command(
     name="export",
     help="Export the relevant artifacts for a job run from the current instance in to a file.",
 )
 @click.argument("run_id", type=str)
 @click.argument("output_file", type=click.Path())
 def export_command(run_id, output_file):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         run = instance.get_run_by_id(run_id)
         if run is None:
             raise click.UsageError(
                 "Could not find run with run_id '{}'.\n{}".format(
                     run_id, _recent_failed_runs_text(instance)
                 )
             )
@@ -69,15 +70,15 @@
     debug_payloads: List[DebugRunPayload] = []
     for input_file in input_files:
         with GzipFile(input_file, "rb") as file:
             blob = file.read().decode("utf-8")
             debug_payload = deserialize_value(blob, DebugRunPayload)
             debug_payloads.append(debug_payload)
 
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         for debug_payload in debug_payloads:
             run = debug_payload.dagster_run
             click.echo(f"Importing run {run.run_id} (Dagster: {debug_payload.version})")
             if not instance.has_snapshot(run.execution_plan_snapshot_id):  # type: ignore  # (possible none)
                 instance.add_snapshot(
                     debug_payload.execution_plan_snapshot,
                     run.execution_plan_snapshot_id,
```

### Comparing `dagster-1.3.6/dagster/_cli/dev.py` & `dagster-1.3.7/dagster/_cli/dev.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import dagster._check as check
 from dagster._serdes import serialize_value
 from dagster._serdes.ipc import interrupt_ipc_subprocess, open_ipc_subprocess
 from dagster._utils.log import configure_loggers
 
 from .job import apply_click_params
-from .utils import get_instance_for_service
+from .utils import get_possibly_temporary_instance_for_cli
 from .workspace.cli_target import (
     ClickArgValue,
     get_workspace_load_target,
     python_file_option,
     python_module_option,
     working_directory_option,
     workspace_option,
@@ -91,15 +91,15 @@
             logger.warning(
                 "Found a dagster instance configuration value (dagster.yaml) in the current"
                 " folder, but your DAGSTER_HOME environment variable is set to"
                 f" {dagster_home_path}. The dagster.yaml file will not be used to configure Dagster"
                 " unless it is placed in the same folder as DAGSTER_HOME."
             )
 
-    with get_instance_for_service("dagster dev", logger_fn=logger.info) as instance:
+    with get_possibly_temporary_instance_for_cli("dagster dev", logger=logger) as instance:
         logger.info("Launching Dagster services...")
 
         args = [
             "--instance-ref",
             serialize_value(instance.get_ref()),
             "--code-server-log-level",
             code_server_log_level,
```

### Comparing `dagster-1.3.6/dagster/_cli/instance.py` & `dagster-1.3.7/dagster/_cli/instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 
 import click
 
 import dagster._check as check
-from dagster._core.instance import DagsterInstance
+
+from .utils import get_instance_for_cli
 
 
 @click.group(name="instance")
 def instance_cli():
     """Commands for working with the current Dagster instance."""
 
 
 @instance_cli.command(name="info", help="List the information about the current instance.")
 def info_command():
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         home = os.environ.get("DAGSTER_HOME")
 
         if instance.is_ephemeral:
             check.invariant(
                 home is None,
                 f'Unexpected state, ephemeral instance but DAGSTER_HOME is set to "{home}"',
             )
@@ -35,29 +36,30 @@
 
         click.echo("\nStorage schema state:\n---------------------")
         click.echo(instance.schema_str())
 
 
 @instance_cli.command(name="migrate", help="Automatically migrate an out of date instance.")
 def migrate_command():
-    home = os.environ.get("DAGSTER_HOME")
-    if not home:
-        click.echo("$DAGSTER_HOME is not set; ephemeral instances do not need to be migrated.")
+    with get_instance_for_cli() as instance:
+        home = os.environ.get("DAGSTER_HOME")
+        if not home:
+            click.echo("$DAGSTER_HOME is not set; ephemeral instances do not need to be migrated.")
+            return
 
-    click.echo(f"$DAGSTER_HOME: {home}\n")
+        click.echo(f"$DAGSTER_HOME: {home}\n")
 
-    with DagsterInstance.get() as instance:
         instance.upgrade(click.echo)
 
         click.echo(instance.info_str())
 
 
 @instance_cli.command(name="reindex", help="Rebuild index over historical runs for performance.")
 def reindex_command():
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         home = os.environ.get("DAGSTER_HOME")
 
         if instance.is_ephemeral:
             click.echo(
                 "$DAGSTER_HOME is not set; ephemeral instances cannot be reindexed.  If you "
                 "intended to migrate a persistent instance, please ensure that $DAGSTER_HOME is "
                 "set accordingly."
```

### Comparing `dagster-1.3.6/dagster/_cli/job.py` & `dagster-1.3.7/dagster/_cli/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 from dagster._utils.hosted_user_process import recon_job_from_origin
 from dagster._utils.indenting_printer import IndentingPrinter
 from dagster._utils.interrupts import capture_interrupts
 from dagster._utils.merger import merge_dicts
 from dagster._utils.yaml_utils import dump_run_config_yaml, load_yaml_from_glob_list
 
 from .config_scaffolder import scaffold_job_config
-from .utils import get_instance_for_service
+from .utils import get_instance_for_cli, get_possibly_temporary_instance_for_cli
 
 T = TypeVar("T")
 T_Callable = TypeVar("T_Callable", bound=Callable[..., Any])
 
 
 @click.group(name="job")
 def job_cli():
@@ -86,15 +86,15 @@
 )
 @job_repository_target_argument
 def job_list_command(**kwargs):
     return execute_list_command(kwargs, click.echo)
 
 
 def execute_list_command(cli_args, print_fn):
-    with get_instance_for_service("``dagster job list``") as instance:
+    with get_possibly_temporary_instance_for_cli("``dagster job list``") as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repository:
             title = f"Repository {external_repository.name}"
             print_fn(title)
             print_fn("*" * len(title))
             first = True
@@ -139,15 +139,15 @@
 @job_cli.command(
     name="print",
     help="Print a job.\n\n{instructions}".format(instructions=get_job_instructions("print")),
 )
 @click.option("--verbose", is_flag=True)
 @job_target_argument
 def job_print_command(verbose, **cli_args):
-    with get_instance_for_service("``dagster job print``") as instance:
+    with get_possibly_temporary_instance_for_cli("``dagster job print``") as instance:
         return execute_print_command(instance, verbose, cli_args, click.echo)
 
 
 def execute_print_command(instance, verbose, cli_args, print_fn):
     with get_external_job_from_kwargs(
         instance,
         version=dagster_version,
@@ -243,15 +243,15 @@
     help="Display the freshness of memoized results for the given job.\n\n{instructions}".format(
         instructions=get_job_in_same_python_env_instructions("list_versions")
     ),
 )
 @python_job_target_argument
 @python_job_config_argument("list_versions")
 def job_list_versions_command(**kwargs):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         execute_list_versions_command(instance, kwargs)
 
 
 def execute_list_versions_command(instance: DagsterInstance, kwargs: ClickArgMapping):
     check.inst_param(instance, "instance", DagsterInstance)
 
     config = list(
@@ -307,15 +307,15 @@
     ),
 )
 @python_job_target_argument
 @python_job_config_argument("execute")
 @click.option("--tags", type=click.STRING, help="JSON string of tags to use for this job run")
 def job_execute_command(**kwargs: ClickArgValue):
     with capture_interrupts():
-        with get_instance_for_service("``dagster job execute``") as instance:
+        with get_possibly_temporary_instance_for_cli("``dagster job execute``") as instance:
             execute_execute_command(instance, kwargs)
 
 
 @telemetry_wrapper
 def execute_execute_command(instance: DagsterInstance, kwargs: ClickArgMapping) -> ExecutionResult:
     check.inst_param(instance, "instance", DagsterInstance)
 
@@ -424,15 +424,15 @@
     "--config-json",
     type=click.STRING,
     help="JSON string of run config to use for this job run. Cannot be used with -c / --config.",
 )
 @click.option("--tags", type=click.STRING, help="JSON string of tags to use for this job run")
 @click.option("--run-id", type=click.STRING, help="The ID to give to the launched job run")
 def job_launch_command(**kwargs) -> DagsterRun:
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         return execute_launch_command(instance, kwargs)
 
 
 @telemetry_wrapper
 def execute_launch_command(
     instance: DagsterInstance,
     kwargs: Mapping[str, str],
@@ -632,15 +632,15 @@
         "\n\nExample: "
         "dagster job backfill log_daily_stats --to 20191201"
     ),
 )
 @click.option("--tags", type=click.STRING, help="JSON string of tags to use for this job run")
 @click.option("--noprompt", is_flag=True)
 def job_backfill_command(**kwargs):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         execute_backfill_command(kwargs, click.echo, instance)
 
 
 def execute_backfill_command(
     cli_args: ClickArgMapping, print_fn: PrintFn, instance: DagsterInstance
 ) -> None:
     with get_workspace_from_kwargs(instance, version=dagster_version, kwargs=cli_args) as workspace:
```

### Comparing `dagster-1.3.6/dagster/_cli/load_handle.py` & `dagster-1.3.7/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_cli/project.py` & `dagster-1.3.7/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_cli/run.py` & `dagster-1.3.7/dagster/_cli/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import click
 from tqdm import tqdm
 
 from dagster import __version__ as dagster_version
 from dagster._cli.workspace.cli_target import get_external_job_from_kwargs, job_target_argument
-from dagster._core.instance import DagsterInstance
+
+from .utils import get_instance_for_cli
 
 
 @click.group(name="run")
 def run_cli():
     """Commands for working with Dagster job runs."""
 
 
 @run_cli.command(name="list", help="List the runs in the current Dagster instance.")
 @click.option("--limit", help="Only list a specified number of runs", default=None, type=int)
 def run_list_command(limit):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         for run in instance.get_runs(limit=limit):
             click.echo(f"Run: {run.run_id}")
             click.echo(f"     Job: {run.job_name}")
 
 
 @run_cli.command(
     name="delete",
     help="Delete a run by id and its associated event logs. Warning: Cannot be undone",
 )
 @click.option("--force", "-f", is_flag=True, default=False, help="Skip prompt to delete run.")
 @click.argument("run_id")
 def run_delete_command(run_id, force):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         if not instance.has_run(run_id):
             raise click.ClickException(f"No run found with id {run_id}.")
 
         if force:
             should_delete_run = True
         else:
             confirmation = click.prompt(
@@ -62,15 +63,15 @@
     else:
         confirmation = click.prompt(
             "Are you sure you want to delete all run history and event logs? Type DELETE."
         )
         should_delete_run = confirmation == "DELETE"
 
     if should_delete_run:
-        with DagsterInstance.get() as instance:
+        with get_instance_for_cli() as instance:
             instance.wipe()
         click.echo("Deleted all run history and event logs.")
     else:
         raise click.ClickException("Exiting without deleting all run history and event logs.")
 
 
 @run_cli.command(
@@ -93,15 +94,15 @@
         raise click.UsageError("Must specify a --from repository label")
 
     if not is_valid_repo_label(from_label):
         raise click.UsageError(
             "`--from` argument must be of the format: <repository_name>@<location_name>"
         )
 
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_job_from_kwargs(
             instance, version=dagster_version, kwargs=kwargs
         ) as external_job:
             new_job_origin = external_job.get_external_origin()
             job_name = external_job.name
             to_label = new_job_origin.external_repository_origin.get_label()
```

### Comparing `dagster-1.3.6/dagster/_cli/schedule.py` & `dagster-1.3.7/dagster/_cli/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 )
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.host_representation import ExternalRepository
 from dagster._core.instance import DagsterInstance
 from dagster._core.scheduler.instigation import InstigatorStatus
 from dagster._core.scheduler.scheduler import DagsterDaemonScheduler
 
+from .utils import get_instance_for_cli
+
 
 @click.group(name="schedule")
 def schedule_cli():
     """Commands for working with Dagster schedules."""
 
 
 def print_changes(external_repository, instance, print_fn=print, preview=False):
@@ -142,15 +144,15 @@
 )
 @repository_target_argument
 def schedule_preview_command(**kwargs):
     return execute_preview_command(kwargs, click.echo)
 
 
 def execute_preview_command(cli_args, print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
 
             print_changes(external_repo, instance, print_fn, preview=True)
 
@@ -164,15 +166,15 @@
 @click.option("--stopped", help="Filter for stopped schedules", is_flag=True, default=False)
 @click.option("--name", help="Only display schedule schedule names", is_flag=True, default=False)
 def schedule_list_command(running, stopped, name, **kwargs):
     return execute_list_command(running, stopped, name, kwargs, click.echo)
 
 
 def execute_list_command(running_filter, stopped_filter, name_filter, cli_args, print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
 
             repository_name = external_repo.name
 
@@ -243,15 +245,15 @@
             "schedules to start. Pass a schedule name or the --start-all flag to start schedules."
         )
         return
     return execute_start_command(schedule_name, start_all, kwargs, click.echo)
 
 
 def execute_start_command(schedule_name, all_flag, cli_args, print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
 
             repository_name = external_repo.name
 
@@ -281,15 +283,15 @@
 @repository_target_argument
 def schedule_stop_command(schedule_name, **kwargs):
     schedule_name = extract_schedule_name(schedule_name)
     return execute_stop_command(schedule_name, kwargs, click.echo)
 
 
 def execute_stop_command(schedule_name, cli_args, print_fn, instance=None):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
 
             try:
                 external_schedule = external_repo.get_external_schedule(schedule_name)
@@ -315,15 +317,15 @@
             "schedules to retrieve logs for. Pass a schedule name"
         )
         return
     return execute_logs_command(schedule_name, kwargs, click.echo)
 
 
 def execute_logs_command(schedule_name, cli_args, print_fn, instance=None):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
 
             if isinstance(instance.scheduler, DagsterDaemonScheduler):
                 return print_fn(
@@ -381,15 +383,15 @@
 @repository_target_argument
 def schedule_restart_command(schedule_name, restart_all_running, **kwargs):
     schedule_name = extract_schedule_name(schedule_name)
     return execute_restart_command(schedule_name, restart_all_running, kwargs, click.echo)
 
 
 def execute_restart_command(schedule_name, all_running_flag, cli_args, print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
 
             repository_name = external_repo.name
 
@@ -446,15 +448,15 @@
 
 @schedule_cli.command(name="wipe", help="Delete the schedule history and turn off all schedules.")
 def schedule_wipe_command():
     return execute_wipe_command(click.echo)
 
 
 def execute_wipe_command(print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         confirmation = click.prompt(
             "Are you sure you want to turn off all schedules and delete all schedule history? Type"
             " DELETE"
         )
         if confirmation == "DELETE":
             instance.wipe_all_schedules()
             print_fn("Turned off all schedules and deleted all schedule history")
@@ -464,15 +466,15 @@
 
 @schedule_cli.command(name="debug", help="Debug information about the scheduler.")
 def schedule_debug_command():
     return execute_debug_command(click.echo)
 
 
 def execute_debug_command(print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         debug_info = instance.scheduler_debug_info()
 
         output = ""
 
         errors = debug_info.errors
         if len(errors):
             title = "Errors (Run `dagster schedule up` to resolve)"
```

### Comparing `dagster-1.3.6/dagster/_cli/sensor.py` & `dagster-1.3.7/dagster/_cli/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     InstigatorState,
     InstigatorStatus,
     SensorInstigatorData,
 )
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.yaml_utils import dump_run_config_yaml
 
+from .utils import get_instance_for_cli
+
 
 @click.group(name="sensor")
 def sensor_cli():
     """Commands for working with Dagster sensors."""
 
 
 def print_changes(external_repository, instance, print_fn=print, preview=False):
@@ -123,15 +125,15 @@
 @click.option("--stopped", help="Filter for stopped sensors", is_flag=True, default=False)
 @click.option("--name", help="Only display sensor sensor names", is_flag=True, default=False)
 def sensor_list_command(running, stopped, name, **kwargs):
     return execute_list_command(running, stopped, name, kwargs, click.echo)
 
 
 def execute_list_command(running_filter, stopped_filter, name_filter, cli_args, print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
             repository_name = external_repo.name
 
             if not name_filter:
@@ -182,15 +184,15 @@
 def sensor_start_command(sensor_name, start_all, **kwargs):
     if not start_all:
         sensor_name = extract_sensor_name(sensor_name)
     return execute_start_command(sensor_name, start_all, kwargs, click.echo)
 
 
 def execute_start_command(sensor_name, all_flag, cli_args, print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
             repository_name = external_repo.name
 
             if all_flag:
@@ -219,15 +221,15 @@
 @repository_target_argument
 def sensor_stop_command(sensor_name, **kwargs):
     sensor_name = extract_sensor_name(sensor_name)
     return execute_stop_command(sensor_name, kwargs, click.echo)
 
 
 def execute_stop_command(sensor_name, cli_args, print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_external_repository_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as external_repo:
             check_repo_and_scheduler(external_repo, instance)
             try:
                 external_sensor = external_repo.get_external_sensor(sensor_name)
                 instance.stop_sensor(
@@ -265,15 +267,15 @@
         since = float(since)
     return execute_preview_command(sensor_name, since, last_run_key, cursor, kwargs, click.echo)
 
 
 def execute_preview_command(
     sensor_name, since, last_run_key, cursor, cli_args, print_fn, instance=None
 ):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_code_location_from_kwargs(
             instance,
             version=dagster_version,
             kwargs=cli_args,
         ) as code_location:
             try:
                 external_repo = get_external_repository_from_code_location(
@@ -343,15 +345,15 @@
 @repository_target_argument
 def sensor_cursor_command(sensor_name, **kwargs):
     sensor_name = extract_sensor_name(sensor_name)
     return execute_cursor_command(sensor_name, kwargs, click.echo)
 
 
 def execute_cursor_command(sensor_name, cli_args, print_fn):
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         with get_code_location_from_kwargs(
             instance, version=dagster_version, kwargs=cli_args
         ) as code_location:
             if bool(cli_args.get("delete")) == bool(cli_args.get("set")):
                 # must use one of delete/set
                 raise click.UsageError("Must set cursor using `--set <value>` or use `--delete`")
```

### Comparing `dagster-1.3.6/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.7/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/__init__.py` & `dagster-1.3.7/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/config_schema.py` & `dagster-1.3.7/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/config_type.py` & `dagster-1.3.7/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/errors.py` & `dagster-1.3.7/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/evaluate_value_result.py` & `dagster-1.3.7/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/field.py` & `dagster-1.3.7/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/field_utils.py` & `dagster-1.3.7/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/post_process.py` & `dagster-1.3.7/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/primitive_mapping.py` & `dagster-1.3.7/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/pythonic_config/__init__.py` & `dagster-1.3.7/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.3.7/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.3.7/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/pythonic_config/utils.py` & `dagster-1.3.7/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/snap.py` & `dagster-1.3.7/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/source.py` & `dagster-1.3.7/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/stack.py` & `dagster-1.3.7/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/traversal_context.py` & `dagster-1.3.7/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/type_printer.py` & `dagster-1.3.7/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_config/validate.py` & `dagster-1.3.7/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/assets.py` & `dagster-1.3.7/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/code_pointer.py` & `dagster-1.3.7/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/container_context/config.py` & `dagster-1.3.7/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/debug.py` & `dagster-1.3.7/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/decorator_utils.py` & `dagster-1.3.7/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/__init__.py` & `dagster-1.3.7/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.7/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.7/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/asset_in.py` & `dagster-1.3.7/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.7/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/asset_out.py` & `dagster-1.3.7/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.7/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         asset. Every value is the set of that asset's partitoins that have been requested by
         this sensor or have been materialized (even if not by this sensor).
     """
 
     latest_storage_id: Optional[int]
     materialized_or_requested_root_asset_keys: AbstractSet[AssetKey]
     materialized_or_requested_root_partitions_by_asset_key: Mapping[AssetKey, PartitionsSubset]
-    evaluation_id: Optional[int]
+    evaluation_id: int
 
     def was_previously_materialized_or_requested(self, asset_key: AssetKey) -> bool:
         return asset_key in self.materialized_or_requested_root_asset_keys
 
     def get_never_requested_never_materialized_partitions(
         self,
         asset_key: AssetKey,
@@ -280,15 +280,15 @@
 
     def with_updates(
         self,
         latest_storage_id: Optional[int],
         run_requests: Sequence[RunRequest],
         newly_materialized_root_asset_keys: AbstractSet[AssetKey],
         newly_materialized_root_partitions_by_asset_key: Mapping[AssetKey, AbstractSet[str]],
-        evaluation_id: Optional[int],
+        evaluation_id: int,
         asset_graph: AssetGraph,
     ) -> "AssetReconciliationCursor":
         """Returns a cursor that represents this cursor plus the updates that have happened within the
         tick.
         """
         requested_root_partitions_by_asset_key: Dict[AssetKey, Set[str]] = defaultdict(set)
         requested_non_partitioned_root_assets: Set[AssetKey] = set()
@@ -361,15 +361,15 @@
 
         (
             latest_storage_id,
             serialized_materialized_or_requested_root_asset_keys,
             serialized_materialized_or_requested_root_partitions_by_asset_key,
         ) = data[:3]
 
-        evaluation_id = data[3] if len(data) == 4 else None
+        evaluation_id = data[3] if len(data) == 4 else 0
 
         materialized_or_requested_root_partitions_by_asset_key = {}
         for (
             key_str,
             serialized_subset,
         ) in serialized_materialized_or_requested_root_partitions_by_asset_key.items():
             key = AssetKey.from_user_string(key_str)
@@ -640,15 +640,17 @@
     ],
 ) -> Tuple[
     Mapping[AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]],
     AbstractSet[AssetKey],
     Mapping[AssetKey, AbstractSet[str]],
     Optional[int],
 ]:
-    materialization_counts_by_asset_key: Dict[AssetKey, int] = defaultdict(int)
+    materialization_requests_by_asset_key: Mapping[
+        AssetKey, Set[AssetKeyPartitionKey]
+    ] = defaultdict(set)
     evaluation_time = instance_queryer.evaluation_time
 
     (
         never_materialized_or_requested_roots,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
     ) = find_never_materialized_or_requested_root_asset_partitions(
@@ -765,21 +767,25 @@
         ):
             conditions.add(ParentMaterializedAutoMaterializeCondition())
 
         # if there are any conditions that would cause us to materialize this candidate unit, we
         # need to ensure they would not cause us to exceed the rate limit
         if conditions:
             if (
+                # has a rate limit
                 auto_materialize_policy.max_materializations_per_minute is not None
-                and materialization_counts_by_asset_key[candidate.asset_key]
+                # has not already been requested
+                and candidate not in materialization_requests_by_asset_key[candidate.asset_key]
+                # current number of requested asset partitions exceeds the rate limit
+                and len(materialization_requests_by_asset_key[candidate.asset_key])
                 >= auto_materialize_policy.max_materializations_per_minute
             ):
                 conditions.add(MaxMaterializationsExceededAutoMaterializeCondition())
             else:
-                materialization_counts_by_asset_key[candidate.asset_key] += 1
+                materialization_requests_by_asset_key[candidate.asset_key].add(candidate)
 
         return conditions
 
     def should_reconcile(
         asset_graph: AssetGraph,
         candidates_unit: Iterable[AssetKeyPartitionKey],
         to_reconcile: AbstractSet[AssetKeyPartitionKey],
@@ -1111,15 +1117,15 @@
         run_requests,
         cursor.with_updates(
             latest_storage_id=latest_storage_id,
             run_requests=run_requests,
             asset_graph=asset_graph,
             newly_materialized_root_asset_keys=newly_materialized_root_asset_keys,
             newly_materialized_root_partitions_by_asset_key=newly_materialized_root_partitions_by_asset_key,
-            evaluation_id=cursor.evaluation_id + 1 if cursor.evaluation_id is not None else 0,
+            evaluation_id=cursor.evaluation_id + 1,
         ),
         build_auto_materialize_asset_evaluations(
             asset_graph, conditions_by_asset_partition, dynamic_partitions_store=instance_queryer
         ),
     )
```

### Comparing `dagster-1.3.6/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.7/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.3.7/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/assets.py` & `dagster-1.3.7/dagster/_core/definitions/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -942,31 +942,33 @@
         # the set of keys that are not selected but are upstream of the selected keys
         input_keys = {
             dep_key for key in asset_subselection for dep_key in self.asset_deps[key]
         }.difference(asset_subselection)
         ins = {}
 
         input_names_by_key = {v: k for k, v in self.keys_by_input_name.items()}
-        output_names_by_key = {v: k for k, v in self.keys_by_output_name.items()}
         op_valid = True
+        input_index = 0
         for input_key in input_keys:
             input_name = input_names_by_key.get(input_key)
             if input_name is not None:
                 # just copy over existing input
                 ins[input_name] = self.op.ins[input_name]
             elif input_key in selected_asset_keys:
                 # There is no input existing for this key, meaning this is something that is produced
                 # within the op if it is not subsetted. If this input is part of the larger
                 # selection that we want to make a job out of, then this would require us to create
                 # a new input such that the dependency would be respected, and therefore a new copy
                 # of the underlying op.
                 op_valid = False
-                output_name = output_names_by_key[input_key]
-                ins[output_name] = In(Nothing)
-                input_names_by_key[input_key] = output_name
+                # create a new input for this key
+                input_name = f"artificial_input_{input_index}"
+                input_index += 1
+                ins[input_name] = In(Nothing)
+                input_names_by_key[input_key] = input_name
 
         # must create a new copy of the op
         if op_valid:
             op_def = self.op
         else:
             # create a hash of the selected keys to generate a unique name for this subsetted op
             suffix = hashlib.md5((str(list(sorted(asset_subselection)))).encode()).hexdigest()[-5:]
```

### Comparing `dagster-1.3.6/dagster/_core/definitions/assets_job.py` & `dagster-1.3.7/dagster/_core/definitions/assets_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/auto_materialize_condition.py` & `dagster-1.3.7/dagster/_core/definitions/auto_materialize_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.3.7/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.7/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/composition.py` & `dagster-1.3.7/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/config.py` & `dagster-1.3.7/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/configurable.py` & `dagster-1.3.7/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/data_time.py` & `dagster-1.3.7/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/data_version.py` & `dagster-1.3.7/dagster/_core/definitions/data_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Tuple,
     Union,
 )
 
 from typing_extensions import Final
 
 from dagster import _check as check
-from dagster._annotations import deprecated
+from dagster._annotations import deprecated, experimental
 from dagster._utils.cached_method import cached_method
 
 if TYPE_CHECKING:
     from dagster._core.definitions.asset_graph import AssetGraph
     from dagster._core.definitions.events import AssetKey
     from dagster._core.events.log import EventLogEntry
     from dagster._core.instance import DagsterInstance
@@ -59,14 +59,39 @@
     ):
         return super(DataVersion, cls).__new__(
             cls,
             value=check.str_param(value, "value"),
         )
 
 
+@experimental
+class DataVersionsByPartition(
+    NamedTuple(
+        "_DataVersionsByPartition", [("data_versions_by_partition", Mapping[str, DataVersion])]
+    )
+):
+    def __new__(
+        cls,
+        data_versions_by_partition: Mapping[str, Union[str, DataVersion]],
+    ):
+        check.dict_param(
+            data_versions_by_partition,
+            "data_versions_by_partition",
+            key_type=str,
+            value_type=(str, DataVersion),
+        )
+        return super(DataVersionsByPartition, cls).__new__(
+            cls,
+            data_versions_by_partition={
+                partition: DataVersion(version) if isinstance(version, str) else version
+                for partition, version in data_versions_by_partition.items()
+            },
+        )
+
+
 DEFAULT_DATA_VERSION: Final[DataVersion] = DataVersion("INITIAL")
 NULL_DATA_VERSION: Final[DataVersion] = DataVersion("NULL")
 UNKNOWN_DATA_VERSION: Final[DataVersion] = DataVersion("UNKNOWN")
 
 
 class DataProvenance(
     NamedTuple(
```

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.7/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import dagster._check as check
 from dagster._annotations import experimental
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKeyPrefix
 from dagster._core.definitions.metadata import (
     MetadataUserInput,
 )
+from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.resource_annotation import get_resource_args
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.source_asset import SourceAsset, SourceAssetObserveFunction
 
 
 @overload
 def observable_source_asset(observe_fn: SourceAssetObserveFunction) -> SourceAsset:
@@ -24,14 +25,15 @@
     metadata: Optional[MetadataUserInput] = None,
     io_manager_key: Optional[str] = None,
     io_manager_def: Optional[object] = None,
     description: Optional[str] = None,
     group_name: Optional[str] = None,
     required_resource_keys: Optional[AbstractSet[str]] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+    partitions_def: Optional[PartitionsDefinition] = None,
 ) -> "_ObservableSourceAsset":
     ...
 
 
 @experimental
 def observable_source_asset(
     observe_fn: Optional[SourceAssetObserveFunction] = None,
@@ -41,14 +43,15 @@
     metadata: Optional[MetadataUserInput] = None,
     io_manager_key: Optional[str] = None,
     io_manager_def: Optional[object] = None,
     description: Optional[str] = None,
     group_name: Optional[str] = None,
     required_resource_keys: Optional[AbstractSet[str]] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+    partitions_def: Optional[PartitionsDefinition] = None,
 ) -> Union[SourceAsset, "_ObservableSourceAsset"]:
     """Create a `SourceAsset` with an associated observation function.
 
     The observation function of a source asset is wrapped inside of an op and can be executed as
     part of a job. Each execution generates an `AssetObservation` event associated with the source
     asset. The source asset observation function should return a metadata dictionary that will be
     attached to the `AssetObservation`.
@@ -69,14 +72,16 @@
         description (Optional[str]): The description of the asset.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. If not provided,
             the name "default" is used.
         required_resource_keys (Optional[Set[str]]): Set of resource keys required by the observe op.
         resource_defs (Optional[Mapping[str, ResourceDefinition]]): (Experimental) resource
             definitions that may be required by the :py:class:`dagster.IOManagerDefinition` provided in
             the `io_manager_def` argument.
+        partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
+            compose the asset.
         observe_fn (Optional[SourceAssetObserveFunction]) Observation function for the source asset.
     """
     if observe_fn is not None:
         return _ObservableSourceAsset()(observe_fn)
 
     return _ObservableSourceAsset(
         name,
@@ -84,14 +89,15 @@
         metadata,
         io_manager_key,
         io_manager_def,
         description,
         group_name,
         required_resource_keys,
         resource_defs,
+        partitions_def,
     )
 
 
 class _ObservableSourceAsset:
     def __init__(
         self,
         name: Optional[str] = None,
@@ -99,28 +105,30 @@
         metadata: Optional[MetadataUserInput] = None,
         io_manager_key: Optional[str] = None,
         io_manager_def: Optional[object] = None,
         description: Optional[str] = None,
         group_name: Optional[str] = None,
         required_resource_keys: Optional[AbstractSet[str]] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+        partitions_def: Optional[PartitionsDefinition] = None,
     ):
         self.name = name
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
         elif key_prefix is None:
             key_prefix = []
         self.key_prefix = key_prefix
         self.metadata = metadata
         self.io_manager_key = io_manager_key
         self.io_manager_def = io_manager_def
         self.description = description
         self.group_name = group_name
         self.required_resource_keys = required_resource_keys
         self.resource_defs = resource_defs
+        self.partitions_def = partitions_def
 
     def __call__(self, observe_fn: SourceAssetObserveFunction) -> SourceAsset:
         source_asset_name = self.name or observe_fn.__name__
         source_asset_key = AssetKey([*self.key_prefix, source_asset_name])
 
         arg_resource_keys = {arg.name for arg in get_resource_args(observe_fn)}
         decorator_resource_keys = set(self.required_resource_keys or [])
@@ -139,8 +147,9 @@
             io_manager_key=self.io_manager_key,
             io_manager_def=self.io_manager_def,
             description=self.description,
             group_name=self.group_name,
             _required_resource_keys=resolved_resource_keys,
             resource_defs=self.resource_defs,
             observe_fn=observe_fn,
+            partitions_def=self.partitions_def,
         )
```

### Comparing `dagster-1.3.6/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.7/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.7/dagster/_core/definitions/definitions_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,35 @@
     """Given a list of jobs, schedules, and sensors along with top-level resource definitions,
     attach the resource definitions to the jobs, schedules, and sensors which require them.
     """
     jobs = jobs or []
     schedules = schedules or []
     sensors = sensors or []
 
+    # Add jobs in schedules and sensors as well
+    jobs = [
+        *jobs,
+        *[
+            schedule.job
+            for schedule in schedules
+            if isinstance(schedule, ScheduleDefinition)
+            and schedule.has_loadable_target()
+            and isinstance(schedule.job, (JobDefinition, UnresolvedAssetJobDefinition))
+        ],
+        *[
+            job
+            for sensor in sensors
+            if sensor.has_loadable_targets()
+            for job in sensor.jobs
+            if isinstance(job, (JobDefinition, UnresolvedAssetJobDefinition))
+        ],
+    ]
+    # Dedupe
+    jobs = list({id(job): job for job in jobs}.values())
+
     # Find unsatisfied jobs
     unsatisfied_jobs = [
         job
         for job in jobs
         if isinstance(job, JobDefinition)
         and (
             job.is_missing_required_resources() or _io_manager_needs_replacement(job, resource_defs)
```

### Comparing `dagster-1.3.6/dagster/_core/definitions/dependency.py` & `dagster-1.3.7/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/events.py` & `dagster-1.3.7/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.7/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.7/dagster/_core/definitions/external_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.7/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.3.7/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.7/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.7/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.7/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/inference.py` & `dagster-1.3.7/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/input.py` & `dagster-1.3.7/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.7/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/job_base.py` & `dagster-1.3.7/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/job_definition.py` & `dagster-1.3.7/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.7/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.7/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.7/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/materialize.py` & `dagster-1.3.7/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.7/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.7/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.7/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.7/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/node_container.py` & `dagster-1.3.7/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/node_definition.py` & `dagster-1.3.7/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/observe.py` & `dagster-1.3.7/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/op_definition.py` & `dagster-1.3.7/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.7/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/op_selection.py` & `dagster-1.3.7/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/output.py` & `dagster-1.3.7/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/partition.py` & `dagster-1.3.7/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.7/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.7/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/policy.py` & `dagster-1.3.7/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.7/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.7/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.7/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.7/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.7/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.7/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.7/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.7/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.7/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/run_config.py` & `dagster-1.3.7/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.7/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/run_request.py` & `dagster-1.3.7/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.7/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.7/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.7/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/selector.py` & `dagster-1.3.7/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.7/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/source_asset.py` & `dagster-1.3.7/dagster/_core/definitions/source_asset.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 )
 
 from typing_extensions import TypeAlias
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, public
 from dagster._core.decorator_utils import get_function_params
-from dagster._core.definitions.data_version import DATA_VERSION_TAG, DataVersion
+from dagster._core.definitions.data_version import (
+    DATA_VERSION_TAG,
+    DataVersion,
+    DataVersionsByPartition,
+)
 from dagster._core.definitions.events import AssetKey, AssetObservation, CoercibleToAssetKey
 from dagster._core.definitions.metadata import (
     ArbitraryMetadataMapping,
     MetadataMapping,
     normalize_metadata,
 )
 from dagster._core.definitions.op_definition import OpDefinition
@@ -37,15 +41,19 @@
     get_resource_key_conflicts,
 )
 from dagster._core.definitions.utils import (
     DEFAULT_GROUP_NAME,
     DEFAULT_IO_MANAGER_KEY,
     validate_group_name,
 )
-from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvalidInvocationError
+from dagster._core.errors import (
+    DagsterInvalidDefinitionError,
+    DagsterInvalidInvocationError,
+    DagsterInvalidObservationError,
+)
 from dagster._core.storage.io_manager import IOManagerDefinition
 from dagster._utils.backcompat import ExperimentalWarning, experimental_arg_warning
 from dagster._utils.merger import merge_dicts
 
 if TYPE_CHECKING:
     from dagster._core.execution.context.compute import (
         OpExecutionContext,
@@ -104,19 +112,14 @@
         _required_resource_keys: Optional[AbstractSet[str]] = None,
         # Add additional fields to with_resources and with_group below
     ):
         from dagster._core.execution.build_resources import (
             wrap_resources_for_execution,
         )
 
-        if partitions_def is not None and observe_fn is not None:
-            raise DagsterInvalidDefinitionError(
-                "Cannot specify a `partitions_def` for an observable source asset."
-            )
-
         if resource_defs is not None:
             experimental_arg_warning("resource_defs", "SourceAsset.__new__")
 
         if io_manager_def is not None:
             experimental_arg_warning("io_manager_def", "SourceAsset.__new__")
 
         self.key = AssetKey.from_coercible(key)
@@ -186,32 +189,57 @@
         )
 
         observe_fn_has_context = is_context_provided(get_function_params(observe_fn))
 
         def fn(context: OpExecutionContext):
             resource_kwarg_keys = [param.name for param in get_resource_args(observe_fn)]
             resource_kwargs = {key: getattr(context.resources, key) for key in resource_kwarg_keys}
-            data_version = (
+            observe_fn_return_value = (
                 observe_fn(context, **resource_kwargs)
                 if observe_fn_has_context
                 else observe_fn(**resource_kwargs)
             )
 
-            check.inst(
-                data_version,
-                DataVersion,
-                "Source asset observation function must return a DataVersion",
-            )
-            tags = {DATA_VERSION_TAG: data_version.value}
-            context.log_event(
-                AssetObservation(
-                    asset_key=self.key,
-                    tags=tags,
+            if isinstance(observe_fn_return_value, DataVersion):
+                if self.partitions_def is not None:
+                    raise DagsterInvalidObservationError(
+                        f"{self.key} is partitioned, so its observe function should return a"
+                        " DataVersionsByPartition, not a DataVersion"
+                    )
+
+                context.log_event(
+                    AssetObservation(
+                        asset_key=self.key,
+                        tags={DATA_VERSION_TAG: observe_fn_return_value.value},
+                    )
+                )
+            elif isinstance(observe_fn_return_value, DataVersionsByPartition):
+                if self.partitions_def is None:
+                    raise DagsterInvalidObservationError(
+                        f"{self.key} is not partitioned, so its observe function should return a"
+                        " DataVersion, not a DataVersionsByPartition"
+                    )
+
+                for (
+                    partition_key,
+                    data_version,
+                ) in observe_fn_return_value.data_versions_by_partition.items():
+                    context.log_event(
+                        AssetObservation(
+                            asset_key=self.key,
+                            tags={DATA_VERSION_TAG: data_version.value},
+                            partition=partition_key,
+                        )
+                    )
+            else:
+                raise DagsterInvalidObservationError(
+                    f"Observe function for {self.key} must return a DataVersion or"
+                    " DataVersionsByPartition, but returned a value of type"
+                    f" {type(observe_fn_return_value)}"
                 )
-            )
 
         return DecoratedOpFunction(fn)
 
     @property
     def required_resource_keys(self) -> AbstractSet[str]:
         return {requirement.key for requirement in self.get_resource_requirements()}
```

### Comparing `dagster-1.3.6/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.7/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/target.py` & `dagster-1.3.7/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.7/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.7/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.7/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/utils.py` & `dagster-1.3.7/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.7/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/errors.py` & `dagster-1.3.7/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/event_api.py` & `dagster-1.3.7/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/events/__init__.py` & `dagster-1.3.7/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/events/log.py` & `dagster-1.3.7/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/events/utils.py` & `dagster-1.3.7/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/api.py` & `dagster-1.3.7/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.7/dagster/_core/execution/asset_backfill.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 from dagster._core.errors import DagsterBackfillFailedError
 from dagster._core.events import DagsterEventType
 from dagster._core.host_representation import (
     ExternalExecutionPlan,
     ExternalJob,
 )
 from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
-from dagster._core.storage.dagster_run import DagsterRunStatus, RunsFilter
+from dagster._core.storage.dagster_run import (
+    CANCELABLE_RUN_STATUSES,
+    DagsterRunStatus,
+    RunsFilter,
+)
 from dagster._core.storage.tags import BACKFILL_ID_TAG, PARTITION_NAME_TAG
 from dagster._core.workspace.context import (
     BaseWorkspaceRequestContext,
     IWorkspaceProcessContext,
 )
 from dagster._utils import hash_collection, utc_datetime_from_timestamp
 from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
@@ -124,14 +128,24 @@
         return (
             (
                 self.materialized_subset | self.failed_and_downstream_subset
             ).num_partitions_and_non_partitioned_assets
             == self.target_subset.num_partitions_and_non_partitioned_assets
         )
 
+    def have_all_requested_runs_finished(self) -> bool:
+        for partition in self.requested_subset.iterate_asset_partitions():
+            if (
+                partition not in self.materialized_subset
+                and partition not in self.failed_and_downstream_subset
+            ):
+                return False
+
+        return True
+
     def get_target_root_asset_partitions(self) -> Iterable[AssetKeyPartitionKey]:
         root_asset_keys = (
             AssetSelection.keys(*self.target_subset.asset_keys)
             .sources()
             .resolve(self.target_subset.asset_graph)
         )
         return list(
@@ -388,79 +402,184 @@
             "serialized_failed_subset": self.failed_and_downstream_subset.to_storage_dict(
                 dynamic_partitions_store=dynamic_partitions_store
             ),
         }
         return json.dumps(storage_dict)
 
 
+def fetch_cancelable_run_ids_for_asset_backfill(instance: DagsterInstance, backfill_id: str):
+    backfill_runs = instance.run_storage.get_runs(
+        filters=RunsFilter(
+            tags={
+                BACKFILL_ID_TAG: backfill_id,
+            }
+        )
+    )
+    return [run.run_id for run in backfill_runs if run.status in CANCELABLE_RUN_STATUSES]
+
+
 def execute_asset_backfill_iteration(
     backfill: "PartitionBackfill",
     workspace_process_context: IWorkspaceProcessContext,
     instance: DagsterInstance,
 ) -> Iterable[None]:
     """Runs an iteration of the backfill, including submitting runs and updating the backfill object
     in the DB.
 
     This is a generator so that we can return control to the daemon and let it heartbeat during
     expensive operations.
     """
-    from dagster._core.execution.backfill import BulkActionStatus
+    from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
 
     asset_graph = ExternalAssetGraph.from_workspace(
         workspace_process_context.create_request_context()
     )
     if backfill.serialized_asset_backfill_data is None:
         check.failed("Asset backfill missing serialized_asset_backfill_data")
 
     asset_backfill_data = AssetBackfillData.from_serialized(
         backfill.serialized_asset_backfill_data, asset_graph, backfill.backfill_timestamp
     )
+    backfill_start_time = utc_datetime_from_timestamp(backfill.backfill_timestamp)
 
-    result = None
-    for result in execute_asset_backfill_iteration_inner(
-        backfill_id=backfill.backfill_id,
-        asset_backfill_data=asset_backfill_data,
-        instance=instance,
-        asset_graph=asset_graph,
-        run_tags=backfill.tags,
-        backfill_start_time=utc_datetime_from_timestamp(backfill.backfill_timestamp),
-    ):
-        yield None
+    instance_queryer = CachingInstanceQueryer(
+        instance=instance, evaluation_time=backfill_start_time
+    )
 
-    if not isinstance(result, AssetBackfillIterationResult):
-        check.failed(
-            "Expected execute_asset_backfill_iteration_inner to return an"
-            " AssetBackfillIterationResult"
-        )
+    if backfill.status == BulkActionStatus.REQUESTED:
+        result = None
+        for result in execute_asset_backfill_iteration_inner(
+            backfill_id=backfill.backfill_id,
+            asset_backfill_data=asset_backfill_data,
+            instance_queryer=instance_queryer,
+            asset_graph=asset_graph,
+            run_tags=backfill.tags,
+            backfill_start_time=backfill_start_time,
+        ):
+            yield None
 
-    updated_backfill = backfill.with_asset_backfill_data(
-        result.backfill_data, dynamic_partitions_store=instance
-    )
-    if result.backfill_data.is_complete():
-        # The asset backfill is complete when all runs to be requested have finished (success,
+        if not isinstance(result, AssetBackfillIterationResult):
+            check.failed(
+                "Expected execute_asset_backfill_iteration_inner to return an"
+                " AssetBackfillIterationResult"
+            )
+
+        pipeline_and_execution_plan_cache: Dict[int, Tuple[ExternalJob, ExternalExecutionPlan]] = {}
+        for run_request in result.run_requests:
+            yield None
+            submit_run_request(
+                run_request=run_request,
+                asset_graph=asset_graph,
+                # create a new request context for each run in case the code location server
+                # is swapped out in the middle of the backfill
+                workspace=workspace_process_context.create_request_context(),
+                instance=instance,
+                pipeline_and_execution_plan_cache=pipeline_and_execution_plan_cache,
+            )
+
+        if result.backfill_data.is_complete():
+            # The asset backfill is complete when all runs to be requested have finished (success,
+            # failure, or cancellation). Since the AssetBackfillData object stores materialization states
+            # per asset partition, the daemon continues to update the backfill data until all runs have
+            # finished in order to display the final partition statuses in the UI.
+            updated_backfill = backfill.with_asset_backfill_data(
+                result.backfill_data, dynamic_partitions_store=instance
+            )
+            updated_backfill = updated_backfill.with_status(BulkActionStatus.COMPLETED)
+        else:
+            # refetch, in case the backfill was canceled in the meantime
+            backfill = cast(PartitionBackfill, instance.get_backfill(backfill.backfill_id))
+            updated_backfill = backfill.with_asset_backfill_data(
+                result.backfill_data, dynamic_partitions_store=instance
+            )
+
+        instance.update_backfill(updated_backfill)
+
+    elif backfill.status == BulkActionStatus.CANCELING:
+        # Find all cancellable runs and mark them as canceled
+        cancelable_run_ids = fetch_cancelable_run_ids_for_asset_backfill(
+            instance, backfill.backfill_id
+        )
+        if cancelable_run_ids:
+            if not instance.run_coordinator:
+                check.failed("The instance must have a run coordinator in order to cancel runs")
+            for run_id in cancelable_run_ids:
+                instance.run_coordinator.cancel_run(run_id)
+
+        # Update the asset backfill data to contain the newly materialized/failed partitions.
+        updated_asset_backfill_data = None
+        for updated_asset_backfill_data in get_canceling_asset_backfill_iteration_data(
+            backfill.backfill_id,
+            asset_backfill_data,
+            instance_queryer,
+            asset_graph,
+            backfill_start_time,
+        ):
+            yield None
+
+        if not isinstance(updated_asset_backfill_data, AssetBackfillData):
+            check.failed(
+                "Expected get_canceling_asset_backfill_iteration_data to return a PartitionBackfill"
+            )
+
+        updated_backfill = backfill.with_asset_backfill_data(
+            updated_asset_backfill_data, dynamic_partitions_store=instance
+        )
+        # The asset backfill is successfully canceled when all requested runs have finished (success,
         # failure, or cancellation). Since the AssetBackfillData object stores materialization states
         # per asset partition, the daemon continues to update the backfill data until all runs have
         # finished in order to display the final partition statuses in the UI.
-        updated_backfill = updated_backfill.with_status(BulkActionStatus.COMPLETED)
+        if updated_asset_backfill_data.have_all_requested_runs_finished():
+            updated_backfill = updated_backfill.with_status(BulkActionStatus.CANCELED)
+
+        instance.update_backfill(updated_backfill)
+    else:
+        check.failed(f"Unexpected backfill status: {backfill.status}")
 
-    pipeline_and_execution_plan_cache: Dict[int, Tuple[ExternalJob, ExternalExecutionPlan]] = {}
 
-    for run_request in result.run_requests:
+def get_canceling_asset_backfill_iteration_data(
+    backfill_id: str,
+    asset_backfill_data: AssetBackfillData,
+    instance_queryer: CachingInstanceQueryer,
+    asset_graph: ExternalAssetGraph,
+    backfill_start_time: datetime,
+) -> Iterable[Optional[AssetBackfillData]]:
+    """For asset backfills in the "canceling" state, fetch the asset backfill data with the updated
+    materialized and failed subsets.
+    """
+    updated_materialized_subset = None
+    for updated_materialized_subset in get_asset_backfill_iteration_materialized_partitions(
+        backfill_id, asset_backfill_data, asset_graph, instance_queryer
+    ):
         yield None
-        submit_run_request(
-            run_request=run_request,
-            asset_graph=asset_graph,
-            # create a new request context for each run in case the code location server
-            # is swapped out in the middle of the backfill
-            workspace=workspace_process_context.create_request_context(),
-            instance=instance,
-            pipeline_and_execution_plan_cache=pipeline_and_execution_plan_cache,
+
+    if not isinstance(updated_materialized_subset, AssetGraphSubset):
+        check.failed(
+            "Expected get_asset_backfill_iteration_materialized_partitions to return an"
+            " AssetGraphSubset"
         )
 
-    instance.update_backfill(updated_backfill)
+    failed_and_downstream_subset = _get_failed_and_downstream_asset_partitions(
+        backfill_id,
+        asset_backfill_data,
+        asset_graph,
+        instance_queryer,
+        backfill_start_time,
+    )
+    updated_backfill_data = AssetBackfillData(
+        target_subset=asset_backfill_data.target_subset,
+        latest_storage_id=asset_backfill_data.latest_storage_id,
+        requested_runs_for_target_roots=asset_backfill_data.requested_runs_for_target_roots,
+        materialized_subset=updated_materialized_subset,
+        failed_and_downstream_subset=failed_and_downstream_subset,
+        requested_subset=asset_backfill_data.requested_subset,
+        backfill_start_time=backfill_start_time,
+    )
+
+    yield updated_backfill_data
 
 
 def submit_run_request(
     asset_graph: ExternalAssetGraph,
     run_request: RunRequest,
     instance: DagsterInstance,
     workspace: BaseWorkspaceRequestContext,
@@ -545,34 +664,88 @@
 
 
 class AssetBackfillIterationResult(NamedTuple):
     run_requests: Sequence[RunRequest]
     backfill_data: AssetBackfillData
 
 
+def get_asset_backfill_iteration_materialized_partitions(
+    backfill_id: str,
+    asset_backfill_data: AssetBackfillData,
+    asset_graph: ExternalAssetGraph,
+    instance_queryer: CachingInstanceQueryer,
+) -> Iterable[Optional[AssetGraphSubset]]:
+    """Returns the partitions that have been materialized by the backfill.
+
+    This function is a generator so we can return control to the daemon and let it heartbeat
+    during expensive operations.
+    """
+    recently_materialized_asset_partitions = AssetGraphSubset(asset_graph)
+    for asset_key in asset_backfill_data.target_subset.asset_keys:
+        records = instance_queryer.get_materialization_records(
+            asset_key=asset_key, after_cursor=asset_backfill_data.latest_storage_id
+        )
+        records_in_backfill = [
+            record
+            for record in records
+            if instance_queryer.run_has_tag(
+                run_id=record.run_id, tag_key=BACKFILL_ID_TAG, tag_value=backfill_id
+            )
+        ]
+        recently_materialized_asset_partitions |= {
+            AssetKeyPartitionKey(asset_key, record.partition_key) for record in records_in_backfill
+        }
+
+        yield None
+
+    updated_materialized_subset = (
+        asset_backfill_data.materialized_subset | recently_materialized_asset_partitions
+    )
+
+    yield updated_materialized_subset
+
+
+def _get_failed_and_downstream_asset_partitions(
+    backfill_id: str,
+    asset_backfill_data: AssetBackfillData,
+    asset_graph: ExternalAssetGraph,
+    instance_queryer: CachingInstanceQueryer,
+    backfill_start_time: datetime,
+) -> AssetGraphSubset:
+    failed_and_downstream_subset = AssetGraphSubset.from_asset_partition_set(
+        asset_graph.bfs_filter_asset_partitions(
+            instance_queryer,
+            lambda asset_partitions, _: any(
+                asset_partition in asset_backfill_data.target_subset
+                for asset_partition in asset_partitions
+            ),
+            _get_failed_asset_partitions(instance_queryer, backfill_id),
+            evaluation_time=backfill_start_time,
+        ),
+        asset_graph,
+    )
+    return failed_and_downstream_subset
+
+
 def execute_asset_backfill_iteration_inner(
     backfill_id: str,
     asset_backfill_data: AssetBackfillData,
     asset_graph: ExternalAssetGraph,
-    instance: DagsterInstance,
+    instance_queryer: CachingInstanceQueryer,
     run_tags: Mapping[str, str],
     backfill_start_time: datetime,
 ) -> Iterable[Optional[AssetBackfillIterationResult]]:
     """Core logic of a backfill iteration. Has no side effects.
 
     Computes which runs should be requested, if any, as well as updated bookkeeping about the status
     of asset partitions targeted by the backfill.
 
     This is a generator so that we can return control to the daemon and let it heartbeat during
     expensive operations.
     """
-    instance_queryer = CachingInstanceQueryer(
-        instance=instance, evaluation_time=backfill_start_time
-    )
-
     initial_candidates: Set[AssetKeyPartitionKey] = set()
     request_roots = not asset_backfill_data.requested_runs_for_target_roots
     if request_roots:
         initial_candidates.update(asset_backfill_data.get_target_root_asset_partitions())
 
         next_latest_storage_id = instance_queryer.get_latest_storage_id(
             DagsterEventType.ASSET_MATERIALIZATION
@@ -598,48 +771,28 @@
             target_asset_keys_and_parents=target_asset_keys_and_parents,
             latest_storage_id=asset_backfill_data.latest_storage_id,
         )
         initial_candidates.update(parent_materialized_asset_partitions)
 
         yield None
 
-        recently_materialized_asset_partitions = AssetGraphSubset(asset_graph)
-        for asset_key in asset_backfill_data.target_subset.asset_keys:
-            records = instance_queryer.get_materialization_records(
-                asset_key=asset_key, after_cursor=asset_backfill_data.latest_storage_id
-            )
-            records_in_backfill = [
-                record
-                for record in records
-                if instance_queryer.run_has_tag(
-                    run_id=record.run_id, tag_key=BACKFILL_ID_TAG, tag_value=backfill_id
-                )
-            ]
-            recently_materialized_asset_partitions |= {
-                AssetKeyPartitionKey(asset_key, record.partition_key)
-                for record in records_in_backfill
-            }
-
+        updated_materialized_subset = None
+        for updated_materialized_subset in get_asset_backfill_iteration_materialized_partitions(
+            backfill_id, asset_backfill_data, asset_graph, instance_queryer
+        ):
             yield None
 
-        updated_materialized_subset = (
-            asset_backfill_data.materialized_subset | recently_materialized_asset_partitions
-        )
+        if not isinstance(updated_materialized_subset, AssetGraphSubset):
+            check.failed(
+                "Expected get_asset_backfill_iteration_materialized_partitions to return an"
+                " AssetGraphSubset"
+            )
 
-        failed_and_downstream_subset = AssetGraphSubset.from_asset_partition_set(
-            asset_graph.bfs_filter_asset_partitions(
-                instance_queryer,
-                lambda asset_partitions, _: any(
-                    asset_partition in asset_backfill_data.target_subset
-                    for asset_partition in asset_partitions
-                ),
-                _get_failed_asset_partitions(instance_queryer, backfill_id),
-                evaluation_time=backfill_start_time,
-            ),
-            asset_graph,
+        failed_and_downstream_subset = _get_failed_and_downstream_asset_partitions(
+            backfill_id, asset_backfill_data, asset_graph, instance_queryer, backfill_start_time
         )
 
         yield None
 
     asset_partitions_to_request = asset_graph.bfs_filter_asset_partitions(
         instance_queryer,
         lambda unit, visited: should_backfill_atomic_asset_partitions_unit(
```

### Comparing `dagster-1.3.6/dagster/_core/execution/backfill.py` & `dagster-1.3.7/dagster/_core/execution/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 
 @whitelist_for_serdes
 class BulkActionStatus(Enum):
     REQUESTED = "REQUESTED"
     COMPLETED = "COMPLETED"
     FAILED = "FAILED"
+    CANCELING = "CANCELING"
     CANCELED = "CANCELED"
 
     @staticmethod
     def from_graphql_input(graphql_str):
         return BulkActionStatus(graphql_str)
 
 
@@ -221,14 +222,19 @@
         else:
             if self.partition_names is None:
                 check.failed("Non-asset backfills should have a non-null partition_names field")
 
             return self.partition_names
 
     def get_num_cancelable(self) -> int:
+        """This method is only valid for job backfills. It eturns the number of partitions that are have
+        not yet been requested by the backfill.
+
+        For asset backfills, returns 0.
+        """
         if self.is_asset_backfill:
             return 0
 
         if self.status != BulkActionStatus.REQUESTED:
             return 0
 
         if self.partition_names is None:
```

### Comparing `dagster-1.3.6/dagster/_core/execution/build_resources.py` & `dagster-1.3.7/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/compute_logs.py` & `dagster-1.3.7/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/context/compute.py` & `dagster-1.3.7/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/context/hook.py` & `dagster-1.3.7/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/context/init.py` & `dagster-1.3.7/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/context/input.py` & `dagster-1.3.7/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/context/invocation.py` & `dagster-1.3.7/dagster/_core/execution/context/invocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,21 +116,20 @@
 
     def __enter__(self):
         self._cm_scope_entered = True
         return self
 
     def __exit__(self, *exc):
         self._resources_cm.__exit__(*exc)
-        if self._instance_provided:
-            self._instance_cm.__exit__(*exc)
+        self._instance_cm.__exit__(*exc)
 
     def __del__(self):
         if self._resources_contain_cm and not self._cm_scope_entered:
             self._resources_cm.__exit__(None, None, None)
-        if self._instance_provided and not self._cm_scope_entered:
+        if not self._cm_scope_entered:
             self._instance_cm.__exit__(None, None, None)
 
     @property
     def op_config(self) -> Any:
         return self._op_config
 
     @property
```

### Comparing `dagster-1.3.6/dagster/_core/execution/context/logger.py` & `dagster-1.3.7/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/context/output.py` & `dagster-1.3.7/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/context/system.py` & `dagster-1.3.7/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/context_creation_job.py` & `dagster-1.3.7/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.7/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.7/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/execution_result.py` & `dagster-1.3.7/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/host_mode.py` & `dagster-1.3.7/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/job_backfill.py` & `dagster-1.3.7/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/job_execution_result.py` & `dagster-1.3.7/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/memoization.py` & `dagster-1.3.7/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/active.py` & `dagster-1.3.7/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/compute.py` & `dagster-1.3.7/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.7/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.7/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.7/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.7/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/handle.py` & `dagster-1.3.7/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.7/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.7/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/objects.py` & `dagster-1.3.7/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.7/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/plan.py` & `dagster-1.3.7/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/state.py` & `dagster-1.3.7/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/step.py` & `dagster-1.3.7/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/plan/utils.py` & `dagster-1.3.7/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.7/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.7/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/resources_init.py` & `dagster-1.3.7/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/retries.py` & `dagster-1.3.7/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.7/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/stats.py` & `dagster-1.3.7/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/tags.py` & `dagster-1.3.7/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.7/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.7/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/execution/with_resources.py` & `dagster-1.3.7/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/executor/base.py` & `dagster-1.3.7/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.7/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/executor/in_process.py` & `dagster-1.3.7/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/executor/init.py` & `dagster-1.3.7/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/executor/multiprocess.py` & `dagster-1.3.7/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.7/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.7/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/__init__.py` & `dagster-1.3.7/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/code_location.py` & `dagster-1.3.7/dagster/_core/host_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/external.py` & `dagster-1.3.7/dagster/_core/host_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/external_data.py` & `dagster-1.3.7/dagster/_core/host_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.7/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.7/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/handle.py` & `dagster-1.3.7/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/historical.py` & `dagster-1.3.7/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/job_index.py` & `dagster-1.3.7/dagster/_core/host_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/origin.py` & `dagster-1.3.7/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/host_representation/represented.py` & `dagster-1.3.7/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/instance/__init__.py` & `dagster-1.3.7/dagster/_core/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/instance/config.py` & `dagster-1.3.7/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/instance/ref.py` & `dagster-1.3.7/dagster/_core/instance/ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,29 +552,24 @@
         return (
             self.run_launcher_data.rehydrate(as_type=RunLauncher)
             if self.run_launcher_data
             else None
         )
 
     @property
-    def secrets_loader(self) -> "SecretsLoader":
-        from dagster._core.secrets.env_file import EnvFileLoader
+    def secrets_loader(self) -> Optional["SecretsLoader"]:
         from dagster._core.secrets.loader import SecretsLoader
 
         # Defining a default here rather than in stored config to avoid
         # back-compat issues when loading the config on older versions where
         # EnvFileLoader was not defined
         return (
             self.secrets_loader_data.rehydrate(as_type=SecretsLoader)
             if self.secrets_loader_data
-            else ConfigurableClassData(
-                "dagster._core.secrets.env_file",
-                "EnvFileLoader",
-                yaml.dump({}),
-            ).rehydrate(as_type=EnvFileLoader)
+            else None
         )
 
     @property
     def custom_instance_class(self) -> Type["DagsterInstance"]:
         return (  # type: ignore  # (ambiguous return type)
             class_from_code_pointer(
                 self.custom_instance_class_data.module_name,
```

### Comparing `dagster-1.3.6/dagster/_core/instance_for_test.py` & `dagster-1.3.7/dagster/_core/instance_for_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,42 +4,20 @@
 from contextlib import ExitStack, contextmanager
 from typing import Any, Iterator, Mapping, Optional
 
 import yaml
 
 from dagster._utils.error import serializable_error_info_from_exc_info
 
+from .._utils.env import environ
 from .._utils.merger import merge_dicts
 from .instance import DagsterInstance
 
 
 @contextmanager
-def environ(env: Mapping[str, str]) -> Iterator[None]:
-    """Temporarily set environment variables inside the context manager and
-    fully restore previous environment afterwards.
-    """
-    previous_values = {key: os.getenv(key) for key in env}
-    for key, value in env.items():
-        if value is None:
-            if key in os.environ:
-                del os.environ[key]
-        else:
-            os.environ[key] = value
-    try:
-        yield
-    finally:
-        for key, value in previous_values.items():
-            if value is None:
-                if key in os.environ:
-                    del os.environ[key]
-            else:
-                os.environ[key] = value
-
-
-@contextmanager
 def instance_for_test(
     overrides: Optional[Mapping[str, Any]] = None,
     set_dagster_home: bool = True,
     temp_dir: Optional[str] = None,
 ) -> Iterator[DagsterInstance]:
     """Creates a persistent :py:class:`~dagster.DagsterInstance` available within a context manager.
```

### Comparing `dagster-1.3.6/dagster/_core/launcher/base.py` & `dagster-1.3.7/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.7/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.7/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/log_manager.py` & `dagster-1.3.7/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/nux.py` & `dagster-1.3.7/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/origin.py` & `dagster-1.3.7/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/run_coordinator/base.py` & `dagster-1.3.7/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.7/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.7/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/scheduler/__init__.py` & `dagster-1.3.7/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/scheduler/execution.py` & `dagster-1.3.7/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/scheduler/instigation.py` & `dagster-1.3.7/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.7/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/secrets/env_file.py` & `dagster-1.3.7/dagster/_core/secrets/env_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import logging
 import os
 from typing import Any, Dict, Mapping, Optional
 
 from dotenv import dotenv_values
 from typing_extensions import Self
 
-import dagster._check as check
 from dagster._config import Field, StringSource
 from dagster._serdes import ConfigurableClass
 from dagster._serdes.config_class import ConfigurableClassData
 
 from .loader import SecretsLoader
 
 
+def get_env_var_dict(base_dir: str) -> Dict[str, str]:
+    env_file_path = os.path.join(base_dir, ".env")
+    if not os.path.exists(env_file_path):
+        return {}
+
+    return {key: val for key, val in dotenv_values(env_file_path).items() if val is not None}
+
+
 class EnvFileLoader(SecretsLoader, ConfigurableClass):
     def __init__(
         self,
         inst_data: Optional[ConfigurableClassData] = None,
         base_dir=None,
     ):
         self._inst_data = inst_data
         self._base_dir = base_dir or os.getcwd()
 
     def get_secrets_for_environment(self, location_name: Optional[str]) -> Dict[str, str]:
         env_file_path = os.path.join(self._base_dir, ".env")
 
-        if not os.path.exists(env_file_path):
-            return {}
-
-        env_var_dict: Dict[str, str] = {
-            key: check.not_none(val)
-            for key, val in dotenv_values(env_file_path).items()
-            if val is not None
-        }
+        env_var_dict = get_env_var_dict(env_file_path)
 
         if len(env_var_dict):
             logging.getLogger("dagster").info(
                 "Loaded environment variables from .env file: "
                 + ",".join([env_var for env_var in env_var_dict]),
             )
         else:
```

### Comparing `dagster-1.3.6/dagster/_core/selector/subset_selector.py` & `dagster-1.3.7/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/snap/__init__.py` & `dagster-1.3.7/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/snap/dagster_types.py` & `dagster-1.3.7/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.7/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.7/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/snap/job_snapshot.py` & `dagster-1.3.7/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/snap/mode.py` & `dagster-1.3.7/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/snap/node.py` & `dagster-1.3.7/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.3.7/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.7/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/README.md` & `dagster-1.3.7/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/env.py` & `dagster-1.3.7/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.3.7/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.7/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/base_storage.py` & `dagster-1.3.7/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.7/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.7/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.7/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.7/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/config.py` & `dagster-1.3.7/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/dagster_run.py` & `dagster-1.3.7/dagster/_core/storage/dagster_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,21 @@
 
 FINISHED_STATUSES = [
     DagsterRunStatus.SUCCESS,
     DagsterRunStatus.FAILURE,
     DagsterRunStatus.CANCELED,
 ]
 
+# Run statuses for runs that can be safely canceled.
+# Does not include the other unfinished statuses for the following reasons:
+# STARTING: Control has been ceded to the run worker, which will eventually move the run to a STARTED.
+# NOT_STARTED: Mostly replaced with STARTING. Runs are only here in the the brief window between
+# creating the run and launching or enqueueing it.
+CANCELABLE_RUN_STATUSES = [DagsterRunStatus.STARTED, DagsterRunStatus.QUEUED]
+
 
 @whitelist_for_serdes(storage_name="PipelineRunStatsSnapshot")
 class DagsterRunStatsSnapshot(
     NamedTuple(
         "_DagsterRunStatsSnapshot",
         [
             ("run_id", str),
```

### Comparing `dagster-1.3.6/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.7/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.7/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/base.py` & `dagster-1.3.7/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.3.7/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.7/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.7/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.7/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.3.7/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/file_manager.py` & `dagster-1.3.7/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.7/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/input_manager.py` & `dagster-1.3.7/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/io_manager.py` & `dagster-1.3.7/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.7/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.7/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.7/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.7/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/migration/utils.py` & `dagster-1.3.7/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.7/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/output_manager.py` & `dagster-1.3.7/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.7/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/root.py` & `dagster-1.3.7/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.7/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/runs/base.py` & `dagster-1.3.7/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.7/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/runs/migration.py` & `dagster-1.3.7/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/runs/schema.py` & `dagster-1.3.7/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.7/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/schedules/base.py` & `dagster-1.3.7/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.7/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.7/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.7/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/sql.py` & `dagster-1.3.7/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/sqlite.py` & `dagster-1.3.7/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.7/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/tags.py` & `dagster-1.3.7/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.7/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.7/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.7/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/system_config/objects.py` & `dagster-1.3.7/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/telemetry.py` & `dagster-1.3.7/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/telemetry_upload.py` & `dagster-1.3.7/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/test_utils.py` & `dagster-1.3.7/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.7/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/config_schema.py` & `dagster-1.3.7/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/dagster_type.py` & `dagster-1.3.7/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/decorator.py` & `dagster-1.3.7/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.7/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.7/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/python_dict.py` & `dagster-1.3.7/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/python_set.py` & `dagster-1.3.7/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/python_tuple.py` & `dagster-1.3.7/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/types/transform_typing.py` & `dagster-1.3.7/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/utility_ops.py` & `dagster-1.3.7/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/utils.py` & `dagster-1.3.7/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.7/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/workspace/config_schema.py` & `dagster-1.3.7/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/workspace/context.py` & `dagster-1.3.7/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/workspace/load.py` & `dagster-1.3.7/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/workspace/load_target.py` & `dagster-1.3.7/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/workspace/permissions.py` & `dagster-1.3.7/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_core/workspace/workspace.py` & `dagster-1.3.7/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/__init__.py` & `dagster-1.3.7/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/asset_daemon.py` & `dagster-1.3.7/dagster/_daemon/asset_daemon.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,25 @@
     ) -> DaemonIterator:
         instance = workspace_process_context.instance
 
         if get_auto_materialize_paused(instance):
             yield
             return
 
+        schedule_storage = check.not_none(
+            instance.schedule_storage,
+            "Auto materialization requires schedule storage to be configured",
+        )
+
+        if not schedule_storage.supports_auto_materialize_asset_evaluations:
+            self._logger.warning(
+                "Auto materialize evaluations are not getting logged. Run `dagster instance"
+                " migrate` to enable."
+            )
+
         workspace = workspace_process_context.create_request_context()
         asset_graph = ExternalAssetGraph.from_workspace(workspace)
         target_asset_keys = {
             target_key
             for target_key in asset_graph.non_source_asset_keys
             if asset_graph.get_auto_materialize_policy(target_key) is not None
         }
@@ -137,7 +148,14 @@
                 external_job_origin=external_job.get_external_origin(),
                 job_code_origin=external_job.get_python_origin(),
                 asset_selection=frozenset(asset_keys),
             )
             instance.submit_run(run.run_id, workspace)
 
         instance.daemon_cursor_storage.set_cursor_values({CURSOR_KEY: new_cursor.serialize()})
+
+        # We enforce uniqueness per (asset key, evaluation id). Store the evaluations after the cursor,
+        # so that if the daemon crashes and doesn't update the cursor we don't try to write duplicates.
+        if schedule_storage.supports_auto_materialize_asset_evaluations:
+            schedule_storage.add_auto_materialize_asset_evaluations(
+                check.not_none(new_cursor.evaluation_id), evaluations
+            )
```

### Comparing `dagster-1.3.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/backfill.py` & `dagster-1.3.7/dagster/_daemon/backfill.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 
 def execute_backfill_iteration(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     debug_crash_flags: Optional[Mapping[str, int]] = None,
 ) -> Iterable[Optional[SerializableErrorInfo]]:
     instance = workspace_process_context.instance
-    backfills = instance.get_backfills(status=BulkActionStatus.REQUESTED)
 
-    if not backfills:
-        logger.debug("No backfill jobs requested.")
+    in_progress_backfills = instance.get_backfills(status=BulkActionStatus.REQUESTED)
+    canceling_backfills = instance.get_backfills(status=BulkActionStatus.CANCELING)
+
+    if not in_progress_backfills and not canceling_backfills:
+        logger.debug("No backfill jobs in progress or canceling.")
         yield None
         return
 
-    for backfill_job in backfills:
+    for backfill_job in [*in_progress_backfills, *canceling_backfills]:
         backfill_id = backfill_job.backfill_id
 
         # refetch, in case the backfill was updated in the meantime
         backfill = cast(PartitionBackfill, instance.get_backfill(backfill_id))
         try:
             if backfill.is_asset_backfill:
                 yield from execute_asset_backfill_iteration(
```

### Comparing `dagster-1.3.6/dagster/_daemon/cli/__init__.py` & `dagster-1.3.7/dagster/_daemon/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 from typing import Optional
 
 import click
 
 from dagster import __version__ as dagster_version
+from dagster._cli.utils import get_instance_for_cli
 from dagster._cli.workspace.cli_target import (
     ClickArgMapping,
     ClickArgValue,
     get_workspace_load_target,
     workspace_target_argument,
 )
 from dagster._core.instance import DagsterInstance, InstanceRef
@@ -54,17 +55,17 @@
 def run_command(
     code_server_log_level: str,
     instance_ref: Optional[str],
     **kwargs: ClickArgValue,
 ) -> None:
     try:
         with capture_interrupts():
-            with DagsterInstance.from_ref(
-                deserialize_value(instance_ref, InstanceRef)
-            ) if instance_ref else DagsterInstance.get() as instance:
+            with get_instance_for_cli(
+                instance_ref=deserialize_value(instance_ref, InstanceRef) if instance_ref else None
+            ) as instance:
                 _daemon_run_command(instance, code_server_log_level, kwargs)
     except KeyboardInterrupt:
         return  # Exit cleanly on interrupt
 
 
 @telemetry_wrapper(metadata={"DAEMON_SESSION_ID": get_telemetry_daemon_session_id()})
 def _daemon_run_command(
@@ -82,47 +83,47 @@
 
 
 @click.command(
     name="liveness-check",
     help="Check for recent heartbeats from the daemon.",
 )
 def liveness_check_command() -> None:
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         if all_daemons_live(instance, heartbeat_tolerance_seconds=_get_heartbeat_tolerance()):
             click.echo("Daemon live")
         else:
             click.echo("Daemon(s) not running")
             sys.exit(1)
 
 
 @click.command(
     name="wipe",
     help="Wipe all heartbeats from storage.",
 )
 def wipe_command() -> None:
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         instance.wipe_daemon_heartbeats()
         click.echo("Daemon heartbeats wiped")
 
 
 @click.command(
     name="heartbeat",
     help="Read and write a heartbeat",
 )
 def debug_heartbeat_command() -> None:
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         debug_daemon_heartbeats(instance)
 
 
 @click.command(
     name="heartbeat-dump",
     help="Log all heartbeat statuses",
 )
 def debug_heartbeat_dump_command() -> None:
-    with DagsterInstance.get() as instance:
+    with get_instance_for_cli() as instance:
         for daemon_status in get_daemon_statuses(instance, instance.get_required_daemon_types()):
             click.echo(daemon_status)
 
 
 @click.group(
     commands={"heartbeat": debug_heartbeat_command, "heartbeat-dump": debug_heartbeat_dump_command}
 )
```

### Comparing `dagster-1.3.6/dagster/_daemon/controller.py` & `dagster-1.3.7/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/daemon.py` & `dagster-1.3.7/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.3.7/dagster/_daemon/monitoring/monitoring_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/sensor.py` & `dagster-1.3.7/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/types.py` & `dagster-1.3.7/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_daemon/workspace.py` & `dagster-1.3.7/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_generate/download.py` & `dagster-1.3.7/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_generate/generate.py` & `dagster-1.3.7/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.3.7/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.7/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/__init__.py` & `dagster-1.3.7/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/client.py` & `dagster-1.3.7/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/compile.py` & `dagster-1.3.7/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/impl.py` & `dagster-1.3.7/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/protos/api.proto` & `dagster-1.3.7/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/proxy_server.py` & `dagster-1.3.7/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/server.py` & `dagster-1.3.7/dagster/_grpc/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import queue
 import sys
 import threading
 import time
 import uuid
 import warnings
 from concurrent.futures import ThreadPoolExecutor
+from contextlib import ExitStack
 from multiprocessing.synchronize import Event as MPEvent
 from subprocess import Popen
 from threading import Event as ThreadingEventType
 from time import sleep
 from typing import Any, Dict, Iterator, List, Mapping, Optional, Sequence, Tuple, cast
 
 import grpc
@@ -257,23 +258,26 @@
         #  - When running `dagster dev` (or `dagit`) in the gRPC server subprocesses that are spun up
         #  - When running code in Dagster Cloud on 1.1 or later
         # When will it not be set?
         #  - When running your own grpc server with `dagster api grpc`
         #  - When using an integration that spins up gRPC servers (for example, the Dagster Helm
         #    chart or the deploy_docker example)
         self._instance_ref = check.opt_inst_param(instance_ref, "instance_ref", InstanceRef)
+        self._exit_stack = ExitStack()
 
         try:
             if inject_env_vars_from_instance:
+                from dagster._cli.utils import get_instance_for_cli
+
                 # If arguments indicate it wants to load env vars, use the passed-in instance
                 # ref (or the dagster.yaml on the filesystem if no instance ref is provided)
-                with DagsterInstance.from_ref(
-                    instance_ref
-                ) if instance_ref else DagsterInstance.get() as instance:
-                    instance.inject_env_vars(location_name)
+                self._instance = self._exit_stack.enter_context(
+                    get_instance_for_cli(instance_ref=instance_ref)
+                )
+                self._instance.inject_env_vars(location_name)
 
             self._loaded_repositories: Optional[LoadedRepositories] = LoadedRepositories(
                 loadable_target_origin,
                 self._entry_point,
                 self._container_image,
             )
         except Exception:
@@ -305,14 +309,16 @@
     def cleanup(self) -> None:
         # In case ShutdownServer was not called
         self._shutdown_once_executions_finish_event.set()
         if self.__heartbeat_thread:
             self.__heartbeat_thread.join()
         self.__cleanup_thread.join()
 
+        self._exit_stack.close()
+
     def _heartbeat_thread(self, heartbeat_timeout: float) -> None:
         while True:
             self._shutdown_once_executions_finish_event.wait(heartbeat_timeout)
             if self._shutdown_once_executions_finish_event.is_set():
                 break
 
             if self.__last_heartbeat_time < time.time() - heartbeat_timeout:
```

### Comparing `dagster-1.3.6/dagster/_grpc/server_watcher.py` & `dagster-1.3.7/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/types.py` & `dagster-1.3.7/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_grpc/utils.py` & `dagster-1.3.7/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_loggers/__init__.py` & `dagster-1.3.7/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_module_alias_map.py` & `dagster-1.3.7/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_scheduler/scheduler.py` & `dagster-1.3.7/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_scheduler/stale.py` & `dagster-1.3.7/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_serdes/__init__.py` & `dagster-1.3.7/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_serdes/config_class.py` & `dagster-1.3.7/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_serdes/ipc.py` & `dagster-1.3.7/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_serdes/serdes.py` & `dagster-1.3.7/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_serdes/utils.py` & `dagster-1.3.7/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_seven/__init__.py` & `dagster-1.3.7/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_seven/abc.py` & `dagster-1.3.7/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_seven/compat/pendulum.py` & `dagster-1.3.7/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/__init__.py` & `dagster-1.3.7/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/alert.py` & `dagster-1.3.7/dagster/_utils/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         default_status=default_status,
         monitor_all_repositories=monitor_all_repositories,
     )
     def email_on_run_failure(context: RunFailureSensorContext):
         email_body = email_body_fn(context)
         if dagit_base_url:
             email_body += (
-                f'<p><a href="{dagit_base_url}/instance/runs/{context.dagster_run.run_id}">View in'
+                f'<p><a href="{dagit_base_url}/runs/{context.dagster_run.run_id}">View in'
                 " Dagit</a></p>"
             )
 
         message = EMAIL_MESSAGE.format(
             email_to=",".join(email_to),
             email_from=email_from,
             email_subject=email_subject_fn(context),
```

### Comparing `dagster-1.3.6/dagster/_utils/backcompat.py` & `dagster-1.3.7/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/backoff.py` & `dagster-1.3.7/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/cached_method.py` & `dagster-1.3.7/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.7/dagster/_utils/caching_instance_queryer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/dagster_type.py` & `dagster-1.3.7/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/error.py` & `dagster-1.3.7/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/external.py` & `dagster-1.3.7/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/forked_pdb.py` & `dagster-1.3.7/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/hosted_user_process.py` & `dagster-1.3.7/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/indenting_printer.py` & `dagster-1.3.7/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/interrupts.py` & `dagster-1.3.7/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/log.py` & `dagster-1.3.7/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/merger.py` & `dagster-1.3.7/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/net.py` & `dagster-1.3.7/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/schedules.py` & `dagster-1.3.7/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/tags.py` & `dagster-1.3.7/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/temp_file.py` & `dagster-1.3.7/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/test/__init__.py` & `dagster-1.3.7/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.7/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.7/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.7/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/timing.py` & `dagster-1.3.7/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/typing_api.py` & `dagster-1.3.7/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster/_utils/yaml_utils.py` & `dagster-1.3.7/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.6/dagster.egg-info/PKG-INFO` & `dagster-1.3.7/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.6
+Version: 1.3.7
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.6/dagster.egg-info/SOURCES.txt` & `dagster-1.3.7/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -520,14 +520,15 @@
 dagster/_utils/__init__.py
 dagster/_utils/alert.py
 dagster/_utils/backcompat.py
 dagster/_utils/backoff.py
 dagster/_utils/cached_method.py
 dagster/_utils/caching_instance_queryer.py
 dagster/_utils/dagster_type.py
+dagster/_utils/env.py
 dagster/_utils/error.py
 dagster/_utils/external.py
 dagster/_utils/forked_pdb.py
 dagster/_utils/hosted_user_process.py
 dagster/_utils/indenting_printer.py
 dagster/_utils/internal_init.py
 dagster/_utils/interrupts.py
```

### Comparing `dagster-1.3.6/dagster.egg-info/requires.txt` & `dagster-1.3.7/dagster.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 click>=5.0
 coloredlogs<=14.0,>=6.1
 Jinja2
 PyYAML>=5.1
 alembic!=1.6.3,!=1.7.0,<1.11.0,>=1.2.1
 croniter>=0.3.34
-grpcio-health-checking>=1.44.0
 packaging>=20.9
 pendulum
 protobuf>=3.20.0
 python-dateutil
 python-dotenv
 pytz
 requests
@@ -26,20 +25,22 @@
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 grpcio<1.48.0,>=1.44.0
+grpcio-health-checking<1.48.0,>=1.44.0
 
 [:python_version < "3.7"]
 contextvars
 
 [:python_version >= "3.11"]
 grpcio>=1.44.0
+grpcio-health-checking>=1.44.0
 
 [black]
 black[jupyter]==22.12.0
 
 [docker]
 docker
 
@@ -70,24 +71,29 @@
 types-toml
 
 [ruff]
 ruff==0.0.255
 
 [test]
 docker
-grpcio-tools>=1.44.0
 mock==3.0.5
 objgraph
 pytest-cov==2.10.1
 pytest-dependency==0.5.1
 pytest-mock==3.3.1
 pytest-rerunfailures==10.0
 pytest-runner==5.2
 pytest-xdist==2.1.0
 pytest==7.0.1
 responses
 snapshottest==0.6.0
 tox==3.25.0
 yamllint
 
+[test:python_version < "3.11"]
+grpcio-tools<1.48.0,>=1.44.0
+
+[test:python_version >= "3.11"]
+grpcio-tools>=1.44.0
+
 [test:python_version >= "3.8"]
 buildkite-test-collector
```

### Comparing `dagster-1.3.6/setup.py` & `dagster-1.3.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,21 @@
     version: Dict[str, str] = {}
     with open(Path(__file__).parent / "dagster/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)
 
     return version["__version__"]
 
 
+# grpcio 1.44.0 is the min version compatible with both protobuf 3 and 4
+GRPC_VERSION_FLOOR = "1.44.0"
+# Also pinned <1.48.0 until the resolution of https://github.com/grpc/grpc/issues/31885
+# (except on python 3.11, where newer versions are required just to install the grpcio package)
+GRPC_VERSION_CAP = "1.48.0"
+
+
 setup(
     name="dagster",
     version=get_version(),
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="The data orchestration platform built for productivity.",
@@ -70,20 +77,18 @@
         "contextvars; python_version < '3.7'",
         "Jinja2",
         "PyYAML>=5.1",
         # core (not explicitly expressed atm)
         # pin around issues in specific versions of alembic that broke our migrations
         "alembic>=1.2.1,!=1.6.3,!=1.7.0,<1.11.0",
         "croniter>=0.3.34",
-        # grpcio 1.44.0 is the min version compatible with both protobuf 3 and 4
-        # Also pinned <1.48.0 until the resolution of https://github.com/grpc/grpc/issues/31885
-        # (except on python 3.11, where newer versions are required just to install the grpcio package)
-        "grpcio>=1.44.0,<1.48.0; python_version<'3.11'",
-        "grpcio>=1.44.0; python_version>='3.11'",
-        "grpcio-health-checking>=1.44.0",
+        f"grpcio>={GRPC_VERSION_FLOOR},<{GRPC_VERSION_CAP}; python_version<'3.11'",
+        f"grpcio>={GRPC_VERSION_FLOOR}; python_version>='3.11'",
+        f"grpcio-health-checking>={GRPC_VERSION_FLOOR},<{GRPC_VERSION_CAP}; python_version<'3.11'",
+        f"grpcio-health-checking>={GRPC_VERSION_FLOOR}; python_version>='3.11'",
         "packaging>=20.9",
         "pendulum",
         "protobuf>=3.20.0",  # min protobuf version to be compatible with both protobuf 3 and 4
         "python-dateutil",
         "python-dotenv",
         "pytz",
         "requests",
@@ -104,15 +109,16 @@
         "pydantic != 1.10.7",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector ; python_version>='3.8'",
             "docker",
-            "grpcio-tools>=1.44.0",  # related to above grpcio pins
+            f"grpcio-tools>={GRPC_VERSION_FLOOR},<{GRPC_VERSION_CAP}; python_version<'3.11'",
+            f"grpcio-tools>={GRPC_VERSION_FLOOR}; python_version>='3.11'",
             "mock==3.0.5",
             "objgraph",
             "pytest-cov==2.10.1",
             "pytest-dependency==0.5.1",
             "pytest-mock==3.3.1",
             "pytest-rerunfailures==10.0",
             "pytest-runner==5.2",
```

