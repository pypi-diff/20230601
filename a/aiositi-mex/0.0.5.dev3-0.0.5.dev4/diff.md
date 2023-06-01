# Comparing `tmp/aiositi-mex-0.0.5.dev3.tar.gz` & `tmp/aiositi-mex-0.0.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiositi-mex-0.0.5.dev3.tar", last modified: Thu Jun  1 02:38:08 2023, max compression
+gzip compressed data, was "aiositi-mex-0.0.5.dev4.tar", last modified: Thu Jun  1 02:55:39 2023, max compression
```

## Comparing `aiositi-mex-0.0.5.dev3.tar` & `aiositi-mex-0.0.5.dev4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.083967 aiositi-mex-0.0.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-01 02:38:08.083967 aiositi-mex-0.0.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.071967 aiositi-mex-0.0.5.dev3/aiositi_mex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-01 02:38:08.000000 aiositi-mex-0.0.5.dev3/aiositi_mex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-01 02:38:08.000000 aiositi-mex-0.0.5.dev3/aiositi_mex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:38:08.000000 aiositi-mex-0.0.5.dev3/aiositi_mex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 02:38:08.000000 aiositi-mex-0.0.5.dev3/aiositi_mex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 02:38:08.000000 aiositi-mex-0.0.5.dev3/aiositi_mex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-01 02:38:08.083967 aiositi-mex-0.0.5.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.071967 aiositi-mex-0.0.5.dev3/siti/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.075967 aiositi-mex-0.0.5.dev3/siti/http/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/http/oauth_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.075967 aiositi-mex-0.0.5.dev3/siti/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.075967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/catalogos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.075967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r01/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r01/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r01/reporte_111.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.075967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r08/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r08/reporte_843.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.079967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r10/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r10/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r10/reporte_10111.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r10/reporte_10121.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.079967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/reporte_13111.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/reporte_13161.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/reporte_13211.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/reporte_13221.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.079967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r24/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r24/reporte_2471.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r24/reporte_2472.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.079967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/reporte_2610.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/reporte_2611.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/reporte_2612.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/reporte_2613.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.079967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r27/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r27/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r27/reporte_2701.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.083967 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r36/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r36/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r36/reporte_3611.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r36/reporte_3612.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r36/reporte_3613.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/reportes.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/seguimiento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/resources/ifpe/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/siti/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.083967 aiositi-mex-0.0.5.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:08.083967 aiositi-mex-0.0.5.dev3/tests/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/tests/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/tests/http/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/tests/http/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-01 02:37:57.000000 aiositi-mex-0.0.5.dev3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.597195 aiositi-mex-0.0.5.dev4/aiositi_mex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-01 02:55:39.000000 aiositi-mex-0.0.5.dev4/aiositi_mex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-01 02:55:39.000000 aiositi-mex-0.0.5.dev4/aiositi_mex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:55:39.000000 aiositi-mex-0.0.5.dev4/aiositi_mex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 02:55:39.000000 aiositi-mex-0.0.5.dev4/aiositi_mex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 02:55:39.000000 aiositi-mex-0.0.5.dev4/aiositi_mex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-01 02:55:39.605195 aiositi-mex-0.0.5.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.597195 aiositi-mex-0.0.5.dev4/siti/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.597195 aiositi-mex-0.0.5.dev4/siti/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/http/oauth_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.597195 aiositi-mex-0.0.5.dev4/siti/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.597195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/catalogos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.597195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r01/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r01/reporte_111.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r08/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r08/reporte_843.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r10/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r10/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r10/reporte_10111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r10/reporte_10121.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/reporte_13111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/reporte_13161.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/reporte_13211.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/reporte_13221.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r24/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r24/reporte_2471.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r24/reporte_2472.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/reporte_2610.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/reporte_2611.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/reporte_2612.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/reporte_2613.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r27/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r27/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r27/reporte_2701.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r36/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r36/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r36/reporte_3611.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r36/reporte_3612.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r36/reporte_3613.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/reportes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/seguimiento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/resources/ifpe/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/siti/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:39.601195 aiositi-mex-0.0.5.dev4/tests/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/tests/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/tests/http/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/tests/http/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-01 02:55:31.000000 aiositi-mex-0.0.5.dev4/tests/test_utils.py
```

### Comparing `aiositi-mex-0.0.5.dev3/PKG-INFO` & `aiositi-mex-0.0.5.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiositi-mex
-Version: 0.0.5.dev3
+Version: 0.0.5.dev4
 Summary: Cliente para enviar reportes a la CNBV.
 Home-page: https://github.com/cuenca-mx/siti-python
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aiositi-mex-0.0.5.dev3/README.md` & `aiositi-mex-0.0.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/aiositi_mex.egg-info/PKG-INFO` & `aiositi-mex-0.0.5.dev4/aiositi_mex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiositi-mex
-Version: 0.0.5.dev3
+Version: 0.0.5.dev4
 Summary: Cliente para enviar reportes a la CNBV.
 Home-page: https://github.com/cuenca-mx/siti-python
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aiositi-mex-0.0.5.dev3/aiositi_mex.egg-info/SOURCES.txt` & `aiositi-mex-0.0.5.dev4/aiositi_mex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/setup.py` & `aiositi-mex-0.0.5.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/exc.py` & `aiositi-mex-0.0.5.dev4/siti/exc.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/http/client.py` & `aiositi-mex-0.0.5.dev4/siti/http/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import os
+import ssl
 from typing import Any, Dict, Optional
 
 import aiohttp
 from aiohttp.client_reqrep import ClientResponse
 
 from ..exc import ERROR_CODES, SitiError
 from .oauth_token import OAuthToken
 
 API_URL = 'https://sitiapi.cnbv.gob.mx:8243'
 API_URL_QA = 'https://sitiapiqa.cnbv.gob.mx:8243'
 
 SITI_DEMO = os.getenv('SITI_DEMO', 'false').lower() == 'true'
 
+ssl_context = ssl.create_default_context()
+ssl_context.check_hostname = False
+ssl_context.verify_mode = ssl.CERT_NONE
+
 
 class Session:
     consumer_key: str
     consumer_secret: str
     base_url: str = API_URL
     oauth_token: Optional[OAuthToken] = None
 
@@ -67,21 +72,23 @@
         # it will populate the token
         if not self.oauth_token or self.oauth_token.is_expired:
             self.oauth_token = OAuthToken.create(
                 self.base_url, self.consumer_key, self.consumer_secret
             )
         url = self.base_url + endpoint
         # establishing a maximum amount of simultaneous connections for async
-        conn = aiohttp.TCPConnector(limit=self._connection_pool_size)
+        conn = aiohttp.TCPConnector(
+            limit=self._connection_pool_size, ssl=ssl_context
+        )
         headers = dict(
             Authorization=f'Bearer {self.oauth_token.token}',  # type: ignore
             accept='application/json',
         )
         async with aiohttp.ClientSession(
-            connector=conn, headers=headers, verify_ssl=False,
+            connector=conn, headers=headers
         ) as session:
             async with session.request(
                 method,
                 url,
                 json=data,
                 **kwargs,
             ) as response:
```

### Comparing `aiositi-mex-0.0.5.dev3/siti/http/oauth_token.py` & `aiositi-mex-0.0.5.dev4/siti/http/oauth_token.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/base.py` & `aiositi-mex-0.0.5.dev4/siti/resources/base.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/__init__.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/__init__.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/base.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/base.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/catalogos.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/catalogos.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r01/reporte_111.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r01/reporte_111.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r08/reporte_843.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r08/reporte_843.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r10/reporte_10111.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r10/reporte_10111.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r10/reporte_10121.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r10/reporte_10121.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/reporte_13111.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/reporte_13111.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/reporte_13161.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/reporte_13161.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/reporte_13211.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/reporte_13211.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r13/reporte_13221.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r13/reporte_13221.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r24/reporte_2471.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r24/reporte_2471.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r24/reporte_2472.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r24/reporte_2472.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/reporte_2610.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/reporte_2610.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/reporte_2611.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/reporte_2611.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/reporte_2612.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/reporte_2612.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 class IdentificadorModuloEstablecimiento(Resource):
     tipo_movimiento: str
     clave_modulo_establecimiento: str
     rfc_modulo_establecimiento: str
     clave_localidad_modulo_establecimiento: Optional[str]
     clave_estado_modulo_establecimiento: Optional[str]
-    clave_municipio_moldulo_establecimiento: Optional[str]  # la api dice moldulo
+    clave_municipio_moldulo_establecimiento: Optional[
+        str
+    ]  # la api dice moldulo
     codigo_postal_modulo_establecimiento: Optional[str]
     latitud_ubicacion_modulo_establecimiento: Optional[str]
     longitud_ubicacion_modulo_establecimiento: Optional[str]
 
 
 class BajaModuloEstablecimiento(Resource):
     causa_baja_modulo_establecimiento: str
```

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r26/reporte_2613.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r26/reporte_2613.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r27/reporte_2701.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r27/reporte_2701.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r36/reporte_3611.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r36/reporte_3611.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r36/reporte_3612.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r36/reporte_3612.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/r36/reporte_3613.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/r36/reporte_3613.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/reportes.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/reportes.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/resources/ifpe/types.py` & `aiositi-mex-0.0.5.dev4/siti/resources/ifpe/types.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/siti/utils.py` & `aiositi-mex-0.0.5.dev4/siti/utils.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/tests/http/test_client.py` & `aiositi-mex-0.0.5.dev4/tests/http/test_client.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.5.dev3/tests/test_utils.py` & `aiositi-mex-0.0.5.dev4/tests/test_utils.py`

 * *Files identical despite different names*

