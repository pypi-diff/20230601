# Comparing `tmp/resilient_lib-48.2.4321.tar.gz` & `tmp/resilient_lib-49.0.4423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_lib-48.2.4321.tar", last modified: Fri May  5 12:34:56 2023, max compression
+gzip compressed data, was "resilient_lib-49.0.4423.tar", last modified: Thu Jun  1 15:58:36 2023, max compression
```

## Comparing `resilient_lib-48.2.4321.tar` & `resilient_lib-49.0.4423.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6221 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/function_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      573 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/integration_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26850 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/poller_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19335 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/requests_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24255 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/resilient_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/templates_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/workflow_status.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5694 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/tab.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      410 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/util/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/data/default_template.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/data/override_template.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/shared_mock_data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/cert.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/key.open.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_payload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12012 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_poller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31154 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_requests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/tests/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5394 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/test_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/test_permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/test_tab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      933 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6305 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.425552 resilient_lib-49.0.4423/resilient_lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      871 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/resilient_lib/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/function_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      573 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/integration_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30035 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/poller_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19335 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/requests_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24321 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/resilient_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/templates_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/components/workflow_status.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/resilient_lib/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5694 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/ui/tab.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/resilient_lib/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      410 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/resilient_lib/util/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.425552 resilient_lib-49.0.4423/resilient_lib.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-06-01 15:58:36.000000 resilient_lib-49.0.4423/resilient_lib.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2023-06-01 15:58:36.433552 resilient_lib-49.0.4423/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      119 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/data/default_template.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/data/override_template.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/shared_mock_data/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/cert.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/key.open.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_payload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13935 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_poller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31154 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_requests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:58:36.429552 resilient_lib-49.0.4423/tests/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5394 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/test_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/test_permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tests/ui/test_tab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      981 2023-06-01 15:57:43.000000 resilient_lib-49.0.4423/tox.ini
```

### Comparing `resilient_lib-48.2.4321/CHANGES` & `resilient_lib-49.0.4423/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2023-05: version 49.0**
+
+* Added new functions for pollers to interact with SOAR
+
 **2023-04: version 48.1**
 
 * Updated SOAR case default filters for poller helper methods
 
 **2023-02: version 48.0**
 
 * Added support for ``verify`` config in app.config when using
```

### Comparing `resilient_lib-48.2.4321/PKG-INFO` & `resilient_lib-49.0.4423/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_lib
-Version: 48.2.4321
+Version: 49.0.4423
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-48.2.4321/README.md` & `resilient_lib-49.0.4423/README.md`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/__init__.py` & `resilient_lib-49.0.4423/resilient_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/function_metrics.py` & `resilient_lib-49.0.4423/resilient_lib/components/function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/function_result.py` & `resilient_lib-49.0.4423/resilient_lib/components/function_result.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/html2markdown.py` & `resilient_lib-49.0.4423/resilient_lib/components/html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/integration_errors.py` & `resilient_lib-49.0.4423/resilient_lib/components/integration_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/oauth2_client_credentials_session.py` & `resilient_lib-49.0.4423/resilient_lib/components/oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/poller_common.py` & `resilient_lib-49.0.4423/resilient_lib/components/poller_common.py`

 * *Files 7% similar despite different names*

```diff
@@ -394,14 +394,70 @@
             result = self._patch_case(case_id, case_payload)
             return result
 
         except Exception as err:
             LOG.error(str(err))
             raise_from(IntegrationError("update_soar_case failed to update case in SOAR"), err)
 
+    def update_soar_cases(self, payload):
+        """
+        Update mulitple IBM SOAR cases (usually from a rendered Jinja template).
+
+        **Example:**
+
+        .. code-block:: python
+
+            payload = {
+                "patches": {
+                    "incidentID1": {
+                        "changes": [
+                            {
+                                "field": {"name": "incident_field_name"},
+                                "old_value": {"field_type": "current_value"},
+                                "new_value": {"field_type": "new_value"}
+                            },
+                            {
+                                "field": {"name": "incident_field_name"},
+                                "old_value": {"id": 1},
+                                "new_value": {"id": 2}
+                            }
+                        ],
+                        "version": 12345 #Current version + 1
+                    },
+                    "2315": {
+                        "changes": [
+                            {
+                                "field": {"name": "start_date"},
+                                "old_value": {"date": None},
+                                "new_value": {"date": 1681753245000}
+                            },
+                            {
+                                "field": {"name": "zip"},
+                                "old_value": {"text": None},
+                                "new_value": {"text": "14294"}
+                            }
+                        ],
+                        "version": 14
+                    }
+                }
+            }
+
+        :param payload: Dictionary that contains changes to make to SOAR cases
+        :type payload: dict
+        :return: Dictionary of failures if any occur
+        :rtype: dict
+        """
+        try:
+            result = self.rest_client.put("/incidents/patch", payload)
+        except Exception as err:
+            LOG.error(str(err))
+            raise_from(IntegrationError("update_soar_cases failed to update cases in SOAR"), err)
+
+        return result
+
     def create_case_comment(self, case_id, note, entity_comment_id=None, entity_comment_header=None):
         """
         Add a comment to the specified SOAR case by ID.
 
         :param case_id: SOAR case ID
         :type case_id: str|int
         :param note: Content to be added as a note to the case
@@ -598,14 +654,37 @@
         # get the SOAR case comments and capture only the text
         soar_comments = self.get_case_comments(str(case_id))
         soar_comment_list = [comment['text'] for comment in soar_comments]
 
         # filter entity comments with our SOAR header
         return self._filter_comments(soar_comment_list, entity_comments, filter_soar_header=soar_header)
 
+    def get_case_tasks(self, case_id, want_layouts=False, want_notes=False, handle_format="names"):
+        """
+        Get all the tasks from a SOAR case
+
+        :param case_id: IBM SOAR case id
+        :type case_id: str|int
+        :param want_layouts: If the task layout should be returned. Default is False.
+        :type want_layouts: bool
+        :param want_notes: If the task notes should be returned. Default is False.
+        :type want_notes: bool
+        :param handle_format: The format to return can be names, ids, or objects. Default is names.
+        :type handle_format: str
+        :return: A list of all the tasks for the given SOAR case
+        :rtype: list
+        """
+        uri = "/incidents/{}/tasks?want_layouts={}&want_notes={}&handle_format={}".format(case_id, want_layouts, want_notes, handle_format)
+        try:
+            tasks = self.rest_client.get(uri=uri)
+        except Exception as err:
+            LOG.error(str(err))
+            raise_from(IntegrationError("get_case_tasks failed to get SOAR case tasks"), err)
+
+        return tasks
 
 @cached(cache=LRUCache(maxsize=100))
 def eval_mapping(eval_value, wrapper=None):
     """
     Map a JSON string to a python object. Safely evaluates the values with the use
     of ``ast.literal_eval`` and can ONLY convert to a list or a dictionary.
```

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/requests_common.py` & `resilient_lib-49.0.4423/resilient_lib/components/requests_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/resilient_common.py` & `resilient_lib-49.0.4423/resilient_lib/components/resilient_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# (c) Copyright IBM Corp. 2018. All Rights Reserved.
+# (c) Copyright IBM Corp. 2023. All Rights Reserved.
 # pragma pylint: disable=unused-argument, no-self-use
 
 import datetime
 import io
 import logging
 import mimetypes
 import os
@@ -233,15 +233,14 @@
     :raises ValueError: if a field is missing
     :return: a Dictionary of all fields with Select/Multi-Select fields handled.
     :rtype: dict
     """
 
     mandatory_fields = field_list
     provided_fields = kwargs
-    return_fields = {}
     mandatory_err_msg = "'{0}' is mandatory and is not set. You must set this value to run this function"
 
     # This is needed to handle something like: validate_fields(('incident_id'), kwargs)
     # In this case field_list will be a string and not a tuple
     if isinstance(mandatory_fields, string_types):
         mandatory_fields = [mandatory_fields]
 
@@ -260,45 +259,47 @@
         placeholder_value = None
 
         if isinstance(field, dict):
             placeholder_value = field.get("placeholder")
             field = field.get("name")
 
         # If the field value is a defined empty str, raise an error
-        if isinstance(provided_fields.get(field), string_types):
-            if not provided_fields.get(field):
-                raise ValueError(mandatory_err_msg.format(field))
+        field_value = provided_fields.get(field)
+        if isinstance(field_value, string_types) and not field_value:
+            raise ValueError(mandatory_err_msg.format(field))
 
-        if provided_fields.get(field) is None:
+        if field_value is None:
             raise ValueError(mandatory_err_msg.format(field))
 
-        if placeholder_value and provided_fields.get(field) == placeholder_value:
+        if placeholder_value and field_value == placeholder_value:
             raise ValueError(
                 "'{0}' is mandatory and still has its placeholder value of '{1}'. You must set this value correctly to run this function".format(
                     field, placeholder_value))
 
     # Loop provided fields and get their value
     for field_name, field_value in provided_fields.items():
 
         # Handle if Select Function Input type
         if isinstance(field_value, dict) and field_value.get("name"):
             field_value = field_value.get("name")
+            provided_fields[field_name] = field_value
 
         # Handle if 'Text with value string Input' type
         elif isinstance(field_value, dict) and field_value.get("content"):
             field_value = field_value.get("content")
+            provided_fields[field_name] = field_value
 
         # Handle if Multi-Select Function Input type
         # There is a chance the list has already been "normalized", so just append as is
         elif isinstance(field_value, list):
             field_value = [f.get("name") if isinstance(f, dict) else f for f in field_value]
 
-        return_fields[field_name] = field_value
+            provided_fields[field_name] = field_value
 
-    return return_fields
+    return provided_fields
 
 
 def get_file_attachment(res_client, incident_id, artifact_id=None, task_id=None, attachment_id=None):
     """
     Call the SOAR REST API to get the attachment or artifact data for
     an Incident or a Task
```

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/templates_common.py` & `resilient_lib-49.0.4423/resilient_lib/components/templates_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/components/workflow_status.py` & `resilient_lib-49.0.4423/resilient_lib/components/workflow_status.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/ui/common.py` & `resilient_lib-49.0.4423/resilient_lib/ui/common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/ui/conditions.py` & `resilient_lib-49.0.4423/resilient_lib/ui/conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/ui/elements.py` & `resilient_lib-49.0.4423/resilient_lib/ui/elements.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/ui/tab.py` & `resilient_lib-49.0.4423/resilient_lib/ui/tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib/util/config.py` & `resilient_lib-49.0.4423/resilient_lib/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/resilient_lib.egg-info/PKG-INFO` & `resilient_lib-49.0.4423/resilient_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-lib
-Version: 48.2.4321
+Version: 49.0.4423
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-48.2.4321/resilient_lib.egg-info/SOURCES.txt` & `resilient_lib-49.0.4423/resilient_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/setup.cfg` & `resilient_lib-49.0.4423/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient      >= 48.1
+	resilient      >= 49.0
 	
-	pytz           ~= 2022.1
+	pytz           ~= 2023.3
 	deprecated     ~= 1.2
 	beautifulsoup4 ~= 4.9
 	
 	jinja2         ~= 3.0; python_version >= "3.6"
 	
 	jinja2         ~= 2.0; python_version == "2.7"
```

### Comparing `resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/cert.pem` & `resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/key.open.pem` & `resilient_lib-49.0.4423/tests/shared_mock_data/mock_certs/key.open.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/test_common.py` & `resilient_lib-49.0.4423/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/test_function_metrics.py` & `resilient_lib-49.0.4423/tests/test_function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/test_html2markdown.py` & `resilient_lib-49.0.4423/tests/test_html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/test_oauth2_client_credentials_session.py` & `resilient_lib-49.0.4423/tests/test_oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/test_payload.py` & `resilient_lib-49.0.4423/tests/test_payload.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/test_poller.py` & `resilient_lib-49.0.4423/tests/test_poller.py`

 * *Files 6% similar despite different names*

```diff
@@ -211,15 +211,56 @@
 
     assert "update_soar_case failed to update case in SOAR" in str(err)
 
     # reset
     fx_mock_resilient_client.patch = old_patch
 
 
+@pytest.mark.livetest
+@pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY_VERSION, reason="poller common requires python3.6 or higher")
+def test_update_soar_cases(fx_mock_resilient_client):
+    soar_common = SOARCommon(fx_mock_resilient_client)
 
+    payload = {
+        "patches": {
+            "2314": {
+                "changes": [
+                    {
+                        "field": {"name": "severity_code"},
+                        "old_value": {"text": "Low"},
+                        "new_value": {"text": "High"}
+                    },
+                    {
+                        "field": {"name": "addr"},
+                        "old_value": {"text": None},
+                        "new_value": {"text": "123 street"}
+                    }
+                ],
+                "version": 12
+            },
+            "2315": {
+                "changes": [
+                    {
+                        "field": {"name": "start_date"},
+                        "old_value": {"date": None},
+                        "new_value": {"date": 1681753245000}
+                    },
+                    {
+                        "field": {"name": "zip"},
+                        "old_value": {"text": None},
+                        "new_value": {"text": "14294"}
+                    }
+                ],
+                "version": 14
+            }
+        }
+    }
+
+    updated_cases = soar_common.update_soar_cases(payload)
+    assert not updated_cases.get("failures")
 
 @pytest.mark.livetest
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY_VERSION, reason="poller common requires python3.6 or higher")
 def test_create_case_comment(fx_mock_resilient_client):
     soar_common = SOARCommon(fx_mock_resilient_client)
 
     comment = "A test comment  ฑ ฒ ณ ด ต ถ ท ธ น "
@@ -292,14 +333,26 @@
     mock_entity_comments = ["new comment to add here", "comment to add"]
     mock_soar_comments = ["new comment to add here"]
     resp = soar_common._filter_comments(mock_soar_comments, mock_entity_comments)
 
     assert resp == ["comment to add"]
 
 
+@pytest.mark.livetest
+@pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY_VERSION, reason="poller common requires python3.6 or higher")
+def test_get_case_tasks(fx_mock_resilient_client):
+    soar_common = SOARCommon(fx_mock_resilient_client)
+
+    resp = soar_common.get_case_tasks(2314)
+
+    assert isinstance(resp, list)
+    # If list returned is greater than 0 then a list of tasks was returned
+    assert len(resp) > 0
+
+
 
 def test_eval_mapping(caplog):
     # test convert str to dict
     mock_config = '"source":"A","tags":["tagA"],"priorities":[40,50]'
     parsed_config = eval_mapping(mock_config, "{{ {} }}")
     assert parsed_config == { "source": "A", "tags": ["tagA"], "priorities": [40, 50] }
```

### Comparing `resilient_lib-48.2.4321/tests/test_requests.py` & `resilient_lib-49.0.4423/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/test_templates.py` & `resilient_lib-49.0.4423/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/ui/test_common.py` & `resilient_lib-49.0.4423/tests/ui/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/ui/test_conditions.py` & `resilient_lib-49.0.4423/tests/ui/test_conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/ui/test_permissions.py` & `resilient_lib-49.0.4423/tests/ui/test_permissions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tests/ui/test_tab.py` & `resilient_lib-49.0.4423/tests/ui/test_tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.2.4321/tox.ini` & `resilient_lib-49.0.4423/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     mock
     setuptools-scm<6.0.0 ; python_version=="2.7"
 
 setenv = 
     SETUPTOOLS_SCM_PRETEND_VERSION={env:SETUPTOOLS_SCM_PRETEND_VERSION}
 
 commands = 
+    pip install ../resilient-app-config-plugins
     pip install ../resilient
     pip install .
     pytest --cov --cov-report xml --capture=no -s {posargs} tests/ --durations=0
 
 [coverage:run]
 source=resilient_lib
```

