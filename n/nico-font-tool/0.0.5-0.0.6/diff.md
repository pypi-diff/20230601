# Comparing `tmp/nico-font-tool-0.0.5.tar.gz` & `tmp/nico-font-tool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nico-font-tool-0.0.5.tar", last modified: Thu Jun  1 09:47:45 2023, max compression
+gzip compressed data, was "nico-font-tool-0.0.6.tar", last modified: Thu Jun  1 10:48:41 2023, max compression
```

## Comparing `nico-font-tool-0.0.5.tar` & `nico-font-tool-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.718335 nico-font-tool-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/src/nico_font_tool/
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/nicofont.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/src/nico_font_tool/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 09:47:45.000000 nico-font-tool-0.0.5/src/nico_font_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:47:45.722335 nico-font-tool-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 09:47:34.000000 nico-font-tool-0.0.5/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:41.857164 nico-font-tool-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-01 10:48:41.857164 nico-font-tool-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 10:48:41.857164 nico-font-tool-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:41.853164 nico-font-tool-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:41.857164 nico-font-tool-0.0.6/src/nico_font_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/src/nico_font_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/src/nico_font_tool/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/src/nico_font_tool/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/src/nico_font_tool/nicofont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/src/nico_font_tool/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:41.857164 nico-font-tool-0.0.6/src/nico_font_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-01 10:48:41.000000 nico-font-tool-0.0.6/src/nico_font_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-01 10:48:41.000000 nico-font-tool-0.0.6/src/nico_font_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:48:41.000000 nico-font-tool-0.0.6/src/nico_font_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 10:48:41.000000 nico-font-tool-0.0.6/src/nico_font_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 10:48:41.000000 nico-font-tool-0.0.6/src/nico_font_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 10:48:41.000000 nico-font-tool-0.0.6/src/nico_font_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:41.857164 nico-font-tool-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 10:48:30.000000 nico-font-tool-0.0.6/tests/test_.py
```

### Comparing `nico-font-tool-0.0.5/LICENSE` & `nico-font-tool-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.5/PKG-INFO` & `nico-font-tool-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nico-font-tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for converting fonts to NICO Game Framework format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: source, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: issues, https://github.com/TakWolf/nico-font-tool.python/issues
```

### Comparing `nico-font-tool-0.0.5/README.md` & `nico-font-tool-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.5/pyproject.toml` & `nico-font-tool-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nico-font-tool"
-version = "0.0.5"
+version = "0.0.6"
 description = "A tool for converting fonts to NICO Game Framework format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
@@ -15,19 +15,19 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "fonttools==4.39.4",
-    "Brotli==1.0.9",
-    "bdffont==0.0.10",
-    "Pillow==9.5.0",
-    "pypng==0.20220715.0",
+    "fonttools>=4.39.4",
+    "Brotli>=1.0.9",
+    "bdffont>=0.0.10",
+    "Pillow>=9.5.0",
+    "pypng>=0.20220715.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/nico-font-tool.python"
 source = "https://github.com/TakWolf/nico-font-tool.python"
 issues = "https://github.com/TakWolf/nico-font-tool.python/issues"
```

### Comparing `nico-font-tool-0.0.5/src/nico_font_tool/__init__.py` & `nico-font-tool-0.0.6/src/nico_font_tool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,28 +72,28 @@
 
     return sheet_data, alphabet
 
 
 def save_palette_png(
         sheet_data: list[list[int]],
         outputs_dir: str | bytes | os.PathLike[str] | os.PathLike[bytes],
-        outputs_name: str,
+        outputs_name: str | bytes,
 ):
     palette = [(255, 255, 255), (0, 0, 0), (255, 0, 255)]
     writer = png.Writer(len(sheet_data[0]), len(sheet_data), palette=palette)
     png_file_path = os.path.join(outputs_dir, f'{outputs_name}.png')
     with open(png_file_path, 'wb') as file:
         writer.write(file, sheet_data)
     logger.info(f"Make: '{png_file_path}'")
 
 
 def save_rgba_png(
         sheet_data: list[list[int]],
         outputs_dir: str | bytes | os.PathLike[str] | os.PathLike[bytes],
-        outputs_name: str,
+        outputs_name: str | bytes,
 ):
     rgba_bitmap = []
     for sheet_data_row in sheet_data:
         rgba_bitmap_row = []
         for color in sheet_data_row:
             if color == _GLYPH_DATA_TRANSPARENT:
                 rgba_bitmap_row.append(0)
@@ -116,13 +116,13 @@
     image.save(png_file_path)
     logger.info(f"Make: '{png_file_path}'")
 
 
 def save_dat_file(
         alphabet: list[str],
         outputs_dir: str | bytes | os.PathLike[str] | os.PathLike[bytes],
-        outputs_name: str,
+        outputs_name: str | bytes,
 ):
     dat_file_path = os.path.join(outputs_dir, f'{outputs_name}.png.dat')
     with open(dat_file_path, 'w', encoding='utf-8') as file:
         file.write(''.join(alphabet))
     logger.info(f"Make: '{dat_file_path}'")
```

### Comparing `nico-font-tool-0.0.5/src/nico_font_tool/bdf.py` & `nico-font-tool-0.0.6/src/nico_font_tool/bdf.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.5/src/nico_font_tool/font.py` & `nico-font-tool-0.0.6/src/nico_font_tool/font.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.5/src/nico_font_tool/nicofont.py` & `nico-font-tool-0.0.6/src/nico_font_tool/nicofont.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 import nico_font_tool
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def execute(args: argparse.Namespace):
-    font_file_path = args.font_file_path
-    outputs_dir = args.outputs_dir
-    outputs_name = args.outputs_name
-    font_size = args.font_size
-    glyph_offset_x = args.glyph_offset_x
-    glyph_offset_y = args.glyph_offset_y
-    glyph_adjust_width = args.glyph_adjust_width
-    glyph_adjust_height = args.glyph_adjust_height
-    mode = args.mode
+    font_file_path: str = args.font_file_path
+    outputs_dir: str = args.outputs_dir
+    outputs_name: str = args.outputs_name
+    font_size: int | None = args.font_size
+    glyph_offset_x: int = args.glyph_offset_x
+    glyph_offset_y: int = args.glyph_offset_y
+    glyph_adjust_width: int = args.glyph_adjust_width
+    glyph_adjust_height: int = args.glyph_adjust_height
+    mode: str = args.mode
 
     if mode != 'palette' and mode != 'rgba':
         raise Exception(f"Unsupported png mode: '{mode}'")
 
     if not os.path.exists(outputs_dir):
         os.makedirs(outputs_dir)
```

### Comparing `nico-font-tool-0.0.5/src/nico_font_tool/opentype.py` & `nico-font-tool-0.0.6/src/nico_font_tool/opentype.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.5/src/nico_font_tool.egg-info/PKG-INFO` & `nico-font-tool-0.0.6/src/nico_font_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nico-font-tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for converting fonts to NICO Game Framework format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: source, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: issues, https://github.com/TakWolf/nico-font-tool.python/issues
```

