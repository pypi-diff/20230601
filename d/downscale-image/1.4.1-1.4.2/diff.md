# Comparing `tmp/downscale_image-1.4.1.tar.gz` & `tmp/downscale_image-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "downscale_image-1.4.1.tar", max compression
+gzip compressed data, was "downscale_image-1.4.2.tar", max compression
```

## Comparing `downscale_image-1.4.1.tar` & `downscale_image-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2365 2023-05-31 02:53:51.764840 downscale_image-1.4.1/downscale_image/__init__.py
--rw-r--r--   0        0        0     3646 2023-05-31 02:35:59.492199 downscale_image-1.4.1/downscale_image/__main__.py
--rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.1/downscale_image/_registry_utils.py
--rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.1/LICENSE
--rw-r--r--   0        0        0     1030 2023-05-31 02:56:32.494086 downscale_image-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.1/README.md
--rw-r--r--   0        0        0     1453 2023-05-31 02:57:14.575802 downscale_image-1.4.1/setup.py
--rw-r--r--   0        0        0     1287 2023-05-31 02:57:14.576991 downscale_image-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2519 2023-05-31 23:42:09.603504 downscale_image-1.4.2/downscale_image/__init__.py
+-rw-r--r--   0        0        0     4164 2023-05-31 23:43:16.623726 downscale_image-1.4.2/downscale_image/__main__.py
+-rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.2/downscale_image/_registry_utils.py
+-rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1048 2023-05-31 23:42:52.419776 downscale_image-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.2/README.md
+-rw-r--r--   0        0        0     1476 2023-05-31 23:45:05.115723 downscale_image-1.4.2/setup.py
+-rw-r--r--   0        0        0     1325 2023-05-31 23:45:05.116722 downscale_image-1.4.2/PKG-INFO
```

### Comparing `downscale_image-1.4.1/downscale_image/__init__.py` & `downscale_image-1.4.2/downscale_image/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Utility to downscale an image to the desired file size using ffmpeg."""
 import os.path
 import pathlib
 import shutil
 import subprocess
 import sys
 import typing
+import logging
 
 SUPPORTED_FILE_EXTENSIONS = [".jpg", ".jpeg", ".png", ".bmp"]
 
+_MODULE_LOGGER = logging.getLogger(__name__)
+_MODULE_LOGGER.addHandler(logging.NullHandler())
 
 def _bytes_to_mega_bytes(bytes: int) -> float:
     return bytes / 1024 / 1024
 
 
 def _get_file_size_in_mega(file: pathlib.Path) -> float:
     file_size = os.path.getsize(file)
@@ -22,16 +25,16 @@
     """Use ffmpeg to scale the image by the desired amount."""
     as_divisor = 1 / scale
     try:
         output = subprocess.check_output(
             f'ffmpeg -i "{img}" -vf scale="iw/{as_divisor:.2f}:-1" "{out_img}"',
             stderr=subprocess.STDOUT,
         )
-    except subprocess.CalledProcessError:
-        print(output, file=sys.stderr)
+    except subprocess.CalledProcessError as e:
+        _MODULE_LOGGER.warning("Failed to process %s:\n %s", img, e.output)
         raise
     except FileNotFoundError:
         print(
             "Error, Could not find ffmpeg to execute. Make sure it is on the PATH variable.",
             file=sys.stderr,
         )
         raise
```

### Comparing `downscale_image-1.4.1/downscale_image/__main__.py` & `downscale_image-1.4.2/downscale_image/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Downscale an image to desired file size."""
+import logging
 import pathlib
 import platform
 import sys
 import typing
 
 import click
 import pathspec
+import tqdm
+import tqdm.contrib.logging
 
 import downscale_image
 
 _ON_WINDOWS = platform.system().lower() == "windows"
+_MODULE_LOGGER = logging.getLogger(__name__)
 
 if _ON_WINDOWS:
     from downscale_image import _registry_utils
 
 _DEFAULT_MATCHES = (
     ["!.venv/", "!.git/", "!objects/", "!.ts/*"]
     + [f"*{ext}" for ext in downscale_image.SUPPORTED_FILE_EXTENSIONS]
@@ -44,27 +48,34 @@
 )
 @click.option(
     "--add-to-right-click-menu",
     help="(Windows only) Register this program in right click menu for supported file types.",
     is_flag=True,
     default=False,
 )
+@click.option(
+    "--continue-on-errors",
+    help="Even if multiple errors are encountered keep going through all images",
+    is_flag=True,
+    default=False
+)
 @click.argument(
     "in_file",
     nargs=-1,
     metavar="FILE_OR_DIRECTORY",
     type=click.Path(exists=True, dir_okay=True, path_type=pathlib.Path),
 )
 def main(
     max_size,
     in_file: typing.Tuple[pathlib.Path],
     add_to_right_click_menu: bool,
     suffix: str,
     prefix: str,
     override_output_format: typing.Optional[str],
+    continue_on_errors: bool,
 ):
     """Downscale file_or_directory to desired max-size."""
     if add_to_right_click_menu:
         if not _ON_WINDOWS:
             raise Exception("Error, registry right click menus are only support on Windows.")
         exe = pathlib.Path(sys.argv[0])
         args = []
@@ -81,35 +92,36 @@
         else:
             files_to_prcoess.append(path)
 
     fail_count = 0
     last_error = None
     if not files_to_prcoess:
         print("Nothing to process.")
-    for file in files_to_prcoess:
-        try:
-            file = file.resolve().relative_to(_CWD)
-        except ValueError:
-            file = file.resolve()
-        print(f"Downscaling {file}...")
-        try:
-            output = downscale_image.downscale(
-                file, max_mega_bytes=max_size, output_prefix=prefix, outtput_suffix=suffix, override_output_format=override_output_format
-            )
-            print(f"Finished. Output stored in {output}\n\n")
-        except Exception as e:
-            fail_count += 1
-            if fail_count > 5:
-                print("Several errors have occured, stopping")
-                break
-            print("An error occured", file=sys.stderr)
-            print(e, file=sys.stderr)
-            last_error = e
-            print("")
-            print("")
+    file: pathlib.Path
+    with tqdm.contrib.logging.logging_redirect_tqdm():
+        for file in tqdm.tqdm(files_to_prcoess, desc="Downscaling: "):
+            try:
+                file = file.resolve().relative_to(_CWD)
+            except ValueError:
+                file = file.resolve()
+            print(f"Downscaling {file}...")
+            try:
+                output = downscale_image.downscale(
+                    file, max_mega_bytes=max_size, output_prefix=prefix, outtput_suffix=suffix, override_output_format=override_output_format
+                )
+                print(f"Finished. Output stored in {output}\n\n")
+            except Exception as e:
+                _MODULE_LOGGER.warning("Failed to downscale (%s), error:\n%s\n\n", file, e)
+                fail_count += 1
+                if not continue_on_errors and fail_count > 5:
+                    print("Several errors have occured, stopping")
+                    break
+                last_error = e
+                print("")
+                print("")
     if last_error:
         print("See above for errors")
         input("Press enter to continue...")
         click.Abort(last_error)
 
 
 if __name__ == "__main__":  # pragma: no cover
```

### Comparing `downscale_image-1.4.1/downscale_image/_registry_utils.py` & `downscale_image-1.4.2/downscale_image/_registry_utils.py`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.1/LICENSE` & `downscale_image-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.1/pyproject.toml` & `downscale_image-1.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "downscale_image"
-version = "1.4.1"
+version = "1.4.2"
 description = "downscale image to desired file size"
 authors = ["mshafer1"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mshafer1/downscale_image"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=8.0"
 # TODO: consider adding static-ffmpeg (https://pypi.org/project/static-ffmpeg/) to remove system dep
 pathspec = "^0.10.1"
+tqdm = "^4.65.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.1"
 pytest-snapshot = ">=0.9.0"
 pytest-cov = ">=3.0"
 
 ni-python-styleguide = ">=0.1.10"
```

### Comparing `downscale_image-1.4.1/README.md` & `downscale_image-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.1/setup.py` & `downscale_image-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['downscale_image']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=8.0', 'pathspec>=0.10.1,<0.11.0']
+['click>=8.0', 'pathspec>=0.10.1,<0.11.0', 'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['downscale-image = downscale_image.__main__:main']}
 
 setup_kwargs = {
     'name': 'downscale-image',
-    'version': '1.4.1',
+    'version': '1.4.2',
     'description': 'downscale image to desired file size',
     'long_description': '# downscale_image\nA utility to downscale an image to the desired file size.\n\nRelies on an install of ffmpeg to incrementally downscale the image file into a new file.\n\nThis modules provides the script `downscale-image`\n\n```\n> downscale-image --help\nUsage: downscale-image [OPTIONS] FILE_OR_DIRECTORY\n\n  Downscale file_or_directory to desired max-size.\n\nOptions:\n  --max-size INTEGER RANGE   Max output size (in MB)  [default: 2; x>0]\n  --add-to-right-click-menu  (Windows only) Register this program in right\n                             click menu for supported file types.\n  --help                     Show this message and exit.\n\n```\n',
     'author': 'mshafer1',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mshafer1/downscale_image',
```

### Comparing `downscale_image-1.4.1/PKG-INFO` & `downscale_image-1.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: downscale-image
-Version: 1.4.1
+Version: 1.4.2
 Summary: downscale image to desired file size
 Home-page: https://github.com/mshafer1/downscale_image
 License: MIT
 Author: mshafer1
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.0)
 Requires-Dist: pathspec (>=0.10.1,<0.11.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/mshafer1/downscale_image
 Description-Content-Type: text/markdown
 
 # downscale_image
 A utility to downscale an image to the desired file size.
 
 Relies on an install of ffmpeg to incrementally downscale the image file into a new file.
```

