# Comparing `tmp/colablib-0.1.3.tar.gz` & `tmp/colablib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.3.tar", last modified: Thu Jun  1 10:16:53 2023, max compression
+gzip compressed data, was "colablib-0.1.4.tar", last modified: Thu Jun  1 10:50:16 2023, max compression
```

## Comparing `colablib-0.1.3.tar` & `colablib-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 10:16:53.843595 colablib-0.1.3/
--rw-rw-rw-   0        0        0      213 2023-06-01 10:16:53.842596 colablib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 10:16:53.834077 colablib-0.1.3/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.3/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.3/colablib/cprint.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.3/colablib/git_utils.py
--rw-rw-rw-   0        0        0     1580 2023-06-01 10:15:05.000000 colablib-0.1.3/colablib/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:16:53.841597 colablib-0.1.3/colablib.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-01 10:16:53.000000 colablib-0.1.3/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-01 10:16:53.000000 colablib-0.1.3/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 10:16:53.000000 colablib-0.1.3/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 10:16:53.000000 colablib-0.1.3/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 10:16:53.843595 colablib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-06-01 10:15:43.000000 colablib-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:50:16.339156 colablib-0.1.4/
+-rw-rw-rw-   0        0        0      213 2023-06-01 10:50:16.338155 colablib-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 10:50:16.316938 colablib-0.1.4/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.4/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.4/colablib/cprint.py
+-rw-rw-rw-   0        0        0     1337 2023-06-01 10:48:41.000000 colablib-0.1.4/colablib/deb_utils.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.4/colablib/git_utils.py
+-rw-rw-rw-   0        0        0     2594 2023-06-01 10:44:06.000000 colablib-0.1.4/colablib/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:50:16.337253 colablib-0.1.4/colablib.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-01 10:50:16.000000 colablib-0.1.4/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-01 10:50:16.000000 colablib-0.1.4/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 10:50:16.000000 colablib-0.1.4/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 10:50:16.000000 colablib-0.1.4/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 10:50:16.339156 colablib-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-06-01 10:49:13.000000 colablib-0.1.4/setup.py
```

### Comparing `colablib-0.1.3/colablib/cprint.py` & `colablib-0.1.4/colablib/cprint.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.3/colablib/git_utils.py` & `colablib-0.1.4/colablib/git_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.3/colablib/py_utils.py` & `colablib-0.1.4/colablib/py_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,83 @@
+import os
+import re
+import requests
 import subprocess
 import sys
+from urllib.parse import urlparse, unquote
 from .cprint import cprint
 
 def is_google_colab():
+    """
+    Checks if the current environment is Google Colab.
+
+    Returns:
+        bool: True if it's Google Colab, False otherwise.
+    """
     try:
         import google.colab
         return True
-    except:
+    except ImportError:
         return False
 
+def get_filename(url):
+    """
+    Extracts the filename from the given URL.
+
+    Args:
+        url (str): The URL to extract the filename from.
+
+    Returns:
+        str: The filename.
+    """
+    response = requests.get(url, stream=True)
+    response.raise_for_status()
+
+    if 'content-disposition' in response.headers:
+        content_disposition = response.headers['content-disposition']
+        filename = re.findall('filename="?([^"]+)"?', content_disposition)[0]
+    else:
+        url_path = urlparse(url).path
+        filename = unquote(os.path.basename(url_path))
+
+    return filename
+
 def get_python_version():
-    try:
-        return sys.version
-    except Exception as e:
-        cprint("Failed to retrieve Python version:", str(e), color="greem")
-        return None
+    """
+    Retrieves the current Python version.
+
+    Returns:
+        str: The Python version.
+    """
+    return sys.version
 
 def get_torch_version():
+    """
+    Retrieves the current PyTorch version.
+
+    Returns:
+        str: The PyTorch version.
+    """
     try: 
         import torch
-    except ImportError:
-        raise ImportError("No torch module found. Please make sure PyTorch is installed.")
-        
-    try:
         return torch.__version__
-    except Exception as e:
-        cprint("Failed to retrieve PyTorch version:", str(e), color="greem")
+    except ImportError:
+        cprint("Failed to retrieve PyTorch version: PyTorch is not installed.", color="red")
         return None
-    
+
 def get_gpu_info(get_gpu_name=False):
+    """
+    Retrieves the GPU info.
+
+    Args:
+        get_gpu_name (bool, optional): Whether to retrieve the GPU name. Default is False.
+
+    Returns:
+        str: The GPU info.
+    """
     command = ["nvidia-smi", "--query-gpu=gpu_name", "--format=csv"]
     result = subprocess.run(command, capture_output=True, text=True)
 
     if result.returncode == 0:
         gpu_info = result.stdout.strip()
         if get_gpu_name:
             if 'name' in gpu_info:
```

