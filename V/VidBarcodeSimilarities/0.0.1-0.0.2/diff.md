# Comparing `tmp/VidBarcodeSimilarities-0.0.1.tar.gz` & `tmp/VidBarcodeSimilarities-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VidBarcodeSimilarities-0.0.1.tar", last modified: Wed May 31 22:50:57 2023, max compression
+gzip compressed data, was "VidBarcodeSimilarities-0.0.2.tar", last modified: Wed May 31 23:07:50 2023, max compression
```

## Comparing `VidBarcodeSimilarities-0.0.1.tar` & `VidBarcodeSimilarities-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:50:57.723614 VidBarcodeSimilarities-0.0.1/
--rw-rw-rw-   0        0        0      496 2023-05-31 22:50:57.718608 VidBarcodeSimilarities-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 22:50:57.600611 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities/
--rw-rw-rw-   0        0        0        0 2023-04-23 16:57:36.000000 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities/__init__.py
--rw-rw-rw-   0        0        0     1444 2023-04-23 16:40:28.000000 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities/model.py
--rw-rw-rw-   0        0        0     1272 2023-05-31 21:32:02.000000 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities/videobarcodesimilarities.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:50:57.714606 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities.egg-info/
--rw-rw-rw-   0        0        0      496 2023-05-31 22:50:57.000000 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-05-31 22:50:57.000000 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:50:57.000000 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-31 22:50:57.000000 VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 22:50:57.727610 VidBarcodeSimilarities-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-05-31 22:46:50.000000 VidBarcodeSimilarities-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:07:50.643760 VidBarcodeSimilarities-0.0.2/
+-rw-rw-rw-   0        0        0      496 2023-05-31 23:07:50.639762 VidBarcodeSimilarities-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 23:07:50.572761 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities/
+-rw-rw-rw-   0        0        0        0 2023-04-23 16:57:36.000000 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities/__init__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-23 16:40:28.000000 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities/model.py
+-rw-rw-rw-   0        0        0     1273 2023-05-31 23:05:13.000000 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities/videobarcodesimilarities.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:07:50.635760 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities.egg-info/
+-rw-rw-rw-   0        0        0      496 2023-05-31 23:07:50.000000 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-05-31 23:07:50.000000 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 23:07:50.000000 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-31 23:07:50.000000 VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 23:07:50.644760 VidBarcodeSimilarities-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-05-31 23:06:20.000000 VidBarcodeSimilarities-0.0.2/setup.py
```

### Comparing `VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities/model.py` & `VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities/model.py`

 * *Files identical despite different names*

### Comparing `VidBarcodeSimilarities-0.0.1/VidBarcodeSimilarities/videobarcodesimilarities.py` & `VidBarcodeSimilarities-0.0.2/VidBarcodeSimilarities/videobarcodesimilarities.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from PIL import Image
 import PIL.ImageOps
 import torchvision.transforms as transforms
 import torch.nn.functional as F
 
 def videoBarcodeSimilarities(image1_path: str, image2_path: str):
     model = SiameseNetwork()
-    PATH = "./dropdart.h5"
+    PATH = "./barimgsim.pt"
     # weights = torch.hub.load_state_dict_from_url(
     #     "https://github.com/smilingprogrammer/RealTimeNudityDetectionAlgorithm/blob/main/barimgsim.pt", progress=True
     # )
     model.load_state_dict(torch.load(PATH))
     model.eval()
 
     image1 = Image.open(image1_path)
```

### Comparing `VidBarcodeSimilarities-0.0.1/setup.py` & `VidBarcodeSimilarities-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="VidBarcodeSimilarities",
-    version="0.0.1",
+    version="0.0.2",
     description="A library to compare similarities between barcode images",
     author="Abdulsobur",
     author_email="Abdulsoburoyewale@gmail.com",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

