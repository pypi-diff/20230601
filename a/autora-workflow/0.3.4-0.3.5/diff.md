# Comparing `tmp/autora-workflow-0.3.4.tar.gz` & `tmp/autora-workflow-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.3.4.tar", last modified: Wed May 24 21:14:09 2023, max compression
+gzip compressed data, was "autora-workflow-0.3.5.tar", last modified: Thu Jun  1 20:29:07 2023, max compression
```

## Comparing `autora-workflow-0.3.4.tar` & `autora-workflow-0.3.5.tar`

### file list

```diff
@@ -1,107 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/docs/cli/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)   249249 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/cli/basic-usage/README.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/cli/basic-usage/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/docs/cli/with-cylc/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/cli/with-cylc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/docs/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/accessing-state-dependent-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/passing-static-parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    57339 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/saving-and-loading-dill.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/using-alternative-planners-and-executors.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-conda/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/examples/cylc-conda/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-conda/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/lib/python/dump_initial_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-pip/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/examples/cylc-pip/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-pip/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/lib/python/dump_initial_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-slurm-pip/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/python/dump_initial_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.200160 autora-workflow-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.168159 autora-workflow-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.176159 autora-workflow-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.180159 autora-workflow-0.3.5/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/autora-workflow.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.180159 autora-workflow-0.3.5/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.180159 autora-workflow-0.3.5/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.180159 autora-workflow-0.3.5/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.184160 autora-workflow-0.3.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-01 20:29:07.200160 autora-workflow-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.184160 autora-workflow-0.3.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.168159 autora-workflow-0.3.5/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.184160 autora-workflow-0.3.5/docs/cli/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)   249249 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/cli/basic-usage/README.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/cli/basic-usage/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.184160 autora-workflow-0.3.5/docs/cli/with-cylc/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/cli/with-cylc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.188160 autora-workflow-0.3.5/docs/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/interactive/accessing-state-dependent-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/interactive/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/interactive/passing-static-parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45729 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/interactive/saving-and-loading-dill.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/interactive/using-alternative-planners-and-executors.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.188160 autora-workflow-0.3.5/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.172159 autora-workflow-0.3.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.188160 autora-workflow-0.3.5/examples/cylc-conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-conda/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-conda/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-conda/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.172159 autora-workflow-0.3.5/examples/cylc-conda/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.188160 autora-workflow-0.3.5/examples/cylc-conda/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-conda/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-conda/lib/python/dump_initial_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.188160 autora-workflow-0.3.5/examples/cylc-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-pip/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-pip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-pip/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.172159 autora-workflow-0.3.5/examples/cylc-pip/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.192160 autora-workflow-0.3.5/examples/cylc-pip/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-pip/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-pip/lib/python/dump_initial_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-pip/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.192160 autora-workflow-0.3.5/examples/cylc-slurm-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-slurm-pip/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-slurm-pip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-slurm-pip/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-slurm-pip/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.172159 autora-workflow-0.3.5/examples/cylc-slurm-pip/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.192160 autora-workflow-0.3.5/examples/cylc-slurm-pip/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-slurm-pip/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-slurm-pip/lib/python/dump_initial_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/examples/cylc-slurm-pip/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.192160 autora-workflow-0.3.5/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:29:07.200160 autora-workflow-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.176159 autora-workflow-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.172159 autora-workflow-0.3.5/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.196160 autora-workflow-0.3.5/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.196160 autora-workflow-0.3.5/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.196160 autora-workflow-0.3.5/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.200160 autora-workflow-0.3.5/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-01 20:29:07.000000 autora-workflow-0.3.5/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-01 20:29:07.000000 autora-workflow-0.3.5/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:29:07.000000 autora-workflow-0.3.5/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 20:29:07.000000 autora-workflow-0.3.5/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 20:29:07.000000 autora-workflow-0.3.5/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:29:07.200160 autora-workflow-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-06-01 20:28:54.000000 autora-workflow-0.3.5/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.3.4/.github/workflows/python-publish.yml` & `autora-workflow-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/.github/workflows/test-pytest.yml` & `autora-workflow-0.3.5/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/.gitignore` & `autora-workflow-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/.idea/autora-workflow.iml` & `autora-workflow-0.3.5/.idea/autora-workflow.iml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/.idea/inspectionProfiles/Project_Default.xml` & `autora-workflow-0.3.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/.idea/runConfigurations/pytest_in_tests.xml` & `autora-workflow-0.3.5/.idea/runConfigurations/pytest_in_tests.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/.pre-commit-config.yaml` & `autora-workflow-0.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/LICENSE.md` & `autora-workflow-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/PKG-INFO` & `autora-workflow-0.3.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.4
+Version: 0.3.5
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: cylc
 License-File: LICENSE.md
 
-# AutoRA Workflow
+# Workflow
 
 Workflow management tools for AutoRA.
 
 ## Quickstart Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
 Workflow is a part of the `autora` package:
 
 ```shell
-pip install -U "autora" --pre
+pip install -U "autora"
 ```
 
 !!! success
     It is recommended to use a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
```

### Comparing `autora-workflow-0.3.4/docs/cli/basic-usage/README.ipynb` & `autora-workflow-0.3.5/docs/cli/basic-usage/README.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/docs/cli/basic-usage/lib.py` & `autora-workflow-0.3.5/docs/cli/basic-usage/lib.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/docs/interactive/accessing-state-dependent-properties.ipynb` & `autora-workflow-0.3.5/docs/interactive/accessing-state-dependent-properties.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/docs/interactive/basic-usage.ipynb` & `autora-workflow-0.3.5/docs/interactive/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/docs/interactive/passing-static-parameters.ipynb` & `autora-workflow-0.3.5/docs/interactive/passing-static-parameters.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/docs/interactive/using-alternative-planners-and-executors.ipynb` & `autora-workflow-0.3.5/docs/interactive/using-alternative-planners-and-executors.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/examples/cylc-conda/README.md` & `autora-workflow-0.3.5/examples/cylc-conda/README.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/examples/cylc-conda/flow.cylc` & `autora-workflow-0.3.5/examples/cylc-conda/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/examples/cylc-conda/lib/python/controller_setup.py` & `autora-workflow-0.3.5/examples/cylc-conda/lib/python/controller_setup.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/examples/cylc-pip/README.md` & `autora-workflow-0.3.5/examples/cylc-pip/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Usage with Cylc workflow manager and conda
+# Usage with Cylc workflow manager and pip
 
 The command line interface can be used with workflow managers like cylc in virtualenv environments.
 
 ## Prerequisites
 
 This example requires:
```

### Comparing `autora-workflow-0.3.4/examples/cylc-pip/flow.cylc` & `autora-workflow-0.3.5/examples/cylc-pip/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/examples/cylc-pip/lib/python/controller_setup.py` & `autora-workflow-0.3.5/examples/cylc-pip/lib/python/controller_setup.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/examples/cylc-slurm-pip/README.md` & `autora-workflow-0.3.5/examples/cylc-slurm-pip/README.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/examples/cylc-slurm-pip/flow.cylc` & `autora-workflow-0.3.5/examples/cylc-slurm-pip/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/python/controller_setup.py` & `autora-workflow-0.3.5/examples/cylc-slurm-pip/lib/python/controller_setup.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/mkdocs/base.yml` & `autora-workflow-0.3.5/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/mkdocs.yml` & `autora-workflow-0.3.5/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 nav:
 - Introduction: 'index.md'
 - Interactive:
     - 'interactive/basic-usage.ipynb'
     - 'interactive/passing-static-parameters.ipynb'
     - "interactive/accessing-state-dependent-properties.ipynb"
     - "interactive/using-alternative-planners-and-executors.ipynb"
-    - "interactive/saving-and-loading-dill.ipynb"
+    - "Saving and loading with dill": "interactive/saving-and-loading-dill.ipynb"
 - Command line:
     - "Basic Usage": "cli/basic-usage/README.ipynb"
     - "Using Cylc": "cli/with-cylc/README.md"
```

### Comparing `autora-workflow-0.3.4/pyproject.toml` & `autora-workflow-0.3.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 dynamic = ["version"]
 
 readme = "docs/index.md"
 license = { text = "MIT License" }
 
 dependencies = [
     "autora-core",
+    "scikit-learn",
+    "matplotlib",
+    "pandas",
     "typer[all]",
     "dill",
 ]
 
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]",
     "autora-workflow[docs]",
 ]
 docs = [
-    "mkdocs-include-markdown-plugin",
+    "autora-core[docs]"
 ]
 cylc = [
     "cylc-flow",
     "cylc-uiserver"
 ]
 
 [project.urls]
```

### Comparing `autora-workflow-0.3.4/src/autora/workflow/__init__.py` & `autora-workflow-0.3.5/src/autora/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/__main__.py` & `autora-workflow-0.3.5/src/autora/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/base.py` & `autora-workflow-0.3.5/src/autora/workflow/base.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/controller.py` & `autora-workflow-0.3.5/src/autora/workflow/controller.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/cycle.py` & `autora-workflow-0.3.5/src/autora/workflow/cycle.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/executor.py` & `autora-workflow-0.3.5/src/autora/workflow/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def _executor_experimentalist(state: SupportsControllerState, params: Dict):
         params_ = resolve_state_params(params, state)
         new_conditions = pipeline(**params_)
 
         if isinstance(new_conditions, pd.DataFrame):
             new_conditions_array = new_conditions
         elif isinstance(new_conditions, np.ndarray):
-            _logger.warning(
+            _logger.debug(
                 f"{new_conditions=} is an ndarray, so variable confusion is a possibility"
             )
             new_conditions_array = new_conditions
         elif isinstance(new_conditions, np.recarray):
             new_conditions_array = new_conditions
         elif isinstance(new_conditions, Iterable):
             # If the pipeline gives us an iterable, we need to make it into a concrete array.
```

### Comparing `autora-workflow-0.3.4/src/autora/workflow/planner.py` & `autora-workflow-0.3.5/src/autora/workflow/planner.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/plotting.py` & `autora-workflow-0.3.5/src/autora/workflow/plotting.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/protocol.py` & `autora-workflow-0.3.5/src/autora/workflow/protocol.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.3.5/src/autora/workflow/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/state/history.py` & `autora-workflow-0.3.5/src/autora/workflow/state/history.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/state/param.py` & `autora-workflow-0.3.5/src/autora/workflow/state/param.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora/workflow/state/snapshot.py` & `autora-workflow-0.3.5/src/autora/workflow/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.4/src/autora_workflow.egg-info/PKG-INFO` & `autora-workflow-0.3.5/src/autora_workflow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.4
+Version: 0.3.5
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: cylc
 License-File: LICENSE.md
 
-# AutoRA Workflow
+# Workflow
 
 Workflow management tools for AutoRA.
 
 ## Quickstart Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
 Workflow is a part of the `autora` package:
 
 ```shell
-pip install -U "autora" --pre
+pip install -U "autora"
 ```
 
 !!! success
     It is recommended to use a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
```

### Comparing `autora-workflow-0.3.4/src/autora_workflow.egg-info/SOURCES.txt` & `autora-workflow-0.3.5/src/autora_workflow.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/cli/basic-usage/lib.py
 docs/cli/with-cylc/README.md
 docs/interactive/accessing-state-dependent-properties.ipynb
 docs/interactive/basic-usage.ipynb
 docs/interactive/passing-static-parameters.ipynb
 docs/interactive/saving-and-loading-dill.ipynb
 docs/interactive/using-alternative-planners-and-executors.ipynb
+docs/javascripts/mathjax.js
 examples/cylc-conda/.gitignore
 examples/cylc-conda/README.md
 examples/cylc-conda/environment.yml
 examples/cylc-conda/flow.cylc
 examples/cylc-conda/lib/python/controller_setup.py
 examples/cylc-conda/lib/python/dump_initial_controller.py
 examples/cylc-pip/.gitignore
```

### Comparing `autora-workflow-0.3.4/tests/test_controller_plots.py` & `autora-workflow-0.3.5/tests/test_controller_plots.py`

 * *Files identical despite different names*

