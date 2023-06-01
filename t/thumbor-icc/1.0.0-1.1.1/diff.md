# Comparing `tmp/thumbor_icc-1.0.0.tar.gz` & `tmp/thumbor_icc-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/thumbor_icc-1.0.0.tar", last modified: Tue Jun 30 13:25:35 2020, max compression
+gzip compressed data, was "thumbor_icc-1.1.1.tar", last modified: Thu Jun  1 15:47:53 2023, max compression
```

## Comparing `thumbor_icc-1.0.0.tar` & `thumbor_icc-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lo        (1000) lo        (1000)        0 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/
--rw-r--r--   0 lo        (1000) lo        (1000)      879 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/PKG-INFO
--rw-r--r--   0 lo        (1000) lo        (1000)      336 2015-12-22 07:03:14.000000 thumbor_icc-1.0.0/README.rst
--rw-r--r--   0 lo        (1000) lo        (1000)       38 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/setup.cfg
--rw-r--r--   0 lo        (1000) lo        (1000)     1113 2020-06-26 14:42:38.000000 thumbor_icc-1.0.0/setup.py
-drwxr-xr-x   0 lo        (1000) lo        (1000)        0 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/thumbor_icc/
--rw-r--r--   0 lo        (1000) lo        (1000)      634 2020-06-26 13:59:25.000000 thumbor_icc-1.0.0/thumbor_icc/__init__.py
-drwxr-xr-x   0 lo        (1000) lo        (1000)        0 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/thumbor_icc/filters/
--rw-r--r--   0 lo        (1000) lo        (1000)        0 2015-12-21 15:42:21.000000 thumbor_icc-1.0.0/thumbor_icc/filters/__init__.py
--rw-r--r--   0 lo        (1000) lo        (1000)     4269 2020-06-30 13:24:47.000000 thumbor_icc-1.0.0/thumbor_icc/filters/icc_profile_apply.py
-drwxr-xr-x   0 lo        (1000) lo        (1000)        0 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/thumbor_icc.egg-info/
--rw-r--r--   0 lo        (1000) lo        (1000)      879 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/thumbor_icc.egg-info/PKG-INFO
--rw-r--r--   0 lo        (1000) lo        (1000)      290 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/thumbor_icc.egg-info/SOURCES.txt
--rw-r--r--   0 lo        (1000) lo        (1000)        1 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/thumbor_icc.egg-info/dependency_links.txt
--rw-r--r--   0 lo        (1000) lo        (1000)       26 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/thumbor_icc.egg-info/requires.txt
--rw-r--r--   0 lo        (1000) lo        (1000)       12 2020-06-30 13:25:35.000000 thumbor_icc-1.0.0/thumbor_icc.egg-info/top_level.txt
+drwxr-xr-x   0 lo        (1000) lo        (1000)        0 2023-06-01 15:47:53.619747 thumbor_icc-1.1.1/
+-rw-r--r--   0 lo        (1000) lo        (1000)      832 2023-06-01 15:47:53.619747 thumbor_icc-1.1.1/PKG-INFO
+-rw-r--r--   0 lo        (1000) lo        (1000)      336 2015-12-22 07:03:14.000000 thumbor_icc-1.1.1/README.rst
+-rw-r--r--   0 lo        (1000) lo        (1000)       38 2023-06-01 15:47:53.623747 thumbor_icc-1.1.1/setup.cfg
+-rw-r--r--   0 lo        (1000) lo        (1000)     1113 2023-06-01 15:43:04.000000 thumbor_icc-1.1.1/setup.py
+drwxr-xr-x   0 lo        (1000) lo        (1000)        0 2023-06-01 15:47:53.619747 thumbor_icc-1.1.1/thumbor_icc/
+-rw-r--r--   0 lo        (1000) lo        (1000)      634 2020-06-26 13:59:25.000000 thumbor_icc-1.1.1/thumbor_icc/__init__.py
+drwxr-xr-x   0 lo        (1000) lo        (1000)        0 2023-06-01 15:47:53.619747 thumbor_icc-1.1.1/thumbor_icc/filters/
+-rw-r--r--   0 lo        (1000) lo        (1000)        0 2015-12-21 15:42:21.000000 thumbor_icc-1.1.1/thumbor_icc/filters/__init__.py
+-rw-r--r--   0 lo        (1000) lo        (1000)     3836 2023-06-01 15:36:52.000000 thumbor_icc-1.1.1/thumbor_icc/filters/icc_profile_apply.py
+drwxr-xr-x   0 lo        (1000) lo        (1000)        0 2023-06-01 15:47:53.619747 thumbor_icc-1.1.1/thumbor_icc.egg-info/
+-rw-r--r--   0 lo        (1000) lo        (1000)      832 2023-06-01 15:47:53.000000 thumbor_icc-1.1.1/thumbor_icc.egg-info/PKG-INFO
+-rw-r--r--   0 lo        (1000) lo        (1000)      290 2023-06-01 15:47:53.000000 thumbor_icc-1.1.1/thumbor_icc.egg-info/SOURCES.txt
+-rw-r--r--   0 lo        (1000) lo        (1000)        1 2023-06-01 15:47:53.000000 thumbor_icc-1.1.1/thumbor_icc.egg-info/dependency_links.txt
+-rw-r--r--   0 lo        (1000) lo        (1000)       26 2023-06-01 15:47:53.000000 thumbor_icc-1.1.1/thumbor_icc.egg-info/requires.txt
+-rw-r--r--   0 lo        (1000) lo        (1000)       12 2023-06-01 15:47:53.000000 thumbor_icc-1.1.1/thumbor_icc.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `thumbor_icc-1.0.0/PKG-INFO` & `thumbor_icc-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: thumbor_icc
-Version: 1.0.0
+Version: 1.1.1
 Summary: Color management filters for thumbor
 Home-page: https://github.com/znerol/thumbor-icc
 Author: Lorenz Schori
 Author-email: lo@znerol.ch
 License: MIT
-Description: Thumbor is a smart imaging service. It enables on-demand crop, resizing and
-        flipping of images. This module provide support for color management profiles.
-        
 Keywords: thumbor,icc,images
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
+
+Thumbor is a smart imaging service. It enables on-demand crop, resizing and
+flipping of images. This module provide support for color management profiles.
```

### Comparing `thumbor_icc-1.0.0/setup.py` & `thumbor_icc-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name="thumbor_icc",
     packages=find_packages(),
-    version="1.0.0",
+    version="1.1.1",
     description="Color management filters for thumbor",
     author="Lorenz Schori",
     author_email="lo@znerol.ch",
     keywords=["thumbor", "icc", "images"],
     license="MIT",
     url="https://github.com/znerol/thumbor-icc",
     classifiers=[
```

### Comparing `thumbor_icc-1.0.0/thumbor_icc/__init__.py` & `thumbor_icc-1.1.1/thumbor_icc/__init__.py`

 * *Files identical despite different names*

### Comparing `thumbor_icc-1.0.0/thumbor_icc/filters/icc_profile_apply.py` & `thumbor_icc-1.1.1/thumbor_icc/filters/icc_profile_apply.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,17 @@
 # -*- coding: utf-8 -*-
 
 """
 A collection of thumbor filters providing better support for color managed
 images.
 """
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import unicode_literals
-
 import os
 
-from cStringIO import StringIO
+from io import BytesIO
 
 from PIL import Image, ImageCms
 from thumbor.filters import BaseFilter, filter_method, PHASE_AFTER_LOAD
 from thumbor.utils import logger
 
 
 # pylint: disable=R0903
@@ -81,22 +77,15 @@
             return
 
         try:
             inmode = self.engine.get_image_mode()
             insize = self.engine.size
             indata = self.engine.get_image_data()
             inimg = Image.frombytes(inmode, insize, indata)
-
-            # In PIL>=3.0.0 / Thumbor 6, icc_profile is sometimes a tuple :/
-            # https://github.com/python-pillow/Pillow/issues/1462
-            profile_data = self.engine.icc_profile
-            # pylint: disable=C0123
-            if type(profile_data) == tuple:
-                profile_data = profile_data[0]
-            inprofile = StringIO(profile_data)
+            inprofile = BytesIO(self.engine.icc_profile)
 
             outmode = "RGBA" if "A" in inmode else "RGB"
         except Exception:
             logger.exception("ICC: Failed to determine image "
                              "properties before attempting to apply "
                              "profile: {:s}".format(profile))
             return
@@ -109,15 +98,15 @@
         except Exception:
             logger.exception("ICC: Failed to apply profile: {:s}, "
                              "inmode: {:s}, "
                              "outmode: {:s}".format(profile, inmode, outmode))
             return
 
         # Reload the image into the engine.
-        outbuf = StringIO()
+        outbuf = BytesIO()
         try:
             outimg.save(outbuf, fmt)
             self.engine.load(outbuf.getvalue(), ext)
         except Exception:
             logger.exception("ICC: Failed load the image with an applied "
                              "profile: {:s}, inmode: {:s}, "
                              "outmode: {:s}".format(profile, inmode, outmode))
```

### Comparing `thumbor_icc-1.0.0/thumbor_icc.egg-info/PKG-INFO` & `thumbor_icc-1.1.1/thumbor_icc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: thumbor-icc
-Version: 1.0.0
+Version: 1.1.1
 Summary: Color management filters for thumbor
 Home-page: https://github.com/znerol/thumbor-icc
 Author: Lorenz Schori
 Author-email: lo@znerol.ch
 License: MIT
-Description: Thumbor is a smart imaging service. It enables on-demand crop, resizing and
-        flipping of images. This module provide support for color management profiles.
-        
 Keywords: thumbor,icc,images
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
+
+Thumbor is a smart imaging service. It enables on-demand crop, resizing and
+flipping of images. This module provide support for color management profiles.
```

