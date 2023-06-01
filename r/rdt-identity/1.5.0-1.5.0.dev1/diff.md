# Comparing `tmp/rdt_identity-1.5.0.tar.gz` & `tmp/rdt_identity-1.5.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.5.0.tar", last modified: Thu Jun  1 21:46:43 2023, max compression
+gzip compressed data, was "rdt_identity-1.5.0.dev1.tar", last modified: Thu Jun  1 20:13:51 2023, max compression
```

## Comparing `rdt_identity-1.5.0.tar` & `rdt_identity-1.5.0.dev1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.043309 rdt_identity-1.5.0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8009 2023-06-01 21:46:43.043414 rdt_identity-1.5.0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.032284 rdt_identity-1.5.0/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.032346 rdt_identity-1.5.0/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.032408 rdt_identity-1.5.0/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.035672 rdt_identity-1.5.0/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1590 2023-06-01 21:46:43.044003 rdt_identity-1.5.0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4178 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.036167 rdt_identity-1.5.0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.032649 rdt_identity-1.5.0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.036934 rdt_identity-1.5.0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.037461 rdt_identity-1.5.0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.038565 rdt_identity-1.5.0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.038854 rdt_identity-1.5.0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3319 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.5.0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4094 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10153 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.5.0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.039308 rdt_identity-1.5.0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.5.0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.039596 rdt_identity-1.5.0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.5.0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.040093 rdt_identity-1.5.0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5780 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.041892 rdt_identity-1.5.0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.042048 rdt_identity-1.5.0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.042368 rdt_identity-1.5.0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-01 21:46:43.043120 rdt_identity-1.5.0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.5.0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.5.0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.5.0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.5.0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17137 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19791 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt_identity-1.5.0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.5.0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.5.0/tests/unit/transformers/test_utils.py
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

### Comparing `rdt_identity-1.5.0/CONTRIBUTING.rst` & `rdt_identity-1.5.0.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/HISTORY.md` & `rdt_identity-1.5.0.dev1/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,9 @@
 # History
 
-## 1.5.0 - 2023-06-01
-
-This release adds a new parameter called `missing_value_generation` to the initialization of certain transformers to specify how missing values should be created. The parameter can be used in the `FloatFormatter`, `BinaryEncoder`, `UnixTimestampEncoder`, `OptimizedTimestampEncoder`, `GaussianNormalizer` and `ClusterBasedNormalizer`. Additionally, it fixes a bug that was causing every column that had nulls to generate them in the same place.
-
-### Deprecations
-
-* The `model_missing_values` parameter is being deprecated in favor of the new `missing_value_generation` parameter.
-
-### Bugs
-
-* Fix randomization when creating null values - Issue [#639](https://github.com/sdv-dev/RDT/issues/639) by @fealho
-
-### New Features
-
-* Allow a no-op handling strategy for missing values (nulls) - Issue [#644](https://github.com/sdv-dev/RDT/issues/644) by @pvk-developer
-* Add add-on detection for premium transformers - Issue [#646](https://github.com/sdv-dev/RDT/issues/646) by @frances-h
-
-### Maintenance
-
-* Performance tests still fragile - Issue [#641](https://github.com/sdv-dev/RDT/issues/641) by @fealho
-* Investigate removing quality tests - Issue [#642](https://github.com/sdv-dev/RDT/issues/642) by @amontanez24
-
 ## 1.4.2 - 2023-05-02
 
 This release fixes a bug that caused datetime and numerical transformers to crash if a column was all NaNs. Additionally, it adds support for Pandas 2.0!
 
 ### Bugs
 
 * Numerical & datetime transformers crash if the entire column is null - Issue [#637](https://github.com/sdv-dev/RDT/issues/637) by @fraces-h
```

### Comparing `rdt_identity-1.5.0/LICENSE` & `rdt_identity-1.5.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/PKG-INFO` & `rdt_identity-1.5.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.5.0
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
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.5.0 Summary: Reversible
-Data Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo,
-Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt,rdt_identity
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Developers Classifier: License :: Free for non-commercial use Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.7,<3.12 Description-Content-Type:
-text/markdown License-File: LICENSE License-File: AUTHORS.rst
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.5.0.dev1 Summary:
+Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
+DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
+rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: Free for non-commercial
+use Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Requires-Python: >=3.7,<3.12
+Description-Content-Type: text/markdown License-File: LICENSE License-File:
+AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
                   %20Alpha-yellow)](https://pypi.org/search/
     ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
    img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
```

### Comparing `rdt_identity-1.5.0/README.md` & `rdt_identity-1.5.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/RELEASE.md` & `rdt_identity-1.5.0.dev1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.5.0.dev1/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/setup.cfg` & `rdt_identity-1.5.0.dev1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.5.0
+current_version = 1.5.0.dev1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt_identity-1.5.0/setup.py` & `rdt_identity-1.5.0.dev1/setup.py`

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
-    version='1.5.0',
+    version='1.5.0.dev1',
     zip_safe=False,
 )
```

### Comparing `rdt_identity-1.5.0/tests/__init__.py` & `rdt_identity-1.5.0.dev1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/code_style.py` & `rdt_identity-1.5.0.dev1/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/contributing.py` & `rdt_identity-1.5.0.dev1/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/datasets/tests/test_utils.py` & `rdt_identity-1.5.0.dev1/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.5.0.dev1/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/test_transformers.py` & `rdt_identity-1.5.0.dev1/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/transformers/test_base.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/integration/transformers/test_text.py` & `rdt_identity-1.5.0.dev1/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/performance/test_performance.py` & `rdt_identity-1.5.0.dev1/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/performance/tests/test_profiling.py` & `rdt_identity-1.5.0.dev1/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/test___init__.py` & `rdt_identity-1.5.0.dev1/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.5.0.dev1/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test___init__.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test_base.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test_null.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test_text.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.0/tests/unit/transformers/test_utils.py` & `rdt_identity-1.5.0.dev1/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

