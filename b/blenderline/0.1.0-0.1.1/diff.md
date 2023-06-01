# Comparing `tmp/blenderline-0.1.0.tar.gz` & `tmp/blenderline-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blenderline-0.1.0.tar", last modified: Thu Jun  1 10:26:40 2023, max compression
+gzip compressed data, was "blenderline-0.1.1.tar", last modified: Thu Jun  1 10:38:48 2023, max compression
```

## Comparing `blenderline-0.1.0.tar` & `blenderline-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.416710 blenderline-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-04-12 21:03:35.000000 blenderline-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6061 2023-06-01 10:26:40.416710 blenderline-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5268 2023-06-01 09:18:03.000000 blenderline-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.354179 blenderline-0.1.0/blenderline/
--rw-rw-rw-   0        0        0        0 2023-04-12 21:15:58.000000 blenderline-0.1.0/blenderline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.373164 blenderline-0.1.0/blenderline/collections/
--rw-rw-rw-   0        0        0      112 2023-05-03 21:08:38.000000 blenderline-0.1.0/blenderline/collections/__init__.py
--rw-rw-rw-   0        0        0      251 2023-05-24 20:47:31.000000 blenderline-0.1.0/blenderline/collections/background.py
--rw-rw-rw-   0        0        0     1322 2023-05-24 20:47:29.000000 blenderline-0.1.0/blenderline/collections/base.py
--rw-rw-rw-   0        0        0      227 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/collections/hdr.py
--rw-rw-rw-   0        0        0      221 2023-05-03 21:08:38.000000 blenderline-0.1.0/blenderline/collections/item.py
--rw-rw-rw-   0        0        0     4294 2023-05-25 16:12:54.000000 blenderline-0.1.0/blenderline/command_line.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.385673 blenderline-0.1.0/blenderline/entries/
--rw-rw-rw-   0        0        0       97 2023-05-03 21:08:38.000000 blenderline-0.1.0/blenderline/entries/__init__.py
--rw-rw-rw-   0        0        0     2114 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/entries/background.py
--rw-rw-rw-   0        0        0      148 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/entries/base.py
--rw-rw-rw-   0        0        0     2007 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/entries/hdr.py
--rw-rw-rw-   0        0        0     2597 2023-05-25 15:18:05.000000 blenderline-0.1.0/blenderline/entries/item.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.389721 blenderline-0.1.0/blenderline/generators/
--rw-rw-rw-   0        0        0       42 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/generators/__init__.py
--rw-rw-rw-   0        0        0     3644 2023-05-25 16:37:57.000000 blenderline-0.1.0/blenderline/generators/image.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.394732 blenderline-0.1.0/blenderline/managers/
--rw-rw-rw-   0        0        0      136 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/managers/__init__.py
--rw-rw-rw-   0        0        0     1263 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/managers/background.py
--rw-rw-rw-   0        0        0     1169 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/managers/hdr.py
--rw-rw-rw-   0        0        0     5990 2023-05-09 20:32:49.000000 blenderline-0.1.0/blenderline/managers/item.py
--rw-rw-rw-   0        0        0     7346 2023-05-25 15:20:58.000000 blenderline-0.1.0/blenderline/managers/scene.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.405445 blenderline-0.1.0/blenderline/references/
--rw-rw-rw-   0        0        0       66 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/references/__init__.py
--rw-rw-rw-   0        0        0     3294 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/references/item.py
--rw-rw-rw-   0        0        0     3504 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/references/path.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.405445 blenderline-0.1.0/blenderline/scripts/
--rw-rw-rw-   0        0        0        0 2023-05-25 11:04:41.000000 blenderline-0.1.0/blenderline/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.409371 blenderline-0.1.0/blenderline/scripts/blender/
--rw-rw-rw-   0        0        0        0 2023-05-02 19:07:19.000000 blenderline-0.1.0/blenderline/scripts/blender/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-05-25 16:05:50.000000 blenderline-0.1.0/blenderline/scripts/blender/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.413879 blenderline-0.1.0/blenderline/scripts/python/
--rw-rw-rw-   0        0        0       70 2023-05-25 11:10:03.000000 blenderline-0.1.0/blenderline/scripts/python/__init__.py
--rw-rw-rw-   0        0        0      113 2023-05-25 15:58:54.000000 blenderline-0.1.0/blenderline/scripts/python/convert.py
--rw-rw-rw-   0        0        0     2223 2023-05-25 15:02:26.000000 blenderline-0.1.0/blenderline/scripts/python/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.416710 blenderline-0.1.0/blenderline/settings/
--rw-rw-rw-   0        0        0       41 2023-05-03 21:08:39.000000 blenderline-0.1.0/blenderline/settings/__init__.py
--rw-rw-rw-   0        0        0    10034 2023-05-25 16:38:02.000000 blenderline-0.1.0/blenderline/settings/image.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:26:40.365484 blenderline-0.1.0/blenderline.egg-info/
--rw-rw-rw-   0        0        0     6061 2023-06-01 10:26:40.000000 blenderline-0.1.0/blenderline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1218 2023-06-01 10:26:40.000000 blenderline-0.1.0/blenderline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 10:26:40.000000 blenderline-0.1.0/blenderline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-01 10:26:40.000000 blenderline-0.1.0/blenderline.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-06-01 10:26:40.000000 blenderline-0.1.0/blenderline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 10:26:40.000000 blenderline-0.1.0/blenderline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 10:26:40.416710 blenderline-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-06-01 10:26:04.000000 blenderline-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.330914 blenderline-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 21:03:35.000000 blenderline-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5722 2023-06-01 10:38:48.330914 blenderline-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5169 2023-06-01 10:35:14.000000 blenderline-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.265613 blenderline-0.1.1/blenderline/
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:15:58.000000 blenderline-0.1.1/blenderline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.289160 blenderline-0.1.1/blenderline/collections/
+-rw-rw-rw-   0        0        0      112 2023-05-03 21:08:38.000000 blenderline-0.1.1/blenderline/collections/__init__.py
+-rw-rw-rw-   0        0        0      251 2023-05-24 20:47:31.000000 blenderline-0.1.1/blenderline/collections/background.py
+-rw-rw-rw-   0        0        0     1322 2023-05-24 20:47:29.000000 blenderline-0.1.1/blenderline/collections/base.py
+-rw-rw-rw-   0        0        0      227 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/collections/hdr.py
+-rw-rw-rw-   0        0        0      221 2023-05-03 21:08:38.000000 blenderline-0.1.1/blenderline/collections/item.py
+-rw-rw-rw-   0        0        0     4294 2023-05-25 16:12:54.000000 blenderline-0.1.1/blenderline/command_line.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.297575 blenderline-0.1.1/blenderline/entries/
+-rw-rw-rw-   0        0        0       97 2023-05-03 21:08:38.000000 blenderline-0.1.1/blenderline/entries/__init__.py
+-rw-rw-rw-   0        0        0     2114 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/entries/background.py
+-rw-rw-rw-   0        0        0      148 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/entries/base.py
+-rw-rw-rw-   0        0        0     2007 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/entries/hdr.py
+-rw-rw-rw-   0        0        0     2597 2023-05-25 15:18:05.000000 blenderline-0.1.1/blenderline/entries/item.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.297575 blenderline-0.1.1/blenderline/generators/
+-rw-rw-rw-   0        0        0       42 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/generators/__init__.py
+-rw-rw-rw-   0        0        0     3644 2023-05-25 16:37:57.000000 blenderline-0.1.1/blenderline/generators/image.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.312248 blenderline-0.1.1/blenderline/managers/
+-rw-rw-rw-   0        0        0      136 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/managers/__init__.py
+-rw-rw-rw-   0        0        0     1263 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/managers/background.py
+-rw-rw-rw-   0        0        0     1169 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/managers/hdr.py
+-rw-rw-rw-   0        0        0     5990 2023-05-09 20:32:49.000000 blenderline-0.1.1/blenderline/managers/item.py
+-rw-rw-rw-   0        0        0     7346 2023-05-25 15:20:58.000000 blenderline-0.1.1/blenderline/managers/scene.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.312248 blenderline-0.1.1/blenderline/references/
+-rw-rw-rw-   0        0        0       66 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/references/__init__.py
+-rw-rw-rw-   0        0        0     3294 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/references/item.py
+-rw-rw-rw-   0        0        0     3504 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/references/path.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.312248 blenderline-0.1.1/blenderline/scripts/
+-rw-rw-rw-   0        0        0        0 2023-05-25 11:04:41.000000 blenderline-0.1.1/blenderline/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.323821 blenderline-0.1.1/blenderline/scripts/blender/
+-rw-rw-rw-   0        0        0        0 2023-05-02 19:07:19.000000 blenderline-0.1.1/blenderline/scripts/blender/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-05-25 16:05:50.000000 blenderline-0.1.1/blenderline/scripts/blender/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.327907 blenderline-0.1.1/blenderline/scripts/python/
+-rw-rw-rw-   0        0        0       70 2023-05-25 11:10:03.000000 blenderline-0.1.1/blenderline/scripts/python/__init__.py
+-rw-rw-rw-   0        0        0      113 2023-05-25 15:58:54.000000 blenderline-0.1.1/blenderline/scripts/python/convert.py
+-rw-rw-rw-   0        0        0     2223 2023-05-25 15:02:26.000000 blenderline-0.1.1/blenderline/scripts/python/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.330914 blenderline-0.1.1/blenderline/settings/
+-rw-rw-rw-   0        0        0       41 2023-05-03 21:08:39.000000 blenderline-0.1.1/blenderline/settings/__init__.py
+-rw-rw-rw-   0        0        0    10034 2023-05-25 16:38:02.000000 blenderline-0.1.1/blenderline/settings/image.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:38:48.281258 blenderline-0.1.1/blenderline.egg-info/
+-rw-rw-rw-   0        0        0     5722 2023-06-01 10:38:48.000000 blenderline-0.1.1/blenderline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1218 2023-06-01 10:38:48.000000 blenderline-0.1.1/blenderline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 10:38:48.000000 blenderline-0.1.1/blenderline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-01 10:38:48.000000 blenderline-0.1.1/blenderline.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2023-06-01 10:38:48.000000 blenderline-0.1.1/blenderline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 10:38:48.000000 blenderline-0.1.1/blenderline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 10:38:48.330914 blenderline-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2023-06-01 10:35:18.000000 blenderline-0.1.1/setup.py
```

### Comparing `blenderline-0.1.0/LICENSE` & `blenderline-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/PKG-INFO` & `blenderline-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blenderline
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pipeline for generating synthetic production line images
 Home-page: https://github.com/MaxvandenHoven/blenderline
 Author: Max van den Hoven
 Author-email: max.hoven@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
@@ -79,38 +79,39 @@
 ```
 blenderline generate --config examples/example_beer/images.json --target data/raw
 ```
 
 This will generate a dataset with the following structure:
 ```
 data/
-â””â”€ raw/
-   â””â”€ example_beer/
-      â”œâ”€ train/
-      â”‚  â”œâ”€ 0/
-      â”‚  â”‚  â”œâ”€ image__f0825a6262fc__0001.png
-      â”‚  â”‚  â”œâ”€ mask__0__8acdea079f10__0001.png
-      â”‚  â”‚  â”œâ”€ mask__1__0181a303d637__0001.png
-      â”‚  â”‚  â””â”€ ...
-      â”‚  â””â”€ 1/
-      â”‚     â”œâ”€ image__7abe7f02c7d9__0001.png
-      â”‚     â”œâ”€ mask__1__19abef8a5cef__0001.png
-      â”‚     â”œâ”€ mask__1__d980d4a83682__0001.png
-      â”‚     â””â”€ ...
-      â”œâ”€ valid/
-      â”‚  â”œâ”€ 0/...
-      â”‚  â””â”€ 1/...
-      â””â”€ label_mapping.json
++- raw/
+   +- example_beer/
+      +- train/
+      |  +- 0/
+      |  |  +- image__f0825a6262fc__0001.png
+      |  |  +- mask__0__8acdea079f10__0001.png
+      |  |  +- mask__1__0181a303d637__0001.png
+      |  |  +- ...
+      |  +- 1/
+      |     +- image__7abe7f02c7d9__0001.png
+      |     +- mask__1__19abef8a5cef__0001.png
+      |     +- mask__1__d980d4a83682__0001.png
+      |     +- ...
+      +- valid/
+      |  +- 0/...
+      |  +- 1/...
+      +- label_mapping.json
 
 ```
 
 While not strictly necessary, setting `--target data/raw` will create a folder structure that allows you to track different versions of the data, e.g., after using the `blenderline convert` command. 
 
 Note that the dataset root folder (here named `example_beer`) contains subfolders for different splits defined in the configuration file. Each split contains a numbered list of instance folders, each containing a rendered image and a set of masks. An example instance might look as follows:
-![Example instance](/img/example-instance.png)
+![Example instance](img/example-instance.png)
+
 
 Image and mask files use the following naming convention:
 ```
 image__<random image ID>__0001.png
 mask__<class ID>__<random mask ID>__0001.png
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `blenderline-0.1.0/README.md` & `blenderline-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -63,38 +63,39 @@
 ```
 blenderline generate --config examples/example_beer/images.json --target data/raw
 ```
 
 This will generate a dataset with the following structure:
 ```
 data/
-└─ raw/
-   └─ example_beer/
-      ├─ train/
-      │  ├─ 0/
-      │  │  ├─ image__f0825a6262fc__0001.png
-      │  │  ├─ mask__0__8acdea079f10__0001.png
-      │  │  ├─ mask__1__0181a303d637__0001.png
-      │  │  └─ ...
-      │  └─ 1/
-      │     ├─ image__7abe7f02c7d9__0001.png
-      │     ├─ mask__1__19abef8a5cef__0001.png
-      │     ├─ mask__1__d980d4a83682__0001.png
-      │     └─ ...
-      ├─ valid/
-      │  ├─ 0/...
-      │  └─ 1/...
-      └─ label_mapping.json
++- raw/
+   +- example_beer/
+      +- train/
+      |  +- 0/
+      |  |  +- image__f0825a6262fc__0001.png
+      |  |  +- mask__0__8acdea079f10__0001.png
+      |  |  +- mask__1__0181a303d637__0001.png
+      |  |  +- ...
+      |  +- 1/
+      |     +- image__7abe7f02c7d9__0001.png
+      |     +- mask__1__19abef8a5cef__0001.png
+      |     +- mask__1__d980d4a83682__0001.png
+      |     +- ...
+      +- valid/
+      |  +- 0/...
+      |  +- 1/...
+      +- label_mapping.json
 
 ```
 
 While not strictly necessary, setting `--target data/raw` will create a folder structure that allows you to track different versions of the data, e.g., after using the `blenderline convert` command. 
 
 Note that the dataset root folder (here named `example_beer`) contains subfolders for different splits defined in the configuration file. Each split contains a numbered list of instance folders, each containing a rendered image and a set of masks. An example instance might look as follows:
-![Example instance](/img/example-instance.png)
+![Example instance](img/example-instance.png)
+
 
 Image and mask files use the following naming convention:
 ```
 image__<random image ID>__0001.png
 mask__<class ID>__<random mask ID>__0001.png
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `blenderline-0.1.0/blenderline/collections/base.py` & `blenderline-0.1.1/blenderline/collections/base.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/command_line.py` & `blenderline-0.1.1/blenderline/command_line.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/entries/background.py` & `blenderline-0.1.1/blenderline/entries/background.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/entries/hdr.py` & `blenderline-0.1.1/blenderline/entries/hdr.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/entries/item.py` & `blenderline-0.1.1/blenderline/entries/item.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/generators/image.py` & `blenderline-0.1.1/blenderline/generators/image.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/managers/background.py` & `blenderline-0.1.1/blenderline/managers/background.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/managers/hdr.py` & `blenderline-0.1.1/blenderline/managers/hdr.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/managers/item.py` & `blenderline-0.1.1/blenderline/managers/item.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/managers/scene.py` & `blenderline-0.1.1/blenderline/managers/scene.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/references/item.py` & `blenderline-0.1.1/blenderline/references/item.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/references/path.py` & `blenderline-0.1.1/blenderline/references/path.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/scripts/blender/generate.py` & `blenderline-0.1.1/blenderline/scripts/blender/generate.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/scripts/python/generate.py` & `blenderline-0.1.1/blenderline/scripts/python/generate.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline/settings/image.py` & `blenderline-0.1.1/blenderline/settings/image.py`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/blenderline.egg-info/PKG-INFO` & `blenderline-0.1.1/blenderline.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blenderline
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pipeline for generating synthetic production line images
 Home-page: https://github.com/MaxvandenHoven/blenderline
 Author: Max van den Hoven
 Author-email: max.hoven@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
@@ -79,38 +79,39 @@
 ```
 blenderline generate --config examples/example_beer/images.json --target data/raw
 ```
 
 This will generate a dataset with the following structure:
 ```
 data/
-â””â”€ raw/
-   â””â”€ example_beer/
-      â”œâ”€ train/
-      â”‚  â”œâ”€ 0/
-      â”‚  â”‚  â”œâ”€ image__f0825a6262fc__0001.png
-      â”‚  â”‚  â”œâ”€ mask__0__8acdea079f10__0001.png
-      â”‚  â”‚  â”œâ”€ mask__1__0181a303d637__0001.png
-      â”‚  â”‚  â””â”€ ...
-      â”‚  â””â”€ 1/
-      â”‚     â”œâ”€ image__7abe7f02c7d9__0001.png
-      â”‚     â”œâ”€ mask__1__19abef8a5cef__0001.png
-      â”‚     â”œâ”€ mask__1__d980d4a83682__0001.png
-      â”‚     â””â”€ ...
-      â”œâ”€ valid/
-      â”‚  â”œâ”€ 0/...
-      â”‚  â””â”€ 1/...
-      â””â”€ label_mapping.json
++- raw/
+   +- example_beer/
+      +- train/
+      |  +- 0/
+      |  |  +- image__f0825a6262fc__0001.png
+      |  |  +- mask__0__8acdea079f10__0001.png
+      |  |  +- mask__1__0181a303d637__0001.png
+      |  |  +- ...
+      |  +- 1/
+      |     +- image__7abe7f02c7d9__0001.png
+      |     +- mask__1__19abef8a5cef__0001.png
+      |     +- mask__1__d980d4a83682__0001.png
+      |     +- ...
+      +- valid/
+      |  +- 0/...
+      |  +- 1/...
+      +- label_mapping.json
 
 ```
 
 While not strictly necessary, setting `--target data/raw` will create a folder structure that allows you to track different versions of the data, e.g., after using the `blenderline convert` command. 
 
 Note that the dataset root folder (here named `example_beer`) contains subfolders for different splits defined in the configuration file. Each split contains a numbered list of instance folders, each containing a rendered image and a set of masks. An example instance might look as follows:
-![Example instance](/img/example-instance.png)
+![Example instance](img/example-instance.png)
+
 
 Image and mask files use the following naming convention:
 ```
 image__<random image ID>__0001.png
 mask__<class ID>__<random mask ID>__0001.png
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `blenderline-0.1.0/blenderline.egg-info/SOURCES.txt` & `blenderline-0.1.1/blenderline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blenderline-0.1.0/setup.py` & `blenderline-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="blenderline",
-    version="0.1.0",
+    version="0.1.1",
     description="A pipeline for generating synthetic production line images",
     packages=find_packages(exclude=["examples*", "data*"]),
+    include_dirs=[
+        "img",
+        "examples",
+    ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MaxvandenHoven/blenderline",
     author="Max van den Hoven",
     author_email="max.hoven@gmail.com",
     license="GPLv3",
     classifiers=[
```

