# Comparing `tmp/pysatSpaceWeather-0.0.8.tar.gz` & `tmp/pysatSpaceWeather-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysatSpaceWeather-0.0.8.tar", last modified: Tue Nov 29 18:12:39 2022, max compression
+gzip compressed data, was "pysatSpaceWeather-0.0.9.tar", last modified: Thu Dec 22 03:56:48 2022, max compression
```

## Comparing `pysatSpaceWeather-0.0.8.tar` & `pysatSpaceWeather-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,40 @@
-drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-11-29 18:12:39.370808 pysatSpaceWeather-0.0.8/
-drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-11-29 18:12:39.355657 pysatSpaceWeather-0.0.8/.github/
-drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-11-29 18:12:39.357690 pysatSpaceWeather-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 aburrell  (5504) staff       (20)      674 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 aburrell  (5504) staff       (20)      762 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 aburrell  (5504) staff       (20)      419 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 aburrell  (5504) staff       (20)     1874 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/.github/pull_request_template.md
-drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-11-29 18:12:39.359714 pysatSpaceWeather-0.0.8/.github/workflows/
--rw-r--r--   0 aburrell  (5504) staff       (20)     1236 2022-11-22 19:24:31.000000 pysatSpaceWeather-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0 aburrell  (5504) staff       (20)     1835 2022-11-22 19:24:31.000000 pysatSpaceWeather-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 aburrell  (5504) staff       (20)     1355 2022-11-22 19:24:31.000000 pysatSpaceWeather-0.0.8/.github/workflows/pysat_rc.yml
--rw-r--r--   0 aburrell  (5504) staff       (20)      881 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/.gitignore
--rw-r--r--   0 aburrell  (5504) staff       (20)     1003 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/.zenodo.json
--rw-r--r--   0 aburrell  (5504) staff       (20)     3445 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/CHANGELOG.md
--rw-r--r--   0 aburrell  (5504) staff       (20)     3232 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 aburrell  (5504) staff       (20)     5883 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 aburrell  (5504) staff       (20)     1513 2020-08-19 14:24:26.000000 pysatSpaceWeather-0.0.8/LICENSE
--rw-r--r--   0 aburrell  (5504) staff       (20)      263 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/MANIFEST.in
--rw-r--r--   0 aburrell  (5504) staff       (20)     3856 2022-11-29 18:12:39.370996 pysatSpaceWeather-0.0.8/PKG-INFO
--rw-r--r--   0 aburrell  (5504) staff       (20)     2785 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/README.md
-drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-11-29 18:12:39.360920 pysatSpaceWeather-0.0.8/pysatSpaceWeather/
--rw-r--r--   0 aburrell  (5504) staff       (20)      426 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/__init__.py
-drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-11-29 18:12:39.367388 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/
--rw-r--r--   0 aburrell  (5504) staff       (20)      259 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/__init__.py
--rw-r--r--   0 aburrell  (5504) staff       (20)     9892 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/ace_epam.py
--rw-r--r--   0 aburrell  (5504) staff       (20)     6686 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/ace_mag.py
--rw-r--r--   0 aburrell  (5504) staff       (20)     6858 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/ace_sis.py
--rw-r--r--   0 aburrell  (5504) staff       (20)     6104 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/ace_swepam.py
-drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-11-29 18:12:39.370368 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/
--rw-r--r--   0 aburrell  (5504) staff       (20)      218 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/__init__.py
--rw-r--r--   0 aburrell  (5504) staff       (20)    13512 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/ace.py
--rw-r--r--   0 aburrell  (5504) staff       (20)     1568 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/dst.py
--rw-r--r--   0 aburrell  (5504) staff       (20)    18786 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/f107.py
--rw-r--r--   0 aburrell  (5504) staff       (20)      789 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/general.py
--rw-r--r--   0 aburrell  (5504) staff       (20)    26162 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/kp_ap.py
--rw-r--r--   0 aburrell  (5504) staff       (20)    11003 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/sw_dst.py
--rw-r--r--   0 aburrell  (5504) staff       (20)    29045 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/sw_f107.py
--rw-r--r--   0 aburrell  (5504) staff       (20)    25955 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/sw_kp.py
--rw-r--r--   0 aburrell  (5504) staff       (20)        6 2022-11-29 18:11:24.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather/version.txt
-drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-11-29 18:12:39.363366 pysatSpaceWeather-0.0.8/pysatSpaceWeather.egg-info/
--rw-r--r--   0 aburrell  (5504) staff       (20)     3856 2022-11-29 18:12:38.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather.egg-info/PKG-INFO
--rw-r--r--   0 aburrell  (5504) staff       (20)     1307 2022-11-29 18:12:39.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather.egg-info/SOURCES.txt
--rw-r--r--   0 aburrell  (5504) staff       (20)        1 2022-11-29 18:12:38.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather.egg-info/dependency_links.txt
--rw-r--r--   0 aburrell  (5504) staff       (20)        1 2022-11-29 18:12:38.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather.egg-info/not-zip-safe
--rw-r--r--   0 aburrell  (5504) staff       (20)       53 2022-11-29 18:12:38.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather.egg-info/requires.txt
--rw-r--r--   0 aburrell  (5504) staff       (20)       18 2022-11-29 18:12:38.000000 pysatSpaceWeather-0.0.8/pysatSpaceWeather.egg-info/top_level.txt
--rw-r--r--   0 aburrell  (5504) staff       (20)       62 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/requirements.txt
--rw-r--r--   0 aburrell  (5504) staff       (20)     1602 2022-11-29 18:12:39.371929 pysatSpaceWeather-0.0.8/setup.cfg
--rw-r--r--   0 aburrell  (5504) staff       (20)      374 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/setup.py
--rw-r--r--   0 aburrell  (5504) staff       (20)      113 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.8/test_requirements.txt
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-12-22 03:56:48.663344 pysatSpaceWeather-0.0.9/
+-rw-r--r--   0 aburrell  (5504) staff       (20)     3827 2022-12-22 03:56:27.000000 pysatSpaceWeather-0.0.9/CHANGELOG.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)     3232 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)     5883 2022-12-20 17:48:59.000000 pysatSpaceWeather-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1513 2020-08-19 14:24:26.000000 pysatSpaceWeather-0.0.9/LICENSE
+-rw-r--r--   0 aburrell  (5504) staff       (20)      263 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/MANIFEST.in
+-rw-r--r--   0 aburrell  (5504) staff       (20)     3906 2022-12-22 03:56:48.663540 pysatSpaceWeather-0.0.9/PKG-INFO
+-rw-r--r--   0 aburrell  (5504) staff       (20)     2785 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/README.md
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-12-22 03:56:48.645507 pysatSpaceWeather-0.0.9/pysatSpaceWeather/
+-rw-r--r--   0 aburrell  (5504) staff       (20)      426 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/__init__.py
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-12-22 03:56:48.657472 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/
+-rw-r--r--   0 aburrell  (5504) staff       (20)      276 2022-12-22 03:56:27.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/__init__.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     9892 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/ace_epam.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     6686 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/ace_mag.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     6858 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/ace_sis.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     6104 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/ace_swepam.py
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-12-22 03:56:48.662920 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/
+-rw-r--r--   0 aburrell  (5504) staff       (20)      411 2022-12-22 03:56:27.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/__init__.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    13512 2022-12-20 17:48:59.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/ace.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1568 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/dst.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    18786 2022-12-20 17:48:59.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/f107.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)      789 2022-12-20 17:48:59.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/general.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    26162 2022-12-20 17:48:59.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/kp_ap.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     6659 2022-12-22 03:56:27.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/lisird.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    11003 2022-11-29 19:07:02.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/sw_dst.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    27784 2022-12-22 03:56:27.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/sw_f107.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    26532 2022-12-22 03:56:27.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/sw_kp.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    11476 2022-12-22 03:56:27.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/sw_mgii.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)        6 2022-12-22 03:56:27.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather/version.txt
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2022-12-22 03:56:48.648909 pysatSpaceWeather-0.0.9/pysatSpaceWeather.egg-info/
+-rw-r--r--   0 aburrell  (5504) staff       (20)     3906 2022-12-22 03:56:48.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather.egg-info/PKG-INFO
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1140 2022-12-22 03:56:48.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather.egg-info/SOURCES.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)        1 2022-12-22 03:56:48.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather.egg-info/dependency_links.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)        1 2022-12-22 03:56:48.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather.egg-info/not-zip-safe
+-rw-r--r--   0 aburrell  (5504) staff       (20)       53 2022-12-22 03:56:48.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather.egg-info/requires.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)       18 2022-12-22 03:56:48.000000 pysatSpaceWeather-0.0.9/pysatSpaceWeather.egg-info/top_level.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)       62 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/requirements.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1641 2022-12-22 03:56:48.664501 pysatSpaceWeather-0.0.9/setup.cfg
+-rw-r--r--   0 aburrell  (5504) staff       (20)      374 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/setup.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)      113 2022-11-16 16:36:19.000000 pysatSpaceWeather-0.0.9/test_requirements.txt
```

### Comparing `pysatSpaceWeather-0.0.8/CHANGELOG.md` & `pysatSpaceWeather-0.0.9/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 Change Log
 ==========
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](https://semver.org/).
 
+[0.0.9] - 2022-12-21
+--------------------
+* Deprecations
+  * Added warnings for the F10.7 and Kp tags that load data belonging in
+  their own Instruments
+* Enhancements
+  * Added tests for Python 3.6.8, continuing support for older systems
+  * Added a cron job for testing
+  * Added an instrument for the LASP MgII core-to-wing index
+  * Added functions for general LISIRD downloads
+
 [0.0.8] - 2022-11-29
 --------------------
 * Bugs
-   * Fixed F10.7 prelim and daily metadata to allow the fill value to keep the
-     same type as the data
+  * Fixed F10.7 prelim and daily metadata to allow the fill value to keep the
+    same type as the data
 * Maintenance
   * Updated the GitHub action version numbers
   * Updated syntax for pysat instrument testing suite
   * Remove deprecated pytest syntax (backwards support for nose)
   * Removed deprecated pandas syntax (iteritems)
   * Added Github action workflow using the latest pysat RC
   * Added new tags for the sw_kp instrument's GFZ data, 'def' and 'now', to
```

### Comparing `pysatSpaceWeather-0.0.8/CODE_OF_CONDUCT.md` & `pysatSpaceWeather-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/CONTRIBUTING.md` & `pysatSpaceWeather-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/LICENSE` & `pysatSpaceWeather-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/PKG-INFO` & `pysatSpaceWeather-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pysatSpaceWeather
-Version: 0.0.8
+Version: 0.0.9
 Summary: 'pysat support for Space Weather Indices'
 Home-page: https://github.com/pysat/pysatSpaceWeather
 Author: Angeline Burrell, et al.
 Author-email: pysat.developers@gmail.com
 Keywords: pysat,ionosphere,heliophysics,magnetosphere,space-weather,forecasting,indexes
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="left">
         <img height="0" width="0px">
         <img width="20%" src="https://raw.githubusercontent.com/pysat/pysatSpaceWeather/main/docs/figures/pysatSpaceWeather.png" alt="pysatSpaceWeather" title="pysatSpaceWeather" </img>
 </div>
```

### Comparing `pysatSpaceWeather-0.0.8/README.md` & `pysatSpaceWeather-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/ace_epam.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/ace_epam.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/ace_mag.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/ace_mag.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/ace_sis.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/ace_sis.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/ace_swepam.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/ace_swepam.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/ace.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/ace.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/dst.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/dst.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/f107.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/f107.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/general.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/general.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/methods/kp_ap.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/methods/kp_ap.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/sw_dst.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/sw_dst.py`

 * *Files identical despite different names*

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/sw_f107.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/sw_f107.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,25 +53,25 @@
 loading multiple days, the data padding feature, and multi_file_day feature
 available from the pyast.Instrument object is not appropriate for '45day' data.
 
 """
 
 import datetime as dt
 import ftplib
-import json
 import numpy as np
 import os
 import pandas as pds
 import pysat
 import requests
 import sys
 import warnings
 
 from pysatSpaceWeather.instruments.methods import f107 as mm_f107
 from pysatSpaceWeather.instruments.methods import general
+from pysatSpaceWeather.instruments.methods import lisird
 
 logger = pysat.logger
 
 # ----------------------------------------------------------------------------
 # Instrument attributes
 
 platform = 'sw'
@@ -120,14 +120,34 @@
     self.references = mm_f107.references(self.tag)
     logger.info(self.acknowledgements)
 
     # Define the historic F10.7 starting time
     if self.tag == 'historic':
         self.lasp_stime = lasp_stime
 
+    # Raise Deprecation warnings
+    if self.tag in ['daily', 'prelim']:
+        # This tag loads more than just F10.7 data, and the behaviour will be
+        # deprecated in v0.1.0
+        warnings.warn("".join(["Upcoming structural changes will prevent ",
+                               "Instruments from loading multiple data sets in",
+                               " one Instrument. In version 0.1.0+ the SSN, ",
+                               "solar flare, and solar mean field data will be",
+                               " accessable from the `sw_ssn`, `sw_flare`, ",
+                               "and `sw_sbfield` Instruments."]),
+                      DeprecationWarning, stacklevel=2)
+    elif self.tag == '45day':
+        # This tag loads more than just F10.7 data, and the behaviour will be
+        # deprecated in v0.1.0
+        warnings.warn("".join(["Upcoming structural changes will prevent ",
+                               "Instruments from loading multiple data sets in",
+                               " one Instrument. In version 0.1.0+ the Ap will",
+                               " be accessable from the `sw_ap` Instrument."]),
+                      DeprecationWarning, stacklevel=2)
+
     return
 
 
 def clean(self):
     """Clean the F10.7 data, empty function as this is not necessary."""
 
     return
@@ -202,15 +222,14 @@
                       meta.labels.name: 'Daily Ap index',
                       meta.labels.notes: '',
                       meta.labels.desc: 'Daily average of 3-h ap indices',
                       meta.labels.fill_val: np.nan,
                       meta.labels.min_val: 0,
                       meta.labels.max_val: 400}
     elif tag == 'historic':
-
         # LASP updated file format in June, 2022. Minimize impact downstream by
         # continuing use of `f107` as primary data product.
         if 'f107_adjusted' in data.columns:
             # There may be a mix of old and new data formats.
             if 'f107' in data.columns:
                 # Only fill NaN in the `f107` and `f107_adjusted` columns
                 # for consistency across both data sets
@@ -460,68 +479,18 @@
         # Test the date array, updating it if necessary
         if date_array.freq != 'MS':
             date_array = pysat.utils.time.create_date_range(
                 dt.datetime(date_array[0].year, date_array[0].month, 1),
                 date_array[-1], freq='MS')
 
         # Download from LASP, by month
-        for dl_date in date_array:
-            # Create the name to which the local file will be saved
-            str_date = dl_date.strftime('%Y-%m')
-            data_file = os.path.join(data_path,
-                                     'f107_monthly_{:s}.txt'.format(str_date))
-
-            if update_files or not os.path.isfile(data_file):
-                # Set the download webpage
-                dstr = ''.join(['http://lasp.colorado.edu/lisird/latis/dap/',
-                                'noaa_radio_flux.json?time%3E=',
-                                dl_date.strftime('%Y-%m-%d'),
-                                'T00:00:00.000Z&time%3C=',
-                                (dl_date + pds.DateOffset(months=1)
-                                 - pds.DateOffset(days=1)).strftime('%Y-%m-%d'),
-                                'T00:00:00.000Z'])
-
-                # The data is returned as a JSON file
-                req = requests.get(dstr)
-
-                # Process the JSON file
-                if req.text.find('Gateway Timeout') >= 0:
-                    raise IOError(''.join(['Gateway timeout when requesting ',
-                                           'file using command: ', dstr]))
-
-                if req.ok:
-                    raw_dict = json.loads(req.text)['noaa_radio_flux']
-                    data = pds.DataFrame.from_dict(raw_dict['samples'])
-                    if data.empty:
-                        warnings.warn("no data for {:}".format(dl_date),
-                                      UserWarning)
-                    else:
-                        # The file format changed over time
-                        try:
-                            # This is the new data format
-                            times = [dt.datetime.strptime(time, '%Y%m%d')
-                                     for time in data.pop('time')]
-                        except ValueError:
-                            # Accepts old file formats
-                            times = [dt.datetime.strptime(time, '%Y %m %d')
-                                     for time in data.pop('time')]
-                        data.index = times
-
-                        # Replace fill value with NaNs
-                        for var in data.columns:
-                            idx, = np.where(data[var] == -99999.0)
-                            data.iloc[idx, :] = np.nan
-
-                        # Create a local CSV file
-                        data.to_csv(data_file, header=True)
-                else:
-                    pysat.logger.info("".join(["Data not downloaded for ",
-                                               dl_date.strftime("%d %b %Y"),
-                                               ", date may be out of range ",
-                                               "for the database."]))
+        freq = pds.DateOffset(months=1, seconds=-1)
+        lisird.download(date_array, data_path, 'f107_monthly_', '%Y-%m',
+                        'noaa_radio_flux', freq, update_files,
+                        {'f107_adjusted': -99999.0, 'f107_observed': -99999.0})
 
     elif tag == 'prelim':
         ftp = ftplib.FTP('ftp.swpc.noaa.gov')  # Connect to host, default port
         ftp.login()  # User anonymous, passwd anonymous
         ftp.cwd('/pub/indices/old_indices')
 
         bad_fname = list()
```

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather/instruments/sw_kp.py` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather/instruments/sw_kp.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,25 @@
 
 def init(self):
     """Initialize the Instrument object with instrument specific values."""
 
     self.acknowledgements = kp_ap.acknowledgements(self.name, self.tag)
     self.references = kp_ap.references(self.name, self.tag)
     pysat.logger.info(self.acknowledgements)
+
+    if self.tag in ["def", "now"]:
+        # This tag loads more than just Kp data, and the behaviour will be
+        # deprecated in v0.1.0
+        warnings.warn("".join(["Upcoming structural changes will prevent ",
+                               "Instruments from loading multiple data sets ",
+                               "in one Instrument. In version 0.1.0+ the Ap ",
+                               "and Cp data will be accessable from the ",
+                               "`sw_ap` and `sw_cp` Instruments."]),
+                      DeprecationWarning, stacklevel=2)
+
     return
 
 
 def clean(self):
     """Clean the Kp, not required for this index (empty function)."""
 
     return
```

### Comparing `pysatSpaceWeather-0.0.8/pysatSpaceWeather.egg-info/PKG-INFO` & `pysatSpaceWeather-0.0.9/pysatSpaceWeather.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pysatSpaceWeather
-Version: 0.0.8
+Version: 0.0.9
 Summary: 'pysat support for Space Weather Indices'
 Home-page: https://github.com/pysat/pysatSpaceWeather
 Author: Angeline Burrell, et al.
 Author-email: pysat.developers@gmail.com
 Keywords: pysat,ionosphere,heliophysics,magnetosphere,space-weather,forecasting,indexes
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="left">
         <img height="0" width="0px">
         <img width="20%" src="https://raw.githubusercontent.com/pysat/pysatSpaceWeather/main/docs/figures/pysatSpaceWeather.png" alt="pysatSpaceWeather" title="pysatSpaceWeather" </img>
 </div>
```

### Comparing `pysatSpaceWeather-0.0.8/setup.cfg` & `pysatSpaceWeather-0.0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,28 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Topic :: Scientific/Engineering :: Physics
 	Topic :: Scientific/Engineering :: Atmospheric Science
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
+	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Operating System :: MacOS :: MacOS X
 	Operating System :: POSIX :: Linux
 	Operating System :: Microsoft :: Windows
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
-python_requires = >= 3.7
+python_requires = >= 3.6
 setup_requires = setuptools >= 38.6; pip >= 10
 include_package_data = True
 zip_safe = False
 packages = find:
 install_requires = netCDF4
 	numpy
 	packaging
```

