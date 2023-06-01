# Comparing `tmp/nekosama-3.tar.gz` & `tmp/nekosama-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nekosama-3.tar", last modified: Sun Apr 30 22:56:48 2023, max compression
+gzip compressed data, was "nekosama-3.1.tar", last modified: Thu Jun  1 17:00:34 2023, max compression
```

## Comparing `nekosama-3.tar` & `nekosama-3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:56:48.013016 nekosama-3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-30 22:56:36.000000 nekosama-3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-30 22:56:48.013016 nekosama-3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-30 22:56:36.000000 nekosama-3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-30 22:56:36.000000 nekosama-3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-30 22:56:48.013016 nekosama-3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-30 22:56:36.000000 nekosama-3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:56:48.009016 nekosama-3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:56:48.009016 nekosama-3/src/nekosama/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-30 22:56:36.000000 nekosama-3/src/nekosama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-30 22:56:36.000000 nekosama-3/src/nekosama/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18398 2023-04-30 22:56:36.000000 nekosama-3/src/nekosama/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-30 22:56:36.000000 nekosama-3/src/nekosama/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-30 22:56:36.000000 nekosama-3/src/nekosama/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:56:48.013016 nekosama-3/src/nekosama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-30 22:56:48.000000 nekosama-3/src/nekosama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-30 22:56:48.000000 nekosama-3/src/nekosama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:56:48.000000 nekosama-3/src/nekosama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 22:56:48.000000 nekosama-3/src/nekosama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 22:56:48.000000 nekosama-3/src/nekosama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:00:34.073588 nekosama-3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 17:00:20.000000 nekosama-3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-01 17:00:34.073588 nekosama-3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-01 17:00:20.000000 nekosama-3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 17:00:20.000000 nekosama-3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-01 17:00:34.073588 nekosama-3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 17:00:20.000000 nekosama-3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:00:34.069588 nekosama-3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:00:34.069588 nekosama-3.1/src/nekosama/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 17:00:20.000000 nekosama-3.1/src/nekosama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-01 17:00:20.000000 nekosama-3.1/src/nekosama/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-06-01 17:00:20.000000 nekosama-3.1/src/nekosama/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-01 17:00:20.000000 nekosama-3.1/src/nekosama/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-01 17:00:20.000000 nekosama-3.1/src/nekosama/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:00:34.069588 nekosama-3.1/src/nekosama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-01 17:00:34.000000 nekosama-3.1/src/nekosama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 17:00:34.000000 nekosama-3.1/src/nekosama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:00:34.000000 nekosama-3.1/src/nekosama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 17:00:34.000000 nekosama-3.1/src/nekosama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 17:00:34.000000 nekosama-3.1/src/nekosama.egg-info/top_level.txt
```

### Comparing `nekosama-3/LICENSE` & `nekosama-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nekosama-3/PKG-INFO` & `nekosama-3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nekosama
-Version: 3
+Version: 3.1
 Summary: A neko sama API
 Home-page: https://github.com/Egsagon/neko-sama-api/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
@@ -47,14 +47,14 @@
 ```
 
 An example can be found in the `main.py` file.
 
 # Setup
 
 - Use python `3.11` or higher
-- Install using pip: `pip install git+https://github.com/Egsagon/neko-sama-api.git`
+- Install using pip: `pip install nekosama`
 - Optionally, install FFMPEG to your system.
 
 # Docs
 
 A simple documentation is available [here](https://github.com/Egsagon/neko-sama-api/blob/master/doc.md).
 For more information, see docstrings and source code.
```

### Comparing `nekosama-3/README.md` & `nekosama-3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,14 @@
 ```
 
 An example can be found in the `main.py` file.
 
 # Setup
 
 - Use python `3.11` or higher
-- Install using pip: `pip install git+https://github.com/Egsagon/neko-sama-api.git`
+- Install using pip: `pip install nekosama`
 - Optionally, install FFMPEG to your system.
 
 # Docs
 
 A simple documentation is available [here](https://github.com/Egsagon/neko-sama-api/blob/master/doc.md).
 For more information, see docstrings and source code.
```

### Comparing `nekosama-3/setup.cfg` & `nekosama-3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nekosama
-version = 3
+version = 3.1
 description = A neko sama API
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/neko-sama-api/
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `nekosama-3/src/nekosama/consts.py` & `nekosama-3.1/src/nekosama/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ani_tags   = r'&quot;(.*?)&quot;'                                   # Get anime search tags
     an_from_ep = r'href=\"(/anime/info/.*)\" class=\"cover\"'           # Get ani url from ep page
     ep_bg      = r'\"head\" style=\"background-image: url\((https://.*)\)' # Get ep bg image url
     
     glob_name  = r'https://.*/anime/(info|episode)/(\d*)-([a-z-\d]*)_(vostfr|vf)' # Get url data
     ani_props  = r'<meta property=\"og:(?P<name>.*)\" content=\"([.\s\S]*?)\" />' # Get meta props
    
+    new_fuse_json = r'atob\(\"(.*?)\"\)' # New temporary json for the fusenet backend update
 
 class provider:
     '''
     Representations of providers.
     Possible values: BEST, FUSE, PSTREAM.
     '''
```

### Comparing `nekosama-3/src/nekosama/core.py` & `nekosama-3.1/src/nekosama/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,21 @@
         
         # Get the provider link to its script
         src = self.get(provider_url , headers = consts.headers).text
         res = re.findall(consts.re.script, src)[0][:-2]
         
         # Get the m3u file url
         src = self.get(res, headers = consts.headers).text
-        res = re.findall(consts.re.m3u8, src)[0]
+        
+        # if provider == consts.provider.FUSE:
+        if 'atob' in src: reg = consts.re.new_fuse_json
+        else: reg = consts.re.m3u8
+        
+        # Parse the encoded json
+        res = re.findall(reg, src)[0]
         raw = base64.b64decode(res).decode()
         m3u = re.findall(consts.re.m3u8_urls, raw)[0].replace('\\', '')[:-1]
         
         print('[FRAG] Fetched m3u file')
         
         # Get the m3u file data
         src = self.get(m3u, headers = consts.headers).text
```

### Comparing `nekosama-3/src/nekosama/download.py` & `nekosama-3.1/src/nekosama/download.py`

 * *Files identical despite different names*

### Comparing `nekosama-3/src/nekosama/utils.py` & `nekosama-3.1/src/nekosama/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import re
 import os
 import subprocess
 from nekosama import consts
 
 from typing import Callable
-from string import ascii_letters, digits
 
 
 def get_closest_value(iter: list[int], value: int):
     '''
     Pick the closest value in a list.
     From www.entechin.com/find-nearest-value-list-python/
     '''
```

### Comparing `nekosama-3/src/nekosama.egg-info/PKG-INFO` & `nekosama-3.1/src/nekosama.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nekosama
-Version: 3
+Version: 3.1
 Summary: A neko sama API
 Home-page: https://github.com/Egsagon/neko-sama-api/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
@@ -47,14 +47,14 @@
 ```
 
 An example can be found in the `main.py` file.
 
 # Setup
 
 - Use python `3.11` or higher
-- Install using pip: `pip install git+https://github.com/Egsagon/neko-sama-api.git`
+- Install using pip: `pip install nekosama`
 - Optionally, install FFMPEG to your system.
 
 # Docs
 
 A simple documentation is available [here](https://github.com/Egsagon/neko-sama-api/blob/master/doc.md).
 For more information, see docstrings and source code.
```

