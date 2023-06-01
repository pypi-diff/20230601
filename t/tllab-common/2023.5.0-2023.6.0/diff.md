# Comparing `tmp/tllab_common-2023.5.0.tar.gz` & `tmp/tllab_common-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2023.5.0.tar", max compression
+gzip compressed data, was "tllab_common-2023.6.0.tar", max compression
```

## Comparing `tllab_common-2023.5.0.tar` & `tllab_common-2023.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.5.0/LICENSE
--rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.5.0/README.md
--rw-r--r--   0        0        0      890 2023-05-15 13:29:04.713409 tllab_common-2023.5.0/pyproject.toml
--rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.5.0/tllab_common/__init__.py
--rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.5.0/tllab_common/findcells.py
--rw-r--r--   0        0        0     5262 2023-05-10 16:28:47.573261 tllab_common-2023.5.0/tllab_common/fit.py
--rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.5.0/tllab_common/misc.py
--rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.5.0/tllab_common/transform.txt
--rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.5.0/tllab_common/transforms.py
--rwxr-xr-x   0        0        0    69946 2023-05-15 13:07:41.540425 tllab_common-2023.5.0/tllab_common/wimread.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.6.0/LICENSE
+-rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.6.0/README.md
+-rw-r--r--   0        0        0      890 2023-06-01 13:11:18.291541 tllab_common-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.6.0/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.6.0/tllab_common/findcells.py
+-rw-r--r--   0        0        0     6262 2023-06-01 13:11:18.323541 tllab_common-2023.6.0/tllab_common/fit.py
+-rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.6.0/tllab_common/misc.py
+-rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.6.0/tllab_common/transform.txt
+-rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.6.0/tllab_common/transforms.py
+-rwxr-xr-x   0        0        0    69943 2023-05-16 13:02:07.073494 tllab_common-2023.6.0/tllab_common/wimread.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.6.0/PKG-INFO
```

### Comparing `tllab_common-2023.5.0/LICENSE` & `tllab_common-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.5.0/README.md` & `tllab_common-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.5.0/pyproject.toml` & `tllab_common-2023.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2023.5.0"
+version = "2023.6.0"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2023.5.0/tllab_common/findcells.py` & `tllab_common-2023.6.0/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.5.0/tllab_common/fit.py` & `tllab_common-2023.6.0/tllab_common/fit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from functools import cached_property
 from scipy.optimize import minimize, OptimizeResult
+from scipy import stats
 from abc import ABCMeta, abstractmethod
 
 
 class Fit(metaclass=ABCMeta):
     def __init__(self, x, y, w=None, log_scale=False):
         x = np.asarray(x)
         y = np.asarray(y)
@@ -78,14 +79,32 @@
     def log_likelihood(self):
         return -self.n * np.log(2 * np.pi * self.r.fun / (self.n - 1)) / 2 - (self.n - 1) / 2
 
     @property
     def bic(self):
         return self.n_p * np.log(self.n) - 2 * self.log_likelihood
 
+    def ftest(self, fit2):
+        """ returns the p-value for the hypothesis that fit2 is the better fit,
+            assuming fit2 is the fit with more free parameters
+            if the fits are swapped the p-value will be negative
+         """
+        if not np.all(self.x == fit2.x):
+            raise ValueError('Only two fits on the same data can be compared.')
+        rss1 = self.get_cost_fun()(self.p)
+        rss2 = fit2.get_cost_fun()(fit2.p)
+        swapped = np.argmin((self.n_p, fit2.n_p))
+        if (swapped and rss1 > rss2) or (not swapped and rss1 < rss2):
+            raise ValueError('The RSS of the fit with the most free parameters should be the smallest.')
+        n = self.n_p if swapped else fit2.n_p
+        dn = np.abs(self.n_p - fit2.n_p)
+        f_value = (np.abs(rss1 - rss2) / dn) / ((rss1 if swapped else rss2) / (len(self.x) - n))
+        p_value = stats.f(dn, len(self.x) - n).sf(f_value)
+        return -p_value if swapped else p_value
+
 
 class Exponential1(Fit):
     n_p = 2
     bounds = ((0, None), (0, None))
 
     @property
     def p0(self):
@@ -168,15 +187,15 @@
         ah = a.copy()
         ah[i] = a[i] * (1 + diffstep) + eps
         f = np.array(fun(ah, *args)).flatten()
         deriv[:, i] = (f - f0) / (ah[i] - a[i]) * w
 
     hesse = np.matmul(deriv.T, deriv)
 
-    if np.linalg.matrix_rank(hesse) == np.shape(hesse)[0]:
-        da = np.sqrt(chisq * np.diag(np.linalg.inv(hesse)))
-    else:
-        try:
+    try:
+        if np.linalg.matrix_rank(hesse) == np.shape(hesse)[0]:
+            da = np.sqrt(chisq * np.diag(np.linalg.inv(hesse)))
+        else:
             da = np.sqrt(chisq * np.diag(np.linalg.pinv(hesse)))
-        except Exception:
-            da = np.full_like(a, np.nan)
+    except (Exception,):
+        da = np.full_like(a, np.nan)
     return chisq, 1.96 * da, r_squared
```

### Comparing `tllab_common-2023.5.0/tllab_common/misc.py` & `tllab_common-2023.6.0/tllab_common/misc.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.5.0/tllab_common/transforms.py` & `tllab_common-2023.6.0/tllab_common/transforms.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.5.0/tllab_common/wimread.py` & `tllab_common-2023.6.0/tllab_common/wimread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1219,28 +1219,28 @@
         # TODO: make sure frame function still works when a subblock has data from more than one frame
         self.reader = czifile.CziFile(self.path)
         self.shape = tuple([self.reader.shape[self.reader.axes.index(directory_entry)] for directory_entry in 'XYCZT'])
         self.len_series = self.reader.shape[self.reader.axes.index('S')] if 'S' in self.reader.axes else 1
         filedict = {}
         for directory_entry in self.reader.filtered_subblock_directory:
             idx = self.get_index(directory_entry, self.reader.start)
-            if 'S' in self.reader.axes and self.series in range(*idx[self.reader.axes.index('S')]):
+            if 'S' not in self.reader.axes or self.series in range(*idx[self.reader.axes.index('S')]):
                 for c in range(*idx[self.reader.axes.index('C')]):
                     for z in range(*idx[self.reader.axes.index('Z')]):
                         for t in range(*idx[self.reader.axes.index('T')]):
                             if (c, z, t) in filedict:
-                                filedict[(c, z, t)].append(directory_entry)
+                                filedict[c, z, t].append(directory_entry)
                             else:
-                                filedict[(c, z, t)] = [directory_entry]
+                                filedict[c, z, t] = [directory_entry]
         x_min = min([f.start[f.axes.index('X')] for f in filedict[0, 0, 0]])
         y_min = min([f.start[f.axes.index('Y')] for f in filedict[0, 0, 0]])
         x_max = max([f.start[f.axes.index('X')] + f.shape[f.axes.index('X')] for f in filedict[0, 0, 0]])
         y_max = max([f.start[f.axes.index('Y')] + f.shape[f.axes.index('Y')] for f in filedict[0, 0, 0]])
         self.shape = (x_max - x_min, y_max - y_min) + \
-                     tuple([self.reader.shape[self.reader.axes.index(directory_entry)] for directory_entry in 'CZT'])
+                     tuple(self.reader.shape[self.reader.axes.index(directory_entry)] for directory_entry in 'CZT')
         self.filedict = filedict
         self.metadata = xmldata(untangle.parse(self.reader.metadata()))
 
         unit = {'nm': 1e9, 'µm': 1e6, 'um': 1e6, 'mm': 1e3, 'm': 1}
         for item in self.metadata['ImageDocument']['Metadata']['Scaling']['Items']['Distance']:
             if item['Id'] == 'X':
                 self.pxsize = float(item['Value']) * unit[item.get('DefaultUnitFormat', 'um')]
```

### Comparing `tllab_common-2023.5.0/PKG-INFO` & `tllab_common-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab-common
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.8,<4.0
```

