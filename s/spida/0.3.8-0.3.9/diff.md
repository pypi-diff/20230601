# Comparing `tmp/spida-0.3.8.tar.gz` & `tmp/spida-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.3.8.tar", last modified: Wed May 31 20:54:22 2023, max compression
+gzip compressed data, was "spida-0.3.9.tar", last modified: Wed May 31 22:18:56 2023, max compression
```

## Comparing `spida-0.3.8.tar` & `spida-0.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.833371 spida-0.3.8/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.3.8/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6148 2023-05-31 20:54:22.832350 spida-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.3.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 20:54:22.834381 spida-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-31 20:53:06.000000 spida-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.790923 spida-0.3.8/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.3.8/spida/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.823669 spida-0.3.8/spida/data/
--rw-rw-rw-   0        0        0        2 2023-05-31 02:38:32.000000 spida-0.3.8/spida/data/config.json
--rw-rw-rw-   0        0        0    18541 2023-05-31 02:36:49.000000 spida-0.3.8/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.831337 spida-0.3.8/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.3.8/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5970 2023-05-31 20:52:48.000000 spida-0.3.8/spida/utils/img.py
--rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.3.8/spida/utils/misc.py
--rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.3.8/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.821575 spida-0.3.8/spida.egg-info/
--rw-rw-rw-   0        0        0     6148 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 22:18:56.719979 spida-0.3.9/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6148 2023-05-31 22:18:56.718822 spida-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 22:18:56.721017 spida-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-05-31 22:17:22.000000 spida-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:18:56.673124 spida-0.3.9/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.3.9/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:18:56.710352 spida-0.3.9/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-31 02:38:32.000000 spida-0.3.9/spida/data/config.json
+-rw-rw-rw-   0        0        0    18541 2023-05-31 02:36:49.000000 spida-0.3.9/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:18:56.717817 spida-0.3.9/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.3.9/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     7006 2023-05-31 22:17:13.000000 spida-0.3.9/spida/utils/img.py
+-rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.3.9/spida/utils/misc.py
+-rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.3.9/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:18:56.709324 spida-0.3.9/spida.egg-info/
+-rw-rw-rw-   0        0        0     6148 2023-05-31 22:18:56.000000 spida-0.3.9/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-31 22:18:56.000000 spida-0.3.9/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:18:56.000000 spida-0.3.9/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-31 22:18:56.000000 spida-0.3.9/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 22:18:56.000000 spida-0.3.9/spida.egg-info/top_level.txt
```

### Comparing `spida-0.3.8/LICENSE` & `spida-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.3.8/PKG-INFO` & `spida-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `spida-0.3.8/README.md` & `spida-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `spida-0.3.8/setup.py` & `spida-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.3.8",
+    version="0.3.9",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
```

### Comparing `spida-0.3.8/spida/stable_diffusion.py` & `spida-0.3.9/spida/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.8/spida/utils/img.py` & `spida-0.3.9/spida/utils/img.py`

 * *Files 10% similar despite different names*

```diff
@@ -125,14 +125,42 @@
                 x * w : (x + 1) * w,
             ] = imgs[i]
         else:
             break
     return dst
 
 
+def slice_imgs(img: np.ndarray, shape: tuple = (512, 512)):
+    """
+    Slice a given image into multiple smaller images of the specified shape.
+
+    Parameters
+    ----------
+    img : numpy.ndarray
+        The input image to be sliced. The shape should be (image height, image width, [number of channels]).
+
+    shape : tuple, optional
+        The desired shape of the smaller sliced images. The default shape is (512, 512).
+
+    Returns
+    -------
+    numpy.ndarray
+        An array containing the sliced images. The shape is (number of sliced images, slice height, slice width, [number of channels]).
+    """
+    img_height, img_width, *img_channels = img.shape
+    h, w = shape
+    y_num, x_num = img_height // h, img_width // w
+    num_imgs = y_num * x_num
+    dsts_shape = (num_imgs, h, w, *img_channels)
+    dsts = np.empty(shape=dsts_shape, dtype=img.dtype)
+    for i, (y, x) in enumerate(np.ndindex(y_num, x_num)):
+        dsts[i] = img[y * h : (y + 1) * h, x * w : (x + 1) * w]
+    return dsts
+
+
 def img2b64str(img: np.ndarray):
     """
     Convert a single image array to base64 string.
 
     Parameters
     ----------
     img : numpy.ndarray
```

### Comparing `spida-0.3.8/spida/utils/misc.py` & `spida-0.3.9/spida/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.8/spida/utils/net.py` & `spida-0.3.9/spida/utils/net.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.8/spida.egg-info/PKG-INFO` & `spida-0.3.9/spida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

