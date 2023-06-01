# Comparing `tmp/VidBarcodeSimilarities-0.0.3.tar.gz` & `tmp/VidBarcodeSimilarities-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VidBarcodeSimilarities-0.0.3.tar", last modified: Thu Jun  1 03:57:32 2023, max compression
+gzip compressed data, was "VidBarcodeSimilarities-0.0.4.tar", last modified: Thu Jun  1 04:52:40 2023, max compression
```

## Comparing `VidBarcodeSimilarities-0.0.3.tar` & `VidBarcodeSimilarities-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 03:57:30.723614 VidBarcodeSimilarities-0.0.3/
--rw-rw-rw-   0        0        0      496 2023-06-01 03:57:30.688604 VidBarcodeSimilarities-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 03:57:26.946612 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities/
--rw-rw-rw-   0        0        0        0 2023-04-23 16:57:36.000000 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities/__init__.py
--rw-rw-rw-   0        0        0     1444 2023-04-23 16:40:28.000000 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities/model.py
--rw-rw-rw-   0        0        0     1271 2023-05-31 23:19:27.000000 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities/videobarcodesimilarities.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:57:30.355605 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities.egg-info/
--rw-rw-rw-   0        0        0      496 2023-06-01 03:57:11.000000 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-06-01 03:57:14.000000 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:57:11.000000 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-01 03:57:12.000000 VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 03:57:30.904608 VidBarcodeSimilarities-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-06-01 03:53:07.000000 VidBarcodeSimilarities-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 04:52:40.113194 VidBarcodeSimilarities-0.0.4/
+-rw-rw-rw-   0        0        0      496 2023-06-01 04:52:40.066199 VidBarcodeSimilarities-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 04:52:39.628197 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities/
+-rw-rw-rw-   0        0        0        0 2023-04-23 16:57:36.000000 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities/__init__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-23 16:40:28.000000 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities/model.py
+-rw-rw-rw-   0        0        0     1377 2023-06-01 04:50:50.000000 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities/videobarcodesimilarities.py
+drwxrwxrwx   0        0        0        0 2023-06-01 04:52:40.045198 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities.egg-info/
+-rw-rw-rw-   0        0        0      496 2023-06-01 04:52:37.000000 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-06-01 04:52:37.000000 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 04:52:37.000000 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-01 04:52:37.000000 VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 04:52:40.168196 VidBarcodeSimilarities-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-06-01 04:51:40.000000 VidBarcodeSimilarities-0.0.4/setup.py
```

### Comparing `VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities/model.py` & `VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities/model.py`

 * *Files identical despite different names*

### Comparing `VidBarcodeSimilarities-0.0.3/VidBarcodeSimilarities/videobarcodesimilarities.py` & `VidBarcodeSimilarities-0.0.4/VidBarcodeSimilarities/videobarcodesimilarities.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
 import torch
 from .model import SiameseNetwork
 from PIL import Image
 import PIL.ImageOps
+import pkg_resources
 import torchvision.transforms as transforms
 import torch.nn.functional as F
 
 def videoBarcodeSimilarities(image1_path: str, image2_path: str):
     model = SiameseNetwork()
-    PATH = "barimgsim.pt"
+    weight_path = pkg_resources.resource_filename(__name__, 'barimgsim.pt')
+    # PATH = "barimgsim.pt"
     # weights = torch.hub.load_state_dict_from_url(
     #     "https://github.com/smilingprogrammer/RealTimeNudityDetectionAlgorithm/blob/main/barimgsim.pt", progress=True
     # )
-    model.load_state_dict(torch.load(PATH))
+    model.load_state_dict(torch.load(weight_path))
     model.eval()
 
     image1 = Image.open(image1_path)
     image2 = Image.open(image2_path)
 
     # Preprocess the images for ResNet50
     preprocess = transforms.Compose([
```

### Comparing `VidBarcodeSimilarities-0.0.3/setup.py` & `VidBarcodeSimilarities-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="VidBarcodeSimilarities",
-    version="0.0.3",
+    version="0.0.4",
     description="A library to compare similarities between barcode images",
     author="Abdulsobur",
     author_email="Abdulsoburoyewale@gmail.com",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

