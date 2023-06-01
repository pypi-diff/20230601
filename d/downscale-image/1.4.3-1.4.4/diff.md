# Comparing `tmp/downscale_image-1.4.3.tar.gz` & `tmp/downscale_image-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "downscale_image-1.4.3.tar", max compression
+gzip compressed data, was "downscale_image-1.4.4.tar", max compression
```

## Comparing `downscale_image-1.4.3.tar` & `downscale_image-1.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3244 2023-06-01 00:51:13.386923 downscale_image-1.4.3/downscale_image/__init__.py
--rw-r--r--   0        0        0     4277 2023-06-01 00:31:04.026787 downscale_image-1.4.3/downscale_image/__main__.py
--rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.3/downscale_image/_registry_utils.py
--rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.3/LICENSE
--rw-r--r--   0        0        0     1048 2023-06-01 00:20:26.238572 downscale_image-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.3/README.md
--rw-r--r--   0        0        0     1476 2023-06-01 00:53:01.081966 downscale_image-1.4.3/setup.py
--rw-r--r--   0        0        0     1325 2023-06-01 00:53:01.082964 downscale_image-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     3244 2023-06-01 00:51:13.386923 downscale_image-1.4.4/downscale_image/__init__.py
+-rw-r--r--   0        0        0     4582 2023-06-01 02:12:48.987919 downscale_image-1.4.4/downscale_image/__main__.py
+-rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.4/downscale_image/_registry_utils.py
+-rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.4/LICENSE
+-rw-r--r--   0        0        0     1048 2023-06-01 02:05:23.958953 downscale_image-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.4/README.md
+-rw-r--r--   0        0        0     1476 2023-06-01 02:15:14.401397 downscale_image-1.4.4/setup.py
+-rw-r--r--   0        0        0     1325 2023-06-01 02:15:14.402399 downscale_image-1.4.4/PKG-INFO
```

### Comparing `downscale_image-1.4.3/downscale_image/__init__.py` & `downscale_image-1.4.4/downscale_image/__init__.py`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.3/downscale_image/__main__.py` & `downscale_image-1.4.4/downscale_image/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 @click.option(
     "--add-to-right-click-menu",
     help="(Windows only) Register this program in right click menu for supported file types.",
     is_flag=True,
     default=False,
 )
 @click.option(
+    "--log-file",
+    help="File to log messages to.",
+    type=click.Path(path_type=pathlib.Path)
+)
+@click.option(
     "--continue-on-errors",
     help="Even if multiple errors are encountered keep going through all images",
     is_flag=True,
     default=False
 )
 @click.argument(
     "in_file",
@@ -68,17 +73,21 @@
     max_size,
     in_file: typing.Tuple[pathlib.Path],
     add_to_right_click_menu: bool,
     suffix: str,
     prefix: str,
     override_output_format: typing.Optional[str],
     continue_on_errors: bool,
+    log_file: typing.Optional[pathlib.Path],
 ):
     """Downscale file_or_directory to desired max-size."""
     logging.basicConfig(format="%(asctime)s %(levelname)s -- %(message)s", level=logging.WARNING)
+    if log_file:
+        root_logger = logging.getLogger()
+        root_logger.addHandler(logging.FileHandler(filename=str(log_file)))
     if add_to_right_click_menu:
         if not _ON_WINDOWS:
             raise Exception("Error, registry right click menus are only support on Windows.")
         exe = pathlib.Path(sys.argv[0])
         args = []
         _registry_utils.register_downscale_commands(str(exe), args)
```

### Comparing `downscale_image-1.4.3/downscale_image/_registry_utils.py` & `downscale_image-1.4.4/downscale_image/_registry_utils.py`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.3/LICENSE` & `downscale_image-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.3/pyproject.toml` & `downscale_image-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "downscale_image"
-version = "1.4.3"
+version = "1.4.4"
 description = "downscale image to desired file size"
 authors = ["mshafer1"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mshafer1/downscale_image"
 include = [
     "LICENSE",
```

### Comparing `downscale_image-1.4.3/README.md` & `downscale_image-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.3/setup.py` & `downscale_image-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.0', 'pathspec>=0.10.1,<0.11.0', 'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['downscale-image = downscale_image.__main__:main']}
 
 setup_kwargs = {
     'name': 'downscale-image',
-    'version': '1.4.3',
+    'version': '1.4.4',
     'description': 'downscale image to desired file size',
     'long_description': '# downscale_image\nA utility to downscale an image to the desired file size.\n\nRelies on an install of ffmpeg to incrementally downscale the image file into a new file.\n\nThis modules provides the script `downscale-image`\n\n```\n> downscale-image --help\nUsage: downscale-image [OPTIONS] FILE_OR_DIRECTORY\n\n  Downscale file_or_directory to desired max-size.\n\nOptions:\n  --max-size INTEGER RANGE   Max output size (in MB)  [default: 2; x>0]\n  --add-to-right-click-menu  (Windows only) Register this program in right\n                             click menu for supported file types.\n  --help                     Show this message and exit.\n\n```\n',
     'author': 'mshafer1',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mshafer1/downscale_image',
```

### Comparing `downscale_image-1.4.3/PKG-INFO` & `downscale_image-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: downscale-image
-Version: 1.4.3
+Version: 1.4.4
 Summary: downscale image to desired file size
 Home-page: https://github.com/mshafer1/downscale_image
 License: MIT
 Author: mshafer1
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

