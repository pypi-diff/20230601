# Comparing `tmp/codinghou-0.0.5.tar.gz` & `tmp/codinghou-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codinghou-0.0.5.tar", last modified: Sun Jan  1 15:21:28 2023, max compression
+gzip compressed data, was "codinghou-0.6.1.tar", last modified: Thu Jun  1 05:33:05 2023, max compression
```

## Comparing `codinghou-0.0.5.tar` & `codinghou-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-01 15:21:28.491289 codinghou-0.0.5/
--rw-rw-rw-   0        0        0      438 2023-01-01 15:21:28.490288 codinghou-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-01-01 01:09:10.000000 codinghou-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-01 15:21:28.457289 codinghou-0.0.5/codinghou/
--rw-rw-rw-   0        0        0     2360 2023-01-01 15:20:49.000000 codinghou-0.0.5/codinghou/__init__.py
--rw-rw-rw-   0        0        0      407 2023-01-01 02:24:48.000000 codinghou-0.0.5/codinghou/main.py
-drwxrwxrwx   0        0        0        0 2023-01-01 15:21:28.487288 codinghou-0.0.5/codinghou.egg-info/
--rw-rw-rw-   0        0        0      438 2023-01-01 15:21:28.000000 codinghou-0.0.5/codinghou.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-01-01 15:21:28.000000 codinghou-0.0.5/codinghou.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-01 15:21:28.000000 codinghou-0.0.5/codinghou.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-01-01 15:21:28.000000 codinghou-0.0.5/codinghou.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-01 15:21:28.000000 codinghou-0.0.5/codinghou.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-01 15:21:28.492288 codinghou-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-01-01 15:20:56.000000 codinghou-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:33:05.639781 codinghou-0.6.1/
+-rw-rw-rw-   0        0        0      438 2023-06-01 05:33:05.638780 codinghou-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-01-01 01:09:10.000000 codinghou-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 05:33:05.618802 codinghou-0.6.1/codinghou/
+-rw-rw-rw-   0        0        0     2360 2023-06-01 05:29:53.000000 codinghou-0.6.1/codinghou/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-01-01 02:24:48.000000 codinghou-0.6.1/codinghou/main.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:33:05.637781 codinghou-0.6.1/codinghou.egg-info/
+-rw-rw-rw-   0        0        0      438 2023-06-01 05:33:05.000000 codinghou-0.6.1/codinghou.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-01 05:33:05.000000 codinghou-0.6.1/codinghou.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 05:33:05.000000 codinghou-0.6.1/codinghou.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-01 05:33:05.000000 codinghou-0.6.1/codinghou.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 05:33:05.000000 codinghou-0.6.1/codinghou.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 05:33:05.639781 codinghou-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-06-01 05:32:05.000000 codinghou-0.6.1/setup.py
```

### Comparing `codinghou-0.0.5/codinghou/__init__.py` & `codinghou-0.6.1/codinghou/__init__.py`

 * *Files identical despite different names*

### Comparing `codinghou-0.0.5/setup.py` & `codinghou-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="codinghou",
-    version="0.0.5",
+    version="0.6.1",
     author="douglee",
     description="CodingHou package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Douglee/codinghou",
     packages=setuptools.find_packages(),
     classifiers=[
```

