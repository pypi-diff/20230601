# Comparing `tmp/oslo.metrics-0.5.1.tar.gz` & `tmp/oslo.metrics-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.metrics-0.5.1.tar", last modified: Thu Jun  1 15:22:24 2023, max compression
+gzip compressed data, was "oslo.metrics-0.6.0.tar", last modified: Fri Feb 10 16:03:56 2023, max compression
```

## Comparing `oslo.metrics-0.5.1.tar` & `oslo.metrics-0.6.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.392530 oslo.metrics-0.5.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2023-06-01 15:22:24.392530 oslo.metrics-0.5.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.388530 oslo.metrics-0.5.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.388530 oslo.metrics-0.5.1/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2758 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.388530 oslo.metrics-0.5.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.388530 oslo.metrics-0.5.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.388530 oslo.metrics-0.5.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3489 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.388530 oslo.metrics-0.5.1/oslo.metrics.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/oslo.metrics.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1303 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/oslo.metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/oslo.metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/oslo.metrics.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/oslo.metrics.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/oslo.metrics.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/oslo.metrics.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-06-01 15:22:24.000000 oslo.metrics-0.5.1/oslo.metrics.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.388530 oslo.metrics-0.5.1/oslo_metrics/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3629 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/__main__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2763 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/message_router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3127 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/message_type.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.388530 oslo.metrics-0.5.1/oslo_metrics/metrics/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/metrics/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2791 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/metrics/oslo_messaging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.392530 oslo.metrics-0.5.1/oslo_metrics/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2266 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/tests/test_message_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/oslo_metrics/tests/test_message_validation.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.384530 oslo.metrics-0.5.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.392530 oslo.metrics-0.5.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/notes/add-reno-0cc4d7566599aebd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/notes/port-config-ac5d9ee247a8ff9b.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.392530 oslo.metrics-0.5.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.392530 oslo.metrics-0.5.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:22:24.392530 oslo.metrics-0.5.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9075 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2023-06-01 15:22:24.392530 oslo.metrics-0.5.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1343 2023-06-01 15:21:54.000000 oslo.metrics-0.5.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.489511 oslo.metrics-0.6.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.489511 oslo.metrics-0.6.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2758 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.489511 oslo.metrics-0.6.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.489511 oslo.metrics-0.6.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.489511 oslo.metrics-0.6.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3489 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.489511 oslo.metrics-0.6.0/oslo.metrics.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/oslo.metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2023-02-10 16:03:56.000000 oslo.metrics-0.6.0/oslo.metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/oslo.metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/oslo.metrics.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/oslo.metrics.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/oslo.metrics.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/oslo.metrics.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-10 16:03:55.000000 oslo.metrics-0.6.0/oslo.metrics.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.489511 oslo.metrics-0.6.0/oslo_metrics/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3629 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/__main__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2763 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/message_router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3127 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/message_type.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/oslo_metrics/metrics/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/metrics/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2791 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/metrics/oslo_messaging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/oslo_metrics/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2266 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/tests/test_message_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/oslo_metrics/tests/test_message_validation.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.485511 oslo.metrics-0.6.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/notes/add-reno-0cc4d7566599aebd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/notes/port-config-ac5d9ee247a8ff9b.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9075 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2023-02-10 16:03:56.493511 oslo.metrics-0.6.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2023-02-10 16:03:26.000000 oslo.metrics-0.6.0/tox.ini
```

### Comparing `oslo.metrics-0.5.1/CONTRIBUTING.rst` & `oslo.metrics-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/ChangeLog` & `oslo.metrics-0.6.0/ChangeLog`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 CHANGES
 =======
 
-0.5.1
+0.6.0
 -----
 
 * Fix logging labales --> labels
-* Update TOX\_CONSTRAINTS\_FILE for stable/zed
-* Update .gitreview for stable/zed
+* Add Python3 antelope unit tests
+* Update master for stable/zed
 
 0.5.0
 -----
 
 * Drop python3.6/3.7 support in testing runtime
 * Remove unnecessary unicode prefixes
 * Update master for stable/yoga
```

### Comparing `oslo.metrics-0.5.1/LICENSE` & `oslo.metrics-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/PKG-INFO` & `oslo.metrics-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.metrics
-Version: 0.5.1
+Version: 0.6.0
 Summary: Oslo Metrics API
 Home-page: https://opendev.org/openstack/oslo.metrics
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ====================
         Oslo Metrics Library
```

### Comparing `oslo.metrics-0.5.1/doc/source/conf.py` & `oslo.metrics-0.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/doc/source/index.rst` & `oslo.metrics-0.6.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/doc/source/user/usage.rst` & `oslo.metrics-0.6.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/oslo.metrics.egg-info/PKG-INFO` & `oslo.metrics-0.6.0/oslo.metrics.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.metrics
-Version: 0.5.1
+Version: 0.6.0
 Summary: Oslo Metrics API
 Home-page: https://opendev.org/openstack/oslo.metrics
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ====================
         Oslo Metrics Library
```

### Comparing `oslo.metrics-0.5.1/oslo.metrics.egg-info/SOURCES.txt` & `oslo.metrics-0.6.0/oslo.metrics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,9 +39,10 @@
 releasenotes/notes/port-config-ac5d9ee247a8ff9b.yaml
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/wallaby.rst
 releasenotes/source/xena.rst
 releasenotes/source/yoga.rst
+releasenotes/source/zed.rst
 releasenotes/source/_static/.placeholder
 releasenotes/source/_templates/.placeholder
```

### Comparing `oslo.metrics-0.5.1/oslo_metrics/__main__.py` & `oslo.metrics-0.6.0/oslo_metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/oslo_metrics/message_router.py` & `oslo.metrics-0.6.0/oslo_metrics/message_router.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/oslo_metrics/message_type.py` & `oslo.metrics-0.6.0/oslo_metrics/message_type.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/oslo_metrics/metrics/oslo_messaging.py` & `oslo.metrics-0.6.0/oslo_metrics/metrics/oslo_messaging.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/oslo_metrics/tests/test_message_process.py` & `oslo.metrics-0.6.0/oslo_metrics/tests/test_message_process.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/oslo_metrics/tests/test_message_validation.py` & `oslo.metrics-0.6.0/oslo_metrics/tests/test_message_validation.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/releasenotes/source/conf.py` & `oslo.metrics-0.6.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/setup.cfg` & `oslo.metrics-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/setup.py` & `oslo.metrics-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.metrics-0.5.1/tox.ini` & `oslo.metrics-0.6.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ignore_basepython_conflict = True
 
 [testenv]
 basepython = python3
 allowlist_externals =
   find
 deps =
-  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/zed}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/test-requirements.txt
 commands =
   find . -type f -name "*.pyc" -delete
   stestr run --slowest {posargs}
 
 [testenv:pep8]
 deps = {[testenv]deps}
@@ -22,15 +22,15 @@
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
 allowlist_externals = rm
 deps =
-  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/zed}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/doc/requirements.txt
 commands =
   rm -fr doc/build
   sphinx-build -W --keep-going -b html doc/source doc/build/html
 
 [testenv:cover]
 setenv =
```

