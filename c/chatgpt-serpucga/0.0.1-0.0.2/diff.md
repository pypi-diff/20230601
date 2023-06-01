# Comparing `tmp/chatgpt_serpucga-0.0.1.tar.gz` & `tmp/chatgpt_serpucga-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_serpucga-0.0.1.tar", last modified: Thu Jun  1 12:01:35 2023, max compression
+gzip compressed data, was "chatgpt_serpucga-0.0.2.tar", last modified: Thu Jun  1 12:24:08 2023, max compression
```

## Comparing `chatgpt_serpucga-0.0.1.tar` & `chatgpt_serpucga-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-01 12:01:35.635851 chatgpt_serpucga-0.0.1/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      615 2023-06-01 12:01:35.635851 chatgpt_serpucga-0.0.1/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt_serpucga-0.0.1/README.md
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-01 12:01:35.631851 chatgpt_serpucga-0.0.1/chatgpt/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5335 2023-06-01 11:54:49.000000 chatgpt_serpucga-0.0.1/chatgpt/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt_serpucga-0.0.1/chatgpt/consts.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-01 12:01:35.635851 chatgpt_serpucga-0.0.1/chatgpt_serpucga.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      615 2023-06-01 12:01:35.000000 chatgpt_serpucga-0.0.1/chatgpt_serpucga.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      216 2023-06-01 12:01:35.000000 chatgpt_serpucga-0.0.1/chatgpt_serpucga.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-06-01 12:01:35.000000 chatgpt_serpucga-0.0.1/chatgpt_serpucga.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        8 2023-06-01 12:01:35.000000 chatgpt_serpucga-0.0.1/chatgpt_serpucga.egg-info/top_level.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-06-01 12:01:35.635851 chatgpt_serpucga-0.0.1/setup.cfg
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      922 2023-06-01 12:00:58.000000 chatgpt_serpucga-0.0.1/setup.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-01 12:24:08.656106 chatgpt_serpucga-0.0.2/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      615 2023-06-01 12:24:08.656106 chatgpt_serpucga-0.0.2/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt_serpucga-0.0.2/README.md
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-01 12:24:08.652106 chatgpt_serpucga-0.0.2/chatgpt/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5335 2023-06-01 12:23:33.000000 chatgpt_serpucga-0.0.2/chatgpt/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt_serpucga-0.0.2/chatgpt/consts.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-01 12:24:08.652106 chatgpt_serpucga-0.0.2/chatgpt_serpucga.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      615 2023-06-01 12:24:08.000000 chatgpt_serpucga-0.0.2/chatgpt_serpucga.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      216 2023-06-01 12:24:08.000000 chatgpt_serpucga-0.0.2/chatgpt_serpucga.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-06-01 12:24:08.000000 chatgpt_serpucga-0.0.2/chatgpt_serpucga.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        8 2023-06-01 12:24:08.000000 chatgpt_serpucga-0.0.2/chatgpt_serpucga.egg-info/top_level.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-06-01 12:24:08.656106 chatgpt_serpucga-0.0.2/setup.cfg
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      922 2023-06-01 12:00:58.000000 chatgpt_serpucga-0.0.2/setup.py
```

### Comparing `chatgpt_serpucga-0.0.1/PKG-INFO` & `chatgpt_serpucga-0.0.2/chatgpt_serpucga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: chatgpt_serpucga
-Version: 0.0.1
+Name: chatgpt-serpucga
+Version: 0.0.2
 Summary: Client library to communicate with the ChatGPT API
 Home-page: https://gitlab.com/Serbaf/chatgpt_client
 Author: Sergio Puche García
 Author-email: spuche@upv.es
 License: GPL3
 Description-Content-Type: text/markdown
```

### Comparing `chatgpt_serpucga-0.0.1/chatgpt/__init__.py` & `chatgpt_serpucga-0.0.2/chatgpt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 import openai
 import tiktoken
 from logutils import get_logger
 from consts import MAX_TOKENS, SUPPORTED_ENGINES, ENGINES0, ENGINES1
 from rich.console import Console
```

### Comparing `chatgpt_serpucga-0.0.1/chatgpt/consts.py` & `chatgpt_serpucga-0.0.2/chatgpt/consts.py`

 * *Files identical despite different names*

### Comparing `chatgpt_serpucga-0.0.1/chatgpt_serpucga.egg-info/PKG-INFO` & `chatgpt_serpucga-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: chatgpt-serpucga
-Version: 0.0.1
+Name: chatgpt_serpucga
+Version: 0.0.2
 Summary: Client library to communicate with the ChatGPT API
 Home-page: https://gitlab.com/Serbaf/chatgpt_client
 Author: Sergio Puche García
 Author-email: spuche@upv.es
 License: GPL3
 Description-Content-Type: text/markdown
```

### Comparing `chatgpt_serpucga-0.0.1/setup.py` & `chatgpt_serpucga-0.0.2/setup.py`

 * *Files identical despite different names*

