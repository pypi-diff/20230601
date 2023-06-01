# Comparing `tmp/flytekit-1.6.2.tar.gz` & `tmp/flytekit-1.6.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.2.tar", last modified: Tue May 30 15:24:06 2023, max compression
+gzip compressed data, was "flytekit-1.6.2b0.tar", last modified: Thu Jun  1 20:41:44 2023, max compression
```

## Comparing `flytekit-1.6.2.tar` & `flytekit-1.6.2b0.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-30 15:23:56.000000 flytekit-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-30 15:23:56.000000 flytekit-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-30 15:24:06.901439 flytekit-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-30 15:23:56.000000 flytekit-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.881439 flytekit-1.6.2/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-05-30 15:24:05.000000 flytekit-1.6.2/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.889439 flytekit-1.6.2/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.889439 flytekit-1.6.2/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36184 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36181 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    77072 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extend/backend/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extend/backend/external_plugin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-30 15:23:56.000000 flytekit-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-30 15:24:06.905439 flytekit-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-30 15:24:05.000000 flytekit-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-01 20:41:42.000000 flytekit-1.6.2b0/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36184 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77072 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extend/backend/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extend/backend/external_plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.347651 flytekit-1.6.2b0/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.347651 flytekit-1.6.2b0/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.347651 flytekit-1.6.2b0/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-01 20:41:42.000000 flytekit-1.6.2b0/setup.py
```

### Comparing `flytekit-1.6.2/LICENSE` & `flytekit-1.6.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/MANIFEST.in` & `flytekit-1.6.2b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/PKG-INFO` & `flytekit-1.6.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.2
+Version: 1.6.2b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.2 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.2b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.2/README.md` & `flytekit-1.6.2b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/__init__.py` & `flytekit-1.6.2b0/flytekit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.2"
+__version__ = "1.6.2b0"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.2/flytekit/bin/entrypoint.py` & `flytekit-1.6.2b0/flytekit/bin/entrypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,22 +179,24 @@
             return os.environ[k]
     return ""
 
 
 @contextlib.contextmanager
 def setup_execution(
     raw_output_data_prefix: str,
+    output_metadata_prefix: Optional[str] = None,
     checkpoint_path: Optional[str] = None,
     prev_checkpoint: Optional[str] = None,
     dynamic_addl_distro: Optional[str] = None,
     dynamic_dest_dir: Optional[str] = None,
 ):
     """
 
-    :param raw_output_data_prefix:
+    :param raw_output_data_prefix: Where to write offloaded data (files, directories, dataframes).
+    :param output_metadata_prefix: Where to write primitive outputs.
     :param checkpoint_path:
     :param prev_checkpoint:
     :param dynamic_addl_distro: Works in concert with the other dynamic arg. If present, indicates that if a dynamic
       task were to run, it should set fast serialize to true and use these values in FastSerializationSettings
     :param dynamic_dest_dir: See above.
     :return:
     """
@@ -243,14 +245,15 @@
                 "exec_launchplan": exe_lp,
                 "api_version": _api_version,
             },
         ),
         logging=user_space_logger,
         tmp_dir=user_workspace_dir,
         raw_output_prefix=raw_output_data_prefix,
+        output_metadata_prefix=output_metadata_prefix,
         checkpoint=checkpointer,
         task_id=_identifier.Identifier(_identifier.ResourceType.TASK, tk_project, tk_domain, tk_name, tk_version),
     )
 
     try:
         file_access = FileAccessProvider(
             local_sandbox_dir=tempfile.mkdtemp(prefix="flyte"),
@@ -333,14 +336,15 @@
     :return:
     """
     if len(resolver_args) < 1:
         raise Exception("cannot be <1")
 
     with setup_execution(
         raw_output_data_prefix,
+        output_prefix,
         checkpoint_path,
         prev_checkpoint,
         dynamic_addl_distro,
         dynamic_dest_dir,
     ) as ctx:
         resolver_obj = load_object_from_module(resolver)
         # Use the resolver to load the actual task object
```

### Comparing `flytekit-1.6.2/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.2b0/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.2b0/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clients/auth/keyring.py` & `flytekit-1.6.2b0/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clients/auth/token_client.py` & `flytekit-1.6.2b0/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clients/auth_helper.py` & `flytekit-1.6.2b0/flytekit/clients/auth_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,17 @@
         return grpc.insecure_channel(cfg.endpoint, **kwargs)
 
     credentials = None
     if "credentials" not in kwargs:
         if cfg.insecure_skip_verify:
             credentials = bootstrap_creds_from_server(cfg.endpoint)
         elif cfg.ca_cert_file_path:
-            credentials = grpc.ssl_channel_credentials(load_cert(cfg.ca_cert_file_path))
+            credentials = grpc.ssl_channel_credentials(
+                crypto.dump_certificate(crypto.FILETYPE_PEM, load_cert(cfg.ca_cert_file_path))
+            )
         else:
             credentials = grpc.ssl_channel_credentials(
                 root_certificates=kwargs.get("root_certificates", None),
                 private_key=kwargs.get("private_key", None),
                 certificate_chain=kwargs.get("certificate_chain", None),
             )
     else:
```

### Comparing `flytekit-1.6.2/flytekit/clients/friendly.py` & `flytekit-1.6.2b0/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.2b0/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.2b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clients/helpers.py` & `flytekit-1.6.2b0/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clients/raw.py` & `flytekit-1.6.2b0/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.2b0/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/helpers.py` & `flytekit-1.6.2b0/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import typing
 
 import grpc
 import rich_click as click
 from google.protobuf.json_format import MessageToJson
 
 from flytekit import configuration
@@ -13,14 +14,15 @@
 from flytekit.clis.sdk_in_container.local_cache import local_cache
 from flytekit.clis.sdk_in_container.metrics import metrics
 from flytekit.clis.sdk_in_container.package import package
 from flytekit.clis.sdk_in_container.register import register
 from flytekit.clis.sdk_in_container.run import run
 from flytekit.clis.sdk_in_container.serialize import serialize
 from flytekit.clis.sdk_in_container.serve import serve
+from flytekit.configuration.file import FLYTECTL_CONFIG_ENV_VAR, FLYTECTL_CONFIG_ENV_VAR_OVERRIDE
 from flytekit.configuration.internal import LocalSDK
 from flytekit.exceptions.base import FlyteException
 from flytekit.exceptions.user import FlyteInvalidInputException
 from flytekit.loggers import cli_logger
 
 
 def validate_package(ctx, param, values):
@@ -116,14 +118,20 @@
     ctx.obj = dict()
 
     # Handle package management - get from the command line, the environment variables, then the config file.
     pkgs = pkgs or LocalSDK.WORKFLOW_PACKAGES.read() or []
     if config:
         ctx.obj[CTX_CONFIG_FILE] = config
         cfg = configuration.ConfigFile(config)
+        # Set here so that if someone has Config.auto() in their user code, the config here will get used.
+        if FLYTECTL_CONFIG_ENV_VAR in os.environ:
+            cli_logger.info(
+                f"Config file arg {config} will override env var {FLYTECTL_CONFIG_ENV_VAR}: {os.environ[FLYTECTL_CONFIG_ENV_VAR]}"
+            )
+        os.environ[FLYTECTL_CONFIG_ENV_VAR_OVERRIDE] = config
         if not pkgs:
             pkgs = LocalSDK.WORKFLOW_PACKAGES.read(cfg)
             if pkgs is None:
                 pkgs = []
     ctx.obj[CTX_PACKAGES] = pkgs
     ctx.obj[CTX_VERBOSE] = verbose
```

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/run.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/serve.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/configuration/__init__.py` & `flytekit-1.6.2b0/flytekit/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/configuration/default_images.py` & `flytekit-1.6.2b0/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/configuration/feature_flags.py` & `flytekit-1.6.2b0/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/configuration/file.py` & `flytekit-1.6.2b0/flytekit/configuration/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 import yaml
 
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.loggers import logger
 
 # This is the env var that the flytectl sandbox instructions say to set
 FLYTECTL_CONFIG_ENV_VAR = "FLYTECTL_CONFIG"
+# This is an explicit override only to be used by pyflyte and takes precedence in get_config_file over the main
+# environment variable.
+# This env var should not be set by users
+FLYTECTL_CONFIG_ENV_VAR_OVERRIDE = "_FLYTECTL_CONFIG_PYFLYTE_OVERRIDE"
 
 
 def _exists(val: typing.Any) -> bool:
     """Check if a value is defined."""
     return isinstance(val, bool) or bool(val is not None and val)
 
 
@@ -235,33 +239,39 @@
 
 
 def get_config_file(c: typing.Union[str, ConfigFile, None]) -> typing.Optional[ConfigFile]:
     """
     Checks if the given argument is a file or a configFile and returns a loaded configFile else returns None
     """
     if c is None:
+        # Pyflyte override env var takes highest precedence
+        # Env var takes second highest precedence
+        flytectl_path_from_env = getenv(FLYTECTL_CONFIG_ENV_VAR_OVERRIDE, getenv(FLYTECTL_CONFIG_ENV_VAR, None))
+        if flytectl_path_from_env:
+            flytectl_path = Path(flytectl_path_from_env)
+            if flytectl_path.exists():
+                logger.info(f"Using flytectl/YAML config {flytectl_path.absolute()}")
+                return ConfigFile(str(flytectl_path.absolute()))
+            else:
+                logger.warning(f"flytectl config file {flytectl_path.absolute()} does not exist, ignoring...")
+
         # See if there's a config file in the current directory where Python is being run from
         current_location_config = Path("flytekit.config")
         if current_location_config.exists():
             logger.info(f"Using configuration from Python process root {current_location_config.absolute()}")
             return ConfigFile(str(current_location_config.absolute()))
 
         # If not, see if there's a config in the user's home directory
         home_dir_config = Path(Path.home(), ".flyte", "config")  # _default_config_file_name in main.py
         if home_dir_config.exists():
             logger.info(f"Using configuration from home directory {home_dir_config.absolute()}")
             return ConfigFile(str(home_dir_config.absolute()))
 
-        # If not, see if the env var that flytectl sandbox tells the user to set is set,
-        # or see if there's something in the default home directory location
+        # If not see if there's something in the default home directory location
         flytectl_path = Path(Path.home(), ".flyte", "config.yaml")
-        flytectl_path_from_env = getenv(FLYTECTL_CONFIG_ENV_VAR, None)
-
-        if flytectl_path_from_env:
-            flytectl_path = Path(flytectl_path_from_env)
         if flytectl_path.exists():
             logger.info(f"Using flytectl/YAML config {flytectl_path.absolute()}")
             return ConfigFile(str(flytectl_path.absolute()))
 
         # If not, then return None and let caller handle
         return None
     if isinstance(c, str):
```

### Comparing `flytekit-1.6.2/flytekit/configuration/internal.py` & `flytekit-1.6.2b0/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/annotation.py` & `flytekit-1.6.2b0/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/base_sql_task.py` & `flytekit-1.6.2b0/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/base_task.py` & `flytekit-1.6.2b0/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/checkpointer.py` & `flytekit-1.6.2b0/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/class_based_resolver.py` & `flytekit-1.6.2b0/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/condition.py` & `flytekit-1.6.2b0/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/constants.py` & `flytekit-1.6.2b0/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/container_task.py` & `flytekit-1.6.2b0/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/context_manager.py` & `flytekit-1.6.2b0/flytekit/core/context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         self,
         execution_date,
         tmp_dir,
         stats,
         execution_id: typing.Optional[_identifier.WorkflowExecutionIdentifier],
         logging,
         raw_output_prefix,
+        output_metadata_prefix=None,
         checkpoint=None,
         decks=None,
         task_id: typing.Optional[_identifier.Identifier] = None,
         **kwargs,
     ):
         """
         Args:
@@ -169,14 +170,15 @@
             decks = []
         self._stats = stats
         self._execution_date = execution_date
         self._working_directory = tmp_dir
         self._execution_id = execution_id
         self._logging = logging
         self._raw_output_prefix = raw_output_prefix
+        self._output_metadata_prefix = output_metadata_prefix
         # AutoDeletingTempDir's should be used with a with block, which creates upon entry
         self._attrs = kwargs
         # It is safe to recreate the Secrets Manager
         self._secrets_manager = SecretsManager()
         self._checkpoint = checkpoint
         self._decks = decks
         self._task_id = task_id
@@ -198,14 +200,18 @@
         return self._logging
 
     @property
     def raw_output_prefix(self) -> str:
         return self._raw_output_prefix
 
     @property
+    def output_metadata_prefix(self) -> str:
+        return self._output_metadata_prefix
+
+    @property
     def working_directory(self) -> str:
         """
         A handle to a special working directory for easily producing temporary files.
         TODO: Usage examples
         """
         return self._working_directory
```

### Comparing `flytekit-1.6.2/flytekit/core/data_persistence.py` & `flytekit-1.6.2b0/flytekit/core/data_persistence.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,29 +199,29 @@
             logger.debug(f"Error in getting {from_path} to {to_path} rec {recursive} {oe}")
             file_system = self.get_filesystem(get_protocol(from_path), anonymous=True)
             if file_system is not None:
                 logger.debug(f"Attempting anonymous get with {file_system}")
                 return file_system.get(from_path, to_path, recursive=recursive)
             raise oe
 
-    def put(self, from_path: str, to_path: str, recursive: bool = False):
+    def put(self, from_path: str, to_path: str, recursive: bool = False, **kwargs):
         file_system = self.get_filesystem_for_path(to_path)
         from_path = self.strip_file_header(from_path)
         if recursive:
             # Only check this for the local filesystem
             if file_system.protocol == "file" and not file_system.isdir(from_path):
                 raise FlyteAssertion(f"Source path {from_path} is not a directory")
             if os.name == "nt" and file_system.protocol == "file":
                 import shutil
 
                 return shutil.copytree(
                     self.strip_file_header(from_path), self.strip_file_header(to_path), dirs_exist_ok=True
                 )
             from_path, to_path = self.recursive_paths(from_path, to_path)
-        return file_system.put(from_path, to_path, recursive=recursive)
+        return file_system.put(from_path, to_path, recursive=recursive, **kwargs)
 
     def get_random_remote_path(self, file_path_or_file_name: typing.Optional[str] = None) -> str:
         """
         Constructs a randomized path on the configured raw_output_prefix (persistence layer). the random bit is a UUID
         and allows for disambiguating paths within the same directory.
 
         Use file_path_or_file_name, when you want a random directory, but want to preserve the leaf file name
@@ -300,27 +300,27 @@
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to get data from {remote_path} to {local_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             )
 
     @timeit("Upload data to remote")
-    def put_data(self, local_path: Union[str, os.PathLike], remote_path: str, is_multipart: bool = False):
+    def put_data(self, local_path: Union[str, os.PathLike], remote_path: str, is_multipart: bool = False, **kwargs):
         """
         The implication here is that we're always going to put data to the remote location, so we .remote to ensure
         we don't use the true local proxy if the remote path is a file://
 
         :param local_path:
         :param remote_path:
         :param is_multipart:
         """
         try:
             local_path = str(local_path)
 
-            self.put(cast(str, local_path), remote_path, recursive=is_multipart)
+            self.put(cast(str, local_path), remote_path, recursive=is_multipart, **kwargs)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to put data from {local_path} to {remote_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             ) from ex
```

### Comparing `flytekit-1.6.2/flytekit/core/docstring.py` & `flytekit-1.6.2b0/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.2b0/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/gate.py` & `flytekit-1.6.2b0/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/interface.py` & `flytekit-1.6.2b0/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/launch_plan.py` & `flytekit-1.6.2b0/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/local_cache.py` & `flytekit-1.6.2b0/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/map_task.py` & `flytekit-1.6.2b0/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/mock_stats.py` & `flytekit-1.6.2b0/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/node.py` & `flytekit-1.6.2b0/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/node_creation.py` & `flytekit-1.6.2b0/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/notification.py` & `flytekit-1.6.2b0/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/pod_template.py` & `flytekit-1.6.2b0/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/promise.py` & `flytekit-1.6.2b0/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/python_auto_container.py` & `flytekit-1.6.2b0/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.2b0/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/python_function_task.py` & `flytekit-1.6.2b0/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/reference.py` & `flytekit-1.6.2b0/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/reference_entity.py` & `flytekit-1.6.2b0/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/resources.py` & `flytekit-1.6.2b0/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/schedule.py` & `flytekit-1.6.2b0/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/shim_task.py` & `flytekit-1.6.2b0/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/task.py` & `flytekit-1.6.2b0/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/testing.py` & `flytekit-1.6.2b0/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/tracker.py` & `flytekit-1.6.2b0/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/type_engine.py` & `flytekit-1.6.2b0/flytekit/core/type_engine.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/type_helpers.py` & `flytekit-1.6.2b0/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/utils.py` & `flytekit-1.6.2b0/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/core/workflow.py` & `flytekit-1.6.2b0/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/deck/deck.py` & `flytekit-1.6.2b0/flytekit/deck/deck.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     MarkdownRenderer can convert Markdown string to HTML
 
     Flyte context saves a list of deck objects, and we use renderers in those decks to render
     the data and create an HTML file when those tasks are executed
 
     Each task has a least three decks (input, output, default). Input/output decks are
     used to render tasks' input/output data, and the default deck is used to render line plots,
-    scatter plots or markdown text. In addition, users can create new decks to render
+    scatter plots or Markdown text. In addition, users can create new decks to render
     their data with custom renderers.
 
     .. warning::
 
         This feature is in beta.
 
     .. code-block:: python
@@ -141,22 +141,26 @@
             ...
         return HTML(raw_html)
     return raw_html
 
 
 def _output_deck(task_name: str, new_user_params: ExecutionParameters):
     ctx = FlyteContext.current_context()
-    if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
-        output_dir = ctx.execution_state.engine_dir
-    else:
-        output_dir = ctx.file_access.get_random_local_directory()
-    deck_path = os.path.join(output_dir, DECK_FILE_NAME)
-    with open(deck_path, "w") as f:
+    local_dir = ctx.file_access.get_random_local_directory()
+    local_path = f"{local_dir}{os.sep}{DECK_FILE_NAME}"
+    with open(local_path, "w") as f:
         f.write(_get_deck(new_user_params, ignore_jupyter=True))
-    logger.info(f"{task_name} task creates flyte deck html to file://{deck_path}")
+    logger.info(f"{task_name} task creates flyte deck html to file://{local_path}")
+    if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
+        remote_path = f"{new_user_params.output_metadata_prefix}{os.sep}{DECK_FILE_NAME}"
+        kwargs: typing.Dict[str, str] = {
+            "ContentType": "text/html",  # For s3
+            "content_type": "text/html",  # For gcs
+        }
+        ctx.file_access.put_data(local_path, remote_path, **kwargs)
 
 
 def get_deck_template() -> "Template":
     from jinja2 import Environment, FileSystemLoader, select_autoescape
 
     root = os.path.dirname(os.path.abspath(__file__))
     templates_dir = os.path.join(root, "html")
```

### Comparing `flytekit-1.6.2/flytekit/deck/html/template.html` & `flytekit-1.6.2b0/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/deck/renderer.py` & `flytekit-1.6.2b0/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/exceptions/scopes.py` & `flytekit-1.6.2b0/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/exceptions/system.py` & `flytekit-1.6.2b0/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/exceptions/user.py` & `flytekit-1.6.2b0/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extend/__init__.py` & `flytekit-1.6.2b0/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extend/backend/base_plugin.py` & `flytekit-1.6.2b0/flytekit/extend/backend/base_plugin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extend/backend/external_plugin_service.py` & `flytekit-1.6.2b0/flytekit/extend/backend/external_plugin_service.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.2b0/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.2b0/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.2b0/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/pytorch/native.py` & `flytekit-1.6.2b0/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.2b0/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/sklearn/native.py` & `flytekit-1.6.2b0/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.2b0/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/tasks/shell.py` & `flytekit-1.6.2b0/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.2b0/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.2b0/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.2b0/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/image_spec/image_spec.py` & `flytekit-1.6.2b0/flytekit/image_spec/image_spec.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.2b0/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.2b0/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/interfaces/random.py` & `flytekit-1.6.2b0/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/interfaces/stats/client.py` & `flytekit-1.6.2b0/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.2b0/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/lazy_import/lazy_module.py` & `flytekit-1.6.2b0/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/loggers.py` & `flytekit-1.6.2b0/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/admin/common.py` & `flytekit-1.6.2b0/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/admin/task_execution.py` & `flytekit-1.6.2b0/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/admin/workflow.py` & `flytekit-1.6.2b0/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/annotation.py` & `flytekit-1.6.2b0/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/array_job.py` & `flytekit-1.6.2b0/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/common.py` & `flytekit-1.6.2b0/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/core/catalog.py` & `flytekit-1.6.2b0/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/core/compiler.py` & `flytekit-1.6.2b0/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/core/condition.py` & `flytekit-1.6.2b0/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/core/errors.py` & `flytekit-1.6.2b0/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/core/execution.py` & `flytekit-1.6.2b0/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/core/identifier.py` & `flytekit-1.6.2b0/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/core/types.py` & `flytekit-1.6.2b0/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/core/workflow.py` & `flytekit-1.6.2b0/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/documentation.py` & `flytekit-1.6.2b0/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/dynamic_job.py` & `flytekit-1.6.2b0/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/execution.py` & `flytekit-1.6.2b0/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/filters.py` & `flytekit-1.6.2b0/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/interface.py` & `flytekit-1.6.2b0/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/launch_plan.py` & `flytekit-1.6.2b0/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/literals.py` & `flytekit-1.6.2b0/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/matchable_resource.py` & `flytekit-1.6.2b0/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/named_entity.py` & `flytekit-1.6.2b0/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/node_execution.py` & `flytekit-1.6.2b0/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/presto.py` & `flytekit-1.6.2b0/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/project.py` & `flytekit-1.6.2b0/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/qubole.py` & `flytekit-1.6.2b0/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/schedule.py` & `flytekit-1.6.2b0/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/security.py` & `flytekit-1.6.2b0/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/task.py` & `flytekit-1.6.2b0/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/types.py` & `flytekit-1.6.2b0/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/models/workflow_closure.py` & `flytekit-1.6.2b0/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/remote/__init__.py` & `flytekit-1.6.2b0/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/remote/backfill.py` & `flytekit-1.6.2b0/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/remote/entities.py` & `flytekit-1.6.2b0/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/remote/executions.py` & `flytekit-1.6.2b0/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/remote/lazy_entity.py` & `flytekit-1.6.2b0/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/remote/remote.py` & `flytekit-1.6.2b0/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/remote/remote_callable.py` & `flytekit-1.6.2b0/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/testing/__init__.py` & `flytekit-1.6.2b0/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/tools/fast_registration.py` & `flytekit-1.6.2b0/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/tools/ignore.py` & `flytekit-1.6.2b0/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/tools/module_loader.py` & `flytekit-1.6.2b0/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/tools/repo.py` & `flytekit-1.6.2b0/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/tools/script_mode.py` & `flytekit-1.6.2b0/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/tools/serialize_helpers.py` & `flytekit-1.6.2b0/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/tools/subprocess.py` & `flytekit-1.6.2b0/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/tools/translator.py` & `flytekit-1.6.2b0/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/directory/__init__.py` & `flytekit-1.6.2b0/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/directory/types.py` & `flytekit-1.6.2b0/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/file/__init__.py` & `flytekit-1.6.2b0/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/file/file.py` & `flytekit-1.6.2b0/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.2b0/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/pickle/pickle.py` & `flytekit-1.6.2b0/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/schema/types.py` & `flytekit-1.6.2b0/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.2b0/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/structured/__init__.py` & `flytekit-1.6.2b0/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.2b0/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/structured/bigquery.py` & `flytekit-1.6.2b0/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.2b0/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.2b0/flytekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.2
+Version: 1.6.2b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.2 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.2b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.2/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.2b0/flytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit.egg-info/requires.txt` & `flytekit-1.6.2b0/flytekit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.2b0/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2/setup.py` & `flytekit-1.6.2b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.2"
+__version__ = "1.6.2b0"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
```

