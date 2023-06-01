# Comparing `tmp/resilient-48.2.4321.tar.gz` & `tmp/resilient-49.0.4423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient-48.2.4321.tar", last modified: Fri May  5 12:33:55 2023, max compression
+gzip compressed data, was "resilient-49.0.4423.tar", last modified: Thu Jun  1 15:58:22 2023, max compression
```

## Comparing `resilient-48.2.4321.tar` & `resilient-49.0.4423.tar`

### file list

```diff
@@ -1,65 +1,70 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8135 2023-05-05 12:33:36.000000 resilient-48.2.4321/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-05-05 12:33:55.543470 resilient-48.2.4321/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2023-05-05 12:33:36.000000 resilient-48.2.4321/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.539470 resilient-48.2.4321/co3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      377 2023-05-05 12:33:36.000000 resilient-48.2.4321/co3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 12:33:36.000000 resilient-48.2.4321/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.539470 resilient-48.2.4321/resilient/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/resilient/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/bin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/bin/finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/bin/gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/bin/res_keyring.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36857 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14360 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/co3argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36941 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1577 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/definitions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12719 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/resilient_rest_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/resilient.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1854 2023-05-05 12:33:55.547470 resilient-48.2.4321/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-05-05 12:33:36.000000 resilient-48.2.4321/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4241 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/shared_mock_data/mock_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_responses/session.JSON
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/.jwk/
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/API_KEY
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/EMAIL
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/EMPTY
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/PASSWORD
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/URL
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/template_test.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2812 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_co3_ii.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17968 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9003 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/xtest_gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/xtest_patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/xtest_res_keyring.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2023-05-05 12:33:36.000000 resilient-48.2.4321/tools/res_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      885 2023-05-05 12:33:36.000000 resilient-48.2.4321/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.933552 resilient-49.0.4423/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8556 2023-06-01 15:57:43.000000 resilient-49.0.4423/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-06-01 15:58:22.933552 resilient-49.0.4423/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2023-06-01 15:57:43.000000 resilient-49.0.4423/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.925552 resilient-49.0.4423/co3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      377 2023-06-01 15:57:43.000000 resilient-49.0.4423/co3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 resilient-49.0.4423/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/resilient/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11460 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/app_config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/resilient/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/bin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/bin/finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/bin/gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/bin/res_keyring.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36857 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12784 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/co3argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39318 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1758 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      854 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/definitions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17717 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2023-06-01 15:57:43.000000 resilient-49.0.4423/resilient/resilient_rest_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/resilient.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      379 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-06-01 15:58:22.000000 resilient-49.0.4423/resilient.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-06-01 15:58:22.933552 resilient-49.0.4423/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-06-01 15:57:43.000000 resilient-49.0.4423/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/tests/shared_mock_data/mock_plugins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_plugins/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_plugins/mock_plugins.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.929552 resilient-49.0.4423/tests/shared_mock_data/mock_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_responses/session.JSON
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.933552 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.933552 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/.jwk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/API_KEY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/EMAIL
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/EMPTY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/PASSWORD
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/shared_mock_data/mock_secrets/URL
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/template_test.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6071 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2812 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_co3_ii.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19399 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11144 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/xtest_gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/xtest_patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2023-06-01 15:57:43.000000 resilient-49.0.4423/tests/xtest_res_keyring.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:22.933552 resilient-49.0.4423/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2023-06-01 15:57:43.000000 resilient-49.0.4423/tools/res_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      933 2023-06-01 15:57:43.000000 resilient-49.0.4423/tox.ini
```

### Comparing `resilient-48.2.4321/CHANGES` & `resilient-49.0.4423/CHANGES`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+**2023-05: version 49.0**
+
+* Added logic to skip retry logic for failed API calls in :class:`resilient.SimpleClient.post() <resilient.co3.SimpleClient.post>`, :class:`resilient.SimpleClient.put() <resilient.co3.SimpleClient.put>` and :class:`resilient.SimpleClient.getput() <resilient.co3.SimpleClient.getput>`
+* Added ``resilient-app-config-plugins`` as a new package to manage third party credentials within SOAR apps
+
 **2023-05: version 48.2**
 
 * Update version of requests-toolbelt to v1.0 to support urllib3 v2.0
 
 **2023-04: version 48.1**
 
 * REST client updated to use ``include_permissions=false`` by default when authenticating to ``/rest/session`` endpoint.
```

### Comparing `resilient-48.2.4321/PKG-INFO` & `resilient-49.0.4423/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 48.2.4321
+Version: 49.0.4423
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-48.2.4321/README.md` & `resilient-49.0.4423/README.md`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/LICENSE` & `resilient-49.0.4423/resilient/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/__init__.py` & `resilient-49.0.4423/resilient/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/bin/finfo.py` & `resilient-49.0.4423/resilient/bin/finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/bin/gadget.py` & `resilient-49.0.4423/resilient/bin/gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/bin/res_keyring.py` & `resilient-49.0.4423/resilient/bin/res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/co3.py` & `resilient-49.0.4423/resilient/co3.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/co3argparse.py` & `resilient-49.0.4423/resilient/co3argparse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2019. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 """Command-line argument parser for Resilient apps"""
 
 import argparse
 import getpass
 import logging
 import os
 import sys
 
-import keyring
-from six import string_types
-
 from resilient import constants, helpers
+from resilient.app_config import AppConfigManager, ProtectedSecretsManager
 
 if sys.version_info.major == 2:
     from io import open
 
     from resilient import (ensure_unicode, get_proxy_dict,
                            get_resilient_circuits_version)
 else:
@@ -28,33 +26,14 @@
     import backports.configparser as configparser
 except ImportError:
     import configparser
 
 logger = logging.getLogger(__name__)
 
 
-class ConfigDict(dict):
-    """A dictionary, with property-based accessor
-
-    >>> opts = {"one": 1}
-    >>> cd = ConfigDict(opts)
-    >>> cd["one"]
-    1
-    >>> cd.one
-    1
-
-    """
-    def __getattr__(self, name):
-        """Attributes are made accessible as properties"""
-        try:
-            return self[name]
-        except KeyError:
-            raise AttributeError()
-
-
 class ArgumentParser(argparse.ArgumentParser):
     """Helper to parse common Resilient command line arguments.
 
     Optionally, arguments can be specified in a config file, section :samp:`[resilient]`.
 
     It is expected that a command line utility that needs to work with a Resilient
     server will create its own class that inherits this class.  Its `__init__`
@@ -129,14 +108,22 @@
         default_stomp_prefetch_limit = int(self.getopt("resilient", "stomp_prefetch_limit") or 20)
         default_resilient_mock = self.getopt("resilient", "resilient_mock")
 
         default_max_request_retries = self.getopt(constants.PACKAGE_NAME, constants.APP_CONFIG_REQUEST_MAX_RETRIES) or constants.APP_CONFIG_REQUEST_MAX_RETRIES_DEFAULT
         default_request_retry_delay = self.getopt(constants.PACKAGE_NAME, constants.APP_CONFIG_REQUEST_RETRY_DELAY) or constants.APP_CONFIG_REQUEST_RETRY_DELAY_DEFAULT
         default_request_retry_backoff = self.getopt(constants.PACKAGE_NAME, constants.APP_CONFIG_REQUEST_RETRY_BACKOFF) or constants.APP_CONFIG_REQUEST_RETRY_BACKOFF_DEFAULT
 
+        # PAM plugin configurations
+        if helpers.is_running_in_app_host(constants.ENV_VAR_APP_HOST_CONTAINER):
+            # no default in app host
+            default_pam_type = None
+        else:
+            # integration server defaults to Keyring
+            default_pam_type = self.getopt(constants.PACKAGE_NAME, constants.PAM_TYPE_CONFIG) or constants.PAM_DEFAULT_PAM_TYPE
+
         self.add_argument("--email",
                           default=default_email,
                           help="The email address to use to authenticate to the Resilient server.")
 
         self.add_argument("--password",
                           default=default_password,
                           help="WARNING:  This is an insecure option since the password "
@@ -217,14 +204,18 @@
                           help="Number of seconds to wait between retries. Defaults to 2")
 
         self.add_argument("--{0}".format(constants.APP_CONFIG_REQUEST_RETRY_BACKOFF),
                           type=int,
                           default=default_request_retry_backoff,
                           help="Multiplier applied to delay between retry attempts. Defaults to 2")
 
+        self.add_argument("--{0}".format(constants.PAM_TYPE_CONFIG),
+                          default=default_pam_type,
+                          help="PAM plugin type to use for pulling secrets. Defaults to Keyring")
+
         v_resc = get_resilient_circuits_version()
 
         # Having --resilient-mock here allows us to run unit tests for resilient-circuits and resilient-sdk
         # This argument will be added if:
         # - resilient-circuits is not installed
         # - resilient-circuits is installed and is > 34
         if not v_resc or (v_resc and v_resc.get("major") > 34):
@@ -255,16 +246,15 @@
         # Parse the known arguments
         args, argv = super(ArgumentParser, self).parse_known_args(args, namespace)
         return _post_process_args(args), argv
 
 
 def _post_process_args(args):
     # Post-process any options that reference keyring or environment variables
-    opts = parse_parameters(vars(args))
-    args = ConfigDict(opts)
+    args = AppConfigManager(vars(args))
 
     # Post-processing for other special options
     password = args.password
     email = args.email
 
     while (not password and email) and (not args.get("no_prompt_password")):
         password = getpass.getpass()
@@ -279,82 +269,23 @@
     if args.get("proxy_host"):
         args["proxy"] = get_proxy_dict(args)
 
     return args
 
 
 def parse_parameters(options):
-    """Given a dict that has configuration keys mapped to values,
+    """
+    Given a dict that has configuration keys mapped to values,
        - If a value begins with '^', redirect to fetch the value from
-         the secret key stored in the keyring.
-         The keyring service name is always just an underscore
-         (so keys must be unique in the whole options dict)
-       - If a value begins with '$', fetch the value from environment.
-
-    >>> opts = {
-    ...    "thing": u"value",
-    ...    "key3": "^val3",
-    ...    "key4": u"$val4",
-    ...    "key5": "$val5",
-    ...    "deep1": {"key1": "val1", "key2": u"^val2"}
-    ... }
-
-    >>> keyring.set_password("_", "val3", "key3password")
-    >>> keyring.set_password("_", "val2", "")
-    >>> keyring.set_password("deep1", "val2", "key2password")
-    >>> os.environ["val4"] = "key4param"
-    >>> os.environ["val5"] = "key5param"
-
-    >>> str(parse_parameters(opts)["key3"])
-    'key3password'
-
-    >>> parse_parameters(opts)["deep1"]["key1"]
-    'val1'
-
-    >>> str(parse_parameters(opts)["deep1"]["key2"])
-    'key2password'
-
-    >>> parse_parameters(opts)["deep1"]["key1"]
-    'val1'
-
-    >>> parse_parameters(opts)["key4"]
-    'key4param'
-
-    >>> parse_parameters(opts)["key5"]
-    'key5param'
-
+         the secret key stored in the plugin provided by pam_type.
+       - If a value begins with '$', fetch the value from environment or protected secret
     """
-    names = ()
-    return _parse_parameters(names, options)
-
-
-def _parse_parameters(names, options):
-    """Parse parameters, with a tuple of names for keyring context"""
-    for key in options.keys():
-        val = options[key]
-        if isinstance(val, dict):
-            val = _parse_parameters(names + (key,), val)
-        if isinstance(val, string_types) and len(val) > 1 and val[0] == "^":
-            # Decode a secret from the keystore
-            val = val[1:]
-            service = ".".join(names) or "_"
-            if service == "resilient":
-                # Special case, becuase of the way we parse commandlines, treat this as root
-                service = "_"
-            logger.debug("keyring get('%s', '%s')", service, val)
-            val = keyring.get_password(service, val)
 
-        if isinstance(val, string_types) and val.startswith(constants.PROTECTED_SECRET_PREFIX):
-            config_name = val[1:]
-
-            if helpers.protected_secret_exists(config_name, constants.PATH_SECRETS_DIR, constants.PATH_JWK_FILE):
-
-                protected_secret = helpers.get_protected_secret(config_name, constants.PATH_SECRETS_DIR, constants.PATH_JWK_FILE)
-
-                val = protected_secret if protected_secret else helpers.get_config_from_env(config_name)
-
-            else:
-                val = helpers.get_config_from_env(config_name)
+    plugin_type_str = helpers.get_pam_type_name(options, ProtectedSecretsManager())
+    plugin_type = helpers.load_pam_plugin(plugin_type_str) if plugin_type_str else None
 
-        options[key] = val
+    # though options is already an AppConfigManager object, the plugin_type was not available
+    # when the options object was initially created -- it was created with the default value.
+    # we need to recreate it with the new pam plugin
+    options = AppConfigManager(options, pam_plugin_type=plugin_type)
 
     return options
```

### Comparing `resilient-48.2.4321/resilient/co3base.py` & `resilient-49.0.4423/resilient/co3base.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,21 +43,19 @@
         self.poolmanager = PoolManager(num_pools=connections,
                                        maxsize=maxsize,
                                        block=block,
                                        ssl_version=ssl.PROTOCOL_TLS if sys.version_info.major == 2 else ssl.PROTOCOL_TLS_CLIENT)
 
 
 class BasicHTTPException(Exception):
-    """Exception for HTTP errors."""
     def __init__(self, response, err_reason=u"Unknown Reason", err_text=u"Unknown Error"):
         """
         Args:
           response - the Response object from the get/put/etc.
         """
-
         err_reason = response.reason if response.reason else err_reason
         err_text = response.text if response.text else err_text
 
         err_message = u"'resilient' API Request FAILED:\nResponse Code: {0}\nReason: {1}. {2}".format(response.status_code, err_reason, err_text)
 
         # Add a __qualname__ attribute if does not exist - needed for PY27
         if not hasattr(BasicHTTPException, "__qualname__"):
@@ -66,27 +64,67 @@
         super(BasicHTTPException, self).__init__(err_message)
 
         self.response = response
 
     def get_response(self):
         return self.response
 
+
+class RetryHTTPException(Exception):
+    """Exception for HTTP errors that should be retried."""
+    def __init__(self, response, err_reason=u"Unknown Reason", err_text=u"Unknown Error"):
+        """
+        Args:
+          response - the Response object from the get/put/etc.
+        """
+
+        err_reason = response.reason if response.reason else err_reason
+        err_text = response.text if response.text else err_text
+
+        err_message = u"'resilient' API Request Retry:\nResponse Code: {0}\nReason: {1}. {2}".format(response.status_code, err_reason, err_text)
+
+        # Add a __qualname__ attribute if does not exist - needed for PY27
+        if not hasattr(RetryHTTPException, "__qualname__"):
+            setattr(RetryHTTPException, "__qualname__", RetryHTTPException.__name__)
+
+        super(RetryHTTPException, self).__init__(err_message)
+
+        self.response = response
+
+    def get_response(self):
+        return self.response
+
     @staticmethod
-    def raise_if_error(response):
+    def raise_if_error(response, skip_retry=[]):
 
         if response.status_code == 401:
             try:
-                raise BasicHTTPException(response, err_reason=constants.ERROR_MSG_CONNECTION_UNAUTHORIZED, err_text=constants.ERROR_MSG_CONNECTION_INVALID_CREDS)
-            except BasicHTTPException:
+                raise RetryHTTPException(response, err_reason=constants.ERROR_MSG_CONNECTION_UNAUTHORIZED, err_text=constants.ERROR_MSG_CONNECTION_INVALID_CREDS)
+            except RetryHTTPException:
                 traceback.print_exc()
                 sys.exit(constants.ERROR_CODE_CONNECTION_UNAUTHORIZED)
 
-        elif response.status_code != 200:
-            raise BasicHTTPException(response)
-
+        elif response.status_code >= 300:
+            # these exceptions should not be retried
+            if response.status_code not in fix_list(skip_retry):
+                raise RetryHTTPException(response)
+            else:
+                raise BasicHTTPException(response)
+
+def fix_list(value):
+    """fix values to always use lists
+
+    :param value: value to test if not a list
+    :type value: list, int
+    :return: converted value if not a list
+    :rtype: list
+    """
+    if value == None:
+        return []
+    return value if isinstance(value, list) else [value]
 
 class NoChange(Exception):
     """
     Exception that can be raised within a get/put handler or a patch callback
     to indicate 'no change' (which then just bypasses the update operation).
     """
     pass
@@ -228,19 +266,19 @@
             r = self.session.get(u"{0}/rest/session?include_permissions={1}".format(self.base_url, "true" if include_permissions else "false"),
                                  auth=HTTPBasicAuth(self.api_key_id, self.api_key_secret),
                                  proxies=self.proxies,
                                  headers=self.make_headers(),
                                  verify=self.verify,
                                  timeout=timeout,
                                  cert=self.cert)
-            BasicHTTPException.raise_if_error(r)
+            RetryHTTPException.raise_if_error(r)
             return r
 
         response = retry_call(__set_api_key,
-                              exceptions=(BasicHTTPException, ConnectionError),
+                              exceptions=(RetryHTTPException, ConnectionError),
                               tries=self.max_connection_retries,
                               delay=self.request_retry_delay,
                               backoff=self.request_retry_backoff)
 
         session = json.loads(response.text)
         self._extract_org_id(session)
         self.api_key_handle = session.get("api_key_handle", None)
@@ -252,15 +290,15 @@
         Args:
           email - the email address to use for authentication.
           password - the password
           timeout - number of seconds to wait for response
         Returns:
           The Resilient session object (dict)
         Raises:
-          BasicHTTPException - if an HTTP exception occurs.
+          RetryHTTPException - if an HTTP exception occurs.
         """
         self.authdata = {
             u'email': ensure_unicode(email),
             u'password': ensure_unicode(password)
         }
         return self._connect(timeout=timeout)
 
@@ -343,19 +381,19 @@
                                   data=json.dumps(self.authdata),
                                   proxies=self.proxies,
                                   headers=self.make_headers(),
                                   verify=self.verify,
                                   timeout=timeout,
                                   cert=self.cert)
 
-            BasicHTTPException.raise_if_error(r)
+            RetryHTTPException.raise_if_error(r)
             return r
 
         response = retry_call(__connect,
-                              exceptions=(BasicHTTPException, ConnectionError),
+                              exceptions=(RetryHTTPException, ConnectionError),
                               tries=self.max_connection_retries,
                               delay=self.request_retry_delay,
                               backoff=self.request_retry_backoff)
 
         session = json.loads(response.text)
         self._extract_org_id(session)
 
@@ -401,30 +439,32 @@
             #
             self.session.cookies.clear()
 
         result = operation(url, **kwargs)
 
         return result
 
-    def get(self, uri, co3_context_token=None, timeout=None, is_uri_absolute=None, get_response_object=None):
+    def get(self, uri, co3_context_token=None, timeout=None, is_uri_absolute=None, get_response_object=None,
+            skip_retry=[]):
         """Gets the specified URI.  Note that this URI is relative to <base_url>/rest/orgs/<org_id>.  So
         for example, if you specify a uri of /incidents, the actual URL would be something like this:
 
             https://app.resilientsystems.com/rest/orgs/201/incidents
 
         Args:
           uri
           co3_context_token
           timeout: number of seconds to wait for response
           is_uri_absolute: if True, does not insert /org/{org_id} into the uri
           get_response_object: if True, returns the response object rather than the json of the response.text
+          skip_retry: list of HTTP responses to skip throwing an exception
         Returns:
           A dictionary, array, or response object with the value returned by the server.
         Raises:
-          BasicHTTPException - if an HTTP exception occurs.
+          RetryHTTPException - if an HTTP exception occurs.
         """
 
         if is_uri_absolute:
             url = u"{0}/rest{1}".format(self.base_url, ensure_unicode(uri))
 
         else:
             url = u"{0}/rest/orgs/{1}{2}".format(self.base_url, self.org_id, ensure_unicode(uri))
@@ -436,19 +476,19 @@
                                       url,
                                       proxies=self.proxies,
                                       cookies=self.cookies,
                                       headers=self.make_headers(co3_context_token),
                                       verify=self.verify,
                                       timeout=timeout,
                                       cert=self.cert)
-            BasicHTTPException.raise_if_error(r)
+            RetryHTTPException.raise_if_error(r, skip_retry=skip_retry)
             return r
 
         response = retry_call(__get,
-                              exceptions=(BasicHTTPException, ConnectionError),
+                              exceptions=(RetryHTTPException, ConnectionError),
                               tries=self.request_max_retries,
                               delay=self.request_retry_delay,
                               backoff=self.request_retry_backoff)
 
         if get_response_object:
             return response
 
@@ -476,61 +516,64 @@
         response = self._execute_request(self.session.get,
                                          url,
                                          proxies=self.proxies,
                                          cookies=self.cookies,
                                          headers=self.make_headers(co3_context_token),
                                          verify=self.verify,
                                          timeout=timeout)
-        BasicHTTPException.raise_if_error(response)
+        RetryHTTPException.raise_if_error(response)
         return response.json()
 
-    def get_content(self, uri, co3_context_token=None, timeout=None):
+    def get_content(self, uri, co3_context_token=None, timeout=None, skip_exceptions=[]):
         """Gets the specified URI.  Note that this URI is relative to <base_url>/rest/orgs/<org_id>.  So
         for example, if you specify a uri of /incidents, the actual URL would be something like this:
 
             https://app.resilientsystems.com/rest/orgs/201/incidents
 
         Args:
           uri
           co3_context_token
           timeout: number of seconds to wait for response
+          skip_retry: list of HTTP responses to skip throwing an exception
         Returns:
           The raw value returned by the server for this resource.
         Raises:
-          BasicHTTPException - if an HTTP exception occurs.
+          RetryHTTPException - if an HTTP exception occurs.
         """
         url = u"{0}/rest/orgs/{1}{2}".format(self.base_url, self.org_id, ensure_unicode(uri))
         response = self._execute_request(self.session.get,
                                          url,
                                          proxies=self.proxies,
                                          cookies=self.cookies,
                                          headers=self.make_headers(co3_context_token),
                                          verify=self.verify,
                                          timeout=timeout,
                                          cert=self.cert)
-        BasicHTTPException.raise_if_error(response)
+        RetryHTTPException.raise_if_error(response, skip_retry=skip_exceptions)
         return response.content
 
-    def post(self, uri, payload, co3_context_token=None, timeout=None, headers=None):
+    def post(self, uri, payload, co3_context_token=None, timeout=None, headers=None,
+             skip_retry=[]):
         """
         Posts to the specified URI.
         Note that this URI is relative to <base_url>/rest/orgs/<org_id>.  So for example, if you
         specify a uri of /incidents, the actual URL would be something like this:
 
             https://app.resilientsystems.com/rest/orgs/201/incidents
         Args:
            uri
            payload
            co3_context_token
            timeout: number of seconds to wait for response
            headers: optional headers to include
+           skip_retry: list of HTTP responses to skip throwing an exception
         Returns:
           A dictionary or array with the value returned by the server.
         Raises:
-          BasicHTTPException - if an HTTP exception occurs.
+          RetryHTTPException - if an HTTP exception occurs.
         """
         url = u"{0}/rest/orgs/{1}{2}".format(self.base_url, self.org_id, ensure_unicode(uri))
 
         # payloads which aren't convertable to json are passed asis
         payload_json = json.dumps(payload) if isinstance(payload, (list, dict)) else payload
 
         #----
@@ -542,49 +585,51 @@
                                       data=payload_json,
                                       proxies=self.proxies,
                                       cookies=self.cookies,
                                       headers=self.make_headers(co3_context_token, additional_headers=headers),
                                       verify=self.verify,
                                       timeout=timeout,
                                       cert=self.cert)
-            BasicHTTPException.raise_if_error(r)
+            RetryHTTPException.raise_if_error(r, skip_retry=skip_retry)
             return r
 
         response = retry_call(__post,
-                              exceptions=(BasicHTTPException, ConnectionError),
+                              exceptions=(RetryHTTPException, ConnectionError),
                               tries=self.request_max_retries,
                               delay=self.request_retry_delay,
                               backoff=self.request_retry_backoff)
 
-        BasicHTTPException.raise_if_error(response)
+        RetryHTTPException.raise_if_error(response, skip_retry=skip_retry)
         try:
             return json.loads(response.text)
         except json.decoder.JSONDecodeError:
             return response.content
 
     def post_attachment(self, uri, filepath,
                         filename=None,
                         mimetype=None,
                         data=None,
                         co3_context_token=None,
                         timeout=None,
-                        bytes_handle=None):
+                        bytes_handle=None,
+                        skip_retry=[]):
         """
         Upload a file to the specified URI
         e.g. "/incidents/<id>/attachments" (for incident attachments)
         or,  "/tasks/<id>/attachments" (for task attachments)
 
         :param uri: The REST URI for posting
         :param filepath:the path of the file to post or if ``None``, use ``bytes_handle``
         :param filename: optional name of the file when posted
         :param mimetype: optional override for the guessed MIME type
         :param data: optional dict with additional MIME parts (not required for file attachments; used in artifacts)
         :param co3_context_token: Action Module context token, if responding to an Action Module event
         :param timeout: optional timeout (seconds)
         :param bytes_handle: BytesIO handle for content, used if ``filepath`` is None
+        :param skip_retry: list of HTTP responses to skip throwing an exception
         """
         filepath = ensure_unicode(filepath)
         if filename:
             filename = ensure_unicode(filename)
         url = u"{0}/rest/orgs/{1}{2}".format(self.base_url, self.org_id, ensure_unicode(uri))
         mime_type = mimetype or mimetypes.guess_type(filename or filepath)[0] or "application/octet-stream"
 
@@ -600,70 +645,71 @@
                                       data=encoder,
                                       proxies=self.proxies,
                                       cookies=self.cookies,
                                       headers=headers,
                                       verify=self.verify,
                                       timeout=timeout,
                                       cert=self.cert)
-            BasicHTTPException.raise_if_error(r)
+            RetryHTTPException.raise_if_error(r, skip_retry=skip_retry)
             return json.loads(r.text)
 
         if filepath:
             with open(filepath, 'rb') as file_handle:
                 attachment_name = filename or os.path.basename(filepath)
                 json_resp = retry_call(__post_attachment,
                                        fkwargs={
                                            "name": attachment_name,
                                            "file_or_bytes_handle": file_handle,
                                            "extra_data": data
                                        },
-                                       exceptions=(BasicHTTPException, ConnectionError),
+                                       exceptions=(RetryHTTPException, ConnectionError),
                                        tries=self.request_max_retries,
                                        delay=self.request_retry_delay,
                                        backoff=self.request_retry_backoff)
                 return json_resp
 
         elif bytes_handle:
             attachment_name = filename if filename else "Unknown"
             json_resp = retry_call(__post_attachment,
                                    fkwargs={
                                        "name": attachment_name,
                                        "file_or_bytes_handle": bytes_handle,
                                        "extra_data": data
                                    },
-                                   exceptions=(BasicHTTPException, ConnectionError),
+                                   exceptions=(RetryHTTPException, ConnectionError),
                                    tries=self.request_max_retries,
                                    delay=self.request_retry_delay,
                                    backoff=self.request_retry_backoff)
             return json_resp
 
         else:
             raise ValueError("Either filepath or bytes_handle are required")
 
     def post_artifact_file(self, uri, artifact_type, artifact_filepath,
                            description=None,
                            value=None,
                            mimetype=None,
                            co3_context_token=None,
                            timeout=None,
-                           bytes_handle=None):
+                           bytes_handle=None,
+                           skip_retry=[]):
         """
         Post a file artifact to the specified URI
         e.g. "/incidents/<id>/artifacts/files"
 
         :param uri: The REST URI for posting
         :param artifact_type: the artifact type name ("IP Address", etc) or type ID
         :param artifact_filepath: the path of the file to post or ``None`` if using ``bytes_handle``
         :param description: optional description for the artifact
         :param value: optional value for the artifact
         :param mimetype: optional override for the guessed MIME type
         :param co3_context_token: Action Module context token, if responding to an Action Module event
         :param timeout: optional timeout (seconds)
         :param bytes_handle: byte content to create as an artifact file, used if ``artifact_filepath`` is ``None``
-
+        :param skip_retry: list of HTTP responses to skip throwing an exception
         """
         artifact = {
             "type": artifact_type,
             "value": value or "",
             "description": description or ""
         }
         mimedata = {
@@ -674,28 +720,28 @@
                                     filename=value if bytes_handle else None,
                                     mimetype=mimetype,
                                     data=mimedata,
                                     co3_context_token=co3_context_token,
                                     timeout=timeout,
                                     bytes_handle=bytes_handle)
 
-    def _get_put(self, uri, apply_func, co3_context_token=None, timeout=None):
+    def _get_put(self, uri, apply_func, co3_context_token=None, timeout=None, skip_retry=[]):
         """Internal helper to do a get/apply/put loop
         (for situations where the put might return a 409/conflict status code)
         """
         url = u"{0}/rest/orgs/{1}{2}".format(self.base_url, self.org_id, ensure_unicode(uri))
         response = self._execute_request(self.session.get,
                                          url,
                                          proxies=self.proxies,
                                          cookies=self.cookies,
                                          headers=self.make_headers(co3_context_token),
                                          verify=self.verify,
                                          timeout=timeout,
                                          cert=self.cert)
-        BasicHTTPException.raise_if_error(response)
+        RetryHTTPException.raise_if_error(response, skip_retry=skip_retry)
         payload = json.loads(response.text)
         try:
             apply_func(payload)
         except NoChange:
             return payload
         payload_json = json.dumps(payload)
         response = self._execute_request(self.session.put,
@@ -707,15 +753,15 @@
                                          verify=self.verify,
                                          timeout=timeout,
                                          cert=self.cert)
         if response.status_code == 200:
             return json.loads(response.text)
         if response.status_code == 409:
             return None
-        BasicHTTPException.raise_if_error(response)
+        RetryHTTPException.raise_if_error(response, skip_retry=skip_retry)
         return None
 
     def get_put(self, uri, apply_func, co3_context_token=None, timeout=None):
         """Performs a get, calls apply_func on the returned value, then calls self.put.
         If the put call returns a 409 error, then retry.
 
         Args:
@@ -732,58 +778,61 @@
         """
         while True:
             obj = self._get_put(uri, apply_func, co3_context_token=co3_context_token, timeout=timeout)
             if obj:
                 return obj
         return None
 
-    def put(self, uri, payload, co3_context_token=None, timeout=None, headers=None):
+    def put(self, uri, payload, co3_context_token=None, timeout=None, headers=None,
+            skip_retry=[]):
         """
         Puts to the specified URI.
         Note that this URI is relative to <base_url>/rest/orgs/<org_id>.  So for example, if you
         specify a uri of /incidents, the actual URL would be something like this:
 
             https://app.resilientsystems.com/rest/orgs/201/incidents
         Args:
            uri
            payload
            headers: optional headers to include
            co3_context_token
            timeout: number of seconds to wait for response
+           skip_retry: list of HTTP responses to skip throwing an exception
         Returns:
           A dictionary or array with the value returned by the server.
         Raises:
-          BasicHTTPException - if an HTTP exception occurs.
+          RetryHTTPException - if an HTTP exception occurs.
         """
         url = u"{0}/rest/orgs/{1}{2}".format(self.base_url, self.org_id, ensure_unicode(uri))
         # payloads which aren't convertable to json are passed asis
         payload_json = json.dumps(payload) if isinstance(payload, (list, dict)) else payload
         response = self._execute_request(self.session.put,
                                          url,
                                          data=payload_json,
                                          proxies=self.proxies,
                                          cookies=self.cookies,
                                          headers=self.make_headers(co3_context_token, additional_headers=headers),
                                          verify=self.verify,
                                          timeout=timeout,
                                          cert=self.cert)
-        BasicHTTPException.raise_if_error(response)
+        RetryHTTPException.raise_if_error(response, skip_retry=skip_retry)
         return json.loads(response.text)
 
-    def delete(self, uri, co3_context_token=None, timeout=None):
+    def delete(self, uri, co3_context_token=None, timeout=None, skip_retry=[]):
         """Deletes the specified URI.
 
         Args:
           uri
           co3_context_token
           timeout: number of seconds to wait for response
+          skip_retry: list of HTTP responses to skip throwing an exception
         Returns:
           A dictionary or array with the value returned by the server.
         Raises:
-          BasicHTTPException - if an HTTP exception occurs.
+          RetryHTTPException - if an HTTP exception occurs.
         """
         url = u"{0}/rest/orgs/{1}{2}".format(self.base_url, self.org_id, ensure_unicode(uri))
 
         # Wrap _execute_request and its related raise_if_error call in
         # inner function so we can add retry logic with dynamic parameters to it
         def __delete():
             r = self._execute_request(self.session.delete,
@@ -794,17 +843,17 @@
                                       verify=self.verify,
                                       timeout=timeout,
                                       cert=self.cert)
             if r.status_code == 204:
                 # 204 - No content is OK for a delete
                 return None
 
-            BasicHTTPException.raise_if_error(r)
+            RetryHTTPException.raise_if_error(r, skip_retry=skip_retry)
             return json.loads(r.text)
 
         response = retry_call(__delete,
-                              exceptions=(BasicHTTPException, ConnectionError),
+                              exceptions=(RetryHTTPException, ConnectionError),
                               tries=self.request_max_retries,
                               delay=self.request_retry_delay,
                               backoff=self.request_retry_backoff)
 
         return response
```

### Comparing `resilient-48.2.4321/resilient/co3sslutil.py` & `resilient-49.0.4423/resilient/co3sslutil.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/constants.py` & `resilient-49.0.4423/resilient/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2021. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 import os
 import pkg_resources
 
 PACKAGE_NAME = "resilient"
 
 ENV_HTTP_PROXY = "HTTP_PROXY"
 ENV_HTTPS_PROXY = "HTTPS_PROXY"
 ENV_NO_PROXY = "NO_PROXY"
 
 PROTECTED_SECRET_PREFIX = "$"
+PROTECTED_SECRET_PREFIX_WITH_BRACKET = "${"
 ALLOW_UNRECOGNIZED = False
 MIN_SUPPORTED_PY3_VERSION = (3, 6)
 
 # ENV Vars
 ENV_VAR_APP_HOST_CONTAINER = "APP_HOST_CONTAINER"
 
 # Headers
@@ -41,7 +42,12 @@
 APP_CONFIG_REQUEST_RETRY_BACKOFF = "request_retry_backoff"
 
 # app config default values
 APP_CONFIG_MAX_CONNECTION_RETRIES_DEFAULT = -1
 APP_CONFIG_REQUEST_MAX_RETRIES_DEFAULT = 5
 APP_CONFIG_REQUEST_RETRY_DELAY_DEFAULT = 2
 APP_CONFIG_REQUEST_RETRY_BACKOFF_DEFAULT = 2
+
+# PAM plugin constants
+PAM_TYPE_CONFIG = "pam_type"
+PAM_TYPE_CONFIG_APP_HOST_SECRET_NAME = "$PAM_TYPE"
+PAM_DEFAULT_PAM_TYPE = "Keyring"
```

### Comparing `resilient-48.2.4321/resilient/definitions.py` & `resilient-49.0.4423/resilient/definitions.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/helpers.py` & `resilient-49.0.4423/resilient/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2021. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 """Common Helper Functions for the resilient library"""
 
 import copy
+import inspect
 import io
 import json
 import logging
 import os
 import shutil
 import sys
 
+import resilient_app_config_plugins
+
 from resilient import constants
 
 if sys.version_info.major < 3:
     # Handle PY 2 specific imports
+    import imp  # deprecated version of 'importlib' required for Python 2
     from urllib import unquote
 
     from urlparse import urlparse
     JSONDecodeError = None  # JSONDecodeError is not available in PY2.7 so we set it to None
 else:
     # Handle PY 3 specific imports
+    import importlib.util
     from json.decoder import JSONDecodeError
     from urllib.parse import unquote, urlparse
-    from jwcrypto import jwk, jwe
+
+    from jwcrypto import jwe, jwk
 
 
 LOG = logging.getLogger(__name__)
 
 CHARS_TO_MASK = [("?", "%3F"), ("#", "%23"), ("/", "%2F")]
 MASK = "_*_{0}_*_"
 
@@ -261,15 +267,15 @@
     """
     Check to see if the APP_HOST_CONTAINER env var is set, the /etc/secrets directory,
     the SECRET_FILE with the encrypted token and the key.jwk file all exist and
     the user has the correct permissions to read them
 
     :param secret_name:  Name of the protected secret file
     :type secret_name: str
-    :param path_secrets_dir: Path to the location of the encrypted secret files, defaults to constants.PATH_SECRETS_DIR, defaults to constants.PATH_SECRETS_DIR
+    :param path_secrets_dir: Path to the location of the encrypted secret files, defaults to constants.PATH_SECRETS_DIR
     :type path_secrets_dir: str, optional
     :param path_jwk_file: Path to the location of the jwk.key file in a JSON format as per https://www.ietf.org/rfc/rfc7517.txt, defaults to constants.PATH_JWK_FILE
     :type path_jwk_file: str
     :return: True if all files are found and the user has the correct permission, False otherwise
     :rtype: bool
     """
     path_secret = os.path.join(path_secrets_dir, secret_name)
@@ -282,25 +288,38 @@
         return False
 
     if not os.path.isdir(path_secrets_dir) or not os.access(path_secrets_dir, os.R_OK):
         LOG.debug("Protected secrets directory at '%s' does not exist or you do not have the correct permissions. No value found for '%s'", path_secrets_dir, secret_name)
         return False
 
     if not os.path.isfile(path_secret) or not os.access(path_secret, os.R_OK):
-        LOG.warning("No protected secret found for '%s' or you do not have the correct permissions to read the file. No value found for '%s'", secret_name, secret_name)
         return False
 
     if not os.path.isfile(path_jwk_file) or not os.access(path_jwk_file, os.R_OK):
         LOG.warning("Could not find JWK at '%s' or you do not have the correct permissions. No value found for '%s'", path_jwk_file, secret_name)
         return False
 
     return True
 
 
-def get_protected_secret(secret_name, path_secrets_dir=constants.PATH_SECRETS_DIR, path_jwk_file=constants.PATH_JWK_FILE):
+def get_protected_secrets_keys(path_secrets_dir=constants.PATH_SECRETS_DIR):
+    """
+    Get a set of the secret keys in the given secrets directory
+
+    :param path_secrets_dir: Path to the location of the encrypted secret files, defaults to constants.PATH_SECRETS_DIR
+    :type path_secrets_dir: str, optional
+    :return: set of secret names
+    :rtype: set[str]
+    """
+    if not os.path.isdir(path_secrets_dir) or not os.access(path_secrets_dir, os.R_OK):
+        return []
+    return {f for f in os.listdir(path_secrets_dir) if os.path.isfile(os.path.join(path_secrets_dir, f))}
+
+
+def get_protected_secret_token_and_key(secret_name, path_secrets_dir=constants.PATH_SECRETS_DIR, path_jwk_file=constants.PATH_JWK_FILE):
     """
     Get the JWK, read the token from a file with
     the secret_name and decrypt it using the JWK
 
     :param secret_name: Name of the protected secret file
     :type secret_name: str
     :param path_secrets_dir: Path to the location of the encrypted secret files, defaults to constants.PATH_SECRETS_DIR
@@ -329,24 +348,15 @@
     if not tkn:
         LOG.error("File for protected secret '%s' is empty or corrupt", secret_name)
         return None
 
     # We need to remove new line and carriage return characters
     tkn = tkn.splitlines()[0]
 
-    try:
-        jwetoken = jwe.JWE()
-        jwetoken.deserialize(tkn)
-        jwetoken.decrypt(key)
-        decrypted_value = jwetoken.payload
-    except Exception as err:
-        LOG.error("Could not decrypt the secret. Invalid key used to decrypt the protected secret '%s'. Error Message: %s", secret_name, str(err))
-        return None
-
-    return decrypted_value.decode("utf-8")
+    return tkn, key
 
 
 def get_jwk(path_jwk_file=constants.PATH_JWK_FILE):
     """
     If the contents of the file at path is valid JSON,
     reads the file and uses the jwcrypto.jwk.JWK class
     get the JWK and returns it else returns None
@@ -382,33 +392,132 @@
 
     except Exception as err:
         LOG.error("Error getting JWK: %s", str(err))
         return None
 
     return aes_key
 
+def decrypt_protected_secret(token, key, secret_name):
+    """
+    Helper method to decrypt a secret given its encrypted value and decryption key.
+
+    NOTE: the decrypted value returned should not be logged to logs or persisted in
+    long lived memory if possible. It should be used in memory and then left to be
+    garbage collected whenever appropriate.
+
+    :param token: encrypted value of the secret
+    :type token: str
+    :param key: decryption key
+    :type key: str
+    :param secret_name: name of the secret to be decrypted. Ex: $MY_SECRET
+    :type secret_name: str
+    :return: plain-text decrypted value of the secret
+    :rtype: str
+    """
+    try:
+        jwetoken = jwe.JWE()
+        jwetoken.deserialize(token)
+        jwetoken.decrypt(key)
+        decrypted_value = jwetoken.payload
+    except Exception as err:
+        LOG.error("Could not decrypt the secret. Invalid key used to decrypt the protected secret '%s'. Error Message: %s", secret_name, str(err))
+        return None
+
+    return decrypted_value.decode("utf-8")
+
 
 def remove_secrets_dir(path_secrets_dir=constants.PATH_SECRETS_DIR):
     """
     Check if we running in App Host and if the secrets directory
     exists, remove it
 
     :param path_secrets_dir: Path to the location of the encrypted secret files, defaults to constants.PATH_SECRETS_DIR
     :type path_secrets_dir: str, optional
     """
     if is_running_in_app_host() and os.path.isdir(path_secrets_dir):
         LOG.debug("Removing secrets directory at: '%s'", path_secrets_dir)
         shutil.rmtree(path_secrets_dir, ignore_errors=True)
 
 
-def get_config_from_env(config_name):
+def get_config_from_env(config_name, default=None):
     """
     Read a variable from the environment given it's
     config_name. If it does not exist, it returns None
 
     :param config_name: Name of the env var to get
     :type config_name: str
+    :param default: default value to return if not found in env; defaults to None
+    :type default: str
     :return: The value of the env var
     :rtype: str
     """
     LOG.debug("Getting environmental variable '%s'", config_name)
-    return os.environ.get(config_name)
+    return os.environ.get(config_name, default)
+
+
+def get_pam_type_name(options, protected_secrets_manager):
+    """
+    Search protected secrets, app.config for PAM plugin type set by the user.
+    Order of hierarchy is:
+        1. The protected secret $PAM_TYPE is checked
+        2. if not found, pam_type is looked for in app.config
+            a. can be referenced by another secret like ``pam_type=$MY_PAM_TYPE``
+            b. or can be provided in plain text like ``pam_type=HashiCorpVault``
+
+    NOTE: this function returns a string indicating the plugin type name, without
+    validating that the given name is a valid plugin -- ``load_pam_plugin`` does the work of
+    validating the given plugin name
+
+    :param options: app configs
+    :type options: ``resilient.app_config.AppConfigManager``
+    :param protected_secrets_manager: Protected Secrets manager
+    :type protected_secrets_manager: ``resilient.app_config.ProtectedSecretsManager``
+    :return: string indicating the plugin's name
+    :rtype: str
+    """
+    return protected_secrets_manager.get(constants.PAM_TYPE_CONFIG_APP_HOST_SECRET_NAME) or protected_secrets_manager.get(options.get(constants.PAM_TYPE_CONFIG)) or options.get(constants.PAM_TYPE_CONFIG)
+
+
+def load_pam_plugin(plugin_type_str):
+    """
+    Validate the plugin given by name and return a "loaded" class type.
+    The plugin is loaded from resilient_app_config_plugins module.
+    The returned value from this function can be used to instantiate a Plugin.
+
+    **Example:**
+
+    .. code-block::python
+
+        plugin_type_str = "Keyring"
+        plugin_type = helpers.load_pam_plugin(plugin_type_str)
+
+        plugin_type() # instantiates a ``resilient_app_config_plugins.Keyring`` obj
+
+    :param plugin_type_str: string name of the plugin object
+        (must be subclass of ``resilient_app_config_plugins.plugin_base.PAMPluginInterface``)
+    :type plugin_type_str: string
+    :raises ValueError: if plugin is not found or not a subclass of ``resilient_app_config_plugins.plugin_base.PAMPluginInterface``
+    :return: class object of plugin which can then be used to instantiate an object of that plugin's class
+    :rtype: type(resilient_app_config_plugins.plugin_base.PAMPluginInterface)
+    """
+
+    # filter all classes found by inspecting the resilient.app_config_plugins module
+    # to only include subclass of the plugin interface (not including the interface)
+    # if a new plugin is created and is currently marked as invalid, check to make sure
+    # it is exposed in the app_config_plugins module (__init__.py)
+    valid_plugin_names = [a[0] for a in inspect.getmembers(resilient_app_config_plugins, inspect.isclass) \
+                        if issubclass(a[1], resilient_app_config_plugins.plugin_base.PAMPluginInterface) and a[1] != resilient_app_config_plugins.plugin_base.PAMPluginInterface]
+    if plugin_type_str not in valid_plugin_names:
+        raise ValueError("Given {0} '{1}' is invalid. {0} must be one of the valid PAM plugin types: {2}".format(
+            constants.PAM_TYPE_CONFIG, plugin_type_str, valid_plugin_names))
+    module = resilient_app_config_plugins
+
+    # get plugin class from module
+    plugin = getattr(module, plugin_type_str)
+
+    # all plugins must implement the abstract interface defined in PAMPluginInterface
+    # this is double checking that the given plugin does in fact implement the interface
+    if not issubclass(plugin, resilient_app_config_plugins.plugin_base.PAMPluginInterface):
+        raise ValueError("Given plugin '{0}' does not implement required interface: '{1}'".format(
+            plugin, resilient_app_config_plugins.plugin_base.PAMPluginInterface))
+
+    return plugin
```

### Comparing `resilient-48.2.4321/resilient/patch.py` & `resilient-49.0.4423/resilient/patch.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient/resilient_rest_mock.py` & `resilient-49.0.4423/resilient/resilient_rest_mock.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/resilient.egg-info/PKG-INFO` & `resilient-49.0.4423/resilient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 48.2.4321
+Version: 49.0.4423
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-48.2.4321/resilient.egg-info/SOURCES.txt` & `resilient-49.0.4423/resilient.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 co3/__init__.py
 resilient/LICENSE
 resilient/__init__.py
+resilient/app_config.py
 resilient/co3.py
 resilient/co3argparse.py
 resilient/co3base.py
 resilient/co3sslutil.py
 resilient/constants.py
 resilient/definitions.py
 resilient/helpers.py
@@ -26,25 +27,28 @@
 resilient/bin/finfo.py
 resilient/bin/gadget.py
 resilient/bin/res_keyring.py
 tests/__init__.py
 tests/conftest.py
 tests/helpers.py
 tests/template_test.json
+tests/test_app_config.py
 tests/test_co3.py
 tests/test_co3_ii.py
 tests/test_co3base.py
 tests/test_co3sslutil.py
 tests/test_finfo.py
 tests/test_helpers.py
 tests/xtest_gadget.py
 tests/xtest_patch.py
 tests/xtest_res_keyring.py
 tests/shared_mock_data/__init__.py
 tests/shared_mock_data/mock_paths.py
+tests/shared_mock_data/mock_plugins/__init__.py
+tests/shared_mock_data/mock_plugins/mock_plugins.py
 tests/shared_mock_data/mock_responses/session.JSON
 tests/shared_mock_data/mock_secrets/API_KEY
 tests/shared_mock_data/mock_secrets/EMAIL
 tests/shared_mock_data/mock_secrets/EMPTY
 tests/shared_mock_data/mock_secrets/PASSWORD
 tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
 tests/shared_mock_data/mock_secrets/URL
```

### Comparing `resilient-48.2.4321/setup.cfg` & `resilient-49.0.4423/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
+	resilient-app-config-plugins
+	
 	retry2            ~= 0.9
 	requests          ~= 2.27
 	requests-toolbelt ~= 1.0
 	six               ~= 1.16
 	
 	jwcrypto          ~= 1.4.0;  python_version >= "3.6"
```

### Comparing `resilient-48.2.4321/tests/conftest.py` & `resilient-49.0.4423/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2021. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 """
 Shared pytest fixtures
 
 Note:
     -   Code after the 'yield' statement in a fixture
         is ran after the test (or scope i.e. test session) has complete
@@ -26,15 +26,15 @@
 from resilient.co3base import BaseClient
 
 from tests.shared_mock_data import mock_paths
 
 
 def _mk_temp_dir():
     if os.path.exists(mock_paths.TEST_TEMP_DIR):
-        shutil.rmtree(mock_paths.TEST_TEMP_DIR)
+        shutil.rmtree(mock_paths.TEST_TEMP_DIR, ignore_errors=True)
 
     os.makedirs(mock_paths.TEST_TEMP_DIR)
 
 
 def _rm_temp_dir():
     if os.path.exists(mock_paths.TEST_TEMP_DIR):
         shutil.rmtree(mock_paths.TEST_TEMP_DIR, ignore_errors=True)
```

### Comparing `resilient-48.2.4321/tests/helpers.py` & `resilient-49.0.4423/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tests/shared_mock_data/mock_responses/session.JSON` & `resilient-49.0.4423/tests/shared_mock_data/mock_responses/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tests/test_co3.py` & `resilient-49.0.4423/tests/test_co3.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tests/test_co3_ii.py` & `resilient-49.0.4423/tests/test_co3_ii.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tests/test_co3base.py` & `resilient-49.0.4423/tests/test_co3base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 import os
 import sys
 
 import pytest
 from mock import patch
 from resilient import constants
-from resilient.co3base import BasicHTTPException
+from resilient.co3base import RetryHTTPException, BasicHTTPException
 
 from tests import helpers
 from tests.shared_mock_data import mock_paths
 
 
 def test_set_api_key_authorized(fx_base_client):
 
@@ -53,20 +53,19 @@
     base_client.max_connection_retries = 3
     base_client.request_retry_backoff = 1
     base_client.request_retry_delay = 1
 
     mock_uri = "{0}/rest/session".format(base_client.base_url)
     requests_adapter.register_uri('GET', mock_uri, status_code=300)
 
-    with pytest.raises(BasicHTTPException):
-        with patch("resilient.co3base.requests.Session.get") as mock_session_get:
-            base_client.set_api_key("123", "456")
+    with pytest.raises(RetryHTTPException):
+        base_client.set_api_key("123", "456")
 
     assert "retrying in 1 seconds" in caplog.text
-    assert mock_session_get.call_count == base_client.max_connection_retries
+    assert len(requests_adapter.request_history) == base_client.max_connection_retries
 
 
 def test_extract_org_id_cloud_account(fx_base_client):
     base_client = fx_base_client[0]
     base_client.org_name = "73c78395-470f-46a8-af7d-5e7d999a5707"
 
     mock_response = helpers.get_mock_response("session")
@@ -157,20 +156,19 @@
     base_client.max_connection_retries = 3
     base_client.request_retry_backoff = 1
     base_client.request_retry_delay = 1
 
     mock_uri = "{0}/rest/session".format(base_client.base_url)
     requests_adapter.register_uri("POST", mock_uri, status_code=300)
 
-    with pytest.raises(BasicHTTPException):
-        with patch("resilient.co3base.requests.Session.post") as mock_session_get:
-            base_client._connect()
+    with pytest.raises(RetryHTTPException):
+        base_client._connect()
 
     assert "retrying in 1 seconds" in caplog.text
-    assert mock_session_get.call_count == base_client.max_connection_retries
+    assert len(requests_adapter.request_history) == base_client.max_connection_retries
 
 
 def test_get(fx_base_client):
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
     incident_id = 1001
 
@@ -189,19 +187,34 @@
     base_client.request_max_retries = 2
     base_client.request_retry_backoff = 1
     base_client.request_retry_delay = 1
 
     mock_uri = '{0}/rest/orgs/{1}/incidents/{2}'.format(base_client.base_url, base_client.org_id, 1001)
     requests_adapter.register_uri('GET', mock_uri, status_code=300)
 
-    with pytest.raises(BasicHTTPException, match=r"Response Code: 300"):
+    with pytest.raises(RetryHTTPException, match=r"Response Code: 300"):
         base_client.get("/incidents/1001")
 
     assert "retrying in 1 seconds" in caplog.text
 
+def test_get_retry_skip(fx_base_client, caplog):
+    base_client = fx_base_client[0]
+    requests_adapter = fx_base_client[1]
+
+    base_client.request_max_retries = 2
+    base_client.request_retry_backoff = 1
+    base_client.request_retry_delay = 1
+
+    mock_uri = '{0}/rest/orgs/{1}/incidents/{2}'.format(base_client.base_url, base_client.org_id, 1001)
+    requests_adapter.register_uri('GET', mock_uri, status_code=404)
+
+    with pytest.raises(BasicHTTPException, match=r"Response Code: 404"):
+        base_client.get("/incidents/1001", skip_retry=[404])
+
+
 
 def test_get_const(fx_base_client):
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
 
     mock_uri = '{0}/rest/const'.format(base_client.base_url)
     mock_response = {"server_version": {"major": 47, "minor": 0, "build_number": 8304, "version": "47.0.8304"}}
@@ -231,19 +244,40 @@
     base_client.request_max_retries = 2
     base_client.request_retry_backoff = 1
     base_client.request_retry_delay = 1
 
     mock_uri = '{0}/rest/orgs/{1}/incidents/{2}'.format(base_client.base_url, base_client.org_id, 1001)
     requests_adapter.register_uri('POST', mock_uri, status_code=300)
 
-    with pytest.raises(BasicHTTPException, match=r"Response Code: 300"):
+    with pytest.raises(RetryHTTPException, match=r"Response Code: 300"):
         base_client.post("/incidents/1001", {"incident_name": "Mock Incident"})
 
     assert "retrying in 1 seconds" in caplog.text
 
+    # test skip which isn't part of the list
+    with pytest.raises(RetryHTTPException, match=r"Response Code: 300"):
+        base_client.post("/incidents/1001", {"incident_name": "Mock Incident"}, skip_retry=404)
+
+def test_post_retry_skip(fx_base_client, caplog):
+    base_client = fx_base_client[0]
+    requests_adapter = fx_base_client[1]
+
+    base_client.request_max_retries = 2
+    base_client.request_retry_backoff = 1
+    base_client.request_retry_delay = 1
+
+    mock_uri = '{0}/rest/orgs/{1}/incidents/{2}'.format(base_client.base_url, base_client.org_id, 1001)
+    requests_adapter.register_uri('POST', mock_uri, status_code=404)
+
+    with pytest.raises(BasicHTTPException, match=r"Response Code: 404"):
+        base_client.post("/incidents/1001", {"incident_name": "Mock Incident"}, skip_retry=[404, 410])
+
+    # single value
+    with pytest.raises(BasicHTTPException, match=r"Response Code: 404"):
+        base_client.post("/incidents/1001", {"incident_name": "Mock Incident"}, skip_retry=404)
 
 def test_client_has_base_headers(fx_base_client):
     base_client = fx_base_client[0]
     headers = base_client.headers
 
     assert headers.get("content-type") == "application/json"
     assert headers.get(constants.HEADER_MODULE_VER_KEY) == constants.HEADER_MODULE_VER_VALUE
@@ -503,15 +537,15 @@
     mock_uri = '{0}/rest/orgs/{1}/incidents/{2}/attachments'.format(base_client.base_url, base_client.org_id, incident_id)
     requests_adapter.register_uri('POST', mock_uri, status_code=300)
 
     uri = "/incidents/{0}/attachments".format(incident_id)
     temp_file_name = "mock_attachment.txt"
     bytes_handle = io.BytesIO(b"these are mock bytes")
 
-    with pytest.raises(BasicHTTPException, match=r"Response Code: 300"):
+    with pytest.raises(RetryHTTPException, match=r"Response Code: 300"):
         base_client.post_attachment(
             uri=uri,
             filepath=None,
             filename=temp_file_name,
             bytes_handle=bytes_handle
         )
 
@@ -550,11 +584,11 @@
     base_client.request_max_retries = 2
     base_client.request_retry_backoff = 1
     base_client.request_retry_delay = 1
 
     mock_uri = '{0}/rest/orgs/{1}/incidents/{2}'.format(base_client.base_url, base_client.org_id, 1001)
     requests_adapter.register_uri('DELETE', mock_uri, status_code=300)
 
-    with pytest.raises(BasicHTTPException, match=r"Response Code: 300"):
+    with pytest.raises(RetryHTTPException, match=r"Response Code: 300"):
         base_client.delete("/incidents/1001")
 
     assert "retrying in 1 seconds" in caplog.text
```

### Comparing `resilient-48.2.4321/tests/test_finfo.py` & `resilient-49.0.4423/tests/test_finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tests/test_helpers.py` & `resilient-49.0.4423/tests/test_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2010, 2021. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2023. All Rights Reserved.
 
 import logging
 import os
 import sys
 
 import pytest
-from resilient import constants, helpers
+from resilient import constants, helpers, app_config
 
 if sys.version_info.major >= 3:
     # Handle PY 3 specific imports
     from jwcrypto.jwk import JWK
 
 
 def test_str_to_bool():
@@ -101,15 +101,17 @@
 
 
 def test_is_running_in_app_host(fx_reset_environmental_variables):
     os.environ[constants.ENV_VAR_APP_HOST_CONTAINER] = "1"
     assert helpers.is_running_in_app_host() is True
 
 
-def test_is_not_running_in_app_host(caplog):
+def test_is_not_running_in_app_host(caplog, fx_reset_environmental_variables):
+    if constants.ENV_VAR_APP_HOST_CONTAINER in os.environ:
+        del os.environ[constants.ENV_VAR_APP_HOST_CONTAINER]
     caplog.set_level(logging.DEBUG)
     assert helpers.is_running_in_app_host() is False
     assert "Not running in an App Host environment" in caplog.text
 
 
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY3_VERSION, reason="requires python3.6 or higher")
 def test_protected_secret_exists(fx_write_protected_secrets, fx_reset_environmental_variables):
@@ -128,51 +130,68 @@
 
     os.environ[constants.ENV_VAR_APP_HOST_CONTAINER] = "1"
     assert helpers.protected_secret_exists("API_KEY", "mock_path", "mock_path") is False
     assert "Protected secrets are only Python >= 3 supported" in caplog.text
 
 
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY3_VERSION, reason="requires python3.6 or higher")
-def test_protected_secret_exists_env_var_not_set(fx_write_protected_secrets):
+def test_protected_secret_exists_env_var_not_set(fx_write_protected_secrets, fx_reset_environmental_variables):
     path_secrets_dir = fx_write_protected_secrets
     path_jwk_file = os.path.join(path_secrets_dir, ".jwk", "key.jwk")
 
+    if constants.ENV_VAR_APP_HOST_CONTAINER in os.environ:
+        del os.environ[constants.ENV_VAR_APP_HOST_CONTAINER]
     assert helpers.protected_secret_exists("API_KEY", path_secrets_dir, path_jwk_file) is False
 
 
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY3_VERSION, reason="requires python3.6 or higher")
+def test_get_protected_secrets_keys(fx_write_protected_secrets, caplog, fx_reset_environmental_variables):
+    path_secrets_dir = fx_write_protected_secrets
+
+    expected_list = {"API_KEY", "EMAIL", "EMPTY", "PASSWORD", "PASSWORD_WITH_SPECIAL_CHARS", "URL"}
+    keys_list = helpers.get_protected_secrets_keys(path_secrets_dir)
+
+    assert isinstance(keys_list, set)
+    assert expected_list == keys_list
+
+@pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY3_VERSION, reason="requires python3.6 or higher")
 def test_get_protected_secret(fx_write_protected_secrets, caplog):
     path_secrets_dir = fx_write_protected_secrets
     path_jwk_file = os.path.join(path_secrets_dir, ".jwk", "key.jwk")
 
-    assert helpers.get_protected_secret("API_KEY", path_secrets_dir, path_jwk_file) == "JbkOxTInUg1aIRGxXI8zOG1A25opU39lDKP1_0rfeVQ"
+    token, key = helpers.get_protected_secret_token_and_key("API_KEY", path_secrets_dir, path_jwk_file)
+    assert token and key
+
+    assert helpers.decrypt_protected_secret(token, key, "API_KEY") == "JbkOxTInUg1aIRGxXI8zOG1A25opU39lDKP1_0rfeVQ"
 
 
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY3_VERSION, reason="requires python3.6 or higher")
 def test_get_protected_secret_empty_file(fx_write_protected_secrets, caplog):
     path_secrets_dir = fx_write_protected_secrets
     path_jwk_file = os.path.join(path_secrets_dir, ".jwk", "key.jwk")
 
-    assert helpers.get_protected_secret("EMPTY", path_secrets_dir, path_jwk_file) is None
+    assert helpers.get_protected_secret_token_and_key("EMPTY", path_secrets_dir, path_jwk_file) is None
     assert "File for protected secret 'EMPTY' is empty or corrupt" in caplog.text
 
 
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY3_VERSION, reason="requires python3.6 or higher")
 def test_get_protected_secret_wrong_key(fx_write_protected_secrets, caplog):
     path_secrets_dir = fx_write_protected_secrets
     path_jwk_file = os.path.join(path_secrets_dir, ".jwk", "key_unused.jwk")
 
-    assert helpers.get_protected_secret("API_KEY", path_secrets_dir, path_jwk_file) is None
+    token, key = helpers.get_protected_secret_token_and_key("API_KEY", path_secrets_dir, path_jwk_file)
+
+    assert helpers.decrypt_protected_secret(token, key, "API_KEY") is None
     assert "Could not decrypt the secret. Invalid key used to decrypt the protected secret 'API_KEY'." in caplog.text
 
 
 @pytest.mark.skipif(sys.version_info >= constants.MIN_SUPPORTED_PY3_VERSION, reason="only run this test in Python 2.7")
 def test_get_protected_secret_unsupported_python_version(caplog):
 
-    assert helpers.get_protected_secret("API_KEY", "mock_path", "mock_path") is None
+    assert helpers.get_protected_secret_token_and_key("API_KEY", "mock_path", "mock_path") is None
     assert "Protected secrets are only Python >= 3 supported" in caplog.text
 
 
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY3_VERSION, reason="requires python3.6 or higher")
 def test_get_jwk(fx_write_protected_secrets):
     path_secrets_dir = fx_write_protected_secrets
     path_jwk_file = os.path.join(path_secrets_dir, ".jwk", "key.jwk")
@@ -199,7 +218,33 @@
     assert "Could not find JWK at 'invalid_path' or you do not have the correct permissions." in caplog.text
 
 
 def test_get_config_from_env(fx_reset_environmental_variables):
     os.environ[constants.ENV_VAR_APP_HOST_CONTAINER] = "1"
     assert helpers.get_config_from_env(constants.ENV_VAR_APP_HOST_CONTAINER) == "1"
     assert helpers.get_config_from_env("invalid_env_var") is None
+
+
+def test_load_pam_plugin_success_builtin():
+    plugin_name = "Keyring"
+    plugin = helpers.load_pam_plugin(plugin_name)
+
+    assert plugin.__name__ == "Keyring"
+
+def test_get_pam_type_name(fx_reset_environmental_variables, fx_write_protected_secrets):
+    path_secrets_dir = fx_write_protected_secrets
+    path_jwk_file = os.path.join(path_secrets_dir, ".jwk", "key.jwk")
+    protected_secrets_manager = app_config.ProtectedSecretsManager(path_secrets_dir, path_jwk_file)
+
+    opts = {"pam_type": None}
+    assert helpers.get_pam_type_name(opts, protected_secrets_manager) == None
+
+    opts = {"pam_type": "HashiCorpVault_Custom"}
+    assert helpers.get_pam_type_name(opts, protected_secrets_manager) == "HashiCorpVault_Custom"
+
+    os.environ["MY_PAM"] = "Keyring"
+    opts = {"pam_type": "$MY_PAM"}
+    assert helpers.get_pam_type_name(opts, protected_secrets_manager) == "Keyring"
+
+    os.environ["PAM_TYPE"] = "HigherPrecedence"
+    opts = {"pam_type": "LowerPrecedence"}
+    assert helpers.get_pam_type_name(opts, protected_secrets_manager) == "HigherPrecedence"
```

### Comparing `resilient-48.2.4321/tests/xtest_gadget.py` & `resilient-49.0.4423/tests/xtest_gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tests/xtest_patch.py` & `resilient-49.0.4423/tests/xtest_patch.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tests/xtest_res_keyring.py` & `resilient-49.0.4423/tests/xtest_res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tools/res_utils.py` & `resilient-49.0.4423/tools/res_utils.py`

 * *Files identical despite different names*

### Comparing `resilient-48.2.4321/tox.ini` & `resilient-49.0.4423/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     requests-mock ~= 1.9
     setuptools-scm<6.0.0 ; python_version=="2.7"
 
 setenv = 
     SETUPTOOLS_SCM_PRETEND_VERSION={env:SETUPTOOLS_SCM_PRETEND_VERSION}
 
 commands = 
+    pip install ../resilient-app-config-plugins
     pip install .
     pytest --cov --cov-report xml --capture=no -s {posargs} tests/ --durations=0
 
 [coverage:run]
 source=resilient
 
 [coverage:report]
```

