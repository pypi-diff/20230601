# Comparing `tmp/sliderule-3.4.0.tar.gz` & `tmp/sliderule-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.4.0.tar", last modified: Wed May 31 19:43:48 2023, max compression
+gzip compressed data, was "sliderule-3.4.1.tar", last modified: Thu Jun  1 15:18:13 2023, max compression
```

## Comparing `sliderule-3.4.0.tar` & `sliderule-3.4.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 19:43:48.075043 sliderule-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-31 19:43:36.000000 sliderule-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-31 19:43:36.000000 sliderule-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-31 19:43:48.075043 sliderule-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-31 19:43:36.000000 sliderule-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-31 19:43:36.000000 sliderule-3.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 19:43:48.075043 sliderule-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-31 19:43:36.000000 sliderule-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 19:43:48.071043 sliderule-3.4.0/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29288 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    17509 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    34861 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    45777 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 19:43:48.071043 sliderule-3.4.0/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-31 19:43:47.000000 sliderule-3.4.0/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-31 19:43:48.000000 sliderule-3.4.0/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 19:43:47.000000 sliderule-3.4.0/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-31 19:43:47.000000 sliderule-3.4.0/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-31 19:43:47.000000 sliderule-3.4.0/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 19:43:48.075043 sliderule-3.4.0/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/build_3dep_DEM_geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-31 19:43:36.000000 sliderule-3.4.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:18:13.337535 sliderule-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-06-01 15:17:57.000000 sliderule-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-01 15:17:57.000000 sliderule-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-01 15:18:13.337535 sliderule-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-01 15:17:57.000000 sliderule-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-01 15:17:57.000000 sliderule-3.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 15:18:13.337535 sliderule-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-01 15:17:57.000000 sliderule-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:18:13.333534 sliderule-3.4.1/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29288 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17509 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34861 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45777 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:18:13.333534 sliderule-3.4.1/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:18:13.337535 sliderule-3.4.1/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/build_3dep_DEM_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-01 15:17:57.000000 sliderule-3.4.1/version.txt
```

### Comparing `sliderule-3.4.0/LICENSE` & `sliderule-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/PKG-INFO` & `sliderule-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.4.0
+Version: 3.4.1
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.4.0/README.md` & `sliderule-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/setup.py` & `sliderule-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/earthdata.py` & `sliderule-3.4.1/sliderule/earthdata.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/gedi.py` & `sliderule-3.4.1/sliderule/gedi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/h5.py` & `sliderule-3.4.1/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/icesat2.py` & `sliderule-3.4.1/sliderule/icesat2.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/io.py` & `sliderule-3.4.1/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/ipxapi.py` & `sliderule-3.4.1/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/ipysliderule.py` & `sliderule-3.4.1/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/raster.py` & `sliderule-3.4.1/sliderule/raster.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule/sliderule.py` & `sliderule-3.4.1/sliderule/sliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/sliderule.egg-info/PKG-INFO` & `sliderule-3.4.1/sliderule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.4.0
+Version: 3.4.1
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.4.0/sliderule.egg-info/SOURCES.txt` & `sliderule-3.4.1/sliderule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/big_query.py` & `sliderule-3.4.1/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/build_3dep_DEM_geojson.py` & `sliderule-3.4.1/utils/build_3dep_DEM_geojson.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.4.1/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.4.1/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.4.1/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/extract_h5_dataset.py` & `sliderule-3.4.1/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/icepyx_region.py` & `sliderule-3.4.1/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/lpdaac_download.py` & `sliderule-3.4.1/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/monitor.py` & `sliderule-3.4.1/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/query_cmr.py` & `sliderule-3.4.1/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/query_elevations.py` & `sliderule-3.4.1/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/query_metrics.py` & `sliderule-3.4.1/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/query_photons.py` & `sliderule-3.4.1/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/query_stac.py` & `sliderule-3.4.1/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/query_version.py` & `sliderule-3.4.1/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/region_of_interest.py` & `sliderule-3.4.1/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/results_to_s3.py` & `sliderule-3.4.1/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/stac.py` & `sliderule-3.4.1/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/stream_events.py` & `sliderule-3.4.1/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/tail_events.py` & `sliderule-3.4.1/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.0/utils/utils.py` & `sliderule-3.4.1/utils/utils.py`

 * *Files identical despite different names*

