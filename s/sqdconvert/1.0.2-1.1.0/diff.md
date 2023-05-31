# Comparing `tmp/sqdconvert-1.0.2.tar.gz` & `tmp/sqdconvert-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqdconvert-1.0.2.tar", last modified: Wed May 31 22:36:56 2023, max compression
+gzip compressed data, was "sqdconvert-1.1.0.tar", last modified: Wed May 31 23:25:12 2023, max compression
```

## Comparing `sqdconvert-1.0.2.tar` & `sqdconvert-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:36:56.733560 sqdconvert-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:15.000000 sqdconvert-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       33 2022-10-15 13:34:47.000000 sqdconvert-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1740 2023-05-31 22:36:56.730549 sqdconvert-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-05-31 14:38:03.000000 sqdconvert-1.0.2/README.md
--rw-rw-rw-   0        0        0      586 2023-05-31 22:36:18.000000 sqdconvert-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 22:36:56.733560 sqdconvert-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0       36 2022-10-14 07:04:07.000000 sqdconvert-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:36:56.548318 sqdconvert-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 22:36:56.659314 sqdconvert-1.0.2/src/sqdconvert/
--rw-rw-rw-   0        0        0      388 2023-05-31 22:36:14.000000 sqdconvert-1.0.2/src/sqdconvert/__init__.py
--rw-rw-rw-   0        0        0     1817 2023-05-31 22:34:26.000000 sqdconvert-1.0.2/src/sqdconvert/__main__.py
--rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqdconvert-1.0.2/src/sqdconvert/color.py
--rw-rw-rw-   0        0        0     2507 2023-05-31 22:29:05.000000 sqdconvert-1.0.2/src/sqdconvert/config.py
--rw-rw-rw-   0        0        0      808 2023-05-31 13:22:38.000000 sqdconvert-1.0.2/src/sqdconvert/errors.py
--rw-rw-rw-   0        0        0     2576 2023-05-31 22:27:59.000000 sqdconvert-1.0.2/src/sqdconvert/start.py
--rw-rw-rw-   0        0        0      291 2023-05-31 22:26:26.000000 sqdconvert-1.0.2/src/sqdconvert/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:36:56.725336 sqdconvert-1.0.2/src/sqdconvert.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 22:36:56.000000 sqdconvert-1.0.2/src/sqdconvert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 23:25:12.499644 sqdconvert-1.1.0/
+-rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:15.000000 sqdconvert-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-10-15 13:34:47.000000 sqdconvert-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1740 2023-05-31 23:25:12.496041 sqdconvert-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-05-31 14:38:03.000000 sqdconvert-1.1.0/README.md
+-rw-rw-rw-   0        0        0      601 2023-05-31 22:44:16.000000 sqdconvert-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 23:25:12.500756 sqdconvert-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       36 2022-10-14 07:04:07.000000 sqdconvert-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:25:12.408013 sqdconvert-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 23:25:12.453517 sqdconvert-1.1.0/src/sqdconvert/
+-rw-rw-rw-   0        0        0      388 2023-05-31 22:48:13.000000 sqdconvert-1.1.0/src/sqdconvert/__init__.py
+-rw-rw-rw-   0        0        0     2610 2023-05-31 23:22:13.000000 sqdconvert-1.1.0/src/sqdconvert/__main__.py
+-rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqdconvert-1.1.0/src/sqdconvert/color.py
+-rw-rw-rw-   0        0        0     2739 2023-05-31 23:23:10.000000 sqdconvert-1.1.0/src/sqdconvert/config.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 13:22:38.000000 sqdconvert-1.1.0/src/sqdconvert/errors.py
+-rw-rw-rw-   0        0        0     2995 2023-05-31 23:08:08.000000 sqdconvert-1.1.0/src/sqdconvert/start.py
+-rw-rw-rw-   0        0        0      291 2023-05-31 22:26:26.000000 sqdconvert-1.1.0/src/sqdconvert/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:25:12.494371 sqdconvert-1.1.0/src/sqdconvert.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-05-31 23:25:12.000000 sqdconvert-1.1.0/src/sqdconvert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-31 23:25:12.000000 sqdconvert-1.1.0/src/sqdconvert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 23:25:12.000000 sqdconvert-1.1.0/src/sqdconvert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-31 23:25:12.000000 sqdconvert-1.1.0/src/sqdconvert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 23:25:12.000000 sqdconvert-1.1.0/src/sqdconvert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 23:25:12.000000 sqdconvert-1.1.0/src/sqdconvert.egg-info/top_level.txt
```

### Comparing `sqdconvert-1.0.2/LICENSE` & `sqdconvert-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.2/PKG-INFO` & `sqdconvert-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqdconvert
-Version: 1.0.2
+Version: 1.1.0
 Summary: convert any audio or video files from one extension to another!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

### Comparing `sqdconvert-1.0.2/pyproject.toml` & `sqdconvert-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqdconvert"
-version = "1.0.2"
+version = "1.1.0"
 description = "convert any audio or video files from one extension to another!"
 authors = [
     { name="sqdnoises" }
 ]
 
 readme = "README.md"
 license = { file = "LICENSE" }
@@ -17,12 +17,13 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
-    "yaspin"
+    "yaspin",
+    "luddite"
 ]
 
 [project.scripts]
 sqdconvert = "sqdconvert.__main__:main"
```

### Comparing `sqdconvert-1.0.2/src/sqdconvert/__main__.py` & `sqdconvert-1.1.0/src/sqdconvert/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import luddite
 import argparse
 import traceback
+
 from . import (
     __name__ as name,
     __description__ as description,
     __copyright__ as copyright,
     __version__ as version
 )
 from . import color, utils 
@@ -22,29 +24,52 @@
     parser.add_argument("-out", "--output",
                         help="output file")
     parser.add_argument("-i", "--interactive",
                         action="store_true", help="start an interactive conversion")
     parser.add_argument("-v", "--verbose",
                         action="store_true", help="print more output")
     parser.add_argument("-c", "--config",
-                        required=False, default="use a different config file")
+                        help="use a different config file")
     parser.add_argument("-V", "--version",
                         action="version", version=name+" "+version)
     parser.add_argument("-l", "--license",
                         action="version", version=copyright+" - MIT License. For more information see: https://opensource.org/license/mit/",
                         help="show program's license and exit")
 
-    config = get_config()
+    try:
+        try:
+            config = get_config()
+        except Exception as e:
+            args = parser.parse_args()
+            raise e
 
-    args = parser.parse_args()
-    if args.config is not None:
-        config = get_config(args.config)
+        args = parser.parse_args()
+        if args.config is not None:
+            config = get_config(args.config)
     
-    try:
         start(args, config)
+    
     except Exception as e:
         if args.verbose:
             traceback.print_exc()
         print(f"{color.bright_red}💥 An error occured! {color.bright_yellow}{utils.get_full_class_name(e)}{color.bright_red}: {str(e)}{color.reset}")
+    
+    try:
+        new_version = luddite.get_version_pypi(name)
+    except:
+        new_version = None
+    
+    try:
+        config
+    except:
+        try_config = False
+    else:
+        try_config = True
+    
+    if new_version and try_config and config.update_notification:
+        print()
+        print(f"{color.bright_green}New version for {color.bright_yellow}{name}{color.bright_green} is available.{color.reset}")
+        print(f"{color.bright_blue}{version} {color.bright_green}>> {color.bright_blue}{new_version}{color.reset}")
+        print(f"{color.bright_white}Use {color.bright_red}pip install -U {name}{color.bright_white} to update!{color.reset}")
 
 if __name__ == "__main__":
     main()
```

### Comparing `sqdconvert-1.0.2/src/sqdconvert/color.py` & `sqdconvert-1.1.0/src/sqdconvert/color.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.2/src/sqdconvert/errors.py` & `sqdconvert-1.1.0/src/sqdconvert/errors.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.2/src/sqdconvert/start.py` & `sqdconvert-1.1.0/src/sqdconvert/start.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import argparse
 
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
+from . import __name__ as name
 from . import color
 from .utils import fs
 from .config import Config
 
 __all__ = [
     "main"
 ]
@@ -19,16 +20,20 @@
 
         if args.input.startswith('"') and args.input.endswith('"'):
             args.input = args.input.lstrip('"').rstrip('"')
         
         if args.output.startswith('"') and args.output.endswith('"'):
             args.output = args.output.lstrip('"').rstrip('"')
     
-    inp = os.path.normpath(args.input)
+    if args.input is None or args.output is None:
+        print(f"{color.bright_red}💥 Provide atleast one argument! {color.bright_green}Maybe you want to try using '{color.bright_yellow}{name} -i{color.bright_green}'?{color.reset}")
+        return print(f"{color.bright_green}❓ Use '{color.bright_yellow}{name} -h{color.bright_green}' for a list of commands.{color.reset}")
+    
     with yaspin(Spinners.dots12, text=f"{color.bright_white}Converting your file...{color.reset}", color="blue") as spinner:
+        inp = os.path.normpath(args.input)
         if os.path.exists(inp):
             if not os.path.isfile(inp):
                 spinner.text = f"{color.red}Input at the specified location is not a file: {color.bright_yellow}'{inp}'{color.reset}"
                 spinner.fail(f"💥")
                 exit()
         else:
             spinner.text = f"{color.red}File not found: {color.bright_yellow}'{inp}'{color.reset}"
```

### Comparing `sqdconvert-1.0.2/src/sqdconvert.egg-info/PKG-INFO` & `sqdconvert-1.1.0/src/sqdconvert.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqdconvert
-Version: 1.0.2
+Version: 1.1.0
 Summary: convert any audio or video files from one extension to another!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

