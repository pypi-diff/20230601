# Comparing `tmp/StrangeSerializerLab3-3.0.tar.gz` & `tmp/StrangeSerializerLab3-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StrangeSerializerLab3-3.0.tar", last modified: Thu Jun  1 10:19:58 2023, max compression
+gzip compressed data, was "StrangeSerializerLab3-4.0.tar", last modified: Thu Jun  1 10:21:30 2023, max compression
```

## Comparing `StrangeSerializerLab3-3.0.tar` & `StrangeSerializerLab3-4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:19:58.904687 StrangeSerializerLab3-3.0/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:19:58.900687 StrangeSerializerLab3-3.0/PKG-INFO
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:19:58.896687 StrangeSerializerLab3-3.0/StrangeSerializerLab3/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)     7080 2023-06-01 07:24:02.000000 StrangeSerializerLab3-3.0/StrangeSerializerLab3/AdditionalFunctions.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      502 2023-06-01 09:39:28.000000 StrangeSerializerLab3-3.0/StrangeSerializerLab3/StrangeFactory.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      249 2023-06-01 10:19:47.000000 StrangeSerializerLab3-3.0/StrangeSerializerLab3/__init__.py
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:19:58.900687 StrangeSerializerLab3-3.0/StrangeSerializerLab3.egg-info/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:19:58.000000 StrangeSerializerLab3-3.0/StrangeSerializerLab3.egg-info/PKG-INFO
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      307 2023-06-01 10:19:58.000000 StrangeSerializerLab3-3.0/StrangeSerializerLab3.egg-info/SOURCES.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)        1 2023-06-01 10:19:58.000000 StrangeSerializerLab3-3.0/StrangeSerializerLab3.egg-info/dependency_links.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)       22 2023-06-01 10:19:58.000000 StrangeSerializerLab3-3.0/StrangeSerializerLab3.egg-info/top_level.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)       38 2023-06-01 10:19:58.904687 StrangeSerializerLab3-3.0/setup.cfg
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      413 2023-06-01 10:19:53.000000 StrangeSerializerLab3-3.0/setup.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:21:30.317237 StrangeSerializerLab3-4.0/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:21:30.317237 StrangeSerializerLab3-4.0/PKG-INFO
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:21:30.317237 StrangeSerializerLab3-4.0/StrangeSerializerLab3/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)     7080 2023-06-01 07:24:02.000000 StrangeSerializerLab3-4.0/StrangeSerializerLab3/AdditionalFunctions.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      504 2023-06-01 10:21:20.000000 StrangeSerializerLab3-4.0/StrangeSerializerLab3/StrangeFactory.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      251 2023-06-01 10:21:20.000000 StrangeSerializerLab3-4.0/StrangeSerializerLab3/__init__.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:21:30.317237 StrangeSerializerLab3-4.0/StrangeSerializerLab3.egg-info/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:21:30.000000 StrangeSerializerLab3-4.0/StrangeSerializerLab3.egg-info/PKG-INFO
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      307 2023-06-01 10:21:30.000000 StrangeSerializerLab3-4.0/StrangeSerializerLab3.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)        1 2023-06-01 10:21:30.000000 StrangeSerializerLab3-4.0/StrangeSerializerLab3.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)       22 2023-06-01 10:21:30.000000 StrangeSerializerLab3-4.0/StrangeSerializerLab3.egg-info/top_level.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)       38 2023-06-01 10:21:30.317237 StrangeSerializerLab3-4.0/setup.cfg
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      413 2023-06-01 10:21:26.000000 StrangeSerializerLab3-4.0/setup.py
```

### Comparing `StrangeSerializerLab3-3.0/StrangeSerializerLab3/AdditionalFunctions.py` & `StrangeSerializerLab3-4.0/StrangeSerializerLab3/AdditionalFunctions.py`

 * *Files identical despite different names*

