# Comparing `tmp/CliRenderer-0.1.4.tar.gz` & `tmp/CliRenderer-0.1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CliRenderer-0.1.4.tar", last modified: Thu Jun  1 13:01:35 2023, max compression
+gzip compressed data, was "CliRenderer-0.1.4.post1.tar", last modified: Thu Jun  1 13:09:38 2023, max compression
```

## Comparing `CliRenderer-0.1.4.tar` & `CliRenderer-0.1.4.post1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:01:35.348923 CliRenderer-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:01:35.344922 CliRenderer-0.1.4/CliRenderer/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/chartools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/colorer.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/CliRenderer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:01:35.344922 CliRenderer-0.1.4/CliRenderer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 13:01:35.000000 CliRenderer-0.1.4/CliRenderer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-01 13:01:35.348923 CliRenderer-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-01 13:01:35.348923 CliRenderer-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:01:35.348923 CliRenderer-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/test/test-speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 13:01:17.000000 CliRenderer-0.1.4/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:09:38.463481 CliRenderer-0.1.4.post1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:09:38.459480 CliRenderer-0.1.4.post1/CliRenderer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/CliRenderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/CliRenderer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/CliRenderer/chartools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/CliRenderer/colorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/CliRenderer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:09:38.463481 CliRenderer-0.1.4.post1/CliRenderer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-01 13:09:38.000000 CliRenderer-0.1.4.post1/CliRenderer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 13:09:38.000000 CliRenderer-0.1.4.post1/CliRenderer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:09:38.000000 CliRenderer-0.1.4.post1/CliRenderer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 13:09:38.000000 CliRenderer-0.1.4.post1/CliRenderer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 13:09:38.000000 CliRenderer-0.1.4.post1/CliRenderer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 13:09:38.000000 CliRenderer-0.1.4.post1/CliRenderer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-01 13:09:38.463481 CliRenderer-0.1.4.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-01 13:09:38.463481 CliRenderer-0.1.4.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:09:38.463481 CliRenderer-0.1.4.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/test/test-speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 13:09:27.000000 CliRenderer-0.1.4.post1/test/test.py
```

### Comparing `CliRenderer-0.1.4/CliRenderer/__init__.py` & `CliRenderer-0.1.4.post1/CliRenderer/__init__.py`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.4/CliRenderer/__main__.py` & `CliRenderer-0.1.4.post1/CliRenderer/__main__.py`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.4/CliRenderer/chartools.py` & `CliRenderer-0.1.4.post1/CliRenderer/chartools.py`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.4/CliRenderer/colorer.py` & `CliRenderer-0.1.4.post1/CliRenderer/colorer.py`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.4/CliRenderer.egg-info/PKG-INFO` & `CliRenderer-0.1.4.post1/CliRenderer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CliRenderer
-Version: 0.1.4
+Version: 0.1.4.post1
 Summary: A CLI tool to render unicode art in the terminal
 Home-page: https://github.com/ultraflame4/CliR
 Author: ultraflame4
 License: MIT
 Keywords: cli,unicode,art,render,terminal
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CliRenderer-0.1.4/LICENSE` & `CliRenderer-0.1.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.4/PKG-INFO` & `CliRenderer-0.1.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CliRenderer
-Version: 0.1.4
+Version: 0.1.4.post1
 Summary: A CLI tool to render unicode art in the terminal
 Home-page: https://github.com/ultraflame4/CliR
 Author: ultraflame4
 License: MIT
 Keywords: cli,unicode,art,render,terminal
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CliRenderer-0.1.4/README.md` & `CliRenderer-0.1.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `CliRenderer-0.1.4/setup.cfg` & `CliRenderer-0.1.4.post1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CliRenderer
-version = 0.1.4
+version = 0.1.4.post1
 author = ultraflame4
 description = A CLI tool to render unicode art in the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = cli, unicode, art, render, terminal
 license = MIT
 license_file = LICENSE
@@ -15,14 +15,15 @@
 install_requires = 
 	numpy~=1.24.2
 	Pillow~=9.5.0
 	rich~=13.3.4
 	CliRenderer~=0.1.0
 	typer~=0.7.0
 	imageio~=2.27.0
+	numba~=0.57.0
 
 [options.entry_points]
 console_scripts = 
 	clirender = CliRenderer.__main__:main
 
 [egg_info]
 tag_build =
```

### Comparing `CliRenderer-0.1.4/test/test-speed.py` & `CliRenderer-0.1.4.post1/test/test-speed.py`

 * *Files identical despite different names*

