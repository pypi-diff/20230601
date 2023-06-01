# Comparing `tmp/dmodel-0.0.1.tar.gz` & `tmp/dmodel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmodel-0.0.1.tar", max compression
+gzip compressed data, was "dmodel-0.0.2.tar", max compression
```

## Comparing `dmodel-0.0.1.tar` & `dmodel-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,22 @@
--rw-r--r--   0        0        0        0 2023-05-25 15:35:16.528817 dmodel-0.0.1/dmodel/__init__.py
--rw-r--r--   0        0        0      302 2023-05-25 15:36:26.201111 dmodel-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      512 2023-05-25 15:36:34.539816 dmodel-0.0.1/setup.py
--rw-r--r--   0        0        0      312 2023-05-25 15:36:34.540154 dmodel-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      153 2023-05-31 04:11:20.266510 dmodel-0.0.2/dmodel/__init__.py
+-rw-r--r--   0        0        0     2059 2023-06-01 03:35:13.320889 dmodel-0.0.2/dmodel/context.py
+-rw-r--r--   0        0        0     3892 2023-05-31 15:11:03.249331 dmodel-0.0.2/dmodel/descriptors.py
+-rw-r--r--   0        0        0      405 2023-05-31 04:15:24.383229 dmodel-0.0.2/dmodel/enums.py
+-rw-r--r--   0        0        0     6520 2023-05-31 00:03:46.089982 dmodel-0.0.2/dmodel/form.py
+-rw-r--r--   0        0        0     9023 2023-06-01 03:36:17.472594 dmodel-0.0.2/dmodel/model.py
+-rw-r--r--   0        0        0      109 2023-05-31 04:24:50.902840 dmodel-0.0.2/dmodel/models/__init__.py
+-rw-r--r--   0        0        0      297 2023-05-31 04:24:51.214456 dmodel-0.0.2/dmodel/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1041 2023-05-31 04:15:24.657420 dmodel-0.0.2/dmodel/models/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0     1916 2023-05-31 04:11:20.562201 dmodel-0.0.2/dmodel/models/__pycache__/person.cpython-39.pyc
+-rw-r--r--   0        0        0     3638 2023-05-31 15:10:08.320435 dmodel-0.0.2/dmodel/models/__pycache__/profile.cpython-39.pyc
+-rw-r--r--   0        0        0     1749 2023-06-01 01:53:47.629907 dmodel-0.0.2/dmodel/models/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     1552 2023-05-31 05:08:13.196011 dmodel-0.0.2/dmodel/models/__pycache__/visit.cpython-39.pyc
+-rw-r--r--   0        0        0      613 2023-05-31 04:15:24.387073 dmodel-0.0.2/dmodel/models/facility.py
+-rw-r--r--   0        0        0     1222 2023-05-31 04:11:20.271322 dmodel-0.0.2/dmodel/models/person.py
+-rw-r--r--   0        0        0     2598 2023-05-31 15:10:08.078964 dmodel-0.0.2/dmodel/models/profile.py
+-rw-r--r--   0        0        0     1164 2023-05-31 15:17:09.448073 dmodel-0.0.2/dmodel/models/user.py
+-rw-r--r--   0        0        0     1397 2023-05-31 05:08:12.916476 dmodel-0.0.2/dmodel/models/visit.py
+-rw-r--r--   0        0        0      662 2023-05-31 04:18:41.392670 dmodel-0.0.2/dmodel/regex.py
+-rw-r--r--   0        0        0      402 2023-05-31 03:37:42.045739 dmodel-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      728 2023-06-01 03:39:34.651027 dmodel-0.0.2/setup.py
+-rw-r--r--   0        0        0      517 2023-06-01 03:39:34.651236 dmodel-0.0.2/PKG-INFO
```

