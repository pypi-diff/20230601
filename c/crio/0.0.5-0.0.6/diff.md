# Comparing `tmp/crio-0.0.5.tar.gz` & `tmp/crio-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\work\crio_proj\dist\.tmp-sfd9yqtr\crio-0.0.5.tar", last modified: Wed May 31 07:50:27 2023, max compression
+gzip compressed data, was "C:\work\crio_proj\dist\.tmp-yqx2yr97\crio-0.0.6.tar", last modified: Thu Jun  1 03:20:10 2023, max compression
```

## Comparing `crio-0.0.5.tar` & `crio-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:50:27.788257 crio-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-02-21 00:14:59.000000 crio-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2888 2023-05-31 07:50:27.788257 crio-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1315 2023-05-31 07:36:07.000000 crio-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 07:50:27.702688 crio-0.0.5/crio/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:50:27.723779 crio-0.0.5/crio/Loadini/
--rw-rw-rw-   0        0        0     4372 2022-03-19 15:07:32.000000 crio-0.0.5/crio/Loadini/Loadini.py
--rw-rw-rw-   0        0        0       28 2022-02-07 03:30:22.000000 crio-0.0.5/crio/Loadini/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:50:27.733792 crio-0.0.5/crio/UDP/
--rw-rw-rw-   0        0        0     8772 2023-02-16 04:32:48.000000 crio-0.0.5/crio/UDP/UDP.py
--rw-rw-rw-   0        0        0       20 2022-02-07 03:30:22.000000 crio-0.0.5/crio/UDP/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.5/crio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:50:27.743683 crio-0.0.5/crio/config/
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.5/crio/config/__init__.py
--rw-rw-rw-   0        0        0    18316 2023-05-31 07:48:36.000000 crio-0.0.5/crio/crio.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:50:27.781268 crio-0.0.5/crio/crio_hs/
--rw-rw-rw-   0        0        0       22 2022-02-07 03:30:22.000000 crio-0.0.5/crio/crio_hs/__init__.py
--rw-rw-rw-   0        0        0    15939 2022-02-07 03:30:22.000000 crio-0.0.5/crio/crio_hs/crio_hs.py
--rw-rw-rw-   0        0        0     1106 2023-02-10 02:00:30.000000 crio-0.0.5/crio/getBenchIni.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:50:27.788257 crio-0.0.5/crio/inis/
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.5/crio/inis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:50:27.718810 crio-0.0.5/crio.egg-info/
--rw-rw-rw-   0        0        0     2888 2023-05-31 07:50:27.000000 crio-0.0.5/crio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-31 07:50:27.000000 crio-0.0.5/crio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:50:27.000000 crio-0.0.5/crio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-31 07:50:27.000000 crio-0.0.5/crio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2023-05-31 07:50:00.000000 crio-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 07:50:27.788257 crio-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 03:20:10.212047 crio-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 00:14:59.000000 crio-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2888 2023-06-01 03:20:10.210046 crio-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1315 2023-05-31 07:36:07.000000 crio-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 03:20:10.178727 crio-0.0.6/crio/
+drwxrwxrwx   0        0        0        0 2023-06-01 03:20:10.197190 crio-0.0.6/crio/Loadini/
+-rw-rw-rw-   0        0        0     4372 2022-03-19 15:07:32.000000 crio-0.0.6/crio/Loadini/Loadini.py
+-rw-rw-rw-   0        0        0       28 2022-02-07 03:30:22.000000 crio-0.0.6/crio/Loadini/__init__.py
+-rw-rw-rw-   0        0        0     8772 2023-02-16 04:32:48.000000 crio-0.0.6/crio/UDP.py
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.6/crio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:20:10.200183 crio-0.0.6/crio/config/
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.6/crio/config/__init__.py
+-rw-rw-rw-   0        0        0    18282 2023-06-01 03:18:14.000000 crio-0.0.6/crio/crio.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:20:10.204191 crio-0.0.6/crio/crio_hs/
+-rw-rw-rw-   0        0        0       22 2022-02-07 03:30:22.000000 crio-0.0.6/crio/crio_hs/__init__.py
+-rw-rw-rw-   0        0        0    15939 2022-02-07 03:30:22.000000 crio-0.0.6/crio/crio_hs/crio_hs.py
+-rw-rw-rw-   0        0        0     1106 2023-02-10 02:00:30.000000 crio-0.0.6/crio/getBenchIni.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:20:10.206690 crio-0.0.6/crio/inis/
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.6/crio/inis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:20:10.190192 crio-0.0.6/crio.egg-info/
+-rw-rw-rw-   0        0        0     2888 2023-06-01 03:20:10.000000 crio-0.0.6/crio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-06-01 03:20:10.000000 crio-0.0.6/crio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 03:20:10.000000 crio-0.0.6/crio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-01 03:20:10.000000 crio-0.0.6/crio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2023-06-01 03:19:16.000000 crio-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 03:20:10.212047 crio-0.0.6/setup.cfg
```

### Comparing `crio-0.0.5/LICENSE` & `crio-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crio-0.0.5/PKG-INFO` & `crio-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crio
-Version: 0.0.5
+Version: 0.0.6
 Summary: library for CRIO operation
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `crio-0.0.5/README.md` & `crio-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `crio-0.0.5/crio/Loadini/Loadini.py` & `crio-0.0.6/crio/Loadini/Loadini.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.5/crio/UDP/UDP.py` & `crio-0.0.6/crio/UDP.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.5/crio/crio.py` & `crio-0.0.6/crio/crio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #import os
 import sys
 import time
 import logging
-# import robot.api.logger as log
 import json
 from importlib.resources import files
 import UDP
 
 '''
 try:
     from utility.getdata import config
```

### Comparing `crio-0.0.5/crio/crio_hs/crio_hs.py` & `crio-0.0.6/crio/crio_hs/crio_hs.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.5/crio/getBenchIni.py` & `crio-0.0.6/crio/getBenchIni.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.5/crio.egg-info/PKG-INFO` & `crio-0.0.6/crio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crio
-Version: 0.0.5
+Version: 0.0.6
 Summary: library for CRIO operation
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

