# Comparing `tmp/gocart-0.4.3.tar.gz` & `tmp/gocart-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.4.3.tar", last modified: Mon May 29 15:12:27 2023, max compression
+gzip compressed data, was "gocart-0.4.4.tar", last modified: Thu Jun  1 14:47:57 2023, max compression
```

## Comparing `gocart-0.4.3.tar` & `gocart-0.4.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 15:12:27.919148 gocart-0.4.3/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3710 2023-05-29 15:07:57.000000 gocart-0.4.3/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-29 15:07:57.000000 gocart-0.4.3/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-29 15:07:57.000000 gocart-0.4.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-05-29 15:12:27.919148 gocart-0.4.3/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5894 2023-05-29 15:07:57.000000 gocart-0.4.3/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 15:12:27.915148 gocart-0.4.3/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 15:12:27.915148 gocart-0.4.3/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4525 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 15:12:27.915148 gocart-0.4.3/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12776 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 15:12:27.915148 gocart-0.4.3/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16256 2023-05-29 15:07:57.000000 gocart-0.4.3/gocart/parsers/lvk.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 15:12:27.907148 gocart-0.4.3/gocart/resources/
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 15:12:27.915148 gocart-0.4.3/gocart/resources/plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-05-29 15:07:58.000000 gocart-0.4.3/gocart/resources/plugins/gp_template.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-29 15:07:58.000000 gocart-0.4.3/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-05-29 15:07:58.000000 gocart-0.4.3/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-29 15:07:58.000000 gocart-0.4.3/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 15:12:27.915148 gocart-0.4.3/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-05-29 15:12:27.000000 gocart-0.4.3/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-05-29 15:12:27.000000 gocart-0.4.3/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-29 15:12:27.000000 gocart-0.4.3/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-29 15:12:27.000000 gocart-0.4.3/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-29 15:11:23.000000 gocart-0.4.3/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-05-29 15:12:27.000000 gocart-0.4.3/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-29 15:12:27.000000 gocart-0.4.3/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-29 15:12:27.919148 gocart-0.4.3/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-05-29 15:07:58.000000 gocart-0.4.3/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3841 2023-06-01 14:43:19.000000 gocart-0.4.4/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-06-01 14:43:19.000000 gocart-0.4.4/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-06-01 14:43:19.000000 gocart-0.4.4/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-01 14:47:57.772820 gocart-0.4.4/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5894 2023-06-01 14:43:19.000000 gocart-0.4.4/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.768820 gocart-0.4.4/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4510 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12776 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16286 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/parsers/lvk.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.760819 gocart-0.4.4/gocart/resources/
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/gocart/resources/plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/resources/plugins/gp_template.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.768820 gocart-0.4.4/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-01 14:46:48.000000 gocart-0.4.4/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-06-01 14:47:57.772820 gocart-0.4.4/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-06-01 14:43:19.000000 gocart-0.4.4/setup.py
```

### Comparing `gocart-0.4.3/CHANGES.md` & `gocart-0.4.4/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 ## Release Notes
 
+**v0.4.4 - June 1, 2023**
+
+- **FIXED**: fix in prob calculations in flattened maps
+- **FIXED**: allowing symlinks in plugin folder
 
 **v0.4.2 - May 28, 2023**
 
 - **ENHANCEMENT**: added a `burst` filtering parameter. If set to True, burst event alerts will pass the filter, otherwise they filtered out (default).
 - **REFACTOR**: maps with `CREATOR: ligo-skymap-from-samples` now named on file as `bilby.multiorder.fits`.
 - **REFACTOR**: try, except added to listen parser. If an alert breaks the parser an ugly error message is reported, but the listener stays alive to listen to subsequent alerts.
 - **FIXED**: burst events causing headaches for filtering and map conversion. The first 'real' burst event provided the necessary alert packet and map to create a realistic unit test for the entire codebase. The code is now much more robust to busrt event alerts.
```

### Comparing `gocart-0.4.3/LICENSE` & `gocart-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/PKG-INFO` & `gocart-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.3
+Version: 0.4.4
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.3.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.4.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.4.3/README.md` & `gocart-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/advanced_settings.yaml` & `gocart-0.4.4/gocart/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/cl_utils.py` & `gocart-0.4.4/gocart/cl_utils.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.4.4/gocart/commonutils/flatten_healpix_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     tableData['PROB'] = tableData['AREA'] * tableData["PROBDENSITY"]
 
     level = ah.nside_to_level(nside)
 
     # UPSAMPLE TABLE
     # FIND THE HIGH-LEVEL PIXEL INDEXES FOR EACH UNIQ PIXEL
     # MAKE A NEW DATAFRAME WITH IPIX64, UNIQ
-    # MATCH EACH NEW UNIQ AGAIN ORIGINAL FRAME UNIQ TO GENERATE DATA FOR IPIX^$ FRAME
-    mask = tableData['NSIDE'] <= nside
+    # MATCH EACH NEW UNIQ AGAINST ORIGINAL FRAME UNIQ TO GENERATE DATA FOR IPIX^$ FRAME
+    mask = (tableData['NSIDE'] <= nside)
     upTable = tableData.loc[mask].copy()
     upTable.reset_index(inplace=True)
     this = uniq2range(nside, upTable['UNIQ'])
     upTable[f'IPIX{nside}'] = [list(range(i, j)) for i, j in zip(this[0], this[1])]
     upTable[f'UNIQLIST'] = upTable.apply(lambda x: [x['UNIQ']] * len(x[f'IPIX{nside}']), axis=1)
 
     ipixNside = np.concatenate(upTable[f'IPIX{nside}'])
@@ -101,15 +101,16 @@
 
     # DOWNSAMPLE TABLE
     mask = tableData['NSIDE'] > nside
     downTable = tableData.loc[mask].copy()
     downTable.reset_index(inplace=True)
 
     # FIND THE PIXEL INDEX AT ORDER NSIDE
-    downTable[f'IPIX{nside}'] = np.floor_divide(tableData.loc[mask, 'IPIX'], np.power(4, (tableData.loc[mask, 'LEVEL'].values - level)))
+    downTable[f'IPIX{nside}'] = np.floor_divide(downTable['IPIX'], np.power(4, (downTable['LEVEL'].values - level)))
+
     # GROUP RESULTS
     if "DISTMU" in downTable.columns:
         downTable = downTable.groupby([f'IPIX{nside}']).agg({'PROB': 'sum', 'DISTMU': 'mean', 'DISTSIGMA': 'mean', 'DISTNORM': 'mean'})
     else:
         downTable = downTable.groupby([f'IPIX{nside}']).agg({'PROB': 'sum'})
     downTable.reset_index(inplace=True)
```

### Comparing `gocart-0.4.3/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.4.4/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/convert/aitoff.py` & `gocart-0.4.4/gocart/convert/aitoff.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/convert/ascii.py` & `gocart-0.4.4/gocart/convert/ascii.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/convert/healpix2cart.py` & `gocart-0.4.4/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/default_settings.yaml` & `gocart-0.4.4/gocart/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/parsers/lvk.py` & `gocart-0.4.4/gocart/parsers/lvk.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             from os.path import expanduser
             from subprocess import Popen, PIPE, STDOUT
             home = expanduser("~")
             # GENERATE A LIST OF FILE PATHS
             pathToDirectory = home + "/.config/gocart/plugins"
             for d in os.listdir(pathToDirectory):
                 filepath = os.path.join(pathToDirectory, d)
-                if os.path.isfile(filepath) and d[:3] == "gp_":
+                if (os.path.isfile(filepath) or os.path.islink(filepath)) and d[:3] == "gp_":
                     cmd = f"""/usr/bin/env python {filepath} {alertDir}"""
                     print(f"PLUGIN: {d}")
                     try:
                         p = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=True)
                         stdout, stderr = p.communicate()
                         print(stdout.decode('utf-8'))
                         if stderr:
```

### Comparing `gocart-0.4.3/gocart/resources/plugins/gp_template.py` & `gocart-0.4.4/gocart/resources/plugins/gp_template.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/setup.cfg` & `gocart-0.4.4/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/test_settings.yaml` & `gocart-0.4.4/gocart/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart/utKit.py` & `gocart-0.4.4/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/gocart.egg-info/PKG-INFO` & `gocart-0.4.4/gocart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.3
+Version: 0.4.4
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.3.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.4.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.4.3/gocart.egg-info/SOURCES.txt` & `gocart-0.4.4/gocart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocart-0.4.3/setup.py` & `gocart-0.4.4/setup.py`

 * *Files identical despite different names*

