# Comparing `tmp/s2cloudless-1.7.0.tar.gz` & `tmp/s2cloudless-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2cloudless-1.7.0.tar", last modified: Mon Feb 13 14:09:02 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `s2cloudless-1.7.0.tar` & `s2cloudless-1.7.1.tar`

### file list

```diff
@@ -1,29 +1,11 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-02-13 14:09:02.929810 s2cloudless-1.7.0/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    18625 2022-09-05 11:10:37.000000 s2cloudless-1.7.0/LICENSE.md
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      139 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5839 2023-02-13 14:09:02.929810 s2cloudless-1.7.0/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4382 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/README.md
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1186 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/pyproject.toml
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       70 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/requirements-dev.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      103 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/requirements.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-02-13 14:09:02.909810 s2cloudless-1.7.0/s2cloudless/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      244 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/s2cloudless/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6744 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/s2cloudless/cloud_detector.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-02-13 14:09:02.913810 s2cloudless-1.7.0/s2cloudless/models/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000) 10975392 2022-09-05 11:10:37.000000 s2cloudless-1.7.0/s2cloudless/models/pixel_s2_cloud_detector_lightGBM_v0.1.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3447 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/s2cloudless/pixel_classifier.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        0 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/s2cloudless/py.typed
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4819 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/s2cloudless/utils.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-02-13 14:09:02.913810 s2cloudless-1.7.0/s2cloudless.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5839 2023-02-13 14:09:02.000000 s2cloudless-1.7.0/s2cloudless.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      571 2023-02-13 14:09:02.000000 s2cloudless-1.7.0/s2cloudless.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-02-13 14:09:02.000000 s2cloudless-1.7.0/s2cloudless.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2022-09-05 11:18:42.000000 s2cloudless-1.7.0/s2cloudless.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      180 2023-02-13 14:09:02.000000 s2cloudless-1.7.0/s2cloudless.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       12 2023-02-13 14:09:02.000000 s2cloudless-1.7.0/s2cloudless.egg-info/top_level.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-02-13 14:09:02.929810 s2cloudless-1.7.0/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2155 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/setup.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-02-13 14:09:02.929810 s2cloudless-1.7.0/tests/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2207 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/tests/test_cloud_detector.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2819 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/tests/test_pixel_classifier.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3880 2023-02-13 14:02:36.000000 s2cloudless-1.7.0/tests/test_utils.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/s2cloudless/__init__.py
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/s2cloudless/cloud_detector.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/s2cloudless/pixel_classifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/s2cloudless/py.typed
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/s2cloudless/utils.py
+-rw-r--r--   0        0        0 10975392 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/s2cloudless/models/pixel_s2_cloud_detector_lightGBM_v0.1.txt
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/.gitignore
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/LICENSE.md
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/README.md
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    26045 2020-02-02 00:00:00.000000 s2cloudless-1.7.1/PKG-INFO
```

### Comparing `s2cloudless-1.7.0/LICENSE.md` & `s2cloudless-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `s2cloudless-1.7.0/PKG-INFO` & `s2cloudless-1.7.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,56 @@
-Metadata-Version: 2.1
-Name: s2cloudless
-Version: 1.7.0
-Summary: Sentinel Hub's cloud detector for Sentinel-2 imagery
-Home-page: https://github.com/sentinel-hub/sentinel2-cloud-detector
-Author: Sinergise EO research team
-Author-email: eoresearch@sinergise.com
-License: CC BY-SA 4.0
-Description: [![Package version](https://badge.fury.io/py/s2cloudless.svg)](https://pypi.org/project/s2cloudless)
-        [![Conda version](https://img.shields.io/conda/vn/conda-forge/s2cloudless.svg)](https://anaconda.org/conda-forge/s2cloudless)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/s2cloudless.svg?style=flat-square)](https://pypi.org/project/s2cloudless)
-        [![Build Status](https://github.com/sentinel-hub/sentinel2-cloud-detector/actions/workflows/ci_action.yml/badge.svg?branch=master)](https://github.com/sentinel-hub/sentinel2-cloud-detector/actions)
-        [![Overall downloads](https://pepy.tech/badge/s2cloudless)](https://pepy.tech/project/s2cloudless)
-        [![Last month downloads](https://pepy.tech/badge/s2cloudless/month)](https://pepy.tech/project/s2cloudless)
-        [![Code coverage](https://codecov.io/gh/sentinel-hub/sentinel2-cloud-detector/branch/master/graph/badge.svg)](https://codecov.io/gh/sentinel-hub/sentinel2-cloud-detector)
-        
-        # Sentinel Hub's cloud detector for Sentinel-2 imagery
-        
-        **NOTE: s2cloudless masks are now available as a precomputed layer within Sentinel Hub. Check the [announcement blog post](https://medium.com/sentinel-hub/cloud-masks-at-your-service-6e5b2cb2ce8a) and [technical documentation](https://docs.sentinel-hub.com/api/latest/#/API/data_access?id=cloud-masks-and-cloud-probabilities).**
-        
-        The **s2cloudless** Python package provides automated cloud detection in
-        Sentinel-2 imagery. The classification is based on a *single-scene pixel-based cloud detector*
-        developed by Sentinel Hub's research team and is described in more detail
-        [in this blog](https://medium.com/sentinel-hub/improving-cloud-detection-with-machine-learning-c09dc5d7cf13).
-        
-        The **s2cloudless** algorithm was part of an international collaborative effort aimed at intercomparing cloud detection algorithms. The s2cloudless algorithm was validated together with 9 other algorithms on 4 different test datasets and in all cases found to be on the Pareto front. See [the paper](https://www.sciencedirect.com/science/article/pii/S0034425722001043?via%3Dihub)
-        
-        ## Installation
-        
-        The package requires a Python version >= 3.7. The package is available on
-        the PyPI package manager and can be installed with
-        
-        ```
-        $ pip install s2cloudless
-        ```
-        
-        To install the package manually, clone the repository and
-        ```
-        $ pip install .
-        ```
-        
-        One of `s2cloudless` dependencies is `lightgbm` package. If having problems during installation, please
-        check the [LightGBM installation guide](https://lightgbm.readthedocs.io/en/latest/Installation-Guide.html).
-        
-        Before installing `s2cloudless` on **Windows**, it is recommended to install package `shapely` from
-        [Unofficial Windows wheels repository](https://www.lfd.uci.edu/~gohlke/pythonlibs/)
-        
-        ## Input: Sentinel-2 scenes
-        
-        The inputs to the cloud detector are Sentinel-2 images. In particular, the cloud detector requires the following 10 Sentinel-2 band reflectances: B01, B02, B04, B05, B08, B8A, B09, B10, B11, B12, which are obtained from raw reflectance values in the following way: `B_i/10000`. From product baseline `04.00` onward additional harmonization factors have to be applied to data according to [instructions from ESA](https://sentinels.copernicus.eu/en/web/sentinel/-/copernicus-sentinel-2-major-products-upgrade-upcoming).
-        
-        You don't need to worry about any of this, if you are using Sentinel-2 data obtained from [Sentinel Hub Process API](https://docs.sentinel-hub.com/api/latest/api/process/). By default, the data is already harmonized according to [documentation](https://docs.sentinel-hub.com/api/latest/data/sentinel-2-l1c/#harmonize-values). The API is supported in Python with [sentinelhub-py](https://github.com/sentinel-hub/sentinelhub-py) package and used within `s2cloudless.CloudMaskRequest` class.
-        
-        ## Examples
-        
-        A Jupyter notebook on how to use the cloud detector to produce cloud mask or cloud probability map
-        can be found in the [examples folder](https://github.com/sentinel-hub/sentinel2-cloud-detector/tree/master/examples).
-        
-        ## License
-        
-        <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">
-        <img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>
-        <br />
-        This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: DEV
+[![Package version](https://badge.fury.io/py/s2cloudless.svg)](https://pypi.org/project/s2cloudless)
+[![Conda version](https://img.shields.io/conda/vn/conda-forge/s2cloudless.svg)](https://anaconda.org/conda-forge/s2cloudless)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/s2cloudless.svg?style=flat-square)](https://pypi.org/project/s2cloudless)
+[![Build Status](https://github.com/sentinel-hub/sentinel2-cloud-detector/actions/workflows/ci_action.yml/badge.svg?branch=master)](https://github.com/sentinel-hub/sentinel2-cloud-detector/actions)
+[![Overall downloads](https://pepy.tech/badge/s2cloudless)](https://pepy.tech/project/s2cloudless)
+[![Last month downloads](https://pepy.tech/badge/s2cloudless/month)](https://pepy.tech/project/s2cloudless)
+[![Code coverage](https://codecov.io/gh/sentinel-hub/sentinel2-cloud-detector/branch/master/graph/badge.svg)](https://codecov.io/gh/sentinel-hub/sentinel2-cloud-detector)
+
+# Sentinel Hub's cloud detector for Sentinel-2 imagery
+
+**NOTE: s2cloudless masks are now available as a precomputed layer within Sentinel Hub. Check the [announcement blog post](https://medium.com/sentinel-hub/cloud-masks-at-your-service-6e5b2cb2ce8a) and [technical documentation](https://docs.sentinel-hub.com/api/latest/#/API/data_access?id=cloud-masks-and-cloud-probabilities).**
+
+The **s2cloudless** Python package provides automated cloud detection in
+Sentinel-2 imagery. The classification is based on a *single-scene pixel-based cloud detector*
+developed by Sentinel Hub's research team and is described in more detail
+[in this blog](https://medium.com/sentinel-hub/improving-cloud-detection-with-machine-learning-c09dc5d7cf13).
+
+The **s2cloudless** algorithm was part of an international collaborative effort aimed at intercomparing cloud detection algorithms. The s2cloudless algorithm was validated together with 9 other algorithms on 4 different test datasets and in all cases found to be on the Pareto front. See [the paper](https://www.sciencedirect.com/science/article/pii/S0034425722001043?via%3Dihub)
+
+## Installation
+
+The package requires a Python version >= 3.8. The package is available on
+the PyPI package manager and can be installed with
+
+```
+$ pip install s2cloudless
+```
+
+To install the package manually, clone the repository and
+```
+$ pip install .
+```
+
+One of `s2cloudless` dependencies is `lightgbm` package. If having problems during installation, please
+check the [LightGBM installation guide](https://lightgbm.readthedocs.io/en/latest/Installation-Guide.html).
+
+Before installing `s2cloudless` on **Windows**, it is recommended to install package `shapely` from
+[Unofficial Windows wheels repository](https://www.lfd.uci.edu/~gohlke/pythonlibs/)
+
+## Input: Sentinel-2 scenes
+
+The inputs to the cloud detector are Sentinel-2 images. In particular, the cloud detector requires the following 10 Sentinel-2 band reflectances: B01, B02, B04, B05, B08, B8A, B09, B10, B11, B12, which are obtained from raw reflectance values in the following way: `B_i/10000`. From product baseline `04.00` onward additional harmonization factors have to be applied to data according to [instructions from ESA](https://sentinels.copernicus.eu/en/web/sentinel/-/copernicus-sentinel-2-major-products-upgrade-upcoming).
+
+You don't need to worry about any of this, if you are using Sentinel-2 data obtained from [Sentinel Hub Process API](https://docs.sentinel-hub.com/api/latest/api/process/). By default, the data is already harmonized according to [documentation](https://docs.sentinel-hub.com/api/latest/data/sentinel-2-l1c/#harmonize-values). The API is supported in Python with [sentinelhub-py](https://github.com/sentinel-hub/sentinelhub-py) package and used within `s2cloudless.CloudMaskRequest` class.
+
+## Examples
+
+A Jupyter notebook on how to use the cloud detector to produce cloud mask or cloud probability map
+can be found in the [examples folder](https://github.com/sentinel-hub/sentinel2-cloud-detector/tree/master/examples).
+
+## License
+
+<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">
+<img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>
+<br />
+This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
```

### Comparing `s2cloudless-1.7.0/s2cloudless/cloud_detector.py` & `s2cloudless-1.7.1/s2cloudless/cloud_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Module for pixel-based classification on Sentinel-2 L1C imagery."""
+from __future__ import annotations
+
 import os
-from typing import Any, Optional
+from typing import Any
 
+import cv2
 import numpy as np
 from lightgbm import Booster
-from scipy.ndimage import convolve
-from skimage.morphology import dilation, disk
 
 from .pixel_classifier import PixelClassifier
-from .utils import MODEL_BAND_IDS
+from .utils import MODEL_BAND_IDS, cv2_disk
 
 MODEL_FILENAME = "pixel_s2_cloud_detector_lightGBM_v0.1.txt"
 
 
 class S2PixelCloudDetector:
     """
     Sentinel Hub's pixel-based cloud detector for Sentinel-2 imagery.
@@ -38,35 +39,36 @@
         loaded.
     """
 
     def __init__(
         self,
         threshold: float = 0.4,
         all_bands: bool = False,
-        average_over: Optional[int] = 1,
-        dilation_size: Optional[int] = 1,
-        model_filename: Optional[str] = None,
+        average_over: int | None = 1,
+        dilation_size: int | None = 1,
+        model_filename: str | None = None,
     ):
         self.threshold = threshold
         self.all_bands = all_bands
         self.average_over = average_over
         self.dilation_size = dilation_size
 
         if model_filename is None:
             package_dir = os.path.dirname(__file__)
             model_filename = os.path.join(package_dir, "models", MODEL_FILENAME)
         self.model_filename = model_filename
 
-        self._classifier: Optional[PixelClassifier] = None
+        self._classifier: PixelClassifier | None = None
 
         if average_over is not None and average_over > 0:
-            self.conv_filter = disk(average_over) / np.sum(disk(average_over))
+            disk = cv2_disk(average_over)
+            self.conv_filter = disk / np.sum(disk)
 
         if dilation_size is not None and dilation_size > 0:
-            self.dilation_filter = disk(dilation_size)
+            self.dilation_filter = cv2_disk(dilation_size)
 
     @property
     def classifier(self) -> PixelClassifier:
         """Provides a classifier object by utilizing lazy-loading to avoid multiple IO operations."""
         if self._classifier is None:
             self._classifier = PixelClassifier(Booster(model_file=self.model_filename))
 
@@ -114,35 +116,38 @@
 
         :param data: A stack of Sentinel-2 images with all required bands in the correct order
         :param kwargs: Any keyword arguments that will be passed to the classifier's prediction method
         :return: raster cloud mask of shape `(N, height, width)`
         """
         self._check_data_dimension(data, 4)
         cloud_probs = self.get_cloud_probability_maps(data, **kwargs)
-        cloud_masks = self.get_mask_from_prob(cloud_probs)
 
-        return cloud_masks
+        return self.get_mask_from_prob(cloud_probs)
 
-    def get_mask_from_prob(self, cloud_probs: np.ndarray, threshold: Optional[float] = None) -> np.ndarray:
+    def get_mask_from_prob(self, cloud_probs: np.ndarray, threshold: float | None = None) -> np.ndarray:
         """
         Returns cloud mask by applying convolution and dilation to cloud probabilities.
 
         :param cloud_probs: cloud probability map of shape `(N, height, width)`
         :param threshold: A float from [0,1] specifying the probability threshold for mask creation
         :return: cloud mask of shape `(N, height, width)`
         """
         self._check_data_dimension(cloud_probs, 3)
         threshold = self.threshold if threshold is None else threshold
 
         if self.average_over:
             cloud_masks = np.asarray(
-                [convolve(cloud_prob, self.conv_filter) > threshold for cloud_prob in cloud_probs], dtype=np.uint8
+                [
+                    cv2.filter2D(cloud_prob, -1, self.conv_filter, borderType=cv2.BORDER_REFLECT) > threshold
+                    for cloud_prob in cloud_probs
+                ],
+                dtype=np.uint8,
             )
         else:
             cloud_masks = (cloud_probs > threshold).astype(np.int8)
 
         if self.dilation_size:
             cloud_masks = np.asarray(
-                [dilation(cloud_mask, self.dilation_filter) for cloud_mask in cloud_masks], dtype=np.uint8
+                [cv2.dilate(cloud_mask, self.dilation_filter) for cloud_mask in cloud_masks], dtype=np.uint8
             )
 
         return cloud_masks
```

### Comparing `s2cloudless-1.7.0/s2cloudless/models/pixel_s2_cloud_detector_lightGBM_v0.1.txt` & `s2cloudless-1.7.1/s2cloudless/models/pixel_s2_cloud_detector_lightGBM_v0.1.txt`

 * *Files identical despite different names*

### Comparing `s2cloudless-1.7.0/s2cloudless/pixel_classifier.py` & `s2cloudless-1.7.1/s2cloudless/pixel_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module for pixel-based classifiers."""
-from typing import Any, Union
+from __future__ import annotations
+
+from typing import Any, Protocol
 
 import numpy as np
 from lightgbm import Booster
-from typing_extensions import Protocol
 
 
 class ClassifierType(Protocol):
     """Defines the necessary classifier interface."""
 
     def predict(self, X: np.ndarray) -> np.ndarray:  # pylint: disable=missing-function-docstring,invalid-name
         ...
@@ -23,23 +24,23 @@
     The classifier can be of a type that is explicitly supported (e.g. `lightgbm.Booster`) or of any class with the
     methods `predict` and `predict_proba`.
 
     This is true for all classifiers that follow scikit-learn's API, which is described at:
     http://scikit-learn.org/stable/developers/contributing.html#apis-of-scikit-learn-objects
     """
 
-    def __init__(self, classifier: Union[Booster, ClassifierType]):
+    def __init__(self, classifier: Booster | ClassifierType):
         """
         :param classifier: An instance of trained classifier to be executed over images
         """
         self._check_classifier(classifier)
         self.classifier = classifier
 
     @staticmethod
-    def _check_classifier(classifier: Union[Booster, ClassifierType]) -> None:
+    def _check_classifier(classifier: Booster | ClassifierType) -> None:
         """Checks if the classifier is suitable."""
         if isinstance(classifier, Booster):
             return
 
         for method_name in ("predict", "predict_proba"):
             method = getattr(classifier, method_name, None)
             if not callable(method):
```

