# Comparing `tmp/pydantic-kedro-0.4.0.tar.gz` & `tmp/pydantic-kedro-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-kedro-0.4.0.tar", last modified: Thu May 11 00:23:30 2023, max compression
+gzip compressed data, was "pydantic-kedro-0.5.0.tar", last modified: Thu Jun  1 20:15:27 2023, max compression
```

## Comparing `pydantic-kedro-0.4.0.tar` & `pydantic-kedro-0.5.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.078284 pydantic-kedro-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.078284 pydantic-kedro-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.078284 pydantic-kedro-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/arbitrary_types.md
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/standalone_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.074284 pydantic-kedro-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/pydantic_kedro/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/_internals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-11 00:23:29.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-11 00:23:30.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:23:29.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:22:28.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 00:23:29.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 00:23:29.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/test/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.078284 pydantic-kedro-0.4.0/src/test/catalogs/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/test/catalogs/conf/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/conf/base/catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/src/test/catalogs/conf/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/conf/local/credentials.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/src/test/catalogs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/data/tst1.json
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/test_basic_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_docs_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_ds_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_ds_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_ds_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/arbitrary_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/docs/standalone_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.915988 pydantic-kedro-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/src/pydantic_kedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/_dict_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/_internals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/pydantic_kedro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:14:38.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 20:15:27.000000 pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.919988 pydantic-kedro-0.5.0/src/test/catalogs/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/catalogs/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/conf/base/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/catalogs/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/conf/local/credentials.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:15:27.923988 pydantic-kedro-0.5.0/src/test/catalogs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/data/tst1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/catalogs/test_basic_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_docs_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_ds_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_ds_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_ds_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_nested_subtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 20:14:26.000000 pydantic-kedro-0.5.0/src/test/test_utils.py
```

### Comparing `pydantic-kedro-0.4.0/.github/dependabot.yml` & `pydantic-kedro-0.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/.github/workflows/python-publish.yml` & `pydantic-kedro-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/.github/workflows/python-testing.yml` & `pydantic-kedro-0.5.0/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/.pre-commit-config.yaml` & `pydantic-kedro-0.5.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     rev: "23.3.0"
     hooks:
       - id: black
     # consider also black-jupyter
   - repo: https://github.com/pre-commit/mirrors-mypy
     # NOTE: This passes ALL files to `mypy`. mypy will cache these.
     # However, we must ignore all missing imports, because pre-commit runs in a separate env
-    rev: "v1.2.0"
+    rev: "v1.3.0"
     hooks:
       - id: mypy
         pass_filenames: false
         args: [--config-file, pyproject.toml, --ignore-missing-imports]
   - repo: https://github.com/DavidAnson/markdownlint-cli2
     rev: v0.7.0
     hooks:
```

### Comparing `pydantic-kedro-0.4.0/LICENSE` & `pydantic-kedro-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/PKG-INFO` & `pydantic-kedro-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.4.0
+Version: 0.5.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.4.0/README.md` & `pydantic-kedro-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/docs/arbitrary_types.md` & `pydantic-kedro-0.5.0/docs/arbitrary_types.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/docs/implementation_details.md` & `pydantic-kedro-0.5.0/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/docs/index.md` & `pydantic-kedro-0.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/docs/standalone_usage.md` & `pydantic-kedro-0.5.0/docs/standalone_usage.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/mkdocs.yml` & `pydantic-kedro-0.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/pyproject.toml` & `pydantic-kedro-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 ]
 urls = { github = "https://github.com/NowanIlfideme/pydantic-kedro" }
 
 [project.optional-dependencies]
 dev = [
     "setuptools>=61.0.0",
     "setuptools-scm[toml]>=6.2",
-    "pre-commit==3.3.1",
+    "pre-commit==3.3.2",
     "black==23.3.0",
     "isort==5.12.0",
-    "ruff==0.0.265",
-    "mypy==1.2.0",
+    "ruff==0.0.270",
+    "mypy==1.3.0",
     "pytest==7.3.1",
     # required for testing
     "kedro[pandas]",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
@@ -102,9 +102,16 @@
 exclude = "src/test"
 
 [[tool.mypy.overrides]]
 module = ["pydantic_kedro.*"]
 disallow_untyped_defs = true
 
 [[tool.mypy.overrides]]
-module = ["setuptools", "setuptools_scm", "fsspec.*", "cloudpickle", "fusepy"]
+module = [
+    "setuptools",
+    "setuptools_scm",
+    "fsspec.*",
+    "cloudpickle",
+    "fusepy",
+    "ruamel.yaml",
+]
 ignore_missing_imports = true
```

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro/__init__.py` & `pydantic-kedro-0.5.0/src/pydantic_kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/auto.py` & `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/auto.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/folder.py` & `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 
 import fsspec
 from fsspec import AbstractFileSystem
 from fsspec.core import strip_protocol
 from fsspec.implementations.local import LocalFileSystem
 from kedro.io.core import AbstractDataSet, parse_dataset_definition
 from pydantic import BaseConfig, BaseModel, Extra, Field
-from pydantic.utils import import_string
 
-from pydantic_kedro._internals import get_kedro_default, get_kedro_map
+from pydantic_kedro._dict_io import PatchPydanticIter, dict_to_model
+from pydantic_kedro._internals import get_kedro_default, get_kedro_map, import_string
 
 __all__ = ["PydanticFolderDataSet"]
 
 
 DATA_PLACEHOLDER = "__DATA_PLACEHOLDER__"
 
 JsonPath = str  # not a "real" JSON Path, but just `.`-separated
+ImportStr = str
 
 logger = logging.getLogger(__name__)
 
 # Some ridiculous types to support nested configurations
 _Bis = Union[bool, int, str, Path, None]
 _Dis1 = Dict[str, _Bis]
 _Dis2 = Dict[str, Union[_Bis, _Dis1]]
@@ -90,15 +91,15 @@
 
         # Ensure parameters exist on the dataset
         sig = inspect.signature(kls)
         params = {}
         for k, v in params_raw.items():
             if k in sig.parameters:
                 params[k] = v
-        return kls(**params)
+        return kls(**params)  # type: ignore
 
 
 KedroDataSetSpec.update_forward_refs()
 
 
 class FolderFormatMetadata(BaseModel):
     """Metadata for the folder-formatted dataset.
@@ -107,22 +108,25 @@
     ----------
     model_class : str
         The class name of the model.
     model_info
         Model parameters, encoded with a data path.
     catalog : dict
         Mapping of "json path" to a dataset spec.
+    pydantic_types : dict
+        Mapping of "json path" to the Pydantic model type, for nested models.
     """
 
     model_class: str
-    model_info: Union[Dict[str, Any], List[Any]]
+    model_info: Dict[str, Any]
     catalog: Dict[JsonPath, KedroDataSetSpec] = {}
+    # pydantic_types: Dict[JsonPath, ImportStr] = {}
 
 
-def mutate_jsp(struct: Union[Dict[str, Any], List[Any]], jsp: List[str], obj: Any) -> None:
+def mutate_jsp(struct: Union[Dict[str, Any], List[Any]], jsp: List[JsonPath], obj: Any) -> None:
     """Mutates `struct` in-place given the jsp (which is json-path-like)."""
     if isinstance(struct, dict):
         key = jsp[0]
         if len(jsp) == 1:
             # Mutate element
             struct[key] = obj
             return
@@ -244,15 +248,15 @@
         model_data: Union[Dict[str, Any], List[Any]] = deepcopy(meta.model_info)
         for jsp_str, ds_spec in meta.catalog.items():
             jsp = jsp_str.split(".")[1:]
             ds_i = ds_spec.to_dataset(base_path=filepath)
             obj_i = ds_i.load()
             mutate_jsp(model_data, jsp, obj_i)
 
-        res = model_cls.parse_obj(model_data)
+        res = dict_to_model(model_data)
         return res
 
     def _save_local(self, data: BaseModel, filepath: str) -> None:
         # Prepare fields for final metadata
         kls = type(data)
         model_class_str = get_import_name(kls)
         model_info: Union[Dict[str, Any], List[Any]] = {}
@@ -283,15 +287,16 @@
                 return kls.__json_encoder__(obj)
             except TypeError:
                 val = f"{starter}__{uuid4()}".replace("-", "")
                 data_map[val] = obj
                 return val
 
         # Roundtrip to apply the encoder and get UUID
-        rt = json.loads(data.json(encoder=fake_encoder))
+        with PatchPydanticIter():
+            rt = json.loads(data.json(encoder=fake_encoder))
 
         # This will map the data to a dataset and actually save it
 
         def visit3(obj: Any, jsp: str, base_path: str) -> Any:
             """Map the data to a dataset in `catalog` and actually saves it."""
             if isinstance(obj, str):
                 if obj in data_map:
@@ -311,14 +316,16 @@
             elif isinstance(obj, list):
                 return [visit3(sub, f"{jsp}.{i}", base_path) for i, sub in enumerate(obj)]
             elif isinstance(obj, dict):
                 return {k: visit3(v, f"{jsp}.{k}", base_path) for k, v in obj.items()}
             return obj
 
         model_info = visit3(rt, "", base_path=filepath)
+        if not isinstance(model_info, dict):
+            raise NotImplementedError("Only dict root is supported for now.")
 
         # Create and write metadata
         meta = FolderFormatMetadata(model_class=model_class_str, model_info=model_info, catalog=catalog)
         with fsspec.open(f"{filepath}/meta.json", mode="w") as f:
             f.write(meta.json())  # type: ignore
 
     def _describe(self) -> Dict[str, Any]:
```

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/json.py` & `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/yaml.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-"""JSON dataset definition for Pydantic."""
+"""YAML dataset definition for Pydantic."""
 
-import json
 from pathlib import PurePosixPath
 from typing import Any, Dict, no_type_check
 
 import fsspec
+import ruamel.yaml as yaml
 from fsspec import AbstractFileSystem
 from kedro.io.core import AbstractDataSet, get_filepath_str, get_protocol_and_path
-from pydantic import BaseModel, create_model, parse_obj_as
-from pydantic.utils import import_string
+from pydantic import BaseModel
+from pydantic_yaml import to_yaml_file
 
-KLS_MARK_STR = "class"
+from pydantic_kedro._dict_io import PatchPydanticIter, dict_to_model
 
 
-class PydanticJsonDataSet(AbstractDataSet[BaseModel, BaseModel]):
-    """Dataset for saving/loading Pydantic models, based on JSON.
+class PydanticYamlDataSet(AbstractDataSet[BaseModel, BaseModel]):
+    """Dataset for saving/loading Pydantic models, based on YAML.
 
     Please note that the Pydantic model must be JSON-serializable.
     That means the fields are "pure" Pydantic fields,
     or you have added `json_encoders` to the model config.
 
     Example:
     -------
     ```python
     class MyModel(BaseModel):
         x: str
 
-    ds = PydanticJsonDataSet('memory://path/to/model.json')  # using memory to avoid tempfile
+    ds = PydanticYamlDataSet('memory://path/to/model.yaml')  # using memory to avoid tempfile
     ds.save(MyModel(x="example"))
     assert ds.load().x == "example"
     ```
     """
 
     def __init__(self, filepath: str) -> None:
-        """Create a new instance of PydanticJsonDataSet to load/save Pydantic models for given filepath.
+        """Create a new instance of PydanticYamlDataSet to load/save Pydantic models for given filepath.
 
         Args:
         ----
-        filepath : The location of the JSON file.
+        filepath : The location of the YAML file.
         """
+        # TODO: Update to just save the path and open it with `fsspec` directly
         # parse the path and protocol (e.g. file, http, s3, etc.)
         protocol, path = get_protocol_and_path(filepath)
         self._protocol = protocol
         self._filepath = PurePosixPath(path)
         self._fs: AbstractFileSystem = fsspec.filesystem(self._protocol)
 
     @property
@@ -57,41 +58,25 @@
         -------
         Pydantic model.
         """
         # using get_filepath_str ensures that the protocol and path
         # are appended correctly for different filesystems
         load_path = get_filepath_str(self._filepath, self._protocol)
         with self._fs.open(load_path, mode="r") as f:
-            dct = json.load(f)
-        assert isinstance(dct, dict), "JSON root must be a mapping."
-        if KLS_MARK_STR not in dct.keys():
-            raise TypeError(f"Cannot determine pydantic model type, missing {KLS_MARK_STR!r}")
-        pyd_kls = import_string(dct[KLS_MARK_STR])
-        assert issubclass(pyd_kls, BaseModel), f"Type must be a Pydantic model, got {type(pyd_kls)!r}."
-        dct.pop(KLS_MARK_STR)  # don't accidentally pass to proper model
-        res = parse_obj_as(pyd_kls, dct)
+            dct = yaml.safe_load(f)
+
+        assert isinstance(dct, dict), "YAML root must be a mapping."
+        res = dict_to_model(dct)
         return res  # type: ignore
 
     @no_type_check
     def _save(self, data: BaseModel) -> None:
         """Save Pydantic model to the filepath."""
-        # Add metadata to our Pydantic model
-        pyd_kls = type(data)
-        if KLS_MARK_STR in pyd_kls.__fields__.keys():
-            raise ValueError(f"Marker {KLS_MARK_STR!r} already exists as a field; can't dump model.")
-        pyd_kls_path = f"{pyd_kls.__module__}.{pyd_kls.__qualname__}"
-        tmp_kls = create_model(
-            pyd_kls.__name__,
-            __base__=pyd_kls,
-            __module__=pyd_kls.__module__,
-            **{KLS_MARK_STR: (str, pyd_kls_path)},
-        )
-        tmp_obj = tmp_kls(**data.dict())
-
         # Open file and write to it
         save_path = get_filepath_str(self._filepath, self._protocol)
-        with self._fs.open(save_path, mode="w") as f:
-            f.write(tmp_obj.json())
+        with PatchPydanticIter():
+            with self._fs.open(save_path, mode="w") as f:
+                to_yaml_file(f, data)
 
     def _describe(self) -> Dict[str, Any]:
         """Return a dict that describes the attributes of the dataset."""
         return dict(filepath=self.filepath, protocol=self._protocol)
```

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/yaml.py` & `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/json.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,47 @@
-"""YAML dataset definition for Pydantic."""
+"""JSON dataset definition for Pydantic."""
 
+import json
 from pathlib import PurePosixPath
 from typing import Any, Dict, no_type_check
 
 import fsspec
 from fsspec import AbstractFileSystem
 from kedro.io.core import AbstractDataSet, get_filepath_str, get_protocol_and_path
-from pydantic import BaseModel, Field, create_model
-from pydantic.utils import import_string
-from pydantic_yaml import parse_yaml_file_as, to_yaml_file
+from pydantic import BaseModel
 
-KLS_MARK_STR = "class"
+from pydantic_kedro._dict_io import PatchPydanticIter, dict_to_model
 
 
-class _YamlPreLoader(BaseModel):
-    """YAML pre-loader model."""
-
-    kls_mark_str: str = Field(alias=KLS_MARK_STR)  # type: ignore
-
-
-class PydanticYamlDataSet(AbstractDataSet[BaseModel, BaseModel]):
-    """Dataset for saving/loading Pydantic models, based on YAML.
+class PydanticJsonDataSet(AbstractDataSet[BaseModel, BaseModel]):
+    """Dataset for saving/loading Pydantic models, based on JSON.
 
     Please note that the Pydantic model must be JSON-serializable.
     That means the fields are "pure" Pydantic fields,
     or you have added `json_encoders` to the model config.
 
     Example:
     -------
     ```python
     class MyModel(BaseModel):
         x: str
 
-    ds = PydanticYamlDataSet('memory://path/to/model.yaml')  # using memory to avoid tempfile
+    ds = PydanticJsonDataSet('memory://path/to/model.json')  # using memory to avoid tempfile
     ds.save(MyModel(x="example"))
     assert ds.load().x == "example"
     ```
     """
 
     def __init__(self, filepath: str) -> None:
-        """Create a new instance of PydanticYamlDataSet to load/save Pydantic models for given filepath.
+        """Create a new instance of PydanticJsonDataSet to load/save Pydantic models for given filepath.
 
         Args:
         ----
-        filepath : The location of the YAML file.
+        filepath : The location of the JSON file.
         """
-        # TODO: Update to just save the path and open it with `fsspec` directly
         # parse the path and protocol (e.g. file, http, s3, etc.)
         protocol, path = get_protocol_and_path(filepath)
         self._protocol = protocol
         self._filepath = PurePosixPath(path)
         self._fs: AbstractFileSystem = fsspec.filesystem(self._protocol)
 
     @property
@@ -64,38 +56,24 @@
         -------
         Pydantic model.
         """
         # using get_filepath_str ensures that the protocol and path
         # are appended correctly for different filesystems
         load_path = get_filepath_str(self._filepath, self._protocol)
         with self._fs.open(load_path, mode="r") as f:
-            preloader = parse_yaml_file_as(_YamlPreLoader, f)
-        pyd_kls = import_string(preloader.kls_mark_str)
-        assert issubclass(pyd_kls, BaseModel), f"Type must be a Pydantic model, got {type(pyd_kls)!r}."
-        with self._fs.open(load_path, mode="r") as f:
-            res = parse_yaml_file_as(pyd_kls, f)
+            dct = json.load(f)
+        assert isinstance(dct, dict), "JSON root must be a mapping."
+        res = dict_to_model(dct)
         return res  # type: ignore
 
     @no_type_check
     def _save(self, data: BaseModel) -> None:
         """Save Pydantic model to the filepath."""
-        # Add metadata to our Pydantic model
-        pyd_kls = type(data)
-        if KLS_MARK_STR in pyd_kls.__fields__.keys():
-            raise ValueError(f"Marker {KLS_MARK_STR!r} already exists as a field; can't dump model.")
-        pyd_kls_path = f"{pyd_kls.__module__}.{pyd_kls.__qualname__}"
-        tmp_kls = create_model(
-            pyd_kls.__name__,
-            __base__=pyd_kls,
-            __module__=pyd_kls.__module__,
-            **{KLS_MARK_STR: (str, pyd_kls_path)},
-        )
-        tmp_obj = tmp_kls(**data.dict())
-
         # Open file and write to it
         save_path = get_filepath_str(self._filepath, self._protocol)
-        with self._fs.open(save_path, mode="w") as f:
-            to_yaml_file(f, tmp_obj)
+        with PatchPydanticIter():
+            with self._fs.open(save_path, mode="w") as f:
+                f.write(data.json())
 
     def _describe(self) -> Dict[str, Any]:
         """Return a dict that describes the attributes of the dataset."""
         return dict(filepath=self.filepath, protocol=self._protocol)
```

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/zip.py` & `pydantic-kedro-0.5.0/src/pydantic_kedro/datasets/zip.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro/models.py` & `pydantic-kedro-0.5.0/src/pydantic_kedro/models.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro/utils.py` & `pydantic-kedro-0.5.0/src/pydantic_kedro/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/PKG-INFO` & `pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.4.0
+Version: 0.5.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/SOURCES.txt` & `pydantic-kedro-0.5.0/src/pydantic_kedro.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 .github/workflows/python-testing.yml
 docs/arbitrary_types.md
 docs/implementation_details.md
 docs/index.md
 docs/reference.md
 docs/standalone_usage.md
 src/pydantic_kedro/__init__.py
+src/pydantic_kedro/_dict_io.py
 src/pydantic_kedro/_internals.py
 src/pydantic_kedro/models.py
 src/pydantic_kedro/py.typed
 src/pydantic_kedro/utils.py
 src/pydantic_kedro/version.py
 src/pydantic_kedro.egg-info/PKG-INFO
 src/pydantic_kedro.egg-info/SOURCES.txt
@@ -37,13 +38,14 @@
 src/test/test_auto.py
 src/test/test_docs_standalone.py
 src/test/test_ds_extended.py
 src/test/test_ds_pandas.py
 src/test/test_ds_simple.py
 src/test/test_import.py
 src/test/test_inheritance.py
+src/test/test_nested_subtypes.py
 src/test/test_utils.py
 src/test/catalogs/test_basic_catalog.py
 src/test/catalogs/conf/base/catalog.yml
 src/test/catalogs/conf/local/.gitkeep
 src/test/catalogs/conf/local/credentials.yml
 src/test/catalogs/data/tst1.json
```

### Comparing `pydantic-kedro-0.4.0/src/test/catalogs/test_basic_catalog.py` & `pydantic-kedro-0.5.0/src/test/catalogs/test_basic_catalog.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/test/test_auto.py` & `pydantic-kedro-0.5.0/src/test/test_auto.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/test/test_docs_standalone.py` & `pydantic-kedro-0.5.0/src/test/test_docs_standalone.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/test/test_ds_extended.py` & `pydantic-kedro-0.5.0/src/test/test_ds_extended.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/test/test_ds_pandas.py` & `pydantic-kedro-0.5.0/src/test/test_ds_pandas.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/test/test_ds_simple.py` & `pydantic-kedro-0.5.0/src/test/test_ds_simple.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.4.0/src/test/test_inheritance.py` & `pydantic-kedro-0.5.0/src/test/test_inheritance.py`

 * *Files identical despite different names*

