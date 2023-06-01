# Comparing `tmp/arithmetica-py-1.0.209.tar.gz` & `tmp/arithmetica-py-1.0.210.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.209.tar", last modified: Wed May 31 23:40:55 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.210.tar", last modified: Thu Jun  1 07:16:41 2023, max compression
```

## Comparing `arithmetica-py-1.0.209.tar` & `arithmetica-py-1.0.210.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:40:55.945339 arithmetica-py-1.0.209/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-31 23:40:41.000000 arithmetica-py-1.0.209/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-31 23:40:55.945339 arithmetica-py-1.0.209/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-05-31 23:40:41.000000 arithmetica-py-1.0.209/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:40:55.945339 arithmetica-py-1.0.209/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-31 23:40:55.000000 arithmetica-py-1.0.209/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 23:40:55.000000 arithmetica-py-1.0.209/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:40:55.000000 arithmetica-py-1.0.209/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 23:40:55.000000 arithmetica-py-1.0.209/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:40:55.945339 arithmetica-py-1.0.209/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-31 23:40:41.000000 arithmetica-py-1.0.209/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:40:55.941339 arithmetica-py-1.0.209/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:40:55.945339 arithmetica-py-1.0.209/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   186606 2023-05-31 23:40:55.000000 arithmetica-py-1.0.209/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-31 23:40:55.000000 arithmetica-py-1.0.209/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-31 23:40:41.000000 arithmetica-py-1.0.209/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 23:40:55.000000 arithmetica-py-1.0.209/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-01 07:16:24.000000 arithmetica-py-1.0.210/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-01 07:16:24.000000 arithmetica-py-1.0.210/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-01 07:16:24.000000 arithmetica-py-1.0.210/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   186606 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-01 07:16:24.000000 arithmetica-py-1.0.210/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.209/LICENSE` & `arithmetica-py-1.0.210/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.209/README.md` & `arithmetica-py-1.0.210/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.209/setup.py` & `arithmetica-py-1.0.210/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.209/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.210/src/python-module/libarithmetica.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.209/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.210/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.209/src/python-module/module.c` & `arithmetica-py-1.0.210/src/python-module/module.c`

 * *Files identical despite different names*

