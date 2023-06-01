# Comparing `tmp/bomf-0.5.0.tar.gz` & `tmp/bomf-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.5.0.tar", last modified: Thu Jun  1 08:34:53 2023, max compression
+gzip compressed data, was "bomf-0.5.1.tar", last modified: Thu Jun  1 09:52:12 2023, max compression
```

## Comparing `bomf-0.5.0.tar` & `bomf-0.5.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.112548 bomf-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.112548 bomf-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 08:34:43.000000 bomf-0.5.0/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-01 08:34:43.000000 bomf-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-01 08:34:43.000000 bomf-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-01 08:34:43.000000 bomf-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-01 08:34:53.116548 bomf-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-01 08:34:43.000000 bomf-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-01 08:34:43.000000 bomf-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 08:34:43.000000 bomf-0.5.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-01 08:34:43.000000 bomf-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-01 08:34:53.116548 bomf-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 08:34:43.000000 bomf-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.112548 bomf-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.112548 bomf-0.5.0/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-01 08:34:43.000000 bomf-0.5.0/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-01 08:34:53.000000 bomf-0.5.0/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-01 08:34:53.000000 bomf-0.5.0/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:34:53.000000 bomf-0.5.0/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:34:53.000000 bomf-0.5.0/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 08:34:53.000000 bomf-0.5.0/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 08:34:53.000000 bomf-0.5.0/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-01 08:34:43.000000 bomf-0.5.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:34:53.116548 bomf-0.5.0/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-06-01 08:34:43.000000 bomf-0.5.0/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.495468 bomf-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.487468 bomf-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.487468 bomf-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 09:52:04.000000 bomf-0.5.1/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-01 09:52:04.000000 bomf-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-01 09:52:04.000000 bomf-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-01 09:52:04.000000 bomf-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-01 09:52:12.495468 bomf-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-01 09:52:04.000000 bomf-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-01 09:52:04.000000 bomf-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 09:52:04.000000 bomf-0.5.1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-01 09:52:04.000000 bomf-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-01 09:52:12.495468 bomf-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 09:52:04.000000 bomf-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.487468 bomf-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.487468 bomf-0.5.1/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.491468 bomf-0.5.1/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.491468 bomf-0.5.1/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.491468 bomf-0.5.1/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.491468 bomf-0.5.1/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.491468 bomf-0.5.1/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.491468 bomf-0.5.1/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.491468 bomf-0.5.1/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-01 09:52:04.000000 bomf-0.5.1/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.491468 bomf-0.5.1/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-01 09:52:12.000000 bomf-0.5.1/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-01 09:52:12.000000 bomf-0.5.1/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:52:12.000000 bomf-0.5.1/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:52:12.000000 bomf-0.5.1/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 09:52:12.000000 bomf-0.5.1/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 09:52:12.000000 bomf-0.5.1/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-01 09:52:04.000000 bomf-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:52:12.495468 bomf-0.5.1/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-06-01 09:52:04.000000 bomf-0.5.1/unittests/test_validation.py
```

### Comparing `bomf-0.5.0/.github/dependabot.yml` & `bomf-0.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.github/workflows/black.yml` & `bomf-0.5.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.github/workflows/codeql-analysis.yml` & `bomf-0.5.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.github/workflows/coverage.yml` & `bomf-0.5.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.github/workflows/packaging_test.yml` & `bomf-0.5.1/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.github/workflows/python-publish.yml` & `bomf-0.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.github/workflows/pythonlint.yml` & `bomf-0.5.1/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.github/workflows/unittests.yml` & `bomf-0.5.1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.gitignore` & `bomf-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/.pre-commit-config.yaml` & `bomf-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/LICENSE` & `bomf-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/PKG-INFO` & `bomf-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.0
+Version: 0.5.1
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.0/README.md` & `bomf-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/pyproject.toml` & `bomf-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/requirements.txt` & `bomf-0.5.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/setup.cfg` & `bomf-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/__init__.py` & `bomf-0.5.1/src/bomf/provider/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,124 @@
 """
-BOMF stands for BO4E Migration Framework.
+providers provide data
+"""
+import json
+import logging
+from abc import ABC, abstractmethod
+from itertools import groupby
+from pathlib import Path
+from typing import Callable, Generic, Mapping, TypeVar, Union
+
+from bomf import PaginationNotSupportedException
+
+SourceDataModel = TypeVar("SourceDataModel")
+"""
+Source data model is the data model of the source (meaning: the data model of the system from which the data originate).
+"""
+
+KeyTyp = TypeVar("KeyTyp")
+"""
+The type of the key used as "primary key" for the source data model
 """
-import asyncio
-from abc import ABC
-from typing import Generic
-
-import attrs
-
-from bomf.filter import Filter
-from bomf.loader.entityloader import EntityLoader, LoadingSummary
-from bomf.mapper import (
-    Bo4eDataSetToTargetMapper,
-    IntermediateDataSet,
-    PaginationNotSupportedException,
-    SourceToBo4eDataSetMapper,
-    TargetDataModel,
-)
-from bomf.provider import KeyTyp, SourceDataProvider
-from bomf.validation import ValidationManager
 
 
 # pylint:disable=too-few-public-methods
-@attrs.define(kw_only=True, auto_attribs=True)
-class MigrationStrategy(ABC, Generic[IntermediateDataSet, TargetDataModel]):
+class SourceDataProvider(ABC, Generic[SourceDataModel, KeyTyp]):
     """
-    A migration strategy describes the whole migration flow of datasets from a source to a target system
+    A source data provider provides entities from the source data system.
+    The source data provider is thought to encapsulate data access behind a unified interface.
     """
 
-    source_data_to_bo4e_mapper: SourceToBo4eDataSetMapper[IntermediateDataSet]
-    """
-    A mapper that transforms source data models into data sets that consist of bo4e objects
-    """
-    validation: ValidationManager[IntermediateDataSet]
-    """
-    a set of validation rules that are applied to the bo4e data sets
-    """
-    bo4e_to_target_mapper: Bo4eDataSetToTargetMapper[TargetDataModel, IntermediateDataSet]
-    """
-    a mapper that transforms bo4e data sets to a structure that suits the target system
-    """
-    target_loader: EntityLoader[TargetDataModel]
+    @abstractmethod
+    async def get_data(self) -> list[SourceDataModel]:
+        """
+        Returns all available entities from the source data model.
+        They will be filtered in a SourceDataModel Filter ("Preselect")
+        """
+
+    async def get_paginated_data(self, offset: int, limit: int) -> list[SourceDataModel]:
+        """
+        Returns source data models in the range [offset, offset+limit]
+        """
+        # This method is not abstract, meaning: the inheriting classes do not have to implement it.
+        # It raises an error by default which is ok.
+        raise PaginationNotSupportedException(f"The source data provider {self.__class__} does not support pagination")
+
+    @abstractmethod
+    async def get_entry(self, key: KeyTyp) -> SourceDataModel:
+        """
+        returns the source data model which has key as key.
+        raises an error if the key is unknown
+        """
+
+
+class ListBasedSourceDataProvider(SourceDataProvider[SourceDataModel, KeyTyp]):
     """
-    The target loader moves the target entities into the actual target system.
+    A source data provider that is instantiated with a list of source data models
     """
 
-    async def _map_to_target_validate_and_load(self, bo4e_datasets: list[IntermediateDataSet]) -> list[LoadingSummary]:
+    def __init__(self, source_data_models: list[SourceDataModel], key_selector: Callable[[SourceDataModel], KeyTyp]):
         """
-        This method encapsulates the steps:
-        1. validation
-        2. mapping intermediate models to target
-        3. load to target system.
-        They have been encapsulated because they're used by both the migrate and migrate_paginated methods.
+        instantiate it by providing a list of source data models
         """
-        validation_result = await self.validation.validate(*bo4e_datasets)
-        target_data_models = await self.bo4e_to_target_mapper.create_target_models(
-            validation_result.succeeded_data_sets
+        self._models: list[SourceDataModel] = source_data_models
+        logger = logging.getLogger(self.__module__)
+        for key, key_models in groupby(source_data_models, key=key_selector):
+            affected_entries_count = len(list(key_models))
+            if affected_entries_count > 1:
+                logger.warning(
+                    "There are %i>1 entries for the key '%s'. You might miss entries because the key is not unique.",
+                    affected_entries_count,
+                    str(key),
+                )
+        self._models_dict: Mapping[KeyTyp, SourceDataModel] = {key_selector(m): m for m in source_data_models}
+        logging.getLogger(self.__module__).info(
+            "Read %i records from %s", len(self._models_dict), str(source_data_models)
         )
-        loading_summaries = await self.target_loader.load_entities(target_data_models)
-        return loading_summaries
+        self.key_selector = key_selector
+
+    async def get_entry(self, key: KeyTyp) -> SourceDataModel:
+        return self._models_dict[key]
+
+    async def get_data(self) -> list[SourceDataModel]:
+        return self._models
 
-    async def migrate(self) -> list[LoadingSummary]:
+    async def get_paginated_data(self, offset: int, limit: int) -> list[SourceDataModel]:
+        if offset > len(self._models):
+            return []
+        return self._models[offset : offset + limit]
+
+
+class JsonFileSourceDataProvider(SourceDataProvider[SourceDataModel, KeyTyp], Generic[SourceDataModel, KeyTyp]):
+    """
+    a source data model provider that is based on a JSON file
+    """
+
+    def __init__(
+        self,
+        json_file_path: Path,
+        data_selector: Callable[[Union[dict, list]], list[SourceDataModel]],
+        key_selector: Callable[[SourceDataModel], KeyTyp],
+        encoding="utf-8",
+    ):
+        """
+        initialize by providing a filepath to the json file and an accessor that describes the position of the data
+        within the file.
         """
-        run the entire migration flow from source to target which includes:
-        1. create bo4e data source using the source_data_set_to_bo4e_mapper
-        2. checking that all the bo4e data sets obey the validation rules
-        3. mapping from bo4e to the target data model
-        4. loading the target data models into the target system.
-        """
-        # todo: here we should add some logging and statistics stuff
-        bo4e_datasets = await self.source_data_to_bo4e_mapper.create_data_sets()
-        loading_summaries = await self._map_to_target_validate_and_load(bo4e_datasets)
-        return loading_summaries
-
-    async def migrate_paginated(self, chunk_size: int) -> list[LoadingSummary]:
-        """
-        This is similar to migrate, but it loads the data in chunks of chunk_size.
-        Therefore, the source_data_to_bo4e_mapper must support pagination.
-        """
-        offset = 0
-        loading_summaries = []
-        while True:
-            try:
-                bo4e_datasets = await self.source_data_to_bo4e_mapper.create_data_sets(
-                    limit=chunk_size, offset=offset
-                )  # this might raise an PaginationNotSupportedException
-            except TypeError as type_error:
-                error_message = str(type_error)
-                if (
-                    "got an unexpected keyword argument 'limit'" in error_message
-                    or "got an unexpected keyword argument 'offset'" in error_message
-                ):
-                    # this case should be prevented by the type checker already
-                    raise PaginationNotSupportedException() from type_error
-                raise
-            if len(bo4e_datasets) == 0:
-                break
-            chunk_loading_summaries = await self._map_to_target_validate_and_load(bo4e_datasets)
-            loading_summaries.extend(chunk_loading_summaries)
-            await asyncio.sleep(1)  # give the system 1s some time to breathe
-            offset += chunk_size
+        with open(json_file_path, "r", encoding=encoding) as json_file:
+            raw_data = json.load(json_file)
+        self._source_data_models: list[SourceDataModel] = data_selector(raw_data)
+        self._key_to_data_model_mapping: Mapping[KeyTyp, SourceDataModel] = {
+            key_selector(sdm): sdm for sdm in self._source_data_models
+        }
+        self.key_selector = key_selector
+
+    async def get_data(self) -> list[SourceDataModel]:
+        return self._source_data_models
+
+    async def get_paginated_data(self, offset: int, limit: int) -> list[SourceDataModel]:
+        if offset > len(self._source_data_models):
+            return []
+        return self._source_data_models[offset : offset + limit]
 
-        return loading_summaries
+    async def get_entry(self, key: KeyTyp) -> SourceDataModel:
+        return self._key_to_data_model_mapping[key]
```

### Comparing `bomf-0.5.0/src/bomf/filter/__init__.py` & `bomf-0.5.1/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.5.1/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/loader/entityloader.py` & `bomf-0.5.1/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/mapper/__init__.py` & `bomf-0.5.1/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/model/__init__.py` & `bomf-0.5.1/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/core/analysis.py` & `bomf-0.5.1/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/core/errors.py` & `bomf-0.5.1/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/core/execution.py` & `bomf-0.5.1/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/core/types.py` & `bomf-0.5.1/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/core/utils.py` & `bomf-0.5.1/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/core/validator.py` & `bomf-0.5.1/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/path_map.py` & `bomf-0.5.1/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/query_map.py` & `bomf-0.5.1/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf/validation/utils.py` & `bomf-0.5.1/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/src/bomf.egg-info/PKG-INFO` & `bomf-0.5.1/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.0
+Version: 0.5.1
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.0/src/bomf.egg-info/SOURCES.txt` & `bomf-0.5.1/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/tox.ini` & `bomf-0.5.1/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/unittests/test_bo4e_data_set.py` & `bomf-0.5.1/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/unittests/test_entity_loader.py` & `bomf-0.5.1/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/unittests/test_filter.py` & `bomf-0.5.1/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/unittests/test_mapper.py` & `bomf-0.5.1/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/unittests/test_migration.py` & `bomf-0.5.1/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/unittests/test_source_data_provider.py` & `bomf-0.5.1/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.0/unittests/test_validation.py` & `bomf-0.5.1/unittests/test_validation.py`

 * *Files identical despite different names*

