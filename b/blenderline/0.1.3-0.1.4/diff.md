# Comparing `tmp/blenderline-0.1.3.tar.gz` & `tmp/blenderline-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blenderline-0.1.3.tar", last modified: Thu Jun  1 10:54:44 2023, max compression
+gzip compressed data, was "blenderline-0.1.4.tar", last modified: Thu Jun  1 10:57:28 2023, max compression
```

## Comparing `blenderline-0.1.3.tar` & `blenderline-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.490784 blenderline-0.1.3/
--rw-rw-rw-   0        0        0    35823 2023-04-12 21:03:35.000000 blenderline-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     5839 2023-06-01 10:54:44.487013 blenderline-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5286 2023-06-01 10:54:23.000000 blenderline-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.421999 blenderline-0.1.3/blenderline/
--rw-rw-rw-   0        0        0        0 2023-04-12 21:15:58.000000 blenderline-0.1.3/blenderline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.433218 blenderline-0.1.3/blenderline/collections/
--rw-rw-rw-   0        0        0      112 2023-05-03 21:08:38.000000 blenderline-0.1.3/blenderline/collections/__init__.py
--rw-rw-rw-   0        0        0      251 2023-05-24 20:47:31.000000 blenderline-0.1.3/blenderline/collections/background.py
--rw-rw-rw-   0        0        0     1322 2023-05-24 20:47:29.000000 blenderline-0.1.3/blenderline/collections/base.py
--rw-rw-rw-   0        0        0      227 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/collections/hdr.py
--rw-rw-rw-   0        0        0      221 2023-05-03 21:08:38.000000 blenderline-0.1.3/blenderline/collections/item.py
--rw-rw-rw-   0        0        0     4294 2023-05-25 16:12:54.000000 blenderline-0.1.3/blenderline/command_line.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.453148 blenderline-0.1.3/blenderline/entries/
--rw-rw-rw-   0        0        0       97 2023-05-03 21:08:38.000000 blenderline-0.1.3/blenderline/entries/__init__.py
--rw-rw-rw-   0        0        0     2114 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/entries/background.py
--rw-rw-rw-   0        0        0      148 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/entries/base.py
--rw-rw-rw-   0        0        0     2007 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/entries/hdr.py
--rw-rw-rw-   0        0        0     2597 2023-05-25 15:18:05.000000 blenderline-0.1.3/blenderline/entries/item.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.456365 blenderline-0.1.3/blenderline/generators/
--rw-rw-rw-   0        0        0       42 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/generators/__init__.py
--rw-rw-rw-   0        0        0     3644 2023-05-25 16:37:57.000000 blenderline-0.1.3/blenderline/generators/image.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.466862 blenderline-0.1.3/blenderline/managers/
--rw-rw-rw-   0        0        0      136 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/managers/__init__.py
--rw-rw-rw-   0        0        0     1263 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/managers/background.py
--rw-rw-rw-   0        0        0     1169 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/managers/hdr.py
--rw-rw-rw-   0        0        0     5990 2023-05-09 20:32:49.000000 blenderline-0.1.3/blenderline/managers/item.py
--rw-rw-rw-   0        0        0     7346 2023-05-25 15:20:58.000000 blenderline-0.1.3/blenderline/managers/scene.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.466862 blenderline-0.1.3/blenderline/references/
--rw-rw-rw-   0        0        0       66 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/references/__init__.py
--rw-rw-rw-   0        0        0     3294 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/references/item.py
--rw-rw-rw-   0        0        0     3504 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/references/path.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.466862 blenderline-0.1.3/blenderline/scripts/
--rw-rw-rw-   0        0        0        0 2023-05-25 11:04:41.000000 blenderline-0.1.3/blenderline/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.477378 blenderline-0.1.3/blenderline/scripts/blender/
--rw-rw-rw-   0        0        0        0 2023-05-02 19:07:19.000000 blenderline-0.1.3/blenderline/scripts/blender/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-05-25 16:05:50.000000 blenderline-0.1.3/blenderline/scripts/blender/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.481484 blenderline-0.1.3/blenderline/scripts/python/
--rw-rw-rw-   0        0        0       70 2023-05-25 11:10:03.000000 blenderline-0.1.3/blenderline/scripts/python/__init__.py
--rw-rw-rw-   0        0        0      113 2023-05-25 15:58:54.000000 blenderline-0.1.3/blenderline/scripts/python/convert.py
--rw-rw-rw-   0        0        0     2223 2023-05-25 15:02:26.000000 blenderline-0.1.3/blenderline/scripts/python/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.487013 blenderline-0.1.3/blenderline/settings/
--rw-rw-rw-   0        0        0       41 2023-05-03 21:08:39.000000 blenderline-0.1.3/blenderline/settings/__init__.py
--rw-rw-rw-   0        0        0    10034 2023-05-25 16:38:02.000000 blenderline-0.1.3/blenderline/settings/image.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:54:44.433218 blenderline-0.1.3/blenderline.egg-info/
--rw-rw-rw-   0        0        0     5839 2023-06-01 10:54:44.000000 blenderline-0.1.3/blenderline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1218 2023-06-01 10:54:44.000000 blenderline-0.1.3/blenderline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 10:54:44.000000 blenderline-0.1.3/blenderline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-01 10:54:44.000000 blenderline-0.1.3/blenderline.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-06-01 10:54:44.000000 blenderline-0.1.3/blenderline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 10:54:44.000000 blenderline-0.1.3/blenderline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 10:54:44.490784 blenderline-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-06-01 10:54:27.000000 blenderline-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.747957 blenderline-0.1.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 21:03:35.000000 blenderline-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     5830 2023-06-01 10:57:28.746379 blenderline-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5277 2023-06-01 10:57:14.000000 blenderline-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.685355 blenderline-0.1.4/blenderline/
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:15:58.000000 blenderline-0.1.4/blenderline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.705495 blenderline-0.1.4/blenderline/collections/
+-rw-rw-rw-   0        0        0      112 2023-05-03 21:08:38.000000 blenderline-0.1.4/blenderline/collections/__init__.py
+-rw-rw-rw-   0        0        0      251 2023-05-24 20:47:31.000000 blenderline-0.1.4/blenderline/collections/background.py
+-rw-rw-rw-   0        0        0     1322 2023-05-24 20:47:29.000000 blenderline-0.1.4/blenderline/collections/base.py
+-rw-rw-rw-   0        0        0      227 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/collections/hdr.py
+-rw-rw-rw-   0        0        0      221 2023-05-03 21:08:38.000000 blenderline-0.1.4/blenderline/collections/item.py
+-rw-rw-rw-   0        0        0     4294 2023-05-25 16:12:54.000000 blenderline-0.1.4/blenderline/command_line.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.715002 blenderline-0.1.4/blenderline/entries/
+-rw-rw-rw-   0        0        0       97 2023-05-03 21:08:38.000000 blenderline-0.1.4/blenderline/entries/__init__.py
+-rw-rw-rw-   0        0        0     2114 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/entries/background.py
+-rw-rw-rw-   0        0        0      148 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/entries/base.py
+-rw-rw-rw-   0        0        0     2007 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/entries/hdr.py
+-rw-rw-rw-   0        0        0     2597 2023-05-25 15:18:05.000000 blenderline-0.1.4/blenderline/entries/item.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.715002 blenderline-0.1.4/blenderline/generators/
+-rw-rw-rw-   0        0        0       42 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/generators/__init__.py
+-rw-rw-rw-   0        0        0     3644 2023-05-25 16:37:57.000000 blenderline-0.1.4/blenderline/generators/image.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.721720 blenderline-0.1.4/blenderline/managers/
+-rw-rw-rw-   0        0        0      136 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/managers/__init__.py
+-rw-rw-rw-   0        0        0     1263 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/managers/background.py
+-rw-rw-rw-   0        0        0     1169 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/managers/hdr.py
+-rw-rw-rw-   0        0        0     5990 2023-05-09 20:32:49.000000 blenderline-0.1.4/blenderline/managers/item.py
+-rw-rw-rw-   0        0        0     7346 2023-05-25 15:20:58.000000 blenderline-0.1.4/blenderline/managers/scene.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.730728 blenderline-0.1.4/blenderline/references/
+-rw-rw-rw-   0        0        0       66 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/references/__init__.py
+-rw-rw-rw-   0        0        0     3294 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/references/item.py
+-rw-rw-rw-   0        0        0     3504 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/references/path.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.730728 blenderline-0.1.4/blenderline/scripts/
+-rw-rw-rw-   0        0        0        0 2023-05-25 11:04:41.000000 blenderline-0.1.4/blenderline/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.730728 blenderline-0.1.4/blenderline/scripts/blender/
+-rw-rw-rw-   0        0        0        0 2023-05-02 19:07:19.000000 blenderline-0.1.4/blenderline/scripts/blender/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-05-25 16:05:50.000000 blenderline-0.1.4/blenderline/scripts/blender/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.730728 blenderline-0.1.4/blenderline/scripts/python/
+-rw-rw-rw-   0        0        0       70 2023-05-25 11:10:03.000000 blenderline-0.1.4/blenderline/scripts/python/__init__.py
+-rw-rw-rw-   0        0        0      113 2023-05-25 15:58:54.000000 blenderline-0.1.4/blenderline/scripts/python/convert.py
+-rw-rw-rw-   0        0        0     2223 2023-05-25 15:02:26.000000 blenderline-0.1.4/blenderline/scripts/python/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.730728 blenderline-0.1.4/blenderline/settings/
+-rw-rw-rw-   0        0        0       41 2023-05-03 21:08:39.000000 blenderline-0.1.4/blenderline/settings/__init__.py
+-rw-rw-rw-   0        0        0    10034 2023-05-25 16:38:02.000000 blenderline-0.1.4/blenderline/settings/image.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:57:28.692368 blenderline-0.1.4/blenderline.egg-info/
+-rw-rw-rw-   0        0        0     5830 2023-06-01 10:57:28.000000 blenderline-0.1.4/blenderline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1218 2023-06-01 10:57:28.000000 blenderline-0.1.4/blenderline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 10:57:28.000000 blenderline-0.1.4/blenderline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-01 10:57:28.000000 blenderline-0.1.4/blenderline.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2023-06-01 10:57:28.000000 blenderline-0.1.4/blenderline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 10:57:28.000000 blenderline-0.1.4/blenderline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 10:57:28.748463 blenderline-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-06-01 10:57:21.000000 blenderline-0.1.4/setup.py
```

### Comparing `blenderline-0.1.3/LICENSE` & `blenderline-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/PKG-INFO` & `blenderline-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blenderline
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pipeline for generating synthetic production line images
 Home-page: https://github.com/MaxvandenHoven/blenderline
 Author: Max van den Hoven
 Author-email: max.hoven@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
@@ -18,15 +18,15 @@
 
 [![GPLv3](https://img.shields.io/static/v1?message=GPLv3&color=blue&label=License&style=flat)](https://www.gnu.org/licenses/gpl-3.0)
 [![Blender](https://img.shields.io/static/v1?message=3.10%2B&logo=python&color=blue&logoColor=white&label=Python&style=flat)](https://www.python.org/)
 [![Blender](https://img.shields.io/static/v1?message=3.4%2B&logo=blender&color=orange&logoColor=white&label=Blender&style=flat)](https://www.blender.org/)
 [![GPLv3](https://img.shields.io/static/v1?message=black&color=black&label=Code%20style&style=flat)](https://github.com/psf/black)
 
 
-![](https://raw.githubusercontent.com/maxvandenhoven/blenderline/main/img/workflow.png?raw=true)
+![](https://raw.githubusercontent.com/maxvandenhoven/blenderline/main/img/workflow.png)
 
 ## 1. Table of Contents
 <details>
 <summary> Table of Contents </summary>
 
 - [1. Table of Contents](#1-table-of-contents)
 - [2. Description](#2-description)
```

### Comparing `blenderline-0.1.3/README.md` & `blenderline-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![GPLv3](https://img.shields.io/static/v1?message=GPLv3&color=blue&label=License&style=flat)](https://www.gnu.org/licenses/gpl-3.0)
 [![Blender](https://img.shields.io/static/v1?message=3.10%2B&logo=python&color=blue&logoColor=white&label=Python&style=flat)](https://www.python.org/)
 [![Blender](https://img.shields.io/static/v1?message=3.4%2B&logo=blender&color=orange&logoColor=white&label=Blender&style=flat)](https://www.blender.org/)
 [![GPLv3](https://img.shields.io/static/v1?message=black&color=black&label=Code%20style&style=flat)](https://github.com/psf/black)
 
 
-![](https://raw.githubusercontent.com/maxvandenhoven/blenderline/main/img/workflow.png?raw=true)
+![](https://raw.githubusercontent.com/maxvandenhoven/blenderline/main/img/workflow.png)
 
 ## 1. Table of Contents
 <details>
 <summary> Table of Contents </summary>
 
 - [1. Table of Contents](#1-table-of-contents)
 - [2. Description](#2-description)
```

### Comparing `blenderline-0.1.3/blenderline/collections/base.py` & `blenderline-0.1.4/blenderline/collections/base.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/command_line.py` & `blenderline-0.1.4/blenderline/command_line.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/entries/background.py` & `blenderline-0.1.4/blenderline/entries/background.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/entries/hdr.py` & `blenderline-0.1.4/blenderline/entries/hdr.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/entries/item.py` & `blenderline-0.1.4/blenderline/entries/item.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/generators/image.py` & `blenderline-0.1.4/blenderline/generators/image.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/managers/background.py` & `blenderline-0.1.4/blenderline/managers/background.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/managers/hdr.py` & `blenderline-0.1.4/blenderline/managers/hdr.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/managers/item.py` & `blenderline-0.1.4/blenderline/managers/item.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/managers/scene.py` & `blenderline-0.1.4/blenderline/managers/scene.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/references/item.py` & `blenderline-0.1.4/blenderline/references/item.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/references/path.py` & `blenderline-0.1.4/blenderline/references/path.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/scripts/blender/generate.py` & `blenderline-0.1.4/blenderline/scripts/blender/generate.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/scripts/python/generate.py` & `blenderline-0.1.4/blenderline/scripts/python/generate.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline/settings/image.py` & `blenderline-0.1.4/blenderline/settings/image.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/blenderline.egg-info/PKG-INFO` & `blenderline-0.1.4/blenderline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blenderline
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pipeline for generating synthetic production line images
 Home-page: https://github.com/MaxvandenHoven/blenderline
 Author: Max van den Hoven
 Author-email: max.hoven@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
@@ -18,15 +18,15 @@
 
 [![GPLv3](https://img.shields.io/static/v1?message=GPLv3&color=blue&label=License&style=flat)](https://www.gnu.org/licenses/gpl-3.0)
 [![Blender](https://img.shields.io/static/v1?message=3.10%2B&logo=python&color=blue&logoColor=white&label=Python&style=flat)](https://www.python.org/)
 [![Blender](https://img.shields.io/static/v1?message=3.4%2B&logo=blender&color=orange&logoColor=white&label=Blender&style=flat)](https://www.blender.org/)
 [![GPLv3](https://img.shields.io/static/v1?message=black&color=black&label=Code%20style&style=flat)](https://github.com/psf/black)
 
 
-![](https://raw.githubusercontent.com/maxvandenhoven/blenderline/main/img/workflow.png?raw=true)
+![](https://raw.githubusercontent.com/maxvandenhoven/blenderline/main/img/workflow.png)
 
 ## 1. Table of Contents
 <details>
 <summary> Table of Contents </summary>
 
 - [1. Table of Contents](#1-table-of-contents)
 - [2. Description](#2-description)
```

### Comparing `blenderline-0.1.3/blenderline.egg-info/SOURCES.txt` & `blenderline-0.1.4/blenderline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.3/setup.py` & `blenderline-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="blenderline",
-    version="0.1.3",
+    version="0.1.4",
     description="A pipeline for generating synthetic production line images",
     packages=find_packages(exclude=["examples*", "data*"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MaxvandenHoven/blenderline",
     author="Max van den Hoven",
     author_email="max.hoven@gmail.com",
```

