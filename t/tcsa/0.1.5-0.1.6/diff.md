# Comparing `tmp/tcsa-0.1.5.tar.gz` & `tmp/tcsa-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/radvi/Downloads/tcsa-0.1.5/dist/.tmp-0p9h5x3_/tcsa-0.1.5.tar", last modified: Thu May 25 12:38:12 2023, max compression
+gzip compressed data, was "/mnt/c/Users/radvi/Downloads/tcsa-0.1.6/dist/.tmp-520ame2s/tcsa-0.1.6.tar", last modified: Thu Jun  1 10:12:45 2023, max compression
```

## Comparing `tcsa-0.1.5.tar` & `tcsa-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-05-25 12:38:12.000000 tcsa-0.1.5/
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)    35159 2022-10-27 09:36:51.000000 tcsa-0.1.5/LICENSE
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       29 2022-07-18 17:33:57.000000 tcsa-0.1.5/MANIFEST.in
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2866 2023-05-25 12:38:12.000000 tcsa-0.1.5/PKG-INFO
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2210 2023-05-25 11:09:05.000000 tcsa-0.1.5/README.md
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     1044 2023-05-25 12:34:13.000000 tcsa-0.1.5/pyproject.toml
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      213 2023-05-25 12:38:12.000000 tcsa-0.1.5/setup.cfg
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       93 2022-07-18 17:43:33.000000 tcsa-0.1.5/setup.py
-drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/
-drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/tcsa/
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6497 2023-05-25 12:34:41.000000 tcsa-0.1.5/src/tcsa/__init__.py
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     1582 2022-10-27 10:30:55.000000 tcsa-0.1.5/src/tcsa/cli.py
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      310 2022-07-08 21:49:00.000000 tcsa-0.1.5/src/tcsa/config.json
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     3371 2022-10-27 10:28:39.000000 tcsa-0.1.5/src/tcsa/data.py
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     8868 2023-05-25 12:31:55.000000 tcsa-0.1.5/src/tcsa/data_preparation.py
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     3881 2022-10-27 10:27:19.000000 tcsa-0.1.5/src/tcsa/manual.py
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     7123 2022-10-27 10:27:38.000000 tcsa-0.1.5/src/tcsa/model.py
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     5925 2023-05-25 12:31:29.000000 tcsa-0.1.5/src/tcsa/pipeline.py
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6732 2023-05-25 12:33:28.000000 tcsa-0.1.5/src/tcsa/prequisite.py
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6775 2022-10-27 10:30:37.000000 tcsa-0.1.5/src/tcsa/thresholding.py
-drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/tcsa.egg-info/
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2866 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/tcsa.egg-info/PKG-INFO
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      467 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/tcsa.egg-info/SOURCES.txt
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        1 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/tcsa.egg-info/dependency_links.txt
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       39 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/tcsa.egg-info/entry_points.txt
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      215 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/tcsa.egg-info/requires.txt
--rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        5 2023-05-25 12:38:12.000000 tcsa-0.1.5/src/tcsa.egg-info/top_level.txt
+drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-06-01 10:12:45.000000 tcsa-0.1.6/
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)    35159 2022-10-27 09:36:51.000000 tcsa-0.1.6/LICENSE
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       29 2022-07-18 17:33:57.000000 tcsa-0.1.6/MANIFEST.in
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2866 2023-06-01 10:12:45.000000 tcsa-0.1.6/PKG-INFO
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2210 2023-06-01 10:05:24.000000 tcsa-0.1.6/README.md
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     1087 2023-06-01 10:04:55.000000 tcsa-0.1.6/pyproject.toml
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      213 2023-06-01 10:12:45.000000 tcsa-0.1.6/setup.cfg
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       93 2022-07-18 17:43:33.000000 tcsa-0.1.6/setup.py
+drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/
+drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/tcsa/
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6497 2023-05-25 12:34:41.000000 tcsa-0.1.6/src/tcsa/__init__.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     1582 2022-10-27 10:30:55.000000 tcsa-0.1.6/src/tcsa/cli.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      310 2022-07-08 21:49:00.000000 tcsa-0.1.6/src/tcsa/config.json
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     3371 2022-10-27 10:28:39.000000 tcsa-0.1.6/src/tcsa/data.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     9080 2023-06-01 10:02:45.000000 tcsa-0.1.6/src/tcsa/data_preparation.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     3881 2022-10-27 10:27:19.000000 tcsa-0.1.6/src/tcsa/manual.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     7123 2022-10-27 10:27:38.000000 tcsa-0.1.6/src/tcsa/model.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     5925 2023-05-25 12:31:29.000000 tcsa-0.1.6/src/tcsa/pipeline.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6732 2023-05-25 12:33:28.000000 tcsa-0.1.6/src/tcsa/prequisite.py
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     6775 2022-10-27 10:30:37.000000 tcsa-0.1.6/src/tcsa/thresholding.py
+drwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        0 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/tcsa.egg-info/
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)     2866 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/tcsa.egg-info/PKG-INFO
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      467 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/tcsa.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        1 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/tcsa.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)       39 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/tcsa.egg-info/entry_points.txt
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)      247 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/tcsa.egg-info/requires.txt
+-rwxrwxrwx   0 rm5417    (1000) rm5417    (1000)        5 2023-06-01 10:12:45.000000 tcsa-0.1.6/src/tcsa.egg-info/top_level.txt
```

### Comparing `tcsa-0.1.5/LICENSE` & `tcsa-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/PKG-INFO` & `tcsa-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcsa
-Version: 0.1.5
+Version: 0.1.6
 Summary: temporalis segmentation pipeline to assess CSA of temporalis muscle
 Author: Computational Oncology
 Project-URL: Homepage, https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline
 Project-URL: Bug Tracker, https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tcsa-0.1.5/README.md` & `tcsa-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/pyproject.toml` & `tcsa-0.1.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tcsa"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Computational Oncology"},
 ]
 description = "temporalis segmentation pipeline to assess CSA of temporalis muscle"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -20,14 +20,16 @@
 dependencies = [
   'keras==2.2.4',
   'tensorflow==1.14.0',
   'segmentation-models==1.0.1',
   'protobuf==3.20.1',
   'h5py==2.10.0',
   'opencv-python',
+  'Pillow==9.5.0', 
+  'matplotlib==3.5.3',
   'antspyx',
   'nibabel',
   'intensity-normalization==2.1.4',
   'scikit-image',
   'gdown',
   'tqdm',
   'simpleitk',
```

### Comparing `tcsa-0.1.5/src/tcsa/__init__.py` & `tcsa-0.1.6/src/tcsa/__init__.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/src/tcsa/cli.py` & `tcsa-0.1.6/src/tcsa/cli.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/src/tcsa/data.py` & `tcsa-0.1.6/src/tcsa/data.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/src/tcsa/data_preparation.py` & `tcsa-0.1.6/src/tcsa/data_preparation.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 # along with this program.  If not, see https://www.gnu.org/licenses/.
 
 from pathlib import Path
 import os
 from shutil import rmtree
 from tqdm import tqdm
 import sys
+import matplotlib.pyplot as plt
+from matplotlib import cm
+from PIL import Image, ImageOps
 
 import numpy as np
 import nibabel as nib
 import ants
 import imageio
 
 from tcsa import PATHS
@@ -219,11 +222,13 @@
         ):
             img = nib.load(slice).get_fdata()
             img = np.rot90(img[:,:], 3)
             filename = slice.name[: -len(''.join(slice.suffixes))]
             output_directory = path_to_test_folder / patient.name / 'original'
             output_directory.mkdir(parents=True, exist_ok=True)
             output_path = output_directory / f'{filename}.png'
-            # additional line to work with new imageio version (2.29.0)
-            img_upd = img.astype('uint8')
-            # end of new code
-            imageio.imsave(str(output_path), img_upd)
+            # additional code to save images in a new way as imageio newest  versions throws an error
+
+            plt.imsave(str(output_path), img, cmap = cm.gray)
+            im_mat = Image.open(str(output_path), 'r')
+            im_mat_gray = ImageOps.grayscale(im_mat)
+            im_mat_gray.save(str(output_path))
```

### Comparing `tcsa-0.1.5/src/tcsa/manual.py` & `tcsa-0.1.6/src/tcsa/manual.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/src/tcsa/model.py` & `tcsa-0.1.6/src/tcsa/model.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/src/tcsa/pipeline.py` & `tcsa-0.1.6/src/tcsa/pipeline.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/src/tcsa/prequisite.py` & `tcsa-0.1.6/src/tcsa/prequisite.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/src/tcsa/thresholding.py` & `tcsa-0.1.6/src/tcsa/thresholding.py`

 * *Files identical despite different names*

### Comparing `tcsa-0.1.5/src/tcsa.egg-info/PKG-INFO` & `tcsa-0.1.6/src/tcsa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcsa
-Version: 0.1.5
+Version: 0.1.6
 Summary: temporalis segmentation pipeline to assess CSA of temporalis muscle
 Author: Computational Oncology
 Project-URL: Homepage, https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline
 Project-URL: Bug Tracker, https://gitlab.com/computational.oncology/temporalis-segmentation-pipeline/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

