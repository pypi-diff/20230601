# Comparing `tmp/crio-0.0.7.tar.gz` & `tmp/crio-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\work\crio_proj\dist\.tmp-9kodqn24\crio-0.0.7.tar", last modified: Thu Jun  1 03:35:39 2023, max compression
+gzip compressed data, was "C:\work\crio_proj\dist\.tmp-1f8ftz4y\crio-0.0.8.tar", last modified: Thu Jun  1 03:43:15 2023, max compression
```

## Comparing `crio-0.0.7.tar` & `crio-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 03:35:39.265495 crio-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-02-21 00:14:59.000000 crio-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       18 2023-06-01 03:34:53.000000 crio-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2888 2023-06-01 03:35:39.264345 crio-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1315 2023-05-31 07:36:07.000000 crio-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 03:35:39.141812 crio-0.0.7/crio/
-drwxrwxrwx   0        0        0        0 2023-06-01 03:35:39.195422 crio-0.0.7/crio/Loadini/
--rw-rw-rw-   0        0        0     4372 2022-03-19 15:07:32.000000 crio-0.0.7/crio/Loadini/Loadini.py
--rw-rw-rw-   0        0        0       28 2022-02-07 03:30:22.000000 crio-0.0.7/crio/Loadini/__init__.py
--rw-rw-rw-   0        0        0     8772 2023-02-16 04:32:48.000000 crio-0.0.7/crio/UDP.py
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.7/crio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:35:39.205741 crio-0.0.7/crio/config/
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.7/crio/config/__init__.py
--rw-rw-rw-   0        0        0    18307 2023-06-01 03:32:25.000000 crio-0.0.7/crio/crio.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:35:39.255895 crio-0.0.7/crio/crio_hs/
--rw-rw-rw-   0        0        0       22 2022-02-07 03:30:22.000000 crio-0.0.7/crio/crio_hs/__init__.py
--rw-rw-rw-   0        0        0    15939 2022-02-07 03:30:22.000000 crio-0.0.7/crio/crio_hs/crio_hs.py
--rw-rw-rw-   0        0        0     1106 2023-02-10 02:00:30.000000 crio-0.0.7/crio/getBenchIni.py
--rw-rw-rw-   0        0        0    12466 2023-02-16 01:32:30.000000 crio-0.0.7/crio/iniconfig.cfg
-drwxrwxrwx   0        0        0        0 2023-06-01 03:35:39.261049 crio-0.0.7/crio/inis/
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.7/crio/inis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:35:39.183426 crio-0.0.7/crio.egg-info/
--rw-rw-rw-   0        0        0     2888 2023-06-01 03:35:38.000000 crio-0.0.7/crio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-06-01 03:35:39.000000 crio-0.0.7/crio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:35:39.000000 crio-0.0.7/crio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-01 03:35:39.000000 crio-0.0.7/crio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2023-06-01 03:33:16.000000 crio-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 03:35:39.266508 crio-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 03:43:15.252078 crio-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 00:14:59.000000 crio-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-06-01 03:34:53.000000 crio-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2888 2023-06-01 03:43:15.243572 crio-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1315 2023-06-01 03:42:47.000000 crio-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 03:43:15.199537 crio-0.0.8/crio/
+drwxrwxrwx   0        0        0        0 2023-06-01 03:43:15.224432 crio-0.0.8/crio/Loadini/
+-rw-rw-rw-   0        0        0     4372 2022-03-19 15:07:32.000000 crio-0.0.8/crio/Loadini/Loadini.py
+-rw-rw-rw-   0        0        0       28 2022-02-07 03:30:22.000000 crio-0.0.8/crio/Loadini/__init__.py
+-rw-rw-rw-   0        0        0     8772 2023-02-16 04:32:48.000000 crio-0.0.8/crio/UDP.py
+-rw-rw-rw-   0        0        0       22 2023-06-01 03:42:21.000000 crio-0.0.8/crio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:43:15.229433 crio-0.0.8/crio/config/
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.8/crio/config/__init__.py
+-rw-rw-rw-   0        0        0    18307 2023-06-01 03:32:25.000000 crio-0.0.8/crio/crio.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:43:15.234430 crio-0.0.8/crio/crio_hs/
+-rw-rw-rw-   0        0        0       22 2022-02-07 03:30:22.000000 crio-0.0.8/crio/crio_hs/__init__.py
+-rw-rw-rw-   0        0        0    15939 2022-02-07 03:30:22.000000 crio-0.0.8/crio/crio_hs/crio_hs.py
+-rw-rw-rw-   0        0        0     1106 2023-02-10 02:00:30.000000 crio-0.0.8/crio/getBenchIni.py
+-rw-rw-rw-   0        0        0    12466 2023-02-16 01:32:30.000000 crio-0.0.8/crio/iniconfig.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 03:43:15.240569 crio-0.0.8/crio/inis/
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.8/crio/inis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:43:15.210346 crio-0.0.8/crio.egg-info/
+-rw-rw-rw-   0        0        0     2888 2023-06-01 03:43:15.000000 crio-0.0.8/crio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-06-01 03:43:15.000000 crio-0.0.8/crio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 03:43:15.000000 crio-0.0.8/crio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-01 03:43:15.000000 crio-0.0.8/crio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2023-06-01 03:42:26.000000 crio-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 03:43:15.253088 crio-0.0.8/setup.cfg
```

### Comparing `crio-0.0.7/LICENSE` & `crio-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crio-0.0.7/PKG-INFO` & `crio-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crio
-Version: 0.0.7
+Version: 0.0.8
 Summary: library for CRIO operation
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -31,15 +31,15 @@
 ## How to install 
 pip install crio
 
 ## How to use:
 
 from crio import crio
 
-a = crio()
+c = crio()
 
 ### Examples:
  
 c=crio()
 
 #Bench 初始化的步骤，例如初始化Bench，将DUT切换到Drawer1,并上电。
 c.configure_route("ClearMotorShorts",True)
```

### Comparing `crio-0.0.7/README.md` & `crio-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## How to install 
 pip install crio
 
 ## How to use:
 
 from crio import crio
 
-a = crio()
+c = crio()
 
 ### Examples:
  
 c=crio()
 
 #Bench 初始化的步骤，例如初始化Bench，将DUT切换到Drawer1,并上电。
 c.configure_route("ClearMotorShorts",True)
```

### Comparing `crio-0.0.7/crio/Loadini/Loadini.py` & `crio-0.0.8/crio/Loadini/Loadini.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.7/crio/UDP.py` & `crio-0.0.8/crio/UDP.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.7/crio/crio.py` & `crio-0.0.8/crio/crio.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.7/crio/crio_hs/crio_hs.py` & `crio-0.0.8/crio/crio_hs/crio_hs.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.7/crio/getBenchIni.py` & `crio-0.0.8/crio/getBenchIni.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.7/crio/iniconfig.cfg` & `crio-0.0.8/crio/iniconfig.cfg`

 * *Files identical despite different names*

### Comparing `crio-0.0.7/crio.egg-info/PKG-INFO` & `crio-0.0.8/crio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crio
-Version: 0.0.7
+Version: 0.0.8
 Summary: library for CRIO operation
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -31,15 +31,15 @@
 ## How to install 
 pip install crio
 
 ## How to use:
 
 from crio import crio
 
-a = crio()
+c = crio()
 
 ### Examples:
  
 c=crio()
 
 #Bench 初始化的步骤，例如初始化Bench，将DUT切换到Drawer1,并上电。
 c.configure_route("ClearMotorShorts",True)
```

