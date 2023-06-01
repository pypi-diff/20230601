# Comparing `tmp/splight-cli-3.0.0.dev1.tar.gz` & `tmp/splight-cli-3.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-cli-3.0.0.dev1.tar", last modified: Thu Jun  1 15:02:14 2023, max compression
+gzip compressed data, was "splight-cli-3.0.0.dev2.tar", last modified: Thu Jun  1 15:10:55 2023, max compression
```

## Comparing `splight-cli-3.0.0.dev1.tar` & `splight-cli-3.0.0.dev2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.382921 splight-cli-3.0.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-01 15:02:14.382921 splight-cli-3.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.374921 splight-cli-3.0.0.dev1/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.374921 splight-cli-3.0.0.dev1/cli/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/component/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/templates/.splightignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/templates/Initialization
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/templates/auto_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/templates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/templates/spec.json
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/templates/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/component/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/component/tests/test_component_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/context/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/context/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/alert/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/asset/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/attribute/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/file/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/manager/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/engine/setpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/engine/setpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/hub/component/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/hub/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/hub/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/hub/component/hub_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/utils/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/utils/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.378921 splight-cli-3.0.0.dev1/cli/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/cli/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:02:14.382921 splight-cli-3.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:14.382921 splight-cli-3.0.0.dev1/splight_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/splight_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/splight_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/splight_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/splight_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/splight_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 15:02:14.000000 splight-cli-3.0.0.dev1/splight_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.418273 splight-cli-3.0.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-01 15:10:55.418273 splight-cli-3.0.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/component/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/templates/.splightignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/templates/Initialization
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/templates/auto_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/templates/spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/templates/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/component/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/component/tests/test_component_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/context/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17144 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/manager/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/engine/setpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/engine/setpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.414273 splight-cli-3.0.0.dev2/cli/hub/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/hub/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/hub/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/hub/component/hub_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.418273 splight-cli-3.0.0.dev2/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/utils/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/utils/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.418273 splight-cli-3.0.0.dev2/cli/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/cli/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:10:55.418273 splight-cli-3.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-01 15:10:54.000000 splight-cli-3.0.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:55.418273 splight-cli-3.0.0.dev2/splight_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-01 15:10:55.000000 splight-cli-3.0.0.dev2/splight_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-01 15:10:55.000000 splight-cli-3.0.0.dev2/splight_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:10:55.000000 splight-cli-3.0.0.dev2/splight_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 15:10:55.000000 splight-cli-3.0.0.dev2/splight_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 15:10:55.000000 splight-cli-3.0.0.dev2/splight_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 15:10:55.000000 splight-cli-3.0.0.dev2/splight_cli.egg-info/top_level.txt
```

### Comparing `splight-cli-3.0.0.dev1/README.md` & `splight-cli-3.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/cli.py` & `splight-cli-3.0.0.dev2/cli/cli.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/component/__init__.py` & `splight-cli-3.0.0.dev2/cli/component/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
 from pathlib import Path
 from typing import Optional
 
 import typer
-from rich.console import Console
-
 from cli.component.component import ComponentManager
 from cli.constants import error_style, success_style
 from cli.context import check_credentials
+from rich.console import Console
 
 component_app = typer.Typer(
     name="Splight Component",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
```

### Comparing `splight-cli-3.0.0.dev1/cli/component/component.py` & `splight-cli-3.0.0.dev2/cli/component/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 import os
 import subprocess
 from enum import auto
 from pathlib import Path
 from typing import List, Optional
 
 from caseconverter import pascalcase
-from jinja2 import Template
-from rich.console import Console
-from splight_lib.component.spec import Spec
-from strenum import LowercaseStrEnum
-
 from cli.component.exceptions import (
     ComponentExecutionError,
     ComponentTestError,
     ComponentTestFileDoesNotExists,
     InvalidSplightCLIVersion,
     ReadmeExists,
 )
@@ -27,14 +22,18 @@
     PYTHON_TESTS_FILE,
     README_FILE,
     SPEC_FILE,
     SPLIGHT_IGNORE,
 )
 from cli.utils import get_template
 from cli.version import __version__
+from jinja2 import Template
+from rich.console import Console
+from splight_lib.component.spec import Spec
+from strenum import LowercaseStrEnum
 
 console = Console()
 
 
 class AvailableLanguages(LowercaseStrEnum):
     PYTHON = auto()
```

### Comparing `splight-cli-3.0.0.dev1/cli/component/exceptions.py` & `splight-cli-3.0.0.dev2/cli/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/component/loaders.py` & `splight-cli-3.0.0.dev2/cli/component/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import subprocess
 from typing import Dict, List, Optional, Union
 
-from splight_lib.logging._internal import get_splight_logger
-
 from cli.component.spec import Spec
 from cli.constants import INIT_FILE, SPEC_FILE
 from cli.utils import get_json_from_file, input_single
+from splight_lib.logging._internal import get_splight_logger
 
 logger = get_splight_logger()
 Primitive = Union[int, str, float, bool]
 
 
 class SpecLoader:
     _NAME_KEY: str = "name"
```

### Comparing `splight-cli-3.0.0.dev1/cli/component/spec.py` & `splight-cli-3.0.0.dev2/cli/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/component/templates/.splightignore` & `splight-cli-3.0.0.dev2/cli/component/templates/.splightignore`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/component/templates/auto_readme.md` & `splight-cli-3.0.0.dev2/cli/component/templates/auto_readme.md`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/component/templates/main.py` & `splight-cli-3.0.0.dev2/cli/component/templates/main.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/component/templates/spec.json` & `splight-cli-3.0.0.dev2/cli/component/templates/spec.json`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/component/templates/tests.py` & `splight-cli-3.0.0.dev2/cli/component/templates/tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
+from main import {{component_name}}
 
 # component is your component loaded as a pytest fixture
 # using local clients for database, datalake and communication
 from splight_lib.testing import mock_component
 
-from main import {{component_name}}
-
 
 def test_simple_example():
     assert 0 == 0, "The world is bad"
     assert "foo" == "foo", "Run away"
 
 
 def test_using_component():
```

### Comparing `splight-cli-3.0.0.dev1/cli/component/tests/test_component_manager.py` & `splight-cli-3.0.0.dev2/cli/component/tests/test_component_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 from dataclasses import dataclass
 from unittest.mock import call, mock_open, patch
 
 import pytest
-from splight_lib.component.spec import Spec
-
 from cli.component.component import ComponentManager
 from cli.component.exceptions import (
     ComponentExecutionError,
     InvalidSplightCLIVersion,
 )
+from splight_lib.component.spec import Spec
 
 COMPONENT_FILES = [
     "Initialization",
     "README.md",
     "spec.json",
     ".splightignore",
     "tests.py",
```

### Comparing `splight-cli-3.0.0.dev1/cli/config/__init__.py` & `splight-cli-3.0.0.dev2/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/constants.py` & `splight-cli-3.0.0.dev2/cli/constants.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/context/__init__.py` & `splight-cli-3.0.0.dev2/cli/context/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/context/workspace.py` & `splight-cli-3.0.0.dev2/cli/context/workspace.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/engine/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/engine/alert/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/alert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,13 +79,13 @@
 
 @alert_app.command()
 def download(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to download"
     ),
-    path: str = typer.Option(".", help="Path to download file")
+    path: str = typer.Option(".", help="Path to download file"),
 ):
     manager = ResourceManager(
         model=MODEL,
     )
     manager.download(instance_id, path=path)
```

### Comparing `splight-cli-3.0.0.dev1/cli/engine/asset/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/asset/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,13 +79,13 @@
 
 @asset_app.command()
 def download(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to download"
     ),
-    path: str = typer.Option(".", help="Path to download file")
+    path: str = typer.Option(".", help="Path to download file"),
 ):
     manager = ResourceManager(
         model=MODEL,
     )
     manager.download(instance_id, path=path)
```

### Comparing `splight-cli-3.0.0.dev1/cli/engine/attribute/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/attribute/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,13 +79,13 @@
 
 @attribute_app.command()
 def download(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to be removed"
     ),
-    path: str = typer.Option(".", help="Path to download file")
+    path: str = typer.Option(".", help="Path to download file"),
 ):
     manager = ResourceManager(
         model=MODEL,
     )
     manager.download(instance_id, path=path)
```

### Comparing `splight-cli-3.0.0.dev1/cli/engine/component/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/component/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import json
 from typing import List, Optional
 
 import typer
-from rich.console import Console
-from splight_lib.models import Component
-
 from cli.constants import error_style, success_style
 from cli.engine.manager import (
-    ResourceManager,
-    ResourceManagerException,
     ComponentUpgradeManager,
     ComponentUpgradeManagerException,
+    ResourceManager,
+    ResourceManagerException,
 )
-
+from rich.console import Console
+from splight_lib.models import Component
 
 component_app = typer.Typer(
     name="Splight Engine Component",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
@@ -82,17 +80,15 @@
         "--version",
         "-v",
         help="The version of the HubComponent to be upgraded to",
     ),
 ):
     """Upgrade a component to a new version of its HubComponent."""
 
-    manager = ComponentUpgradeManager(
-        component_id=from_component_id
-    )
+    manager = ComponentUpgradeManager(component_id=from_component_id)
 
     try:
         new_component = manager.upgrade(version)
     except ComponentUpgradeManagerException as exc:
         console.print(exc, style=error_style)
         raise typer.Exit(1)
 
@@ -150,13 +146,13 @@
 
 @component_app.command()
 def download(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to download"
     ),
-    path: str = typer.Option(".", help="Path to download file")
+    path: str = typer.Option(".", help="Path to download file"),
 ):
     manager = ResourceManager(
         model=MODEL,
     )
     manager.download(instance_id, path=path)
```

### Comparing `splight-cli-3.0.0.dev1/cli/engine/datalake/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/datalake/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import List
 
 import typer
-from rich.console import Console
-from splight_lib.models import Boolean, Number, String
-
 from cli.constants import error_style
 from cli.engine.manager import DatalakeManager, DatalakeManagerException
+from rich.console import Console
+from splight_lib.models import Boolean, Number, String
 
 datalake_app = typer.Typer(
     name="Splight Engine Datalake",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
```

### Comparing `splight-cli-3.0.0.dev1/cli/engine/file/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/file/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,13 +88,13 @@
 
 @file_app.command()
 def download(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to download"
     ),
-    path: str = typer.Option(".", help="Path to download file")
+    path: str = typer.Option(".", help="Path to download file"),
 ):
     manager = ResourceManager(
         model=MODEL,
     )
     manager.download(instance_id, path=path)
```

### Comparing `splight-cli-3.0.0.dev1/cli/engine/manager/exceptions.py` & `splight-cli-3.0.0.dev2/cli/engine/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/engine/manager/manager.py` & `splight-cli-3.0.0.dev2/cli/engine/manager/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import json
 import os
 import shutil
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Type, Union
 
 import pandas as pd
-from pydantic import BaseModel
-from rich.console import Console
-from rich.table import Table
-from splight_lib.models import Component, ComponentObject, File, HubComponent
-from splight_lib.models.base import (
-    SplightDatabaseBaseModel,
-    SplightDatalakeBaseModel,
-)
-from splight_lib.models.component import InputParameter, Parameter
-
 from cli.component.exceptions import InvalidCSVColumns
 from cli.component.loaders import SpecLoader
 from cli.constants import REQUIRED_DATALAKE_COLUMNS  # error_style,
 from cli.constants import success_style, warning_style
 from cli.engine.manager.exceptions import (
     ComponentCreateError,
     InvalidComponentId,
     UpdateParametersError,
     VersionUpdateError,
 )
 from cli.hub.component.exceptions import HubComponentNotFound
+from pydantic import BaseModel
+from rich.console import Console
+from rich.table import Table
+from splight_lib.models import Component, ComponentObject, File, HubComponent
+from splight_lib.models.base import (
+    SplightDatabaseBaseModel,
+    SplightDatalakeBaseModel,
+)
+from splight_lib.models.component import InputParameter, Parameter
 
 SplightModel = Type[SplightDatabaseBaseModel]
 
 
 class ResourceManagerException(Exception):
     pass
```

### Comparing `splight-cli-3.0.0.dev1/cli/engine/secret/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/secret/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,13 +75,13 @@
 
 @secret_app.command()
 def download(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to be removed"
     ),
-    path: str = typer.Option(".", help="Path to download file")
+    path: str = typer.Option(".", help="Path to download file"),
 ):
     manager = ResourceManager(
         model=MODEL,
     )
     manager.download(instance_id, path=path)
```

### Comparing `splight-cli-3.0.0.dev1/cli/engine/setpoint/__init__.py` & `splight-cli-3.0.0.dev2/cli/engine/setpoint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,13 +66,13 @@
 
 @setpoint_app.command()
 def download(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to download"
     ),
-    path: str = typer.Option(".", help="Path to download file")
+    path: str = typer.Option(".", help="Path to download file"),
 ):
     manager = ResourceManager(
         model=MODEL,
     )
     manager.download(instance_id, path=path)
```

### Comparing `splight-cli-3.0.0.dev1/cli/hub/component/__init__.py` & `splight-cli-3.0.0.dev2/cli/hub/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/hub/component/exceptions.py` & `splight-cli-3.0.0.dev2/cli/hub/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/hub/component/hub_manager.py` & `splight-cli-3.0.0.dev2/cli/hub/component/hub_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import json
 import os
 import shutil
 from typing import Optional
 
 import pathspec
 import py7zr
-from rich.console import Console
-from rich.table import Table
-from splight_lib.models import HubComponent, HubComponentVersion
-
 from cli.component.component import ComponentManager
 from cli.constants import (
     COMPRESSION_TYPE,
     PYTHON_TESTS_FILE,
     SPEC_FILE,
     SPLIGHT_IGNORE,
     success_style,
@@ -21,20 +17,22 @@
     ComponentAlreadyExists,
     ComponentDirectoryAlreadyExists,
     ComponentPullError,
     ComponentPushError,
     HubComponentNotFound,
 )
 from cli.utils.loader import Loader
+from rich.console import Console
+from rich.table import Table
+from splight_lib.models import HubComponent, HubComponentVersion
 
 console = Console()
 
 
 class HubComponentManager:
-
     def push(self, path: str, force: Optional[bool] = False):
         with open(os.path.join(path, SPEC_FILE)) as fid:
             spec = json.load(fid)
 
         name = spec["name"]
         version = spec["version"]
```

### Comparing `splight-cli-3.0.0.dev1/cli/settings.py` & `splight-cli-3.0.0.dev2/cli/settings.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/utils/input.py` & `splight-cli-3.0.0.dev2/cli/utils/input.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/utils/loader.py` & `splight-cli-3.0.0.dev2/cli/utils/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from itertools import cycle
 from shutil import get_terminal_size
 from threading import Thread
 from time import sleep
+from typing import Optional
 
 from colorama import Fore, Style
 
 
-from typing import Optional
-
-
 class Loader:
     def __init__(
         self,
         desc: str = "Loading...",
         end: Optional[str] = None,
         timeout: float = 0.1,
         msg: Optional[str] = None,
```

### Comparing `splight-cli-3.0.0.dev1/cli/utils/pprint.py` & `splight-cli-3.0.0.dev2/cli/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/utils/yaml.py` & `splight-cli-3.0.0.dev2/cli/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/cli/workspace/__init__.py` & `splight-cli-3.0.0.dev2/cli/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/setup.py` & `splight-cli-3.0.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0.dev1/splight_cli.egg-info/SOURCES.txt` & `splight-cli-3.0.0.dev2/splight_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

