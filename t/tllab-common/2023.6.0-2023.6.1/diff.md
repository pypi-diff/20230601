# Comparing `tmp/tllab_common-2023.6.0.tar.gz` & `tmp/tllab_common-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2023.6.0.tar", max compression
+gzip compressed data, was "tllab_common-2023.6.1.tar", max compression
```

## Comparing `tllab_common-2023.6.0.tar` & `tllab_common-2023.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.6.0/LICENSE
--rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.6.0/README.md
--rw-r--r--   0        0        0      890 2023-06-01 13:11:18.291541 tllab_common-2023.6.0/pyproject.toml
--rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.6.0/tllab_common/__init__.py
--rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.6.0/tllab_common/findcells.py
--rw-r--r--   0        0        0     6262 2023-06-01 13:11:18.323541 tllab_common-2023.6.0/tllab_common/fit.py
--rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.6.0/tllab_common/misc.py
--rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.6.0/tllab_common/transform.txt
--rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.6.0/tllab_common/transforms.py
--rwxr-xr-x   0        0        0    69943 2023-05-16 13:02:07.073494 tllab_common-2023.6.0/tllab_common/wimread.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.6.1/LICENSE
+-rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.6.1/README.md
+-rw-r--r--   0        0        0      890 2023-06-01 13:22:00.111940 tllab_common-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.6.1/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.6.1/tllab_common/findcells.py
+-rw-r--r--   0        0        0     6333 2023-06-01 13:22:00.139940 tllab_common-2023.6.1/tllab_common/fit.py
+-rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.6.1/tllab_common/misc.py
+-rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.6.1/tllab_common/transform.txt
+-rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.6.1/tllab_common/transforms.py
+-rwxr-xr-x   0        0        0    69943 2023-05-16 13:02:07.073494 tllab_common-2023.6.1/tllab_common/wimread.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.6.1/PKG-INFO
```

### Comparing `tllab_common-2023.6.0/LICENSE` & `tllab_common-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.0/README.md` & `tllab_common-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.0/pyproject.toml` & `tllab_common-2023.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2023.6.0"
+version = "2023.6.1"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2023.6.0/tllab_common/findcells.py` & `tllab_common-2023.6.1/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.0/tllab_common/fit.py` & `tllab_common-2023.6.1/tllab_common/fit.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,33 +77,36 @@
 
     @property
     def log_likelihood(self):
         return -self.n * np.log(2 * np.pi * self.r.fun / (self.n - 1)) / 2 - (self.n - 1) / 2
 
     @property
     def bic(self):
+        """ Bayesian Information Criterion: the fit with the smallest bic should be the best fit """
         return self.n_p * np.log(self.n) - 2 * self.log_likelihood
 
     def ftest(self, fit2):
         """ returns the p-value for the hypothesis that fit2 is the better fit,
             assuming fit2 is the fit with more free parameters
-            if the fits are swapped the p-value will be negative
-         """
+            if the fits are swapped the p-value will be negative """
         if not np.all(self.x == fit2.x):
             raise ValueError('Only two fits on the same data can be compared.')
         rss1 = self.get_cost_fun()(self.p)
         rss2 = fit2.get_cost_fun()(fit2.p)
         swapped = np.argmin((self.n_p, fit2.n_p))
-        if (swapped and rss1 > rss2) or (not swapped and rss1 < rss2):
-            raise ValueError('The RSS of the fit with the most free parameters should be the smallest.')
-        n = self.n_p if swapped else fit2.n_p
-        dn = np.abs(self.n_p - fit2.n_p)
-        f_value = (np.abs(rss1 - rss2) / dn) / ((rss1 if swapped else rss2) / (len(self.x) - n))
-        p_value = stats.f(dn, len(self.x) - n).sf(f_value)
-        return -p_value if swapped else p_value
+        if swapped and rss1 > rss2:
+            return -1
+        elif not swapped and rss1 < rss2:
+            return 1
+        else:
+            n = self.n_p if swapped else fit2.n_p
+            dn = np.abs(self.n_p - fit2.n_p)
+            f_value = (np.abs(rss1 - rss2) / dn) / ((rss1 if swapped else rss2) / (len(self.x) - n))
+            p_value = stats.f(dn, len(self.x) - n).sf(f_value)
+            return -p_value if swapped else p_value
 
 
 class Exponential1(Fit):
     n_p = 2
     bounds = ((0, None), (0, None))
 
     @property
```

### Comparing `tllab_common-2023.6.0/tllab_common/misc.py` & `tllab_common-2023.6.1/tllab_common/misc.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.0/tllab_common/transforms.py` & `tllab_common-2023.6.1/tllab_common/transforms.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.0/tllab_common/wimread.py` & `tllab_common-2023.6.1/tllab_common/wimread.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.0/PKG-INFO` & `tllab_common-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab-common
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.8,<4.0
```

