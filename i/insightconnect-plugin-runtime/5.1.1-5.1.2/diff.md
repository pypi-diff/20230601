# Comparing `tmp/insightconnect-plugin-runtime-5.1.1.tar.gz` & `tmp/insightconnect-plugin-runtime-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insightconnect-plugin-runtime-5.1.1.tar", last modified: Fri May 12 11:21:03 2023, max compression
+gzip compressed data, was "insightconnect-plugin-runtime-5.1.2.tar", last modified: Thu Jun  1 09:41:42 2023, max compression
```

## Comparing `insightconnect-plugin-runtime-5.1.1.tar` & `insightconnect-plugin-runtime-5.1.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.078558 insightconnect-plugin-runtime-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-12 11:21:03.078558 insightconnect-plugin-runtime-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-05-12 11:20:24.000000 insightconnect-plugin-runtime-5.1.1/insightconnect-plugin-swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.070558 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.070558 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.070558 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/clients/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/clients/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.070558 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/data/input_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/data/output_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.070558 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-12 11:21:03.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-12 11:21:03.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:21:03.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-12 11:21:03.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 11:21:03.000000 insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:21:03.078558 insightconnect-plugin-runtime-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.070558 insightconnect-plugin-runtime-5.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
--rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.074558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.078558 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:03.078558 insightconnect-plugin-runtime-5.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_aws_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_custom_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_server_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 11:19:28.000000 insightconnect-plugin-runtime-5.1.1/tests/unit/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.700027 insightconnect-plugin-runtime-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-01 09:41:42.700027 insightconnect-plugin-runtime-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-06-01 09:40:59.000000 insightconnect-plugin-runtime-5.1.2/insightconnect-plugin-swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.692027 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26847 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/clients/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/clients/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/data/input_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/data/output_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-01 09:41:42.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-01 09:41:42.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:41:42.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 09:41:42.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 09:41:42.000000 insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:41:42.700027 insightconnect-plugin-runtime-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.696027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.700027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.700027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.700027 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:41:42.700027 insightconnect-plugin-runtime-5.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_aws_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_custom_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_server_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 09:40:05.000000 insightconnect-plugin-runtime-5.1.2/tests/unit/test_variables.py
```

### Comparing `insightconnect-plugin-runtime-5.1.1/PKG-INFO` & `insightconnect-plugin-runtime-5.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.1.1
+Version: 5.1.2
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
```

### Comparing `insightconnect-plugin-runtime-5.1.1/README.md` & `insightconnect-plugin-runtime-5.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
```

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect-plugin-swagger.json` & `insightconnect-plugin-runtime-5.1.2/insightconnect-plugin-swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -447,95 +447,95 @@
         "version": "1.0"
     },
     "swagger": "2.0",
     "definitions": {
         "PluginInfo": {
             "type": "object",
             "properties": {
-                "number_of_workers": {
-                    "type": "integer",
-                    "format": "int32"
-                },
-                "title": {
+                "plugin_spec_version": {
                     "type": "string"
                 },
-                "enable_cache": {
-                    "type": "boolean"
-                },
-                "threads": {
-                    "type": "integer",
-                    "format": "int32"
+                "vendor": {
+                    "type": "string"
                 },
-                "name": {
+                "description": {
                     "type": "string"
                 },
-                "plugin_spec_version": {
+                "support": {
                     "type": "string"
                 },
-                "description": {
+                "title": {
                     "type": "string"
                 },
-                "version": {
+                "enable_cache": {
+                    "type": "boolean"
+                },
+                "name": {
                     "type": "string"
                 },
                 "tags": {
                     "type": "array",
                     "items": {
                         "type": "string"
                     }
                 },
-                "sdk_version": {
-                    "type": "string"
+                "number_of_workers": {
+                    "type": "integer",
+                    "format": "int32"
                 },
-                "support": {
+                "threads": {
+                    "type": "integer",
+                    "format": "int32"
+                },
+                "sdk_version": {
                     "type": "string"
                 },
-                "vendor": {
+                "version": {
                     "type": "string"
                 }
             }
         },
         "ActionTriggerOutputBody": {
             "type": "object",
             "properties": {
                 "log": {
                     "type": "string"
                 },
-                "status": {
-                    "type": "string"
+                "meta": {
+                    "type": "object"
                 },
                 "output": {
                     "type": "object"
                 },
-                "meta": {
-                    "type": "object"
+                "status": {
+                    "type": "string"
                 }
             },
             "required": [
                 "log",
                 "meta",
                 "output",
                 "status"
             ]
         },
         "ActionTriggerOutput": {
             "type": "object",
             "properties": {
-                "version": {
-                    "type": "string"
+                "body": {
+                    "$ref": "#/definitions/ActionTriggerOutputBody"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "action_event",
                         "trigger_event"
                     ]
                 },
-                "body": {
-                    "$ref": "#/definitions/ActionTriggerOutputBody"
+                "version": {
+                    "type": "string"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
@@ -545,203 +545,203 @@
             "properties": {
                 "status": {
                     "type": "string"
                 },
                 "log": {
                     "type": "string"
                 },
-                "output": {
+                "state": {
                     "type": "object"
                 },
                 "meta": {
                     "type": "object"
                 },
-                "state": {
+                "output": {
                     "type": "object"
                 }
             },
             "required": [
                 "log",
                 "meta",
                 "output",
                 "state",
                 "status"
             ]
         },
         "TaskOutput": {
             "type": "object",
             "properties": {
-                "version": {
-                    "type": "string"
+                "body": {
+                    "$ref": "#/definitions/TaskOutputBody"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "task_event"
                     ]
                 },
-                "body": {
-                    "$ref": "#/definitions/TaskOutputBody"
+                "version": {
+                    "type": "string"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "ActionTriggerInputBody": {
             "type": "object",
             "properties": {
-                "action": {
-                    "type": "string"
-                },
                 "connection": {
                     "type": "object"
                 },
+                "action": {
+                    "type": "string"
+                },
                 "input": {
                     "type": "object"
                 }
             },
             "required": [
                 "action",
                 "connection",
                 "input"
             ]
         },
         "ActionTriggerInput": {
             "type": "object",
             "properties": {
-                "version": {
-                    "type": "string"
+                "body": {
+                    "$ref": "#/definitions/ActionTriggerInputBody"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "action_event",
                         "trigger_event"
                     ]
                 },
-                "body": {
-                    "$ref": "#/definitions/ActionTriggerInputBody"
+                "version": {
+                    "type": "string"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "TaskInputBody": {
             "type": "object",
             "properties": {
-                "task": {
-                    "type": "string"
-                },
                 "connection": {
                     "type": "object"
                 },
-                "state": {
+                "input": {
                     "type": "object"
                 },
-                "input": {
+                "state": {
                     "type": "object"
+                },
+                "task": {
+                    "type": "string"
                 }
             },
             "required": [
                 "connection",
                 "input",
                 "state",
                 "task"
             ]
         },
         "TaskInput": {
             "type": "object",
             "properties": {
-                "version": {
-                    "type": "string"
+                "body": {
+                    "$ref": "#/definitions/TaskInputBody"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "task_event"
                     ]
                 },
-                "body": {
-                    "$ref": "#/definitions/TaskInputBody"
+                "version": {
+                    "type": "string"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "ActionTriggerDetails": {
             "type": "object",
             "properties": {
-                "input": {
-                    "type": "object"
-                },
-                "title": {
+                "description": {
                     "type": "string"
                 },
                 "output": {
                     "type": "object"
                 },
-                "description": {
+                "input": {
+                    "type": "object"
+                },
+                "title": {
                     "type": "string"
                 }
             }
         },
         "ConnectionDetails": {
             "type": "object",
             "properties": {
+                "required": {
+                    "type": "array",
+                    "items": {
+                        "type": "string"
+                    }
+                },
                 "type": {
                     "type": "string"
                 },
                 "properties": {
                     "type": "object"
                 },
                 "title": {
                     "type": "string"
-                },
-                "required": {
-                    "type": "array",
-                    "items": {
-                        "type": "string"
-                    }
                 }
             }
         },
         "ConnectionTestOutput": {
             "type": "object",
             "properties": {
                 "message": {
                     "type": "object"
                 }
             }
         },
         "TaskDetails": {
             "type": "object",
             "properties": {
+                "description": {
+                    "type": "string"
+                },
                 "title": {
                     "type": "string"
                 },
                 "input": {
                     "type": "object"
                 },
-                "schedule": {
-                    "type": "object"
-                },
                 "state": {
                     "type": "object"
                 },
-                "description": {
-                    "type": "string"
+                "schedule": {
+                    "type": "object"
                 },
                 "output": {
                     "type": "object"
                 }
             }
         }
     }
```

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/__init__.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/api/endpoints.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/api/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from insightconnect_plugin_runtime.api.schemas import (
     PluginInfoSchema,
     ActionTriggerDetailsSchema,
     TaskDetailsSchema,
     ConnectionDetailsSchema,
 )
+from insightconnect_plugin_runtime.util import OutputMasker
 
 
 class Endpoints:
     def __init__(self, logger, plugin, spec, debug, workers, threads, master_pid):
         self.plugin = plugin
         self.logger = structlog.get_logger("plugin")
         self.spec = spec
@@ -676,14 +677,15 @@
         except Exception:
             self.logger.warn("Unable to get SDK version")
             version = "0.0.0"
 
         return version
 
     def run_action_trigger_task(self, input_message, test=False):
+        connection = input_message.get("body", {}).get("connection", {})
         status_code = 200
         output = None
         try:
             output = self.plugin.handle_step(
                 input_message, is_debug=self.debug, is_test=test
             )
         except LoggedException as error:
@@ -701,15 +703,15 @@
             elif isinstance(wrapped_exception, ServerException):
                 # I'm unsure about this
                 status_code = 500
             else:
                 status_code = 500
         finally:
             self.logger.debug("Request output: %s", output)
-            response = jsonify(output)
+            response = jsonify(OutputMasker.mask_output_data(connection, output))
             response.status_code = status_code
             return response
 
     @staticmethod
     def handle_wrapped_exception(wrapped_exception):
         if isinstance(wrapped_exception, (ConnectionTestException, ClientException)):
             return 400
```

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/api/schemas.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/api/schemas.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/cli.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/clients/aws_client.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/clients/aws_client.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/clients/oauth.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/clients/oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/connection.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/connection.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/data/input_message_schema.json` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/data/input_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/data/output_message_schema.json` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/data/output_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/dispatcher.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/dispatcher.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/exceptions.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/helper.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/helper.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/metrics.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/plugin.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/plugin.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/schema.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/server.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/step.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/step.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/trigger.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime/variables.py` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime/variables.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime.egg-info/PKG-INFO` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.1.1
+Version: 5.1.2
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
```

### Comparing `insightconnect-plugin-runtime-5.1.1/insightconnect_plugin_runtime.egg-info/SOURCES.txt` & `insightconnect-plugin-runtime-5.1.2/insightconnect_plugin_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/setup.py` & `insightconnect-plugin-runtime-5.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="insightconnect-plugin-runtime",
-    version="5.1.1",
+    version="5.1.2",
     description="InsightConnect Plugin Runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rapid7 Integrations Alliance",
     author_email="integrationalliance@rapid7.com",
     url="https://github.com/rapid7/komand-plugin-sdk-python",
     packages=find_packages(),
     install_requires=[
-        "requests==2.26.0",
+        "requests==2.31.0",
         "python_jsonschema_objects==0.3.12",
         "jsonschema==3.2.0",
         "certifi==2022.12.7",
         "Flask==2.3.2",
         "gunicorn==20.0.4",
         "greenlet>=0.4.17, <=1.1.2",
         "gevent==20.9.0",
```

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/__init__.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/__init__.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/conftest.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/test_cli.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/test_hello_world.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/plugin/hello_world/tests/test_server.py` & `insightconnect-plugin-runtime-5.1.2/tests/plugin/hello_world/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_action.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_aws_action.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_aws_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_custom_encoder.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_endpoints.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_exceptions.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_helpers.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_metrics.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_oauth.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_schema.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_server_spec.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_server_spec.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.1/tests/unit/test_trigger.py` & `insightconnect-plugin-runtime-5.1.2/tests/unit/test_trigger.py`

 * *Files identical despite different names*

