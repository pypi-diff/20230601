# Comparing `tmp/astro-elk-0.8.tar.gz` & `tmp/astro-elk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-elk-0.8.tar", last modified: Tue May 16 00:35:37 2023, max compression
+gzip compressed data, was "astro-elk-0.9.tar", last modified: Thu Jun  1 01:46:21 2023, max compression
```

## Comparing `astro-elk-0.8.tar` & `astro-elk-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:35:37.477417 astro-elk-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-16 00:35:37.477417 astro-elk-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-16 00:35:26.000000 astro-elk-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:35:37.473417 astro-elk-0.8/astro_elk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-16 00:35:37.000000 astro-elk-0.8/astro_elk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-16 00:35:37.000000 astro-elk-0.8/astro_elk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:35:37.000000 astro-elk-0.8/astro_elk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-16 00:35:37.000000 astro-elk-0.8/astro_elk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 00:35:37.000000 astro-elk-0.8/astro_elk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:35:37.477417 astro-elk-0.8/elk/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 00:35:26.000000 astro-elk-0.8/elk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 00:35:26.000000 astro-elk-0.8/elk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-05-16 00:35:26.000000 astro-elk-0.8/elk/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-16 00:35:26.000000 astro-elk-0.8/elk/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-16 00:35:26.000000 astro-elk-0.8/elk/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-16 00:35:26.000000 astro-elk-0.8/elk/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-16 00:35:26.000000 astro-elk-0.8/elk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 00:35:37.477417 astro-elk-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-16 00:35:26.000000 astro-elk-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:46:21.925234 astro-elk-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-01 01:46:21.925234 astro-elk-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-01 01:46:10.000000 astro-elk-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:46:21.925234 astro-elk-0.9/astro_elk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-01 01:46:21.000000 astro-elk-0.9/astro_elk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-01 01:46:21.000000 astro-elk-0.9/astro_elk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 01:46:21.000000 astro-elk-0.9/astro_elk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 01:46:21.000000 astro-elk-0.9/astro_elk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 01:46:21.000000 astro-elk-0.9/astro_elk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:46:21.925234 astro-elk-0.9/elk/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 01:46:10.000000 astro-elk-0.9/elk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 01:46:10.000000 astro-elk-0.9/elk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-06-01 01:46:10.000000 astro-elk-0.9/elk/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-06-01 01:46:10.000000 astro-elk-0.9/elk/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-01 01:46:10.000000 astro-elk-0.9/elk/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-06-01 01:46:10.000000 astro-elk-0.9/elk/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-01 01:46:10.000000 astro-elk-0.9/elk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-01 01:46:21.925234 astro-elk-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-01 01:46:10.000000 astro-elk-0.9/setup.py
```

### Comparing `astro-elk-0.8/PKG-INFO` & `astro-elk-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-elk
-Version: 0.8
+Version: 0.9
 Summary: This python package computes, and corrects ensemble light curves for TESS pixels within a specified aperature, from TESS FFI data.
 Home-page: https://github.com/tobin-wainer/TESS_Cluster_Project/
 Author: Tobin Wainer, Tom Wagg
 Author-email: tobinw@uw.edu
 License: MIT
 Platform: UNKNOWN
 Provides: elk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astro-elk Version: 0.8 Summary: This python package
+Metadata-Version: 2.1 Name: astro-elk Version: 0.9 Summary: This python package
 computes, and corrects ensemble light curves for TESS pixels within a specified
 aperature, from TESS FFI data. Home-page: https://github.com/tobin-wainer/
 TESS_Cluster_Project/ Author: Tobin Wainer, Tom Wagg Author-email:
 tobinw@uw.edu License: MIT Platform: UNKNOWN Provides: elk Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Provides-Extra: test Provides-
 Extra: docs
    src="https://raw.githubusercontent.com/tobin-wainer/elk/main/docs/_static/
```

### Comparing `astro-elk-0.8/README.md` & `astro-elk-0.9/README.md`

 * *Files identical despite different names*

### Comparing `astro-elk-0.8/astro_elk.egg-info/PKG-INFO` & `astro-elk-0.9/astro_elk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-elk
-Version: 0.8
+Version: 0.9
 Summary: This python package computes, and corrects ensemble light curves for TESS pixels within a specified aperature, from TESS FFI data.
 Home-page: https://github.com/tobin-wainer/TESS_Cluster_Project/
 Author: Tobin Wainer, Tom Wagg
 Author-email: tobinw@uw.edu
 License: MIT
 Platform: UNKNOWN
 Provides: elk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astro-elk Version: 0.8 Summary: This python package
+Metadata-Version: 2.1 Name: astro-elk Version: 0.9 Summary: This python package
 computes, and corrects ensemble light curves for TESS pixels within a specified
 aperature, from TESS FFI data. Home-page: https://github.com/tobin-wainer/
 TESS_Cluster_Project/ Author: Tobin Wainer, Tom Wagg Author-email:
 tobinw@uw.edu License: MIT Platform: UNKNOWN Provides: elk Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Provides-Extra: test Provides-
 Extra: docs
    src="https://raw.githubusercontent.com/tobin-wainer/elk/main/docs/_static/
```

### Comparing `astro-elk-0.8/elk/ensemble.py` & `astro-elk-0.9/elk/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,17 +433,20 @@
                       'lc_lens': [str([len(lc.corrected_lc) if lc is not None else -99 for lc in self.lcs])]})
 
 
 def from_fits(filepath, existing_class=None, **kwargs):
     # if an existing class is not provided then create a new blank one
     if existing_class is None:
         # work out what the output path is based on the filepath input
-        output_path = os.path.join(*filepath.split("/")[:-2])
-        if filepath[0] == "/":
-            output_path = "/" + output_path
+        if len(filepath.split("/")) == 2:
+            output_path = "."
+        else:
+            output_path = os.path.join(*filepath.split("/")[:-2])
+            if filepath[0] == "/":
+                output_path = "/" + output_path
         new_ecl = EnsembleLC(identifier="", radius=None, cluster_age=None, output_path=output_path, **kwargs)
     else:
         new_ecl = existing_class
 
     # open up the fits file and load in the information
     with fits.open(filepath) as hdul:
         details = hdul[0]
```

### Comparing `astro-elk-0.8/elk/lightcurve.py` & `astro-elk-0.9/elk/lightcurve.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.8/elk/plot.py` & `astro-elk-0.9/elk/plot.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.8/elk/stats.py` & `astro-elk-0.9/elk/stats.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.8/elk/utils.py` & `astro-elk-0.9/elk/utils.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.8/setup.cfg` & `astro-elk-0.9/setup.cfg`

 * *Files identical despite different names*

