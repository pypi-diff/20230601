# Comparing `tmp/hestia-earth-orchestrator-0.5.3.tar.gz` & `tmp/hestia-earth-orchestrator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-orchestrator-0.5.3.tar", last modified: Fri May 12 13:24:02 2023, max compression
+gzip compressed data, was "hestia-earth-orchestrator-0.6.0.tar", last modified: Thu Jun  1 14:20:19 2023, max compression
```

## Comparing `hestia-earth-orchestrator-0.5.3.tar` & `hestia-earth-orchestrator-0.6.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.734708 hestia-earth-orchestrator-0.5.3/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2380 2023-05-12 13:24:02.733791 hestia-earth-orchestrator-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.720957 hestia-earth-orchestrator-0.5.3/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.722790 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.722790 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/config/
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.723707 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.723707 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/emissions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/emissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/emissions/deleted.py
--rw-rw-rw-   0 root         (0) root         (0)     4497 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.724624 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.725540 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/
--rw-rw-rw-   0 root         (0) root         (0)     1416 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/merge_append.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/merge_default.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/merge_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2659 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/merge_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.727374 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/run/
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/run/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2875 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/run/add_key_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/run/always.py
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.728291 hestia-earth-orchestrator-0.5.3/hestia_earth_orchestrator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2380 2023-05-12 13:24:02.000000 hestia-earth-orchestrator-0.5.3/hestia_earth_orchestrator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-12 13:24:02.000000 hestia-earth-orchestrator-0.5.3/hestia_earth_orchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 13:24:02.000000 hestia-earth-orchestrator-0.5.3/hestia_earth_orchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-12 13:24:02.000000 hestia-earth-orchestrator-0.5.3/hestia_earth_orchestrator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-12 13:24:02.000000 hestia-earth-orchestrator-0.5.3/hestia_earth_orchestrator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 13:24:02.734708 hestia-earth-orchestrator-0.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.719123 hestia-earth-orchestrator-0.5.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.730124 hestia-earth-orchestrator-0.5.3/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.731041 hestia-earth-orchestrator-0.5.3/tests/models/emissions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/models/emissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/models/emissions/test_deleted.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/models/test_transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.731041 hestia-earth-orchestrator-0.5.3/tests/strategies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.732874 hestia-earth-orchestrator-0.5.3/tests/strategies/merge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/merge/test_merge_append.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/merge/test_merge_default.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/merge/test_merge_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3207 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/merge/test_merge_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:24:02.733791 hestia-earth-orchestrator-0.5.3/tests/strategies/run/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/run/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3236 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/run/test_add_blank_node_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/run/test_add_key_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-12 13:23:46.000000 hestia-earth-orchestrator-0.5.3/tests/strategies/run/test_always.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.032527 hestia-earth-orchestrator-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-06-01 14:20:19.031527 hestia-earth-orchestrator-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.023527 hestia-earth-orchestrator-0.6.0/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.024527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.024527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/config/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.025527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.025527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/emissions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/emissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/emissions/deleted.py
+-rw-rw-rw-   0 root         (0) root         (0)     4128 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/transformations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.025527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.026527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_append.py
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2659 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.027527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/add_key_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/always.py
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.028527 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 14:20:19.032527 hestia-earth-orchestrator-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.022527 hestia-earth-orchestrator-0.6.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.029527 hestia-earth-orchestrator-0.6.0/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.029527 hestia-earth-orchestrator-0.6.0/tests/models/emissions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/models/emissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/models/emissions/test_deleted.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/models/test_transformations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.029527 hestia-earth-orchestrator-0.6.0/tests/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.030527 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_append.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3207 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.031527 hestia-earth-orchestrator-0.6.0/tests/strategies/run/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/run/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/run/test_add_blank_node_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/run/test_add_key_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/run/test_always.py
```

### Comparing `hestia-earth-orchestrator-0.5.3/LICENSE` & `hestia-earth-orchestrator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/PKG-INFO` & `hestia-earth-orchestrator-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-orchestrator
-Version: 0.5.3
+Version: 0.6.0
 Summary: Hestia's module to orchestrate the models.
 Home-page: https://gitlab.com/hestia-earth/hestia-engine-orchestrator
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-orchestrator-0.5.3/README.md` & `hestia-earth-orchestrator-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/__init__.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/log.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/__init__.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/emissions/deleted.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/emissions/deleted.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/models/transformations.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/transformations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from copy import deepcopy
 from functools import reduce
 from hestia_earth.schema import CompletenessJSONLD
 from hestia_earth.utils.lookup import download_lookup, get_table_value, column_name
+from hestia_earth.models.transformation.input.utils import replace_input_field
+from hestia_earth.models.utils.transformation import previous_transformation
+from hestia_earth.models.utils.product import find_by_product
 
 from . import run as run_node, _import_model
-from hestia_earth.orchestrator.utils import _new_practice, _filter_by_keys, find_term_match
+from hestia_earth.orchestrator.utils import _new_practice, _filter_by_keys
 
 
 def _full_completeness():
     completeness = CompletenessJSONLD().to_dict()
     keys = list(completeness.keys())
     keys.remove('@type')
     return {
@@ -49,42 +52,30 @@
     ]
     return data
 
 
 def _run_models(cycle: dict, transformation: dict, models: list):
     data = _convert_transformation(cycle, transformation)
     result = run_node(data, models)
-    return _filter_by_keys(result, ['term', 'inputs', 'products', 'emissions'])
-
-
-def _previous_transformation(cycle: dict, transformations: list, transformation: dict):
-    term_id = transformation.get('previousTransformationTerm', {}).get('@id')
-    return next(
-        (v for v in transformations if v.get('term', {}).get('@id') == term_id),
-        cycle
-    )
+    return _filter_by_keys(result, [
+        'transformationId', 'term', 'inputs', 'products', 'emissions'
+    ])
 
 
-def _apply_transformation_share(previous: dict, current: dict, is_first_transformation: bool = False):
+def _apply_transformation_share(previous: dict, current: dict):
     share = current.get('transformedShare', 100)
-    products = previous.get('products', [])
-
-    def replace_field(input: dict, field: str):
-        term_id = input.get('term', {}).get('@id')
-        product_value = find_term_match(products, term_id).get(field, [])
-        should_replace = len(product_value) > 0 and (not is_first_transformation or len(input.get('value', [])) == 0)
-        return {field: [v * share / 100 for v in product_value]} if should_replace else {}
 
     def replace_value(input: dict):
+        product = find_by_product(previous, input)
         return {
             **input,
-            **replace_field(input, 'value'),
-            **replace_field(input, 'min'),
-            **replace_field(input, 'max'),
-            **replace_field(input, 'sd')
+            **replace_input_field(previous, None, input, product, share, 'value'),
+            **replace_input_field(previous, None, input, product, share, 'min'),
+            **replace_input_field(previous, None, input, product, share, 'max'),
+            **replace_input_field(previous, None, input, product, share, 'sd')
         }
 
     return {**current, 'inputs': list(map(replace_value, current.get('inputs', [])))}
 
 
 def _add_excreta_inputs(previous: dict, current: dict):
     run = _import_model('transformation.input.excreta').get('run')
@@ -96,19 +87,19 @@
     # model will add the inputs directly in the transformation
     run(cycle)
     return current
 
 
 def _run_transformation(cycle: dict, models: list):
     def run(transformations: list, transformation: dict):
-        previous = _previous_transformation(cycle, transformations, transformation)
-        transformation = _apply_transformation_share(previous, transformation, len(transformations) == 0)
+        previous = previous_transformation(cycle, transformations, transformation)
+        transformation = _apply_transformation_share(previous, transformation)
         # add missing excreta Input when relevant and apply the value share as well
         transformation = _add_excreta_inputs(previous, transformation)
-        transformation = _apply_transformation_share(previous, transformation, len(transformations) == 0)
+        transformation = _apply_transformation_share(previous, transformation)
         transformation = _run_models(cycle, transformation, models)
         return transformations + [transformation]
     return run
 
 
 def run(models: list, cycle: dict):
     transformations = cycle.get('transformations', [])
```

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/__init__.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/merge_append.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_append.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/merge_list.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_list.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/merge/merge_node.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_node.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth/orchestrator/utils.py` & `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth_orchestrator.egg-info/PKG-INFO` & `hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-orchestrator
-Version: 0.5.3
+Version: 0.6.0
 Summary: Hestia's module to orchestrate the models.
 Home-page: https://gitlab.com/hestia-earth/hestia-engine-orchestrator
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-orchestrator-0.5.3/hestia_earth_orchestrator.egg-info/SOURCES.txt` & `hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/setup.py` & `hestia-earth-orchestrator-0.6.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
-REQUIRES = (HERE / "requirements.txt").read_text().splitlines()
+
+def parse_require(path: pathlib.Path): return path.read_text().splitlines()
+
+
+REQUIRES = parse_require(HERE / "requirements.txt") + parse_require(HERE / "requirements-models.txt")
 
 # This call to setup() does all the work
 setup(
     name='hestia-earth-orchestrator',
     version=VERSION,
     description="Hestia's module to orchestrate the models.",
     long_description=README,
```

### Comparing `hestia-earth-orchestrator-0.5.3/tests/models/emissions/test_deleted.py` & `hestia-earth-orchestrator-0.6.0/tests/models/emissions/test_deleted.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/tests/models/test_transformations.py` & `hestia-earth-orchestrator-0.6.0/tests/models/test_transformations.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/tests/strategies/merge/test_merge_append.py` & `hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_append.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/tests/strategies/merge/test_merge_list.py` & `hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_list.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/tests/strategies/merge/test_merge_node.py` & `hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_node.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.5.3/tests/strategies/run/test_add_blank_node_if_missing.py` & `hestia-earth-orchestrator-0.6.0/tests/strategies/run/test_add_blank_node_if_missing.py`

 * *Files identical despite different names*

