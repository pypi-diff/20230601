# Comparing `tmp/nico-font-tool-0.0.4.tar.gz` & `tmp/nico-font-tool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nico-font-tool-0.0.4.tar", last modified: Fri May 26 07:39:47 2023, max compression
+gzip compressed data, was "nico-font-tool-0.0.5.tar", last modified: Thu Jun  1 09:47:45 2023, max compression
```

## Comparing `nico-font-tool-0.0.4.tar` & `nico-font-tool-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.676383 nico-font-tool-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-26 07:39:47.676383 nico-font-tool-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:39:47.676383 nico-font-tool-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.672383 nico-font-tool-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.672383 nico-font-tool-0.0.4/src/nico_font_tool/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/nicofont.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.672383 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.672383 nico-font-tool-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.718335 nico-font-tool-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/src/nico_font_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/nicofont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/tests/test_.py
```

### Comparing `nico-font-tool-0.0.4/LICENSE` & `nico-font-tool-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.4/PKG-INFO` & `nico-font-tool-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: nico-font-tool
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for converting fonts to NICO Game Framework format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: source, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: issues, https://github.com/TakWolf/nico-font-tool.python/issues
 Keywords: nico,game-engine,font
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NICO Font Tool - Python
 
+[![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/nico-font-tool)](https://pypi.org/project/nico-font-tool/)
 
 A tool for converting fonts to [NICO Game Framework](https://github.com/ftsf/nico) format fonts.
 
 This is the Python version. The Nim version see: [nico-font-tool](https://github.com/TakWolf/nico-font-tool).
 
 ## Installation
```

### Comparing `nico-font-tool-0.0.4/README.md` & `nico-font-tool-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # NICO Font Tool - Python
 
+[![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/nico-font-tool)](https://pypi.org/project/nico-font-tool/)
 
 A tool for converting fonts to [NICO Game Framework](https://github.com/ftsf/nico) format fonts.
 
 This is the Python version. The Nim version see: [nico-font-tool](https://github.com/TakWolf/nico-font-tool).
 
 ## Installation
```

### Comparing `nico-font-tool-0.0.4/pyproject.toml` & `nico-font-tool-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [project]
 name = "nico-font-tool"
-version = "0.0.4"
+version = "0.0.5"
 description = "A tool for converting fonts to NICO Game Framework format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
 maintainers = [
     { name = "TakWolf" },
 ]
 keywords = ["nico", "game-engine", "font"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "fonttools==4.39.3",
+    "fonttools==4.39.4",
     "Brotli==1.0.9",
-    "bdffont==0.0.7",
+    "bdffont==0.0.10",
     "Pillow==9.5.0",
     "pypng==0.20220715.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/nico-font-tool.python"
 source = "https://github.com/TakWolf/nico-font-tool.python"
```

### Comparing `nico-font-tool-0.0.4/src/nico_font_tool/__init__.py` & `nico-font-tool-0.0.5/src/nico_font_tool/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 
 from nico_font_tool.bdf import BdfRasterizer
 from nico_font_tool.font import FontRasterizer
 from nico_font_tool.opentype import OpenTypeRasterizer
 
 logger = logging.getLogger('nico-font-tool')
 
-_glyph_data_transparent = 0
-_glyph_data_solid = 1
-_glyph_data_border = 2
+_GLYPH_DATA_TRANSPARENT = 0
+_GLYPH_DATA_SOLID = 1
+_GLYPH_DATA_BORDER = 2
 
 
 def create_sheet(
         font_file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
         font_size: int = None,
         glyph_offset_x: int = 0,
         glyph_offset_y: int = 0,
         glyph_adjust_width: int = 0,
         glyph_adjust_height: int = 0,
 ) -> tuple[list[list[int]], list[str]]:
-    # 根据扩展名加载字体光栅器
     font_rasterizer: FontRasterizer
     font_ext = os.path.splitext(font_file_path)[1]
     if font_ext == '.otf' or font_ext == '.ttf' or font_ext == '.woff' or font_ext == '.woff2':
         if font_size is None:
             raise Exception('OpenType need a font size')
         font_rasterizer = OpenTypeRasterizer(
             font_file_path,
@@ -44,42 +43,35 @@
             glyph_adjust_width,
             glyph_adjust_height,
         )
     else:
         raise Exception(f'Font file type not supported: {font_ext}')
     logger.info(f"Loaded font file: '{font_file_path}'")
 
-    # 图集对象，初始化左边界
-    sheet_data = [[_glyph_data_border] for _ in range(font_rasterizer.adjusted_line_height)]
-
-    # 字母表
+    sheet_data = [[_GLYPH_DATA_BORDER] for _ in range(font_rasterizer.adjusted_line_height)]
     alphabet = []
 
-    # 遍历字体全部字符
     for code_point in font_rasterizer.get_code_point_sequence():
         c = chr(code_point)
         if not c.isprintable():
             continue
 
-        # 栅格化
         glyph_data, adjusted_advance_width = font_rasterizer.rasterize_glyph(code_point)
         if glyph_data is None:
             continue
         logger.info(f'Rasterize glyph: {code_point} - {c} - {adjusted_advance_width}')
 
-        # 合并到图集
         for y in range(font_rasterizer.adjusted_line_height):
             for x in range(adjusted_advance_width):
                 if glyph_data[y][x] > 0:
-                    sheet_data[y].append(_glyph_data_solid)
+                    sheet_data[y].append(_GLYPH_DATA_SOLID)
                 else:
-                    sheet_data[y].append(_glyph_data_transparent)
-            sheet_data[y].append(_glyph_data_border)
+                    sheet_data[y].append(_GLYPH_DATA_TRANSPARENT)
+            sheet_data[y].append(_GLYPH_DATA_BORDER)
 
-        # 添加到字母表
         alphabet.append(c)
 
     return sheet_data, alphabet
 
 
 def save_palette_png(
         sheet_data: list[list[int]],
@@ -99,20 +91,20 @@
         outputs_dir: str | bytes | os.PathLike[str] | os.PathLike[bytes],
         outputs_name: str,
 ):
     rgba_bitmap = []
     for sheet_data_row in sheet_data:
         rgba_bitmap_row = []
         for color in sheet_data_row:
-            if color == _glyph_data_transparent:
+            if color == _GLYPH_DATA_TRANSPARENT:
                 rgba_bitmap_row.append(0)
                 rgba_bitmap_row.append(0)
                 rgba_bitmap_row.append(0)
                 rgba_bitmap_row.append(0)
-            elif color == _glyph_data_solid:
+            elif color == _GLYPH_DATA_SOLID:
                 rgba_bitmap_row.append(0)
                 rgba_bitmap_row.append(0)
                 rgba_bitmap_row.append(0)
                 rgba_bitmap_row.append(255)
             else:
                 rgba_bitmap_row.append(255)
                 rgba_bitmap_row.append(0)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nico-font-tool-0.0.4/src/nico_font_tool/bdf.py` & `nico-font-tool-0.0.5/src/nico_font_tool/bdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 import os
 
-import bdffont
+from bdffont import BdfFont
 
 from nico_font_tool.font import FontRasterizer
 
 
 class BdfRasterizer(FontRasterizer):
     def __init__(
             self,
             font_file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
             glyph_offset_x: int = 0,
             glyph_offset_y: int = 0,
             glyph_adjust_width: int = 0,
             glyph_adjust_height: int = 0,
     ):
-        self.font = bdffont.load_bdf(font_file_path)
+        self.font = BdfFont.load(font_file_path)
 
         ascent = self.font.properties.font_ascent
-        if ascent is None:
-            ascent = self.font.bounding_box_height + self.font.bounding_box_offset_y
         descent = -self.font.properties.font_descent
-        if descent is None:
-            descent = self.font.bounding_box_offset_y
+        if ascent is None or descent is None:
+            max_top = 0
+            min_bottom = 0
+            for glyph in self.font.code_point_to_glyph.values():
+                (_, bounding_box_height), (_, bounding_box_offset_y), _ = glyph.get_8bit_aligned_bitmap(optimize_bitmap=True)
+                top = bounding_box_height + bounding_box_offset_y
+                if top > max_top:
+                    max_top = top
+                bottom = bounding_box_offset_y
+                if bottom < min_bottom:
+                    min_bottom = bottom
+            if ascent is None:
+                ascent = max_top
+            if descent is None:
+                descent = min_bottom
 
         super().__init__(
             ascent,
             descent,
             glyph_offset_x,
             glyph_offset_y,
             glyph_adjust_width,
```

### Comparing `nico-font-tool-0.0.4/src/nico_font_tool/font.py` & `nico-font-tool-0.0.5/src/nico_font_tool/font.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.4/src/nico_font_tool/nicofont.py` & `nico-font-tool-0.0.5/src/nico_font_tool/nicofont.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.4/src/nico_font_tool/opentype.py` & `nico-font-tool-0.0.5/src/nico_font_tool/opentype.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.4/src/nico_font_tool.egg-info/PKG-INFO` & `nico-font-tool-0.0.5/src/nico_font_tool.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: nico-font-tool
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for converting fonts to NICO Game Framework format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: source, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: issues, https://github.com/TakWolf/nico-font-tool.python/issues
 Keywords: nico,game-engine,font
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NICO Font Tool - Python
 
+[![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/nico-font-tool)](https://pypi.org/project/nico-font-tool/)
 
 A tool for converting fonts to [NICO Game Framework](https://github.com/ftsf/nico) format fonts.
 
 This is the Python version. The Nim version see: [nico-font-tool](https://github.com/TakWolf/nico-font-tool).
 
 ## Installation
```

