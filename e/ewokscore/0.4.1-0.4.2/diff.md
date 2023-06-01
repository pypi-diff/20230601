# Comparing `tmp/ewokscore-0.4.1.tar.gz` & `tmp/ewokscore-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewokscore-0.4.1.tar", last modified: Mon May 15 08:25:37 2023, max compression
+gzip compressed data, was "dist/ewokscore-0.4.2.tar", last modified: Thu Jun  1 16:14:14 2023, max compression
```

## Comparing `ewokscore-0.4.1.tar` & `ewokscore-0.4.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-15 07:53:03.000000 ewokscore-0.4.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2622 2023-05-15 08:25:37.000000 ewokscore-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-05-15 07:53:03.000000 ewokscore-0.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-15 07:53:03.000000 ewokscore-0.4.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1251 2023-05-15 08:25:37.000000 ewokscore-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-15 07:53:03.000000 ewokscore-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-15 08:23:36.000000 ewokscore-0.4.1/src/ewokscore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/bindings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/cliutils/
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/cliconvertutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/cliexecuteutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/clilogutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/dynamictask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/events/
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/contexts.py
--rw-rw-rw-   0 root         (0) root         (0)     4996 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/global_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/handlers/base.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/handlers/sqlite3.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/initialize_events.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/send_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/graph/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12469 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/error_handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/graph/execute/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/graph/execute/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4888 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/execute/sequential.py
--rw-rw-rw-   0 root         (0) root         (0)     7034 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/multigraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/
--rw-rw-rw-   0 root         (0) root         (0)     4434 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/v0_0.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/v0_1.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/v0_2.py
--rw-rw-rw-   0 root         (0) root         (0)     6805 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)    10936 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/subgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     5551 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/taskgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     8690 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     8562 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/inittask.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/methodtask.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/missing_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     5623 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/file.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     6064 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/uri.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/ppftasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3415 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2287 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/registration.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/scripttask.py
--rw-rw-rw-   0 root         (0) root         (0)    14259 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/task.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/taskwithprogress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/discover_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic2.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic3.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/cyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     4139 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/demo.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/empty.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/triangle1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/loadtest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/loadtest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/loadtest/graph.json
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/loadtest/subgraph.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/addfunc.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/condsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/errorsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/nooutputtask.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/simplemethods.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/sumlist.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/sumtask.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7990 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_default_error_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_dynamic_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     7341 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_execute_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     6597 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2700 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph_start_end_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     7463 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_link_is_required.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_method_task.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_persistence.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_script_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8223 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_sub_graph.py
--rw-rw-rw-   0 root         (0) root         (0)    10730 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_sub_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     4985 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_task_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_uri.py
--rw-rw-rw-   0 root         (0) root         (0)    14406 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_variable.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_variable_namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7495 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_workflow_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4916 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/utils/show.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    21246 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2622 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4175 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      264 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-01 08:57:52.000000 ewokscore-0.4.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-06-01 16:14:14.000000 ewokscore-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-01 08:57:52.000000 ewokscore-0.4.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-01 08:57:52.000000 ewokscore-0.4.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2023-06-01 16:14:14.000000 ewokscore-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-01 08:57:52.000000 ewokscore-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-01 16:11:21.000000 ewokscore-0.4.2/src/ewokscore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/bindings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/cliutils/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/cliutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/cliutils/cliconvertutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/cliutils/cliexecuteutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/cliutils/clilogutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/cliutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/dynamictask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/events/
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/events/contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/events/global_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/events/handlers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/events/handlers/sqlite3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/events/initialize_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/events/send_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/graph/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12469 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/error_handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/graph/execute/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:14:08.000000 ewokscore-0.4.2/src/ewokscore/graph/execute/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/execute/sequential.py
+-rw-rw-rw-   0 root         (0) root         (0)     7034 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/multigraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/graph/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/schema/v0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/schema/v0_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/schema/v0_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-01 13:17:43.000000 ewokscore-0.4.2/src/ewokscore/graph/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)    10936 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/subgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5556 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/taskgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/graph/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8690 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8562 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/inittask.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/methodtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/missing_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/persistence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/persistence/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     5623 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/persistence/file.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/persistence/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/persistence/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/persistence/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/persistence/uri.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/ppftasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3415 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-01 13:26:50.000000 ewokscore-0.4.2/src/ewokscore/registration.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/scripttask.py
+-rw-rw-rw-   0 root         (0) root         (0)    14409 2023-06-01 12:09:51.000000 ewokscore-0.4.2/src/ewokscore/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2023-06-01 16:11:21.000000 ewokscore-0.4.2/src/ewokscore/task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/taskwithprogress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:14:08.000000 ewokscore-0.4.2/src/ewokscore/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/discover_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:14:08.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/acyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/acyclic2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/acyclic3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/cyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4139 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/triangle1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/loadtest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:14:08.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/loadtest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/loadtest/graph.json
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/loadtest/subgraph.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:14:08.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/addfunc.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/condsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/errorsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/nooutputtask.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/simplemethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/sumlist.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/sumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7990 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_default_error_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_dynamic_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     7341 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_execute_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     6597 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_graph_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_graph_start_end_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_link_is_required.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_method_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_persistence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_script_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8223 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_sub_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    10730 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_sub_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_task_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_uri.py
+-rw-rw-rw-   0 root         (0) root         (0)    14406 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_variable_namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7495 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/test_workflow_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 16:14:08.000000 ewokscore-0.4.2/src/ewokscore/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/tests/utils/show.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-06-01 08:57:52.000000 ewokscore-0.4.2/src/ewokscore/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21421 2023-06-01 12:09:51.000000 ewokscore-0.4.2/src/ewokscore/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4175 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-01 16:14:14.000000 ewokscore-0.4.2/src/ewokscore.egg-info/top_level.txt
```

### Comparing `ewokscore-0.4.1/LICENSE.md` & `ewokscore-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/PKG-INFO` & `ewokscore-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.4.1
+Version: 0.4.2
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
```

### Comparing `ewokscore-0.4.1/README.md` & `ewokscore-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/setup.cfg` & `ewokscore-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 install_requires = 
 	numpy >=1.15
 	networkx >=2
 	silx >=1
 	pyyaml >=5.1
 	h5py >=2.8
 	packaging
-	ewoksutils >=0.1
+	ewoksutils >=0.1.2
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.json
```

### Comparing `ewokscore-0.4.1/src/ewokscore/bindings.py` & `ewokscore-0.4.2/src/ewokscore/bindings.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/cliutils/__init__.py` & `ewokscore-0.4.2/src/ewokscore/cliutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/cliutils/cliconvertutils.py` & `ewokscore-0.4.2/src/ewokscore/cliutils/cliconvertutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/cliutils/cliexecuteutils.py` & `ewokscore-0.4.2/src/ewokscore/cliutils/cliexecuteutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/cliutils/clilogutils.py` & `ewokscore-0.4.2/src/ewokscore/cliutils/clilogutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/cliutils/utils.py` & `ewokscore-0.4.2/src/ewokscore/cliutils/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/dynamictask.py` & `ewokscore-0.4.2/src/ewokscore/dynamictask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/events/__init__.py` & `ewokscore-0.4.2/src/ewokscore/events/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/events/contexts.py` & `ewokscore-0.4.2/src/ewokscore/events/contexts.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/events/global_state.py` & `ewokscore-0.4.2/src/ewokscore/events/global_state.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/events/initialize_events.py` & `ewokscore-0.4.2/src/ewokscore/events/initialize_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             f"{execinfo['host_name']}-{execinfo['process_id']}-{execinfo['user_name']}"
         )
         execinfo["workflow_id"] = default
     elif isinstance(workflow, str):
         execinfo["workflow_id"] = workflow
     else:
         try:
-            execinfo["workflow_id"] = workflow.graph["id"]
+            execinfo["workflow_id"] = str(workflow.graph["id"])
         except KeyError:
             raise ValueError("the graph needs an 'id' for execution events")
     execinfo.update(static_workflow_info)
     return execinfo
 
 
 def init_node(
```

### Comparing `ewokscore-0.4.1/src/ewokscore/events/send_events.py` & `ewokscore-0.4.2/src/ewokscore/events/send_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/analysis.py` & `ewokscore-0.4.2/src/ewokscore/graph/analysis.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/compare.py` & `ewokscore-0.4.2/src/ewokscore/graph/compare.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/error_handlers.py` & `ewokscore-0.4.2/src/ewokscore/graph/error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/execute/sequential.py` & `ewokscore-0.4.2/src/ewokscore/graph/execute/sequential.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/graph_io.py` & `ewokscore-0.4.2/src/ewokscore/graph/graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/multigraph.py` & `ewokscore-0.4.2/src/ewokscore/graph/multigraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/schema/__init__.py` & `ewokscore-0.4.2/src/ewokscore/graph/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/serialize.py` & `ewokscore-0.4.2/src/ewokscore/graph/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
 def _dict_to_networkx(graph: dict) -> networkx.DiGraph:
     graph.setdefault("directed", True)
     graph.setdefault("nodes", list())
     graph.setdefault("links", list())
     graph.setdefault("graph", dict())
 
-    if not graph["graph"].get("id"):
+    if "id" not in graph["graph"]:
         logger.warning('Graph has no "id": use "notspecified"')
         graph["graph"]["id"] = "notspecified"
     normalize_schema_version(graph)
 
     return networkx.readwrite.json_graph.node_link_graph(graph)
```

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/subgraph.py` & `ewokscore-0.4.2/src/ewokscore/graph/subgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/taskgraph.py` & `ewokscore-0.4.2/src/ewokscore/graph/taskgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     @property
     def graph_id(self) -> Hashable:
         return self.graph.graph.get("id", qualname(type(self)))
 
     @property
     def graph_label(self) -> str:
-        return self.graph.graph.get("label", self.graph_id)
+        return str(self.graph.graph.get("label", self.graph_id))
 
     def __eq__(self, other):
         if not isinstance(other, type(self)):
             raise TypeError(other, type(other))
         return graphs_are_equal(self.graph, other.graph)
 
     def load(
```

### Comparing `ewokscore-0.4.1/src/ewokscore/graph/validate.py` & `ewokscore-0.4.2/src/ewokscore/graph/validate.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/hashing.py` & `ewokscore-0.4.2/src/ewokscore/hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/inittask.py` & `ewokscore-0.4.2/src/ewokscore/inittask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/methodtask.py` & `ewokscore-0.4.2/src/ewokscore/methodtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/missing_data.py` & `ewokscore-0.4.2/src/ewokscore/missing_data.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/node.py` & `ewokscore-0.4.2/src/ewokscore/node.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/persistence/atomic.py` & `ewokscore-0.4.2/src/ewokscore/persistence/atomic.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/persistence/file.py` & `ewokscore-0.4.2/src/ewokscore/persistence/file.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/persistence/json.py` & `ewokscore-0.4.2/src/ewokscore/persistence/json.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/persistence/nexus.py` & `ewokscore-0.4.2/src/ewokscore/persistence/nexus.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/persistence/proxy.py` & `ewokscore-0.4.2/src/ewokscore/persistence/proxy.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/persistence/uri.py` & `ewokscore-0.4.2/src/ewokscore/persistence/uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/ppftasks.py` & `ewokscore-0.4.2/src/ewokscore/ppftasks.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/progress.py` & `ewokscore-0.4.2/src/ewokscore/progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/registration.py` & `ewokscore-0.4.2/src/ewokscore/registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,19 @@
         return list(cls._SUBCLASS_REGISTRY.values())
 
     @classmethod
     def get_subclass(cls, registry_name, _second_attempt=False):
         """Retrieving a derived class"""
         subclass = cls._SUBCLASS_REGISTRY.get(registry_name)
         if subclass is None:
-            candidates = []
-            for name, value in cls._SUBCLASS_REGISTRY.items():
-                if name.endswith("." + registry_name):
-                    candidates.append(name)
+            candidates = [
+                name
+                for name in cls._SUBCLASS_REGISTRY
+                if name.endswith("." + registry_name)
+            ]
             if len(candidates) == 1:
                 subclass = cls._SUBCLASS_REGISTRY.get(candidates[0])
         if subclass is None:
             if _second_attempt:
                 lst = cls.get_subclass_names()
                 raise RuntimeError(
                     f"Class {repr(registry_name)} is not imported. Imported classes are {repr(lst)}"
```

### Comparing `ewokscore-0.4.1/src/ewokscore/scripttask.py` & `ewokscore-0.4.2/src/ewokscore/scripttask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/task.py` & `ewokscore-0.4.2/src/ewokscore/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,36 +202,39 @@
         return self.get_input_uhashes()
 
     def get_input_uhashes(self):
         return self.__inputs.get_variable_uhashes()
 
     @property
     def input_values(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'input_values' is deprecated in favor of the function 'get_input_values'",
             DeprecationWarning,
         )
         return self.get_input_values()
 
     def get_input_values(self):
         return self.__inputs.get_variable_values()
 
     @property
     def named_input_values(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'named_input_values' is deprecated in favor of the function 'get_named_input_values'",
             DeprecationWarning,
         )
         return self.get_named_input_values()
 
     def get_named_input_values(self):
         return self.__inputs.get_named_variable_values()
 
     @property
     def positional_input_values(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'positional_input_values' is deprecated in favor of the function 'get_positional_input_values'",
             DeprecationWarning,
         )
         return self.__inputs.get_positional_input_values()
 
     def get_positional_input_values(self):
@@ -256,36 +259,39 @@
     def get_output_value(self, key, default=missing_data.MISSING_DATA):
         if self.missing_outputs[key]:
             return default
         return self.outputs[key]
 
     @property
     def output_uhashes(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'output_uhashes' is deprecated in favor of the function 'get_output_uhashes'",
             DeprecationWarning,
         )
         return self.get_output_uhashes()
 
     def get_output_uhashes(self):
         return self.__outputs.get_variable_uhashes()
 
     @property
     def output_values(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'output_values' is deprecated in favor of the function 'get_output_values'",
             DeprecationWarning,
         )
         return self.get_output_values()
 
     def get_output_values(self):
         return self.__outputs.get_variable_values()
 
     @property
     def output_transfer_data(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'output_transfer_data' is deprecated in favor of the function 'get_output_transfer_data'",
             DeprecationWarning,
         )
         return self.get_output_transfer_data()
 
     def get_output_transfer_data(self):
```

### Comparing `ewokscore-0.4.1/src/ewokscore/task_discovery.py` & `ewokscore-0.4.2/src/ewokscore/task_discovery.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import sys
 import inspect
-import importlib
-import importlib.util
 from typing import Callable, Iterable, Optional
-from .task import Task
+
 from ewoksutils.import_utils import qualname
+from ewoksutils.import_utils import import_module
+
+from .task import Task
 
 
 def discover_tasks_from_modules(
     *module_names: Iterable[str], task_type="class"
 ) -> Iterable[dict]:
     return list(iter_discover_tasks_from_modules(*module_names, task_type=task_type))
 
 
 def iter_discover_tasks_from_modules(
-    *module_names: Iterable[str], task_type="class"
+    *module_names: Iterable[str], task_type="class", reload: bool = False
 ) -> Iterable[dict]:
     if "" not in sys.path:
         # This happens when the python process was launched
         # through a python console script
         sys.path.append("")
 
     if task_type == "method":
-        yield from _iter_method_tasks(*module_names)
+        yield from _iter_method_tasks(*module_names, reload=reload)
     elif task_type == "ppfmethod":
         yield from _iter_method_tasks(
-            *module_names, filter_method_name=lambda name: name == "run"
+            *module_names, filter_method_name=lambda name: name == "run", reload=reload
         )
     elif task_type == "class":
         for module_name in module_names:
-            importlib.import_module(module_name)
+            import_module(module_name, reload=reload)
         yield from _iter_registered_tasks(*module_names)
     else:
         raise ValueError("Class type does not support discovery")
 
 
 def _iter_registered_tasks(*filter_modules: Iterable[str]) -> Iterable[dict]:
     """Yields all task classes registered in the current process."""
@@ -53,21 +54,22 @@
             "output_names": list(cls.output_names()),
             "category": category,
         }
 
 
 def _iter_method_tasks(
     *module_names: Iterable[str],
-    filter_method_name: Optional[Callable[[str], bool]] = None
+    filter_method_name: Optional[Callable[[str], bool]] = None,
+    reload: bool = False
 ) -> Iterable[dict]:
     """Yields all task methods from the provided module_names. The module_names will be will
     imported for discovery.
     """
     for module_name in module_names:
-        mod = importlib.import_module(module_name)
+        mod = import_module(module_name, reload=reload)
         for method in inspect.getmembers(mod, inspect.isfunction):
             method_name, method_qn = method
             if filter_method_name and not filter_method_name(method_name):
                 continue
             if method_name.startswith("_"):
                 continue
             task_identifier = qualname(method_qn)
```

### Comparing `ewokscore-0.4.1/src/ewokscore/taskwithprogress.py` & `ewokscore-0.4.2/src/ewokscore/taskwithprogress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/__init__.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic1.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/acyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic2.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/acyclic2.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic3.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/acyclic3.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/cyclic1.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/cyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/demo.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/demo.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/triangle1.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/graphs/triangle1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/sumlist.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/sumlist.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/sumtask.py` & `ewokscore-0.4.2/src/ewokscore/tests/examples/tasks/sumtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_cli_utils.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_default_error_handlers.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_default_error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_dynamic_tasks.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_dynamic_tasks.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_events.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_examples.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_execute_graph.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_execute_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_graph.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_graph_io.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_graph_schema.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_graph_schema.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_graph_serialize.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_graph_start_end_nodes.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_graph_start_end_nodes.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_hashing.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_link_is_required.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_link_is_required.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_method_task.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_method_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_persistence.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_script_task.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_script_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_sub_graph.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_sub_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_sub_graph_serialize.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_sub_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_task.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_task_discovery.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_task_progress.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_task_progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_uri.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_variable.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_variable_namespaces.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_variable_namespaces.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/test_workflow_events.py` & `ewokscore-0.4.2/src/ewokscore/tests/test_workflow_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/tests/utils/results.py` & `ewokscore-0.4.2/src/ewokscore/tests/utils/results.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/utils.py` & `ewokscore-0.4.2/src/ewokscore/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.1/src/ewokscore/variable.py` & `ewokscore-0.4.2/src/ewokscore/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,47 +417,51 @@
     def force_non_existing(self):
         super().force_non_existing()
         for v in self.values():
             v.force_non_existing()
 
     @property
     def variable_uhashes(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'variable_uhashes' is deprecated in favor of the function 'get_variable_uhashes'",
             DeprecationWarning,
         )
         return self.get_variable_uhashes()
 
     def get_variable_uhashes(self):
         return {name: var.uhash for name, var in self.items()}
 
     @property
     def variable_values(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'variable_values' is deprecated in favor of the function 'get_variable_values'",
             DeprecationWarning,
         )
         return self.get_variable_values()
 
     def get_variable_values(self):
         return {k: v.value for k, v in self.items() if not v.is_missing()}
 
     @property
     def variable_data_proxies(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'variable_data_proxies' is deprecated in favor of the function 'get_variable_data_proxies'",
             DeprecationWarning,
         )
         return self.get_variable_data_proxies()
 
     def get_variable_data_proxies(self):
         return {k: v.data_proxy for k, v in self.items()}
 
     @property
     def variable_uris(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'variable_uris' is deprecated in favor of the function 'get_variable_uris'",
             DeprecationWarning,
         )
         return self.get_variable_uris()
 
     def get_variable_uris(self):
@@ -466,14 +470,15 @@
             proxy = v.data_proxy
             if proxy:
                 uris[k] = proxy.uri
         return uris
 
     @property
     def variable_transfer_data(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'variable_transfer_data' is deprecated in favor of the function 'get_variable_transfer_data'",
             DeprecationWarning,
         )
         return self.get_variable_transfer_data()
 
     def get_variable_transfer_data(self):
@@ -487,14 +492,15 @@
                 data[name] = var.copy_without_references()
             else:
                 data[name] = var.value
         return data
 
     @property
     def named_variable_values(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'named_variable_values' is deprecated in favor of the function 'get_named_variable_values'",
             DeprecationWarning,
         )
         return self.get_named_variable_values()
 
     def get_named_variable_values(self):
@@ -502,14 +508,15 @@
             k: v.value
             for k, v in self.items()
             if isinstance(k, str) and not v.is_missing()
         }
 
     @property
     def positional_variable_values(self):
+        """DEPRECATED"""
         warnings.warn(
             "the property 'positional_variable_values' is deprecated in favor of the function 'get_positional_variable_values'",
             DeprecationWarning,
         )
         return self.get_positional_variable_values()
 
     def get_positional_variable_values(self):
```

### Comparing `ewokscore-0.4.1/src/ewokscore.egg-info/PKG-INFO` & `ewokscore-0.4.2/src/ewokscore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.4.1
+Version: 0.4.2
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
```

### Comparing `ewokscore-0.4.1/src/ewokscore.egg-info/SOURCES.txt` & `ewokscore-0.4.2/src/ewokscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

