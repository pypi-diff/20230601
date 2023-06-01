# Comparing `tmp/downscale_image-1.4.2.tar.gz` & `tmp/downscale_image-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "downscale_image-1.4.2.tar", max compression
+gzip compressed data, was "downscale_image-1.4.3.tar", max compression
```

## Comparing `downscale_image-1.4.2.tar` & `downscale_image-1.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2519 2023-05-31 23:42:09.603504 downscale_image-1.4.2/downscale_image/__init__.py
--rw-r--r--   0        0        0     4164 2023-05-31 23:43:16.623726 downscale_image-1.4.2/downscale_image/__main__.py
--rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.2/downscale_image/_registry_utils.py
--rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.2/LICENSE
--rw-r--r--   0        0        0     1048 2023-05-31 23:42:52.419776 downscale_image-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.2/README.md
--rw-r--r--   0        0        0     1476 2023-05-31 23:45:05.115723 downscale_image-1.4.2/setup.py
--rw-r--r--   0        0        0     1325 2023-05-31 23:45:05.116722 downscale_image-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3244 2023-06-01 00:51:13.386923 downscale_image-1.4.3/downscale_image/__init__.py
+-rw-r--r--   0        0        0     4277 2023-06-01 00:31:04.026787 downscale_image-1.4.3/downscale_image/__main__.py
+-rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.3/downscale_image/_registry_utils.py
+-rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.3/LICENSE
+-rw-r--r--   0        0        0     1048 2023-06-01 00:20:26.238572 downscale_image-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.3/README.md
+-rw-r--r--   0        0        0     1476 2023-06-01 00:53:01.081966 downscale_image-1.4.3/setup.py
+-rw-r--r--   0        0        0     1325 2023-06-01 00:53:01.082964 downscale_image-1.4.3/PKG-INFO
```

### Comparing `downscale_image-1.4.2/downscale_image/__init__.py` & `downscale_image-1.4.3/downscale_image/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility to downscale an image to the desired file size using ffmpeg."""
+import os
 import os.path
 import pathlib
 import shutil
 import subprocess
 import sys
 import typing
 import logging
@@ -16,14 +17,32 @@
     return bytes / 1024 / 1024
 
 
 def _get_file_size_in_mega(file: pathlib.Path) -> float:
     file_size = os.path.getsize(file)
     return _bytes_to_mega_bytes(file_size)
 
+def _decrements():
+    """
+    >>> t = _decrements(); list([next(t) for _ in range(15)])
+    [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.09, 0.08, 0.07, 0.06, 0.05]
+
+    >>> t = _decrements(); _ = [next(t) for _ in range(15)]; list([next(t) for _ in range(10)])
+    [0.04, 0.03, 0.02, 0.01, 0.009, 0.008, 0.007, 0.006, 0.005, 0.004]
+    """
+    step_size = 1
+    current_value = 1.0
+    yield current_value
+    while True: # iterate forever
+        step = 10**(-step_size)
+        if current_value - step <= 0:
+            step_size += 1
+            step = 10**(-step_size)
+        current_value = round(current_value- step, step_size)
+        yield round(current_value, 3)
 
 def _scale(img: pathlib.Path, out_img: pathlib.Path, scale: float) -> pathlib.Path:
     """Use ffmpeg to scale the image by the desired amount."""
     as_divisor = 1 / scale
     try:
         output = subprocess.check_output(
             f'ffmpeg -i "{img}" -vf scale="iw/{as_divisor:.2f}:-1" "{out_img}"',
@@ -38,37 +57,38 @@
             file=sys.stderr,
         )
         raise
     return out_img
 
 
 def downscale(
-    img: pathlib.Path, max_mega_bytes: float, *_, output_prefix="", outtput_suffix="_smaller", override_output_format: typing.Optional[str]=None
+    img: pathlib.Path, max_mega_bytes: float, *_, output_prefix="", output_suffix="_smaller", override_output_format: typing.Optional[str]=None
 ) -> pathlib.Path:
     """Incrementally downscale img until it is <= max_mega_bytes in size."""
     current_size = _get_file_size_in_mega(img)
     working_img = img
-    current_scale = 1.0
-    current_multiplier = 10
+    scales = _decrements()
+    current_scale = next(scales)
 
     if current_size <= max_mega_bytes:
         print("Not changing")
         return img
 
     out_suffix = f".{override_output_format}" if override_output_format else ".".join(img.suffixes)
-    working_img = img.parent / (output_prefix + img.stem + outtput_suffix + out_suffix)
+    working_img = img.parent / (output_prefix + img.stem + output_suffix + out_suffix)
     working_img.parent.mkdir(exist_ok=True, parents=True)
-    shutil.copyfile(img, working_img)
+    try:
+        shutil.copyfile(img, working_img)
+    except:
+        os.chmod(working_img, 0o777) # read and write by everyone
+        shutil.copyfile(img, working_img)
 
     while current_size > max_mega_bytes:
         if working_img.is_file():
             working_img.unlink()
 
         working_img = _scale(img, out_img=working_img, scale=current_scale)
 
         current_size = _get_file_size_in_mega(working_img)
-        current_scale -= 1 / current_multiplier
-        if current_scale < 0:
-            current_scale = 1/current_multiplier
-            current_multiplier += 10
+        current_scale = next(scales)
 
     return working_img
```

### Comparing `downscale_image-1.4.2/downscale_image/__main__.py` & `downscale_image-1.4.3/downscale_image/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     add_to_right_click_menu: bool,
     suffix: str,
     prefix: str,
     override_output_format: typing.Optional[str],
     continue_on_errors: bool,
 ):
     """Downscale file_or_directory to desired max-size."""
+    logging.basicConfig(format="%(asctime)s %(levelname)s -- %(message)s", level=logging.WARNING)
     if add_to_right_click_menu:
         if not _ON_WINDOWS:
             raise Exception("Error, registry right click menus are only support on Windows.")
         exe = pathlib.Path(sys.argv[0])
         args = []
         _registry_utils.register_downscale_commands(str(exe), args)
 
@@ -91,28 +92,28 @@
             files_to_prcoess.extend([path / p for p in spec.match_tree(path)])
         else:
             files_to_prcoess.append(path)
 
     fail_count = 0
     last_error = None
     if not files_to_prcoess:
-        print("Nothing to process.")
+        _MODULE_LOGGER.warning("Nothing to process.")
     file: pathlib.Path
     with tqdm.contrib.logging.logging_redirect_tqdm():
         for file in tqdm.tqdm(files_to_prcoess, desc="Downscaling: "):
             try:
                 file = file.resolve().relative_to(_CWD)
             except ValueError:
                 file = file.resolve()
             print(f"Downscaling {file}...")
             try:
                 output = downscale_image.downscale(
-                    file, max_mega_bytes=max_size, output_prefix=prefix, outtput_suffix=suffix, override_output_format=override_output_format
+                    file, max_mega_bytes=max_size, output_prefix=prefix, output_suffix=suffix, override_output_format=override_output_format
                 )
-                print(f"Finished. Output stored in {output}\n\n")
+                print(f"Finished. Output stored in {output}\n")
             except Exception as e:
                 _MODULE_LOGGER.warning("Failed to downscale (%s), error:\n%s\n\n", file, e)
                 fail_count += 1
                 if not continue_on_errors and fail_count > 5:
                     print("Several errors have occured, stopping")
                     break
                 last_error = e
```

### Comparing `downscale_image-1.4.2/downscale_image/_registry_utils.py` & `downscale_image-1.4.3/downscale_image/_registry_utils.py`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.2/LICENSE` & `downscale_image-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.2/pyproject.toml` & `downscale_image-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "downscale_image"
-version = "1.4.2"
+version = "1.4.3"
 description = "downscale image to desired file size"
 authors = ["mshafer1"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mshafer1/downscale_image"
 include = [
     "LICENSE",
```

### Comparing `downscale_image-1.4.2/README.md` & `downscale_image-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.2/setup.py` & `downscale_image-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.0', 'pathspec>=0.10.1,<0.11.0', 'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['downscale-image = downscale_image.__main__:main']}
 
 setup_kwargs = {
     'name': 'downscale-image',
-    'version': '1.4.2',
+    'version': '1.4.3',
     'description': 'downscale image to desired file size',
     'long_description': '# downscale_image\nA utility to downscale an image to the desired file size.\n\nRelies on an install of ffmpeg to incrementally downscale the image file into a new file.\n\nThis modules provides the script `downscale-image`\n\n```\n> downscale-image --help\nUsage: downscale-image [OPTIONS] FILE_OR_DIRECTORY\n\n  Downscale file_or_directory to desired max-size.\n\nOptions:\n  --max-size INTEGER RANGE   Max output size (in MB)  [default: 2; x>0]\n  --add-to-right-click-menu  (Windows only) Register this program in right\n                             click menu for supported file types.\n  --help                     Show this message and exit.\n\n```\n',
     'author': 'mshafer1',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mshafer1/downscale_image',
```

### Comparing `downscale_image-1.4.2/PKG-INFO` & `downscale_image-1.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: downscale-image
-Version: 1.4.2
+Version: 1.4.3
 Summary: downscale image to desired file size
 Home-page: https://github.com/mshafer1/downscale_image
 License: MIT
 Author: mshafer1
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

