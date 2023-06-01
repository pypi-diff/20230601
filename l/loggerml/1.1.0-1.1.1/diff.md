# Comparing `tmp/loggerml-1.1.0.tar.gz` & `tmp/loggerml-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-1.1.0.tar", last modified: Sat May  6 01:13:39 2023, max compression
+gzip compressed data, was "loggerml-1.1.1.tar", last modified: Thu Jun  1 15:08:39 2023, max compression
```

## Comparing `loggerml-1.1.0.tar` & `loggerml-1.1.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.973788 loggerml-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-06 01:13:18.000000 loggerml-1.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.953788 loggerml-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.957788 loggerml-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 01:13:18.000000 loggerml-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-06 01:13:18.000000 loggerml-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-06 01:13:18.000000 loggerml-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 01:13:18.000000 loggerml-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-06 01:13:39.973788 loggerml-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-06 01:13:18.000000 loggerml-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-06 01:13:18.000000 loggerml-1.1.0/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.961788 loggerml-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.961788 loggerml-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   234446 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)    45761 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/advanced.png
--rw-r--r--   0 runner    (1001) docker     (123)   501978 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    28005 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/base.png
--rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/no_n_batches.png
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/regex.png
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/contribute.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.965788 loggerml-1.1.0/docs/features/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/features/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/features/no_batches.md
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/features/regex.md
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/features/with_tracker.md
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/logml_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/vs_tqdm.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.965788 loggerml-1.1.0/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.965788 loggerml-1.1.0/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-06 01:13:18.000000 loggerml-1.1.0/licenses_tier/RICH_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.969788 loggerml-1.1.0/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.969788 loggerml-1.1.0/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-06 01:13:18.000000 loggerml-1.1.0/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 01:13:39.000000 loggerml-1.1.0/logml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-05-06 01:13:18.000000 loggerml-1.1.0/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-06 01:13:18.000000 loggerml-1.1.0/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-06 01:13:18.000000 loggerml-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 01:13:18.000000 loggerml-1.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 01:13:18.000000 loggerml-1.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.969788 loggerml-1.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-06 01:13:18.000000 loggerml-1.1.0/scripts/integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-06 01:13:18.000000 loggerml-1.1.0/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:13:39.973788 loggerml-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 01:13:18.000000 loggerml-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.953788 loggerml-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.973788 loggerml-1.1.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_multi_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_two_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.973788 loggerml-1.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.081397 loggerml-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 15:08:21.000000 loggerml-1.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.073397 loggerml-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.077397 loggerml-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 15:08:21.000000 loggerml-1.1.1/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 15:08:21.000000 loggerml-1.1.1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-01 15:08:21.000000 loggerml-1.1.1/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-01 15:08:21.000000 loggerml-1.1.1/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-01 15:08:21.000000 loggerml-1.1.1/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 15:08:21.000000 loggerml-1.1.1/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-01 15:08:21.000000 loggerml-1.1.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 15:08:21.000000 loggerml-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-06-01 15:08:21.000000 loggerml-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-01 15:08:21.000000 loggerml-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 15:08:21.000000 loggerml-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-01 15:08:39.081397 loggerml-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-06-01 15:08:21.000000 loggerml-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-01 15:08:21.000000 loggerml-1.1.1/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.077397 loggerml-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.077397 loggerml-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   234446 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/_static/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    45761 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/_static/advanced.png
+-rw-r--r--   0 runner    (1001) docker     (123)   501978 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/_static/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    28005 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/_static/base.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/_static/no_n_batches.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/_static/regex.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/contribute.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.077397 loggerml-1.1.1/docs/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/features/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/features/no_batches.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/features/regex.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/features/with_tracker.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/logml_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-01 15:08:21.000000 loggerml-1.1.1/docs/vs_tqdm.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.081397 loggerml-1.1.1/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 15:08:21.000000 loggerml-1.1.1/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 15:08:21.000000 loggerml-1.1.1/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 15:08:21.000000 loggerml-1.1.1/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-01 15:08:21.000000 loggerml-1.1.1/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-01 15:08:21.000000 loggerml-1.1.1/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.081397 loggerml-1.1.1/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-01 15:08:21.000000 loggerml-1.1.1/licenses_tier/RICH_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.081397 loggerml-1.1.1/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-01 15:08:39.000000 loggerml-1.1.1/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-01 15:08:39.000000 loggerml-1.1.1/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:08:39.000000 loggerml-1.1.1/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 15:08:39.000000 loggerml-1.1.1/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 15:08:39.000000 loggerml-1.1.1/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.081397 loggerml-1.1.1/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-01 15:08:21.000000 loggerml-1.1.1/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 15:08:38.000000 loggerml-1.1.1/logml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22730 2023-06-01 15:08:21.000000 loggerml-1.1.1/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-01 15:08:21.000000 loggerml-1.1.1/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 15:08:21.000000 loggerml-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-01 15:08:21.000000 loggerml-1.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 15:08:21.000000 loggerml-1.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.081397 loggerml-1.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-01 15:08:21.000000 loggerml-1.1.1/scripts/integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-01 15:08:21.000000 loggerml-1.1.1/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:08:39.081397 loggerml-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 15:08:21.000000 loggerml-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.073397 loggerml-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.081397 loggerml-1.1.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-01 15:08:21.000000 loggerml-1.1.1/tests/integration/inte_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-01 15:08:21.000000 loggerml-1.1.1/tests/integration/inte_multi_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-01 15:08:21.000000 loggerml-1.1.1/tests/integration/inte_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-01 15:08:21.000000 loggerml-1.1.1/tests/integration/inte_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-01 15:08:21.000000 loggerml-1.1.1/tests/integration/inte_two_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:08:39.081397 loggerml-1.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-01 15:08:21.000000 loggerml-1.1.1/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-01 15:08:21.000000 loggerml-1.1.1/tests/unit/test_time_utils.py
```

### Comparing `loggerml-1.1.0/.github/workflows/pipy_deployment.yaml` & `loggerml-1.1.1/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/.github/workflows/pydocstyle.yaml` & `loggerml-1.1.1/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/.github/workflows/pylint.yaml` & `loggerml-1.1.1/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/.github/workflows/tests.yaml` & `loggerml-1.1.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/.pylintrc` & `loggerml-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/CONTRIBUTING.md` & `loggerml-1.1.1/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ## Pull request checklist
 
 Before proposing a PR you must follow some rule:
 
 - Pull requests typically comprise a **single git commit**. In preparing a pull
   request for review, you may need to squash together multiple commits.
 
-- Code should work on Python 3.8-3.10
+- Code should work on Python 3.7-3.10
 
 - Code should respect [PEP8](https://peps.python.org/pep-0008/)
 
 - The format of the docstrings follows [Numpy guidline](https://numpydoc.readthedocs.io/en/latest/format.html)
 
 Before submitting a PR you should run this pipeline:
```

### Comparing `loggerml-1.1.0/LICENSE` & `loggerml-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/PKG-INFO` & `loggerml-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 1.1.0
+Version: 1.1.1
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-1.1.0/README.md` & `loggerml-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,27 @@
 
 ![Alt Text](docs/_static/base.gif)
 
 Note that the expected remaining time of the overall train is displayed as well as
 the one for the epoch. The logger also provides also the possibility to average the
 logged values over an epoch or a full training.
 
+### Save the logs
+
+In Linux you can use `tee` to save the logs in a file and display them in the console.
+However you need to use `unbuffer` to keep the style:
+
+```bash
+unbuffer python main.py --color=auto | tee output.log
+```
+
+See
+[here](https://superuser.com/questions/352697/preserve-colors-while-piping-to-tee)
+for details.
+
 ### Advanced usage
 
 Now you can add a validation logger, customize the logger with your own styles
 and colors, compute the average of some values over batch, add a dynamic
 message at each batch, update the value only every some batches and more!
 
 At initialization you can set default configuration for the logger that will be
```

### Comparing `loggerml-1.1.0/README_pipy.md` & `loggerml-1.1.1/README_pipy.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/Makefile` & `loggerml-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/_static/advanced.gif` & `loggerml-1.1.1/docs/_static/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/_static/advanced.png` & `loggerml-1.1.1/docs/_static/advanced.png`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/_static/base.gif` & `loggerml-1.1.1/docs/_static/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/_static/base.png` & `loggerml-1.1.1/docs/_static/base.png`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/_static/no_n_batches.png` & `loggerml-1.1.1/docs/_static/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/_static/regex.png` & `loggerml-1.1.1/docs/_static/regex.png`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/conf.py` & `loggerml-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/contribute.md` & `loggerml-1.1.1/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/features/no_batches.md` & `loggerml-1.1.1/docs/features/no_batches.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/features/regex.md` & `loggerml-1.1.1/docs/features/regex.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/features/with_tracker.md` & `loggerml-1.1.1/docs/features/with_tracker.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/index.rst` & `loggerml-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/license.md` & `loggerml-1.1.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/make.bat` & `loggerml-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/docs/quickstart.md` & `loggerml-1.1.1/docs/quickstart.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,27 @@
 
 ![Alt Text](_static/base.gif)
 
 Note that the expected remaining time of the overall train is displayed as well as
 the one for the epoch. The logger also provides also the possibility to average the
 logged values over an epoch or a full training.
 
+## Save the logs
+
+In Linux you can use `tee` to save the logs in a file and display them in the console.
+However you need to use `unbuffer` to keep the style:
+
+```bash
+unbuffer python main.py --color=auto | tee output.log
+```
+
+See
+[here](https://superuser.com/questions/352697/preserve-colors-while-piping-to-tee)
+for details.
+
 ## Advanced usage
 
 Now you can add a validation logger, customize the logger with your own styles
 and colors, compute the average of some values over batch, add a dynamic
 message at each batch, update the value only every some batches and more!
 
 At initialization you can set default configuration for the logger that will be
```

### Comparing `loggerml-1.1.0/docs/vs_tqdm.md` & `loggerml-1.1.1/docs/vs_tqdm.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/github_actions_utils/pydocstyle_manager.py` & `loggerml-1.1.1/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/github_actions_utils/pylint_manager.py` & `loggerml-1.1.1/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/github_actions_utils/pytest_manager.py` & `loggerml-1.1.1/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/licenses_tier/RICH_LICENSE` & `loggerml-1.1.1/licenses_tier/RICH_LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/loggerml.egg-info/PKG-INFO` & `loggerml-1.1.1/loggerml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 1.1.0
+Version: 1.1.1
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-1.1.0/loggerml.egg-info/SOURCES.txt` & `loggerml-1.1.1/loggerml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/logml/__init__.py` & `loggerml-1.1.1/logml/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/logml/logger.py` & `loggerml-1.1.1/logml/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,22 +86,22 @@
     def __init__(
         self,
         n_epochs: int,
         n_batches: Optional[int],
         log_interval: Optional[int] = 1,
         name: Optional[str] = None,
         *,
-        styles: Union[Dict, str] = '',
+        styles: Union[Dict, str] = "",
         sizes: Union[Dict, int] = 6,
         average: Optional[List[str]] = None,
         silent: bool = False,
         show_bar: bool = True,
         show_time: bool = True,
         bold_keys: bool = False,
-        name_style: str = '',
+        name_style: str = "",
     ) -> None:
         # Log parameters
         self.silent = silent
         self.name = name
         self.show_bar = show_bar
         self.show_time = show_time
         self.bold_keys = bold_keys
@@ -136,23 +136,23 @@
         self._renderable = None
         self.console = RICH_CONSOLE
         # Table and message infos from the previous log of the same batch
         self._prev_tables_list: List[Table] = []
         self._prev_table_width = 0
         self._prev_row: List[Text] = []
         self._prev_flat_cell = True
-        self._prev_message = ''
+        self._prev_message = ""
         # Force live display to end at exit
         atexit.register(self.stop)
 
     def log(
         self,
         values: Dict[str, VarType],
         *,
-        message: str = '',
+        message: str = "",
         styles: Union[Dict[str, str], str, None] = None,
         sizes: Union[Dict[str, int], int, None] = None,
         average: Optional[List[str]] = None,
     ) -> None:
         """Log the values with style.
 
         Parameters
@@ -227,14 +227,15 @@
             # refresh at log intervals
             or self.current_batch % self.log_interval == 0
             # refresh at first batch
             or self.current_batch == 1
             # refresh at last batch (if n_batches is specified)
             or (self.n_batches and self.current_batch == self.n_batches)
         )
+
         self.live.update(renderable=self._renderable, refresh=refresh)
 
     def tqdm(
         self,
         iterable: Iterable,
         *,
         reset_means: bool = True,
@@ -314,15 +315,15 @@
             self.step += 1
             self.current_batch += 1
         # Reset the previous table info
         self._prev_tables_list = []
         self._prev_table_width = 0
         self._prev_row = []
         self._prev_flat_cell = True
-        self._prev_message = ''
+        self._prev_message = ""
 
     def start_batch(self) -> None:
         """Declare a new batch. Alias for :meth:`new_batch`."""
         self.new_batch()
 
     def detach(self, *, skipline: bool = True) -> None:
         """Stop the live display.
@@ -336,15 +337,15 @@
             at the end of an epoch. Otherwise, the print will be shown above
             the live display.
         """
         if self.console._live is not None:  # pylint: disable=protected-access
             self.console._live.stop()  # pylint: disable=protected-access
             self.console.clear_live()
         if not self.silent and skipline:
-            self.console.print('')
+            self.console.print("")
 
     def stop(self) -> None:
         """Stop the live display.
 
         Stop the live display while keeping the current display visible in
         the terminal. Alias for :meth:`detach` with `skipline=False`.
 
@@ -379,15 +380,15 @@
             auto_refresh=False,
         )
         self._renderable = None
         self._prev_tables_list = []
         self._prev_table_width = 0
         self._prev_row = []
         self._prev_flat_cell = True
-        self._prev_message = ''
+        self._prev_message = ""
 
     def get_vals(self, *, average: Optional[List[str]] = None) -> Dict[str, VarType]:
         """Get the last values called with log, optionally averaged.
 
         Parameters
         ----------
         average : List[str], optional
@@ -435,18 +436,17 @@
         """Update the internal values."""
         if key not in self._counts:
             self._counts[key] = 0
         if key not in self.mean_vals:
             self.mean_vals[key] = 0
         self._counts[key] += 1
         if isinstance(val, (int, float)):
-            mean = (
-                (self.mean_vals[key] * (self._counts[key] - 1) + val)
-                / self._counts[key]
-            )
+            mean = (self.mean_vals[key] * (self._counts[key] - 1) + val) / self._counts[
+                key
+            ]
             self.mean_vals[key] = mean
         self.vals[key] = val
 
     def _build_name(self) -> Text:
         """Build the name of the logger."""
         return Text(text=self.name, style=self.name_style)
 
@@ -478,17 +478,17 @@
         # a bar that cycles every 20 log intervals or every 100 batches
         # if log_interval is None.
         if self.log_interval:
             progress = (self.step // self.log_interval) % 20
             arrow_len = int(54 * progress / 19)
         else:
             arrow_len = int(54 * (self.step % 100) / 99)
-        bar_list = [' '] * 54
+        bar_list = [" "] * 54
         for i in range(3):
-            bar_list[(arrow_len + i) % 54] = '='
+            bar_list[(arrow_len + i) % 54] = "="
         return Text(f"[{''.join(bar_list)}]", overflow="ellipsis")
 
     def _build_time_info(self) -> Text:
         """Build time info text."""
         (delta_glob, delta_epoch, eta_glob, eta_epoch) = get_time_range(
             current_time=time.time(),
             start_glob=self._glob_time,
@@ -497,17 +497,15 @@
             current_batch=self.current_batch,
             n_epochs=self.n_epochs,
             n_batches=self.n_batches,
         )
         delta_glob_str = sec_to_timestr(delta_glob)
         delta_epoch_str = sec_to_timestr(delta_epoch)
         eta_glob_str = sec_to_timestr(eta_glob) if eta_glob is not None else " ? "
-        eta_epoch_str = (
-            sec_to_timestr(eta_epoch) if eta_epoch is not None else " ? "
-        )
+        eta_epoch_str = sec_to_timestr(eta_epoch) if eta_epoch is not None else " ? "
         time_str = (
             f"[global {delta_glob_str} < {eta_glob_str} | "
             f"epoch {delta_epoch_str} < {eta_epoch_str}]"
         )
         return Text(time_str, overflow="ellipsis")
 
     def _build_keys_vals(
@@ -536,15 +534,18 @@
 
         # New table
         tables_list.append(Table(show_header=False, show_edge=False))
 
         for key, val in values.items():
             # Get style, size and average bool
             style = self._get_param(
-                key, styles, self._default_styles, default_value='',
+                key,
+                styles,
+                self._default_styles,
+                default_value="",
             )
             size = self._get_param(key, sizes, self._default_sizes, default_value=6)
             avg = self._get_param(
                 key, average, self._default_average, default_value=False
             )
             # Format value and get average if needed
             if isinstance(val, (int, float)) and not isinstance(val, bool):
@@ -563,17 +564,17 @@
                 table_width = 0
                 row = []
             cell = Text(justify="center")
             # Add key and value on the cell
             key_style = str(style) + " bold" if self.bold_keys else style
             cell.append(str(key), style=key_style)
             if flat_cell:
-                cell.append(': ' + str(val), style=style)
+                cell.append(": " + str(val), style=style)
             else:
-                cell.append('\n' + str(val), style=style)
+                cell.append("\n" + str(val), style=style)
             row.append(cell)
             table_width += cell_width
         # Add the last row
         tables_list[-1].add_row(*row)
         # Store the tables, last row and its width for the next log of the same batch
         self._prev_tables_list = tables_list
         self._prev_table_width = table_width
@@ -607,15 +608,15 @@
     def _build_message(self, message: str) -> Text:
         """Build message."""
         if not message and self._prev_message:
             # No current message but previous message => keep previous message
             message = self._prev_message
         else:
             self._prev_message = message
-        return Text(message, justify='left')
+        return Text(message, justify="left")
 
 
 def _regex_looking(key: str, config: DictVarType) -> Optional[VarType]:
     """Look on config (dict) for pattern matching and return the value."""
     if key in config:
         return config[key]
     val = None
```

### Comparing `loggerml-1.1.0/logml/time_utils.py` & `loggerml-1.1.1/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/pyproject.toml` & `loggerml-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/scripts/pre-commit-checks.sh` & `loggerml-1.1.1/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/tests/integration/inte_logger.py` & `loggerml-1.1.1/tests/integration/inte_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 logger.new_batch()
                 time.sleep(0.015)
                 styles = {"train loss": "green", "train acc": "blue"}
                 logger.log(
                     {
                         "train loss": 1 - epoch / n_epochs,
                         "train acc": 100 * batch / n_batches,
-                        "loss name": 'mse',
+                        "loss name": "mse",
                         "best run": True,
                     },
                     message="This is...\nok?",
                     styles=styles,
                     average=["mse"],
                 )
         if i == 0:
```

### Comparing `loggerml-1.1.0/tests/integration/inte_multi_logs.py` & `loggerml-1.1.1/tests/integration/inte_multi_logs.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 
 def main() -> None:
     """Integration test for multi logs on same step."""
     logger = Logger(1, 1)
     logger.new_epoch()
     logger.new_batch()
-    logger.log({'loss1': 0.1}, styles='blue', message='ERROR')
-    logger.log({'loss2': 0.2}, styles='red', message='Good')
-    logger.log({'loss3': 0.3}, styles='yellow')
-    logger.log({'loss4': 0.4}, styles='green')
-    logger.log({'loss5': 0.5}, styles='blue')
-    logger.log({'loss6': 0.6}, styles='red')
-    logger.log({'loss7': 0.7}, styles='yellow')
-    logger.log({'loss8': 0.8}, styles='green')
-    logger.log({'loss9': 0.9}, styles='blue')
-    logger.log({'loss10': 1.0}, styles='red')
-    logger.log({'loss11': 1.1}, styles='yellow')
-    logger.log({'loss12': 1.2}, styles='green')
-    logger.log({'loss13': 1.3}, styles='blue')
-    logger.log({'loss14': 1.4}, styles='red')
+    logger.log({"loss1": 0.1}, styles="blue", message="ERROR")
+    logger.log({"loss2": 0.2}, styles="red", message="Good")
+    logger.log({"loss3": 0.3}, styles="yellow")
+    logger.log({"loss4": 0.4}, styles="green")
+    logger.log({"loss5": 0.5}, styles="blue")
+    logger.log({"loss6": 0.6}, styles="red")
+    logger.log({"loss7": 0.7}, styles="yellow")
+    logger.log({"loss8": 0.8}, styles="green")
+    logger.log({"loss9": 0.9}, styles="blue")
+    logger.log({"loss10": 1.0}, styles="red")
+    logger.log({"loss11": 1.1}, styles="yellow")
+    logger.log({"loss12": 1.2}, styles="green")
+    logger.log({"loss13": 1.3}, styles="blue")
+    logger.log({"loss14": 1.4}, styles="red")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `loggerml-1.1.0/tests/integration/inte_regex.py` & `loggerml-1.1.1/tests/integration/inte_regex.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         for _ in logger.tqdm(range(1)):
             logger.log(
                 {
                     "interm loss": 0.04,
                     "train loss": 0.01,
                     "train acc": 56,
                     "val loss": 0.02,
-                    "val acc": 52
+                    "val acc": 52,
                 },
-                styles={"val.*": "yellow", "val acc": "orange3"}
+                styles={"val.*": "yellow", "val acc": "orange3"},
             )
     print("Should be red, blue, green, yellow and orange.")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `loggerml-1.1.0/tests/integration/inte_two_loggers.py` & `loggerml-1.1.1/tests/integration/inte_two_loggers.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.1.0/tests/unit/test_logger.py` & `loggerml-1.1.1/tests/unit/test_logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Test logger.py."""
-
 import pytest
 import pytest_check as check
 
 from logml.logger import Logger
 
 
 def test_logger() -> None:
@@ -28,15 +27,15 @@
             for batch in range(n_batches):
                 logger.start_batch()
                 styles = {"train loss": "green", "train acc": "blue"}
                 logger.log(
                     {
                         "train loss": 1 - int(100 * epoch / n_epochs) / 100,
                         "train acc": 100 - int(100 * batch / n_batches) / 100,
-                        "loss name": 'mse',
+                        "loss name": "mse",
                         "best run": True,
                     },
                     message="This is...\nok?",
                     styles=styles,
                     average=["mse"],
                 )
                 logger.log({"additional loss": 0.05})
@@ -63,66 +62,66 @@
         logger = Logger(2, 5)
         logger.new_batch()
         logger.log({"train loss": 1, "train acc": 1})
 
 
 def test_internal_values() -> None:
     """Test for internal values update."""
-    logger = Logger(n_epochs=3, n_batches=2, average=['val2'])
+    logger = Logger(n_epochs=3, n_batches=2, average=["val2"])
     logger.new_epoch()
     logger.new_batch()
-    logger.log({'val1': 1.0, 'val2': 2.0})
-    check.equal((logger.vals['val1'], logger.vals['val2']), (1.0, 2.0))
-    check.equal((logger.mean_vals['val1'], logger.mean_vals['val2']), (1.0, 2.0))
+    logger.log({"val1": 1.0, "val2": 2.0})
+    check.equal((logger.vals["val1"], logger.vals["val2"]), (1.0, 2.0))
+    check.equal((logger.mean_vals["val1"], logger.mean_vals["val2"]), (1.0, 2.0))
     logger.new_batch()
-    logger.log({'val1': 0.5, 'val2': 1.0})
-    check.equal((logger.vals['val1'], logger.vals['val2']), (0.5, 1.0))
-    check.equal((logger.mean_vals['val1'], logger.mean_vals['val2']), (0.75, 1.5))
+    logger.log({"val1": 0.5, "val2": 1.0})
+    check.equal((logger.vals["val1"], logger.vals["val2"]), (0.5, 1.0))
+    check.equal((logger.mean_vals["val1"], logger.mean_vals["val2"]), (0.75, 1.5))
     logger.new_epoch()
-    check.equal((logger.vals['val1'], logger.vals['val2']), (0.5, 1.0))
-    check.equal((logger.mean_vals['val1'], logger.mean_vals['val2']), (0, 0))
+    check.equal((logger.vals["val1"], logger.vals["val2"]), (0.5, 1.0))
+    check.equal((logger.mean_vals["val1"], logger.mean_vals["val2"]), (0, 0))
     logger.new_batch()
-    logger.log({'val1': 2.0, 'val2': 1.0})
-    check.equal((logger.vals['val1'], logger.vals['val2']), (2.0, 1.0))
-    check.equal((logger.mean_vals['val1'], logger.mean_vals['val2']), (2.0, 1.0))
+    logger.log({"val1": 2.0, "val2": 1.0})
+    check.equal((logger.vals["val1"], logger.vals["val2"]), (2.0, 1.0))
+    check.equal((logger.mean_vals["val1"], logger.mean_vals["val2"]), (2.0, 1.0))
     logger.new_epoch(reset_means=False)
     logger.new_batch()
-    logger.log({'val1': 1.0, 'val2': 2.0})
-    check.equal((logger.mean_vals['val1'], logger.mean_vals['val2']), (1.5, 1.5))
+    logger.log({"val1": 1.0, "val2": 2.0})
+    check.equal((logger.mean_vals["val1"], logger.mean_vals["val2"]), (1.5, 1.5))
     # Test get_vals
-    check.equal(logger.get_vals(average=['val2']), {'val1': 1.0, 'val2': 1.5})
-    check.equal(logger.get_vals(), {'val1': 1.0, 'val2': 2.0})
-    check.equal(logger.get_vals(average=['val.*']), {'val1': 1.5, 'val2': 1.5})
+    check.equal(logger.get_vals(average=["val2"]), {"val1": 1.0, "val2": 1.5})
+    check.equal(logger.get_vals(), {"val1": 1.0, "val2": 2.0})
+    check.equal(logger.get_vals(average=["val.*"]), {"val1": 1.5, "val2": 1.5})
 
     logger.stop()
 
 
 def test_silent(capsys: pytest.CaptureFixture) -> None:
     """Test silent logger."""
     captured = capsys.readouterr()
-    logger = Logger(5, 5, name='Test', silent=True)
+    logger = Logger(5, 5, name="Test", silent=True)
     for _ in range(5):
         logger.new_epoch()
         for _ in range(5):
             logger.new_batch()
-            logger.log({'loss': 0.02})
+            logger.log({"loss": 0.02})
     captured = capsys.readouterr()
-    check.equal(captured.out, '')
+    check.equal(captured.out, "")
 
 
 def test_tqdm() -> None:
     """Test tqdm method."""
     n_epochs = 10
     n_batches = 10
     logger = Logger(n_epochs=n_epochs, n_batches=n_batches)
     for _ in range(10):
         logger.new_epoch()  # Should be avoided but should not raise error
         for _ in logger.tqdm(range(10)):
             logger.new_batch()  # Should be avoided but should not raise error
-            logger.log({'loss': 0.02})
+            logger.log({"loss": 0.02})
     logger = Logger(n_epochs=1, n_batches=None)
     for _ in range(1):
         for _ in logger.tqdm(range(10)):
             pass
     check.equal(logger.n_batches, 10)
 
 
@@ -132,15 +131,10 @@
         n_epochs=10,
         n_batches=10,
         styles={".* loss": "red", "train loss": "blue", ".* acc": "green"},
     )
     for _ in range(10):
         for _ in logger.tqdm(range(10)):
             logger.log(
-                {
-                    "val loss": 0.02,
-                    "train loss": 0.01,
-                    "train acc": 56,
-                    "val acc": 52
-                },
-                styles={"val.*": "yellow", "val acc": "blue"}
+                {"val loss": 0.02, "train loss": 0.01, "train acc": 56, "val acc": 52},
+                styles={"val.*": "yellow", "val acc": "blue"},
             )
```

### Comparing `loggerml-1.1.0/tests/unit/test_time_utils.py` & `loggerml-1.1.1/tests/unit/test_time_utils.py`

 * *Files identical despite different names*

