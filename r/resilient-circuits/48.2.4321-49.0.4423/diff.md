# Comparing `tmp/resilient_circuits-48.2.4321.tar.gz` & `tmp/resilient_circuits-49.0.4423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_circuits-48.2.4321.tar", last modified: Fri May  5 12:35:11 2023, max compression
+gzip compressed data, was "resilient_circuits-49.0.4423.tar", last modified: Thu Jun  1 15:58:50 2023, max compression
```

## Comparing `resilient_circuits-48.2.4321.tar` & `resilient_circuits-49.0.4423.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12364 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-05-05 12:35:11.447470 resilient_circuits-48.2.4321/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.439470 resilient_circuits-48.2.4321/resilient_circuits/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/README
--rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/action_message.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    59349 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/actions_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/actions_test_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10353 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11847 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/app_argument_parser.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6029 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/app_function_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/app_restartable.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.439470 resilient_circuits-48.2.4321/resilient_circuits/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/bin/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/bin/res_action_test.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    17085 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/bin/resilient_circuits_cmd.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2996 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/bin/service_wrapper.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.439470 resilient_circuits-48.2.4321/resilient_circuits/cmds/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13670 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/cmds/selftest.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/resilient_circuits/data/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3063 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/data/app.config.base
--rwxrwxr-x   0 travis    (2000) travis    (2000)    20046 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11921 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/helpers.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/keyring_arguments.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3395 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/rest_helper.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    14446 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/stomp_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/stomp_events.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/stomp_transport.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/template_functions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/resilient_circuits/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/util/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/util/resilient_config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/util/resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1128 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/validate_configs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.439470 resilient_circuits-48.2.4321/resilient_circuits.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/top_level.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1511 2023-05-05 12:35:11.447470 resilient_circuits-48.2.4321/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/cmds/test_selftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3803 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/selftest_tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/selftest_tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/selftest_tests/mocked_fail_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/selftest_tests/mocked_success_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      282 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/selftest_tests/mocked_unimplemented_script.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_commented_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_import_definition.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      545 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_action_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_actions_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_app_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1663 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_app_restartable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7756 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7974 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_resilient_circuits_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_rest_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_stomp_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/util/test_resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12779 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/PKG-INFO
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/LICENSE
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/README
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/action_message.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    59967 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/actions_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/actions_test_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11442 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12400 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/app_argument_parser.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6658 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/app_function_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/app_restartable.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/bin/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/bin/res_action_test.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    17085 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/bin/resilient_circuits_cmd.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2996 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/bin/service_wrapper.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/cmds/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15923 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/cmds/selftest.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2824 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/data/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3063 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/data/app.config.base
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    19901 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11958 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/helpers.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/keyring_arguments.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3395 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/rest_helper.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    14446 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/stomp_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/stomp_events.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/stomp_transport.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/template_functions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/util/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/util/resilient_config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/util/resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1128 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/resilient_circuits/validate_configs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.229552 resilient_circuits-49.0.4423/resilient_circuits.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      176 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-01 15:58:50.000000 resilient_circuits-49.0.4423/resilient_circuits.egg-info/top_level.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1511 2023-06-01 15:58:50.237552 resilient_circuits-49.0.4423/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      287 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5845 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/cmds/test_selftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3803 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/selftest_tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/selftest_tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/selftest_tests/mocked_fail_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/selftest_tests/mocked_success_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      282 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/selftest_tests/mocked_unimplemented_script.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_commented_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_import_definition.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      545 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_action_message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_actions_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2491 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_app_restartable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7756 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7974 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_resilient_circuits_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_rest_helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_stomp_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:50.233552 resilient_circuits-49.0.4423/tests/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tests/util/test_resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2023-06-01 15:57:43.000000 resilient_circuits-49.0.4423/tox.ini
```

### Comparing `resilient_circuits-48.2.4321/CHANGES` & `resilient_circuits-49.0.4423/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+**2023-05: version 49.0**
+
+* Improved logging on restarts
+* Improved obfuscation of sensitive information from app.config in logs
+* Added ability to disable persistent sessions for ``resilient-lib.RequestsCommon`` in app functions using new optional ``rc_use_persistent_sessions`` configuration parameter
+* Added ``resilient-app-config-plugins`` as a new package to manage third party credentials within SOAR apps
+
 **2023-04: version 48.1**
 
 * Better log handling for errors upon restart
 * Added new configs for log rotation. ``log_max_bytes`` sets the maximum bytes per log file; defaults to ``10000000``. 
   ``log_backup_count`` sets the maximum number of log files to keep as backups while files rotate; defaults to ``10``
 * Improved log filtering for sensitive values
```

### Comparing `resilient_circuits-48.2.4321/PKG-INFO` & `resilient_circuits-49.0.4423/resilient_circuits.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resilient_circuits
-Version: 48.2.4321
+Name: resilient-circuits
+Version: 49.0.4423
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-48.2.4321/README.md` & `resilient_circuits-49.0.4423/README.md`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/LICENSE` & `resilient_circuits-49.0.4423/resilient_circuits/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/__init__.py` & `resilient_circuits-49.0.4423/resilient_circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/action_message.py` & `resilient_circuits-49.0.4423/resilient_circuits/action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/actions_component.py` & `resilient_circuits-49.0.4423/resilient_circuits/actions_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,15 +920,21 @@
                     str_traceback = "".join(traceback)
 
                     if logging.getLogger().getEffectiveLevel() == logging.DEBUG:
                         message = u"{0}\n{1}".format(message, str_traceback)
 
                     log_message = u"{0}\n{1}".format(message, str_traceback)
 
-            LOG.error(u"%s (%s): %s", repr(fevent), repr(etype), log_message)
+            # any event that had "opts" as an argument to it will be output here with "repr(fevent)"
+            # so we have to see if the event has "opts" as an arg. If so, then just output the
+            # type of the event, not the whole repr of the event.
+            # Example:
+            # ERROR [actions_component] Circuits event <class 'resilient_circuits.app_restartable.reload'> raised exception ...
+            rep = type(fevent) if hasattr(fevent, "kwargs") and "opts" in fevent.kwargs else repr(fevent)
+            LOG.error(u"Circuits event %s raised exception (%s): %s", rep, repr(etype), log_message)
 
             # Try find the underlying Action or Function message
             if fevent and fevent.args and not isinstance(fevent, ActionMessageBase):
                 for arg in fevent.args:
                     if isinstance(arg, ActionMessageBase):
                         fevent = arg
                         break
@@ -1230,15 +1236,15 @@
                 # reply_message is an ActionAcknowledgementDTO
                 reply_dto = {"message_type": status,
                              "message": message,
                              "complete": True}
                 if function_result:
                     LOG.debug("[%s] Result: %s", function_result.name, function_result.value)
                     reply_dto["results"] = function_result.value
-                reply_message = json.dumps(reply_dto, indent=2)
+                reply_message = json.dumps(reply_dto, indent=2, default=lambda o: "<<non-serializable: {0}>>".format(type(o).__qualname__))
                 if not fevent.test:
                     self.fire(Send(headers={'correlation-id': correlation_id},
                                    body=reply_message,
                                    destination=reply_to,
                                    message_id=message_id))
                 else:
                     # Test action, nothing to Ack
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/actions_test_component.py` & `resilient_circuits-49.0.4423/resilient_circuits/actions_test_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/app.py` & `resilient_circuits-49.0.4423/resilient_circuits/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2018. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 """Action Module server
 
 This uses the `Circuits <http://circuitsframework.com/>` framework to
 listen on multiple message destinations, send their events to the relevant
 handlers, and acknowledge the messages when they have been processed.
 
 """
 
 from __future__ import print_function
 
 import logging
 from logging.handlers import RotatingFileHandler
-from six import string_types
+from six import string_types, PY3
 import re
 import os
 import filelock
 from circuits import Manager, BaseComponent, Component, Debugger, Loader
 from resilient import get_config_file
 from resilient import constants as resilient_constants
 from resilient_circuits import constants, helpers
@@ -36,19 +36,32 @@
 
     """
     def __init__(self):
         super(RedactingFilter, self).__init__()
 
     def filter(self, record):
         # Best effort regex filter pattern to redact password logging.
+        if PY3: # struggles to convert unicode dicts in PY2 -- so PY3 only
+            record.msg = str(record.msg)
         if isinstance(record.msg, string_types):
             for p in constants.PASSWD_PATTERNS:
                 if p in record.msg.lower():
-                    regex = r"{0}(?=.*?'|\":\s)(None,|.+?,|.+?'|.+\"|}})".format(p)
-                    record.msg = re.sub(regex, r"***", record.msg)
+                    regex = re.compile(r"""
+                        ({0}           # start capturing group for password pattern from constants.PASSWD_PATTERNS
+                        \w*?[\'\"]?    # match any word characters (lazy) and zero or one quotation marks
+                        \W*?u?[\'\"]   # match any non-word characters (lazy) up until exactly one quotation mark
+                                       # and potentially a u'' situation for PY27
+                                       # (this quotation mark indicates the beginning of the secret value)
+                        )              # end first capturing group
+                        (.+?)          # capture the problematic content (lazy capture up until end quotation mark)
+                        ([\'\"])       # capturing group to end the regex match
+                    """.format(p), re.X)
+
+                    # keep first and third capturing groups, but replace inner group with "***"
+                    record.msg = regex.sub(r"\1***\3", record.msg)
 
         return True
 
 
 # Main component for our application
 class App(Component):
     """Our main app component, which sets up the Resilient services and other components"""
@@ -80,14 +93,15 @@
         if self.opts.get("api_key_id", None):
             LOG.info("Resilient api key id: %s", self.opts.get("api_key_id"))
         if self.opts.get("api_key_id", None) and self.opts.get("email", None):
             LOG.warning("The user and api key configuration settings are both enabled. Credentials will default to the "
                         "api key settings.")
         LOG.info("Resilient org: %s", self.opts.get("org"))
         LOG.info("Logging Level: %s", self.opts.get("loglevel"))
+        LOG.info("App Config plugin: %s", self.opts.pam_plugin.__class__.__name__)
         if self.opts.get("test_actions", False):
             # Make all components aware that we are in test mode
             ResilientComponent.test_mode = True
 
         # Make all components aware that we are in selftest mode
         ResilientComponent.IS_SELFTEST = self.IS_SELFTEST
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/app_argument_parser.py` & `resilient_circuits-49.0.4423/resilient_circuits/app_argument_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2021. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 import logging
 import os
 
 from resilient import constants as res_constants
 from resilient import get_config_file
 from resilient import helpers as res_helpers
@@ -28,14 +28,15 @@
     DEFAULT_NO_PROMPT_PASS = "False"
     DEFAULT_STOMP_TIMEOUT = 60
     DEFAULT_STOMP_MAX_RETRIES = 3
     DEFAULT_MAX_CONNECTION_RETRIES = res_constants.APP_CONFIG_MAX_CONNECTION_RETRIES_DEFAULT
     DEFAULT_NUM_WORKERS = 25
     DEFAULT_APP_EXCEPTION = False
     DEFAULT_HEARTBEAT_TIMEOUT_THRESHOLD = None
+    DEFAULT_RC_USE_PERSISTENT_SESSIONS = True
 
     def __init__(self, config_file=None):
 
         self._setup_temp_logger()
         config_file = config_file or get_config_file()
         super(AppArgumentParser, self).__init__(config_file=config_file)
 
@@ -69,14 +70,15 @@
                                             "log_http_responses") or ""
         default_resource_prefix = self.getopt(self.DEFAULT_APP_SECTION, "resource_prefix") or None
         default_num_workers = self.getopt(self.DEFAULT_APP_SECTION, "num_workers") or self.DEFAULT_NUM_WORKERS
         default_trap_exception = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_TRAP_EXCEPTION) or self.DEFAULT_APP_EXCEPTION
         default_trap_exception = self._is_true(default_trap_exception)
 
         default_heartbeat_timeout_threshold = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_HEARTBEAT_TIMEOUT_THRESHOLD) or self.DEFAULT_HEARTBEAT_TIMEOUT_THRESHOLD
+        default_rc_use_persistent_sessions = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_RC_USE_PERSISTENT_SESSIONS) or self.DEFAULT_RC_USE_PERSISTENT_SESSIONS
 
         self._unset_temp_logger()
 
         self.add_argument("--stomp-host",
                           type=str,
                           default=default_stomp_url,
                           help="Resilient server STOMP host url")
@@ -171,25 +173,29 @@
                           type=bool,
                           default=default_trap_exception,
                           help=("If set to 'True' a Function's exception will be ignored"))
         self.add_argument("--{0}".format(constants.APP_CONFIG_HEARTBEAT_TIMEOUT_THRESHOLD),
                           type=int,
                           default=default_heartbeat_timeout_threshold,
                           help=("The amount of time in seconds that can occur between HeartbeatTimeouts before exiting"))
+        self.add_argument("--{0}".format(constants.APP_CONFIG_RC_USE_PERSISTENT_SESSIONS),
+                          type=str,
+                          default=default_rc_use_persistent_sessions,
+                          help=("Set to False to disable the use of persistent sessions with RequestsCommon in app functions"))
 
     def parse_args(self, args=None, namespace=None, ALLOW_UNRECOGNIZED=False):
         """Parse commandline arguments and construct an opts dictionary"""
         self._setup_temp_logger()
         opts = super(AppArgumentParser, self).parse_args(args, namespace, ALLOW_UNRECOGNIZED)
         if self.config:
             for section in self.config.sections():
                 items = dict((item.lower(), self.config.get(section, item)) for item in self.config.options(section))
                 opts.update({section: items})
 
-            parse_parameters(opts)
+            opts = parse_parameters(opts)
 
             # Once we have read the app.config and decrypted any protected secrets
             # we must remove the secrets directory
             res_helpers.remove_secrets_dir()
 
         validate_configs(opts, VALIDATE_DICT)
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/app_function_component.py` & `resilient_circuits-49.0.4423/resilient_circuits/app_function_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2021. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 """Implementation of AppFunctionComponent"""
 
 import logging
 import threading
 from collections import namedtuple
-from resilient_circuits import ResilientComponent, handler, StatusMessage
-from resilient_lib import RequestsCommon, validate_fields
+
+from resilient_circuits import (ResilientComponent, StatusMessage, constants,
+                                handler)
+from resilient_circuits.app_argument_parser import AppArgumentParser
+from resilient_lib import (RequestsCommon, RequestsCommonWithoutSession,
+                           str_to_bool, validate_fields)
 
 
 class AppFunctionComponent(ResilientComponent):
     """
     Each package that has been generated with the ``resilient-sdk codegen`` command
     that contains a SOAR Function, an :class:`AppFunctionComponent` will be generated
     in the package's ``components`` directory
@@ -56,19 +60,28 @@
 
         # Validate app_configs and get dictionary as result
         self._app_configs_as_dict = validate_fields(required_app_configs, opts.get(package_name, {}))
 
         # This variable also is used to get the app.configs
         self.options = self._app_configs_as_dict
 
-        # Instansiate RequestsCommon with dictionary of _app_configs_as_dict
-        self.rc = RequestsCommon(opts=opts, function_opts=self._app_configs_as_dict)
-
-        # Convert _app_configs_as_dict to namedtuple
-        self.app_configs = namedtuple("app_configs", self._app_configs_as_dict.keys())(*self._app_configs_as_dict.values())
+        # Instantiate RequestsCommon with dictionary of _app_configs_as_dict
+        if str_to_bool(opts.get(constants.APP_CONFIG_RC_USE_PERSISTENT_SESSIONS, AppArgumentParser.DEFAULT_RC_USE_PERSISTENT_SESSIONS)):
+            requests_common_type = RequestsCommon
+        else:
+            requests_common_type = RequestsCommonWithoutSession
+
+        self.rc = requests_common_type(opts=opts, function_opts=self._app_configs_as_dict)
+
+        # NOTE: self.app_configs used to be a namedtuple.
+        # Since v49 this is no longer a namedtuple.
+        # It behaves the same way that a namedtuple would, but
+        # instead is a resilient.app_config.AppConfig object.
+        # This allows for pluggable PAM connectors/plugins
+        self.app_configs = self._app_configs_as_dict
 
         self._local_storage = threading.local()
 
         self.LOG = logging.getLogger(__name__)
 
         super(AppFunctionComponent, self).__init__(opts)
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/app_restartable.py` & `resilient_circuits-49.0.4423/resilient_circuits/app_restartable.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/bin/res_action_test.py` & `resilient_circuits-49.0.4423/resilient_circuits/bin/res_action_test.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/bin/resilient_circuits_cmd.py` & `resilient_circuits-49.0.4423/resilient_circuits/bin/resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/bin/service_wrapper.py` & `resilient_circuits-49.0.4423/resilient_circuits/bin/service_wrapper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/cmds/selftest.py` & `resilient_circuits-49.0.4423/resilient_circuits/cmds/selftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2021. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 import logging
 import os
 import time
 from collections import defaultdict
 from threading import Thread
 
@@ -46,14 +46,63 @@
     # Remove resilient-circuits logging handler
     LOG.parent.handlers = []
 
     LOG.info("\nERROR: could not connect to SOAR at '{0}'.\nReason: {1}\nError Code: {2}".format(host, reason, ERROR_EXIT_CODES_MAP.get(status_code, 1)))
     exit(ERROR_EXIT_CODES_MAP.get(status_code, 1))
 
 
+def check_pam_plugin_selftest(app_configs):
+    """
+    Run PAM plugin's 'selftest' function which will check if the plugin
+    is properly configured.
+
+    Some plugins may not have a selftest or some app configurations may
+    not have a plugin -- in either of those cases, let it go with simply
+    a log message.
+
+    In the case the the plugin exists, and has a selftest, run it.
+    The function should return a tuple of bool, str where the first
+    element is True if the plugin is correctly configured and
+    the second element is a reason if it is incorrectly configured.
+
+    :param app_configs: app configs for the app -- should contain a .pam_plugin object
+    :type app_configs: ``resilient.app_config.AppConfigManager``
+    """
+    LOG.info("{0}Testing PAM Plugin details{0}".format(constants.LOG_DIVIDER))
+
+    if not app_configs or not hasattr(app_configs, "pam_plugin"):
+        LOG.info("{0}No Plugin specified. Skipping test{0}".format(constants.LOG_DIVIDER))
+        return
+
+    try:
+        LOG.info("- Running pam plugin selftest")
+        result = app_configs.pam_plugin.selftest()
+    except NotImplementedError:
+        LOG.warning("{0}PAM Plugin selftest not implemented for custom plugin. Skipping test{0}".format(constants.LOG_DIVIDER))
+        return
+    except Exception as err:
+        LOG.warning("Unknown error while running PAM Plugin selftest: {0}".format(str(err)))
+        return
+
+    # result should be a tuple of (bool, str),
+    # but in the case that something is improperly implemented,
+    # assume that if not a tuple that the result is the bool portion
+    # and use that bool and "REASON UNKNOWN"
+    if isinstance(result, tuple):
+        selftest_pass, reason = result
+    else:
+        LOG.warning("PAM Plugin selftest did not return the expected tuple. Make sure selftest is properly implemented")
+        selftest_pass, reason = (result, "REASON UNKNOWN")
+
+    if not selftest_pass:
+        LOG.error("\nERROR: PAM Plugin test failed. Reason: {0}.\nError Code: {1}".format(reason, ERROR_EXIT_CODES_MAP.get(1, 1)))
+        exit(ERROR_EXIT_CODES_MAP.get(1, 1))
+    else:
+        LOG.info("{0}PAM Plugin correctly configured{0}".format(constants.LOG_DIVIDER))
+
 def check_soar_rest_connection(cmd_line_args, app_configs):
     """
     Check if we can  successfully get a resilient_client
     therefore that will tell us if we have configured the app.config
     file correctly in order to establish a REST connection and authenticate
     with SOAR
 
@@ -302,12 +351,13 @@
     if hasattr(cmd_line_args, "print_env") and cmd_line_args.print_env:
         LOG.info("- Printing runtime environment")
         LOG.info(helpers.get_env_str(pkg_resources.working_set))
 
     LOG.info("- Getting app.configs")
     app_configs = helpers.get_configs(ALLOW_UNRECOGNIZED=True)
 
+    check_pam_plugin_selftest(app_configs)
     check_soar_rest_connection(cmd_line_args, app_configs)
     check_soar_stomp_connection(cmd_line_args, app_configs)
     run_apps_selftest(cmd_line_args, app_configs)
 
     LOG.info("{0}selftest complete{0}".format(constants.LOG_DIVIDER))
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/component_loader.py` & `resilient_circuits-49.0.4423/resilient_circuits/component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/constants.py` & `resilient_circuits-49.0.4423/resilient_circuits/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 SELFTEST_UNIMPLEMENTED_STATE = "unimplemented"
 
 # app configs
 INBOUND_MSG_APP_CONFIG_Q_NAME = "inbound_destination_api_name"
 APP_CONFIG_TRAP_EXCEPTION = "trap_exception"
 APP_CONFIG_SELFTEST_TIMEOUT = "selftest_timeout"
 APP_CONFIG_HEARTBEAT_TIMEOUT_THRESHOLD = "heartbeat_timeout_threshold"
+APP_CONFIG_RC_USE_PERSISTENT_SESSIONS = "rc_use_persistent_sessions"
 APP_CONFIG_LOG_MAX_BYTES = "log_max_bytes"
 APP_CONFIG_LOG_BACKUP_COUNT = "log_backup_count"
 
 # Headers
 HEADER_CIRCUITS_VER_KEY = "Resilient-Circuits-Version"
 HEADER_CIRCUITS_VER_VALUE = pkg_resources.get_distribution(PACKAGE_NAME).version
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/data/app.config.base` & `resilient_circuits-49.0.4423/resilient_circuits/data/app.config.base`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/decorators.py` & `resilient_circuits-49.0.4423/resilient_circuits/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,20 +162,16 @@
 
                 :param evt: The Event with the StompFrame and the Message read off the Message Destination
                 :type ia: resilient_circuits.action_message.FunctionMessage
                 """
                 result_list = []
                 LOG.debug("Running _invoke_inbound_app in Thread: %s", threading.currentThread().name)
 
-                # Get the required attribute from the message
-                message = evt.message
-                inbound_action = message.get("action", "Unknown")
-
                 # Invoke the actual Function
-                ia_results = ia(itself, evt.message, inbound_action)
+                ia_results = ia(itself, evt.message, evt.message.get("action", "Unknown"))
 
                 for r in ia_results:
                     LOG.debug(r)
                     result_list.append(r)
 
                 return result_list
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/helpers.py` & `resilient_circuits-49.0.4423/resilient_circuits/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2020. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 """Common Helper Functions for resilient-circuits"""
 import sys
 import pkg_resources
 import logging
 import copy
 import re
@@ -112,15 +112,15 @@
     Or uses the `get_config_file()` method in resilient if None
 
     :param path_config_file: path to the app.config to parse
     :type path_config_file: str
     :param ALLOW_UNRECOGNIZED: bool to specify if AppArgumentParser will allow unknown comandline args or not. Default is False
     :type ALLOW_UNRECOGNIZED: bool
     :return: dictionary of all the configs in the app.config file
-    :rtype: dict
+    :rtype: ``resilient.app_config.AppConfigManager``
     """
     from resilient import get_config_file
     from resilient_circuits.app_argument_parser import AppArgumentParser
 
     if not path_config_file:
         path_config_file = get_config_file()
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/rest_helper.py` & `resilient_circuits-49.0.4423/resilient_circuits/rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/stomp_component.py` & `resilient_circuits-49.0.4423/resilient_circuits/stomp_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/stomp_events.py` & `resilient_circuits-49.0.4423/resilient_circuits/stomp_events.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/stomp_transport.py` & `resilient_circuits-49.0.4423/resilient_circuits/stomp_transport.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/template_functions.py` & `resilient_circuits-49.0.4423/resilient_circuits/template_functions.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/util/__init__.py` & `resilient_circuits-49.0.4423/resilient_circuits/util/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/util/resilient_config.py` & `resilient_circuits-49.0.4423/resilient_circuits/util/resilient_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/util/resilient_customize.py` & `resilient_circuits-49.0.4423/resilient_circuits/util/resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits/validate_configs.py` & `resilient_circuits-49.0.4423/resilient_circuits/validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/resilient_circuits.egg-info/PKG-INFO` & `resilient_circuits-49.0.4423/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resilient-circuits
-Version: 48.2.4321
+Name: resilient_circuits
+Version: 49.0.4423
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-48.2.4321/resilient_circuits.egg-info/SOURCES.txt` & `resilient_circuits-49.0.4423/resilient_circuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/setup.cfg` & `resilient_circuits-49.0.4423/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient     >= 48.1
-	resilient-lib >= 48.1
+	resilient     >= 49.0
+	resilient-lib >= 49.0
 	
 	stompest      ~= 2.3
 	circuits      ~= 3.2
 	pysocks       ~= 1.6
 	filelock      ~= 3.2
 	
 	watchdog      ~= 2.1;  python_version >= "3.6"
```

### Comparing `resilient_circuits-48.2.4321/tests/conftest.py` & `resilient_circuits-49.0.4423/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/helpers.py` & `resilient_circuits-49.0.4423/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_app_config` & `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_app_config`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_app_function_component.py` & `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_commented_app_config` & `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_commented_app_config`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_component.py` & `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_constants.py` & `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_constants.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_function_component.py` & `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_import_definition.txt` & `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_import_definition.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_paths.py` & `resilient_circuits-49.0.4423/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_action_message.py` & `resilient_circuits-49.0.4423/tests/test_action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_actions_component.py` & `resilient_circuits-49.0.4423/tests/test_actions_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_app_config.py` & `resilient_circuits-49.0.4423/tests/test_app_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_app_function_component.py` & `resilient_circuits-49.0.4423/tests/test_app_function_component.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # (c) Copyright IBM Corp. 2010, 2021. All Rights Reserved.
 
-import pytest
-from resilient_lib import IntegrationError, RequestsCommon
-from resilient_circuits import StatusMessage
-from tests import mock_constants, AppFunctionMockComponent
+from resilient_circuits import StatusMessage, constants
+from resilient_lib import RequestsCommon, RequestsCommonWithoutSession
+from tests import AppFunctionMockComponent, mock_constants
 
+from resilient.app_config import AppConfigManager
 
 resilient_mock = mock_constants.RESILIENT_MOCK
 config_data = mock_constants.CONFIG_DATA
 
 
 def test_basic_instantiation(circuits_app):
+    opts = AppConfigManager(mock_constants.MOCK_OPTS)
     mock_cmp = AppFunctionMockComponent(
-        opts=mock_constants.MOCK_OPTS,
+        opts=opts,
         package_name=mock_constants.MOCK_PACKAGE_NAME,
         required_app_configs=mock_constants.MOCK_REQUIRED_APP_CONFIGS)
 
     assert mock_cmp.PACKAGE_NAME == mock_constants.MOCK_PACKAGE_NAME
-    assert mock_cmp.opts == mock_constants.MOCK_OPTS
+    assert mock_cmp.opts == opts
     assert mock_cmp.required_app_configs == mock_constants.MOCK_REQUIRED_APP_CONFIGS
     assert isinstance(mock_cmp.rc, RequestsCommon)
     assert mock_cmp.app_configs.url == "https://www.mockexample.com"
     assert mock_cmp.options == mock_cmp._app_configs_as_dict
 
+def test_basic_instantiation_rc_without_session(circuits_app):
+    opts = AppConfigManager(mock_constants.MOCK_OPTS)
+    opts[constants.APP_CONFIG_RC_USE_PERSISTENT_SESSIONS] = "False"
+    mock_cmp = AppFunctionMockComponent(
+        opts=opts,
+        package_name=mock_constants.MOCK_PACKAGE_NAME,
+        required_app_configs=mock_constants.MOCK_REQUIRED_APP_CONFIGS)
+
+    assert mock_cmp.PACKAGE_NAME == mock_constants.MOCK_PACKAGE_NAME
+    assert mock_cmp.opts == opts
+    assert mock_cmp.required_app_configs == mock_constants.MOCK_REQUIRED_APP_CONFIGS
+    assert isinstance(mock_cmp.rc, RequestsCommonWithoutSession)
+    assert mock_cmp.app_configs.url == "https://www.mockexample.com"
+    assert mock_cmp.options == mock_cmp._app_configs_as_dict
+
 
 def test_status_message(circuits_app):
     mock_msg = u"Custom message with unicode լ խ ծ կ հ ձ ղ ճ"
     mock_cmp = AppFunctionMockComponent(opts=mock_constants.MOCK_OPTS)
     mock_status_message = mock_cmp.status_message(mock_msg)
     assert isinstance(mock_status_message, StatusMessage)
     assert mock_status_message.text == mock_msg
```

### Comparing `resilient_circuits-48.2.4321/tests/test_app_restartable.py` & `resilient_circuits-49.0.4423/tests/test_app_restartable.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_component_loader.py` & `resilient_circuits-49.0.4423/tests/test_component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_decorators.py` & `resilient_circuits-49.0.4423/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_errors.py` & `resilient_circuits-49.0.4423/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_helpers.py` & `resilient_circuits-49.0.4423/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_resilient_circuits_cmd.py` & `resilient_circuits-49.0.4423/tests/test_resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_rest_helper.py` & `resilient_circuits-49.0.4423/tests/test_rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_stomp_component.py` & `resilient_circuits-49.0.4423/tests/test_stomp_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/test_templates.py` & `resilient_circuits-49.0.4423/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tests/util/test_resilient_customize.py` & `resilient_circuits-49.0.4423/tests/util/test_resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.2.4321/tox.ini` & `resilient_circuits-49.0.4423/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     mock
     setuptools-scm<6.0.0 ; python_version=="2.7"
 
 setenv = 
     SETUPTOOLS_SCM_PRETEND_VERSION={env:SETUPTOOLS_SCM_PRETEND_VERSION}
 
 commands = 
+    pip install ../resilient-app-config-plugins
     pip install ../resilient
     pip install ../resilient-lib
     pip install .
     pip install ../pytest-resilient-circuits
     coverage run -m pytest --cov --cov-report xml --capture=no -s {posargs} tests/ --durations=0
 
 [coverage:run]
```

