# Comparing `tmp/cliconfig-1.0.0b3.tar.gz` & `tmp/cliconfig-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-1.0.0b3.tar", last modified: Tue May 30 14:52:42 2023, max compression
+gzip compressed data, was "cliconfig-1.0.0b4.tar", last modified: Thu Jun  1 11:59:58 2023, max compression
```

## Comparing `cliconfig-1.0.0b3.tar` & `cliconfig-1.0.0b4.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.669768 cliconfig-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.645768 cliconfig-1.0.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.653768 cliconfig-1.0.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-30 14:52:42.669768 cliconfig-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.653768 cliconfig-1.0.0b3/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26940 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/cliconfig/yaml_tags/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/yaml_tags/_yaml_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.653768 cliconfig-1.0.0b3/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/README_pypi.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/cliconfig.processing_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:52:42.669768 cliconfig-1.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/delete/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/delete/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/delete/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/fallback.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.645768 cliconfig-1.0.0b3/tests/configs/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/integration/test1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test1/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test1/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test1/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/integration/test2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/exp1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/exp2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/exp3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/integration/test2/models/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/models/resnet100.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/models/resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/models/vit_b16.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.665768 cliconfig-1.0.0b3/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/multi_files_with_tags.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.665768 cliconfig-1.0.0b3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.665768 cliconfig-1.0.0b3/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.665768 cliconfig-1.0.0b3/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/processing/test_base_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_ex_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.548691 cliconfig-1.0.0b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.552691 cliconfig-1.0.0b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.552691 cliconfig-1.0.0b4/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30509 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/cliconfig/yaml_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/yaml_tags/_yaml_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.552691 cliconfig-1.0.0b4/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/README_pypi.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/cliconfig.processing_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/delete/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/delete/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/fallback.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.548691 cliconfig-1.0.0b4/tests/configs/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/integration/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test1/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test1/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test1/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/integration/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/exp1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/exp2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/exp3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/integration/test2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/models/resnet100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/models/resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/models/vit_b16.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/multi_files_with_tags.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/processing/test_base_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_ex_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-1.0.0b3/.github/workflows/pipy_deployment.yaml` & `cliconfig-1.0.0b4/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/.github/workflows/pydocstyle.yaml` & `cliconfig-1.0.0b4/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/.github/workflows/pylint.yaml` & `cliconfig-1.0.0b4/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/.github/workflows/tests.yaml` & `cliconfig-1.0.0b4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/.pylintrc` & `cliconfig-1.0.0b4/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/CONTRIBUTING.md` & `cliconfig-1.0.0b4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/LICENSE` & `cliconfig-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/PKG-INFO` & `cliconfig-1.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: cli,config,cliconfig,python,yaml,merge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `cliconfig-1.0.0b3/README.md` & `cliconfig-1.0.0b4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,18 @@
   (except for tuples and sets, which are not handled by YAML) as well as unions
   (using "Union" or "|"), optional values, nested list, and nested dict.
   For instance: `@type:List[Dict[str, int|float]]`.
 * `@select`: This tag select sub-config(s) to keep and delete the other
   sub-configs in the same parent config. The tagged key is not deleted if it is
   in the parent config.
 * `@delete`: This tag deletes the key from the config before merging.
+* `@new`: This tag allows to add new key(s) to the config that are not already
+  present in the default config(s). It can be used for single parameter or a
+  sub-config. Disclaimer: it is preferable to have exhaustive default config(s)
+  instead of abusing this tag for readability and for security concerning typos.
 
 The tags are applied in the following order: `@merge`, `@select`, `@copy`, `@type`
 and then `@delete`.
 
 Please note that the tags serve as triggers for internal processing and will be
 automatically removed from the key after processing.
 
@@ -247,19 +251,19 @@
 which means that modifying or adding keys directly in the additional configs may
 not be possible (because only the merge of default configuration allow adding new keys).
 If you need to modify or add keys within a dictionary, consider enclosing it in a list.
 
 For instance:
 
 ```yaml
---- default.yaml
+# default.yaml
 logging:
   metrics: ['train loss', 'val loss']
   styles: [{'train loss': 'red', 'val loss': 'blue'}]
---- experiment.yaml
+# experiment.yaml
 logging:
   metrics: ['train loss', 'val loss', 'val acc']
   styles: [{'train loss': 'red', 'val loss': 'blue', 'val acc': 'cyan'}]
 ```
 
 ## How to contribute
```

### Comparing `cliconfig-1.0.0b3/cliconfig/__init__.py` & `cliconfig-1.0.0b4/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/base.py` & `cliconfig-1.0.0b4/cliconfig/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/cli_parser.py` & `cliconfig-1.0.0b4/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/config_routines.py` & `cliconfig-1.0.0b4/cliconfig/config_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/dict_routines.py` & `cliconfig-1.0.0b4/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/process_routines.py` & `cliconfig-1.0.0b4/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/processing/_type_parser.py` & `cliconfig-1.0.0b4/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/processing/base.py` & `cliconfig-1.0.0b4/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/processing/builtin.py` & `cliconfig-1.0.0b4/cliconfig/processing/builtin.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,22 +40,24 @@
     almost all of the other processings.
     Pre-merge order: -20.0
 
     Examples
     --------
     .. code-block:: yaml
 
-        --- # config1.yaml
+        # config1.yaml
         a:
           b: 1
           b_path@merge_after: dict2.yaml
-        --- # config2.yaml
+
+        # config2.yaml
         a.b: 2
         c_path@merge_add: config3.yaml
-        --- # config3.yaml
+
+        # config3.yaml
         c: 3
 
     Before merging, the config1 is interpreted as the dict:
 
     ::
 
         {'a': {'b': 2, 'b_path': 'config2.yaml'}, 'c_path': 'config3.yaml', 'c': 3}
@@ -537,19 +539,19 @@
     .. code-block:: yaml
 
         # main.yaml
         1@select@delete: configs.config1
         2@merge_add@delete: config1.yaml
         3@merge_add@delete: config2.yaml
 
-        --- # config1.yaml
+        # config1.yaml
         configs.config1.param: 1
         configs.config1.param2: 2
 
-        --- # config2.yaml
+        # config2.yaml
         configs.config2.param: 3
         configs.config2.param: 4
 
     Here we want to merge two config files and select one sub-config.
     We use the corresponding tags but we don't have a good name for the keys
     and instead of adding a new parameter in the default configuration with
     random names like "1", "2", "3", we use the ``@delete`` tag to delete the
@@ -574,14 +576,102 @@
         keys = list(flat_config.dict.keys())
         for key in keys:
             if is_tag_in(key, "delete"):
                 del flat_config.dict[key]
         return flat_config
 
 
+class ProcessNew(Processing):
+    """Allow new sub-config/parameter absent from default config with tag ``@new``.
+
+    The tagged sub-config/parameter and its value is stored during pre-merge and
+    is deleted to avoid error on merge due to new key. It is then restored on
+    post-merge. Finally, the tag is restored on pre-save for further loading.
+    This processing is applied very late on pre-merge to allow
+    the others processing to be applied before deleting the parameters.
+    The post-merge processing is applied very early to allow the other processing
+    to use this new parameter.
+    Pre-merge order: 30.0
+    Post-merge order: -20.0
+    Pre-save order: 0.0
+
+    Disclaimer: It is preferable to have an exhaustive default configuration instead
+    of abusing this processing to improve the readability and to avoid typos errors
+    in the name of the parameters or their sub-configs.
+
+    Examples
+    --------
+    .. code-block:: yaml
+
+        # default.yaml
+        param1: 1
+
+        # additional.yaml
+        param2@new: 2
+        subconfig@new.subsubconfig:
+            param3: 3
+            param4: 4
+
+    Use default.yaml as default configuration and add additional.yaml as additional
+    configuration via CLI results on the configuration containing param1, param2
+    and the nested config containing param3 and param4.
+    Without the ``@new`` tag, an error is raised because param2 is not present in
+    the default configuration.
+
+    Note
+    ----
+
+        * Tag a subconfig by adding ``@new`` at the end of the key containing
+          the sub-config dict in your yaml file.
+        * When a parameter is added with this processing, it is possible to modify it
+          later via config merge without the tag because the parameter is then present
+          in the current configuration.
+        * If the tagged parameter or sub-config is already present in the current
+          configuration, no error are raised and the value is still updated on
+          post-merge. It may no have influence in practice.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.premerge_order = 30.0
+        self.postmerge_order = -20.0
+        self.new_vals: Dict[str, Any] = {}
+        self.new_vals_backup: Dict[str, Any] = {}
+
+    def premerge(self, flat_config: Config) -> Config:
+        """Pre-merge processing."""
+        keys = list(flat_config.dict.keys())
+        for key in keys:
+            # NOTE: we don't use is_tag_in because we want to look
+            # for tags in the sub-configs too.
+            if "@new@" in key or "@new." in key or key.endswith("@new"):
+                clean_key = clean_all_tags(key)
+                self.new_vals[clean_key] = flat_config.dict[key]
+                self.new_vals_backup[clean_key] = flat_config.dict[key]
+                del flat_config.dict[key]
+        return flat_config
+
+    def postmerge(self, flat_config: Config) -> Config:
+        """Post-merge processing."""
+        flat_config.dict.update(self.new_vals)
+        # Reset the new values to avoid re-adding them later
+        self.new_vals = {}
+        return flat_config
+
+    def presave(self, flat_config: Config) -> Config:
+        """Pre-save processing."""
+        # Restore the tag @new to allow loading the config later by allowing
+        # these new parameters.
+        for key in self.new_vals_backup:
+            if key in flat_config.dict:
+                flat_config.dict[key + "@new"] = self.new_vals_backup[key]
+                del flat_config.dict[key]
+        return flat_config
+
+
 class ProcessCheckTags(Processing):
     """Raise an error if a tag is present in a key after pre-merging processes.
 
     This security processing is always applied after all pre-merge process and
     checks for '@' in the keys. It raises an error if one is found.
     """
 
@@ -636,8 +726,9 @@
         self.list: List[Processing] = [
             ProcessCheckTags(),
             ProcessMerge(),
             ProcessCopy(),
             ProcessTyping(),
             ProcessSelect(),
             ProcessDelete(),
+            ProcessNew(),
         ]
```

### Comparing `cliconfig-1.0.0b3/cliconfig/processing/create.py` & `cliconfig-1.0.0b4/cliconfig/processing/create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/tag_routines.py` & `cliconfig-1.0.0b4/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig/yaml_tags/_yaml_tags.py` & `cliconfig-1.0.0b4/cliconfig/yaml_tags/_yaml_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/cliconfig.egg-info/PKG-INFO` & `cliconfig-1.0.0b4/cliconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: cli,config,cliconfig,python,yaml,merge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `cliconfig-1.0.0b3/cliconfig.egg-info/SOURCES.txt` & `cliconfig-1.0.0b4/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/Makefile` & `cliconfig-1.0.0b4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/README_pypi.rst` & `cliconfig-1.0.0b4/docs/README_pypi.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/_static/logo.png` & `cliconfig-1.0.0b4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/_static/logo_extend.png` & `cliconfig-1.0.0b4/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/cliconfig_api.rst` & `cliconfig-1.0.0b4/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/conf.py` & `cliconfig-1.0.0b4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/edge_cases.md` & `cliconfig-1.0.0b4/docs/edge_cases.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 which means that modifying or adding keys directly in the additional configs may
 not be possible (because only the merge of default configuration allow adding new keys).
 If you need to modify or add keys within a dictionary, consider enclosing it in a list.
 
 For instance:
 
 ```yaml
---- default.yaml
+# default.yaml
 logging:
   metrics: ['train loss', 'val loss']
   styles: [{'train loss': 'red', 'val loss': 'blue'}]
---- experiment.yaml
+
+# experiment.yaml
 logging:
   metrics: ['train loss', 'val loss', 'val acc']
   styles: [{'train loss': 'red', 'val loss': 'blue', 'val acc': 'cyan'}]
 ```
```

### Comparing `cliconfig-1.0.0b3/docs/license.md` & `cliconfig-1.0.0b4/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/make.bat` & `cliconfig-1.0.0b4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/docs/processing.md` & `cliconfig-1.0.0b4/docs/processing.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 (called "processing" to simplify): `premerge`, `postmerge`, `endbuild`, `postload`
 and `presave`. These names correspond to the timing they are applied. Each processing
 have the signature:
 
 ```python
 def premerge(self, flat_config: Config) -> Config:
     ...
+    return flat_config
 ```
 
 Where `Config` is a simple class containing only two attributes (and no methods):
 `dict` that is the configuration dict and `process_list`, the list of processing objects
 (we discuss about this in a section below). Note that it is
 also the class of the object returned by the `make_config` function.
```

### Comparing `cliconfig-1.0.0b3/docs/quickstart.md` & `cliconfig-1.0.0b4/docs/quickstart.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,18 @@
   after each update, even if the tag is no longer present. It supports basic types
   (except for tuples and sets, which are not handled by YAML) as well as unions
   (using "Union" or "|"), optional values, nested list, and nested dict.
   For instance: `@type:List[Dict[str, int|float]]`.
 * `@select`: This tag select sub-config(s) to keep and delete the other
   sub-configs in the same parent config
 * `@delete`: This tag deletes the key from the config before merging.
+* `@new`: This tag allows to add new key(s) to the config that are not already
+  present in the default config(s). It can be used for single parameter or a
+  sub-config. Disclaimer: it is preferable to have exhaustive default config(s)
+  instead of abusing this tag for readability and for security concerning typos.
 
 The tags are applied in the following order: `@merge`, `@select`, `@copy`, `@type`
 and then `@delete`.
 
 Please note that the tags serve as triggers for internal processing and will be
 automatically removed from the key after processing.
```

### Comparing `cliconfig-1.0.0b3/github_actions_utils/pydocstyle_manager.py` & `cliconfig-1.0.0b4/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/github_actions_utils/pylint_manager.py` & `cliconfig-1.0.0b4/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/github_actions_utils/pytest_manager.py` & `cliconfig-1.0.0b4/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-1.0.0b4/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/pre-commit-checks.sh` & `cliconfig-1.0.0b4/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/pyproject.toml` & `cliconfig-1.0.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/configs/integration/test2/default.yaml` & `cliconfig-1.0.0b4/tests/configs/integration/test2/default.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/conftest.py` & `cliconfig-1.0.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/integration/test_inte_multiple_tags.py` & `cliconfig-1.0.0b4/tests/integration/test_inte_multiple_tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     proc_run_id = create_processing_value(
         lambda run_id: run_id if run_id is not None else random.randint(0, 1000000),
         regex="run_id.*",
     )
     config = make_config(
         "tests/configs/integration/test2/default.yaml",
         process_list=[proc_pos_enc_type, proc_optim_type, proc_protect, proc_run_id],
+        add_default_processing=True,
     )
     expected_dict = {
         "project_name": "ImageClassif",
         "models": {
             "archi_name": "models.vit_b16",
             "vit_b16": {
                 "pos_enc_type": "absolute",
@@ -124,14 +125,20 @@
             "n_epochs": 20,
             "optimizer": {
                 "type": "Adam",
                 "lr": 0.001,
                 "momentum": 0,
             },
         },
+        "metadata": {
+            "exp_details": {
+                "goal": "Test multiple processings",
+                "config_folder": "tests/configs/integration/test2",
+            }
+        },
     }
     check.is_instance(config.dict["run_id"], int)
     config_dict = deepcopy(config.dict)
     del config_dict["run_id"]
     check.equal(config_dict, expected_dict)
     save_config(config, "tests/tmp/config.yaml")
     saved_dict = load_dict("tests/tmp/config.yaml")
```

### Comparing `cliconfig-1.0.0b3/tests/unit/processing/test_base_processing.py` & `cliconfig-1.0.0b4/tests/unit/processing/test_base_processing.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/processing/test_builtin.py` & `cliconfig-1.0.0b4/tests/unit/processing/test_builtin.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from cliconfig.dict_routines import flatten
 from cliconfig.processing.builtin import (
     DefaultProcessings,
     ProcessCheckTags,
     ProcessCopy,
     ProcessDelete,
     ProcessMerge,
+    ProcessNew,
     ProcessSelect,
     ProcessTyping,
 )
 
 
 def test_process_merge() -> None:
     """Test ProcessMerge."""
@@ -307,14 +308,59 @@
         },
         [processing],
     )
     config = processing.premerge(config)
     check.equal(config.dict, {})
 
 
+def test_process_new() -> None:
+    """Test ProcessNew."""
+    processing = ProcessNew()
+    flat_dict = {
+        "param1": 1,
+        "config1": {
+            "param2": 2,
+            "subconfig@new": {"param3": 3, "param4": 4},
+        },
+        "config2@new@tag.subconfig.param3": 3,
+        "config3.subconfig@new.param4": 4,
+    }
+    flat_dict = flatten(flat_dict)
+    config = Config(flat_dict, [processing])
+    check.equal(
+        processing.premerge(config).dict,
+        {
+            "param1": 1,
+            "config1.param2": 2,
+        },
+    )
+    check.equal(
+        processing.postmerge(config).dict,
+        {
+            "param1": 1,
+            "config1.param2": 2,
+            "config1.subconfig.param3": 3,
+            "config1.subconfig.param4": 4,
+            "config2.subconfig.param3": 3,
+            "config3.subconfig.param4": 4,
+        },
+    )
+    check.equal(
+        processing.presave(config).dict,
+        {
+            "param1": 1,
+            "config1.param2": 2,
+            "config1.subconfig.param3@new": 3,
+            "config1.subconfig.param4@new": 4,
+            "config2.subconfig.param3@new": 3,
+            "config3.subconfig.param4@new": 4,
+        },
+    )
+
+
 def test_process_check_tags() -> None:
     """Test ProcessCheckTags."""
     processing = ProcessCheckTags()
     flat_dict = {
         "config.param1": 1,
         "param1": 2,
     }
@@ -339,9 +385,10 @@
     for proc in [
         ProcessCheckTags(),
         ProcessMerge(),
         ProcessCopy(),
         ProcessTyping(),
         ProcessDelete(),
         ProcessSelect(),
+        ProcessNew(),
     ]:
         check.is_in(proc, config.process_list)
```

### Comparing `cliconfig-1.0.0b3/tests/unit/processing/test_create.py` & `cliconfig-1.0.0b4/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/processing/test_type_parser.py` & `cliconfig-1.0.0b4/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/test_base_config.py` & `cliconfig-1.0.0b4/tests/unit/test_base_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/test_cli_parser.py` & `cliconfig-1.0.0b4/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/test_config_routines.py` & `cliconfig-1.0.0b4/tests/unit/test_config_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/test_dict_routines.py` & `cliconfig-1.0.0b4/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/test_ex_docs.py` & `cliconfig-1.0.0b4/tests/unit/test_ex_docs.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/test_process_routines.py` & `cliconfig-1.0.0b4/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b3/tests/unit/test_tag_routines.py` & `cliconfig-1.0.0b4/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*

