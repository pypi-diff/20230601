# Comparing `tmp/StrangeSerializerLab3-6.0.tar.gz` & `tmp/StrangeSerializerLab3-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StrangeSerializerLab3-6.0.tar", last modified: Thu Jun  1 10:26:40 2023, max compression
+gzip compressed data, was "StrangeSerializerLab3-7.0.tar", last modified: Thu Jun  1 10:31:18 2023, max compression
```

## Comparing `StrangeSerializerLab3-6.0.tar` & `StrangeSerializerLab3-7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:26:40.681960 StrangeSerializerLab3-6.0/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:26:40.681960 StrangeSerializerLab3-6.0/PKG-INFO
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:26:40.677960 StrangeSerializerLab3-6.0/StrangeSerializerLab3/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)     7080 2023-06-01 07:24:02.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3/AdditionalFunctions.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      504 2023-06-01 10:21:20.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeFactory.py
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:26:40.677960 StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeJSON/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      588 2023-06-01 09:39:28.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeJSON/StrangeJsonSerializer.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)     1442 2023-06-01 08:44:19.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeJSON/parser.py
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:26:40.677960 StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeXML/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      600 2023-06-01 09:39:28.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeXML/StrangeXmlSerializer.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)     3114 2023-06-01 08:46:03.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeXML/parser.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      256 2023-06-01 10:24:04.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3/__init__.py
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:26:40.677960 StrangeSerializerLab3-6.0/StrangeSerializerLab3.egg-info/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:26:40.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3.egg-info/PKG-INFO
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      510 2023-06-01 10:26:40.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3.egg-info/SOURCES.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)        1 2023-06-01 10:26:40.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3.egg-info/dependency_links.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)       89 2023-06-01 10:26:40.000000 StrangeSerializerLab3-6.0/StrangeSerializerLab3.egg-info/top_level.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)       38 2023-06-01 10:26:40.681960 StrangeSerializerLab3-6.0/setup.cfg
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      486 2023-06-01 10:26:37.000000 StrangeSerializerLab3-6.0/setup.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:31:18.471024 StrangeSerializerLab3-7.0/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:31:18.471024 StrangeSerializerLab3-7.0/PKG-INFO
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:31:18.467024 StrangeSerializerLab3-7.0/StrangeSerializerLab3/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)     7080 2023-06-01 07:24:02.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3/AdditionalFunctions.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      415 2023-06-01 10:30:38.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeFactory.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:31:18.467024 StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeJSON/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      588 2023-06-01 09:39:28.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeJSON/StrangeJsonSerializer.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)     1442 2023-06-01 08:44:19.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeJSON/parser.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:31:18.471024 StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeXML/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      600 2023-06-01 09:39:28.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeXML/StrangeXmlSerializer.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)     3114 2023-06-01 08:46:03.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeXML/parser.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      256 2023-06-01 10:24:04.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3/__init__.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:31:18.467024 StrangeSerializerLab3-7.0/StrangeSerializerLab3.egg-info/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:31:18.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3.egg-info/PKG-INFO
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      510 2023-06-01 10:31:18.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)        1 2023-06-01 10:31:18.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)       89 2023-06-01 10:31:18.000000 StrangeSerializerLab3-7.0/StrangeSerializerLab3.egg-info/top_level.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)       38 2023-06-01 10:31:18.471024 StrangeSerializerLab3-7.0/setup.cfg
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      486 2023-06-01 10:31:16.000000 StrangeSerializerLab3-7.0/setup.py
```

### Comparing `StrangeSerializerLab3-6.0/StrangeSerializerLab3/AdditionalFunctions.py` & `StrangeSerializerLab3-7.0/StrangeSerializerLab3/AdditionalFunctions.py`

 * *Files identical despite different names*

### Comparing `StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeJSON/StrangeJsonSerializer.py` & `StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeJSON/StrangeJsonSerializer.py`

 * *Files identical despite different names*

### Comparing `StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeJSON/parser.py` & `StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeJSON/parser.py`

 * *Files identical despite different names*

### Comparing `StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeXML/StrangeXmlSerializer.py` & `StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeXML/StrangeXmlSerializer.py`

 * *Files identical despite different names*

### Comparing `StrangeSerializerLab3-6.0/StrangeSerializerLab3/StrangeXML/parser.py` & `StrangeSerializerLab3-7.0/StrangeSerializerLab3/StrangeXML/parser.py`

 * *Files identical despite different names*

