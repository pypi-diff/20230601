# Comparing `tmp/sqdconvert-1.0.1.tar.gz` & `tmp/sqdconvert-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqdconvert-1.0.1.tar", last modified: Wed May 31 14:39:38 2023, max compression
+gzip compressed data, was "sqdconvert-1.0.2.tar", last modified: Wed May 31 22:36:56 2023, max compression
```

## Comparing `sqdconvert-1.0.1.tar` & `sqdconvert-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:39:38.519025 sqdconvert-1.0.1/
--rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:15.000000 sqdconvert-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       33 2022-10-15 13:34:47.000000 sqdconvert-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1740 2023-05-31 14:39:38.516829 sqdconvert-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-05-31 14:38:03.000000 sqdconvert-1.0.1/README.md
--rw-rw-rw-   0        0        0      586 2023-05-31 14:38:54.000000 sqdconvert-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 14:39:38.519823 sqdconvert-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       36 2022-10-14 07:04:07.000000 sqdconvert-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:39:38.340208 sqdconvert-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 14:39:38.438143 sqdconvert-1.0.1/src/sqdconvert/
--rw-rw-rw-   0        0        0      388 2023-05-31 14:38:51.000000 sqdconvert-1.0.1/src/sqdconvert/__init__.py
--rw-rw-rw-   0        0        0     1326 2023-05-31 14:38:38.000000 sqdconvert-1.0.1/src/sqdconvert/__main__.py
--rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqdconvert-1.0.1/src/sqdconvert/color.py
--rw-rw-rw-   0        0        0     2482 2023-05-31 11:05:18.000000 sqdconvert-1.0.1/src/sqdconvert/config.py
--rw-rw-rw-   0        0        0      808 2023-05-31 13:22:38.000000 sqdconvert-1.0.1/src/sqdconvert/errors.py
--rw-rw-rw-   0        0        0     2570 2023-05-31 13:50:23.000000 sqdconvert-1.0.1/src/sqdconvert/start.py
--rw-rw-rw-   0        0        0      219 2023-05-31 10:23:22.000000 sqdconvert-1.0.1/src/sqdconvert/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:39:38.511685 sqdconvert-1.0.1/src/sqdconvert.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 22:36:56.733560 sqdconvert-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:15.000000 sqdconvert-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-10-15 13:34:47.000000 sqdconvert-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1740 2023-05-31 22:36:56.730549 sqdconvert-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-05-31 14:38:03.000000 sqdconvert-1.0.2/README.md
+-rw-rw-rw-   0        0        0      586 2023-05-31 22:36:18.000000 sqdconvert-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 22:36:56.733560 sqdconvert-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       36 2022-10-14 07:04:07.000000 sqdconvert-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:36:56.548318 sqdconvert-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 22:36:56.659314 sqdconvert-1.0.2/src/sqdconvert/
+-rw-rw-rw-   0        0        0      388 2023-05-31 22:36:14.000000 sqdconvert-1.0.2/src/sqdconvert/__init__.py
+-rw-rw-rw-   0        0        0     1817 2023-05-31 22:34:26.000000 sqdconvert-1.0.2/src/sqdconvert/__main__.py
+-rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqdconvert-1.0.2/src/sqdconvert/color.py
+-rw-rw-rw-   0        0        0     2507 2023-05-31 22:29:05.000000 sqdconvert-1.0.2/src/sqdconvert/config.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 13:22:38.000000 sqdconvert-1.0.2/src/sqdconvert/errors.py
+-rw-rw-rw-   0        0        0     2576 2023-05-31 22:27:59.000000 sqdconvert-1.0.2/src/sqdconvert/start.py
+-rw-rw-rw-   0        0        0      291 2023-05-31 22:26:26.000000 sqdconvert-1.0.2/src/sqdconvert/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:36:56.725336 sqdconvert-1.0.2/src/sqdconvert.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/top_level.txt
```

### Comparing `sqdconvert-1.0.1/LICENSE` & `sqdconvert-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.1/PKG-INFO` & `sqdconvert-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqdconvert
-Version: 1.0.1
+Version: 1.0.2
 Summary: convert any audio or video files from one extension to another!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

### Comparing `sqdconvert-1.0.1/pyproject.toml` & `sqdconvert-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqdconvert"
-version = "1.0.1"
+version = "1.0.2"
 description = "convert any audio or video files from one extension to another!"
 authors = [
     { name="sqdnoises" }
 ]
 
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `sqdconvert-1.0.1/src/sqdconvert/color.py` & `sqdconvert-1.0.2/src/sqdconvert/color.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.1/src/sqdconvert/config.py` & `sqdconvert-1.0.2/src/sqdconvert/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import json
 from datetime import datetime
+
 from . import color, errors
+from .utils import fs
 
 default_config_path = os.path.normpath(os.path.expandvars(os.path.expanduser("~/.sqdconfig/sqdconvert/")))
 os.makedirs(default_config_path, exist_ok=True)
 
 class Config:
     def __init__(self, config) -> None:
         try:
@@ -20,30 +22,30 @@
                         ffmpeg_path = _p
                 
                     else:
                         raise errors.FFmpegNotFound(config["ffmpeg_path"])
             else:
                 raise errors.FFmpegNotFound(config["ffmpeg_path"])
         
-            _ffpath = ffmpeg_path.split("\\")
+            _ffpath = ffmpeg_path.split(fs)
             self.ffmpeg_path = []
             for x in _ffpath:
                 if " " in x:
                     x = '"'+x+'"'
                 self.ffmpeg_path.append(x)
             
-            self.ffmpeg_path = "\\".join(self.ffmpeg_path)
+            self.ffmpeg_path = fs.join(self.ffmpeg_path)
             
         except Exception as e:
             raise errors.ConfigLoadError(e)
 
 def make_default_config():
     t = datetime.now()
     return """{
-    "ffmpeg_path": ""
+    "ffmpeg_path": "ffmpeg"
 }
 """, f"""// Default Config -- Generated on {t.day}/{t.month}/{t.year}"""
 """{
     "ffmpeg_path": "path to ffmpeg"
 }
 """
```

### Comparing `sqdconvert-1.0.1/src/sqdconvert/errors.py` & `sqdconvert-1.0.2/src/sqdconvert/errors.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.1/src/sqdconvert/start.py` & `sqdconvert-1.0.2/src/sqdconvert/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import argparse
 
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
-from . import color, errors
+from . import color
+from .utils import fs
 from .config import Config
 
 __all__ = [
     "main"
 ]
 
 def main(args: argparse.ArgumentParser, config: Config) -> None:
@@ -36,19 +37,19 @@
 
         out = os.path.normpath(args.output)
         if os.path.exists(out):
             spinner.text = f"{color.red}File already exists: {color.bright_yellow}'{out}'{color.reset}"
             spinner.fail(f"💥")
             exit()
 
-        filename = out.split("\\")[-1]
-        if "\\" in out:
-            _out = out.split("\\")
+        filename = out.split(fs)[-1]
+        if fs in out:
+            _out = out.split(fs)
             _out.pop(-1)
-            out_path = "\\".join(_out)
+            out_path = fs.join(_out)
         else:
             out_path = "."
 
         os.makedirs(out_path, exist_ok=True)    
 
         status = os.system(f'{config.ffmpeg_path} -i "{inp}" "{out}" {"" if args.verbose else "-hide_banner -loglevel error"}')
```

### Comparing `sqdconvert-1.0.1/src/sqdconvert.egg-info/PKG-INFO` & `sqdconvert-1.0.2/src/sqdconvert.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqdconvert
-Version: 1.0.1
+Version: 1.0.2
 Summary: convert any audio or video files from one extension to another!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

