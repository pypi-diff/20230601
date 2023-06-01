# Comparing `tmp/NanoComp-1.9.1.tar.gz` & `tmp/NanoComp-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NanoComp-1.9.1.tar", last modified: Mon Sep  2 07:54:31 2019, max compression
+gzip compressed data, was "dist/NanoComp-1.9.2.tar", last modified: Wed Sep 25 05:26:53 2019, max compression
```

## Comparing `NanoComp-1.9.1.tar` & `NanoComp-1.9.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-09-02 07:54:31.000000 NanoComp-1.9.1/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       42 2019-02-19 09:59:02.000000 NanoComp-1.9.1/MANIFEST.in
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-09-02 07:54:31.000000 NanoComp-1.9.1/NanoComp.egg-info/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     5955 2019-09-02 07:54:30.000000 NanoComp-1.9.1/NanoComp.egg-info/PKG-INFO
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      352 2019-09-02 07:54:30.000000 NanoComp-1.9.1/NanoComp.egg-info/SOURCES.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        1 2019-09-02 07:54:30.000000 NanoComp-1.9.1/NanoComp.egg-info/dependency_links.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       53 2019-09-02 07:54:30.000000 NanoComp-1.9.1/NanoComp.egg-info/entry_points.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      122 2019-09-02 07:54:30.000000 NanoComp-1.9.1/NanoComp.egg-info/requires.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       17 2019-09-02 07:54:30.000000 NanoComp-1.9.1/NanoComp.egg-info/top_level.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     5955 2019-09-02 07:54:31.000000 NanoComp-1.9.1/PKG-INFO
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     4438 2019-03-28 15:42:11.000000 NanoComp-1.9.1/README.md
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-09-02 07:54:31.000000 NanoComp-1.9.1/nanocomp/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     6926 2019-07-09 09:05:32.000000 NanoComp-1.9.1/nanocomp/NanoComp.py
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        0 2019-02-19 09:59:02.000000 NanoComp-1.9.1/nanocomp/__init__.py
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)    14273 2019-08-30 12:06:13.000000 NanoComp-1.9.1/nanocomp/compplots.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)    10806 2019-06-20 08:03:25.000000 NanoComp-1.9.1/nanocomp/utils.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)       22 2019-08-30 13:45:39.000000 NanoComp-1.9.1/nanocomp/version.py
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-09-02 07:54:31.000000 NanoComp-1.9.1/scripts/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      670 2019-02-19 09:59:02.000000 NanoComp-1.9.1/scripts/test.sh
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       70 2019-09-02 07:54:31.000000 NanoComp-1.9.1/setup.cfg
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1817 2019-06-20 07:38:17.000000 NanoComp-1.9.1/setup.py
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-09-25 05:26:53.000000 NanoComp-1.9.2/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       42 2019-02-19 09:59:02.000000 NanoComp-1.9.2/MANIFEST.in
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-09-25 05:26:53.000000 NanoComp-1.9.2/NanoComp.egg-info/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     5955 2019-09-25 05:26:53.000000 NanoComp-1.9.2/NanoComp.egg-info/PKG-INFO
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      390 2019-09-25 05:26:53.000000 NanoComp-1.9.2/NanoComp.egg-info/SOURCES.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        1 2019-09-25 05:26:53.000000 NanoComp-1.9.2/NanoComp.egg-info/dependency_links.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       53 2019-09-25 05:26:53.000000 NanoComp-1.9.2/NanoComp.egg-info/entry_points.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      122 2019-09-25 05:26:53.000000 NanoComp-1.9.2/NanoComp.egg-info/requires.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       17 2019-09-25 05:26:53.000000 NanoComp-1.9.2/NanoComp.egg-info/top_level.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     5955 2019-09-25 05:26:53.000000 NanoComp-1.9.2/PKG-INFO
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     4438 2019-03-28 15:42:11.000000 NanoComp-1.9.2/README.md
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-09-25 05:26:53.000000 NanoComp-1.9.2/nanocomp/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     6926 2019-07-09 09:05:32.000000 NanoComp-1.9.2/nanocomp/NanoComp.py
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        0 2019-02-19 09:59:02.000000 NanoComp-1.9.2/nanocomp/__init__.py
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)    14289 2019-09-24 12:10:19.000000 NanoComp-1.9.2/nanocomp/compplots.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)    10806 2019-06-20 08:03:25.000000 NanoComp-1.9.2/nanocomp/utils.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)       22 2019-09-24 12:40:02.000000 NanoComp-1.9.2/nanocomp/version.py
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-09-25 05:26:53.000000 NanoComp-1.9.2/scripts/
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1231 2019-09-09 05:40:09.000000 NanoComp-1.9.2/scripts/get_cumulative_yield_table.py
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      670 2019-02-19 09:59:02.000000 NanoComp-1.9.2/scripts/test.sh
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       70 2019-09-25 05:26:53.000000 NanoComp-1.9.2/setup.cfg
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1817 2019-06-20 07:38:17.000000 NanoComp-1.9.2/setup.py
```

### Comparing `NanoComp-1.9.1/NanoComp.egg-info/PKG-INFO` & `NanoComp-1.9.2/NanoComp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NanoComp
-Version: 1.9.1
+Version: 1.9.2
 Summary: Comparing runs of Oxford Nanopore sequencing data and alignments
 Home-page: https://github.com/wdecoster/NanoComp
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description: # NanoComp
```

### Comparing `NanoComp-1.9.1/PKG-INFO` & `NanoComp-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NanoComp
-Version: 1.9.1
+Version: 1.9.2
 Summary: Comparing runs of Oxford Nanopore sequencing data and alignments
 Home-page: https://github.com/wdecoster/NanoComp
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description: # NanoComp
```

### Comparing `NanoComp-1.9.1/README.md` & `NanoComp-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `NanoComp-1.9.1/nanocomp/NanoComp.py` & `NanoComp-1.9.2/nanocomp/NanoComp.py`

 * *Files identical despite different names*

### Comparing `NanoComp-1.9.1/nanocomp/compplots.py` & `NanoComp-1.9.2/nanocomp/compplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,26 +225,26 @@
                 title="Histogram of read lengths")
     hist.html, hist.fig = plot_overlay_histogram(df, palette, title=hist.title)
     hist.save()
 
     hist_norm = Plot(path=path + "NanoComp_OverlayHistogram_Normalized.html",
                      title="Normalized histogram of read lengths")
     hist_norm.html, hist_norm.fig = plot_overlay_histogram(
-        df, palette, title=hist_norm.title, histnorm="probability")
+        df, palette, title=hist_norm.title, histnorm="probability density")
     hist_norm.save()
 
     log_hist = Plot(path=path + "NanoComp_OverlayLogHistogram.html",
                     title="Histogram of log transformed read lengths")
     log_hist.html, log_hist.fig = plot_log_histogram(df, palette, title=log_hist.title)
     log_hist.save()
 
     log_hist_norm = Plot(path=path + "NanoComp_OverlayLogHistogram_Normalized.html",
                          title="Normalized histogram of log transformed read lengths")
     log_hist_norm.html, log_hist_norm.fig = plot_log_histogram(
-        df, palette, title=log_hist_norm.title, histnorm="probability")
+        df, palette, title=log_hist_norm.title, histnorm="probability density")
     log_hist_norm.save()
 
     return [hist, hist_norm, log_hist, log_hist_norm]
 
 
 def plot_overlay_histogram(df, palette, title, histnorm=""):
     data = []
```

### Comparing `NanoComp-1.9.1/nanocomp/utils.py` & `NanoComp-1.9.2/nanocomp/utils.py`

 * *Files identical despite different names*

### Comparing `NanoComp-1.9.1/scripts/test.sh` & `NanoComp-1.9.2/scripts/test.sh`

 * *Files identical despite different names*

### Comparing `NanoComp-1.9.1/setup.py` & `NanoComp-1.9.2/setup.py`

 * *Files identical despite different names*

