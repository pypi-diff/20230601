# Comparing `tmp/CalSciPy-0.3.0.tar.gz` & `tmp/CalSciPy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.3.0.tar", last modified: Wed May 24 14:31:11 2023, max compression
+gzip compressed data, was "CalSciPy-0.3.1.tar", last modified: Thu Jun  1 21:02:50 2023, max compression
```

## Comparing `CalSciPy-0.3.0.tar` & `CalSciPy-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.846920 CalSciPy-0.3.0/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     4947 2023-05-24 14:31:11.844948 CalSciPy-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.3.0/README.md
--rw-rw-rw-   0        0        0     2303 2023-05-24 14:30:46.000000 CalSciPy-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 14:31:11.847954 CalSciPy-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.711637 CalSciPy-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.769629 CalSciPy-0.3.0/src/CalSciPy/
--rw-rw-rw-   0        0        0      368 2023-05-24 14:06:12.000000 CalSciPy-0.3.0/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-05-24 14:10:25.000000 CalSciPy-0.3.0/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3270 2023-05-24 14:25:43.000000 CalSciPy-0.3.0/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     9766 2023-05-24 14:18:29.000000 CalSciPy-0.3.0/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     4603 2023-05-24 14:11:21.000000 CalSciPy-0.3.0/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     8973 2023-05-24 14:26:47.000000 CalSciPy-0.3.0/src/CalSciPy/interactive_visuals.py
--rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.3.0/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     7557 2023-05-03 19:58:49.000000 CalSciPy-0.3.0/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.3.0/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0    10311 2023-05-24 14:19:33.000000 CalSciPy-0.3.0/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.3.0/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.794633 CalSciPy-0.3.0/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4947 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      376 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.3.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.839926 CalSciPy-0.3.0/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.3.0/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.3.0/tests/test_bruker.py
--rw-rw-rw-   0        0        0      492 2023-05-24 14:14:23.000000 CalSciPy-0.3.0/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.3.0/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.3.0/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.3.0/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.3.0/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.3.0/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.179371 CalSciPy-0.3.1/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     4947 2023-06-01 21:02:50.177378 CalSciPy-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.3.1/README.md
+-rw-rw-rw-   0        0        0     2303 2023-06-01 21:02:24.000000 CalSciPy-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 21:02:50.179371 CalSciPy-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.040372 CalSciPy-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.102371 CalSciPy-0.3.1/src/CalSciPy/
+-rw-rw-rw-   0        0        0      368 2023-05-24 14:06:12.000000 CalSciPy-0.3.1/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    10702 2023-06-01 20:59:59.000000 CalSciPy-0.3.1/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3270 2023-05-24 14:25:43.000000 CalSciPy-0.3.1/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0     9766 2023-05-24 14:18:29.000000 CalSciPy-0.3.1/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     4603 2023-05-24 14:11:21.000000 CalSciPy-0.3.1/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     8973 2023-05-24 14:26:47.000000 CalSciPy-0.3.1/src/CalSciPy/interactive_visuals.py
+-rw-rw-rw-   0        0        0    10046 2023-06-01 20:59:59.000000 CalSciPy-0.3.1/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     8876 2023-05-26 15:07:57.000000 CalSciPy-0.3.1/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.3.1/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0    10311 2023-05-24 14:19:33.000000 CalSciPy-0.3.1/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.3.1/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.127371 CalSciPy-0.3.1/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4947 2023-06-01 21:02:49.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-01 21:02:50.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 21:02:49.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      376 2023-06-01 21:02:49.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 21:02:49.000000 CalSciPy-0.3.1/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.3.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:02:50.171370 CalSciPy-0.3.1/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.3.1/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.3.1/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      492 2023-05-24 14:14:23.000000 CalSciPy-0.3.1/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.3.1/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.3.1/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.3.1/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.3.1/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.3.1/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.3.0/LICENSE` & `CalSciPy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/PKG-INFO` & `CalSciPy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.3.0/README.md` & `CalSciPy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/pyproject.toml` & `CalSciPy-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.3.0"
+version = "0.3.1"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
```

### Comparing `CalSciPy-0.3.0/src/CalSciPy/bruker.py` & `CalSciPy-0.3.1/src/CalSciPy/bruker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 from __future__ import annotations
 from typing import Tuple, Optional, Union, List, Any
-import numpy as np
+from operator import eq
 from pathlib import Path
+from itertools import product
+
+
+import numpy as np
 from prettytable import PrettyTable
 import cv2
 from PPVD.parsing import convert_permitted_types_to_required, find_num_unique_files_given_static_substring, \
     find_num_unique_files_containing_tag
 from tqdm import tqdm as tq
-from itertools import product
+
+
 from .misc import PatternMatching, calculate_frames_per_file, generate_blocks, generate_padded_filename
-from operator import eq
 from .io_tools import _load_single_tif, _save_single_tif
 
 
 """
-These functions have been incorporated into pyPrairieView and will be deprecated in the future
+These functions have been incorporated into pyPrairieView and will likely be deprecated in the future and/or 
+pyPrairieView will absorbed into CalSciPy
 """
 
 
-def generate_bruker_naming_convention(channel: int = 0, plane: int = 0, num_channels: int = 1, num_planes: int = 1) \
+def generate_bruker_naming_convention(channel: int, plane: int, num_channels: int = 1, num_planes: int = 1) \
         -> str:
     """
     Generates the expected bruker naming convention for images collected with an arbitrary number of cycles & channels
 
-    This function expects that the naming convention is {experiment_name}_Cycle00000_Ch0_000000.ome.tiff
-    where the channel is one-indexed. The 5-digit cycle id represents the frame if using multiplane imaging and
-    the 6-digit tag represents the plane. Otherwise, the 5-digit tag is static and the 6-digit tag represents the frame.
-    Channel and plane are *zero-indexed*.
+    This function expects that the naming convention is _Cycle00000_Ch0_000000.ome.tiff where the channel is
+    one-indexed. The 5-digit cycle id represents the frame if using multiplane imaging and the 6-digit tag represents
+    the plane. Otherwise, the 5-digit tag is static and the 6-digit tag represents the frame.
+
+    Please note that the parameters channel and plane are *zero-indexed*.
 
     :param channel: channel to produce name for
-    :type channel: int = 0
     :param plane: plane to produce name for
-    :type plane: int = 0
     :param num_channels: number of channels
-    :type num_channels: int = 1
     :param num_planes: number of planes
-    :type num_planes: int = 1
-    :return:
+    :returns: proper naming convention
     """
-    # if channel + 1 > num_channels:
-    #    raise AssertionError("Channel selection exceeds the amount of identified channels")
-    # if plane + 1 > num_planes:
-    #    raise AssertionError("Plane selection exceeds the amount of identified planes")
     if num_channels > 1:
         num_channels = 2
     if num_planes > 1:
         num_planes = 2
     with PatternMatching([num_channels, num_planes], [eq, eq]) as case:
         if case([1, 1]):
             return "*.ome.tif"
@@ -58,20 +56,19 @@
 
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def determine_imaging_content(folder: Union[str, Path]) -> Tuple[int, int, int, int, int]:  # noqa: C901
     """
     This function determines the number of channels and planes within a folder containing .tif files
     exported by Bruker's Prairieview software. It also determines the size of the images (frames, y-pixels, x-pixels).
-    It's a quick / fast alternative to parsing its respective xml. Dependent on the naming conventions of PrairieView.
+    It's a quick / fast alternative to parsing its respective xml. However, note that the function is dependent on the
+    naming conventions of PrairieView and will not work on arbitrary folders.
 
     :param folder: folder containing bruker imaging data
-    :type folder: str or pathlib.Path
     :returns: channels, planes, frames, height, width
-    :rtype: tuple[int, int, int, int, int]
     """
 
     _files = [_file for _file in folder.glob("*.tif") if _file.is_file()]
 
     def _extract_file_identifiers(str_to_split: str) -> list:
         return str_to_split.split("_")[-3:]
 
@@ -121,28 +118,24 @@
     # apparently * on a return is illegal for python 3.7  # noqa
 
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def load_bruker_tifs(folder: Union[str, Path],
                      channel: Optional[int] = None, plane: Optional[int] = None) -> Tuple[np.ndarray]:  # noqa: C901
     """
-    Load images collected and exported to .tif by Bruker's Prairieview software to a tuple of numpy arrays.
+    This function loads images collected and converted to .tif files by Bruker's Prairieview software.
     If multiple channels or multiple planes exist, each channel and plane combination is loaded to a separate
     numpy array. Identification of multiple channels / planes is dependent on :func:`determine_imaging_content`.
-    Images are loaded as unsigned 16-bit, though note that raw bruker files are natively 12 or 13-bit.
+    Images are loaded as unsigned 16-bit (:class:`numpy.uint16`), though note that raw bruker files are
+    natively 12 or 13-bit.
 
     :param folder: folder containing a sequence of single frame tiff files
-    :type folder: str or pathlib.Path
     :param channel: specific channel to load from dataset (zero-indexed)
-    :type channel: Optional[int] = None
     :param plane: specific plane to load from dataset (zero-indexed)
-    :type plane: Optional[int] = None
-    :return: All .tif files in the directory loaded to a tuple of numpy arrays
-        (frames, y-pixels, x-pixels, :class:`np.uint16`)
-    :rtype: tuple[numpy.ndarray]
+    :return: a tuple of numpy arrays (frames, y-pixels, x-pixels, :class:`numpy.uint16`)
      """
     num_channels, num_planes, num_frames, y, x = determine_imaging_content(folder)
     _pretty_print_image_description(num_channels, num_planes, num_frames, y, x)
 
     images = []
     if channel is None and plane is None:
         for channel_, plane_ in product(range(num_channels), range(num_planes)):
@@ -152,26 +145,21 @@
     return tuple(images)
 
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def repackage_bruker_tifs(input_folder: Union[str, Path], output_folder: Union[str, Path],
                           channel: int = 0, plane: int = 0) -> None:
     """
-    Repackages a folder containing .tif files exported by Bruker's Prairieview software into a sequence of <4 GB .tif
-    stacks. Channels are planes are **zero-indexed**.
+    This function repackages a folder containing .tif files exported by Bruker's Prairieview software into a sequence
+    of <4 GB .tif stacks. Note that parameters channel and plane are **zero-indexed**.
 
     :param input_folder: folder containing a sequence of single frame .tif files exported by Bruker's Prairieview
-    :type input_folder: str or pathlib.Path
     :param output_folder: empty folder where .tif stacks will be saved
-    :type output_folder: str or pathlib.Path
-    :param channel: optional input specifying channel
-    :type channel: int = 0
-    :param plane: optional input specifying plane
-    :type plane: int = 0
-    :rtype: None
+    :param channel: specify channel
+    :param plane: specify plane
     """
     num_channels, num_planes, num_frames, y, x = determine_imaging_content(input_folder)
     _pretty_print_image_description(num_channels, num_planes, num_frames, y, x)
 
     naming_convention = generate_bruker_naming_convention(channel, plane, num_channels, num_planes)
 
     files = list(input_folder.glob(naming_convention))
@@ -207,25 +195,19 @@
 
 def _load_bruker_tif_stack(input_folder: Path, channel: int, plane: int,
                            num_channels: int, num_planes: int) -> np.ndarray:
     """
     Implementation function to load a single bruker tif stack
 
     :param input_folder: folder containing tif stack
-    :type input_folder: pathlib.Path
     :param channel: selected channel to load
-    :type channel: int
     :param plane: selected plane to load
-    :type plane: int
     :param num_channels: total number of channels
-    :type num_channels: int
     :param num_planes: total number of planes
-    :type num_planes: int
-    :return: loaded images
-    :rtype: numpy.ndarray
+    :returns: loaded images
     """
     naming_convention = generate_bruker_naming_convention(channel, plane, num_channels, num_planes)
     files = list(input_folder.glob(naming_convention))
     pbar = tq(total=len(files))
     pbar.set_description("".join(["Loading Channel ", str(channel), " Plane ", str(plane)]))
     images = [_verbose_load_single_tif(file, pbar) for file in files]
     pbar.close()
```

### Comparing `CalSciPy-0.3.0/src/CalSciPy/coloring.py` & `CalSciPy-0.3.1/src/CalSciPy/coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/src/CalSciPy/event_processing.py` & `CalSciPy-0.3.1/src/CalSciPy/event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/src/CalSciPy/image_processing.py` & `CalSciPy-0.3.1/src/CalSciPy/image_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/src/CalSciPy/interactive_visuals.py` & `CalSciPy-0.3.1/src/CalSciPy/interactive_visuals.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/src/CalSciPy/io_tools.py` & `CalSciPy-0.3.1/src/CalSciPy/io_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 from __future__ import annotations
 from typing import Union, Optional
 from pathlib import Path
-import cv2
+from json import load, dump
+
+
 from PIL import Image
 import numpy as np
-from json import load, dump
+import cv2
 from PPVD.validation import validate_extension, validate_filename
 from PPVD.parsing import convert_permitted_types_to_required
+
+
 from .misc import generate_blocks, calculate_frames_per_file
 
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def load_binary(path: Union[str, Path], mapped: bool = False) -> Union[np.ndarray, np.memmap]:
+    """
+    This function loads images saved in language-agnostic binary format. Ideal for optimal read/write speeds and
+    highly-robust to corruption. However, the downside is that the images and their metadata are split into two
+    separate files. Images are saved with the *.bin* extension, while metadata is saved with extension *.json*.
+    If for some reason you lose the metadata, you can still load the binary if you know three of the following:
+    number of frames, y-pixels, x-pixels, and the datatype (:class:`numpy.dtype`)
+
+    :param path: folder containing binary file
+    :param mapped: boolean indicating whether to load image using memory-mapping
+    :returns: image (frames, y-pixels, x-pixels)
+    """
     if not path.is_file():
         path = path.joinpath("binary_video")
 
     # add extensions
     meta_filename = path.with_suffix(".json")
     imaging_filename = path.with_suffix(".bin")
 
@@ -31,44 +46,38 @@
 
 
 @validate_filename(pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def load_images(path: Union[str, Path]) -> np.ndarray:
     """
     Load images into a numpy array. If path is a folder, all .tif files found non-recursively in the directory will be
-    compiled to a single array
+    compiled to a single array.
 
     :param path: a file containing images or a folder containing several imaging stacks
-    :type path: str or pathlib.Path
     :return: numpy array (frames, y-pixels, x-pixels)
-    :rtype: numpy.ndarray
     """
     if path.is_file():
         return _load_single_tif(path)
     else:
         return _load_many_tif(path)
 
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def save_binary(path: Union[str, Path], images: np.ndarray) -> int:
     """
     Save images to language-agnostic binary format. Ideal for optimal read/write speeds and highly-robust to corruption.
     However, the downside is that the images and their metadata are split into two separate files. Images are saved with
     the *.bin* extension, while metadata is saved with extension *.json*. If for some reason you lose the metadata, you
     can still load the binary if you know three of the following: number of frames, y-pixels, x-pixels, and the
-    datatype. The datatype is almost always unsigned 16-bit for all modern imaging systems--even if they are collected
-    at 12 or 13-bit.
+    datatype. The datatype is almost always unsigned 16-bit (:class:`numpy.uint16`) for all modern imaging
+    systems--even if they are collected at 12 or 13-bit.
 
-    :param path: path to save images to. The path stem is considered the filename if it doesn't have any extension.
-    If no filename is provided then the default filename is *binary_video*.
-    :type path: str or pathlib.Path
+    :param path: path to save images to. The path stem is considered the filename if it doesn't have any extension. If no filename is provided then the default filename is *binary_video*.
     :param images: images to save (frames, y-pixels, x-pixels)
-    :type images: numpy.ndarray
-    :return: 0 if successful
-    :rtype: int
+    :returns: 0 if successful
     """
     # parse the desired path
     if path.is_file():
         name = Path.name
         file_path = Path(path.parents)
     else:
         name = "binary_video"
@@ -93,21 +102,17 @@
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def save_images(path: Union[str, Path], images: np.ndarray, size_cap: float = 3.9) -> int:
     """
     Save a numpy array to a single .tif file. If size > 4GB then saved as a series of files. If path is not a file and
     already exists the default filename will be *images*.
 
     :param path: filename or absolute path
-    :type path: str or pathlib.Path
     :param images: numpy array (frames, y pixels, x pixels)
-    :type images: numpy.ndarray
     :param size_cap: maximum size per file
-    :type size_cap: float = 3.9
-    :return: returns 0 if successful
-    :rtype: int
+    :returns: returns 0 if successful
     """
     # parse desired path
     if Path.exists(path):
         if path.is_file():
             name = path.name
             file_path = path.parent
         else:
@@ -149,17 +154,15 @@
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def _load_many_tif(folder: Union[str, Path]) -> np.ndarray:
     """
     Loads all .tif's within a folder into a single numpy array.
 
     :param folder: folder containing a sequence of tiff stacks
-    :type folder: str or pathlib.Path
-    :return: a numpy array containing the images (frames, y-pixels, x-pixels)
-    :rtype: numpy.ndarray
+    :returns: a numpy array containing the images (frames, y-pixels, x-pixels)
     """
     files = list(folder.glob("*tif"))
     images = [_load_single_tif(file) for file in files]
 
     for image in images:
         assert (image.shape[1:] == images[0].shape[1:]), "Images don't maintain consistent shape"
 
@@ -211,15 +214,14 @@
 
 class _Metadata:
     def __init__(self, images: Optional[np.ndarray] = None):
         """
         Metadata object using for saving/loading binary images
 
         :param images: images in numpy array (frames, y-pixels, x-pixels)
-        :type images: numpy.ndarray
         """
         self.frames, self.y, self.x, self.dtype = None, None, None, None
 
         if images is not None:
             self.frames, self.y, self.x = images.shape
             self.dtype = str(images.dtype)
```

### Comparing `CalSciPy-0.3.0/src/CalSciPy/misc.py` & `CalSciPy-0.3.1/src/CalSciPy/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,7 +200,48 @@
         :return: whether the case/s are matched by the value/s
         :rtype: bool
         """
         for value, comparator, case in zip(self.value, self.comparison_expressions, cases):
             if not comparator(value, case):
                 return False
         return True
+        
+        
+def sliding_window(sequence: np.ndarray, window_length: int, function: Callable, *args, **kwargs) -> np.ndarray:
+    window_gen = generate_sliding_window(range(sequence.shape[-1]), window_length, 1)
+    values = []
+    sequence_length = sequence.shape[-1] - window_length + 2
+    pbar = tqdm(total=sequence_length, desc="Calculating baselines...")
+    try:
+        for step in window_gen:
+            values.append(function(sequence[..., step], *args, **kwargs))
+            pbar.update(1)
+    except (RuntimeError, StopIteration):
+        pass
+    pbar.close()
+    return np.array(values)
+
+
+def generate_sliding_window(sequence: Iterable, window_length: int, step_size: int = 1) -> np.ndarray:
+
+    window = deque(maxlen=window_length)
+    iterable = iter(sequence)
+
+    for _ in range(window_length):
+        window.append(next(iterable))
+
+    while True:
+        try:
+            yield tuple(window)
+            for idx in range(step_size):
+                window.append(next(iterable))
+
+        except StopIteration:
+            # noinspection PyUnboundLocalVariable
+            if idx == 0:
+                pass
+            elif idx == step_size:
+                pass
+            else:
+                yield tuple(window)
+            raise StopIteration
+
```

### Comparing `CalSciPy-0.3.0/src/CalSciPy/reorganization.py` & `CalSciPy-0.3.1/src/CalSciPy/reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/src/CalSciPy/trace_processing.py` & `CalSciPy-0.3.1/src/CalSciPy/trace_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.3.1/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.3.0/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.3.1/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/tests/test_a_install.py` & `CalSciPy-0.3.1/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/tests/test_bruker.py` & `CalSciPy-0.3.1/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/tests/test_event_processing.py` & `CalSciPy-0.3.1/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/tests/test_io_tools.py` & `CalSciPy-0.3.1/tests/test_io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/tests/test_misc.py` & `CalSciPy-0.3.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/tests/test_reorganization.py` & `CalSciPy-0.3.1/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.0/tests/test_trace_processing.py` & `CalSciPy-0.3.1/tests/test_trace_processing.py`

 * *Files identical despite different names*

