# Comparing `tmp/longPolling-0.0.3.tar.gz` & `tmp/longPolling-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longPolling-0.0.3.tar", last modified: Thu May 18 15:36:35 2023, max compression
+gzip compressed data, was "longPolling-0.0.4.tar", last modified: Thu Jun  1 15:55:24 2023, max compression
```

## Comparing `longPolling-0.0.3.tar` & `longPolling-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 15:36:35.663687 longPolling-0.0.3/
--rw-rw-rw-   0        0        0     1854 2023-05-18 15:36:35.662687 longPolling-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-05-18 14:34:19.000000 longPolling-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 15:36:35.636687 longPolling-0.0.3/longPolling/
--rw-rw-rw-   0        0        0       67 2023-04-26 15:30:57.000000 longPolling-0.0.3/longPolling/__init__.py
--rw-rw-rw-   0        0        0     5478 2023-05-18 15:30:27.000000 longPolling-0.0.3/longPolling/client.py
--rw-rw-rw-   0        0        0     6998 2023-05-18 15:30:47.000000 longPolling-0.0.3/longPolling/server.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:36:35.662687 longPolling-0.0.3/longPolling.egg-info/
--rw-rw-rw-   0        0        0     1854 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 15:36:35.663687 longPolling-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-05-18 15:36:19.000000 longPolling-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:55:24.244370 longPolling-0.0.4/
+-rw-rw-rw-   0        0        0     1920 2023-06-01 15:55:24.243369 longPolling-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1213 2023-06-01 15:50:36.000000 longPolling-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-01 15:55:24.112368 longPolling-0.0.4/longPolling/
+-rw-rw-rw-   0        0        0      579 2023-05-31 14:01:47.000000 longPolling-0.0.4/longPolling/__init__.py
+-rw-rw-rw-   0        0        0     5990 2023-05-31 14:01:31.000000 longPolling-0.0.4/longPolling/client.py
+-rw-rw-rw-   0        0        0     8101 2023-06-01 15:49:06.000000 longPolling-0.0.4/longPolling/server.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:55:24.212370 longPolling-0.0.4/longPolling.egg-info/
+-rw-rw-rw-   0        0        0     1920 2023-06-01 15:55:23.000000 longPolling-0.0.4/longPolling.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-01 15:55:24.000000 longPolling-0.0.4/longPolling.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 15:55:23.000000 longPolling-0.0.4/longPolling.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-01 15:55:23.000000 longPolling-0.0.4/longPolling.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 15:55:23.000000 longPolling-0.0.4/longPolling.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 15:55:24.244370 longPolling-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2023-06-01 15:49:28.000000 longPolling-0.0.4/setup.py
```

### Comparing `longPolling-0.0.3/longPolling/client.py` & `longPolling-0.0.4/longPolling/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+Copyright (c) 2023 Gou Haoming
+longPolling is licensed under Mulan PSL v2.
+You can use this software according to the terms and conditions of the Mulan PSL v2. 
+You may obtain a copy of Mulan PSL v2 at:
+        http://license.coscl.org.cn/MulanPSL2 
+THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.  
+See the Mulan PSL v2 for more details.  
+"""
 import requests
 import threading
 import time
 from typing import Callable,Any,Union,Literal
 import logging
 import rsa
 class Client():
```

### Comparing `longPolling-0.0.3/setup.py` & `longPolling-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 setup(
     name = 'longPolling',
-    version = '0.0.3',
+    version = '0.0.4',
     keywords = ['long polling',"flask","http","thread"],
     description = 'Simple long polling implementation',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/long-polling/",
     install_requires = [
```

