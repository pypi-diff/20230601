# Comparing `tmp/CliRenderer-0.1.3.tar.gz` & `tmp/CliRenderer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CliRenderer-0.1.3.tar", last modified: Thu Jun  1 12:41:52 2023, max compression
+gzip compressed data, was "CliRenderer-0.1.4.tar", last modified: Thu Jun  1 13:01:35 2023, max compression
```

## Comparing `CliRenderer-0.1.3.tar` & `CliRenderer-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:41:52.079712 CliRenderer-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:41:52.075712 CliRenderer-0.1.3/CliRenderer/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/CliRenderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/CliRenderer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/CliRenderer/chartools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/CliRenderer/colorer.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/CliRenderer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:41:52.075712 CliRenderer-0.1.3/CliRenderer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-01 12:41:52.000000 CliRenderer-0.1.3/CliRenderer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 12:41:52.000000 CliRenderer-0.1.3/CliRenderer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:41:52.000000 CliRenderer-0.1.3/CliRenderer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 12:41:52.000000 CliRenderer-0.1.3/CliRenderer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 12:41:52.000000 CliRenderer-0.1.3/CliRenderer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 12:41:52.000000 CliRenderer-0.1.3/CliRenderer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-01 12:41:52.079712 CliRenderer-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-01 12:41:52.079712 CliRenderer-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:41:52.075712 CliRenderer-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/test/test-speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 12:41:39.000000 CliRenderer-0.1.3/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:01:35.348923 CliRenderer-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:01:35.344922 CliRenderer-0.1.4/CliRenderer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/chartools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/colorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:01:35.344922 CliRenderer-0.1.4/CliRenderer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-01 13:01:35.348923 CliRenderer-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-01 13:01:35.348923 CliRenderer-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:01:35.348923 CliRenderer-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/test/test-speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/test/test.py
```

### Comparing `CliRenderer-0.1.3/CliRenderer/__init__.py` & `CliRenderer-0.1.4/CliRenderer/__init__.py`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.3/CliRenderer/__main__.py` & `CliRenderer-0.1.4/CliRenderer/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import importlib.metadata
 from pathlib import Path
 
+import colorama
+import rich
 import typer as typer
 from PIL import Image
 from rich.console import Console
 import imageio as iio
 from io import StringIO
 from CliRenderer import render, Flags
 
@@ -47,12 +50,14 @@
         output.parent.mkdir(parents=True, exist_ok=True)
         with open(output, "wb") as f:
             f.write(string.encode("utf-8"))
 
     print(string)
     print(f"Saved output to {output}... Read it using `cat {output}`")
 def main():
+    rich.print(f"[bold white]CliRenderer installed version: {importlib.metadata.version('CliRenderer')}.[/bold white]")
+    rich.print("[grey37]Version shown may not be accurate! (especially you are running from source!)[/grey37]\n")
     typer.run(cli_main)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `CliRenderer-0.1.3/CliRenderer/chartools.py` & `CliRenderer-0.1.4/CliRenderer/chartools.py`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.3/CliRenderer/colorer.py` & `CliRenderer-0.1.4/CliRenderer/colorer.py`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.3/CliRenderer.egg-info/PKG-INFO` & `CliRenderer-0.1.4/CliRenderer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: CliRenderer
-Version: 0.1.3
+Version: 0.1.4
 Summary: A CLI tool to render unicode art in the terminal
 Home-page: https://github.com/ultraflame4/CliR
 Author: ultraflame4
 License: MIT
 Keywords: cli,unicode,art,render,terminal
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CliRenderer
 
 A text renderer that renders unicode art from images to the terminal
 
 ## Installation
-Check the releases page for the latest version and instructions on how to install it.
+**Install the latest version with**: `pip install CliRenderer`
 
 ## Usage
 See `clirender --help` for a list of options and arguments.
 
 ### Notice when reading output
 
 #### Linux
```

### Comparing `CliRenderer-0.1.3/LICENSE` & `CliRenderer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.3/PKG-INFO` & `CliRenderer-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: CliRenderer
-Version: 0.1.3
+Version: 0.1.4
 Summary: A CLI tool to render unicode art in the terminal
 Home-page: https://github.com/ultraflame4/CliR
 Author: ultraflame4
 License: MIT
 Keywords: cli,unicode,art,render,terminal
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CliRenderer
 
 A text renderer that renders unicode art from images to the terminal
 
 ## Installation
-Check the releases page for the latest version and instructions on how to install it.
+**Install the latest version with**: `pip install CliRenderer`
 
 ## Usage
 See `clirender --help` for a list of options and arguments.
 
 ### Notice when reading output
 
 #### Linux
```

### Comparing `CliRenderer-0.1.3/README.md` & `CliRenderer-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # CliRenderer
 
 A text renderer that renders unicode art from images to the terminal
 
 ## Installation
-Check the releases page for the latest version and instructions on how to install it.
+**Install the latest version with**: `pip install CliRenderer`
 
 ## Usage
 See `clirender --help` for a list of options and arguments.
 
 ### Notice when reading output
 
 #### Linux
```

### Comparing `CliRenderer-0.1.3/setup.cfg` & `CliRenderer-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CliRenderer
-version = 0.1.3
+version = 0.1.4
 author = ultraflame4
 description = A CLI tool to render unicode art in the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = cli, unicode, art, render, terminal
 license = MIT
 license_file = LICENSE
```

### Comparing `CliRenderer-0.1.3/test/test-speed.py` & `CliRenderer-0.1.4/test/test-speed.py`

 * *Files identical despite different names*

