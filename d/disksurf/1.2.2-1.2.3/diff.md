# Comparing `tmp/disksurf-1.2.2.tar.gz` & `tmp/disksurf-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disksurf-1.2.2.tar", last modified: Mon Jan 23 15:48:19 2023, max compression
+gzip compressed data, was "disksurf-1.2.3.tar", last modified: Thu Jun  1 10:01:17 2023, max compression
```

## Comparing `disksurf-1.2.2.tar` & `disksurf-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-01-23 15:48:19.190576 disksurf-1.2.2/
--rw-r--r--   0 richardteague   (501) staff       (20)     1068 2022-07-28 16:21:18.000000 disksurf-1.2.2/LICENSE
--rw-r--r--   0 richardteague   (501) staff       (20)     3728 2023-01-23 15:48:19.190478 disksurf-1.2.2/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)     3297 2022-07-28 16:21:18.000000 disksurf-1.2.2/README.md
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-01-23 15:48:19.189357 disksurf-1.2.2/disksurf/
--rw-r--r--   0 richardteague   (501) staff       (20)      103 2022-07-28 16:21:18.000000 disksurf-1.2.2/disksurf/__init__.py
--rw-r--r--   0 richardteague   (501) staff       (20)     8959 2022-07-28 16:21:18.000000 disksurf-1.2.2/disksurf/detect_peaks.py
--rw-r--r--   0 richardteague   (501) staff       (20)    57188 2023-01-09 16:42:53.000000 disksurf-1.2.2/disksurf/observation.py
--rw-r--r--   0 richardteague   (501) staff       (20)    61353 2023-01-23 15:47:41.000000 disksurf-1.2.2/disksurf/surface.py
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-01-23 15:48:19.190338 disksurf-1.2.2/disksurf.egg-info/
--rw-r--r--   0 richardteague   (501) staff       (20)     3728 2023-01-23 15:48:19.000000 disksurf-1.2.2/disksurf.egg-info/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)      275 2023-01-23 15:48:19.000000 disksurf-1.2.2/disksurf.egg-info/SOURCES.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-01-23 15:48:19.000000 disksurf-1.2.2/disksurf.egg-info/dependency_links.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       57 2023-01-23 15:48:19.000000 disksurf-1.2.2/disksurf.egg-info/requires.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        9 2023-01-23 15:48:19.000000 disksurf-1.2.2/disksurf.egg-info/top_level.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-01-23 15:48:19.190609 disksurf-1.2.2/setup.cfg
--rw-r--r--   0 richardteague   (501) staff       (20)      842 2023-01-23 15:47:46.000000 disksurf-1.2.2/setup.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-06-01 10:01:17.872152 disksurf-1.2.3/
+-rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:30:47.000000 disksurf-1.2.3/LICENSE
+-rw-r--r--   0 richardteague   (501) staff       (20)     3728 2023-06-01 10:01:17.872057 disksurf-1.2.3/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)     3297 2023-03-27 18:30:47.000000 disksurf-1.2.3/README.md
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-06-01 10:01:17.871364 disksurf-1.2.3/disksurf/
+-rw-r--r--   0 richardteague   (501) staff       (20)      103 2023-03-27 18:30:47.000000 disksurf-1.2.3/disksurf/__init__.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    58364 2023-06-01 10:00:09.000000 disksurf-1.2.3/disksurf/observation.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    61353 2023-03-27 18:30:47.000000 disksurf-1.2.3/disksurf/surface.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-06-01 10:01:17.871905 disksurf-1.2.3/disksurf.egg-info/
+-rw-r--r--   0 richardteague   (501) staff       (20)     3728 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)      250 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/SOURCES.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/dependency_links.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       57 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/requires.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        9 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/top_level.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-06-01 10:01:17.872182 disksurf-1.2.3/setup.cfg
+-rw-r--r--   0 richardteague   (501) staff       (20)      842 2023-06-01 08:52:13.000000 disksurf-1.2.3/setup.py
```

### Comparing `disksurf-1.2.2/LICENSE` & `disksurf-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.2/PKG-INFO` & `disksurf-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disksurf
-Version: 1.2.2
+Version: 1.2.3
 Summary: Infer and reproject a disk's 3D structure.
 Home-page: https://github.com/richteague/disksurf
 Author: Richard Teague
 Author-email: rteague@mit.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disksurf Version: 1.2.2 Summary: Infer and
+Metadata-Version: 2.1 Name: disksurf Version: 1.2.3 Summary: Infer and
 reproject a disk's 3D structure. Home-page: https://github.com/richteague/
 disksurf Author: Richard Teague Author-email: rteague@mit.edu License: MIT
 Classifier: Programming Language :: Python :: 3.5 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # disksurf
                             [HD163296_zeroth.png]
                       [Documentation_Status] [DOI] [DOI]
```

### Comparing `disksurf-1.2.2/README.md` & `disksurf-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.2/disksurf/observation.py` & `disksurf-1.2.3/disksurf/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .detect_peaks import detect_peaks
 from astropy.convolution import convolve, Gaussian2DKernel
+from scipy.signal import find_peaks
 import matplotlib.pyplot as plt
 from .surface import surface
 from gofish import imagecube
 import numpy as np
 
 
 class observation(imagecube):
@@ -24,15 +24,16 @@
         super().__init__(path=path, FOV=FOV, velocity_range=velocity_range)
         self.data_aligned_rotated = {}
         self.mask_keplerian = {}
 
     def get_emission_surface(self, inc, PA, vlsr, x0=0.0, y0=0.0, chans=None,
             r_min=None, r_max=None, smooth=None, nsigma=None, min_SNR=5,
             force_opposite_sides=True, force_correct_shift=False,
-            detect_peaks_kwargs=None, get_keplerian_mask_kwargs=None):
+            detect_peaks_kwargs=None, get_keplerian_mask_kwargs=None,
+            bisector=False):
         """
         Implementation of the method described in Pinte et al. (2018). There
         are several pre-processing options to help with the peak detection.
 
         Args:
             inc (float): Disk inclination in [degrees].
             PA (float): Disk position angle in [degrees].
@@ -65,14 +66,18 @@
                 to ``smooth_threshold``.
             detect_peaks_kwargs (optional[dict]): Keyword arguments passed to
                 ``detect_peaks``. If any values are duplicated from those
                 required for ``get_emission_surface``, they will be
                 overwritten.
             get_keplerian_mask_kwargs (optional[dict]): Keyward arguments passed
                 to ``get_keplerian_mask``.
+            bisector (optional[float]): If provided, use a bisector to infer the
+                location of the peaks. This value, spanning between 0 and 1,
+                specifies the relative height at which the bisector is
+                calculated.
 
         Returns:
             A ``disksurf.surface`` instance containing the extracted emission
             surface.
         """
 
         # Grab the cut down and masked data.
@@ -115,29 +120,31 @@
 
         if smooth or 0.0 > 0.0:
             kernel = np.hanning(2.0 * smooth * self.bmaj / self.dpix)
             kernel /= np.sum(kernel)
         else:
             kernel = None
 
-        # Find all the peaks.
+        # Find all the peaks. Here we select between typical peak finding and
+        # a bisector measurement.
 
         if self.verbose:
             print("Detecting peaks...")
         _surf = self._detect_peaks(data=np.where(mask, data, 0.0),
                                    inc=inc,
                                    r_min=r_min,
                                    r_max=r_max,
                                    vlsr=vlsr,
                                    chans=chans,
                                    kernel=kernel,
                                    min_SNR=min_SNR,
                                    detect_peaks_kwargs=detect_peaks_kwargs,
                                    force_opposite_sides=force_opposite_sides,
-                                   force_correct_shift=force_correct_shift)
+                                   force_correct_shift=force_correct_shift,
+                                   bisector=bisector)
         if self.verbose:
             print("Done!")
         return surface(*_surf,
                        chans=chans,
                        rms=self.estimate_RMS(),
                        x0=x0,
                        y0=y0,
@@ -591,19 +598,19 @@
             if self.verbose:
                 print("Rotating data cube...")
             data = observation._rotate_image(data, PA)
         return data
 
     def _detect_peaks(self, data, inc, r_min, r_max, vlsr, chans, min_SNR=5.0,
             kernel=None, return_back=True, detect_peaks_kwargs=None,
-            force_opposite_sides=True, force_correct_shift=True):
+            force_opposite_sides=True, force_correct_shift=True,
+            bisector=False):
         """Wrapper for `detect_peaks.py`."""
 
         inc_rad = np.radians(inc)
-        detect_peaks_kwargs = detect_peaks_kwargs or {}
 
         # Infer the correct range in the x direction.
 
         x_idx_max = abs(self.xaxis + r_max).argmin() + 1
         x_idx_min = abs(self.xaxis - r_max).argmin()
         assert x_idx_min < x_idx_max
 
@@ -616,14 +623,20 @@
 
         # Estimate the noise to remove low SNR pixels.
 
         if min_SNR is not None:
             min_Inu = min_SNR * self.estimate_RMS()
         else:
             min_Inu = -1e10
+        min_difference = -self.estimate_RMS()
+
+        # Minimum distance between the peaks. 
+
+        detect_peaks_kw = detect_peaks_kwargs or {}
+        distance = detect_peaks_kw.pop('distance', 0.5 * self.bmaj / self.dpix)
 
         # Loop through each channel, then each vertical pixel column to extract
         # the peaks.
 
         _surface = []
         for c_idx in range(data.shape[0]):
 
@@ -633,15 +646,14 @@
             c_idx_tot = c_idx + chans.min()
             if not any([ct[0] <= c_idx_tot <= ct[1] for ct in chans]):
                 continue
 
             for x_idx in range(x_idx_min, x_idx_max):
 
                 x_c = self.xaxis[x_idx]
-                mpd = detect_peaks_kwargs.get('mpd', 0.05 * abs(x_c))
                 v = self.velax[c_idx_tot]
 
                 try:
 
                     # Grab the appropriate column of pixels and optionally
                     # smooth them with a Hanning convolution.
 
@@ -651,26 +663,38 @@
                         cut_b = np.convolve(cut[::-1], kernel, mode='same')
                         cut = np.mean([cut_a, cut_b[::-1]], axis=0)
 
                     # Returns an array of all the peaks found in the cut and
                     # sort them into order of increasing intensity. Then split
                     # these into those above and below the major axis.
 
-                    y_idx = detect_peaks(cut, mpd=mpd, **detect_peaks_kwargs)
-                    y_idx += y_idx_min
-                    y_idx = y_idx[data[c_idx, y_idx, x_idx].argsort()]
-
-                    # Check that the two peaks have a minimum SNR value.
-
-                    if min(data[c_idx, y_idx[-2:], x_idx]) < min_Inu:
-                        raise ValueError("Out of bounds (RMS).")
-
+                    if bisector:
+                        intersection = -np.abs(cut - bisector * np.nanmax(cut))
+                        y_idx, props = find_peaks(x=intersection,
+                                                  distance=distance,
+                                                  height=min_difference)
+                        
+                        # Fail if there are more than four peaks. 
+
+                        if len(y_idx) != 4:
+                            raise ValueError("More than four peaks detected.")
+
+                        y_idx = np.mean([y_idx[1:], y_idx[:-1]], axis=0)
+                        y_idx = y_idx.astype('int')[[0, -1]]
+
+                    else:
+                        y_idx, props = find_peaks(x=cut,
+                                                  distance=distance,
+                                                  height=min_Inu)
+                        y_idx = y_idx[np.argsort(props['peak_heights'])]
+                        
                     # Reorder the points so the further side (_f) is a larger
                     # offset from the disk major axis.
 
+                    y_idx += y_idx_min
                     y_n, y_f = sorted(self.yaxis[y_idx[-2:]])
                     if abs(y_n) > abs(y_f):
                         y_f, y_n = y_n, y_f
 
                     # Remove points that are on the same side of the major
                     # axis of the disk. This may remove poinst in the outer
                     # disk, but that's more conservative anyway. There is the
```

### Comparing `disksurf-1.2.2/disksurf/surface.py` & `disksurf-1.2.3/disksurf/surface.py`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.2/disksurf.egg-info/PKG-INFO` & `disksurf-1.2.3/disksurf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disksurf
-Version: 1.2.2
+Version: 1.2.3
 Summary: Infer and reproject a disk's 3D structure.
 Home-page: https://github.com/richteague/disksurf
 Author: Richard Teague
 Author-email: rteague@mit.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disksurf Version: 1.2.2 Summary: Infer and
+Metadata-Version: 2.1 Name: disksurf Version: 1.2.3 Summary: Infer and
 reproject a disk's 3D structure. Home-page: https://github.com/richteague/
 disksurf Author: Richard Teague Author-email: rteague@mit.edu License: MIT
 Classifier: Programming Language :: Python :: 3.5 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # disksurf
                             [HD163296_zeroth.png]
                       [Documentation_Status] [DOI] [DOI]
```

### Comparing `disksurf-1.2.2/setup.py` & `disksurf-1.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="disksurf",
-    version="1.2.2",
+    version="1.2.3",
     author="Richard Teague",
     author_email="rteague@mit.edu",
     description=("Infer and reproject a disk's 3D structure."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/richteague/disksurf",
     packages=["disksurf"],
```

