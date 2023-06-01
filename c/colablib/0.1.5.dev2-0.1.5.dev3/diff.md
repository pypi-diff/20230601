# Comparing `tmp/colablib-0.1.5.dev2.tar.gz` & `tmp/colablib-0.1.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.5.dev2.tar", last modified: Thu Jun  1 11:45:31 2023, max compression
+gzip compressed data, was "colablib-0.1.5.dev3.tar", last modified: Thu Jun  1 13:52:00 2023, max compression
```

## Comparing `colablib-0.1.5.dev2.tar` & `colablib-0.1.5.dev3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 11:45:31.698766 colablib-0.1.5.dev2/
--rw-rw-rw-   0        0        0      218 2023-06-01 11:45:31.697768 colablib-0.1.5.dev2/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 11:45:31.672308 colablib-0.1.5.dev2/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev2/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev2/colablib/cprint.py
--rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev2/colablib/deb_utils.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev2/colablib/git_utils.py
--rw-rw-rw-   0        0        0     2594 2023-06-01 10:44:06.000000 colablib-0.1.5.dev2/colablib/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:45:31.695769 colablib-0.1.5.dev2/colablib.egg-info/
--rw-rw-rw-   0        0        0      218 2023-06-01 11:45:31.000000 colablib-0.1.5.dev2/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-01 11:45:31.000000 colablib-0.1.5.dev2/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 11:45:31.000000 colablib-0.1.5.dev2/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 11:45:31.000000 colablib-0.1.5.dev2/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 11:45:31.699761 colablib-0.1.5.dev2/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-06-01 11:44:36.000000 colablib-0.1.5.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:52:00.142321 colablib-0.1.5.dev3/
+-rw-rw-rw-   0        0        0      218 2023-06-01 13:52:00.141308 colablib-0.1.5.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 13:52:00.129443 colablib-0.1.5.dev3/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev3/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev3/colablib/cprint.py
+-rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev3/colablib/deb_utils.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev3/colablib/git_utils.py
+-rw-rw-rw-   0        0        0     3330 2023-06-01 12:22:37.000000 colablib-0.1.5.dev3/colablib/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:52:00.140306 colablib-0.1.5.dev3/colablib.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-06-01 13:51:59.000000 colablib-0.1.5.dev3/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-01 13:52:00.000000 colablib-0.1.5.dev3/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 13:51:59.000000 colablib-0.1.5.dev3/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 13:51:59.000000 colablib-0.1.5.dev3/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 13:52:00.142321 colablib-0.1.5.dev3/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-06-01 13:50:59.000000 colablib-0.1.5.dev3/setup.py
```

### Comparing `colablib-0.1.5.dev2/colablib/cprint.py` & `colablib-0.1.5.dev3/colablib/cprint.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev2/colablib/deb_utils.py` & `colablib-0.1.5.dev3/colablib/deb_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev2/colablib/git_utils.py` & `colablib-0.1.5.dev3/colablib/git_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev2/colablib/py_utils.py` & `colablib-0.1.5.dev3/colablib/py_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 import requests
 import subprocess
 import sys
+import time 
 from urllib.parse import urlparse, unquote
 from .cprint import cprint
 
 def is_google_colab():
     """
     Checks if the current environment is Google Colab.
 
@@ -15,14 +16,40 @@
     """
     try:
         import google.colab
         return True
     except ImportError:
         return False
 
+def calculate_elapsed_time(start_time):
+    """
+    Calculate the elapsed time between a given start time and the current time.
+
+    Args:
+        start_time (float): The start time in seconds since the epoch.
+
+    Returns:
+        str: A formatted string representing the elapsed time.
+
+    Example:
+        >>> calculate_elapsed_time(time.time() - 30)
+        '30 sec'
+        >>> calculate_elapsed_time(time.time() - 120)
+        '2 mins 0 sec'
+    """
+    end_time = time.time()
+    elapsed_time = int(end_time - start_time)
+
+    if elapsed_time < 60:
+        return f"{elapsed_time} sec"
+    else:
+        mins, secs = divmod(elapsed_time, 60)
+        return f"{mins} mins {secs} sec"
+
+    
 def get_filename(url):
     """
     Extracts the filename from the given URL.
 
     Args:
         url (str): The URL to extract the filename from.
```

