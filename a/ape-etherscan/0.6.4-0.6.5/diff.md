# Comparing `tmp/ape-etherscan-0.6.4.tar.gz` & `tmp/ape-etherscan-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-etherscan-0.6.4.tar", last modified: Thu May  4 20:15:14 2023, max compression
+gzip compressed data, was "ape-etherscan-0.6.5.tar", last modified: Thu Jun  1 21:39:27 2023, max compression
```

## Comparing `ape-etherscan-0.6.4.tar` & `ape-etherscan-0.6.5.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.026023 ape-etherscan-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.026023 ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.026023 ape-etherscan-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/ape_etherscan/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/ape_etherscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/mock_responses/get_account_transactions.json
--rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/mock_responses/get_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/mock_responses/get_proxy_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/mock_responses/get_vyper_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/test_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/ape_etherscan/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/ape_etherscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/mock_responses/get_account_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/mock_responses/get_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/mock_responses/get_proxy_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/mock_responses/get_vyper_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/test_etherscan.py
```

### Comparing `ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/bug.md` & `ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/feature.md` & `ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/work-item.md` & `ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/release-drafter.yml` & `ape-etherscan-0.6.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/workflows/codeql.yml` & `ape-etherscan-0.6.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/workflows/commit.yaml` & `ape-etherscan-0.6.5/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/workflows/prtitle.yaml` & `ape-etherscan-0.6.5/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/workflows/publish.yaml` & `ape-etherscan-0.6.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/workflows/stale-prs.yml` & `ape-etherscan-0.6.5/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.github/workflows/test.yaml` & `ape-etherscan-0.6.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.gitignore` & `ape-etherscan-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/.pre-commit-config.yaml` & `ape-etherscan-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/CONTRIBUTING.md` & `ape-etherscan-0.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/LICENSE` & `ape-etherscan-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/PKG-INFO` & `ape-etherscan-0.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.4
+Version: 0.6.5
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
         The following blockchain explorers are supported in this plugin:
         
         - [Etherscan](https://etherscan.io/) for Ethereum networks.
         - [Ftmscan](https://ftmscan.com) for Fantom networks.
         - [Arbiscan](https://arbiscan.io) for Arbitrum networks.
         - [Optimistic Etherscan](https://optimistic.etherscan.io) for Optimism networks.
         - [Polygonscan](https://polygonscan.com) for Polygon networks.
+        - [Polygonscan ZkEVM](https://zkevm.polygonscan.com) for Polygon ZkEVM networks.
         - [Snowtrace](https://snowtrace.io) for Avalanche networks.
+        - [Basescan](https://basescan.org) for Base networks.
         - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
         
         ## Dependencies
         
         - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
         
         ## Installation
@@ -54,14 +56,16 @@
         
         You can obtain an API key by registering with Etherscan and visiting [this page](https://etherscan.io/myapikey).
         
         ```bash
         export ETHERSCAN_API_KEY=SAMPLE_KEY
         export FTMSCAN_API_KEY=SAMPLE_KEY
         export ARBISCAN_API_KEY=SAMPLE_KEY
+        export POLYGON_ZKEVM_ETHERSCAN_API_KEY=SAMPLE_KEY
+        export BASESCAN_API_KEY=SAMPLE_KEY
         ```
         
         ## Transaction URLs
         
         When you have this plugin installed, Etherscan explorer URLs appear in CLI output.
         
         ```bash
@@ -124,14 +128,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
```

### Comparing `ape-etherscan-0.6.4/README.md` & `ape-etherscan-0.6.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 The following blockchain explorers are supported in this plugin:
 
 - [Etherscan](https://etherscan.io/) for Ethereum networks.
 - [Ftmscan](https://ftmscan.com) for Fantom networks.
 - [Arbiscan](https://arbiscan.io) for Arbitrum networks.
 - [Optimistic Etherscan](https://optimistic.etherscan.io) for Optimism networks.
 - [Polygonscan](https://polygonscan.com) for Polygon networks.
+- [Polygonscan ZkEVM](https://zkevm.polygonscan.com) for Polygon ZkEVM networks.
 - [Snowtrace](https://snowtrace.io) for Avalanche networks.
+- [Basescan](https://basescan.org) for Base networks.
 - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
 
 ## Dependencies
 
 - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
 
 ## Installation
@@ -46,14 +48,16 @@
 
 You can obtain an API key by registering with Etherscan and visiting [this page](https://etherscan.io/myapikey).
 
 ```bash
 export ETHERSCAN_API_KEY=SAMPLE_KEY
 export FTMSCAN_API_KEY=SAMPLE_KEY
 export ARBISCAN_API_KEY=SAMPLE_KEY
+export POLYGON_ZKEVM_ETHERSCAN_API_KEY=SAMPLE_KEY
+export BASESCAN_API_KEY=SAMPLE_KEY
 ```
 
 ## Transaction URLs
 
 When you have this plugin installed, Etherscan explorer URLs appear in CLI output.
 
 ```bash
```

### Comparing `ape-etherscan-0.6.4/ape_etherscan/client.py` & `ape-etherscan-0.6.5/ape_etherscan/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import os
 import random
+import time
 from io import StringIO
 from typing import Dict, Iterator, List, Optional
 
 from ape.logging import logger
-from ape.utils import USER_AGENT
+from ape.utils import USER_AGENT, ManagerAccessMixin
 from requests import Session
 
 from ape_etherscan.exceptions import UnhandledResultError, UnsupportedEcosystemError
 from ape_etherscan.types import EtherscanResponse, SourceCodeResponse
 from ape_etherscan.utils import API_KEY_ENV_KEY_MAP
 
 
@@ -36,14 +37,24 @@
         )
     elif ecosystem_name == "optimism":
         return (
             "https://optimistic.etherscan.io"
             if network_name == "mainnet"
             else "https://goerli-optimism.etherscan.io"
         )
+    elif ecosystem_name == "polygon-zkevm":
+        return (
+            "https://zkevm.polygonscan.com"
+            if network_name == "mainnet"
+            else "https://testnet-zkevm.polygonscan.com"
+        )
+    elif ecosystem_name == "base":
+        return (
+            "https://basescan.org" if network_name == "mainnet" else "https://goerli.basescan.org"
+        )
     elif ecosystem_name == "polygon":
         return (
             "https://polygonscan.com"
             if network_name == "mainnet"
             else "https://mumbai.polygonscan.com"
         )
     elif ecosystem_name == "avalanche":
@@ -83,14 +94,26 @@
         )
     elif ecosystem_name == "optimism":
         return (
             "https://api-optimistic.etherscan.io/api"
             if network_name == "mainnet"
             else "https://api-goerli-optimistic.etherscan.io/api"
         )
+    elif ecosystem_name == "polygon-zkevm":
+        return (
+            "https://api-zkevm.polygonscan.com/api"
+            if network_name == "mainnet"
+            else "https://api-testnet-zkevm.polygonscan.com/api"
+        )
+    elif ecosystem_name == "base":
+        return (
+            "https://api.basescan.org/api"
+            if network_name == "mainnet"
+            else "https://api-goerli.basescan.org/api"
+        )
     elif ecosystem_name == "polygon":
         return (
             "https://api.polygonscan.com/api"
             if network_name == "mainnet"
             else "https://api-testnet.polygonscan.com/api"
         )
     elif ecosystem_name == "avalanche":
@@ -105,38 +128,63 @@
             if network_name != "mainnet"
             else "https://api.bscscan.com/api"
         )
 
     raise UnsupportedEcosystemError(ecosystem_name)
 
 
-class _APIClient:
+class _APIClient(ManagerAccessMixin):
     DEFAULT_HEADERS = {"User-Agent": USER_AGENT}
     session = Session()
 
     def __init__(self, ecosystem_name: str, network_name: str, module_name: str):
         self._ecosystem_name = ecosystem_name
         self._network_name = network_name
         self._module_name = module_name
+        self._last_call = 0.0
 
     @property
     def base_uri(self) -> str:
         return get_etherscan_api_uri(self._ecosystem_name, self._network_name)
 
     @property
     def base_params(self) -> Dict:
         return {"module": self._module_name}
 
+    @property
+    def _rate_limit(self) -> int:
+        config = self.config_manager.get_config("etherscan")
+        return getattr(config, self.network_manager.ecosystem.name.lower()).rate_limit
+
+    @property
+    def _retries(self) -> int:
+        config = self.config_manager.get_config("etherscan")
+        return getattr(config, self.network_manager.ecosystem.name.lower()).retries
+
+    @property
+    def _min_time_between_calls(self) -> float:
+        return 1 / self._rate_limit  # seconds / calls per second
+
     def _get(
         self,
         params: Optional[Dict] = None,
         headers: Optional[Dict[str, str]] = None,
         raise_on_exceptions: bool = True,
     ) -> EtherscanResponse:
         params = self.__authorize(params)
+
+        # Rate limit
+        if time.time() - self._last_call < self._min_time_between_calls:
+            time_to_sleep = self._min_time_between_calls - (time.time() - self._last_call)
+            logger.debug(f"Sleeping {time_to_sleep} seconds to avoid rate limit")
+            # NOTE: Sleep time is in seconds (float for subseconds)
+            time.sleep(time_to_sleep)
+
+        self._last_call = time.time()
+
         return self._request(
             "GET",
             params=params,
             headers=headers,
             raise_on_exceptions=raise_on_exceptions,
         )
 
@@ -151,22 +199,34 @@
         method: str,
         raise_on_exceptions: bool = True,
         headers: Optional[Dict] = None,
         params: Optional[Dict] = None,
         data: Optional[Dict] = None,
     ) -> EtherscanResponse:
         headers = headers or self.DEFAULT_HEADERS
-        response = self.session.request(
-            method.upper(), self.base_uri, headers=headers, params=params, data=data
-        )
+        for i in range(self._retries):
+            response = self.session.request(
+                method.upper(),
+                self.base_uri,
+                headers=headers,
+                params=params,
+                data=data,
+                timeout=1024,
+            )
+            if response.status_code == 429:
+                time.sleep(2**i)
+                continue
+
+            # Recieved a real response unrelated to rate limiting.
+            if raise_on_exceptions:
+                response.raise_for_status()
+            elif not 200 <= response.status_code < 300:
+                logger.error(response.text)
 
-        if raise_on_exceptions:
-            response.raise_for_status()
-        elif not 200 <= response.status_code < 300:
-            logger.error(response.text)
+            break
 
         return EtherscanResponse(response, self._ecosystem_name, raise_on_exceptions)
 
     def __authorize(self, params_or_data: Optional[Dict] = None) -> Optional[Dict]:
         env_var_key = API_KEY_ENV_KEY_MAP.get(self._ecosystem_name)
         if not env_var_key:
             return params_or_data
@@ -237,15 +297,14 @@
             "contractname": contract_name,
             "evmversion": evm_version,
             "licenseType": license_type,
             "optimizationUsed": int(optimization_used),
             "runs": optimization_runs,
             "sourceCode": StringIO(json.dumps(standard_json_output)),
         }
-
         iterator = 1
         for lib_address, lib_name in libraries.items():
             json_dict[f"libraryname{iterator}"] = lib_name
             json_dict[f"libraryaddress{iterator}"] = lib_address
             iterator += 1
 
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
```

### Comparing `ape-etherscan-0.6.4/ape_etherscan/exceptions.py` & `ape-etherscan-0.6.5/ape_etherscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/ape_etherscan/explorer.py` & `ape-etherscan-0.6.5/ape_etherscan/explorer.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/ape_etherscan/query.py` & `ape-etherscan-0.6.5/ape_etherscan/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,33 @@
             self.provider.network.name.replace("-fork", ""),
         )
 
     @singledispatchmethod
     def estimate_query(self, query: QueryType) -> Optional[int]:  # type: ignore[override]
         return None
 
+    @property
+    def rate_limit(self) -> int:
+        config = self.config_manager.get_config("etherscan")
+        return getattr(config, self.network_manager.ecosystem.name.lower()).rate_limit
+
     @estimate_query.register
     def estimate_account_transaction_query(self, query: AccountTransactionQuery) -> Optional[int]:
         if self.network_manager.active_provider:
             # Ignore unsupported networks.
             ecosystem = self.network_manager.provider.network.ecosystem.name
             network = self.network_manager.provider.network.name
             if network not in NETWORKS.get(ecosystem, {}):
                 return None
 
-        # About 15 ms per page of 100 transactions
-        return 1500 * (1 + query.stop_nonce - query.start_nonce) // 100
+        # About 15 ms per page of 100 transactions, with rate limit applied
+        if query.stop_nonce - query.stop_nonce <= 100:
+            return 15
+
+        return (10000 // self.rate_limit) * (1 + query.stop_nonce - query.start_nonce) // 100
 
     @singledispatchmethod
     def perform_query(self, query: QueryType) -> Iterator:  # type: ignore[override]
         raise QueryEngineError(
             f"{self.__class__.__name__} cannot handle {query.__class__.__name__} queries."
         )
```

### Comparing `ape-etherscan-0.6.4/ape_etherscan/types.py` & `ape-etherscan-0.6.5/ape_etherscan/types.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/ape_etherscan/utils.py` & `ape-etherscan-0.6.5/ape_etherscan/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 API_KEY_ENV_KEY_MAP = {
     "arbitrum": "ARBISCAN_API_KEY",
     "ethereum": "ETHERSCAN_API_KEY",
     "fantom": "FTMSCAN_API_KEY",
     "optimism": "OPTIMISTIC_ETHERSCAN_API_KEY",
+    "polygon-zkevm": "POLYGON_ZKEVM_ETHERSCAN_API_KEY",
+    "base": "BASESCAN_API_KEY",
     "polygon": "POLYGONSCAN_API_KEY",
     "avalanche": "SNOWTRACE_API_KEY",
     "bsc": "BSCSCAN_API_KEY",
 }
 NETWORKS = {
     "ethereum": [
         "mainnet",
@@ -21,14 +23,22 @@
         "opera",
         "testnet",
     ],
     "optimism": [
         "mainnet",
         "goerli",
     ],
+    "base": [
+        "mainnet",
+        "goerli",
+    ],
+    "polygon-zkevm": [
+        "mainnet",
+        "goerli",
+    ],
     "polygon": [
         "mainnet",
         "mumbai",
     ],
     "avalanche": [
         "mainnet",
         "fuji",
```

### Comparing `ape-etherscan-0.6.4/ape_etherscan/verify.py` & `ape-etherscan-0.6.5/ape_etherscan/verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,24 +264,33 @@
             logger.debug("Dumping standard JSON output:\n")
             standard_json = json.dumps(standard_input_json, indent=2)
             logger.debug(f"{standard_json}\n")
 
         # NOTE: Etherscan does not allow directory prefixes on the source ID.
         request_source_id = Path(source_id).name
 
-        guid = self._contract_client.verify_source_code(
-            standard_input_json,
-            str(version),
-            contract_name=f"{request_source_id}:{self._contract_type.name}",
-            optimization_used=optimized,
-            optimization_runs=runs,
-            constructor_arguments=self.constructor_arguments,
-            evm_version=evm_version,
-            license_type=license_code_value,
-        )
+        try:
+            guid = self._contract_client.verify_source_code(
+                standard_input_json,
+                str(version),
+                contract_name=f"{request_source_id}:{self._contract_type.name}",
+                optimization_used=optimized,
+                optimization_runs=runs,
+                constructor_arguments=self.constructor_arguments,
+                evm_version=evm_version,
+                license_type=license_code_value,
+            )
+        except EtherscanResponseError as err:
+            if "source code already verified" in str(err):
+                logger.warning(str(err))
+                return
+
+            else:
+                raise  # this error
+
         self._wait_for_verification(guid)
 
     def _get_standard_input_json(
         self, source_id: str, base_folder: Optional[Path] = None, **settings
     ) -> Dict:
         base_dir = base_folder or self.project_manager.contracts_folder
         source_path = base_dir / source_id
@@ -336,14 +345,19 @@
             try:
                 verification_update = self._contract_client.check_verify_status(guid)
                 guid_did_exist = True
             except EtherscanResponseError as err:
                 if "Resource not found" in str(err) and guid_did_exist:
                     # Sometimes, the GUID resource is gone before receiving a passing verification
                     verification_update = f"{pass_key}Complete"
+
+                elif "source code already verified" in str(err):
+                    # Consider this a pass.
+                    verification_update = "Already Verified"
+
                 else:
                     raise  # Original error
 
             if verification_update.startswith(fail_key):
                 err_msg = verification_update.split(fail_key)[-1].strip()
                 raise ContractVerificationError(err_msg)
             elif verification_update == "Already Verified" or verification_update.startswith(
```

### Comparing `ape-etherscan-0.6.4/ape_etherscan.egg-info/PKG-INFO` & `ape-etherscan-0.6.5/ape_etherscan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.4
+Version: 0.6.5
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
         The following blockchain explorers are supported in this plugin:
         
         - [Etherscan](https://etherscan.io/) for Ethereum networks.
         - [Ftmscan](https://ftmscan.com) for Fantom networks.
         - [Arbiscan](https://arbiscan.io) for Arbitrum networks.
         - [Optimistic Etherscan](https://optimistic.etherscan.io) for Optimism networks.
         - [Polygonscan](https://polygonscan.com) for Polygon networks.
+        - [Polygonscan ZkEVM](https://zkevm.polygonscan.com) for Polygon ZkEVM networks.
         - [Snowtrace](https://snowtrace.io) for Avalanche networks.
+        - [Basescan](https://basescan.org) for Base networks.
         - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
         
         ## Dependencies
         
         - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
         
         ## Installation
@@ -54,14 +56,16 @@
         
         You can obtain an API key by registering with Etherscan and visiting [this page](https://etherscan.io/myapikey).
         
         ```bash
         export ETHERSCAN_API_KEY=SAMPLE_KEY
         export FTMSCAN_API_KEY=SAMPLE_KEY
         export ARBISCAN_API_KEY=SAMPLE_KEY
+        export POLYGON_ZKEVM_ETHERSCAN_API_KEY=SAMPLE_KEY
+        export BASESCAN_API_KEY=SAMPLE_KEY
         ```
         
         ## Transaction URLs
         
         When you have this plugin installed, Etherscan explorer URLs appear in CLI output.
         
         ```bash
@@ -124,14 +128,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
```

### Comparing `ape-etherscan-0.6.4/ape_etherscan.egg-info/SOURCES.txt` & `ape-etherscan-0.6.5/ape_etherscan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .github/workflows/draft.yaml
 .github/workflows/prtitle.yaml
 .github/workflows/publish.yaml
 .github/workflows/stale-prs.yml
 .github/workflows/test.yaml
 ape_etherscan/__init__.py
 ape_etherscan/client.py
+ape_etherscan/config.py
 ape_etherscan/exceptions.py
 ape_etherscan/explorer.py
 ape_etherscan/py.typed
 ape_etherscan/query.py
 ape_etherscan/types.py
 ape_etherscan/utils.py
 ape_etherscan/verify.py
```

### Comparing `ape-etherscan-0.6.4/ape_etherscan.egg-info/requires.txt` & `ape-etherscan-0.6.5/ape_etherscan.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 eth-ape<0.7,>=0.6.7
 requests
 
 [dev]
 ape-arbitrum
+ape-base
 ape-bsc
 ape-fantom
 ape-optimism
 ape-polygon
+ape-polygon
 ape-infura
 ape-solidity
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
 pytest-mock
@@ -56,18 +58,20 @@
 setuptools
 setuptools-scm
 wheel
 twine
 
 [test]
 ape-arbitrum
+ape-base
 ape-bsc
 ape-fantom
 ape-optimism
 ape-polygon
+ape-polygon
 ape-infura
 ape-solidity
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
 pytest-mock
```

### Comparing `ape-etherscan-0.6.4/pyproject.toml` & `ape-etherscan-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/setup.py` & `ape-etherscan-0.6.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "ape-arbitrum",  # Needed for Arbitrum integration
+        "ape-base",  # Needed for Base networks integration
         "ape-bsc",  # For testing BSC integration
         "ape-fantom",  # For testing Fantom integration
         "ape-optimism",  # Needed for Optimism integration
         "ape-polygon",  # Needed for Polygon integration
+        "ape-polygon",  # Needed for Polygon ZkEVM integration
         "ape-infura",  # Needed for live network tests
         "ape-solidity",  # Needed for contract verification tests
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7",  # Strategy-based fuzzer
         "pytest-mock",  # Test mocker
@@ -72,15 +74,15 @@
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-etherscan",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.7,<0.7",
         "requests",  # Use same version as eth-ape
     ],
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_etherscan"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_etherscan": ["py.typed"]},
@@ -91,9 +93,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ape-etherscan-0.6.4/tests/conftest.py` & `ape-etherscan-0.6.5/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import os
 from io import StringIO
+from json import JSONDecodeError
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import IO, Any, Callable, Dict, Optional, Union
+from unittest.mock import MagicMock
 
 import _io  # type: ignore
 import ape
 import pytest
 from ape.api import ExplorerAPI
 from ape.exceptions import NetworkError
 from ape.logging import logger
@@ -37,15 +39,15 @@
     "startblock": None,
     "offset": 100,
     "page": 1,
     "sort": "asc",
 }
 FOO_SOURCE_CODE = """
 // SPDX-License-Identifier: AGPL-3.0
-pragma solidity ^0.8.2;
+pragma solidity ^0.8.20;
 
 import "@bar/bar.sol";
 
 library MyLib {
     function insert(uint value) public returns (bool) {
         return true;
     }
@@ -55,15 +57,15 @@
     function register(uint value) public {
         require(MyLib.insert(value));
     }
 }
 """
 BAR_SOURCE_CODE = r"""
 // SPDX-License-Identifier: AGPL-3.0
-pragma solidity ^0.8.2;
+pragma solidity ^0.8.20;
 
 contract bar {
 }
 """
 APE_CONFIG_FILE = r"""
 dependencies:
   - name: bar
@@ -213,15 +215,17 @@
         def get_url_f(testnet: bool = False, tld: str = "io"):
             f_str = f"https://api-{{}}.{{}}.{tld}/api" if testnet else f"https://api.{{}}.{tld}/api"
             return f_str.format
 
         url = get_url_f()
         testnet_url = get_url_f(testnet=True)
         com_url = get_url_f(tld="com")
+        org_url = get_url_f(tld="org")
         com_testnet_url = get_url_f(testnet=True, tld="com")
+        org_testnet_url = get_url_f(testnet=True, tld="org")
 
         return {
             "ethereum": {
                 "mainnet": url("etherscan"),
                 "goerli": testnet_url("goerli", "etherscan"),
                 "sepolia": testnet_url("sepolia", "etherscan"),
             },
@@ -237,14 +241,22 @@
                 "mainnet": testnet_url("optimistic", "etherscan"),
                 "goerli": testnet_url("goerli-optimistic", "etherscan"),
             },
             "polygon": {
                 "mainnet": com_url("polygonscan"),
                 "mumbai": com_testnet_url("testnet", "polygonscan"),
             },
+            "base": {
+                "goerli": org_testnet_url("goerli", "basescan"),
+                "mainnet": org_url("basescan"),
+            },
+            "polygon-zkevm": {
+                "mainnet": com_testnet_url("zkevm", "polygonscan"),
+                "goerli": com_testnet_url("testnet-zkevm", "polygonscan"),
+            },
             "avalanche": {"mainnet": url("snowtrace"), "fuji": testnet_url("testnet", "snowtrace")},
             "bsc": {
                 "mainnet": com_url("bscscan"),
                 "testnet": com_testnet_url("testnet", "bscscan"),
             },
         }
 
@@ -268,35 +280,47 @@
                 if key not in expected_params:
                     # Allow skipping certain assertions
                     continue
 
                 # Handler StringIO objects
                 if isinstance(val, StringIO):
                     assert isinstance(actual_params[key], StringIO)
-                    actual_json = json.loads(actual_params[key].read())
-                    expected_json = json.loads(val.read())
+                    text = actual_params[key].read()
+                    if text:
+                        try:
+                            actual_json = json.loads(text)
+                        except JSONDecodeError:
+                            pytest.fail(f"Response text is not JSON: '{text}'.")
+                            return
+                    else:
+                        # Empty.
+                        actual_json = {}
+
+                    val = val.read()
+                    expected_json = json.loads(val) if val else {}
                     assert actual_json == expected_json
 
                 else:
                     msg = f"expected={key}"
                     if params:
                         msg = f"{msg} module={params['module']} action={params['action']}"
 
                     assert actual_params[key] == val, msg
 
             if return_value:
                 return return_value
 
             elif side_effect:
-                return self.get_mock_response(side_effect())
+                result = side_effect()
+                return result if isinstance(result, Response) else self.get_mock_response(result)
 
         self._handlers[method.lower()][module] = handler
         self._session.request.side_effect = self.handle_request
 
-    def handle_request(self, method, base_uri, headers=None, params=None, data=None):
+    def handle_request(self, method, base_uri, timeout, headers=None, params=None, data=None):
         if params and "apikey" in params:
             del params["apikey"]
         if data and "apiKey" in data:
             del data["apiKey"]
 
         assert base_uri == self._expected_base_uri
 
@@ -307,28 +331,52 @@
         else:
             raise AssertionError("Expected either 'params' or 'data'.")
 
         handler = self._handlers[method.lower()][module]
         return handler(self, method, base_uri, headers=headers, params=params, data=data)
 
     def setup_mock_get_contract_type_response(self, file_name: str):
-        expected_address = CONTRACT_ADDRESS_MAP[file_name]
-        expected_params = {
-            "module": "contract",
-            "action": "getsourcecode",
-            "address": expected_address,
-        }
+        response = self._get_contract_type_response(file_name)
+        address = CONTRACT_ADDRESS_MAP[file_name]
+        expected_params = self._expected_get_ct_params(address)
+        self.add_handler("GET", "contract", expected_params, return_value=response)
+        response.expected_address = address
+        return response
+
+    def setup_mock_get_contract_type_response_with_throttling(
+        self, file_name: str, retries: int = 2
+    ):
+        response = self._get_contract_type_response(file_name)
+        address = CONTRACT_ADDRESS_MAP[file_name]
+        expected_params = self._expected_get_ct_params(address)
+        throttled = self._mocker.MagicMock(spec=Response)
+        throttled.status_code = 429
+
+        class ThrottleMock:
+            counter = 0
+
+            def side_effect(self):
+                if self.counter < retries:
+                    self.counter += 1
+                    return throttled
+
+                return response
+
+        throttler = ThrottleMock()
+        self.add_handler("GET", "contract", expected_params, side_effect=throttler.side_effect)
+        response.expected_address = address
+        return throttler, response
 
+    def _get_contract_type_response(self, file_name: str) -> Any:
         test_data_path = MOCK_RESPONSES_PATH / f"{file_name}.json"
         with open(test_data_path) as response_data_file:
-            response = self.get_mock_response(response_data_file, file_name=file_name)
+            return self.get_mock_response(response_data_file, file_name=file_name)
 
-        self.add_handler("GET", "contract", expected_params, return_value=response)
-        response.expected_address = expected_address
-        return response
+    def _expected_get_ct_params(self, address: str) -> Dict:
+        return {"module": "contract", "action": "getsourcecode", "address": address}
 
     def setup_mock_account_transactions_response(self, address: Optional[AddressType] = None):
         file_name = "get_account_transactions.json"
         test_data_path = MOCK_RESPONSES_PATH / file_name
 
         if address:
             params = EXPECTED_ACCOUNT_TXNS_PARAMS.copy()
@@ -338,35 +386,42 @@
 
         with open(test_data_path) as response_data_file:
             response = self.get_mock_response(response_data_file, file_name=file_name)
             self.add_handler("GET", "account", params, return_value=response)
             self.set_network("ethereum", "mainnet")
             return response
 
-    def get_mock_response(self, response_data: Union[IO, Dict, str], **kwargs):
+    def get_mock_response(
+        self, response_data: Optional[Union[IO, Dict, str, MagicMock]] = None, **kwargs
+    ):
         if isinstance(response_data, str):
             return self.get_mock_response({"result": response_data})
 
         elif isinstance(response_data, _io.TextIOWrapper):
             return self.get_mock_response(json.load(response_data), **kwargs)
 
+        elif isinstance(response_data, MagicMock):
+            # Mock wasn't set.
+            response_data = {}
+
         response = self._mocker.MagicMock(spec=Response)
         response.json.return_value = response_data
-        response.text = json.dumps(response_data)
+        response.text = json.dumps(response_data or {})
+
         response.status_code = 200
 
         for key, val in kwargs.items():
             setattr(response, key, val)
 
         return response
 
 
 @pytest.fixture
 def verification_params(address_to_verify):
-    ctor_args = "3133643932303665363338366532313839353566356166306565336362000000000000000000000000000000000000000000000000"  # noqa: E501
+    ctor_args = "00002833623465633162323163303133643932303665363338366532313839353566356166306565336362000000000000000000000000000000000000000000000000"  # noqa: E501
 
     return {
         "action": "verifysourcecode",
         "codeformat": "solidity-standard-json-input",
         "constructorArguements": ctor_args,
         "contractaddress": address_to_verify,
         "contractname": "foo.sol:foo",
```

### Comparing `ape-etherscan-0.6.4/tests/mock_responses/get_account_transactions.json` & `ape-etherscan-0.6.5/tests/mock_responses/get_account_transactions.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/tests/mock_responses/get_contract_response.json` & `ape-etherscan-0.6.5/tests/mock_responses/get_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/tests/mock_responses/get_proxy_contract_response.json` & `ape-etherscan-0.6.5/tests/mock_responses/get_proxy_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/tests/mock_responses/get_vyper_contract_response.json` & `ape-etherscan-0.6.5/tests/mock_responses/get_vyper_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.4/tests/test_etherscan.py` & `ape-etherscan-0.6.5/tests/test_etherscan.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,18 @@
         ("optimism", "mainnet-fork", "optimistic.etherscan.io"),
         ("optimism", "goerli", "goerli-optimism.etherscan.io"),
         ("optimism", "goerli-fork", "goerli-optimism.etherscan.io"),
         ("polygon", "mainnet", "polygonscan.com"),
         ("polygon", "mainnet-fork", "polygonscan.com"),
         ("polygon", "mumbai", "mumbai.polygonscan.com"),
         ("polygon", "mumbai-fork", "mumbai.polygonscan.com"),
+        ("polygon-zkevm", "mainnet", "zkevm.polygonscan.com"),
+        ("polygon-zkevm", "goerli", "testnet-zkevm.polygonscan.com"),
+        ("base", "mainnet", "basescan.org"),
+        ("base", "goerli", "goerli.basescan.org"),
         ("avalanche", "mainnet", "snowtrace.io"),
         ("avalanche", "fuji", "testnet.snowtrace.io"),
         ("bsc", "mainnet", "bscscan.com"),
         ("bsc", "mainnet-fork", "bscscan.com"),
         ("bsc", "testnet", "testnet.bscscan.com"),
         ("bsc", "testnet-fork", "testnet.bscscan.com"),
     ],
@@ -144,14 +148,30 @@
     #  to the parametrization.
     response = mock_backend.setup_mock_get_contract_type_response(file_name)
     actual = explorer.get_contract_type(response.expected_address).name
     expected = EXPECTED_CONTRACT_NAME_MAP[response.file_name]
     assert actual == expected
 
 
+def test_get_contract_type_with_rate_limiting(mock_backend, explorer):
+    """
+    This test ensures the rate limiting logic in the Etherscan client works.
+    """
+
+    file_name = "get_vyper_contract_response"
+    setter_upper = mock_backend.setup_mock_get_contract_type_response_with_throttling
+    throttler, response = setter_upper(file_name)
+
+    # We still eventually get the response.
+    actual = explorer.get_contract_type(response.expected_address).name
+    expected = EXPECTED_CONTRACT_NAME_MAP[response.file_name]
+    assert actual == expected
+    assert throttler.counter == 2  # Prove that it actually throttled.
+
+
 def test_get_account_transactions(mock_backend, account):
     mock_backend.setup_mock_account_transactions_response(account.address)
     query = AccountTransactionQuery(
         start_nonce=0, stop_nonce=0, columns=["txn_hash"], account=account.address
     )
     actual = next(account.query_manager.engines["etherscan"].perform_query(query)).txn_hash
     expected = "0x5780b43d819035ed1fa079171bdce7f0bbeaa6b01f201f8985d279a66cfc6844"
```

