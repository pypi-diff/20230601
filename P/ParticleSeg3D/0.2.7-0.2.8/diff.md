# Comparing `tmp/ParticleSeg3D-0.2.7.tar.gz` & `tmp/ParticleSeg3D-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParticleSeg3D-0.2.7.tar", last modified: Wed May 31 15:16:50 2023, max compression
+gzip compressed data, was "ParticleSeg3D-0.2.8.tar", last modified: Thu Jun  1 12:15:59 2023, max compression
```

## Comparing `ParticleSeg3D-0.2.7.tar` & `ParticleSeg3D-0.2.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-05-31 15:16:50.344584 ParticleSeg3D-0.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/nifti2tiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/nifti2zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/tiff2nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/tiff2zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/zarr2tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/border_core2instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/model_nnunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/train/instance2border_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/train/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28913 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-31 15:16:50.344584 ParticleSeg3D-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:59.885473 ParticleSeg3D-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-06-01 12:15:59.885473 ParticleSeg3D-0.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:59.881473 ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-06-01 12:15:59.000000 ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 12:15:59.000000 ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:15:59.000000 ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 12:15:59.000000 ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 12:15:59.000000 ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 12:15:59.000000 ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:59.881473 ParticleSeg3D-0.2.8/particleseg3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:59.881473 ParticleSeg3D-0.2.8/particleseg3d/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:59.881473 ParticleSeg3D-0.2.8/particleseg3d/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/conversion/nifti2tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/conversion/nifti2zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/conversion/tiff2nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/conversion/tiff2zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/conversion/zarr2tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:59.885473 ParticleSeg3D-0.2.8/particleseg3d/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/inference/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/inference/border_core2instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/inference/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/inference/model_nnunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/inference/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:59.885473 ParticleSeg3D-0.2.8/particleseg3d/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/train/instance2border_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/train/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:59.885473 ParticleSeg3D-0.2.8/particleseg3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28913 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/particleseg3d/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-01 12:15:59.889473 ParticleSeg3D-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:15:42.000000 ParticleSeg3D-0.2.8/setup.py
```

### Comparing `ParticleSeg3D-0.2.7/LICENSE` & `ParticleSeg3D-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/PKG-INFO` & `ParticleSeg3D-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticleSeg3D
-Version: 0.2.7
+Version: 0.2.8
 Summary: Scalable, out-of-the box segmentation of individual particles from mineral samples acquired with micro CT
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/PKG-INFO` & `ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticleSeg3D
-Version: 0.2.7
+Version: 0.2.8
 Summary: Scalable, out-of-the box segmentation of individual particles from mineral samples acquired with micro CT
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/SOURCES.txt` & `ParticleSeg3D-0.2.8/ParticleSeg3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/README.md` & `ParticleSeg3D-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/conversion/nifti2tiff.py` & `ParticleSeg3D-0.2.8/particleseg3d/conversion/nifti2tiff.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/conversion/nifti2zarr.py` & `ParticleSeg3D-0.2.8/particleseg3d/conversion/tiff2nifti.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,37 @@
+from typing import Tuple
+import tifffile
 import argparse
 from particleseg3d.utils import utils
-from tqdm import tqdm
 from os.path import join
-import zarr
+from tqdm import tqdm
 import os
 
 
-def all_nifti2zarr(load_dir: str, save_dir: str) -> None:
-    """
-    Converts all nifti files into zarr files.
-
-    Args:
-        load_dir (str): Directory where the nifti files are located.
-        save_dir (str): Directory where the zarr files should be saved.
-    """
-    names = utils.load_filepaths(load_dir, extension=".nii.gz", return_path=False, return_extension=False)
-    for name in tqdm(names, desc="Image conversion"):
-        nifti2zarr(join(load_dir, name + ".nii.gz"), join(save_dir, name + ".zarr"))
-
-
-def nifti2zarr(load_filepath: str, save_filepath: str) -> None:
+def tiff2nifti(load_dir: str, save_dir: str, spacing: Tuple[float, float, float]) -> None:
     """
-    Converts a single nifti file to a zarr file.
+    Converts a set of TIFF image slices to a NIFTI image.
 
     Args:
-        load_filepath (str): Path to the nifti file.
-        save_dir (str): Path to where the zarr file should be saved.
+        load_dir (str): Path to the TIFF files.
+        save_dir (str): Path to where the NIFTI image should be saved.
     """
-    image = utils.load_nifti(load_filepath)
-    image_zarr = zarr.open(save_filepath, shape=image.shape, mode='w')
-    image_zarr[...] = image
+    name = os.path.basename(os.path.normpath(load_dir))
+    filepaths = utils.load_filepaths(load_dir, extension=["tif", "tiff", "TIF", "TIFF"])
+    image = tifffile.imread(filepaths)
+    utils.save_nifti(join(save_dir, name + ".nii.gz"), image, spacing=spacing)
 
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('-i', "--input", required=True,
-                        help="Absolute input path to the file(s) that should be converted to from Nifti to Zarr.")
-    parser.add_argument('-o', "--output", required=True, help="Absolute output path to the folder that should be used for the Zarr images.")
+                        help="Absolute input path to the folder of TIFF images that should be converted to a single NIFTI image.")
+    parser.add_argument('-o', "--output", required=True, help="Absolute output path to the folder, where the NIFTI image should be saved without the filename.")
+    parser.add_argument('-s', "--spacing", required=True, type=float, nargs=3,
+                        help="The image spacing given as three numbers separate by spaces.")
     args = parser.parse_args()
 
-    if not args.input.endswith(".nii.gz"):
-        all_nifti2zarr(args.input, args.output)
-    else:
-        nifti2zarr(args.input, args.output)
+    tiff2nifti(args.input, args.output, args.spacing)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/conversion/tiff2nifti.py` & `ParticleSeg3D-0.2.8/particleseg3d/conversion/tiff2zarr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from typing import Tuple
-import tifffile
-import argparse
-from particleseg3d.utils import utils
-from os.path import join
-from tqdm import tqdm
-import os
-
-
-def tiff2nifti(load_dir: str, save_dir: str, spacing: Tuple[float, float, float]) -> None:
-    """
-    Converts a set of TIFF image slices to a NIFTI image.
-
-    Args:
-        load_dir (str): Path to the TIFF files.
-        save_dir (str): Path to where the NIFTI image should be saved.
-    """
-    name = os.path.basename(os.path.normpath(load_dir))
-    filepaths = utils.load_filepaths(load_dir, extension=["tif", "tiff", "TIF", "TIFF"])
-    image = tifffile.imread(filepaths)
-    utils.save_nifti(join(save_dir, name + ".nii.gz"), image, spacing=spacing)
-
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('-i', "--input", required=True,
-                        help="Absolute input path to the folder of TIFF images that should be converted to a single NIFTI image.")
-    parser.add_argument('-o', "--output", required=True, help="Absolute output path to the folder, where the NIFTI image should be saved without the filename.")
-    parser.add_argument('-s', "--spacing", required=True, type=float, nargs=3,
-                        help="The image spacing given as three numbers separate by spaces.")
-    args = parser.parse_args()
-
-    tiff2nifti(args.input, args.output, args.spacing)
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import os
+from particleseg3d.utils import utils
+import tifffile
+from tqdm import tqdm
+from os.path import join
+import zarr
+
+
+def tiff2zarr(load_dir: str, save_dir: str) -> None:
+    """
+    Converts a set of TIFF image slices to a Zarr image.
+
+    Args:
+        load_dir (str): Path to the TIFF files.
+        save_dir (str): Path to where the Zarr image should be saved.
+    """
+    name = os.path.basename(os.path.normpath(load_dir))
+    filepaths = utils.load_filepaths(load_dir, extension=["tif", "tiff", "TIF", "TIFF"])
+    image_shape = tifffile.imread(filepaths[0]).shape
+    image_shape = (len(filepaths), *image_shape)
+    image_zarr = zarr.open(join(save_dir, name + ".zarr"), shape=image_shape, mode='w')
+    for i, filepath in enumerate(tqdm(filepaths)):
+        image_slice = tifffile.imread(filepath)    
+        image_zarr[i] = image_slice
+
+
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-i', "--input", required=True,
+                        help="Absolute input path to the folder that contains the TIFF image slices that should be converted to a Zarr image.")
+    parser.add_argument('-o', "--output", required=True, help="Absolute output path to the folder that should be used to save the Zarr image.")
+    args = parser.parse_args()
+
+    tiff2zarr(args.input, args.output)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/conversion/zarr2tiff.py` & `ParticleSeg3D-0.2.8/particleseg3d/conversion/zarr2tiff.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/inference/aggregator.py` & `ParticleSeg3D-0.2.8/particleseg3d/inference/aggregator.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/inference/border_core2instance.py` & `ParticleSeg3D-0.2.8/particleseg3d/inference/border_core2instance.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/inference/inference.py` & `ParticleSeg3D-0.2.8/particleseg3d/inference/inference.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/inference/model_nnunet.py` & `ParticleSeg3D-0.2.8/particleseg3d/inference/model_nnunet.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/inference/sampler.py` & `ParticleSeg3D-0.2.8/particleseg3d/inference/sampler.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/train/instance2border_core.py` & `ParticleSeg3D-0.2.8/particleseg3d/train/instance2border_core.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/train/preprocess.py` & `ParticleSeg3D-0.2.8/particleseg3d/train/preprocess.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/particleseg3d/utils/utils.py` & `ParticleSeg3D-0.2.8/particleseg3d/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/pyproject.toml` & `ParticleSeg3D-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.7/setup.cfg` & `ParticleSeg3D-0.2.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 [options.entry_points]
 console_scripts = 
 	ps3d_inference = particleseg3d.inference.inference:main
 	ps3d_tiff2zarr = particleseg3d.conversion.tiff2zarr:main
 	ps3d_zarr2tiff = particleseg3d.conversion.zarr2tiff:main
 	ps3d_tiff2nifti = particleseg3d.conversion.tiff2nifti:main
 	ps3d_nifti2tiff = particleseg3d.conversion.nifti2tiff:main
+	ps3d_nifti2zarr = particleseg3d.conversion.nifti2zarr:main
 	ps3d_train_preprocess = particleseg3d.train.preprocess:main
 
 [options.extras_require]
 testing = 
 	tox
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
```

