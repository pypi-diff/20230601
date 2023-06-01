# Comparing `tmp/rdt_identity-1.4.2.dev0.tar.gz` & `tmp/rdt_identity-1.5.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.4.2.dev0.tar", last modified: Mon May  1 18:10:53 2023, max compression
+gzip compressed data, was "rdt_identity-1.5.0.dev1.tar", last modified: Thu Jun  1 20:13:51 2023, max compression
```

## Comparing `rdt_identity-1.4.2.dev0.tar` & `rdt_identity-1.5.0.dev1.tar`

### file list

```diff
@@ -1,80 +1,74 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.139033 rdt_identity-1.4.2.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42880 2023-04-26 21:05:25.000000 rdt_identity-1.4.2.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-05-01 18:10:53.139134 rdt_identity-1.4.2.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.127908 rdt_identity-1.4.2.dev0/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.127971 rdt_identity-1.4.2.dev0/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.128033 rdt_identity-1.4.2.dev0/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.131330 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-05-01 18:10:53.139824 rdt_identity-1.4.2.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4183 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.131804 rdt_identity-1.4.2.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.128281 rdt_identity-1.4.2.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.132518 rdt_identity-1.4.2.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.133022 rdt_identity-1.4.2.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    43103 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134071 rdt_identity-1.4.2.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134360 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134809 rdt_identity-1.4.2.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.135130 rdt_identity-1.4.2.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.4.2.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.135715 rdt_identity-1.4.2.dev0/tests/quality/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/dataset_info.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10137 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/quality/test_quality.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.136295 rdt_identity-1.4.2.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/test__addons.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.137949 rdt_identity-1.4.2.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138108 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138407 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138889 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21103 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.032195 rdt_identity-1.5.0.dev1/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    43337 2023-06-01 18:24:00.000000 rdt_identity-1.5.0.dev1/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-06-01 20:13:51.032276 rdt_identity-1.5.0.dev1/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.021031 rdt_identity-1.5.0.dev1/rdt/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.021093 rdt_identity-1.5.0.dev1/rdt/transformers/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.021154 rdt_identity-1.5.0.dev1/rdt/transformers/addons/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.024462 rdt_identity-1.5.0.dev1/rdt/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/rdt/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/rdt/transformers/addons/identity/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-06-01 20:13:51.032745 rdt_identity-1.5.0.dev1/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4183 2023-06-01 20:13:37.000000 rdt_identity-1.5.0.dev1/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.024988 rdt_identity-1.5.0.dev1/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.021391 rdt_identity-1.5.0.dev1/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.025772 rdt_identity-1.5.0.dev1/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.026255 rdt_identity-1.5.0.dev1/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-05-24 18:51:48.000000 rdt_identity-1.5.0.dev1/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.027320 rdt_identity-1.5.0.dev1/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.027646 rdt_identity-1.5.0.dev1/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3319 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4094 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10153 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.5.0.dev1/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.028108 rdt_identity-1.5.0.dev1/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.5.0.dev1/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.028570 rdt_identity-1.5.0.dev1/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.5.0.dev1/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.029068 rdt_identity-1.5.0.dev1/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5780 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-05-24 18:51:48.000000 rdt_identity-1.5.0.dev1/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.030926 rdt_identity-1.5.0.dev1/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.031093 rdt_identity-1.5.0.dev1/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.031414 rdt_identity-1.5.0.dev1/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 20:13:51.032052 rdt_identity-1.5.0.dev1/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 19:29:32.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 19:29:32.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17137 2023-06-01 19:29:32.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19791 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-05-31 20:48:48.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.5.0.dev1/tests/unit/transformers/test_utils.py
```

### Comparing `rdt_identity-1.4.2.dev0/CONTRIBUTING.rst` & `rdt_identity-1.5.0.dev1/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -171,18 +171,17 @@
 For more detailed guide on writing transformers, refer to the `Development Guide`_.
 
 On top of adding the new class, unit tests must be written to cover all of the methods the new
 class uses. In some cases, integration tests may also be required. More details on this can be
 found below.
 
 If the transformer adds a previously unsupported `sdtype` to RDT, then more steps will need
-to be taken for the quality and performance tests. A new `DatasetGenerator` class may need to
-be created for the `sdtype`. You may also need to find a real world dataset containing this
-`sdtype` and request for it to be added. More details for these steps can be found below in
-the `Transformer Performance`_ and `Transformer Quality`_ sections respectively.
+to be taken for performance tests. A new `DatasetGenerator` class may need to be created for
+the `sdtype`. More details for these steps can be found below in the `Transformer Performance`_
+section.
 
 Transformer Validations
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 .. _Code Style:
 
 Code Style
@@ -414,72 +413,14 @@
    3    Reverse Transform Time  6.641531e-07        Yes   s / row             1.080660
    4          Transform Memory  8.896317e+01        Yes  Mb / row             0.656664
    5            Transform Time  5.217231e-07        Yes   s / row             0.484631
 
 Fix any performance issues that are reported. If there are no errors but performance
 can be improved, this function should be used for reference.
 
-.. _Transformer Quality:
-
-Transformer Quality
-"""""""""""""""""""
-
-To assess the quality of a transformer, we run quality tests that apply the Transformer
-on all the real world datasets that contain the Transformer input sdtype. The quality tests
-look at how well the original correlations are preserved by using transformed data to train
-regression models that predict other columns in the data. We compare the transformer's quality
-results to that of other transformers of the same sdtype.
-
-.. _Adding a Dataset:
-
-Adding a Dataset
-****************
-
-If the transformer you are creating adds a new sdtype, then a dataset with that sdtype may need to
-be added for the quality tests. This only needs to be done if the transformer being added is 
-expected to preserve or expose relationships in the data. This can be done using the following
-steps:
-
-1. Find a dataset containing the sdtype your transformer uses as an input.
-
-2. Test your transformer against this dataset by loading it into a ``DataFrame`` and using the
-   ``get_transformer_regression_scores`` in the ``test_quality`` package::
-
-    from tests.quality.test_quality import get_transformer_regression_scores
-    get_transformer_regression_scores(data, sdtype, dataset_name, [transformer])
-
-3. If the scores are higher than the ``TEST_THRESHOLD`` in the ``test_quality`` package, contact
-   one of the `RDT core contributors`_ on GitHub and ask them to add the dataset. Once this is
-   done, the quality tests should pass.
-
-Validating Quality
-******************
-
-Validate the quality of your transformer using the ``validate_transformer_quality`` function.
-This function returns a ``pandas.DataFrame`` containing the scores attained by the transformer
-on each dataset, how that score compares to average and whether or not it is acceptable.
-
-.. code-block:: Python
-
-   In [1]: from tests.contributing import validate_transformer_quality
-
-   In [2]: results = validate_transformer_quality('rdt.transformers.FrequencyEncoder') # Replace FrequencyEncoder with your transformer
-   Validating Quality Tests for transformer FrequencyEncoder
-
-   SUCCESS: The quality tests were successful.
-
-   In [3]: results
-   Out [3]:
-                     Dataset     Score  Compared To Average  Acceptable
-   0                   adult  0.223325             0.443181        True
-   1      student_placements  0.457490             0.994631        True
-   2  student_placements_pii  0.457490             0.988428        True
-
-Fix any quality issues that are reported.
-
 Finalize Your Transformer
 """""""""""""""""""""""""
 
 Re-run all the previous validations until they pass. For a final verification, run
 ``validate_pull_request`` and fix any errors reported. This function runs all the checks described
 above. It also prints a table summarizing the results of all these checks.
 
@@ -492,15 +433,14 @@
 
    Check              Correct    Details
    -----------------  ---------  ----------------------------------------------------------------------
    Code Style         Yes        Code Style is acceptable.
    Unit Tests         Yes        The unit tests are correct and run successfully.
    Integration tests  Yes        The integration tests run successfully.
    Performance Tests  Yes        The performance of the transformer is acceptable.
-   Quality tests      Yes        The output data quality is acceptable.
    Clean Repository   Yes        There are no unexpected changes in the repository.
 
    SUCCESS: The Pull Request can be made!
    You can now commit all your changes, push to GitHub and create a Pull Request.
 
    In [3]: valid
    Out [3]: True
@@ -524,22 +464,16 @@
 7. Run the ``validate_transformer_unit_tests`` function and fix the reported errors.
 8. Run the ``validate_transformer_integration`` function and fix the reported errors.
 9. If required, implement the `Dataset Generators` for the new sdtype. This is described in the
    `Creating Dataset Generators`_ section.
 10. Run the ``validate_transformer_performance`` function and fix any errors reported.
     If there are no errors but performance can be improved, this function should be used for
     reference.
-11. If this transformer is expected to help preserve relationships in the data, run the
-    ``validate_transformer_quality`` function. If the quality is too low, make the
-    necessary enhancements to the transformer.
-12. If the quality tests fail because there is no dataset for the transformer's sdtype,
-    follow the steps in the `Adding a Dataset`_ section to add a real world dataset
-    containing the new sdtype to the quality tests.
-13. Run the ``validate_pull_request`` function as a final check and fix any errors reported.
-14. After all the previous steps pass, all the new and modified files can be committed and pushed
+11. Run the ``validate_pull_request`` function as a final check and fix any errors reported.
+12. After all the previous steps pass, all the new and modified files can be committed and pushed
     to github, and a Pull Request can be submitted. Follow the steps in the
     `Pull Request Guidelines`_ section to submit your Pull Request.
 
 .. _Github actions page: https://github.com/sdv-dev/RDT/actions
 .. _nullable boolean type: https://pandas.pydata.org/pandas-docs/version/1.0/user_guide/boolean.html
 .. _RDT core contributors: https://github.com/orgs/sdv-dev/teams/core-contributors
 .. _dataset generator folder: https://github.com/sdv-dev/RDT/tree/master/tests/datasets
```

### Comparing `rdt_identity-1.4.2.dev0/HISTORY.md` & `rdt_identity-1.5.0.dev1/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # History
 
+## 1.4.2 - 2023-05-02
+
+This release fixes a bug that caused datetime and numerical transformers to crash if a column was all NaNs. Additionally, it adds support for Pandas 2.0!
+
+### Bugs
+
+* Numerical & datetime transformers crash if the entire column is null - Issue [#637](https://github.com/sdv-dev/RDT/issues/637) by @fraces-h
+
+### Maintenance
+
+* Remove upper bound for pandas - Issue [#633](https://github.com/sdv-dev/RDT/issues/633) by @pvk-developer
+
 ## 1.4.1 - 2023-04-25
 
 This release patches an issue that prevented the `RegexGenerator` from working with regexes that had a very large number of possible combinations.
 
 ### Bugs
 
 * RegexGenerator continues to have problems if there are too many possibilities - Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer
```

### Comparing `rdt_identity-1.4.2.dev0/LICENSE` & `rdt_identity-1.5.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/PKG-INFO` & `rdt_identity-1.5.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.4.2.dev0
+Version: 1.5.0.dev1
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt,rdt_identity
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.4.2.dev0 Summary:
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.5.0.dev1 Summary:
 Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
 DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
 rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `rdt_identity-1.4.2.dev0/README.md` & `rdt_identity-1.5.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/RELEASE.md` & `rdt_identity-1.5.0.dev1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.5.0.dev1/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/setup.cfg` & `rdt_identity-1.5.0.dev1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.2.dev0
+current_version = 1.5.0.dev1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt_identity-1.4.2.dev0/setup.py` & `rdt_identity-1.5.0.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,10 +136,10 @@
         exclude=['rdt.transformers.addons.*']
     ),
     python_requires='>=3.7,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.4.2.dev0',
+    version='1.5.0.dev1',
     zip_safe=False,
 )
```

### Comparing `rdt_identity-1.4.2.dev0/tests/__init__.py` & `rdt_identity-1.5.0.dev1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/code_style.py` & `rdt_identity-1.5.0.dev1/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/contributing.py` & `rdt_identity-1.5.0.dev1/tests/contributing.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 from rdt.transformers import get_transformer_class, get_transformers_by_type
 from tests.code_style import (
     get_test_location, validate_test_location, validate_test_names, validate_transformer_addon,
     validate_transformer_importable_from_parent_module, validate_transformer_module,
     validate_transformer_subclass)
 from tests.integration.test_transformers import validate_transformer
 from tests.performance import validate_performance
-from tests.quality.test_quality import (
-    TEST_THRESHOLD, get_regression_scores, get_results_table, get_test_cases)
 
 # Mapping of validation method to (check name, check description).
 CHECK_DETAILS = {
     '_validate_dataset_generators': (
         'Dataset Generators',
         'At least one Dataset Generator exists for the Transformer sdtype.',
     ),
@@ -343,72 +341,14 @@
     coverage_name = module_name.replace('.', '_')
     export_dir = Path('htmlcov') / f'{coverage_name}_py.html'
     print(export_dir.absolute().as_uri())
 
     return rounded_score
 
 
-def validate_transformer_quality(transformer):
-    """Validate quality tests for a transformer.
-
-    This function creates a DataFrame containing the results
-    from running the quality tests for this transformer against
-    all the datasets with columns of its input sdtype. It does the
-    following steps:
-    1. A DataFrame containing the regression scores obtained from running the
-    transformers of the input sdtype against the datasets in the test cases is
-    created. Each row in the DataFrame has the transformer name, dataset name,
-    column name and score. The scores are computed as follows:
-        - For every transformer of the sdtype, transform all the
-        columns of that sdtype.
-        - For every numerical column in the dataset, the transformed
-        columns are used as features to train a regression model.
-        - The score is the coefficient of determination obtained from
-        that model trying to predict the target column.
-    2. Once the scores are gathered, a results table is created. Each row has
-    a transformer name, dataset name, average score for the dataset,
-    a score comparing the transformer's average score for the dataset to
-    the average of the average score for the dataset across all transformers of
-    the same sdtype, and whether or not the score passed the test threshold.
-
-    Returns:
-        DataFrame containing the following columns for each dataset the transformer
-        is validated against: ``Dataset``, ``Score``, ``Compared To Average``, ``Acceptable``.
-    """
-    if isinstance(transformer, str):
-        transformer = get_transformer_class(transformer)
-
-    print(f'Validating Quality Tests for transformer {transformer.get_name()}\n')
-
-    input_sdtype = transformer.get_input_sdtype()
-    test_cases = get_test_cases({input_sdtype})
-    regression_scores = get_regression_scores(test_cases, get_transformers_by_type())
-    results = get_results_table(regression_scores)
-
-    transformer_results = results[results['transformer_name'] == transformer.get_name()]
-    transformer_results = transformer_results.drop('transformer_name', axis=1)
-    transformer_results['Acceptable'] = False
-    passing_relative_scores = transformer_results['score_relative_to_average'] > TEST_THRESHOLD
-    acceptable_indices = passing_relative_scores | (transformer_results['score'] > TEST_THRESHOLD)
-    transformer_results.loc[acceptable_indices, 'Acceptable'] = True
-    new_names = {
-        'dataset_name': 'Dataset',
-        'score': 'Score',
-        'score_relative_to_average': 'Compared To Average'
-    }
-    transformer_results = transformer_results.rename(columns=new_names)
-
-    if transformer_results['Acceptable'].all():
-        print('SUCCESS: The quality tests were successful.\n')
-    else:
-        print('Failure: The quality tests were NOT successful.\n')
-
-    return transformer_results.reset_index(drop=True)
-
-
 def validate_transformer_performance(transformer):
     """Validate the performance of a transformer.
 
     Run the specified Transformer on all the Dataset Generators of the indicated sdtype
     and produce a report about its performance and how it compares to the other
     Transformers of the same sdtype.
 
@@ -531,20 +471,18 @@
     if not inspect.isclass(transformer):
         transformer = get_transformer_class(transformer)
 
     code_style = validate_transformer_code_style(transformer)
     unit_tests = validate_transformer_unit_tests(transformer)
     integration_tests = validate_transformer_integration(transformer)
     performance_tests = validate_transformer_performance(transformer)
-    quality_tests = validate_transformer_quality(transformer)
     clean_repository = check_clean_repository()
 
     unit_bool = unit_tests == 1.0
     performance_bool = 'No' not in performance_tests['Acceptable'].unique()
-    quality_bool = quality_tests['Acceptable'].all()
 
     results = [
         _build_validation_dict(
             'Code Style',
             code_style,
             'Code Style is acceptable.',
             'Code Style is unacceptable!'
@@ -564,20 +502,14 @@
         _build_validation_dict(
             'Performance Tests',
             performance_bool,
             'The performance of the transformer is acceptable.',
             'The performance of the transformer is unacceptable!'
         ),
         _build_validation_dict(
-            'Quality tests',
-            quality_bool,
-            'The output data quality is acceptable.',
-            'The output data quality is unacceptable.',
-        ),
-        _build_validation_dict(
             'Clean Repository',
             clean_repository,
             'There are no unexpected changes in the repository.',
             'There are unexpected changes in the repository!'
         ),
 
     ]
@@ -585,15 +517,14 @@
     results = pd.DataFrame(results)
 
     success = all([
         code_style,
         unit_bool,
         integration_tests,
         performance_bool,
-        quality_bool,
         clean_repository
     ])
 
     print('\n')
     print(tabulate(results, headers='keys', showindex=False))
 
     if success:
```

### Comparing `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_utils.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.5.0.dev1/tests/integration/test_hyper_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from rdt import HyperTransformer, get_demo
 from rdt.errors import ConfigNotSetError, InvalidConfigError, InvalidDataError, NotFittedError
 from rdt.transformers import (
     AnonymizedFaker, BaseTransformer, BinaryEncoder, ClusterBasedNormalizer, FloatFormatter,
     FrequencyEncoder, LabelEncoder, OneHotEncoder, RegexGenerator, UnixTimestampEncoder,
     get_default_transformer, get_default_transformers)
+from rdt.transformers.datetime import OptimizedTimestampEncoder
+from rdt.transformers.numerical import GaussianNormalizer
 from rdt.transformers.pii.anonymizer import PseudoAnonymizedFaker
 
 
 class DummyTransformerNumerical(BaseTransformer):
 
     INPUT_SDTYPE = 'categorical'
 
@@ -1055,38 +1057,38 @@
             -2.467182e-01,
             3.873711e-01,
             9.571797e-17,
             1.286486e-01
         ],
         'balance.component': [0.0, 0, 0, 0, 0],
         'card_type': [
-            0.3273532539594452,
-            0.36028672438848,
-            0.665212975367718,
-            0.8806283675768456,
-            0.23386325679767678
+            0.31440326318001877,
+            0.2879792449993428,
+            0.7147347796329043,
+            0.9397813187279729,
+            0.25144169889394075
         ]
     })
     expected_second_transformed = pd.DataFrame({
         'age': [18.0, 25.0, 54.0, 60.0, 31.0],
         'signup_day': [1.577837e+18, 1.455840e+18, 1.554077e+18, 1.228090e+18, 1.463357e+18],
         'balance.normalized': [
             -2.693016e-01,
             -2.467182e-01,
             3.873711e-01,
             9.571797e-17,
             1.286486e-01
         ],
         'balance.component': [0.0, 0, 0, 0, 0],
         'card_type': [
-            0.24748494176070168,
-            0.3886965582883772,
-            0.7408364277428201,
-            0.9194352110397322,
-            0.2293601452128275
+            0.20248666820805558,
+            0.4408301080724041,
+            0.7082705433167992,
+            0.8911691002937682,
+            0.2679993642397502
         ]
     })
 
     ht1.fit(data)
     first_transformed1 = ht1.transform(data)
     ht2.fit(data)
     first_transformed2 = ht2.transform(data)
@@ -1103,30 +1105,30 @@
             '4863061245886958069',
             '4039466324278480',
             '4217004814656859',
             '4343691397776091'
         ],
         'age': [18, 25, 54, 60, 31],
         'name': ['AAAAA', 'AAAAB', 'AAAAC', 'AAAAD', 'AAAAE'],
-        'signup_day': [np.nan, '02/19/2016', '04/01/2019', np.nan, '05/16/2016'],
-        'balance': [np.nan, 5400, 150000, np.nan, 91000],
+        'signup_day': ['01/01/2020', '02/19/2016', '04/01/2019', np.nan, np.nan],
+        'balance': [250, 5400, 150000, 61662.5, 91000],
         'card_type': ['Visa', 'Visa', 'Master Card', 'Amex', 'Visa']
     })
     expected_second_reverse = pd.DataFrame({
         'credit_card': [
             '4208002654643',
             '3547584322792794',
             '30187802217181',
             '4138954513622487900',
             '346502559595986'
         ],
         'age': [18, 25, 54, 60, 31],
         'name': ['AAAAF', 'AAAAG', 'AAAAH', 'AAAAI', 'AAAAJ'],
-        'signup_day': ['01/01/2020', '02/19/2016', np.nan, '12/01/2008', '05/16/2016'],
-        'balance': [250, 5400, np.nan, 61662.5, 91000],
+        'signup_day': ['01/01/2020', np.nan, '04/01/2019', '12/01/2008', np.nan],
+        'balance': [np.nan, 5400, np.nan, 61662.5, 91000],
         'card_type': ['Visa', 'Visa', 'Master Card', 'Amex', 'Visa']
     })
     first_reverse1 = ht1.reverse_transform(first_transformed1)
     first_reverse2 = ht2.reverse_transform(first_transformed1)
     second_reverse1 = ht1.reverse_transform(first_transformed1)
     pd.testing.assert_frame_equal(first_reverse1, expected_first_reverse)
     pd.testing.assert_frame_equal(first_reverse2, expected_first_reverse)
@@ -1301,7 +1303,58 @@
     ht.fit(data2)
     transformed = ht.transform(data2)
     reverse_transformed2 = ht.reverse_transform(transformed)
 
     # Assert
     assert reverse_transformed1['id1'].tolist() != reverse_transformed2['id1'].tolist()
     assert reverse_transformed1['id2'].tolist() != reverse_transformed2['id2'].tolist()
+
+
+def test_random_seed():
+    # Setup
+    data = pd.DataFrame({
+        'num1': [1, np.nan, 2] * 10,
+        'num2': [1, np.nan, 2] * 10,
+        'num3': [1, np.nan, 2] * 10,
+        'num4': [1, np.nan, 2] * 10,
+        'num5': [1, np.nan, 2] * 10,
+        'num6': [1, np.nan, 2] * 10,
+        'date1': [np.datetime64('2020-10-10'), np.datetime64('2021-11-11'), np.nan] * 10,
+        'date2': [np.datetime64('2020-10-10'), np.datetime64('2021-11-11'), np.nan] * 10,
+        'date3': [np.datetime64('2020-10-10'), np.datetime64('2021-11-11'), np.nan] * 10,
+        'date4': [np.datetime64('2020-10-10'), np.datetime64('2021-11-11'), np.nan] * 10,
+    })
+
+    ht = HyperTransformer()
+    ht.detect_initial_config(data)
+    ht.update_transformers({
+        'num1': FloatFormatter(),
+        'num2': FloatFormatter(),
+        'num3': ClusterBasedNormalizer(),
+        'num4': ClusterBasedNormalizer(),
+        'num5': GaussianNormalizer(),
+        'num6': GaussianNormalizer(),
+        'date1': UnixTimestampEncoder(),
+        'date2': UnixTimestampEncoder(),
+        'date3': OptimizedTimestampEncoder(),
+        'date4': OptimizedTimestampEncoder(),
+    })
+
+    # Run
+    ht.fit(data)
+    transformed = ht.transform(data)
+    reversed1 = ht.reverse_transform(transformed)
+
+    # Assert
+    assert reversed1['num1'].isna().tolist() != reversed1['num2'].isna().tolist()
+    assert reversed1['num3'].isna().tolist() != reversed1['num4'].isna().tolist()
+    assert reversed1['num5'].isna().tolist() != reversed1['num6'].isna().tolist()
+    assert reversed1['date1'].isna().tolist() != reversed1['date2'].isna().tolist()
+    assert reversed1['date3'].isna().tolist() != reversed1['date4'].isna().tolist()
+
+    # Run
+    ht.reset_randomization()
+    transformed = ht.transform(data)
+    reversed2 = ht.reverse_transform(transformed)
+
+    # Assert
+    pd.testing.assert_frame_equal(reversed1, reversed2)
```

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/test_transformers.py` & `rdt_identity-1.5.0.dev1/tests/integration/test_transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 PRIMARY_SDTYPES = ['boolean', 'categorical', 'datetime', 'numerical']
 
 # Additional arguments for transformers
 TRANSFORMER_ARGS = {
     'BinaryEncoder': {
         'missing_value_replacement': -1,
-        'model_missing_values': True
+        'missing_value_generation': 'from_column'
     },
     'UnixTimestampEncoder': {
-        'model_missing_values': True
+        'missing_value_generation': 'from_column'
     },
     'OptimizedTimestampEncoder': {
-        'model_missing_values': True
+        'missing_value_generation': 'from_column'
     },
     'FloatFormatter': {
-        'model_missing_values': True
+        'missing_value_generation': 'from_column'
     },
     'GaussianNormalizer': {
-        'model_missing_values': True
+        'missing_value_generation': 'from_column'
     },
     'ClusterBasedNormalizer': {
-        'model_missing_values': True
+        'missing_value_generation': 'from_column'
     },
 }
 
 # Mapping of rdt sdtype to dtype
 SDTYPE_TO_DTYPES = {
     'boolean': ['b', 'O'],
     'categorical': ['O', 'i', 'f'],
```

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_base.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_boolean.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,32 +38,55 @@
             assert value is False or np.isnan(value)
 
     def test_boolean_missing_value_replacement_mode(self):
         """Test BinaryEncoder when `missing_value_replacement` is set to 'mode'.
 
         Ensure that the BinaryEncoder can fit, transform, and reverse transform on
         boolean data when `missing_value_replacement` is set to `'mode'` and
-        `model_missing_values` is set to True. Expect that the reverse
+        `missing_value_generation` is set to 'from_column'. Expect that the reverse
         transformed data is the same as the input.
-
-        Input:
-            - boolean data with None values
-        Output:
-            - The reversed transformed data
         """
         # Setup
         data = pd.DataFrame([True, True, None, False], columns=['bool'])
         column = 'bool'
-        transformer = BinaryEncoder(missing_value_replacement='mode', model_missing_values=True)
+        transformer = BinaryEncoder(
+            missing_value_replacement='mode',
+            missing_value_generation='from_column'
+        )
 
         # Run
         transformer.fit(data, column)
         transformed = transformer.transform(data)
         reverse = transformer.reverse_transform(transformed)
 
         # Assert
         expected_transformed = pd.DataFrame({
             'bool': [1., 1., 1., 0.],
             'bool.is_null': [0., 0., 1., 0.]
         })
         pd.testing.assert_frame_equal(transformed, expected_transformed)
         pd.testing.assert_frame_equal(reverse, data)
+
+    def test_boolean_missing_value_generation_none(self):
+        """Test the BinaryEncoder when `missing_value_generation` is None.
+
+        In this test we should get `nans` on the transformed data.
+        """
+        # Setup
+        data = pd.DataFrame([True, True, None, False], columns=['bool'])
+        column = 'bool'
+        transformer = BinaryEncoder(
+            missing_value_replacement='mode',
+            missing_value_generation=None
+        )
+
+        # Run
+        transformer.fit(data, column)
+        transformed = transformer.transform(data)
+        reverse = transformer.reverse_transform(transformed)
+
+        # Assert
+        expected_transformed = pd.DataFrame({
+            'bool': [1., 1., None, 0.],
+        })
+        pd.testing.assert_frame_equal(transformed, expected_transformed)
+        pd.testing.assert_frame_equal(reverse, data)
```

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_datetime.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,57 +2,102 @@
 import pandas as pd
 
 from rdt.transformers.datetime import OptimizedTimestampEncoder, UnixTimestampEncoder
 
 
 class TestUnixTimestampEncoder:
     def test_unixtimestampencoder(self):
+        # Setup
         ute = UnixTimestampEncoder(missing_value_replacement='mean')
         data = pd.DataFrame({'column': pd.to_datetime([None, '1996-10-17', '1965-05-23'])})
-        ute.set_random_state(np.random.RandomState(7), 'reverse_transform')
 
         # Run
         ute.fit(data, column='column')
+        ute.set_random_state(np.random.RandomState(7), 'reverse_transform')
         transformed = ute.transform(data)
         reverted = ute.reverse_transform(transformed)
 
         # Asserts
         expected_transformed = pd.DataFrame({
             'column': [3.500064e+17, 845510400000000000, -145497600000000000]
         })
 
         pd.testing.assert_frame_equal(expected_transformed, transformed)
         pd.testing.assert_frame_equal(reverted, data)
 
     def test_unixtimestampencoder_different_format(self):
         ute = UnixTimestampEncoder(missing_value_replacement='mean', datetime_format='%b %d, %Y')
         data = pd.DataFrame({'column': [None, 'Oct 17, 1996', 'May 23, 1965']})
-        ute.set_random_state(np.random.RandomState(7), 'reverse_transform')
 
         # Run
         ute.fit(data, column='column')
+        ute.set_random_state(np.random.RandomState(7), 'reverse_transform')
         transformed = ute.transform(data)
         reverted = ute.reverse_transform(transformed)
 
         # Asserts
         expect_transformed = pd.DataFrame({
             'column': [3.500064e+17, 845510400000000000, -145497600000000000]
         })
         pd.testing.assert_frame_equal(expect_transformed, transformed)
         pd.testing.assert_frame_equal(reverted, data)
 
+    def test_unixtimestampencoder_with_missing_value_generation_none(self):
+        """Test that transformed data will contain null values."""
+        # Setup
+        ute = UnixTimestampEncoder(
+            missing_value_replacement='mean',
+            missing_value_generation=None,
+            datetime_format='%b %d, %Y'
+        )
+        data = pd.DataFrame({'column': [None, 'Oct 17, 1996', 'May 23, 1965']})
+
+        # Run
+        ute.fit(data, column='column')
+        ute.set_random_state(np.random.RandomState(7), 'reverse_transform')
+        transformed = ute.transform(data)
+        reverted = ute.reverse_transform(transformed)
+
+        # Asserts
+        expect_transformed = pd.DataFrame({
+            'column': [None, 845510400000000000, -145497600000000000]
+        })
+        pd.testing.assert_frame_equal(expect_transformed, transformed)
+        pd.testing.assert_frame_equal(reverted, data)
+
+    def test_unixtimestampencoder_with_model_missing_values(self):
+        """Test that `model_missing_values` is accepted by the transformer."""
+        # Setup
+        ute = UnixTimestampEncoder('mean', True)
+        data = pd.DataFrame({'column': pd.to_datetime([None, '1996-10-17', '1965-05-23'])})
+
+        # Run
+        ute.fit(data, column='column')
+        ute.set_random_state(np.random.RandomState(7), 'reverse_transform')
+        transformed = ute.transform(data)
+        reverted = ute.reverse_transform(transformed)
+
+        # Asserts
+        expected_transformed = pd.DataFrame({
+            'column': [3.500064e+17, 845510400000000000, -145497600000000000],
+            'column.is_null': [1., 0., 0.]
+        })
+
+        pd.testing.assert_frame_equal(expected_transformed, transformed)
+        pd.testing.assert_frame_equal(reverted, data)
+
 
 class TestOptimizedTimestampEncoder:
     def test_optimizedtimestampencoder(self):
         ote = OptimizedTimestampEncoder(missing_value_replacement='mean')
-        ote.set_random_state(np.random.RandomState(7), 'reverse_transform')
         data = pd.DataFrame({'column': pd.to_datetime([None, '1996-10-17', '1965-05-23'])})
 
         # Run
         ote.fit(data, column='column')
+        ote.set_random_state(np.random.RandomState(7), 'reverse_transform')
         transformed = ote.transform(data)
         reverted = ote.reverse_transform(transformed)
 
         # Asserts
         expect_transformed = pd.DataFrame({'column': [4051.0, 9786.0, -1684.0]})
         pd.testing.assert_frame_equal(expect_transformed, transformed)
         pd.testing.assert_frame_equal(reverted, data)
```

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_numerical.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import pandas as pd
 
 from rdt.transformers.numerical import ClusterBasedNormalizer, FloatFormatter, GaussianNormalizer
 
 
 class TestFloatFormatter:
 
-    def test_model_missing_values(self):
+    def test_missing_value_generation_from_column(self):
         data = pd.DataFrame([1, 2, 1, 2, np.nan, 1], columns=['a'])
         column = 'a'
 
         nt = FloatFormatter(
             missing_value_replacement='mean',
-            model_missing_values=True,
+            missing_value_generation='from_column',
         )
         nt.fit(data, column)
         transformed = nt.transform(data)
 
         assert isinstance(transformed, pd.DataFrame)
         assert transformed.shape == (6, 2)
         assert list(transformed.iloc[:, 1]) == [0, 0, 0, 0, 1, 0]
@@ -35,15 +35,15 @@
 
         assert isinstance(transformed, pd.DataFrame)
         assert transformed.shape == (5, 1)
 
         reverse = nt.reverse_transform(transformed)
         assert list(reverse['a']) == [1, 2, 1, 2, 1]
 
-    def test_int_nan_not_model_missing_values(self):
+    def test_int_nan_not_missing_value_generation(self):
         data = pd.DataFrame([1, 2, 1, 2, 1, np.nan], columns=['a'])
         column = 'a'
 
         nt = FloatFormatter()
         nt.fit(data, column)
         transformed = nt.transform(data)
 
@@ -66,14 +66,52 @@
 
         assert isinstance(transformed, pd.DataFrame)
         assert transformed.shape == (5, 1)
 
         reverse = nt.reverse_transform(transformed)
         assert list(reverse['a']) == [1, 2, 1, 2, 1]
 
+    def test_missing_value_generation_none(self):
+        """Test when ``missing_value_generation`` is ``None``.
+
+        When ``missing_value_generation`` is ``None`` we are expecting to have
+        ``None`` or null values in our ``transformed`` data.
+        """
+        # Setup
+        data = pd.DataFrame([1, 2, 1, 2, 1, np.nan], columns=['a'])
+        column = 'a'
+        fft = FloatFormatter(missing_value_generation=None)
+        fft.fit(data, column)
+
+        # Run
+        transformed = fft.transform(data)
+
+        # Assert
+        assert isinstance(transformed, pd.DataFrame)
+        assert transformed.shape == (6, 1)
+        assert pd.isna(transformed['a'].iloc[5])
+
+    def test_model_missing_value(self):
+        """Test that we are still able to use ``model_missing_value``."""
+        # Setup
+        data = pd.DataFrame([1, 2, 1, 2, np.nan, 1], columns=['a'])
+        column = 'a'
+
+        # Run
+        nt = FloatFormatter('mean', True)
+        nt.fit(data, column)
+        transformed = nt.transform(data)
+        reverse = nt.reverse_transform(transformed)
+
+        # Assert
+        assert isinstance(transformed, pd.DataFrame)
+        assert transformed.shape == (6, 2)
+        assert list(transformed.iloc[:, 1]) == [0, 0, 0, 0, 1, 0]
+        np.testing.assert_array_almost_equal(reverse, data, decimal=2)
+
 
 class TestGaussianNormalizer:
 
     def test_stats(self):
         data = pd.DataFrame(np.random.normal(loc=4, scale=4, size=1000), columns=['a'])
         column = 'a'
 
@@ -87,43 +125,44 @@
         np.testing.assert_almost_equal(transformed['a'].mean(), 0, decimal=1)
         np.testing.assert_almost_equal(transformed['a'].std(), 1, decimal=1)
 
         reverse = ct.reverse_transform(transformed)
 
         np.testing.assert_array_almost_equal(reverse, data, decimal=1)
 
-    def test_model_missing_values(self):
+    def test_missing_value_generation_from_column(self):
         data = pd.DataFrame([1, 2, 1, 2, np.nan, 1], columns=['a'])
         column = 'a'
 
-        ct = GaussianNormalizer(model_missing_values=True)
+        ct = GaussianNormalizer(missing_value_generation='from_column')
         ct.fit(data, column)
         transformed = ct.transform(data)
 
         assert isinstance(transformed, pd.DataFrame)
         assert transformed.shape == (6, 2)
         assert list(transformed.iloc[:, 1]) == [0, 0, 0, 0, 1, 0]
 
         reverse = ct.reverse_transform(transformed)
 
         np.testing.assert_array_almost_equal(reverse, data, decimal=2)
 
-    def test_not_model_missing_values(self):
+    def test_missing_value_generation_random(self):
         data = pd.DataFrame([1, 2, 1, 2, np.nan, 1], columns=['a'])
         column = 'a'
 
-        ct = GaussianNormalizer(model_missing_values=False)
+        ct = GaussianNormalizer(missing_value_generation='random')
         ct.fit(data, column)
         transformed = ct.transform(data)
 
         assert isinstance(transformed, pd.DataFrame)
         assert transformed.shape == (6, 1)
 
         reverse = ct.reverse_transform(transformed)
-        expected = pd.DataFrame([np.nan, 2, 1, np.nan, 1.4, 1], columns=['a'])
+        expected = pd.DataFrame(
+            [1., 1.9999999510423996, 1., 1.9999999510423996, 1.4, 1.], columns=['a'])
         pd.testing.assert_frame_equal(reverse, expected)
 
     def test_int(self):
         data = pd.DataFrame([1, 2, 1, 2, 1], columns=['a'])
         column = 'a'
 
         ct = GaussianNormalizer()
@@ -136,15 +175,15 @@
         reverse = ct.reverse_transform(transformed)
         assert list(reverse['a']) == [1, 2, 1, 2, 1]
 
     def test_int_nan(self):
         data = pd.DataFrame([1, 2, 1, 2, 1, np.nan], columns=['a'])
         column = 'a'
 
-        ct = GaussianNormalizer(model_missing_values=True)
+        ct = GaussianNormalizer(missing_value_generation='from_column')
         ct.fit(data, column)
         transformed = ct.transform(data)
 
         assert isinstance(transformed, pd.DataFrame)
         assert transformed.shape == (6, 2)
 
         reverse = ct.reverse_transform(transformed)
@@ -180,15 +219,15 @@
         random_state = np.random.get_state()
         np.random.set_state(np.random.RandomState(10).get_state())
         data = self.generate_data()
         mask = np.random.choice([1, 0], data.shape, p=[.1, .9]).astype(bool)
         data[mask] = np.nan
         column = 'col'
 
-        bgmm_transformer = ClusterBasedNormalizer(model_missing_values=True)
+        bgmm_transformer = ClusterBasedNormalizer(missing_value_generation='from_column')
         bgmm_transformer.fit(data, column)
         transformed = bgmm_transformer.transform(data)
 
         assert isinstance(transformed, pd.DataFrame)
         assert transformed.shape == (200, 3)
         assert all(isinstance(x, float) for x in transformed['col.normalized'])
         assert all(isinstance(x, float) for x in transformed['col.component'])
```

### Comparing `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_text.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/performance/test_performance.py` & `rdt_identity-1.5.0.dev1/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/performance/tests/test_profiling.py` & `rdt_identity-1.5.0.dev1/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.5.0.dev1/tests/unit/test_hyper_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1356,21 +1356,23 @@
             - Dataframe with newly generated data from the return values of the transformers.
         """
         # Setup
         instance = Mock()
         instance._fitted = True
         instance._modified_config = False
         instance._subset.return_value = False
+        instance.random_state = {}
 
         random_element = AnonymizedFaker(
             function_name='random_element',
             function_kwargs={'elements': ['a']}
         )
         random_element.columns = ['random_element']
         random_element.output_columns = []
+        random_element.set_random_state(np.random.RandomState(42), 'reverse_transform')
 
         regex_id = RegexGenerator(regex_format='id_[0-9]')
         regex_id.reset_randomization()
         regex_id.columns = ['id']
         regex_id.output_columns = []
 
         instance.field_transformers = {
```

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test___init__.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_base.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import abc
+import re
 from unittest.mock import Mock, call, patch
 
 import numpy as np
 import pandas as pd
 import pytest
 
+from rdt.errors import TransformerInputError
 from rdt.transformers import BaseTransformer, NullTransformer
 from rdt.transformers.base import random_state, set_random_states
 
 
 @patch('rdt.transformers.base.np')
 def test_set_random_states(mock_numpy):
     """Test that the method updates the random states correctly.
@@ -114,27 +116,21 @@
             transformer.set_random_state(new_state, 'fake_method')
 
     def test_reset_randomization(self):
         """Test that the random seed for ``reverse_transform`` is reset."""
         # Setup
         transformer = BaseTransformer()
         transformer.random_states['fit'] = 0
-        transformer.random_states['transform'] = 2
-        transformer.random_states['reverse_transform'] = None
 
         # Run
         transformer.reset_randomization()
 
         # Assert
         fit_state = transformer.INITIAL_FIT_STATE
-        transform_state = transformer.INITIAL_TRANSFORM_STATE
-        reverse_transform_state = transformer.INITIAL_REVERSE_TRANSFORM_STATE
         assert transformer.random_states['fit'] == fit_state
-        assert transformer.random_states['transform'] == transform_state
-        assert transformer.random_states['reverse_transform'] == reverse_transform_state
 
     def test_get_subclasses(self):
         """Test the ``get_subclasses`` method.
 
         Validate that any subclass of the ``BaseTransformer`` is returned by the
         ``get_subclasses`` method except if it also inherits from the ``ABC`` class.
 
@@ -240,14 +236,97 @@
 
         # Run
         output = transformer._get_output_to_property('sdtype')
 
         # Assert
         assert output == {'abc.col': 'float', 'abc': 'categorical'}
 
+    def test__set_missing_value_generation(self):
+        """Test that ``missing_value_generation`` is set if the value is valid."""
+        # Setup
+        instance_none = Mock()
+        instance_random = Mock()
+        instance_from_column = Mock()
+
+        # Run
+        BaseTransformer._set_missing_value_generation(instance_none, None)
+        BaseTransformer._set_missing_value_generation(instance_random, 'random')
+        BaseTransformer._set_missing_value_generation(instance_from_column, 'from_column')
+
+        # Assert
+        assert instance_none.missing_value_generation is None
+        assert instance_random.missing_value_generation == 'random'
+        assert instance_from_column.missing_value_generation == 'from_column'
+
+    def test__set_missing_value_generation_invalid(self):
+        """Test that ``missing_value_generation`` raises an error if the given value is invalid."""
+        # Setup
+        instance = Mock()
+        error_msg = re.escape(
+            "'missing_value_generation' must be one of the following values: None, 'from_column' "
+            "or 'random'."
+        )
+
+        # Run / Assert
+        with pytest.raises(TransformerInputError, match=error_msg):
+            BaseTransformer._set_missing_value_generation(instance, 'None')
+
+    @patch('rdt.transformers.base.warnings')
+    def test_model_missing_values(self, mock_warnings):
+        """Test ``model_missing_values`` property.
+
+        Test that when ``instance.model_missing_values`` is being called a ``boolean`` value
+        is returned whether ``missing_value_generation`` is ``from_column`` or not.
+        """
+        # Setup
+        instance = BaseTransformer()
+        instance.missing_value_generation = 'from_column'
+
+        # Run
+        result = instance.model_missing_values
+
+        # Assert
+        assert result is True
+        mock_warnings.warn.assert_called_once_with((
+            "Future versions of RDT will not support the 'model_missing_values' parameter. "
+            "Please switch to using the 'missing_value_generation' parameter instead."
+        ), FutureWarning)
+
+    @patch('rdt.transformers.base.warnings')
+    def test__set_model_missing_values_true(self, mock_warnings):
+        """Test that a ``FutureWarning`` is being raised."""
+        # Setup
+        instance = Mock()
+        # Run
+        BaseTransformer._set_model_missing_values(instance, True)
+
+        # Assert
+        mock_warnings.warn.assert_called_once_with((
+            "Future versions of RDT will not support the 'model_missing_values' parameter. "
+            "Please switch to using the 'missing_value_generation' parameter to select your "
+            'strategy.'), FutureWarning
+        )
+        instance._set_missing_value_generation.assert_called_once_with('from_column')
+
+    @patch('rdt.transformers.base.warnings')
+    def test__set_model_missing_values_false(self, mock_warnings):
+        """Test that a ``FutureWarning`` is being raised."""
+        # Setup
+        instance = Mock()
+        # Run
+        BaseTransformer._set_model_missing_values(instance, False)
+
+        # Assert
+        mock_warnings.warn.assert_called_once_with((
+            "Future versions of RDT will not support the 'model_missing_values' parameter. "
+            "Please switch to using the 'missing_value_generation' parameter to select your "
+            'strategy.'), FutureWarning
+        )
+        instance._set_missing_value_generation.assert_called_once_with('random')
+
     def test___repr___no_parameters(self):
         """Test that the ``__str__`` method returns the class name.
 
         The ``__repr__`` method should return the class name followed by paranthesis.
         """
         # Setup
         transformer = BaseTransformer()
@@ -1000,14 +1079,15 @@
 
         class Dummy(BaseTransformer):
             columns = ['a', 'b', 'd']
 
         dummy_transformer = Dummy()
 
         # Run
+        dummy_transformer.set_random_state(np.random.RandomState(42), 'transform')
         transformed_data = dummy_transformer.transform(data)
 
         # Assert
         pd.testing.assert_frame_equal(transformed_data, data)
 
     def test_transform_drop_true(self):
         """Test the ``transform``.
@@ -1046,14 +1126,15 @@
             def _transform(self, data):
                 self._passed_data = data.copy()
                 return np.zeros(len(data))
 
         dummy_transformer = Dummy()
 
         # Run
+        dummy_transformer.set_random_state(np.random.RandomState(42), 'transform')
         transformed_data = dummy_transformer.transform(data)
 
         # Assert
         expected_passed = pd.DataFrame({
             'a': [1, 2, 3],
             'b': [4, 5, 6],
         })
@@ -1141,14 +1222,15 @@
 
         class Dummy(BaseTransformer):
             output_columns = ['a', 'b', 'd']
 
         dummy_transformer = Dummy()
 
         # Run
+        dummy_transformer.set_random_state(np.random.RandomState(42), 'reverse_transform')
         transformed_data = dummy_transformer.reverse_transform(data)
 
         # Assert
         pd.testing.assert_frame_equal(transformed_data, data)
 
     def test_reverse_transform(self):
         """Test the ``reverse_transform`` method.
@@ -1171,14 +1253,15 @@
 
             def _reverse_transform(self, data):
                 self._passed_data = data.copy()
                 return np.zeros((len(data), 2))
 
         # Run
         dummy_transformer = Dummy()
+        dummy_transformer.set_random_state(np.random.RandomState(42), 'reverse_transform')
         transformed_data = dummy_transformer.reverse_transform(data)
 
         # Assert
         expected_passed = pd.DataFrame({
             'a': [1, 2, 3],
             'b.is_null': [4, 5, 6],
         })
```

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_boolean.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,25 @@
     def test___init__(self):
         """Test default instance"""
         # Run
         transformer = BinaryEncoder()
 
         # Asserts
         error_message = 'Unexpected missing_value_replacement'
+        error_generation = 'Unexpected missing_value_generation'
         assert transformer.missing_value_replacement == 'mode', error_message
-        assert not transformer.model_missing_values, 'model_missing_values is False by default'
+        assert transformer.missing_value_generation == 'random', error_generation
+
+    def test___init___model_missing_value_passed(self):
+        """Test when model missing value is passed to the init."""
+        # Run
+        transformer = BinaryEncoder(model_missing_values=True)
+
+        # Assert
+        transformer.missing_value_generation == 'from_column'
 
     def test__fit_missing_value_replacement_not_ignore(self):
         """Test _fit missing_value_replacement not equal to ignore"""
         # Setup
         data = pd.Series([False, True, True, False, True])
 
         # Run
@@ -41,18 +50,22 @@
         transformer = BinaryEncoder(missing_value_replacement=0)
         transformer._fit(data)
 
         # Asserts
         error_msg = 'Unexpected fill value'
         assert transformer.null_transformer._missing_value_replacement == 0, error_msg
 
-    def test__fit_model_missing_values(self):
-        """Test output_properties contains 'is_null' column when model_missing_values=True."""
+    def test__fit_missing_value_generation_from_column(self):
+        """Test output_properties contains 'is_null' column.
+
+        When missing_value_generation is 'from_column' the expected output is to have an extra
+        column.
+        """
         # Setup
-        transformer = BinaryEncoder(model_missing_values=True)
+        transformer = BinaryEncoder(missing_value_generation='from_column')
         data = pd.Series([True, np.nan])
 
         # Run
         transformer._fit(data)
 
         # Assert
         assert transformer.output_properties == {
```

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_datetime.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,39 @@
 from rdt.transformers.datetime import OptimizedTimestampEncoder, UnixTimestampEncoder
 from rdt.transformers.null import NullTransformer
 
 
 class TestUnixTimestampEncoder:
 
     def test___init__(self):
-        """Test the ``__init__`` method.
-
-        Validate the passed arguments are stored as attributes.
+        """Test the ``__init__`` method and the passed arguments are stored as attributes."""
+        # Run
+        transformer = UnixTimestampEncoder(
+            missing_value_replacement='mode',
+            missing_value_generation='from_column',
+            datetime_format='%M-%d-%Y'
+        )
 
-        Setup:
-            - initialize a ``UnixTimestampEncoder`` with values for each parameter.
+        # Asserts
+        assert transformer.missing_value_replacement == 'mode'
+        assert transformer.missing_value_generation == 'from_column'
+        assert transformer.datetime_format == '%M-%d-%Y'
 
-        Side effect:
-            - the ``missing_value_replacement`` attribute has been assigned as ``'mode'``.
-            - the ``model_missing_values`` attribute has been assigned as True.
-            - the ``datetime_format`` attribute has been assigned.
-        """
-        # Setup
+    def test___init__with_model_missing_values(self):
+        """Test the ``__init__`` method and the passed arguments are stored as attributes."""
+        # Run
         transformer = UnixTimestampEncoder(
             missing_value_replacement='mode',
-            model_missing_values=True,
+            model_missing_values=False,
             datetime_format='%M-%d-%Y'
         )
 
         # Asserts
         assert transformer.missing_value_replacement == 'mode'
-        assert transformer.model_missing_values is True
+        assert transformer.missing_value_generation == 'random'
         assert transformer.datetime_format == '%M-%d-%Y'
 
     def test__convert_to_datetime(self):
         """Test the ``_convert_to_datetime`` method.
 
         Test to make sure the transformer converts the data to datetime
         if it is of type ``object`` and can be converted.
@@ -244,33 +247,24 @@
     def test__fit(self, null_transformer_mock):
         """Test the ``_fit`` method for numpy arrays.
 
         Validate that this method (1) sets ``self.null_transformer`` to the
         ``NullTransformer`` with the correct attributes, (2) calls the
         ``self.null_transformer``'s ``fit`` method, and (3) calls the
         ``_transform_helper`` method with the transformed data.
-
-        Input:
-            - a pandas Series.
-
-        Side effects:
-            - sets ``self.null_transformer`` to the ``NullTransformer`` with
-            the correct attributes.
-            - calls the ``self.null_transformer``'s ``fit`` method.
-            - calls the ``_transform_helper`` method with the transformed data.
         """
         # Setup
         data = pd.to_datetime(['2020-01-01', '2020-02-01', '2020-03-01'])
         transformer = UnixTimestampEncoder()
 
         # Run
         transformer._fit(data)
 
         # Assert
-        null_transformer_mock.assert_called_once_with('mean', False)
+        null_transformer_mock.assert_called_once_with('mean', 'random')
         assert null_transformer_mock.return_value.fit.call_count == 1
         np.testing.assert_allclose(
             null_transformer_mock.return_value.fit.call_args_list[0][0][0],
             np.array([1.577837e+18, 1.580515e+18, 1.583021e+18]), rtol=1e-5
         )
 
     def test__fit_calls_transform_helper(self):
@@ -310,18 +304,22 @@
         # Assert
         np.testing.assert_array_equal(
             mock__guess_datetime_format_for_array.call_args[0][0],
             np.array(['2020-02-01', '2020-03-01'])
         )
         assert transformer.datetime_format == '%Y-%m-%d'
 
-    def test__fit_model_missing_values(self):
-        """Test output_properties contains 'is_null' column when model_missing_values=True."""
+    def test__fit_missing_value_generation(self):
+        """Test output_properties contains 'is_null' column.
+
+        When missing_value_generation is 'from_column' the expected output is to have an extra
+        column.
+        """
         # Setup
-        transformer = UnixTimestampEncoder(model_missing_values=True)
+        transformer = UnixTimestampEncoder(missing_value_generation='from_column')
         data = pd.Series(['2020-02-01', np.nan])
 
         # Run
         transformer._fit(data)
 
         # Assert
         assert transformer.output_properties == {
@@ -330,26 +328,14 @@
         }
 
     def test__transform(self):
         """Test the ``_transform`` method for numpy arrays.
 
         Validate that this method calls the ``null_transformer.transform`` method.
         It should also check that the final output is correct.
-
-        Setup:
-            - mock behavior of ``_fit``.
-
-        Input:
-            - a pandas Series.
-
-        Output:
-            - a numpy array containing the transformed data.
-
-        Side effect:
-            - calls the ``null_transformer.transform`` method with the transformed data.
         """
         # Setup
         data = pd.to_datetime(['2020-01-01', '2020-02-01', '2020-03-01'])
         transformer = UnixTimestampEncoder()
         transformer.null_transformer = Mock()
 
         # Run
@@ -362,20 +348,14 @@
             np.array([[1.577837e+18, 1.580515e+18, 1.583021e+18]]), rtol=1e-5
         )
 
     def test__reverse_transform_all_none(self):
         """Test the ``_reverse_transform`` method with ``None`` values.
 
         Validate that the method transforms ``None`` into ``NaT``.
-
-        Input:
-            - A ``pd.Series`` with ``None`` as a value.
-
-        Output:
-            - A ``DatetimeIndex`` with ``NaT`` as a value.
         """
         # Setup
         ute = UnixTimestampEncoder()
         ute.null_transformer = NullTransformer('mean')
 
         # Run
         output = ute._reverse_transform(pd.Series([None]))
@@ -384,45 +364,29 @@
         expected = pd.Series(pd.to_datetime(['NaT']))
         pd.testing.assert_series_equal(output, expected)
 
     def test__reverse_transform(self):
         """Test the ``_reverse_transform`` method.
 
         Validate that the method correctly reverse transforms.
-
-        Input:
-            - a numpy array.
-
-        Output:
-            - a pandas ``DatetimeIndex`` of the correct datetimes.
         """
         # Setup
         ute = UnixTimestampEncoder()
         transformed = np.array([1.5778368e+18, 1.5805152e+18, 1.5830208e+18])
         ute.null_transformer = NullTransformer('mean')
 
         # Run
         output = ute._reverse_transform(transformed)
 
         # Assert
         expected = pd.Series(pd.to_datetime(['2020-01-01', '2020-02-01', '2020-03-01']))
         pd.testing.assert_series_equal(output, expected)
 
     def test__reverse_transform_datetime_format_dtype_is_datetime(self):
-        """Test the ``_reverse_transform`` method returns the correct datetime format.
-
-        Setup:
-            - Set the instance to have a different ``datetime_format``.
-
-        Input:
-            - a numpy array of integers.
-
-        Output:
-            - a pandas ``Series`` of the datetimes in the right format.
-        """
+        """Test the ``_reverse_transform`` method returns the correct datetime format."""
         # Setup
         ute = UnixTimestampEncoder()
         ute.datetime_format = '%b %d, %Y'
         transformed = np.array([1.5778368e+18, 1.5805152e+18, 1.5830208e+18])
         ute._dtype = np.dtype('<M8[ns]')
         ute.null_transformer = NullTransformer('mean')
 
@@ -430,25 +394,15 @@
         output = ute._reverse_transform(transformed)
 
         # Assert
         expected = pd.Series(pd.to_datetime(['Jan 01, 2020', 'Feb 01, 2020', 'Mar 01, 2020']))
         pd.testing.assert_series_equal(output, expected)
 
     def test__reverse_transform_datetime_format(self):
-        """Test the ``_reverse_transform`` method returns the correct datetime format.
-
-        Setup:
-            - Set the instance to have a different ``datetime_format``.
-
-        Input:
-            - a numpy array of integers.
-
-        Output:
-            - a pandas ``Series`` of the datetimes in the right format.
-        """
+        """Test the ``_reverse_transform`` method returns the correct datetime format."""
         # Setup
         ute = UnixTimestampEncoder()
         ute.datetime_format = '%b %d, %Y'
         transformed = np.array([1.5778368e+18, 1.5805152e+18, 1.5830208e+18])
         ute._dtype = 'object'
         ute.null_transformer = NullTransformer('mean')
 
@@ -456,25 +410,15 @@
         output = ute._reverse_transform(transformed)
 
         # Assert
         expected = pd.Series(['Jan 01, 2020', 'Feb 01, 2020', 'Mar 01, 2020'])
         pd.testing.assert_series_equal(output, expected)
 
     def test__reverse_transform_datetime_format_with_strftime_formats(self):
-        """Test the ``_reverse_transform`` method returns the correct datetime format.
-
-        Setup:
-            - Set the instance to have a different ``datetime_format`` which includes `-` on it.
-
-        Input:
-            - a numpy array of integers.
-
-        Output:
-            - a pandas ``Series`` of the datetimes in the right format.
-        """
+        """Test the ``_reverse_transform`` method returns the correct datetime format."""
         # Setup
         ute = UnixTimestampEncoder()
         ute.datetime_format = '%b %-d, %Y'
         transformed = np.array([1.5778368e+18, 1.5805152e+18, 1.5830208e+18])
         ute._dtype = 'object'
         ute.null_transformer = NullTransformer('mean')
 
@@ -491,20 +435,14 @@
 
     def test__find_divider(self):
         """Test the ``_find_divider`` method.
 
         Find the greatest common denominator out of these values: [10] * 9 + [60, 60, 24],
         where each consecutive value in the list is multiplied by the previous one
         (so 10, 100, 1000, etc).
-
-        Input:
-            - a numpy array.
-
-        Side effect:
-            - sets ``self.divider`` to the correct divider.
         """
         # Setup
         data = np.array([100, 7919])
         transformer = OptimizedTimestampEncoder()
 
         # Run
         transformer._find_divider(data)
@@ -513,20 +451,14 @@
         assert transformer.divider == 1
 
     def test__transform_helper(self):
         """Test the ``_transform_helper`` method.
 
         Validate the helper method produces the values stripped to the smallest
         non-zero time unit.
-
-        Input:
-            - a pandas series of datetimes.
-
-        Output:
-            - a pandas series of the transformed datetimes.
         """
         # Setup
         data = pd.to_datetime(['2020-01-01', '2020-02-01', '2020-03-01'])
         transformer = OptimizedTimestampEncoder()
 
         # Run
         transformed = transformer._transform_helper(data)
@@ -537,20 +469,14 @@
         ]))
 
     def test__reverse_transform_helper(self):
         """Test the ``_reverse_transform_helper`` method.
 
         Validate the helper produces the values multiplied by the
         smallest non-zero time unit.
-
-        Input:
-            - a pandas series of timestamps.
-
-        Output:
-            - a numpy array of the values multiplied by ``self.divider``.
         """
         # Setup
         data = pd.Series([18262., 18293., 18322.])
         transformer = OptimizedTimestampEncoder()
         transformer.divider = 1000
         transformer.null_transformer = Mock()
         transformer.null_transformer.reverse_transform.side_effect = lambda x: x
```

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_null.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_null.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,98 @@
 """Unit tests for the NullTransformer."""
 
+import re
 from unittest.mock import patch
 
 import numpy as np
 import pandas as pd
+import pytest
 
+from rdt.errors import TransformerInputError
 from rdt.transformers import NullTransformer
 
 
 class TestNullTransformer:
 
     def test___init__default(self):
         """Test the initialization without passing any default arguments.
 
         When no arguments are passed, the attributes should be populated
         with the right values.
-
-        Input:
-            - nothing
-
-        Expected Side Effects:
-            - The `_missing_value_replacement` attribute should be `None`.
-            - The `_model_missing_values` attribute should be `False`.
         """
         # Run
         transformer = NullTransformer()
 
         # Assert
         assert transformer._missing_value_replacement is None
-        assert not transformer._model_missing_values
+        assert transformer._missing_value_generation == 'random'
 
     def test___init__not_default(self):
         """Test the initialization passing values different than defaults.
 
         When arguments are passed, the attributes should be populated
         with the right values.
 
         Input:
             - Values different than the defaults.
 
         Expected Side Effects:
             - The attributes should be populated with the given values.
         """
         # Run
-        transformer = NullTransformer('a_missing_value_replacement', False)
+        transformer = NullTransformer('a_missing_value_replacement', None)
 
         # Assert
         assert transformer._missing_value_replacement == 'a_missing_value_replacement'
-        assert not transformer._model_missing_values
+        assert transformer._missing_value_generation is None
+
+    def test___init__raises_error(self):
+        """Test the initialization passing invalid values for ``missing_value_generation``."""
+        # Setup
+        error_msg = re.escape(
+            "'missing_value_generation' must be one of the following values: None, 'from_column' "
+            "or 'random'."
+        )
+
+        # Run / Assert
+        with pytest.raises(TransformerInputError, match=error_msg):
+            NullTransformer('mean', 'None')
 
     def test_models_missing_values(self):
         """Test the models_missing_values method.
 
-        If the `model_missing_values` attributes evalutes to True, the
-        `create_model_missing_values` method should return the same value.
+        Test that when ``missing_value_generation`` is ``'from_column'``, this returns
+        ``True``.
+        """
+        # Setup
+        transformer = NullTransformer('something', missing_value_generation='from_column')
 
-        Setup:
-            - Create an instance and set _model_missing_values to True
+        # Run
+        models_missing_values = transformer.models_missing_values()
 
-        Expected Output:
-            - True
+        # Assert
+        assert models_missing_values is True
+
+    def test_models_missing_values_missing_value_generation_is_none(self):
+        """Test the models_missing_values method.
+
+        Test that when ``missing_value_generation`` is other than ``'from_column'``, this returns
+        ``False``.
         """
         # Setup
-        transformer = NullTransformer('something', model_missing_values=True)
-        transformer._model_missing_values = True
+        none_transformer = NullTransformer('something', missing_value_generation=None)
+        random_transformer = NullTransformer('something', missing_value_generation='random')
 
         # Run
-        models_missing_values = transformer.models_missing_values()
+        none_models_missing_values = none_transformer.models_missing_values()
+        random_models_missing_values = random_transformer.models_missing_values()
 
         # Assert
-        assert models_missing_values
+        assert none_models_missing_values is False
+        assert random_models_missing_values is False
 
     def test__get_missing_value_replacement_scalar(self):
         """Test _get_missing_value_replacement when a scalar value is passed.
 
         If a missing_value_replacement different from None, 'mean' or 'mode' is
         passed to __init__, that value is returned.
 
@@ -236,241 +255,193 @@
         # Assert
         logger_mock.info.assert_called_once_with(
             "'missing_value_replacement' cannot be set to 'mode' when "
             'the provided data only contains NaNs. Using 0 instead.'
         )
         assert missing_value_replacement == 0
 
-    def test_fit_model_missing_values_none_and_nulls(self):
-        """Test fit when null column is none and there are nulls.
-
-        If there are nulls in the data and model_missing_values was given as None,
-        then the _model_missing_values attribute should be set to True.
-        Also validate that the null attribute and the _missing_value_replacement attributes
-        are set accordingly.
+    def test_fit_missing_value_generation_is_none_and_nulls(self):
+        """Test fit when ``missing_value_generation`` is ``None`` and there are nulls.
 
-        Setup:
-            - A NullTransformer with default arguments.
-
-        Input:
-            - pd.Series of integers that contains nulls.
-
-        Expected Side Effects:
-            - the model_missing_values attribute should be set to True.
-            - the nulls attribute should be set to True.
-            - the missing_value_replacement should be set to the mean of the given integers.
+        Nothing has been learned, nulls stay as ``None`` and the ``_missing_value_replacement``
+        is still ``'mean'`` or the default value.
         """
         # Setup
-        transformer = NullTransformer(missing_value_replacement='mean', model_missing_values=True)
+        transformer = NullTransformer(
+            missing_value_replacement='mean',
+            missing_value_generation=None
+        )
 
         # Run
         data = pd.Series([1, 2, np.nan])
         transformer.fit(data)
 
         # Assert
-        assert transformer.nulls
-        assert transformer._model_missing_values
-        assert transformer._missing_value_replacement == 1.5
-
-    def test_fit_model_missing_values_none_and_no_nulls(self):
-        """Test fit when null column is none and there are NO nulls.
-
-        If there are no nulls in the data and model_missing_values was given as ``False``,
-        then the _model_missing_values attribute should be set to ``False``.
-        Also validate that the null attribute and the ``_missing_value_replacement`` attributes
-        are set accordingly.
-
-        Setup:
-            - A NullTransformer with default arguments.
+        assert transformer.nulls is None
+        assert transformer._missing_value_replacement == 'mean'  # Has not been altered.
 
-        Input:
-            - pd.Series of strings that contains no nulls.
-
-        Expected Side Effects:
-            - the model_missing_values attribute should be set to False.
-            - the nulls attribute should be set to False.
-            - the missing_value_replacement should be set to ``np.nan``, default.
-        """
+    def test_fit_missing_value_generation_from_column_and_no_nulls(self):
+        """Test fit when ``missing_value_generation`` is 'from_column' and there are nulls."""
         # Setup
-        transformer = NullTransformer()
+        transformer = NullTransformer(missing_value_generation='from_column')
 
         # Run
         data = pd.Series(['a', 'b', 'b'])
         transformer.fit(data)
 
         # Assert
         assert not transformer.nulls
-        assert not transformer._model_missing_values
+        assert transformer._missing_value_generation is None
         assert transformer._missing_value_replacement is None
 
-    def test_fit_model_missing_values_not_none(self):
-        """Test fit when null column is set to True/False.
-
-        If model_missing_values is set to True or False, the _model_missing_values should
-        get that value regardless of whether there are nulls or not.
-
-        Notice that this test covers 4 scenarios at once.
+    def test_fit_with_multiple_missing_value_generations(self):
+        """Test fit when ``missing_value_generation`` is set to its three possibilities.
 
-        Setup:
-            - 4 NullTransformer intances, 2 of them passing False for the model_missing_values
-              and 2 of them passing True.
-
-        Input:
-            - 2 pd.Series, one containing nulls and the other not containing nulls.
+        Test that when there are multiple scenarios given, the null transformer is able to
+        either learn the mode or mean to replace the value but following the
+        ``missing_value_generation`` strategy.
 
-        Expected Side Effects:
-            - the _model_missing_values attribute should be set to True or False as indicated
-              in the Transformer creation.
-            - the nulls attribute should be True or False depending on whether
-              the input data contains nulls or not.
+        Notice that this test covers 5 scenarios at once.
         """
         # Setup
-        model_missing_values_false_nulls = NullTransformer(
+        missing_value_generation_random_nulls = NullTransformer(
             missing_value_replacement='mode',
-            model_missing_values=False
+            missing_value_generation='random'
         )
-        model_missing_values_false_no_nulls = NullTransformer(
+        missing_value_generation_random_no_nulls = NullTransformer(
             missing_value_replacement='mode',
-            model_missing_values=False
+            missing_value_generation='random'
+        )
+        missing_value_generation_column_nulls = NullTransformer(
+            missing_value_replacement='mean',
+            missing_value_generation='from_column'
         )
-        model_missing_values_true_nulls = NullTransformer(
+        missing_value_generation_column_no_nulls = NullTransformer(
+            missing_value_replacement='mean',
+            missing_value_generation='from_column'
+        )
+
+        missing_value_generation_none_int = NullTransformer(
             missing_value_replacement='mean',
-            model_missing_values=True
+            missing_value_generation=None
         )
-        model_missing_values_true_no_nulls = NullTransformer(
+        missing_value_generation_none_str = NullTransformer(
             missing_value_replacement='mean',
-            model_missing_values=True
+            missing_value_generation=None
         )
+
         nulls_str = pd.Series(['a', 'b', 'b', np.nan])
         no_nulls_str = pd.Series(['a', 'b', 'b', 'c'])
         nulls_int = pd.Series([1, 2, 3, np.nan])
         no_nulls_int = pd.Series([1, 2, 3, 4])
 
         # Run
-        model_missing_values_false_nulls.fit(nulls_str)
-        model_missing_values_false_no_nulls.fit(no_nulls_str)
-        model_missing_values_true_nulls.fit(nulls_int)
-        model_missing_values_true_no_nulls.fit(no_nulls_int)
-
-        # Assert
-        assert not model_missing_values_false_nulls._model_missing_values
-        assert model_missing_values_false_nulls.nulls
-        assert model_missing_values_false_nulls._missing_value_replacement == 'b'
-
-        assert not model_missing_values_false_no_nulls._model_missing_values
-        assert not model_missing_values_false_no_nulls.nulls
-        assert model_missing_values_false_no_nulls._missing_value_replacement == 'b'
-
-        assert model_missing_values_true_nulls._model_missing_values
-        assert model_missing_values_true_nulls.nulls
-        assert model_missing_values_true_nulls._missing_value_replacement == 2
-
-        assert not model_missing_values_true_no_nulls._model_missing_values
-        assert not model_missing_values_true_no_nulls.nulls
-        assert model_missing_values_true_no_nulls._missing_value_replacement == 2.5
+        missing_value_generation_random_nulls.fit(nulls_str)
+        missing_value_generation_random_no_nulls.fit(no_nulls_str)
+        missing_value_generation_column_nulls.fit(nulls_int)
+        missing_value_generation_column_no_nulls.fit(no_nulls_int)
+        missing_value_generation_none_int.fit(nulls_int)
+        missing_value_generation_none_str.fit(nulls_str)
+
+        # Assert
+        assert missing_value_generation_random_nulls._missing_value_generation == 'random'
+        assert missing_value_generation_random_nulls.nulls
+        assert missing_value_generation_random_nulls._missing_value_replacement == 'b'
+
+        assert missing_value_generation_random_no_nulls._missing_value_generation == 'random'
+        assert not missing_value_generation_random_no_nulls.nulls
+        assert missing_value_generation_random_no_nulls._missing_value_replacement == 'b'
+
+        assert missing_value_generation_column_nulls._missing_value_generation == 'from_column'
+        assert missing_value_generation_column_nulls.nulls
+        assert missing_value_generation_column_nulls._missing_value_replacement == 2
+
+        assert missing_value_generation_column_no_nulls._missing_value_generation is None
+        assert not missing_value_generation_column_no_nulls.nulls
+        assert missing_value_generation_column_no_nulls._missing_value_replacement == 2.5
+
+        assert missing_value_generation_none_int._missing_value_generation is None
+        assert missing_value_generation_none_int.nulls is None
+        assert missing_value_generation_none_int._missing_value_replacement == 'mean'
+
+        assert missing_value_generation_none_str._missing_value_generation is None
+        assert missing_value_generation_none_str.nulls is None
+        assert missing_value_generation_none_str._missing_value_replacement == 'mean'
 
-    def test_transform__model_missing_values_true(self):
-        """Test transform when _model_missing_values.
+    def test_transform__missing_value_generation_from_column(self):
+        """Test transform when ``_missing_value_generation`` is set to ``from_column``.
 
-        When _model_missing_values, the nulls should be replaced
-        by the _missing_value_replacement and another column flagging the nulls
+        When ``missing_value_generation`` is 'from_column', the nulls should be replaced
+        by the ``_missing_value_replacement`` and another column flagging the nulls
         should be created.
-
-        Setup:
-            - NullTransformer instance with _model_missing_values set to True,
-              _missing_value_replacement set to a scalar value.
-
-        Input:
-            - A pd.Series of strings with nulls.
-
-        Expected Output:
-            - Exactly the same as the input, replacing the nulls with the
-              scalar value.
-
-        Expected Side Effects:
-            - The input data has the null values replaced.
         """
         # Setup
-        transformer = NullTransformer()
+        transformer = NullTransformer(missing_value_generation='from_column')
         transformer.nulls = False
-        transformer._model_missing_values = True
         transformer._missing_value_replacement = 'c'
         input_data = pd.Series(['a', 'b', np.nan])
 
         # Run
         output = transformer.transform(input_data)
 
         # Assert
         expected_output = np.array([
             ['a', 0.0],
             ['b', 0.0],
             ['c', 1.0],
         ], dtype=object)
         np.testing.assert_equal(expected_output, output)
 
-    def test_transform__model_missing_values_false(self):
-        """Test transform when _model_missing_values is False.
-
-        When the _model_missing_values is false, the nulls should be replaced
-        by the _missing_value_replacement.
+    def test_transform__missing_value_generation_random(self):
+        """Test transform when ``_missing_value_generation`` is set to ``random``.
 
-        Setup:
-            - NullTransformer instance with _model_missing_values set to False,
-              _missing_value_replacement set to a scalar value.
-
-        Input:
-            - A pd.Series of integers with nulls.
-
-        Expected Output:
-            - Same data as the input, replacing the nulls with the
-              scalar value.
-
-        Expected Side Effects:
-            - The input data has not been modified.
+        Test that when the ``_missing_value_generation`` is set to ``random``, the nulls should
+        be replaced by the ``_missing_value_replacement``.
         """
         # Setup
         transformer = NullTransformer()
-        transformer._model_missing_values = False
         transformer._missing_value_replacement = 3
         input_data = pd.Series([1, 2, np.nan])
 
         # Run
         output = transformer.transform(input_data)
 
         # Assert
         expected_output = np.array([1, 2, 3])
         np.testing.assert_equal(expected_output, output)
 
         modified_input_data = pd.Series([1, 2, np.nan])
         pd.testing.assert_series_equal(modified_input_data, input_data)
 
-    def test_reverse_transform__model_missing_values_true_nulls_true(self):
-        """Test reverse_transform when _model_missing_values and nulls are True.
+    def test_transform__missing_value_generation_is_none(self):
+        """Test transform when ``_missing_value_generation`` is set to ``from_column``.
 
-        When _model_missing_values and nulls attributes are both True, the second column
-        in the input data should be used to decide which values to replace
-        with nan, by selecting the rows where the null column value is > 0.5.
+        When ``missing_value_generation`` is 'None', the nulls should be returned.
+        """
+        # Setup
+        transformer = NullTransformer(missing_value_generation=None)
+        transformer.nulls = False
+        transformer._missing_value_replacement = 'c'
+        input_data = pd.Series([1., 2., np.nan])
 
-        Setup:
-            - NullTransformer instance with _model_missing_values and nulls
-              attributes set to True.
+        # Run
+        output = transformer.transform(input_data)
 
-        Input:
-            - 2d numpy array with variate float values.
+        # Assert
+        np.testing.assert_equal(input_data, output)
 
-        Expected Output:
-            - pd.Series containing the first column from the input data
-              with the values indicated by the first column replaced by nans.
+    def test_reverse_transform__missing_value_generation_from_column_with_nulls(self):
+        """Test reverse_transform when ``missing_value_generation`` is ``from_column`` and nulls.
 
-        Expected Side Effects:
-            - the input data should have been modified.
+        When ``missing_value_generation`` is ``from_column`` and there are nulls, the second column
+        in the input data should be used to decide which values to replace with nan,
+        by selecting the rows where the null column value is > 0.5.
         """
         # Setup
-        transformer = NullTransformer()
-        transformer._model_missing_values = True
+        transformer = NullTransformer(missing_value_generation='from_column')
         transformer.nulls = True
         input_data = np.array([
             [0.0, 0.0],
             [0.2, 0.2],
             [0.4, 0.4],
             [0.6, 0.6],
             [0.8, 0.8],
@@ -479,34 +450,23 @@
         # Run
         output = transformer.reverse_transform(input_data)
 
         # Assert
         expected_output = pd.Series([0.0, 0.2, 0.4, np.nan, np.nan])
         pd.testing.assert_series_equal(expected_output, output)
 
-    def test_reverse_transform__model_missing_values_true_nulls_false(self):
-        """Test reverse_transform when _model_missing_values and nulls is False.
-
-        When _model_missing_values but nulls are False, the second column of the
-        input data must be dropped and the first one returned as a Series without
-        having been modified.
-
-        Setup:
-            - NullTransformer instance with _model_missing_values set to True and nulls
-              attribute set to False
+    def test_reverse_transform__missing_value_generation_from_column_no_nulls(self):
+        """Test reverse_transform when ``missing_value_generation`` is ``from_column``, no nulls.
 
-        Input:
-            - 2d numpy array with variate float values.
-
-        Expected Output:
-            - pd.Series containing the first column from the input data unmodified.
+        When ``missing_value_generation`` is ``from_column`` but no nulls are found, the second
+        column of the input data must be dropped and the first one returned as a ``pd.Series``
+        without having been modified.
         """
         # Setup
-        transformer = NullTransformer()
-        transformer._model_missing_values = True
+        transformer = NullTransformer(missing_value_generation='from_column')
         transformer.nulls = False
         input_data = np.array([
             [0.0, 0.0],
             [0.2, 0.2],
             [0.4, 0.4],
             [0.6, 0.6],
             [0.8, 0.8],
@@ -516,67 +476,42 @@
         output = transformer.reverse_transform(input_data)
 
         # Assert
         expected_output = pd.Series([0.0, 0.2, 0.4, 0.6, 0.8])
         pd.testing.assert_series_equal(expected_output, output)
 
     @patch('rdt.transformers.null.np.random')
-    def test_reverse_transform__model_missing_values_false_nulls_true(self, random_mock):
-        """Test reverse_transform when _model_missing_values is False and nulls.
+    def test_reverse_transform__missing_value_generation_random_with_nulls(self, random_mock):
+        """Test reverse_transform when ``missing_value_generation`` is ``random`` and nulls.
 
-        When _model_missing_values is False and the nulls attribute, a ``_null_percentage``
+        When ``missing_value_generation`` is ``random`` and there are nulls, a ``_null_percentage``
         of values should randomly be replaced with ``np.nan``.
-
-        Setup:
-            - NullTransformer instance with _model_missing_values set to False and nulls
-              attribute set to True.
-            - A mock for ``np.random``.
-
-        Input:
-            - 1d numpy array with variate float values.
-
-        Expected Output:
-            - pd.Series containing the same data as input, with the random values
-            replaced with ``np.nan``.
         """
         # Setup
-        transformer = NullTransformer()
-        transformer._model_missing_values = False
+        transformer = NullTransformer(missing_value_generation='random')
         transformer.nulls = True
         transformer._null_percentage = 0.5
         input_data = np.array([0.0, 0.2, 0.4, 0.6])
         random_mock.random.return_value = np.array([1, 1, 0, 1])
 
         # Run
         output = transformer.reverse_transform(input_data)
 
         # Assert
         expected_output = pd.Series([0.0, 0.2, np.nan, 0.6])
         pd.testing.assert_series_equal(expected_output, output)
 
-    def test_reverse_transform__model_missing_values_false_nulls_false(self):
-        """Test reverse_transform when _model_missing_values is False and nulls.
-
-        When _model_missing_values is False and the nulls attribute is also False, the
-        input data is not modified at all.
+    def test_reverse_transform__missing_value_generation_random_no_nulls(self):
+        """Test reverse_transform when missing_value_generation is ``random`` and no nulls.
 
-        Setup:
-            - NullTransformer instance with _model_missing_values and nulls attributes
-              set to False, and the _missing_value_replacement set to a scalar value.
-
-        Input:
-            - 1d numpy array with variate float values, containing the _missing_value_replacement
-              among them.
-
-        Expected Output:
-            - pd.Series containing the same data as input, without modification.
+        When ``missing_value_generation`` is ``random`` and there are no nulls, the input data
+        is not modified at all.
         """
         # Setup
-        transformer = NullTransformer()
-        transformer._model_missing_values = False
+        transformer = NullTransformer(missing_value_generation='random')
         transformer.nulls = False
         transformer._missing_value_replacement = 0.4
         input_data = np.array([0.0, 0.2, 0.4, 0.6])
 
         # Run
         output = transformer.reverse_transform(input_data)
```

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_numerical.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 class TestFloatFormatter(TestCase):
 
     def test___init__super_attrs(self):
         """super() arguments are properly passed and set as attributes."""
         nt = FloatFormatter(
             missing_value_replacement='mode',
-            model_missing_values=False
+            missing_value_generation='random'
         )
 
         assert nt.missing_value_replacement == 'mode'
-        assert nt.model_missing_values is False
+        assert nt.missing_value_generation == 'random'
 
     def test__learn_rounding_digits_more_than_15_decimals(self):
         """Test the _learn_rounding_digits method with more than 15 decimals.
 
         If the data has more than 15 decimals, return None and raise warning.
         """
         # Setup
@@ -404,18 +404,22 @@
         )
         transformer._fit(data)
 
         # Asserts
         assert transformer._min_value == -5000
         assert transformer._max_value == 4000
 
-    def test__fit_model_missing_values(self):
-        """Test output_properties contains 'is_null' column when model_missing_values=True."""
+    def test__fit_missing_value_replacement_from_column(self):
+        """Test output_properties contains 'is_null' column.
+
+        When ``missing_value_generation`` is ``from_column`` an output property ``is_null`` should
+        exist.
+        """
         # Setup
-        transformer = FloatFormatter(model_missing_values=True)
+        transformer = FloatFormatter(missing_value_generation='from_column')
         data = pd.Series([1, np.nan])
 
         # Run
         transformer._fit(data)
 
         # Assert
         assert transformer.output_properties == {
@@ -766,21 +770,21 @@
 
 
 class TestGaussianNormalizer:
 
     def test___init__super_attrs(self):
         """super() arguments are properly passed and set as attributes."""
         ct = GaussianNormalizer(
-            model_missing_values=False,
+            missing_value_generation='random',
             learn_rounding_scheme=False,
             enforce_min_max_values=False
         )
 
         assert ct.missing_value_replacement == 'mean'
-        assert ct.model_missing_values is False
+        assert ct.missing_value_generation == 'random'
         assert ct.learn_rounding_scheme is False
         assert ct.enforce_min_max_values is False
 
     def test___init__str_distr(self):
         """If distribution is a str, it is resolved using the _DISTRIBUTIONS dict."""
         ct = GaussianNormalizer(distribution='gamma')
 
@@ -965,33 +969,22 @@
             call_value[0][0],
             np.array([0.0, 0.5, 1.0])
         )
         assert ct.output_properties == {
             None: {'sdtype': 'float', 'next_transformer': None},
         }
 
-    def test__fit_model_missing_values(self):
+    def test__fit_missing_value_generation_from_column(self):
         """Test the ``_fit`` method.
 
         Validate that ``_fit`` calls ``_get_univariate``.
-
-        Setup:
-            - create an instance of the ``GaussianNormalizer`` with ``model_missing_values``
-            set to True.
-            - mock the  ``_get_univariate`` method.
-
-        Input:
-            - a pandas series of float values.
-
-        Side effect:
-            - call the `_get_univariate`` method.
         """
         # Setup
         data = pd.Series([0.0, np.nan, 1.0])
-        ct = GaussianNormalizer(model_missing_values=True)
+        ct = GaussianNormalizer(missing_value_generation='from_column')
         ct._get_univariate = Mock()
 
         # Run
         ct._fit(data)
 
         # Assert
         ct._get_univariate.return_value.fit.assert_called_once()
@@ -1061,152 +1054,104 @@
         # Assert
         expected = np.array([-0.67449, 0, 0.67449])
         np.testing.assert_allclose(transformed_data, expected, rtol=1e-3)
 
     def test__transform(self):
         """Test the ``_transform`` method.
 
-        Validate that ``_transform`` produces the correct values when ``model_missing_values``
-        is True.
-
-        Setup:
-            - create an instance of the ``GaussianNormalizer``, where:
-                - ``self._univariate`` is a mock.
-                - ``self.null_transformer``  is a ``NullTransformer``.
-                - fit the ``self.null_transformer``.
-
-        Input:
-            - a pandas series of float values.
-
-        Ouput:
-            - a numpy array of the transformed data.
+        Validate that ``_transform`` produces the correct values when ``missing_value_generation``
+        is 'from_column'.
         """
         # Setup
         data = pd.Series([0.0, 1.0, 2.0, np.nan])
         ct = GaussianNormalizer()
         ct._univariate = Mock()
         ct._univariate.cdf.return_value = np.array([0.25, 0.5, 0.75, 0.5])
-        ct.null_transformer = NullTransformer(None, model_missing_values=True)
+        ct.null_transformer = NullTransformer('mean', missing_value_generation='from_column')
         ct.null_transformer.fit(data)
 
         # Run
         transformed_data = ct._transform(data)
 
         # Assert
         expected = np.array([
             [-0.67449, 0, 0.67449, 0],
             [0, 0, 0, 1.0]
         ]).T
-        np.testing.assert_allclose(transformed_data, expected, rtol=1e-3)
+        np.testing.assert_allclose(transformed_data, expected, rtol=1e-2)
 
-    def test__transform_model_missing_values_none(self):
+    def test__transform_missing_value_generation_is_random(self):
         """Test the ``_transform`` method.
 
-        Validate that ``_transform`` produces the correct values when ``model_missing_values``
-        is ``False``.
-
-        Setup:
-            - create an instance of the ``GaussianNormalizer``, where:
-                - ``self._univariate`` is a mock.
-                - ``self.null_transformer``  is a ``NullTransformer``.
-                - fit the ``self.null_transformer``.
-
-        Input:
-            - a pandas series of float values.
-
-        Ouput:
-            - a numpy array of the transformed data.
+        Validate that ``_transform`` produces the correct values when ``missing_value_generation``
+        is ``random``.
         """
         # Setup
         data = pd.Series([
             0.0, 1.0, 2.0, 1.0
         ])
         ct = GaussianNormalizer()
         ct._univariate = Mock()
         ct._univariate.cdf.return_value = np.array([0.25, 0.5, 0.75, 0.5])
-        ct.null_transformer = NullTransformer('mean', model_missing_values=False)
+        ct.null_transformer = NullTransformer('mean', missing_value_generation='random')
 
         # Run
         ct.null_transformer.fit(data)
         transformed_data = ct._transform(data)
 
         # Assert
         expected = np.array([-0.67449, 0, 0.67449, 0]).T
         np.testing.assert_allclose(transformed_data, expected, rtol=1e-3)
 
     def test__reverse_transform(self):
         """Test the ``_reverse_transform`` method.
 
         Validate that ``_reverse_transform`` produces the correct values when
-        ``model_missing_values`` is True.
-
-        Setup:
-            - create an instance of the ``GaussianNormalizer``, where:
-                - ``self._univariate`` is a mock.
-                - ``self.null_transformer``  is a ``NullTransformer``.
-                - fit the ``self.null_transformer``.
-
-        Input:
-            - a pandas series of float values.
-
-        Ouput:
-            - a numpy array of the transformed data.
+        ``missing_value_generation`` is 'from_column'.
         """
         # Setup
         data = np.array([
             [-0.67449, 0, 0.67449, 0],
             [0, 0, 0, 1.0],
         ]).T
         expected = pd.Series([
             0.0, 1.0, 2.0, np.nan
         ])
         ct = GaussianNormalizer()
         ct._univariate = Mock()
         ct._univariate.ppf.return_value = np.array([0.0, 1.0, 2.0, 1.0])
         ct.null_transformer = NullTransformer(
             missing_value_replacement='mean',
-            model_missing_values=True
+            missing_value_generation='from_column'
         )
 
         # Run
         ct.null_transformer.fit(expected)
         transformed_data = ct._reverse_transform(data)
 
         # Assert
         np.testing.assert_allclose(transformed_data, expected, rtol=1e-3)
 
-    def test__reverse_transform_model_missing_values_none(self):
+    def test__reverse_transform_missing_value_generation(self):
         """Test the ``_reverse_transform`` method.
 
         Validate that ``_reverse_transform`` produces the correct values when
-        ``model_missing_values`` is None.
-
-        Setup:
-            - create an instance of the ``GaussianNormalizer``, where:
-                - ``self._univariate`` is a mock.
-                - ``self.null_transformer``  is a ``NullTransformer``.
-                - fit the ``self.null_transformer``.
-
-        Input:
-            - a pandas series of float values.
-
-        Ouput:
-            - a numpy array of the transformed data.
+        ``missing_value_generation`` is 'random'.
         """
         # Setup
         data = pd.Series(
             [-0.67449, 0, 0.67449, 0]
         ).T
         expected = pd.Series([
             0.0, 1.0, 2.0, 1.0
         ])
         ct = GaussianNormalizer()
         ct._univariate = Mock()
         ct._univariate.ppf.return_value = np.array([0.0, 1.0, 2.0, 1.0])
-        ct.null_transformer = NullTransformer(None, model_missing_values=False)
+        ct.null_transformer = NullTransformer(None, missing_value_generation='random')
 
         # Run
         ct.null_transformer.fit(expected)
         transformed_data = ct._reverse_transform(data)
 
         # Assert
         np.testing.assert_allclose(transformed_data, expected, rtol=1e-3)
@@ -1274,35 +1219,22 @@
 
     @patch('rdt.transformers.numerical.BayesianGaussianMixture')
     def test__fit_missing_value_replacement(self, mock_bgm):
         """Test ``_fit`` with ``np.nan`` values.
 
         Validate that the method sets the internal variables to the correct values
         when given a pandas Series containing ``np.nan`` values.
-
-        Setup:
-            - patch a ``BayesianGaussianMixture`` with ``weights_`` containing two components
-            greater than the ``weight_threshold`` parameter.
-            - create an instance of the ``ClusterBasedNormalizer``.
-
-        Input:
-            - a pandas Series containing some ``np.nan`` values.
-
-        Side Effects:
-            - the sum of ``valid_component_indicator`` should equal to 2
-            (the number of ``weights_`` greater than the threshold).
-            - set the ``null_transformer`` appropriately.
         """
         # Setup
         bgm_instance = mock_bgm.return_value
         bgm_instance.weights_ = np.array([10.0, 5.0, 0.0])
         transformer = ClusterBasedNormalizer(
             max_clusters=10,
             weight_threshold=0.005,
-            model_missing_values=True
+            missing_value_generation='from_column'
         )
 
         data = pd.Series(np.random.random(size=100))
         mask = np.random.choice([1, 0], data.shape, p=[.1, .9]).astype(bool)
         data[mask] = np.nan
 
         # Run
@@ -1469,15 +1401,15 @@
             [9.74533917e-01, 2.54660826e-02, 0.0],
             [9.74533917e-01, 2.54660826e-02, 0.0],
             [7.88963658e-05, 9.99921104e-01, 0.0]
         ])
         transformer._bgm_transformer.predict_proba.return_value = probabilities
 
         transformer.valid_component_indicator = np.array([True, True, False])
-        transformer.null_transformer = NullTransformer(0.0, model_missing_values=True)
+        transformer.null_transformer = NullTransformer(0.0, missing_value_generation='from_column')
         data = pd.Series([0.01, np.nan, -0.01, -0.01, 0.0, 0.99, 0.97, np.nan, np.nan, 0.97])
 
         # Run
         transformer.null_transformer.fit(data)
         output = transformer._transform(data)
 
         # Asserts
@@ -1591,49 +1523,36 @@
             [1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
         ]).transpose()
         np.testing.assert_allclose(
             transformer._reverse_transform_helper.call_args[0][0],
             call_data
         )
 
-    def test__reverse_transform_missing_value_replacement_model_missing_values_is_true(self):
+    def test__reverse_transform_missing_value_replacement_missing_value_replacement_from_col(self):
         """Test ``_reverse_transform`` with ``np.nan`` values.
 
         Validate that the method correctly calls ``_reverse_transform_helper`` and produces the
         appropriate output when passed a numpy array containing ``np.nan`` values.
-
-        Setup:
-            - create an instance of the ``ClusterBasedNormalizer`` where the ``output_columns``
-            is a list of two columns.
-            - mock the `_reverse_transform_helper` with the appropriate return value.
-            - set ``null_transformer`` to ``NullTransformer`` with ``model_missing_values`` as
-              True, then fit it to a pandas Series.
-
-        Input:
-            - a numpy ndarray containing transformed ``np.nan`` values.
-
-        Ouput:
-            - a pandas Series with the reverse transformed data.
-
-        Side Effects:
-            - ``_reverse_transform_helper`` should be called once with the correct data.
         """
         # Setup
         transformer = ClusterBasedNormalizer(
-            model_missing_values=True,
+            missing_value_generation='from_column',
             max_clusters=3
         )
         transformer.output_columns = ['col.normalized', 'col.component']
         transformer._reverse_transform_helper = Mock()
         transformer._reverse_transform_helper.return_value = np.array([
             0.68351419, 0.67292805, 0.66234274, 0.66234274, 0.67292805,
             0.63579893, 0.62239389, 0.67292805, 0.67292805, 0.62239389
         ])
 
-        transformer.null_transformer = NullTransformer('mean', model_missing_values=True)
+        transformer.null_transformer = NullTransformer(
+            'mean',
+            missing_value_generation='from_column'
+        )
         transformer.null_transformer.fit(pd.Series([0, np.nan]))
 
         data = np.array([
             [-0.033, -0.046, -0.058, -0.058, -0.046, 0.134, 0.122, -0.046, -0.046, 0.122],
             [0, 0, 0, 0, 0, 1, 1, 0, 0, 1],
             [1, 1, 1, 1, 1, 0, 0, 0, 1, 0]
         ]).transpose()
@@ -1662,50 +1581,33 @@
         transformer._reverse_transform_helper.assert_called_once()
         np.testing.assert_allclose(
             transformer._reverse_transform_helper.call_args[0][0],
             call_data,
             rtol=1e-1
         )
 
-    def test__reverse_transform_missing_value_replacement_model_missing_values_is_false(self):
+    def test__reverse_transform_missing_value_replacement_missing_value_replacement_random(self):
         """Test ``_reverse_transform`` with ``np.nan`` values.
 
         Validate that the method correctly calls ``_reverse_transform_helper`` and produces the
         appropriate output when passed a numpy array containing ``np.nan`` values.
-
-        Setup:
-            - create an instance of the ``ClusterBasedNormalizer`` where the ``output_columns``
-            is a list of two columns.
-            - mock the `_reverse_transform_helper` with the appropriate return value.
-            - set ``null_transformer`` to ``NullTransformer`` with ``model_missing_values`` as
-              False, then fit it to a pandas Series.
-            - Mock the ``nul_transformer.reverse_transform`` method to get predicatable outputs.
-
-        Input:
-            - a numpy ndarray containing transformed ``np.nan`` values.
-
-        Ouput:
-            - a pandas Series with the reverse transformed data.
-
-        Side Effects:
-            - ``_reverse_transform_helper`` should be called once with the correct data.
         """
         # Setup
         transformer = ClusterBasedNormalizer(
-            model_missing_values=True,
+            missing_value_generation='from_column',
             max_clusters=3
         )
         transformer.output_columns = ['col.normalized', 'col.component']
         transformer._reverse_transform_helper = Mock()
         transformer._reverse_transform_helper.return_value = np.array([
             0.68351419, 0.67292805, 0.66234274, 0.66234274, 0.67292805,
             0.63579893, 0.62239389, 0.67292805, 0.67292805, 0.62239389
         ])
 
-        transformer.null_transformer = NullTransformer('mean', model_missing_values=False)
+        transformer.null_transformer = NullTransformer('mean', missing_value_generation='random')
         transformer.null_transformer.fit(pd.Series([0, np.nan]))
         transformer.null_transformer.reverse_transform = Mock()
         transformer.null_transformer.reverse_transform.return_value = np.array(
             [np.nan, np.nan, np.nan, np.nan, np.nan, 0.635799, np.nan, 0.672928, 0.672928, np.nan]
         )
 
         data = np.array([
```

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_text.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_utils.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

