# Comparing `tmp/slice_bin-0.1.0.tar.gz` & `tmp/slice_bin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slice_bin-0.1.0.tar", max compression
+gzip compressed data, was "slice_bin-0.1.1.tar", max compression
```

## Comparing `slice_bin-0.1.0.tar` & `slice_bin-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       15 2023-06-01 13:21:56.534499 slice_bin-0.1.0/README.md
--rw-r--r--   0        0        0      402 2023-06-01 13:38:31.201698 slice_bin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 13:25:01.651727 slice_bin-0.1.0/src/slice_bin/__init__.py
--rw-r--r--   0        0        0     1754 2023-06-01 15:57:01.236345 slice_bin-0.1.0/src/slice_bin/__main__.py
--rw-r--r--   0        0        0     1290 2023-06-01 15:56:11.488251 slice_bin-0.1.0/src/slice_bin/lib.py
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 slice_bin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-01 16:19:30.344061 slice_bin-0.1.1/LICENSE
+-rw-r--r--   0        0        0      653 2023-06-01 16:18:51.648723 slice_bin-0.1.1/README.md
+-rw-r--r--   0        0        0      402 2023-06-01 16:19:10.981393 slice_bin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 13:25:01.651727 slice_bin-0.1.1/src/slice_bin/__init__.py
+-rw-r--r--   0        0        0     1754 2023-06-01 15:57:01.236345 slice_bin-0.1.1/src/slice_bin/__main__.py
+-rw-r--r--   0        0        0     1290 2023-06-01 15:56:11.488251 slice_bin-0.1.1/src/slice_bin/lib.py
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 slice_bin-0.1.1/PKG-INFO
```

### Comparing `slice_bin-0.1.0/src/slice_bin/__main__.py` & `slice_bin-0.1.1/src/slice_bin/__main__.py`

 * *Files identical despite different names*

### Comparing `slice_bin-0.1.0/src/slice_bin/lib.py` & `slice_bin-0.1.1/src/slice_bin/lib.py`

 * *Files identical despite different names*

