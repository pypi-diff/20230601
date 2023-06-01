# Comparing `tmp/APIxoo-0.2.0.tar.gz` & `tmp/APIxoo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APIxoo-0.2.0.tar", last modified: Sun May 21 13:42:00 2023, max compression
+gzip compressed data, was "APIxoo-0.3.0.tar", last modified: Thu Jun  1 11:30:59 2023, max compression
```

## Comparing `APIxoo-0.2.0.tar` & `APIxoo-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:42:00.296353 APIxoo-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:42:00.296353 APIxoo-0.2.0/APIxoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-21 13:41:47.000000 APIxoo-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-21 13:42:00.296353 APIxoo-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 13:41:47.000000 APIxoo-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:42:00.296353 APIxoo-0.2.0/apixoo/
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-21 13:41:47.000000 APIxoo-0.2.0/apixoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-21 13:41:47.000000 APIxoo-0.2.0/apixoo/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-21 13:41:47.000000 APIxoo-0.2.0/apixoo/pixel_bean.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-05-21 13:41:47.000000 APIxoo-0.2.0/apixoo/pixel_bean_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:42:00.296353 APIxoo-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 13:41:47.000000 APIxoo-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:30:59.852181 APIxoo-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:30:59.848181 APIxoo-0.3.0/APIxoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-01 11:30:48.000000 APIxoo-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-01 11:30:59.852181 APIxoo-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-01 11:30:48.000000 APIxoo-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:30:59.852181 APIxoo-0.3.0/apixoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-01 11:30:48.000000 APIxoo-0.3.0/apixoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-01 11:30:48.000000 APIxoo-0.3.0/apixoo/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-01 11:30:48.000000 APIxoo-0.3.0/apixoo/pixel_bean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-01 11:30:48.000000 APIxoo-0.3.0/apixoo/pixel_bean_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:30:59.852181 APIxoo-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 11:30:48.000000 APIxoo-0.3.0/setup.py
```

### Comparing `APIxoo-0.2.0/APIxoo.egg-info/PKG-INFO` & `APIxoo-0.3.0/APIxoo.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 Metadata-Version: 2.1
 Name: APIxoo
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python wrapper for Divoom Pixoo server API
 Home-page: https://github.com/redphx/apixoo
 Download-URL: https://github.com/redphx/apixoo
 Author: redphx
 License: MIT
 Keywords: apixoo,divoom,pixoo,pixoo64
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# [WIP] APIxoo
-Python module to interact with Divoom Pixoo app's server. .  
+[![PyPI](https://img.shields.io/pypi/v/APIxoo?label=PyPI%20Package)](https://pypi.org/project/APIxoo/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+# APIxoo
+Python package to interact with Divoom Pixoo app's server.  
+Unlike other packages, this one will only focus on interacting with Divoom Pixoo's server.  
   
-Unlike other libraries, this one will only focus on interacting with Divoom Pixoo's server.  
+For ESP32/Arduino, check [redphx/DivoomClient](https://github.com/redphx/DivoomClient). 
 
-- Support decoding Divoom's animation formats to GIFs (16x16, 32x32, 64x64).  
+## Features
+- [x] Login
+- [x] Decode Divoom's animation formats to GIFs (16x16, 32x32, 64x64).  
+- [x] Get animation by ID
+- [x] Get animations by Category
+- [x] Get animations by Album
+- [ ] Get animations by User
+- [ ] Search animations & users
+- [ ] Like/Dislike animation
+- [ ] Comment on animation
+- [ ] Upload animations
 
 ## Install
 ```
 pip install APIxoo
 ```
 
 ## Example
```

### Comparing `APIxoo-0.2.0/LICENSE.md` & `APIxoo-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `APIxoo-0.2.0/PKG-INFO` & `APIxoo-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 Metadata-Version: 2.1
 Name: APIxoo
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python wrapper for Divoom Pixoo server API
 Home-page: https://github.com/redphx/apixoo
 Download-URL: https://github.com/redphx/apixoo
 Author: redphx
 License: MIT
 Keywords: apixoo,divoom,pixoo,pixoo64
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# [WIP] APIxoo
-Python module to interact with Divoom Pixoo app's server. .  
+[![PyPI](https://img.shields.io/pypi/v/APIxoo?label=PyPI%20Package)](https://pypi.org/project/APIxoo/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+# APIxoo
+Python package to interact with Divoom Pixoo app's server.  
+Unlike other packages, this one will only focus on interacting with Divoom Pixoo's server.  
   
-Unlike other libraries, this one will only focus on interacting with Divoom Pixoo's server.  
+For ESP32/Arduino, check [redphx/DivoomClient](https://github.com/redphx/DivoomClient). 
 
-- Support decoding Divoom's animation formats to GIFs (16x16, 32x32, 64x64).  
+## Features
+- [x] Login
+- [x] Decode Divoom's animation formats to GIFs (16x16, 32x32, 64x64).  
+- [x] Get animation by ID
+- [x] Get animations by Category
+- [x] Get animations by Album
+- [ ] Get animations by User
+- [ ] Search animations & users
+- [ ] Like/Dislike animation
+- [ ] Comment on animation
+- [ ] Upload animations
 
 ## Install
 ```
 pip install APIxoo
 ```
 
 ## Example
```

### Comparing `APIxoo-0.2.0/apixoo/__init__.py` & `APIxoo-0.3.0/apixoo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import hashlib
+from typing import Union
 
 import requests
 
 from .const import (
     AlbumInfo,
     ApiEndpoint,
     GalleryCategory,
@@ -113,15 +114,15 @@
             resp_json['GalleryId'] = gallery_id
             return GalleryInfo(resp_json)
         except Exception:
             return None
 
     def get_category_files(
         self,
-        category: int | GalleryCategory,
+        category: Union[int, GalleryCategory],
         dimension: GalleryDimension = GalleryDimension.W32H32,
         sort: GallerySorting = GallerySorting.MOST_LIKED,
         file_type: GalleryType = GalleryType.ALL,
         page: int = 1,
         per_page: int = 20,
     ) -> list:
         """Get a list of galleries by Category"""
```

### Comparing `APIxoo-0.2.0/apixoo/const.py` & `APIxoo-0.3.0/apixoo/const.py`

 * *Files identical despite different names*

### Comparing `APIxoo-0.2.0/apixoo/pixel_bean.py` & `APIxoo-0.3.0/apixoo/pixel_bean.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 from PIL import Image
 
 
 class PixelBean(object):
     @property
     def total_frames(self):
         return self._total_frames
@@ -22,14 +24,22 @@
     def palettes(self):
         return self._palettes
 
     @property
     def frames_data(self):
         return self._frames_data
 
+    @property
+    def width(self):
+        return self._width
+
+    @property
+    def height(self):
+        return self._height
+
     def __init__(
         self,
         total_frames: int,
         speed: int,
         row_count: int,
         column_count: int,
         palettes: list,
@@ -38,50 +48,97 @@
         self._total_frames = total_frames
         self._speed = speed
         self._row_count = row_count
         self._column_count = column_count
         self._palettes = palettes
         self._frames_data = frames_data
 
+        self._width = column_count * 16
+        self._height = row_count * 16
+
+    def _resize(
+        self,
+        img: Image,
+        scale: Union[int, float] = 1,
+        target_width: int = None,
+        target_height: int = None,
+    ) -> Image:
+        """Resize frame image"""
+        # Default params -> don't do anything
+        if scale == 1 and not target_width and not target_height:
+            return img
+
+        org_width = img.width
+        org_height = img.height
+
+        width = img.width
+        height = img.height
+
+        if scale != 1:
+            width = round(width * scale)
+            height = round(height * scale)
+        elif target_width or target_height:
+            # Set specific width/height
+            if target_width and target_height:
+                width = target_width
+                height = target_height
+            elif target_width and not target_height:
+                width = target_width
+                height = round((target_width * org_height) / org_width)
+            elif target_height and not target_width:
+                width = round((target_height * org_width) / org_height)
+                height = target_height
+
+        # Resize image if needed
+        if width != org_width or height != org_height:
+            img = img.resize((width, height), Image.NEAREST)
+
+        return img
+
+    def get_frame_image(
+        self,
+        frame_number: int,
+        scale: Union[int, float] = 1,
+        target_width: int = None,
+        target_height: int = None,
+    ) -> Image:
+        """Get Pillow Image of a frame"""
+        if frame_number <= 0 or frame_number > self.total_frames:
+            raise Exception('Frame number out of range!')
+
+        frame_data = self._frames_data[frame_number - 1]
+        img = Image.new('RGB', (self._width, self._height))
+        for y in range(self._row_count * 16):
+            for x in range(self.column_count * 16):
+                palette_index = frame_data[y][x]
+                rgb = self._palettes[palette_index]
+                img.putpixel((x, y), rgb)
+
+        img = self._resize(
+            img, scale=scale, target_width=target_width, target_height=target_height
+        )
+        return img
+
     def save_to_gif(
         self,
         output_path: str,
-        scale: int | float = 1,
-        width: int = None,
-        height: int = None,
+        scale: Union[int, float] = 1,
+        target_width: int = None,
+        target_height: int = None,
     ) -> None:
         """Convert animation to GIF file"""
         gif_frames = []
 
-        org_width = self._column_count * 16
-        org_height = self._row_count * 16
-
-        for _, frame_data in enumerate(self._frames_data):
-            img = Image.new('RGBA', (org_width, org_height))
-            for y in range(self._row_count * 16):
-                for x in range(self.column_count * 16):
-                    palette_index = frame_data[y][x]
-                    rgb = self._palettes[palette_index]
-                    img.putpixel((x, y), rgb)
-
-            # Scale image
-            if scale != 1:
-                width = round(img.width * scale)
-                height = round(img.height * scale)
-            else:
-                # Set specific width/height
-                if width and not height:
-                    height = round((width * org_height) / org_width)
-                elif height and not width:
-                    width = round((height * org_width) / org_height)
-
-            # Resize image if needed
-            if width != org_width and height != org_height:
-                img = img.resize((width, height), Image.NEAREST)
-
+        for frame_number in range(self._total_frames):
+            img = self.get_frame_image(
+                frame_number,
+                scale=scale,
+                target_width=target_width,
+                target_height=target_height,
+            )
             gif_frames.append(img)
 
         # Save to GIF
         gif_frames[0].save(
             output_path,
             append_images=gif_frames[1:],
             duration=self._speed,
```

### Comparing `APIxoo-0.2.0/apixoo/pixel_bean_decoder.py` & `APIxoo-0.3.0/apixoo/pixel_bean_decoder.py`

 * *Files identical despite different names*

### Comparing `APIxoo-0.2.0/setup.py` & `APIxoo-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 long_desc = open("README.md").read()
 required = ['requests']
 
 setup(
     name='APIxoo',
-    version="0.2.0",
+    version="0.3.0",
     author="redphx",
     license="MIT",
     url="https://github.com/redphx/apixoo",
     download_url="https://github.com/redphx/apixoo",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     description="Python wrapper for Divoom Pixoo server API",
```

