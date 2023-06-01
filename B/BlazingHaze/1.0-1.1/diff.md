# Comparing `tmp/BlazingHaze-1.0.tar.gz` & `tmp/BlazingHaze-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlazingHaze-1.0.tar", last modified: Thu Jun  1 18:25:28 2023, max compression
+gzip compressed data, was "BlazingHaze-1.1.tar", last modified: Thu Jun  1 18:31:58 2023, max compression
```

## Comparing `BlazingHaze-1.0.tar` & `BlazingHaze-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:25:28.997674 BlazingHaze-1.0/
-drwxrwxrwx   0        0        0        0 2023-06-01 18:25:28.959219 BlazingHaze-1.0/BlazingHaze/
--rw-rw-rw-   0        0        0        0 2023-06-01 18:24:31.000000 BlazingHaze-1.0/BlazingHaze/__init__.py
--rw-rw-rw-   0        0        0    22317 2023-06-01 16:58:30.000000 BlazingHaze-1.0/BlazingHaze/slot.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:25:28.997674 BlazingHaze-1.0/BlazingHaze.egg-info/
--rw-rw-rw-   0        0        0      459 2023-06-01 18:25:28.000000 BlazingHaze-1.0/BlazingHaze.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-01 18:25:28.000000 BlazingHaze-1.0/BlazingHaze.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:25:28.000000 BlazingHaze-1.0/BlazingHaze.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-01 18:25:28.000000 BlazingHaze-1.0/BlazingHaze.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 18:25:28.000000 BlazingHaze-1.0/BlazingHaze.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-06-01 18:20:36.000000 BlazingHaze-1.0/LICENSE
--rw-rw-rw-   0        0        0      459 2023-06-01 18:25:28.997674 BlazingHaze-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-06-01 18:21:15.000000 BlazingHaze-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 18:25:28.997674 BlazingHaze-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 18:31:58.314968 BlazingHaze-1.1/
+drwxrwxrwx   0        0        0        0 2023-06-01 18:31:58.292220 BlazingHaze-1.1/BlazingHaze/
+-rw-rw-rw-   0        0        0        0 2023-06-01 18:24:31.000000 BlazingHaze-1.1/BlazingHaze/__init__.py
+-rw-rw-rw-   0        0        0    22317 2023-06-01 16:58:30.000000 BlazingHaze-1.1/BlazingHaze/slot.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:31:58.314968 BlazingHaze-1.1/BlazingHaze.egg-info/
+-rw-rw-rw-   0        0        0      459 2023-06-01 18:31:58.000000 BlazingHaze-1.1/BlazingHaze.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-01 18:31:58.000000 BlazingHaze-1.1/BlazingHaze.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:31:58.000000 BlazingHaze-1.1/BlazingHaze.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 18:31:58.000000 BlazingHaze-1.1/BlazingHaze.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 18:31:58.000000 BlazingHaze-1.1/BlazingHaze.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-06-01 18:20:36.000000 BlazingHaze-1.1/LICENSE
+-rw-rw-rw-   0        0        0      459 2023-06-01 18:31:58.314968 BlazingHaze-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-06-01 18:31:34.000000 BlazingHaze-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:31:58.314968 BlazingHaze-1.1/setup.cfg
```

### Comparing `BlazingHaze-1.0/BlazingHaze/slot.py` & `BlazingHaze-1.1/BlazingHaze/slot.py`

 * *Files identical despite different names*

### Comparing `BlazingHaze-1.0/LICENSE` & `BlazingHaze-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BlazingHaze-1.0/pyproject.toml` & `BlazingHaze-1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BlazingHaze"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Slot Casino Machine"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-    "tkinter >= 3.9.16",
-    "pillow >= 9.5.0",
+    "pillow >= 9.5.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

