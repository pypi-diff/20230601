# Comparing `tmp/voxelwise_tutorials-0.1.5.tar.gz` & `tmp/voxelwise_tutorials-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelwise_tutorials-0.1.5.tar", last modified: Tue Feb  7 22:46:49 2023, max compression
+gzip compressed data, was "voxelwise_tutorials-0.1.6.tar", last modified: Wed May 31 23:13:13 2023, max compression
```

## Comparing `voxelwise_tutorials-0.1.5.tar` & `voxelwise_tutorials-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:46:49.594416 voxelwise_tutorials-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-02-07 22:46:49.594416 voxelwise_tutorials-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 22:46:49.594416 voxelwise_tutorials-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:46:49.594416 voxelwise_tutorials-0.1.5/voxelwise_tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/delayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/io.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/regression_toy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:46:49.594416 voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_delayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_regression_toy.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-02-07 22:46:36.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:46:49.594416 voxelwise_tutorials-0.1.5/voxelwise_tutorials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-02-07 22:46:49.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-07 22:46:49.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 22:46:49.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-07 22:46:49.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-07 22:46:49.000000 voxelwise_tutorials-0.1.5/voxelwise_tutorials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:13:13.240598 voxelwise_tutorials-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-31 23:13:13.240598 voxelwise_tutorials-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:13:13.240598 voxelwise_tutorials-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:13:13.236598 voxelwise_tutorials-0.1.6/voxelwise_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/delayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/regression_toy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:13:13.240598 voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_delayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_regression_toy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-05-31 23:12:58.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:13:13.236598 voxelwise_tutorials-0.1.6/voxelwise_tutorials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-31 23:13:13.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-31 23:13:13.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:13:13.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-31 23:13:13.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 23:13:13.000000 voxelwise_tutorials-0.1.6/voxelwise_tutorials.egg-info/top_level.txt
```

### Comparing `voxelwise_tutorials-0.1.5/LICENSE.md` & `voxelwise_tutorials-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/PKG-INFO` & `voxelwise_tutorials-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelwise_tutorials
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools and tutorials for voxelwise modeling
 Maintainer: Tom Dupre la Tour
 Maintainer-email: tom.dupre-la-tour@m4x.org
 License: BSD (3-clause)
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: github
@@ -19,17 +19,18 @@
 Welcome to the voxelwise modeling tutorial from the
 `Gallantlab <https://gallantlab.org>`_.
 
 Tutorials
 =========
 
 This repository contains tutorials describing how to use the voxelwise modeling
-framework. Voxelwise modeling is a framework to perform functional magnetic
-resonance imaging (fMRI) data analysis, fitting encoding models at the voxel
-level.
+framework. `Voxelwise modeling
+<https://gallantlab.github.io/voxelwise_tutorials/voxelwise_modeling.html>`_ is
+a framework to perform functional magnetic resonance imaging (fMRI) data
+analysis, fitting encoding models at the voxel level.
 
 To explore these tutorials, one can:
 
 - read the rendered examples in the tutorials
   `website <https://gallantlab.github.io/voxelwise_tutorials/>`_ (recommended)
 - run the Python scripts (`tutorials <tutorials>`_ directory)
 - run the Jupyter notebooks (`tutorials/notebooks <tutorials/notebooks>`_ directory)
@@ -108,15 +109,15 @@
 Cite as
 =======
 
 If you use one of our packages in your work (``voxelwise_tutorials`` [1]_,
 ``himalaya`` [2]_, ``pycortex`` [3]_, or ``pymoten`` [4]_), please cite the
 corresponding publications:
 
-.. [1] Dupré La Tour, T., Visconti di Oleggio Castello, M., & Gallant, J. L. (2022).
+.. [1] Dupré La Tour, T., Visconti di Oleggio Castello, M., & Gallant, J. L. (2023).
    Voxelwise modeling tutorials: an encoding model approach to functional MRI analysis.
    *In preparation*.
 
 .. [2] Dupré La Tour, T., Eickenberg, M., Nunez-Elizalde, A.O., & Gallant, J. L. (2022).
    Feature-space selection with banded ridge regression. NeuroImage.
    https://doi.org/10.1016/j.neuroimage.2022.119728
```

### Comparing `voxelwise_tutorials-0.1.5/README.rst` & `voxelwise_tutorials-0.1.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 Welcome to the voxelwise modeling tutorial from the
 `Gallantlab <https://gallantlab.org>`_.
 
 Tutorials
 =========
 
 This repository contains tutorials describing how to use the voxelwise modeling
-framework. Voxelwise modeling is a framework to perform functional magnetic
-resonance imaging (fMRI) data analysis, fitting encoding models at the voxel
-level.
+framework. `Voxelwise modeling
+<https://gallantlab.github.io/voxelwise_tutorials/voxelwise_modeling.html>`_ is
+a framework to perform functional magnetic resonance imaging (fMRI) data
+analysis, fitting encoding models at the voxel level.
 
 To explore these tutorials, one can:
 
 - read the rendered examples in the tutorials
   `website <https://gallantlab.github.io/voxelwise_tutorials/>`_ (recommended)
 - run the Python scripts (`tutorials <tutorials>`_ directory)
 - run the Jupyter notebooks (`tutorials/notebooks <tutorials/notebooks>`_ directory)
@@ -96,15 +97,15 @@
 Cite as
 =======
 
 If you use one of our packages in your work (``voxelwise_tutorials`` [1]_,
 ``himalaya`` [2]_, ``pycortex`` [3]_, or ``pymoten`` [4]_), please cite the
 corresponding publications:
 
-.. [1] Dupré La Tour, T., Visconti di Oleggio Castello, M., & Gallant, J. L. (2022).
+.. [1] Dupré La Tour, T., Visconti di Oleggio Castello, M., & Gallant, J. L. (2023).
    Voxelwise modeling tutorials: an encoding model approach to functional MRI analysis.
    *In preparation*.
 
 .. [2] Dupré La Tour, T., Eickenberg, M., Nunez-Elizalde, A.O., & Gallant, J. L. (2022).
    Feature-space selection with banded ridge regression. NeuroImage.
    https://doi.org/10.1016/j.neuroimage.2022.119728
```

### Comparing `voxelwise_tutorials-0.1.5/setup.py` & `voxelwise_tutorials-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/delayer.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/delayer.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/io.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/io.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/regression_toy.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/regression_toy.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_delayer.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_delayer.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_io.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_mappers.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_model.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_regression_toy.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_regression_toy.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/tests/test_utils.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/utils.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/utils.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/viz.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,18 +69,21 @@
 
 def plot_flatmap_from_mapper(voxels, mapper_file, ax=None, alpha=0.7,
                              cmap='inferno', vmin=None, vmax=None,
                              with_curvature=True, with_rois=True,
                              with_colorbar=True,
                              colorbar_location=(.4, .9, .2, .05)):
     """Plot a flatmap from a mapper file, with 1D data.
+    
+    This function is equivalent to the pycortex functions:
+    cortex.quickshow(cortex.Volume(voxels, ...), ...)
 
     Note that this function does not have the full capability of pycortex,
-    (like cortex.quickshow) since it is based on flatmap mappers and not on the
-    original brain surface of the subject.
+    since it is based on flatmap mappers and not on the original brain
+    surface of the subject.
 
     Parameters
     ----------
     voxels : array of shape (n_voxels, )
         Data to be plotted.
     mapper_file : str
         File name of the mapper.
@@ -218,17 +221,20 @@
                                 alpha=0.7, cmap='BuOr_2D', vmin=None,
                                 vmax=None, vmin2=None, vmax2=None,
                                 with_curvature=True, with_rois=True,
                                 with_colorbar=True, label_1='', label_2='',
                                 colorbar_location=(.45, .85, .1, .1)):
     """Plot a flatmap from a mapper file, with 2D data.
 
+    This function is equivalent to the pycortex functions:
+    cortex.quickshow(cortex.Volume2D(voxels_1, voxels_2, ...), ...)
+
     Note that this function does not have the full capability of pycortex,
-    (like cortex.quickshow) since it is based on flatmap mappers and not on the
-    original brain surface of the subject.
+    since it is based on flatmap mappers and not on the original brain
+    surface of the subject.
 
     Parameters
     ----------
     voxels_1 : array of shape (n_voxels, )
         Data to be plotted.
     voxels_2 : array of shape (n_voxels, )
         Data to be plotted.
@@ -367,17 +373,20 @@
 
 def plot_3d_flatmap_from_mapper(voxels_1, voxels_2, voxels_3, mapper_file,
                                 ax=None, alpha=0.7, vmin=None, vmax=None,
                                 vmin2=None, vmax2=None, vmin3=None, vmax3=None,
                                 with_curvature=True, with_rois=True):
     """Plot a flatmap from a mapper file, with 3D data.
 
+    This function is equivalent to the pycortex functions:
+    cortex.quickshow(cortex.VolumeRGB(voxels_1, voxels_2, voxels_3, ...), ...)
+
     Note that this function does not have the full capability of pycortex,
-    (like cortex.quickshow) since it is based on flatmap mappers and not on the
-    original brain surface of the subject.
+    since it is based on flatmap mappers and not on the original brain
+    surface of the subject.
 
     Parameters
     ----------
     voxels_1 : array of shape (n_voxels, )
         Data to be plotted.
     voxels_2 : array of shape (n_voxels, )
         Data to be plotted.
```

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials/wordnet.py` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials/wordnet.py`

 * *Files identical despite different names*

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials.egg-info/PKG-INFO` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelwise-tutorials
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools and tutorials for voxelwise modeling
 Maintainer: Tom Dupre la Tour
 Maintainer-email: tom.dupre-la-tour@m4x.org
 License: BSD (3-clause)
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: github
@@ -19,17 +19,18 @@
 Welcome to the voxelwise modeling tutorial from the
 `Gallantlab <https://gallantlab.org>`_.
 
 Tutorials
 =========
 
 This repository contains tutorials describing how to use the voxelwise modeling
-framework. Voxelwise modeling is a framework to perform functional magnetic
-resonance imaging (fMRI) data analysis, fitting encoding models at the voxel
-level.
+framework. `Voxelwise modeling
+<https://gallantlab.github.io/voxelwise_tutorials/voxelwise_modeling.html>`_ is
+a framework to perform functional magnetic resonance imaging (fMRI) data
+analysis, fitting encoding models at the voxel level.
 
 To explore these tutorials, one can:
 
 - read the rendered examples in the tutorials
   `website <https://gallantlab.github.io/voxelwise_tutorials/>`_ (recommended)
 - run the Python scripts (`tutorials <tutorials>`_ directory)
 - run the Jupyter notebooks (`tutorials/notebooks <tutorials/notebooks>`_ directory)
@@ -108,15 +109,15 @@
 Cite as
 =======
 
 If you use one of our packages in your work (``voxelwise_tutorials`` [1]_,
 ``himalaya`` [2]_, ``pycortex`` [3]_, or ``pymoten`` [4]_), please cite the
 corresponding publications:
 
-.. [1] Dupré La Tour, T., Visconti di Oleggio Castello, M., & Gallant, J. L. (2022).
+.. [1] Dupré La Tour, T., Visconti di Oleggio Castello, M., & Gallant, J. L. (2023).
    Voxelwise modeling tutorials: an encoding model approach to functional MRI analysis.
    *In preparation*.
 
 .. [2] Dupré La Tour, T., Eickenberg, M., Nunez-Elizalde, A.O., & Gallant, J. L. (2022).
    Feature-space selection with banded ridge regression. NeuroImage.
    https://doi.org/10.1016/j.neuroimage.2022.119728
```

### Comparing `voxelwise_tutorials-0.1.5/voxelwise_tutorials.egg-info/SOURCES.txt` & `voxelwise_tutorials-0.1.6/voxelwise_tutorials.egg-info/SOURCES.txt`

 * *Files identical despite different names*

