# Comparing `tmp/wow-ocr-0.0.1.tar.gz` & `tmp/wow-ocr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow-ocr-0.0.1.tar", last modified: Thu Jun  1 16:17:02 2023, max compression
+gzip compressed data, was "wow-ocr-0.0.2.tar", last modified: Thu Jun  1 17:03:20 2023, max compression
```

## Comparing `wow-ocr-0.0.1.tar` & `wow-ocr-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 16:17:02.707114 wow-ocr-0.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)     1022 2023-05-31 15:58:44.000000 wow-ocr-0.0.1/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     2496 2023-06-01 16:17:02.707114 wow-ocr-0.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      839 2023-06-01 15:45:25.000000 wow-ocr-0.0.1/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      925 2023-06-01 16:16:05.000000 wow-ocr-0.0.1/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)      102 2023-06-01 16:17:02.707114 wow-ocr-0.0.1/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 16:17:02.707114 wow-ocr-0.0.1/wow_ocr/
--rw-rw-r--   0 user      (1000) user      (1000)       75 2023-06-01 11:11:48.000000 wow-ocr-0.0.1/wow_ocr/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    31392 2023-06-01 16:06:19.000000 wow-ocr-0.0.1/wow_ocr/detector.py
--rw-rw-r--   0 user      (1000) user      (1000)     2779 2023-06-01 11:20:11.000000 wow-ocr-0.0.1/wow_ocr/pipeline.py
--rw-rw-r--   0 user      (1000) user      (1000)    19802 2023-06-01 16:10:07.000000 wow-ocr-0.0.1/wow_ocr/recognizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     4304 2023-06-01 11:21:03.000000 wow-ocr-0.0.1/wow_ocr/tools.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 16:17:02.707114 wow-ocr-0.0.1/wow_ocr.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2496 2023-06-01 16:17:02.000000 wow-ocr-0.0.1/wow_ocr.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      295 2023-06-01 16:17:02.000000 wow-ocr-0.0.1/wow_ocr.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-01 16:17:02.000000 wow-ocr-0.0.1/wow_ocr.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      174 2023-06-01 16:17:02.000000 wow-ocr-0.0.1/wow_ocr.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-01 16:17:02.000000 wow-ocr-0.0.1/wow_ocr.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 17:03:20.920844 wow-ocr-0.0.2/
+-rw-rw-r--   0 user      (1000) user      (1000)     1022 2023-05-31 15:58:44.000000 wow-ocr-0.0.2/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2653 2023-06-01 17:03:20.920844 wow-ocr-0.0.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      996 2023-06-01 17:01:47.000000 wow-ocr-0.0.2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      925 2023-06-01 17:02:44.000000 wow-ocr-0.0.2/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      102 2023-06-01 17:03:20.920844 wow-ocr-0.0.2/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 17:03:20.916844 wow-ocr-0.0.2/wow_ocr/
+-rw-rw-r--   0 user      (1000) user      (1000)       75 2023-06-01 11:11:48.000000 wow-ocr-0.0.2/wow_ocr/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    31392 2023-06-01 16:06:19.000000 wow-ocr-0.0.2/wow_ocr/detector.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2779 2023-06-01 11:20:11.000000 wow-ocr-0.0.2/wow_ocr/pipeline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19802 2023-06-01 16:10:07.000000 wow-ocr-0.0.2/wow_ocr/recognizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12944 2023-06-01 16:57:08.000000 wow-ocr-0.0.2/wow_ocr/tools.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 17:03:20.920844 wow-ocr-0.0.2/wow_ocr.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2653 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      295 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      174 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/top_level.txt
```

### Comparing `wow-ocr-0.0.1/LICENSE` & `wow-ocr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wow-ocr-0.0.1/PKG-INFO` & `wow-ocr-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ocr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A packaged OCR model to read texts into WoW screenshots
 Author-email: Geo <geoffrey.menon38@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -37,18 +37,24 @@
 
 - Chat
 - Combat log
 - Nameplates
 - UI frames
 - Map
 
+Installation
+-----
+
+### ```pip install wow-ocr```
+
+
 Usage
 ----
 
-Models will use pre trained weights, you don't have to train anything
+Models will use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
 
 ```
 import wow_ocr
 
 # Init pipeline, detector and recognizer models with pre trained weights
 pipeline = wow_ocr.pipeline.Pipeline()
 
@@ -67,8 +73,7 @@
 # # Each list of predictions in prediction_groups is a list of
 # # (word, box) tuples.
 
 ```
 
 ![](p1.webp)
 ![](p2.webp)
-
```

### Comparing `wow-ocr-0.0.1/README.md` & `wow-ocr-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 
 - Chat
 - Combat log
 - Nameplates
 - UI frames
 - Map
 
+Installation
+-----
+
+### ```pip install wow-ocr```
+
+
 Usage
 ----
 
-Models will use pre trained weights, you don't have to train anything
+Models will use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
 
 ```
 import wow_ocr
 
 # Init pipeline, detector and recognizer models with pre trained weights
 pipeline = wow_ocr.pipeline.Pipeline()
 
@@ -35,8 +41,7 @@
 # # Each list of predictions in prediction_groups is a list of
 # # (word, box) tuples.
 
 ```
 
 ![](p1.webp)
 ![](p2.webp)
-
```

### Comparing `wow-ocr-0.0.1/pyproject.toml` & `wow-ocr-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wow-ocr"
-version = "0.0.1"
+version = "0.0.2"
 description = "A packaged OCR model to read texts into WoW screenshots"
 readme = "README.md"
 authors = [{ name = "Geo", email = "geoffrey.menon38@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `wow-ocr-0.0.1/wow_ocr/detector.py` & `wow-ocr-0.0.2/wow_ocr/detector.py`

 * *Files identical despite different names*

### Comparing `wow-ocr-0.0.1/wow_ocr/pipeline.py` & `wow-ocr-0.0.2/wow_ocr/pipeline.py`

 * *Files identical despite different names*

### Comparing `wow-ocr-0.0.1/wow_ocr/recognizer.py` & `wow-ocr-0.0.2/wow_ocr/recognizer.py`

 * *Files identical despite different names*

### Comparing `wow-ocr-0.0.1/wow_ocr.egg-info/PKG-INFO` & `wow-ocr-0.0.2/wow_ocr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ocr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A packaged OCR model to read texts into WoW screenshots
 Author-email: Geo <geoffrey.menon38@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -37,18 +37,24 @@
 
 - Chat
 - Combat log
 - Nameplates
 - UI frames
 - Map
 
+Installation
+-----
+
+### ```pip install wow-ocr```
+
+
 Usage
 ----
 
-Models will use pre trained weights, you don't have to train anything
+Models will use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
 
 ```
 import wow_ocr
 
 # Init pipeline, detector and recognizer models with pre trained weights
 pipeline = wow_ocr.pipeline.Pipeline()
 
@@ -67,8 +73,7 @@
 # # Each list of predictions in prediction_groups is a list of
 # # (word, box) tuples.
 
 ```
 
 ![](p1.webp)
 ![](p2.webp)
-
```

