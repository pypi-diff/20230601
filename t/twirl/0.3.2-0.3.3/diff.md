# Comparing `tmp/twirl-0.3.2.tar.gz` & `tmp/twirl-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twirl-0.3.2.tar", max compression
+gzip compressed data, was "twirl-0.3.3.tar", max compression
```

## Comparing `twirl-0.3.2.tar` & `twirl-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4918 2023-05-16 17:00:41.638710 twirl-0.3.2/README.md
--rw-r--r--   0        0        0     2902 2023-05-16 17:00:41.646710 twirl-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4126 2023-05-16 17:00:41.646710 twirl-0.3.2/twirl/__init__.py
--rw-r--r--   0        0        0     3535 2023-05-16 17:00:41.646710 twirl-0.3.2/twirl/geometry.py
--rw-r--r--   0        0        0     3520 2023-05-16 17:00:41.646710 twirl-0.3.2/twirl/match.py
--rw-r--r--   0        0        0     2145 2023-05-16 17:00:41.646710 twirl-0.3.2/twirl/quads.py
--rw-r--r--   0        0        0     2174 2023-05-16 17:00:41.646710 twirl-0.3.2/twirl/triangles.py
--rw-r--r--   0        0        0     5981 1970-01-01 00:00:00.000000 twirl-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     5037 2023-06-01 13:52:02.904590 twirl-0.3.3/README.md
+-rw-r--r--   0        0        0     2902 2023-06-01 13:52:02.912590 twirl-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5151 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/__init__.py
+-rw-r--r--   0        0        0     3535 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/geometry.py
+-rw-r--r--   0        0        0     3520 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/match.py
+-rw-r--r--   0        0        0     2145 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/quads.py
+-rw-r--r--   0        0        0     2174 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/triangles.py
+-rw-r--r--   0        0        0     6100 1970-01-01 00:00:00.000000 twirl-0.3.3/PKG-INFO
```

### Comparing `twirl-0.3.2/README.md` & `twirl-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -150,7 +150,9 @@
 This package has made use of the algorithm from
 
 Lang, D. et al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary Astronomical Images_. The Astronomical Journal, 139(5), pp.1782–1800. [doi:10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-6256/139/5/1782).
 
 implemented in
 
 Garcia, L. J. et al. (2022). prose: a Python framework for modular astronomical images processing. MNRAS, vol. 509, no. 4, pp. 4817–4828, 2022. [doi:10.1093/mnras/stab3113](https://academic.oup.com/mnras/article-abstract/509/4/4817/6414007).
+
+See this [documentation page](https://twirl.readthedocs.io/en/latest/md/acknowledgement.html) for the BibTeX entries.
```

#### html2text {}

```diff
@@ -50,8 +50,10 @@
 Acknowledgements This package has made use of the algorithm from Lang, D. et
 al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary
 Astronomical Images_. The Astronomical Journal, 139(5), pp.1782â1800. [doi:
 10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-
 6256/139/5/1782). implemented in Garcia, L. J. et al. (2022). prose: a Python
 framework for modular astronomical images processing. MNRAS, vol. 509, no. 4,
 pp. 4817â4828, 2022. [doi:10.1093/mnras/stab3113](https://academic.oup.com/
-mnras/article-abstract/509/4/4817/6414007).
+mnras/article-abstract/509/4/4817/6414007). See this [documentation page]
+(https://twirl.readthedocs.io/en/latest/md/acknowledgement.html) for the BibTeX
+entries.
```

### Comparing `twirl-0.3.2/pyproject.toml` & `twirl-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twirl"
-version = "0.3.2"
+version = "0.3.3"
 description = "Astrometric plate solving in Python"
 authors = ["Lionel J. Garcia <lionel_garcia@live.fr>"]
 maintainers = [
   "Lionel J. Garcia <lionel_garcia@live.fr>",
   "Michael J. Roberts <michael@observerly.com>",
 ]
 license = "MIT"
```

### Comparing `twirl-0.3.2/twirl/__init__.py` & `twirl-0.3.3/twirl/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from typing import Tuple, Union
 
+import astropy
 import astropy.units as u
 import numpy as np
 from astropy.coordinates import SkyCoord
 from astropy.units import Quantity
-from astropy.wcs.utils import fit_wcs_from_points
+from astropy.wcs.utils import WCS, fit_wcs_from_points
+from skimage.measure import label, regionprops
 
 from twirl.geometry import pad
 from twirl.match import cross_match, find_transform, get_transform_matrix
 
 
 def compute_wcs(
     pixel_coords: np.ndarray,
     radecs: np.ndarray,
     tolerance: int = 5,
     asterism=4,
     min_match=None,
-):
+) -> WCS:
     """
     Compute the WCS solution for an image given pixel coordinates and some unordered RA-DEC values.
 
     Parameters
     ----------
     pixel_coords : np.ndarray
         Pixel coordinates of the sources in the image, shape (n, 2)
@@ -125,7 +127,34 @@
             f"ra BETWEEN {ra-ra_fov/2} AND {ra+ra_fov/2} AND "
             f"dec BETWEEN {dec-dec_fov/2} AND {dec+dec_fov/2} "
             "order by phot_g_mean_mag"
         )
 
     table = job.get_results()
     return np.array([table["ra"].value.data, table["dec"].value.data]).T
+
+
+def find_peaks(data: np.ndarray, threshold: float = 2.0) -> np.ndarray:
+    """
+    Find the coordinates of the peaks in a 2D array.
+
+    Parameters
+    ----------
+    data : np.ndarray
+        The 2D array to search for peaks.
+    threshold : float, optional
+        The threshold (in unit of image standard deviation) above which a pixel is considered
+        part of a peak, i.e.
+        The default is 2.0.
+
+    Returns
+    -------
+    np.ndarray
+        An array of shape (N, 2) containing the (x, y) coordinates of the N peaks
+        found in the input array. The peaks are sorted by decreasing flux.
+    """
+    threshold = threshold * np.nanstd(data) + np.nanmedian(data)
+    regions = regionprops(label(data > threshold), data)
+    coordinates = np.array([region.weighted_centroid[::-1] for region in regions])
+    fluxes = np.array([np.sum(region.intensity_image) for region in regions])
+
+    return coordinates[np.argsort(fluxes)[::-1]]
```

### Comparing `twirl-0.3.2/twirl/geometry.py` & `twirl-0.3.3/twirl/geometry.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.2/twirl/match.py` & `twirl-0.3.3/twirl/match.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.2/twirl/quads.py` & `twirl-0.3.3/twirl/quads.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.2/twirl/triangles.py` & `twirl-0.3.3/twirl/triangles.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.2/PKG-INFO` & `twirl-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twirl
-Version: 0.3.2
+Version: 0.3.3
 Summary: Astrometric plate solving in Python
 Home-page: https://twirl.readthedocs.io
 License: MIT
 Keywords: astronomy,astrometry,plate-solving
 Author: Lionel J. Garcia
 Author-email: lionel_garcia@live.fr
 Maintainer: Lionel J. Garcia
@@ -180,7 +180,9 @@
 
 Lang, D. et al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary Astronomical Images_. The Astronomical Journal, 139(5), pp.1782–1800. [doi:10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-6256/139/5/1782).
 
 implemented in
 
 Garcia, L. J. et al. (2022). prose: a Python framework for modular astronomical images processing. MNRAS, vol. 509, no. 4, pp. 4817–4828, 2022. [doi:10.1093/mnras/stab3113](https://academic.oup.com/mnras/article-abstract/509/4/4817/6414007).
 
+See this [documentation page](https://twirl.readthedocs.io/en/latest/md/acknowledgement.html) for the BibTeX entries.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twirl Version: 0.3.2 Summary: Astrometric plate
+Metadata-Version: 2.1 Name: twirl Version: 0.3.3 Summary: Astrometric plate
 solving in Python Home-page: https://twirl.readthedocs.io License: MIT
 Keywords: astronomy,astrometry,plate-solving Author: Lionel J. Garcia Author-
 email: lionel_garcia@live.fr Maintainer: Lionel J. Garcia Maintainer-email:
 lionel_garcia@live.fr Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -64,8 +64,10 @@
 Acknowledgements This package has made use of the algorithm from Lang, D. et
 al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary
 Astronomical Images_. The Astronomical Journal, 139(5), pp.1782â1800. [doi:
 10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-
 6256/139/5/1782). implemented in Garcia, L. J. et al. (2022). prose: a Python
 framework for modular astronomical images processing. MNRAS, vol. 509, no. 4,
 pp. 4817â4828, 2022. [doi:10.1093/mnras/stab3113](https://academic.oup.com/
-mnras/article-abstract/509/4/4817/6414007).
+mnras/article-abstract/509/4/4817/6414007). See this [documentation page]
+(https://twirl.readthedocs.io/en/latest/md/acknowledgement.html) for the BibTeX
+entries.
```

