# Comparing `tmp/ethpm-types-0.5.1.tar.gz` & `tmp/ethpm-types-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.5.1.tar", last modified: Tue May 23 13:43:33 2023, max compression
+gzip compressed data, was "ethpm-types-0.5.2.tar", last modified: Thu Jun  1 20:02:29 2023, max compression
```

## Comparing `ethpm-types-0.5.1.tar` & `ethpm-types-0.5.2.tar`

### file list

```diff
@@ -1,88 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.831462 ethpm-types-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.815462 ethpm-types-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.815462 ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-23 13:43:33.831462 ethpm-types-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.823462 ethpm-types-0.5.1/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 13:43:33.835461 ethpm-types-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.823462 ethpm-types-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.811462 ethpm-types-0.5.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.831462 ethpm-types-0.5.1/tests/data/Compiled/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/HasError.json
--rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (123)    43486 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (123)   220464 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.831462 ethpm-types-0.5.1/tests/data/Sources/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Sources/SolidityContract.sol
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Sources/VyperContract.vy
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_hexbytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_sourcemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.493046 ethpm-types-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.485046 ethpm-types-0.5.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/tests/data/Compiled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/HasError.json
+-rw-r--r--   0 runner    (1001) docker     (123) 12327472 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/SolFallbackAndReceive.json
+-rw-r--r--   0 runner    (1001) docker     (123)   227889 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/VyDefault.json
+-rw-r--r--   0 runner    (1001) docker     (123)   230644 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/tests/data/Sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/SolFallbackAndReceive.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/SolidityContract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/VyDefault.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/VyperContract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_hexbytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_sourcemap.py
```

### Comparing `ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.github/release-drafter.yml` & `ethpm-types-0.5.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.github/workflows/commitlint.yaml` & `ethpm-types-0.5.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.github/workflows/docs.yaml` & `ethpm-types-0.5.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.github/workflows/prtitle.yaml` & `ethpm-types-0.5.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.github/workflows/publish.yaml` & `ethpm-types-0.5.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.github/workflows/test.yaml` & `ethpm-types-0.5.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.gitignore` & `ethpm-types-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/.pre-commit-config.yaml` & `ethpm-types-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/CONTRIBUTING.md` & `ethpm-types-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/LICENSE` & `ethpm-types-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/PKG-INFO` & `ethpm-types-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.5.1
+Version: 0.5.2
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.5.1/README.md` & `ethpm-types-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/build_docs.py` & `ethpm-types-0.5.2/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/docs/_static/custom.css` & `ethpm-types-0.5.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/docs/_static/custom.js` & `ethpm-types-0.5.2/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/docs/_templates/layout.html` & `ethpm-types-0.5.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/docs/conf.py` & `ethpm-types-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/docs/favicon.ico` & `ethpm-types-0.5.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/docs/logo.gif` & `ethpm-types-0.5.2/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types/__init__.py` & `ethpm-types-0.5.2/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types/abi.py` & `ethpm-types-0.5.2/ethpm_types/abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types/ast.py` & `ethpm-types-0.5.2/ethpm_types/ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types/base.py` & `ethpm-types-0.5.2/ethpm_types/base.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types/contract_type.py` & `ethpm-types-0.5.2/ethpm_types/contract_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 from functools import singledispatchmethod
-from typing import Callable, Dict, Iterable, List, Optional, TypeVar, Union
+from typing import Callable, Dict, Iterable, List, Optional, Type, TypeVar, Union
 
 from eth_utils import add_0x_prefix, is_0x_prefixed
 from pydantic import Field, validator
 
 from ethpm_types.abi import (
     ABI,
     ConstructorABI,
     ErrorABI,
     EventABI,
     FallbackABI,
     MethodABI,
+    ReceiveABI,
     StructABI,
 )
 from ethpm_types.ast import ASTNode
 from ethpm_types.base import BaseModel
 from ethpm_types.sourcemap import PCMap, SourceMap
 from ethpm_types.utils import Hex, HexBytes, is_valid_hex
 
+ABILIST_T = TypeVar("ABILIST_T", bound=Union[MethodABI, EventABI, StructABI, ErrorABI])
+"""The generic used for the ABIList class. Only for type-checking."""
+
+ABI_SINGLETON_T = TypeVar("ABI_SINGLETON_T", bound=Union[FallbackABI, ConstructorABI, ReceiveABI])
+"""
+The generic used for discovering the unique ABIs from the list.
+Only for type-checking.
+"""
+
 
 # TODO link references & link values are for solidity, not used with Vyper
 # Offsets are for dynamic links, e.g. EIP1167 proxy forwarder
 class LinkDependency(BaseModel):
     offsets: List[int]
     """
     The locations within the corresponding bytecode where the value for this
@@ -132,25 +142,22 @@
     The runtime portion of bytecode for this Contract Instance.
     When present, the value from this field supersedes the ``runtimeBytecode``
     from the :class:`~ethpm_types.contract_type.ContractType` for this
     ``ContractInstance``.
     """
 
 
-T = TypeVar("T", bound=Union[MethodABI, EventABI, StructABI, ErrorABI])
-
-
-class ABIList(List[T]):
+class ABIList(List[ABILIST_T]):
     """
     Adds selection by name, selector and keccak(selector).
     """
 
     def __init__(
         self,
-        iterable: Optional[Iterable[T]] = None,
+        iterable: Optional[Iterable[ABILIST_T]] = None,
         *,
         selector_id_size: int = 32,
         selector_hash_fn: Optional[Callable[[str], bytes]] = None,
     ):
         self._selector_id_size = selector_id_size
         self._selector_hash_fn = selector_hash_fn
         super().__init__(iterable or ())
@@ -319,44 +326,39 @@
         """
         The constructor of the contract, if it has one. For example,
         your smart-contract (in Solidity) may define a ``constructor() public {}``.
         This property contains information about the parameters needed to initialize
         a contract.
         """
 
-        constructor_abi: Optional[ConstructorABI] = None
-        for abi in self.abi:
-            if isinstance(abi, ConstructorABI):
-                constructor_abi = abi
-                break
-
-        constructor_abi = constructor_abi or ConstructorABI(
-            type="constructor"
-        )  # Use default constructor (no args)
-        constructor_abi.contract_type = self
-        return constructor_abi
+        # Use default constructor (no args) when no defined.
+        abi = self._get_first_instance(ConstructorABI) or ConstructorABI(type="constructor")
+        abi.contract_type = self
+        return abi
 
     @property
-    def fallback(self) -> FallbackABI:
+    def fallback(self) -> Optional[FallbackABI]:
         """
         The fallback method of the contract, if it has one. A fallback method
         is external, has no name, arguments, or return value, and gets invoked
         when the user attempts to call a method that does not exist.
         """
 
-        fallback_abi: Optional[FallbackABI] = None
-        for abi in self.abi:
-            if isinstance(abi, FallbackABI):
-                fallback_abi = abi
-                break
-
-        # Use default fallback (no args) if not defined
-        fallback_abi = fallback_abi or FallbackABI(type="fallback")
-        fallback_abi.contract_type = self
-        return fallback_abi
+        return self._get_first_instance(FallbackABI)
+
+    @property
+    def receive(self) -> Optional[ReceiveABI]:
+        """
+        The ``receive()`` method of the contract, if it has one. A contract may
+        have 0-1 ``receive()`` methods defined. It gets executed when calling
+        the contract with empty calldata. The method is not allowed any arguments
+        and cannot return anything.
+        """
+
+        return self._get_first_instance(ReceiveABI)
 
     @property
     def view_methods(self) -> ABIList[MethodABI]:
         """
         The call-methods (read-only method, non-payable methods) defined in a smart contract.
 
         Returns:
@@ -429,14 +431,27 @@
 
         return ABIList(
             method_abis,
             selector_id_size=selector_id_size,
             selector_hash_fn=self._selector_hash_fn,
         )
 
+    def _get_first_instance(self, _type: Type[ABI_SINGLETON_T]) -> Optional[ABI_SINGLETON_T]:
+        for abi in self.abi:
+            if not isinstance(abi, _type):
+                continue
+
+            # TODO: Figure out better way than type ignore.
+            #  getting `<nothing> has no attribute contract_type`.
+            #  probably using generics wrong but not sure how else to do it.
+            abi.contract_type = self  # type: ignore[attr-defined]
+            return abi
+
+        return None
+
 
 class BIP122_URI(str):
     """
     A URI scheme for looking up blocks.
     `BIP-122 <https://github.com/bitcoin/bips/blob/master/bip-0122.mediawiki>`__.
 
     URI Format::
```

### Comparing `ethpm-types-0.5.1/ethpm_types/manifest.py` & `ethpm-types-0.5.2/ethpm_types/manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types/source.py` & `ethpm-types-0.5.2/ethpm_types/source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types/sourcemap.py` & `ethpm-types-0.5.2/ethpm_types/sourcemap.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types/utils.py` & `ethpm-types-0.5.2/ethpm_types/utils.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.5.2/ethpm_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.5.1
+Version: 0.5.2
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.5.1/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.5.2/ethpm_types.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -60,13 +60,17 @@
 tests/test_package_manifest.py
 tests/test_pc_map.py
 tests/test_schema_fuzzing.py
 tests/test_source.py
 tests/test_sourcemap.py
 tests/data/Compiled/HasError.json
 tests/data/Compiled/OpenZeppelinContracts.json
+tests/data/Compiled/SolFallbackAndReceive.json
 tests/data/Compiled/SolidityContract.json
 tests/data/Compiled/TestStrategy.srcmap
+tests/data/Compiled/VyDefault.json
 tests/data/Compiled/VyperContract.json
 tests/data/Sources/HasError.sol
+tests/data/Sources/SolFallbackAndReceive.sol
 tests/data/Sources/SolidityContract.sol
+tests/data/Sources/VyDefault.vy
 tests/data/Sources/VyperContract.vy
```

### Comparing `ethpm-types-0.5.1/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.5.2/ethpm_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/pyproject.toml` & `ethpm-types-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/setup.py` & `ethpm-types-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/conftest.py` & `ethpm-types-0.5.2/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from pathlib import Path
 
 import pytest
 
 from ethpm_types import ContractType, PackageManifest, Source
 
 BASE = Path(__file__).parent / "data"
@@ -16,22 +15,21 @@
     def fn(name: str) -> ContractType:
         return ContractType.parse_file(COMPILED_BASE / f"{name}.json")
 
     return fn
 
 
 @pytest.fixture
-def oz_package_manifest_dict():
-    oz_manifest_file = COMPILED_BASE / "OpenZeppelinContracts.json"
-    return json.loads(oz_manifest_file.read_text())
+def oz_package_manifest_path():
+    return COMPILED_BASE / "OpenZeppelinContracts.json"
 
 
 @pytest.fixture
-def oz_package(oz_package_manifest_dict):
-    return PackageManifest.parse_obj(oz_package_manifest_dict)
+def oz_package(oz_package_manifest_path):
+    return PackageManifest.parse_file(oz_package_manifest_path)
 
 
 @pytest.fixture
 def source_base() -> Path:
     return SOURCE_BASE
 
 
@@ -70,7 +68,23 @@
 def contract_with_error(get_contract_type):
     return get_contract_type("HasError")
 
 
 @pytest.fixture(params=("Vyper", "Solidity"))
 def contract(request, get_contract_type):
     yield get_contract_type(f"{request.param}Contract")
+
+
+@pytest.fixture
+def solidity_fallback_and_receive_contract(get_contract_type):
+    return get_contract_type("SolFallbackAndReceive")
+
+
+@pytest.fixture
+def vyper_default_contract(get_contract_type):
+    return get_contract_type("VyDefault")
+
+
+@pytest.fixture(params=("Vyper", "Solidity"))
+def fallback_contract(request, get_contract_type):
+    key = "VyDefault" if request.param == "Vyper" else "SolFallbackAndReceive"
+    return get_contract_type(key)
```

### Comparing `ethpm-types-0.5.1/tests/data/Compiled/HasError.json` & `ethpm-types-0.5.2/tests/data/Compiled/HasError.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/data/Compiled/TestStrategy.srcmap` & `ethpm-types-0.5.2/tests/data/Compiled/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/data/Sources/SolidityContract.sol` & `ethpm-types-0.5.2/tests/data/Sources/SolidityContract.sol`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/data/Sources/VyperContract.vy` & `ethpm-types-0.5.2/tests/data/Sources/VyperContract.vy`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/test_ast.py` & `ethpm-types-0.5.2/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/test_cairo.py` & `ethpm-types-0.5.2/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/test_contract_type.py` & `ethpm-types-0.5.2/tests/test_contract_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -194,15 +194,14 @@
 
 def test_contract_type_backrefs(oz_contract_type):
     assert oz_contract_type.events, "setup: Test contract should have events"
     assert oz_contract_type.view_methods, "setup: Test contract should have view methods"
     assert oz_contract_type.mutable_methods, "setup: Test contract should have mutable methods"
 
     assert oz_contract_type.constructor.contract_type == oz_contract_type
-    assert oz_contract_type.fallback.contract_type == oz_contract_type
     assert all(e.contract_type == oz_contract_type for e in oz_contract_type.events)
     assert all(m.contract_type == oz_contract_type for m in oz_contract_type.mutable_methods)
     assert all(m.contract_type == oz_contract_type for m in oz_contract_type.view_methods)
 
 
 @view_selector_parametrization
 def test_select_view_method_from_all_methods(selector, vyper_contract):
@@ -217,7 +216,38 @@
 
 
 def test_repr(vyper_contract):
     assert repr(vyper_contract) == "<ContractType VyperContract>"
 
     vyper_contract.name = None
     assert repr(vyper_contract) == "<ContractType>"
+
+
+def test_solidity_fallback_and_receive(solidity_fallback_and_receive_contract):
+    """
+    Ensure we can detect the fallback and receive methods when they are defined.
+    For solidity, you can define both.
+    """
+    assert solidity_fallback_and_receive_contract.fallback.type == "fallback"
+    assert solidity_fallback_and_receive_contract.receive.type == "receive"
+
+    # Typically, if receive is defined, fallback is non-payable.
+    # Though, that is not always the case.
+    assert solidity_fallback_and_receive_contract.fallback.stateMutability == "nonpayable"
+
+
+def test_vyper_default(vyper_default_contract):
+    """
+    Ensure the Vyper default method shows up as the fallback method in the contract.
+    """
+    assert vyper_default_contract.fallback.type == "fallback"
+
+
+def test_fallback_and_receive_not_defined(contract):
+    """
+    Ensure that when the fallback method is not defined, in a Solidity contract,
+    it is None. Same with the receive method. Runs for both Solidity and Vyper.
+    """
+
+    # Both `VyperContract` and `SolidityContract` do not define these.
+    assert contract.receive is None
+    assert contract.fallback is None
```

### Comparing `ethpm-types-0.5.1/tests/test_hexbytes.py` & `ethpm-types-0.5.2/tests/test_hexbytes.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/test_package_manifest.py` & `ethpm-types-0.5.2/tests/test_package_manifest.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,18 +36,15 @@
                     assert source.content_is_valid(), f"Invalid checksum for '{source_name}'"
 
     else:
         with pytest.raises(ValidationError):
             PackageManifest.parse_obj(example_json).dict()
 
 
-def test_open_zeppelin_contracts(oz_package, oz_package_manifest_dict):
-    actual = oz_package.dict()
-    assert actual == oz_package_manifest_dict
-
+def test_open_zeppelin_contracts(oz_package):
     for source_name, source in oz_package.sources.items():
         # NOTE: Per EIP-2678, "Checksum is only required if content is missing"
         if not source.content:
             assert source.content_is_valid(), f"Invalid checksum for '{source_name}'"
 
 
 def test_file_bases_dependency_url():
```

### Comparing `ethpm-types-0.5.1/tests/test_pc_map.py` & `ethpm-types-0.5.2/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/test_schema_fuzzing.py` & `ethpm-types-0.5.2/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/test_source.py` & `ethpm-types-0.5.2/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.1/tests/test_sourcemap.py` & `ethpm-types-0.5.2/tests/test_sourcemap.py`

 * *Files identical despite different names*

