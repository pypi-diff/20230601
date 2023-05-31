# Comparing `tmp/openet-ssebop-0.2.6.tar.gz` & `tmp/openet-ssebop-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openet-ssebop-0.2.6.tar", last modified: Fri Jul  8 15:31:27 2022, max compression
+gzip compressed data, was "openet-ssebop-0.2.8.tar", last modified: Wed May 31 21:58:40 2023, max compression
```

## Comparing `openet-ssebop-0.2.6.tar` & `openet-ssebop-0.2.8.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-07-08 15:31:27.723778 openet-ssebop-0.2.6/
--rw-r--r--   0 mortonc  (11773) staff       (20)    11356 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/LICENSE.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)      132 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/MANIFEST.in
--rw-r--r--   0 mortonc  (11773) staff       (20)    14106 2022-07-08 15:31:27.723930 openet-ssebop-0.2.6/PKG-INFO
--rw-r--r--   0 mortonc  (11773) staff       (20)    13415 2022-02-10 18:13:26.000000 openet-ssebop-0.2.6/README.rst
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-07-08 15:31:27.712928 openet-ssebop-0.2.6/openet/
--rw-r--r--   0 mortonc  (11773) staff       (20)     6148 2022-06-21 14:06:48.000000 openet-ssebop-0.2.6/openet/.DS_Store
--rw-r--r--   0 mortonc  (11773) staff       (20)       65 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/__init__.py
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-07-08 15:31:27.717693 openet-ssebop-0.2.6/openet/ssebop/
--rw-r--r--   0 mortonc  (11773) staff       (20)      133 2022-04-07 13:58:20.000000 openet-ssebop-0.2.6/openet/ssebop/__init__.py
--rw-r--r--   0 mortonc  (11773) staff       (20)    40509 2022-06-17 01:05:19.000000 openet-ssebop-0.2.6/openet/ssebop/collection.py
--rw-r--r--   0 mortonc  (11773) staff       (20)    92453 2022-05-26 21:57:32.000000 openet-ssebop-0.2.6/openet/ssebop/image.py
--rw-r--r--   0 mortonc  (11773) staff       (20)    16214 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/interpolate.py
--rw-r--r--   0 mortonc  (11773) staff       (20)      816 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/ipytest.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     4616 2022-06-17 01:05:21.000000 openet-ssebop-0.2.6/openet/ssebop/landsat.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     6978 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/model.py
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-07-08 15:31:27.721698 openet-ssebop-0.2.6/openet/ssebop/tests/
--rw-r--r--   0 mortonc  (11773) staff       (20)     1009 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/tests/conftest.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     1982 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/tests/test_a_utils.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     3109 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/tests/test_b_landsat.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     7867 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/tests/test_b_model.py
--rw-r--r--   0 mortonc  (11773) staff       (20)    78222 2022-04-06 14:14:33.000000 openet-ssebop-0.2.6/openet/ssebop/tests/test_c_image.py
--rw-r--r--   0 mortonc  (11773) staff       (20)    28488 2022-03-09 17:10:23.000000 openet-ssebop-0.2.6/openet/ssebop/tests/test_d_collection.py
--rw-r--r--   0 mortonc  (11773) staff       (20)    11236 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/tests/test_d_interpolate.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     3594 2022-02-10 18:11:19.000000 openet-ssebop-0.2.6/openet/ssebop/utils.py
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-07-08 15:31:27.723554 openet-ssebop-0.2.6/openet_ssebop.egg-info/
--rw-r--r--   0 mortonc  (11773) staff       (20)    14106 2022-07-08 15:31:27.000000 openet-ssebop-0.2.6/openet_ssebop.egg-info/PKG-INFO
--rw-r--r--   0 mortonc  (11773) staff       (20)      772 2022-07-08 15:31:27.000000 openet-ssebop-0.2.6/openet_ssebop.egg-info/SOURCES.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)        1 2022-07-08 15:31:27.000000 openet-ssebop-0.2.6/openet_ssebop.egg-info/dependency_links.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)        1 2022-04-05 13:41:50.000000 openet-ssebop-0.2.6/openet_ssebop.egg-info/not-zip-safe
--rw-r--r--   0 mortonc  (11773) staff       (20)       61 2022-07-08 15:31:27.000000 openet-ssebop-0.2.6/openet_ssebop.egg-info/requires.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)        7 2022-07-08 15:31:27.000000 openet-ssebop-0.2.6/openet_ssebop.egg-info/top_level.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)       63 2022-07-08 15:31:27.724475 openet-ssebop-0.2.6/setup.cfg
--rw-r--r--   0 mortonc  (11773) staff       (20)     2096 2022-04-07 13:56:34.000000 openet-ssebop-0.2.6/setup.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-05-31 21:58:40.954370 openet-ssebop-0.2.8/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11356 2023-05-01 17:38:26.000000 openet-ssebop-0.2.8/LICENSE.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      132 2023-05-01 17:38:26.000000 openet-ssebop-0.2.8/MANIFEST.in
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    14456 2023-05-31 21:58:40.954435 openet-ssebop-0.2.8/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    13785 2023-05-31 21:51:29.000000 openet-ssebop-0.2.8/README.rst
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-05-31 21:58:40.951205 openet-ssebop-0.2.8/openet/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-05-01 17:38:27.000000 openet-ssebop-0.2.8/openet/__init__.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-05-31 21:58:40.952377 openet-ssebop-0.2.8/openet/ssebop/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      133 2023-05-31 21:58:02.000000 openet-ssebop-0.2.8/openet/ssebop/__init__.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    41063 2023-05-30 14:13:34.000000 openet-ssebop-0.2.8/openet/ssebop/collection.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    92607 2023-05-30 21:41:38.000000 openet-ssebop-0.2.8/openet/ssebop/image.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    16268 2023-05-30 21:50:15.000000 openet-ssebop-0.2.8/openet/ssebop/interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      816 2023-05-01 17:38:27.000000 openet-ssebop-0.2.8/openet/ssebop/ipytest.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     4553 2023-05-30 18:05:48.000000 openet-ssebop-0.2.8/openet/ssebop/landsat.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     6954 2023-05-30 18:05:48.000000 openet-ssebop-0.2.8/openet/ssebop/model.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-05-31 21:58:40.953488 openet-ssebop-0.2.8/openet/ssebop/tests/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1009 2023-05-01 17:38:27.000000 openet-ssebop-0.2.8/openet/ssebop/tests/conftest.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2317 2023-05-30 21:52:32.000000 openet-ssebop-0.2.8/openet/ssebop/tests/test_a_utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3109 2023-05-01 17:38:27.000000 openet-ssebop-0.2.8/openet/ssebop/tests/test_b_landsat.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     7867 2023-05-01 17:38:27.000000 openet-ssebop-0.2.8/openet/ssebop/tests/test_b_model.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    76911 2023-05-30 18:14:01.000000 openet-ssebop-0.2.8/openet/ssebop/tests/test_c_image.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    29030 2023-05-30 18:31:36.000000 openet-ssebop-0.2.8/openet/ssebop/tests/test_d_collection.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11236 2023-05-01 17:38:27.000000 openet-ssebop-0.2.8/openet/ssebop/tests/test_d_interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3652 2023-05-30 18:21:07.000000 openet-ssebop-0.2.8/openet/ssebop/utils.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-05-31 21:58:40.954270 openet-ssebop-0.2.8/openet_ssebop.egg-info/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    14456 2023-05-31 21:58:40.000000 openet-ssebop-0.2.8/openet_ssebop.egg-info/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      755 2023-05-31 21:58:40.000000 openet-ssebop-0.2.8/openet_ssebop.egg-info/SOURCES.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2023-05-31 21:58:40.000000 openet-ssebop-0.2.8/openet_ssebop.egg-info/dependency_links.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2023-05-30 13:08:12.000000 openet-ssebop-0.2.8/openet_ssebop.egg-info/not-zip-safe
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       61 2023-05-31 21:58:40.000000 openet-ssebop-0.2.8/openet_ssebop.egg-info/requires.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2023-05-31 21:58:40.000000 openet-ssebop-0.2.8/openet_ssebop.egg-info/top_level.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       63 2023-05-31 21:58:40.954700 openet-ssebop-0.2.8/setup.cfg
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2096 2023-05-01 17:38:27.000000 openet-ssebop-0.2.8/setup.py
```

### Comparing `openet-ssebop-0.2.6/LICENSE.txt` & `openet-ssebop-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openet-ssebop-0.2.6/PKG-INFO` & `openet-ssebop-0.2.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: openet-ssebop
-Version: 0.2.6
+Version: 0.2.8
 Summary: Earth Engine based SSEBop Model
 Home-page: https://github.com/Open-ET/openet-ssebop
+Download-URL: https://github.com/Open-ET/openet-ssebop/archive/v0.2.8.tar.gz
 Author: Gabe Parrish, Mac Friedrichs, Gabriel Senay
 Author-email: gparrish@contractor.usgs.gov
 License: Apache
-Download-URL: https://github.com/Open-ET/openet-ssebop/archive/v0.2.6.tar.gz
 Keywords: SSEBop OpenET Evapotranspiration Earth Engine
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 ===============
 OpenET - SSEBop
 ===============
 
-|version| |build| |codecov|
+|version| |build|
 
 **WARNING: This code is in development, is being provided without support, and is subject to change at any time without notification**
 
 This repository provides `Google Earth Engine <https://earthengine.google.com/>`__ Python API based implementation of the SSEBop ET model.
 
 The Operational Simplified Surface Energy Balance (SSEBop) model computes daily total actual evapotranspiration (ETa) using land surface temperature (Ts), maximum air temperature (Ta) and reference ET (ETr or ETo).
 The SSEBop model does not solve all the energy balance terms explicitly; rather, it defines the limiting conditions based on "gray-sky" net radiation balance principles and an air temperature parameter.
-This approach predefines unique sets of "hot/dry" and "cold/wet" limiting values for each pixel, allowing an operational model setup and a relatively shorter compute time.
+This approach predefines unique sets of "hot/dry" and "cold/wet" limiting values for each pixel, allowing an operational model setup and a relatively shorter compute time. More information on the GEE implementation of SSEBop is published in Senay2022_ and Senay2023_ with additional details and model assessment.
 
 *Basic SSEBop model implementation in Earth Engine:*
 
 .. image:: docs/SSEBop_GEE_diagram.jpg
 
 Model Design
 ============
@@ -40,37 +39,39 @@
 The primary component of the SSEBop model is the Image() class.  The Image class can be used to compute a single fraction of reference ET (ETf) image from a single input image.  The Image class should generally be instantiated from an Earth Engine Landsat image using the collection specific methods listed below.  ET image collections can be built by computing ET in a function that is mapped over a collection of input images.  Please see the `Example Notebooks`_ for more details.
 
 Input Collections
 =================
 
 SSEBop ET can currently be computed for Landsat Collection 2 Level 2 (SR/ST) images and Landsat Collection 1 Top-Of-Atmosphere (TOA) images from the following Earth Engine image collections:
 
+ * LANDSAT/LC09/C02/T1_L2
  * LANDSAT/LC08/C02/T1_L2
  * LANDSAT/LE07/C02/T1_L2
  * LANDSAT/LT05/C02/T1_L2
  * LANDSAT/LC08/C01/T1_TOA or LANDSAT/LC08/C01/T1_RT_TOA
  * LANDSAT/LE07/C01/T1_TOA or LANDSAT/LE07/C01/T1_RT_TOA
  * LANDSAT/LT05/C01/T1_TOA
 
 
-**Note:** Users are encouraged to prioritize use of Collection 2 data where available. Collection 1 will be produced by USGS until 2022-01-01, and maintained by Earth Engine until 2023-01-01. [`More Information <https://developers.google.com/earth-engine/guides/landsat#landsat-collection-status>`__]
+**Note:** Users are encouraged to prioritize use of Collection 2 data where available. Collection 1 was produced by USGS until 2022-01-01, and maintained by Earth Engine until 2023-01-01. [`More Information <https://developers.google.com/earth-engine/guides/landsat#landsat-collection-status>`__]
 
 Landsat Collection 2 SR/ST Input Image
 --------------------------------------
 
 To instantiate the class for a Landsat Collection 2 SR/ST image, use the Image.from_landsat_c2_sr method.
 
 The input Landsat image must have the following bands and properties:
 
 =================  ======================================
 SPACECRAFT_ID      Band Names
 =================  ======================================
 LANDSAT_5          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B7, ST_B6, QA_PIXEL
 LANDSAT_7          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B7, ST_B6, QA_PIXEL
 LANDSAT_8          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B6, SR_B7, ST_B10, QA_PIXEL
+LANDSAT_9          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B6, SR_B7, ST_B10, QA_PIXEL
 =================  ======================================
 
 Landsat Collection 1 TOA Input Image
 ------------------------------------
 
 To instantiate the class for a Landsat Collection 1 TOA image, use the Image.from_landsat_c1_toa() method.
 
@@ -85,15 +86,15 @@
 =================  ======================================
 
 =================  =============================================
 Property           Description
 =================  =============================================
 system:index       - Landsat Scene ID
                    - Must be in the Earth Engine format (e.g. LC08_044033_20170716)
-                   - Used to lookup the scene specific c-factor
+                   - Used to lookup the scene specific c-factor (DEPRECATED)
 system:time_start  Image datetime in milliseconds since 1970
 SPACECRAFT_ID      - Used to determine which Landsat type
                    - Must be: LANDSAT_5, LANDSAT_7, or LANDSAT_8
 =================  =============================================
 
 Model Output
 ------------
@@ -145,56 +146,49 @@
 ==================
 
 Maximum Daily Air Temperature (Tmax)
 ------------------------------------
 The daily maximum air temperature (Tmax) is essential for establishing the maximum ET limit (cold boundary) as explained in Senay2017_.
 Support for source options includes CIMIS, GRIDMET, DAYMET, and other custom Image Collections. See the model Image class docstrings for more information.
 
-Default Asset ID: *projects/usgs-ssebop/tmax/daymet_median_v2* (Daily median from 1980-2018)
+Default Asset ID: *projects/usgs-ssebop/tmax/daymet_v4_mean_1981_2010* (Daily median from 1981-2010)
 
 Land Surface Temperature (LST)
 ------------------------------
 Land Surface Temperature is currently calculated in the SSEBop approach two ways:
 
 * Landsat Collection 2 Level-2 (ST band) images directly. More information can be found at: `USGS Landsat Collection 2 Level-2 Science Products <https://www.usgs.gov/core-science-systems/nli/landsat/landsat-collection-2-level-2-science-products>`__
 
 * Landsat Collection 1 Top-of-Atmosphere images by including an on-the-fly function for calibration steps and atmospheric correction techniques. These include calculations for: (1) spectral radiance conversion to the at-sensor brightness temperature; (2) atmospheric absorption and re-emission value; and (3) surface emissivity. For additional information, users can refer to section 3.2 of the Methodology in Senay2016_.
 
 Temperature Difference (dT)
 ---------------------------
 The SSEBop ET model uses dT as a predefined temperature difference between Thot and Tcold for each pixel.
 In SSEBop formulation, hot and cold limits are defined on the same pixel; therefore, dT actually represents the vertical temperature difference between the surface temperature of a theoretical bare/dry condition of a given pixel and the air temperature at the canopy level of the same pixel as explained in Senay2018_. The input dT is calculated under "gray-sky" conditions and assumed not to change from year to year, but is unique for each day and location.
 
-Default Asset ID: *projects/usgs-ssebop/dt/daymet_median_v2*
-
-Elevation
----------
-The default elevation dataset is the USGS SRTM global image asset.
-
-Default Asset ID: `USGS/SRTMGL1_003 <https://developers.google.com/earth-engine/datasets/catalog/USGS_SRTMGL1_003>`__
-
-The elevation parameter will accept any Earth Engine image.
+Default Asset ID: *projects/usgs-ssebop/dt/daymet_median_v6*
 
 Temperature Correction (*c factor*)
 -----------------------------------
-In order to correspond the maximum air temperature with cold/wet limiting environmental conditions, the SSEBop model uses a temperature correction coefficient (*c factor*, sometimes labeled interchangeably as Tcorr) uniquely calculated for each Landsat scene from well-watered/vegetated pixels.
-This temperature correction component is based on a ratio of Tmax and LST that has passed through several conditions such as NDVI limits. The SSEBop model utilizes the *c factor* as a function of the maximum air temperature, so the data source of the *c factor* collection needs to match the data source of the air temperature. **Note:** *Tcorr* refers to the pixel-based ratio of LST_cold and Tmax while *c factor* is a statistical value that represents a region such as a 5-km grid or scene-wide value.
+In order to correspond the maximum air temperature with cold/wet limiting environmental conditions, the SSEBop model uses a temperature correction coefficient (*c factor*, sometimes labeled interchangeably as Tcorr) uniquely calculated for each Landsat scene.
+This temperature correction component is uniquely developed for SSEBop using a Forcing and Normalizing Operation (FANO) method featuring a linear relation between a normalized land surface temperature difference and NDVI difference using the dT parameter and a proportionality constant.
 
-.. image:: docs/GriddedCfactor_example.png
+ **Note:** *Tcorr* refers to the pixel-based ratio of LST_cold and Tmax while *c factor* is a statistical value that represents a region such as a 5-km grid size (or larger) value.
 
-This parameter can be implemented dynamically as a scene-based single *c factor* (this is the default) or using precomputed spatially varying Image Assets where a gridded *c factor* is generated for every 5-km (advanced setting).
+More information on parameter design and model improvements using the FANO method can be found in Senay2023_. Additional SSEBop model algorithm theoretical basis documentation can be found `here <https://www.usgs.gov/media/files/landsat-4-9-collection-2-level-3-provisional-actual-evapotranspiration-algorithm>`__.
 
-* Using either DYNAMIC or SCENE_GRIDDED settings, the *c factor* parameter is read from precomputed Earth Engine image collections based on the Landsat scene ID (from the system:index property). Monthly/annual climatology values are used if Tcorr cannot be determined for a given Landsat scene. If fallback values have not been computed for the target path/row, a default value of 0.978 will be used.
-* Currently, SCENE_GRIDDED is only supported for Landsat Collection 2 across CONUS (since model version 0.1.5x) and requires a matching Tmax source. See `this example notebook <examples/tcorr_gridded.ipynb>`__ for more information.
+The 'FANO' parameter (default) can be implemented dynamically for each Landsat scene within the SSEBop Image object using the following Tcorr source:
 
-Default Asset IDs
+.. code-block:: python
 
-Scene ID: projects/usgs-ssebop/tcorr_scene/daymet_median_v2_scene
+    model_obj = model.Image.from_landsat_c2_sr(
+        tcorr_source='FANO',
+        )
 
-Monthly ID: projects/usgs-ssebop/tcorr_scene/daymet_median_v2_monthly
+The FANO parameterization allows the establishment of the cold boundary condition regardless of vegetation cover density, improving the performance and operational implementation of the SSEBop ET model in sparsely vegetated landscapes, dynamic growing seasons, and varying locations around the world.
 
 Installation
 ============
 
 The OpenET SSEBop python module can be installed via pip:
 
 .. code-block:: console
@@ -238,21 +232,22 @@
 .. [Senay2018]
  | Senay, G. (2018). Satellite Psychrometric Formulation of the Operational Simplified Surface Energy Balance (SSEBop) Model for Quantifying and Mapping Evapotranspiration. *Applied Engineering in Agriculture*, 34(3).
  | `https://doi.org/10.13031/aea.12614 <https://doi.org/10.13031/aea.12614>`__
 .. [Senay2019]
  | Senay, G., Schauer, M., Velpuri, N.M., Singh, R.K., Kagone, S., Friedrichs, M., Litvak, M.E., Douglas-Mankin, K.R. (2019). Long-Term (1986–2015) Crop Water Use Characterization over the Upper Rio Grande Basin of United States and Mexico Using Landsat-Based Evapotranspiration. *Remote Sensing*, 11(13):1587.
  | `https://doi.org/10.3390/rs11131587 <https://doi.org/10.3390/rs11131587>`__
 .. [Schauer2019]
- | Schauer, M.,Senay, G. (2019). Characterizing Crop Water Use Dynamics in the Central Valley of California Using Landsat-Derived Evapotranspiration. *Remote Sensing*, 11(15):1782.
+ | Schauer, M., Senay, G. (2019). Characterizing Crop Water Use Dynamics in the Central Valley of California Using Landsat-Derived Evapotranspiration. *Remote Sensing*, 11(15):1782.
  | `https://doi.org/10.3390/rs11151782 <https://doi.org/10.3390/rs11151782>`__
+.. [Senay2022]
+ | Senay, G.B., Friedrichs, M., Morton, C., Parrish, G. E., Schauer, M., Khand, K., ... & Huntington, J. (2022). Mapping actual evapotranspiration using Landsat for the conterminous United States: Google Earth Engine implementation and assessment of the SSEBop model. *Remote Sensing of Environment*, 275, 113011
+ | `https://doi.org/10.1016/j.rse.2022.113011 <https://doi.org/10.1016/j.rse.2022.113011>`__
+.. [Senay2023]
+ | Senay, G.B., Parrish, G. E., Schauer, M., Friedrichs, M., Khand, K., Boiko, O., Kagone, S., Dittmeier, R., Arab, S., Ji, L. (2023). Improving the Operational Simplified Surface Energy Balance evapotranspiration model using the Forcing and Normalizing Operation. *Remote Sensing*, 15(1):260.
+ | `https://doi.org/10.3390/rs15010260 <https://doi.org/10.3390/rs15010260>`__
 
 .. |build| image:: https://github.com/Open-ET/openet-ssebop/workflows/build/badge.svg
    :alt: Build status
    :target: https://github.com/Open-ET/openet-ssebop
 .. |version| image:: https://badge.fury.io/py/openet-ssebop.svg
    :alt: Latest version on PyPI
    :target: https://badge.fury.io/py/openet-ssebop
-.. |codecov| image:: https://codecov.io/gh/Open-ET/openet-ssebop/branch/main/graphs/badge.svg
-   :alt: Coverage Status
-   :target: https://codecov.io/gh/Open-ET/openet-ssebop
-
-
```

### Comparing `openet-ssebop-0.2.6/README.rst` & `openet-ssebop-0.2.8/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ===============
 OpenET - SSEBop
 ===============
 
-|version| |build| |codecov|
+|version| |build|
 
 **WARNING: This code is in development, is being provided without support, and is subject to change at any time without notification**
 
 This repository provides `Google Earth Engine <https://earthengine.google.com/>`__ Python API based implementation of the SSEBop ET model.
 
 The Operational Simplified Surface Energy Balance (SSEBop) model computes daily total actual evapotranspiration (ETa) using land surface temperature (Ts), maximum air temperature (Ta) and reference ET (ETr or ETo).
 The SSEBop model does not solve all the energy balance terms explicitly; rather, it defines the limiting conditions based on "gray-sky" net radiation balance principles and an air temperature parameter.
-This approach predefines unique sets of "hot/dry" and "cold/wet" limiting values for each pixel, allowing an operational model setup and a relatively shorter compute time.
+This approach predefines unique sets of "hot/dry" and "cold/wet" limiting values for each pixel, allowing an operational model setup and a relatively shorter compute time. More information on the GEE implementation of SSEBop is published in Senay2022_ and Senay2023_ with additional details and model assessment.
 
 *Basic SSEBop model implementation in Earth Engine:*
 
 .. image:: docs/SSEBop_GEE_diagram.jpg
 
 Model Design
 ============
@@ -22,37 +22,39 @@
 The primary component of the SSEBop model is the Image() class.  The Image class can be used to compute a single fraction of reference ET (ETf) image from a single input image.  The Image class should generally be instantiated from an Earth Engine Landsat image using the collection specific methods listed below.  ET image collections can be built by computing ET in a function that is mapped over a collection of input images.  Please see the `Example Notebooks`_ for more details.
 
 Input Collections
 =================
 
 SSEBop ET can currently be computed for Landsat Collection 2 Level 2 (SR/ST) images and Landsat Collection 1 Top-Of-Atmosphere (TOA) images from the following Earth Engine image collections:
 
+ * LANDSAT/LC09/C02/T1_L2
  * LANDSAT/LC08/C02/T1_L2
  * LANDSAT/LE07/C02/T1_L2
  * LANDSAT/LT05/C02/T1_L2
  * LANDSAT/LC08/C01/T1_TOA or LANDSAT/LC08/C01/T1_RT_TOA
  * LANDSAT/LE07/C01/T1_TOA or LANDSAT/LE07/C01/T1_RT_TOA
  * LANDSAT/LT05/C01/T1_TOA
 
 
-**Note:** Users are encouraged to prioritize use of Collection 2 data where available. Collection 1 will be produced by USGS until 2022-01-01, and maintained by Earth Engine until 2023-01-01. [`More Information <https://developers.google.com/earth-engine/guides/landsat#landsat-collection-status>`__]
+**Note:** Users are encouraged to prioritize use of Collection 2 data where available. Collection 1 was produced by USGS until 2022-01-01, and maintained by Earth Engine until 2023-01-01. [`More Information <https://developers.google.com/earth-engine/guides/landsat#landsat-collection-status>`__]
 
 Landsat Collection 2 SR/ST Input Image
 --------------------------------------
 
 To instantiate the class for a Landsat Collection 2 SR/ST image, use the Image.from_landsat_c2_sr method.
 
 The input Landsat image must have the following bands and properties:
 
 =================  ======================================
 SPACECRAFT_ID      Band Names
 =================  ======================================
 LANDSAT_5          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B7, ST_B6, QA_PIXEL
 LANDSAT_7          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B7, ST_B6, QA_PIXEL
 LANDSAT_8          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B6, SR_B7, ST_B10, QA_PIXEL
+LANDSAT_9          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B6, SR_B7, ST_B10, QA_PIXEL
 =================  ======================================
 
 Landsat Collection 1 TOA Input Image
 ------------------------------------
 
 To instantiate the class for a Landsat Collection 1 TOA image, use the Image.from_landsat_c1_toa() method.
 
@@ -67,15 +69,15 @@
 =================  ======================================
 
 =================  =============================================
 Property           Description
 =================  =============================================
 system:index       - Landsat Scene ID
                    - Must be in the Earth Engine format (e.g. LC08_044033_20170716)
-                   - Used to lookup the scene specific c-factor
+                   - Used to lookup the scene specific c-factor (DEPRECATED)
 system:time_start  Image datetime in milliseconds since 1970
 SPACECRAFT_ID      - Used to determine which Landsat type
                    - Must be: LANDSAT_5, LANDSAT_7, or LANDSAT_8
 =================  =============================================
 
 Model Output
 ------------
@@ -127,56 +129,49 @@
 ==================
 
 Maximum Daily Air Temperature (Tmax)
 ------------------------------------
 The daily maximum air temperature (Tmax) is essential for establishing the maximum ET limit (cold boundary) as explained in Senay2017_.
 Support for source options includes CIMIS, GRIDMET, DAYMET, and other custom Image Collections. See the model Image class docstrings for more information.
 
-Default Asset ID: *projects/usgs-ssebop/tmax/daymet_median_v2* (Daily median from 1980-2018)
+Default Asset ID: *projects/usgs-ssebop/tmax/daymet_v4_mean_1981_2010* (Daily median from 1981-2010)
 
 Land Surface Temperature (LST)
 ------------------------------
 Land Surface Temperature is currently calculated in the SSEBop approach two ways:
 
 * Landsat Collection 2 Level-2 (ST band) images directly. More information can be found at: `USGS Landsat Collection 2 Level-2 Science Products <https://www.usgs.gov/core-science-systems/nli/landsat/landsat-collection-2-level-2-science-products>`__
 
 * Landsat Collection 1 Top-of-Atmosphere images by including an on-the-fly function for calibration steps and atmospheric correction techniques. These include calculations for: (1) spectral radiance conversion to the at-sensor brightness temperature; (2) atmospheric absorption and re-emission value; and (3) surface emissivity. For additional information, users can refer to section 3.2 of the Methodology in Senay2016_.
 
 Temperature Difference (dT)
 ---------------------------
 The SSEBop ET model uses dT as a predefined temperature difference between Thot and Tcold for each pixel.
 In SSEBop formulation, hot and cold limits are defined on the same pixel; therefore, dT actually represents the vertical temperature difference between the surface temperature of a theoretical bare/dry condition of a given pixel and the air temperature at the canopy level of the same pixel as explained in Senay2018_. The input dT is calculated under "gray-sky" conditions and assumed not to change from year to year, but is unique for each day and location.
 
-Default Asset ID: *projects/usgs-ssebop/dt/daymet_median_v2*
-
-Elevation
----------
-The default elevation dataset is the USGS SRTM global image asset.
-
-Default Asset ID: `USGS/SRTMGL1_003 <https://developers.google.com/earth-engine/datasets/catalog/USGS_SRTMGL1_003>`__
-
-The elevation parameter will accept any Earth Engine image.
+Default Asset ID: *projects/usgs-ssebop/dt/daymet_median_v6*
 
 Temperature Correction (*c factor*)
 -----------------------------------
-In order to correspond the maximum air temperature with cold/wet limiting environmental conditions, the SSEBop model uses a temperature correction coefficient (*c factor*, sometimes labeled interchangeably as Tcorr) uniquely calculated for each Landsat scene from well-watered/vegetated pixels.
-This temperature correction component is based on a ratio of Tmax and LST that has passed through several conditions such as NDVI limits. The SSEBop model utilizes the *c factor* as a function of the maximum air temperature, so the data source of the *c factor* collection needs to match the data source of the air temperature. **Note:** *Tcorr* refers to the pixel-based ratio of LST_cold and Tmax while *c factor* is a statistical value that represents a region such as a 5-km grid or scene-wide value.
+In order to correspond the maximum air temperature with cold/wet limiting environmental conditions, the SSEBop model uses a temperature correction coefficient (*c factor*, sometimes labeled interchangeably as Tcorr) uniquely calculated for each Landsat scene.
+This temperature correction component is uniquely developed for SSEBop using a Forcing and Normalizing Operation (FANO) method featuring a linear relation between a normalized land surface temperature difference and NDVI difference using the dT parameter and a proportionality constant.
 
-.. image:: docs/GriddedCfactor_example.png
+ **Note:** *Tcorr* refers to the pixel-based ratio of LST_cold and Tmax while *c factor* is a statistical value that represents a region such as a 5-km grid size (or larger) value.
 
-This parameter can be implemented dynamically as a scene-based single *c factor* (this is the default) or using precomputed spatially varying Image Assets where a gridded *c factor* is generated for every 5-km (advanced setting).
+More information on parameter design and model improvements using the FANO method can be found in Senay2023_. Additional SSEBop model algorithm theoretical basis documentation can be found `here <https://www.usgs.gov/media/files/landsat-4-9-collection-2-level-3-provisional-actual-evapotranspiration-algorithm>`__.
 
-* Using either DYNAMIC or SCENE_GRIDDED settings, the *c factor* parameter is read from precomputed Earth Engine image collections based on the Landsat scene ID (from the system:index property). Monthly/annual climatology values are used if Tcorr cannot be determined for a given Landsat scene. If fallback values have not been computed for the target path/row, a default value of 0.978 will be used.
-* Currently, SCENE_GRIDDED is only supported for Landsat Collection 2 across CONUS (since model version 0.1.5x) and requires a matching Tmax source. See `this example notebook <examples/tcorr_gridded.ipynb>`__ for more information.
+The 'FANO' parameter (default) can be implemented dynamically for each Landsat scene within the SSEBop Image object using the following Tcorr source:
 
-Default Asset IDs
+.. code-block:: python
 
-Scene ID: projects/usgs-ssebop/tcorr_scene/daymet_median_v2_scene
+    model_obj = model.Image.from_landsat_c2_sr(
+        tcorr_source='FANO',
+        )
 
-Monthly ID: projects/usgs-ssebop/tcorr_scene/daymet_median_v2_monthly
+The FANO parameterization allows the establishment of the cold boundary condition regardless of vegetation cover density, improving the performance and operational implementation of the SSEBop ET model in sparsely vegetated landscapes, dynamic growing seasons, and varying locations around the world.
 
 Installation
 ============
 
 The OpenET SSEBop python module can be installed via pip:
 
 .. code-block:: console
@@ -220,19 +215,22 @@
 .. [Senay2018]
  | Senay, G. (2018). Satellite Psychrometric Formulation of the Operational Simplified Surface Energy Balance (SSEBop) Model for Quantifying and Mapping Evapotranspiration. *Applied Engineering in Agriculture*, 34(3).
  | `https://doi.org/10.13031/aea.12614 <https://doi.org/10.13031/aea.12614>`__
 .. [Senay2019]
  | Senay, G., Schauer, M., Velpuri, N.M., Singh, R.K., Kagone, S., Friedrichs, M., Litvak, M.E., Douglas-Mankin, K.R. (2019). Long-Term (1986–2015) Crop Water Use Characterization over the Upper Rio Grande Basin of United States and Mexico Using Landsat-Based Evapotranspiration. *Remote Sensing*, 11(13):1587.
  | `https://doi.org/10.3390/rs11131587 <https://doi.org/10.3390/rs11131587>`__
 .. [Schauer2019]
- | Schauer, M.,Senay, G. (2019). Characterizing Crop Water Use Dynamics in the Central Valley of California Using Landsat-Derived Evapotranspiration. *Remote Sensing*, 11(15):1782.
+ | Schauer, M., Senay, G. (2019). Characterizing Crop Water Use Dynamics in the Central Valley of California Using Landsat-Derived Evapotranspiration. *Remote Sensing*, 11(15):1782.
  | `https://doi.org/10.3390/rs11151782 <https://doi.org/10.3390/rs11151782>`__
+.. [Senay2022]
+ | Senay, G.B., Friedrichs, M., Morton, C., Parrish, G. E., Schauer, M., Khand, K., ... & Huntington, J. (2022). Mapping actual evapotranspiration using Landsat for the conterminous United States: Google Earth Engine implementation and assessment of the SSEBop model. *Remote Sensing of Environment*, 275, 113011
+ | `https://doi.org/10.1016/j.rse.2022.113011 <https://doi.org/10.1016/j.rse.2022.113011>`__
+.. [Senay2023]
+ | Senay, G.B., Parrish, G. E., Schauer, M., Friedrichs, M., Khand, K., Boiko, O., Kagone, S., Dittmeier, R., Arab, S., Ji, L. (2023). Improving the Operational Simplified Surface Energy Balance evapotranspiration model using the Forcing and Normalizing Operation. *Remote Sensing*, 15(1):260.
+ | `https://doi.org/10.3390/rs15010260 <https://doi.org/10.3390/rs15010260>`__
 
 .. |build| image:: https://github.com/Open-ET/openet-ssebop/workflows/build/badge.svg
    :alt: Build status
    :target: https://github.com/Open-ET/openet-ssebop
 .. |version| image:: https://badge.fury.io/py/openet-ssebop.svg
    :alt: Latest version on PyPI
    :target: https://badge.fury.io/py/openet-ssebop
-.. |codecov| image:: https://codecov.io/gh/Open-ET/openet-ssebop/branch/main/graphs/badge.svg
-   :alt: Coverage Status
-   :target: https://codecov.io/gh/Open-ET/openet-ssebop
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/collection.py` & `openet-ssebop-0.2.8/openet/ssebop/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,15 +440,16 @@
                         'system:time_start', ee.Date('2022-01-01').millis()))
                 elif 'LC08' in coll_id:
                     input_coll = input_coll.filter(ee.Filter.gt(
                         'system:time_start', ee.Date('2013-04-01').millis()))
 
                 def compute_vars(image):
                     model_obj = Image.from_landsat_c1_sr(
-                        sr_image=ee.Image(image), **self.model_args)
+                        sr_image=ee.Image(image), **self.model_args
+                    )
                     return model_obj.calculate(variables)
 
                 # Skip going into image class if variables is not set so raw
                 #   landsat collection can be returned for getting image_id_list
                 if variables:
                     input_coll = ee.ImageCollection(input_coll.map(compute_vars))
 
@@ -484,15 +485,16 @@
                 variables = self.variables
             else:
                 raise ValueError('variables parameter must be set')
 
         return self._build(variables=variables)
 
     def interpolate(self, variables=None, t_interval='custom',
-                    interp_method='linear', interp_days=32, **kwargs):
+                    interp_method='linear', interp_days=32, use_joins=False,
+                    **kwargs):
         """
 
         Parameters
         ----------
         variables : list, optional
             List of variables that will be returned in the Image Collection.
             If variables is not set here it must be specified in the class
@@ -502,14 +504,18 @@
             The default 'custom' interval will aggregate all days within the
             start/end dates and return an image collection with a single image.
         interp_method : {'linear}, optional
             Interpolation method (the default is 'linear').
         interp_days : int, str, optional
             Number of extra days before the start date and after the end date
             to include in the interpolation calculation. (the default is 32).
+        use_joins : bool, optional
+            If True, use joins to link the target and source collections.
+            If False, the source collection will be filtered for each target image.
+            This parameter is passed through to interpolate.daily().
         kwargs : dict, optional
 
         Returns
         -------
         ee.ImageCollection
 
         Raises
@@ -571,42 +577,42 @@
         interp_start_date = interp_start_dt.date().isoformat()
         interp_end_date = interp_end_dt.date().isoformat()
 
         # Update model_args if reference ET parameters were passed to interpolate
         # Intentionally using model_args (instead of self.et_reference_source, etc.) in
         #   this function since model_args is passed to Image class in _build()
         # if 'et' in variables or 'et_reference' in variables:
-        if ('et_reference_source' in kwargs.keys() and \
+        if ('et_reference_source' in kwargs.keys() and
                 kwargs['et_reference_source'] is not None):
             self.model_args['et_reference_source'] = kwargs['et_reference_source']
-        if ('et_reference_band' in kwargs.keys() and \
+        if ('et_reference_band' in kwargs.keys() and
                 kwargs['et_reference_band'] is not None):
             self.model_args['et_reference_band'] = kwargs['et_reference_band']
-        if ('et_reference_factor' in kwargs.keys() and \
+        if ('et_reference_factor' in kwargs.keys() and
                 kwargs['et_reference_factor'] is not None):
             self.model_args['et_reference_factor'] = kwargs['et_reference_factor']
-        if ('et_reference_resample' in kwargs.keys() and \
+        if ('et_reference_resample' in kwargs.keys() and
                 kwargs['et_reference_resample'] is not None):
             self.model_args['et_reference_resample'] = kwargs['et_reference_resample']
-        if ('et_reference_date_type' in kwargs.keys() and \
+        if ('et_reference_date_type' in kwargs.keys() and
                 kwargs['et_reference_date_type'] is not None):
             self.model_args['et_reference_date_type'] = kwargs['et_reference_date_type']
 
         # Check that all reference ET parameters were set
         # print(self.model_args)
         for et_reference_param in ['et_reference_source', 'et_reference_band',
                                    'et_reference_factor']:
             if et_reference_param not in self.model_args.keys():
                 raise ValueError(f'{et_reference_param} was not set')
             elif not self.model_args[et_reference_param]:
                 raise ValueError(f'{et_reference_param} was not set')
 
         if type(self.model_args['et_reference_source']) is str:
-            # Assume a string source is an single image collection ID
-            #   not an list of collection IDs or ee.ImageCollection
+            # Assume a string source is a single image collection ID
+            #   not a list of collection IDs or ee.ImageCollection
             if ('et_reference_date_type' not in self.model_args.keys() or
                     self.model_args['et_reference_date_type'] is None or
                     self.model_args['et_reference_date_type'].lower() == 'daily'):
                 daily_et_ref_coll = ee.ImageCollection(self.model_args['et_reference_source'])\
                     .filterDate(start_date, end_date)\
                     .select([self.model_args['et_reference_band']], ['et_reference'])
             elif self.model_args['et_reference_date_type'].lower() == 'doy':
@@ -668,30 +674,33 @@
         if 'count' in variables:
             interp_vars.append('mask')
             # interp_vars.remove('count')
 
         # Build initial scene image collection
         scene_coll = self._build(
             variables=interp_vars, start_date=interp_start_date,
-            end_date=interp_end_date)
+            end_date=interp_end_date,
+        )
 
         # For count, compute the composite/mosaic image for the mask band only
         if 'count' in variables:
             aggregate_coll = openet.core.interpolate.aggregate_to_daily(
                 image_coll=scene_coll.select(['mask']),
-                start_date=start_date, end_date=end_date)
+                start_date=start_date, end_date=end_date,
+            )
 
             # The following is needed because the aggregate collection can be
             #   empty if there are no scenes in the target date range but there
             #   are scenes in the interpolation date range.
             # Without this the count image will not be built but the other
             #   bands will be which causes a non-homogenous image collection.
             aggregate_coll = aggregate_coll.merge(
                 ee.Image.constant(0).rename(['mask'])
-                    .set({'system:time_start': ee.Date(start_date).millis()}))
+                    .set({'system:time_start': ee.Date(start_date).millis()})
+            )
 
         # Including count/mask causes problems in interpolate.daily() function.
         # Issues with mask being an int but the values need to be double.
         # Casting the mask band to a double would fix this problem also.
         if 'mask' in interp_vars:
             interp_vars.remove('mask')
 
@@ -699,24 +708,26 @@
         # NOTE: the daily function is not computing ET (ETf x ETr)
         #   but is returning the target (ETr) band
         daily_coll = openet.core.interpolate.daily(
             target_coll=daily_et_ref_coll,
             source_coll=scene_coll.select(interp_vars),
             interp_method=interp_method,
             interp_days=interp_days,
+            use_joins=use_joins,
         )
 
         # Compute ET from ET fraction and reference ET (if necessary)
-        # if 'et' in variables or 'et_fraction' in variables:
-        def compute_et(img):
-            """This function assumes reference ET and ET fraction are present"""
-            et_img = img.select(['et_fraction'])\
-                .multiply(img.select(['et_reference']))
-            return img.addBands(et_img.rename('et'))
-        daily_coll = daily_coll.map(compute_et)
+        # CGM - The conditional is needed if only interpolating NDVI
+        if 'et' in variables or 'et_fraction' in variables:
+            def compute_et(img):
+                """This function assumes reference ET and ET fraction are present"""
+                et_img = img.select(['et_fraction'])\
+                    .multiply(img.select(['et_reference']))
+                return img.addBands(et_img.rename('et'))
+            daily_coll = daily_coll.map(compute_et)
 
         interp_properties = {
             'cloud_cover_max': self.cloud_cover_max,
             'collections': ', '.join(self.collections),
             'interp_days': interp_days,
             'interp_method': interp_method,
             'model_name': openet.ssebop.MODEL_NAME,
@@ -759,15 +770,16 @@
             if 'et' in variables:
                 image_list.append(et_img.float())
             if 'et_reference' in variables:
                 image_list.append(et_reference_img.float())
             if 'et_fraction' in variables:
                 # Compute average et fraction over the aggregation period
                 image_list.append(
-                    et_img.divide(et_reference_img).rename(['et_fraction']).float())
+                    et_img.divide(et_reference_img).rename(['et_fraction']).float()
+                )
             if 'ndvi' in variables:
                 # Compute average ndvi over the aggregation period
                 ndvi_img = daily_coll \
                     .filterDate(agg_start_date, agg_end_date) \
                     .mean().select(['ndvi']).float()
                 image_list.append(ndvi_img)
             if 'count' in variables:
@@ -790,15 +802,16 @@
                 # It should be since it is coming from the interpolate source
                 #   collection, but what if source is GRIDMET (+6 UTC)?
                 agg_start_date = ee.Date(daily_img.get('system:time_start'))
                 # CGM - This calls .sum() on collections with only one image
                 return aggregate_image(
                     agg_start_date=agg_start_date,
                     agg_end_date=ee.Date(agg_start_date).advance(1, 'day'),
-                    date_format='YYYYMMdd')
+                    date_format='YYYYMMdd',
+                )
 
             return ee.ImageCollection(daily_coll.map(aggregate_daily))
 
         elif t_interval.lower() == 'monthly':
             def month_gen(iter_start_dt, iter_end_dt):
                 iter_dt = iter_start_dt
                 # Conditional is "less than" because end date is exclusive
@@ -807,15 +820,16 @@
                     iter_dt += relativedelta(months=+1)
             month_list = ee.List(list(month_gen(start_dt, end_dt)))
 
             def aggregate_monthly(agg_start_date):
                 return aggregate_image(
                     agg_start_date=agg_start_date,
                     agg_end_date=ee.Date(agg_start_date).advance(1, 'month'),
-                    date_format='YYYYMM')
+                    date_format='YYYYMM',
+                )
 
             return ee.ImageCollection(month_list.map(aggregate_monthly))
 
         elif t_interval.lower() == 'annual':
             def year_gen(iter_start_dt, iter_end_dt):
                 iter_dt = iter_start_dt
                 while iter_dt < iter_end_dt:
@@ -823,23 +837,25 @@
                     iter_dt += relativedelta(years=+1)
             year_list = ee.List(list(year_gen(start_dt, end_dt)))
 
             def aggregate_annual(agg_start_date):
                 return aggregate_image(
                     agg_start_date=agg_start_date,
                     agg_end_date=ee.Date(agg_start_date).advance(1, 'year'),
-                    date_format='YYYY')
+                    date_format='YYYY',
+                )
 
             return ee.ImageCollection(year_list.map(aggregate_annual))
 
         elif t_interval.lower() == 'custom':
             # Returning an ImageCollection to be consistent
             return ee.ImageCollection(aggregate_image(
                 agg_start_date=start_date, agg_end_date=end_date,
-                date_format='YYYYMMdd'))
+                date_format='YYYYMMdd',
+            ))
 
     def get_image_ids(self):
         """Return image IDs of the input images
 
         Returns
         -------
         list
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/image.py` & `openet-ssebop-0.2.8/openet/ssebop/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         dt_source : str, float, {'DAYMET_MEDIAN_V0', 'DAYMET_MEDIAN_V1', 'DAYMET_MEDIAN_V2'}, optional
             dT source  (the default is None).
         tcorr_source : {'DYNAMIC', 'GRIDDED', 'SCENE_GRIDDED',
                         'SCENE', 'SCENE_DAILY', 'SCENE_MONTHLY',
                         'SCENE_ANNUAL', 'SCENE_DEFAULT', or float}, optional
             Tcorr source keyword (the default is 'DYNAMIC').
         tmax_source : {'CIMIS', 'DAYMET_V3', 'DAYMET_V4', 'GRIDMET',
-                       'DAYMET_MEDIAN_V2', 'CIMIS_MEDIAN_V1', 'GRIDMET_MEDIAN_V1',
+                       'DAYMET_MEDIAN_V2', 'CIMIS_MEDIAN_V1',
                        collection ID, or float}, optional
             Maximum air temperature source.  The default is
             'projects/usgs-ssebop/tmax/daymet_v3_median_1980_2018'.
         elr_flag : bool, str, optional
             If True, apply Elevation Lapse Rate (ELR) adjustment
             (the default is False).
         dt_min : float, optional
@@ -253,15 +253,14 @@
         # if 'min_pixels_per_image' in kwargs.keys():
         #     self.min_pixels_per_image = kwargs['min_pixels_per_image']
         # else:
         #     self.min_pixels_per_image = 250
 
         # print(f'this is the tcorr source passed to the image class {tcorr_source}')
 
-
     def calculate(self, variables=['et', 'et_reference', 'et_fraction']):
         """Return a multiband image of calculated variables
 
         Parameters
         ----------
         variables : list
 
@@ -323,15 +322,16 @@
         if (self._dt_resample and type(self._dt_resample) is str and
                 self._dt_resample.lower() in ['bilinear', 'bicubic']):
             dt = self.dt.resample(self._dt_resample)
         else:
             dt = self.dt
 
         et_fraction = model.et_fraction(
-            lst=self.lst, tmax=tmax, tcorr=self.tcorr, dt=dt)
+            lst=self.lst, tmax=tmax, tcorr=self.tcorr, dt=dt
+        )
 
         # TODO: Add support for setting the conversion source dataset
         # TODO: Interpolate "instantaneous" ETo and ETr?
         # TODO: Move openet.refetgee import to top?
         # TODO: Check if etr/eto is right (I think it is)
         if self.et_fraction_type.lower() == 'grass':
             import openet.refetgee
@@ -341,20 +341,24 @@
             
             # Interpolating hourly NLDAS to the Landsat scene time
             # CGM - The 2 hour window is useful in case an image is missing
             #   I think EEMETRIC is using a 4 hour window
             # CGM - Need to check if the NLDAS images are instantaneous
             #   or some sort of average of the previous or next hour
             time_start = ee.Number(self._time_start)
-            nldas_prev_img = ee.Image(nldas_coll
+            nldas_prev_img = ee.Image(
+                nldas_coll
                 .filterDate(time_start.subtract(2 * 60 * 60 * 1000), time_start)
-                .limit(1, 'system:time_start', False).first())
-            nldas_next_img = ee.Image(nldas_coll
+                .limit(1, 'system:time_start', False).first()
+            )
+            nldas_next_img = ee.Image(
+                nldas_coll
                 .filterDate(time_start, time_start.add(2 * 60 * 60 * 1000))
-                .first())
+                .first()
+            )
             nldas_prev_time = ee.Number(nldas_prev_img.get('system:time_start'))
             nldas_next_time = ee.Number(nldas_next_img.get('system:time_start'))
             time_ratio = time_start.subtract(nldas_prev_time)\
                 .divide(nldas_next_time.subtract(nldas_prev_time))
             nldas_img = nldas_next_img.subtract(nldas_prev_img)\
                 .multiply(time_ratio).add(nldas_prev_img)\
                 .set({'system:time_start': self._time_start})
@@ -390,15 +394,15 @@
                     .select([self.et_reference_band])
             elif self.et_reference_date_type.lower() == 'doy':
                 # Assume the image collection is a climatology with a "DOY" property
                 et_reference_coll = ee.ImageCollection(self.et_reference_source)\
                     .filter(ee.Filter.rangeContains('DOY', self._doy, self._doy))\
                     .select([self.et_reference_band])
                 #     .limit(1, 'system:time_start', True)
-
+                # DEADBEEF
                 # # CGM - Is this mapped function over GRIDMET really needed?
                 # #   Couldn't you just filter the source to the image DOY
                 # def et_reference_replace_daily(image):
                 #     """Mapping function to get daily time_start and system:index
                 #
                 #     Returns the doy-based reference et with daily time properties from GRIDMET
                 #     """
@@ -537,67 +541,76 @@
             dt_img = ee.Image(dt_coll.first()).clamp(self._dt_min, self._dt_max)
         elif self._dt_source.upper() == 'CIMIS':
             # CGM - Should we check this here or catch the exception in elev()
             # if self._elev_source is None:
             #     raise Exception('elev_source must be set if dt_source="CIMIS"')
             input_img = ee.Image(
                 ee.ImageCollection('projects/earthengine-legacy/assets/'
-                                   'projects/climate-engine/cimis/daily')\
-                    .filterDate(self._start_date, self._end_date)\
-                    .select(['Tx', 'Tn', 'Rs', 'Tdew'])\
-                    .first())
+                                   'projects/climate-engine/cimis/daily')
+                .filterDate(self._start_date, self._end_date)
+                .select(['Tx', 'Tn', 'Rs', 'Tdew'])
+                .first()
+            )
             # Convert units to T [K], Rs [MJ m-2 d-1], ea [kPa]
             # Compute Ea from Tdew
             dt_img = model.dt(
                 tmax=input_img.select(['Tx']).add(273.15),
                 tmin=input_img.select(['Tn']).add(273.15),
                 rs=input_img.select(['Rs']),
                 ea=input_img.select(['Tdew']).add(237.3).pow(-1)
-                    .multiply(input_img.select(['Tdew']))\
-                    .multiply(17.27).exp().multiply(0.6108).rename(['ea']),
+                    .multiply(input_img.select(['Tdew']))
+                    .multiply(17.27).exp().multiply(0.6108),
                 elev=self.elev,
-                doy=self._doy).clamp(self._dt_min, self._dt_max)
+                doy=self._doy,
+            )
+            dt_img = dt_img.clamp(self._dt_min, self._dt_max)
         elif self._dt_source.upper() == 'DAYMET':
             input_img = ee.Image(
-                ee.ImageCollection('NASA/ORNL/DAYMET_V3')\
-                    .filterDate(self._start_date, self._end_date)\
-                    .select(['tmax', 'tmin', 'srad', 'dayl', 'vp'])\
-                    .first())
+                ee.ImageCollection('NASA/ORNL/DAYMET_V3')
+                .filterDate(self._start_date, self._end_date)
+                .select(['tmax', 'tmin', 'srad', 'dayl', 'vp'])
+                .first()
+            )
             # Convert units to T [K], Rs [MJ m-2 d-1], ea [kPa]
             # Solar unit conversion from DAYMET documentation:
             #   https://daymet.ornl.gov/overview.html
             dt_img = model.dt(
                 tmax=input_img.select(['tmax']).add(273.15),
                 tmin=input_img.select(['tmin']).add(273.15),
-                rs=input_img.select(['srad'])\
-                    .multiply(input_img.select(['dayl'])).divide(1000000),
+                rs=input_img.select(['srad']).multiply(input_img.select(['dayl']))
+                    .divide(1000000),
                 ea=input_img.select(['vp'], ['ea']).divide(1000),
                 elev=self.elev,
-                doy=self._doy).clamp(self._dt_min, self._dt_max)
+                doy=self._doy,
+            )
+            dt_img = dt_img.clamp(self._dt_min, self._dt_max)
         elif self._dt_source.upper() == 'GRIDMET':
             input_img = ee.Image(
-                ee.ImageCollection('IDAHO_EPSCOR/GRIDMET')\
-                    .filterDate(self._start_date, self._end_date)\
-                    .select(['tmmx', 'tmmn', 'srad', 'sph'])\
-                    .first())
+                ee.ImageCollection('IDAHO_EPSCOR/GRIDMET')
+                .filterDate(self._start_date, self._end_date)
+                .select(['tmmx', 'tmmn', 'srad', 'sph'])
+                .first()
+            )
             # Convert units to T [K], Rs [MJ m-2 d-1], ea [kPa]
             q = input_img.select(['sph'], ['q'])
             pair = self.elev.multiply(-0.0065).add(293.0).divide(293.0).pow(5.26)\
                 .multiply(101.3)
             # pair = self.elev.expression(
             #     '101.3 * pow((293.0 - 0.0065 * elev) / 293.0, 5.26)',
-            #     {'elev': self.elev})
+            #     {'elev': self.elev}
+            # )
             dt_img = model.dt(
                 tmax=input_img.select(['tmmx']),
                 tmin=input_img.select(['tmmn']),
                 rs=input_img.select(['srad']).multiply(0.0864),
-                ea=q.multiply(0.378).add(0.622).pow(-1).multiply(q)\
-                    .multiply(pair).rename(['ea']),
+                ea=q.multiply(0.378).add(0.622).pow(-1).multiply(q).multiply(pair),
                 elev=self.elev,
-                doy=self._doy).clamp(self._dt_min, self._dt_max)
+                doy=self._doy,
+            )
+            dt_img = dt_img.clamp(self._dt_min, self._dt_max)
         else:
             raise ValueError('Invalid dt_source: {}\n'.format(self._dt_source))
 
         ## MF: moved this resample to happen at the et_fraction function
         # if (self._dt_resample and
         #         self._dt_resample.lower() in ['bilinear', 'bicubic']):
         #     dt_img = dt_img.resample(self._dt_resample)
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/interpolate.py` & `openet-ssebop-0.2.8/openet/ssebop/interpolate.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,16 +154,16 @@
         et_reference_date_type = model_args['et_reference_date_type']
     else:
         et_reference_date_type = None
         # logging.debug('et_reference_date_type was not set, default to "daily"')
         # et_reference_date_type = 'daily'
 
     if type(et_reference_source) is str:
-        # Assume a string source is an single image collection ID
-        #   not an list of collection IDs or ee.ImageCollection
+        # Assume a string source is a single image collection ID
+        #   not a list of collection IDs or ee.ImageCollection
         if (et_reference_date_type is None or
                 et_reference_date_type.lower() == 'daily'):
             daily_et_ref_coll = ee.ImageCollection(et_reference_source) \
                 .filterDate(start_date, end_date) \
                 .select([et_reference_band], ['et_reference'])
         elif et_reference_date_type.lower() == 'doy':
             # Assume the image collection is a climatology with a "DOY" property
@@ -220,42 +220,44 @@
     # This probably isn't needed since scene_coll was built to this range
     scene_coll = scene_coll.filterDate(interp_start_date, interp_end_date)
 
     # For count, compute the composite/mosaic image for the mask band only
     if 'count' in variables:
         aggregate_coll = openet.core.interpolate.aggregate_to_daily(
             image_coll = scene_coll.select(['mask']),
-            start_date=start_date, end_date=end_date)
+            start_date=start_date, end_date=end_date,
+        )
 
         # The following is needed because the aggregate collection can be
         #   empty if there are no scenes in the target date range but there
         #   are scenes in the interpolation date range.
         # Without this the count image will not be built but the other
         #   bands will be which causes a non-homogeneous image collection.
         aggregate_coll = aggregate_coll.merge(
             ee.Image.constant(0).rename(['mask'])
-                .set({'system:time_start': ee.Date(start_date).millis()}))
+                .set({'system:time_start': ee.Date(start_date).millis()})
+        )
 
     # Interpolate to a daily time step
     # NOTE: the daily function is not computing ET (ETf x ETr)
     #   but is returning the target (ETr) band
     daily_coll = openet.core.interpolate.daily(
         target_coll=daily_et_ref_coll,
         source_coll=scene_coll.select(interp_vars),
-        interp_method=interp_method, interp_days=interp_days,
+        interp_method=interp_method,
+        interp_days=interp_days,
         use_joins=use_joins,
     )
 
     # Compute ET from ETf and ETr (if necessary)
     # The check for et_fraction is needed since it is back computed from ET and ETr
     # if 'et' in variables or 'et_fraction' in variables:
     def compute_et(img):
         """This function assumes ETr and ETf are present"""
-        et_img = img.select(['et_fraction']) \
-            .multiply(img.select(['et_reference']))
+        et_img = img.select(['et_fraction']).multiply(img.select(['et_reference']))
         return img.addBands(et_img.double().rename('et'))
 
     daily_coll = daily_coll.map(compute_et)
 
     def aggregate_image(agg_start_date, agg_end_date, date_format):
         """Aggregate the daily images within the target date range
 
@@ -291,16 +293,16 @@
         if 'et' in variables:
             image_list.append(et_img.float())
         if 'et_reference' in variables:
             image_list.append(et_reference_img.float())
         if 'et_fraction' in variables:
             # Compute average et fraction over the aggregation period
             image_list.append(
-                et_img.divide(et_reference_img).rename(
-                    ['et_fraction']).float())
+                et_img.divide(et_reference_img).rename(['et_fraction']).float()
+            )
         if 'ndvi' in variables:
             # Compute average ndvi over the aggregation period
             ndvi_img = daily_coll \
                 .filterDate(agg_start_date, agg_end_date) \
                 .mean().select(['ndvi']).float()
             image_list.append(ndvi_img)
         if 'count' in variables:
@@ -322,15 +324,16 @@
             # It should be since it is coming from the interpolate source
             #   collection, but what if source is GRIDMET (+6 UTC)?
             agg_start_date = ee.Date(daily_img.get('system:time_start'))
             # CGM - This calls .sum() on collections with only one image
             return aggregate_image(
                 agg_start_date=agg_start_date,
                 agg_end_date=ee.Date(agg_start_date).advance(1, 'day'),
-                date_format='YYYYMMdd')
+                date_format='YYYYMMdd',
+            )
 
         return ee.ImageCollection(daily_coll.map(agg_daily))
 
     elif t_interval.lower() == 'monthly':
         def month_gen(iter_start_dt, iter_end_dt):
             iter_dt = iter_start_dt
             # Conditional is "less than" because end date is exclusive
@@ -340,15 +343,16 @@
 
         month_list = ee.List(list(month_gen(start_dt, end_dt)))
 
         def agg_monthly(agg_start_date):
             return aggregate_image(
                 agg_start_date=agg_start_date,
                 agg_end_date=ee.Date(agg_start_date).advance(1, 'month'),
-                date_format='YYYYMM')
+                date_format='YYYYMM',
+            )
 
         return ee.ImageCollection(month_list.map(agg_monthly))
 
     elif t_interval.lower() == 'annual':
         def year_gen(iter_start_dt, iter_end_dt):
             iter_dt = iter_start_dt
             while iter_dt < iter_end_dt:
@@ -357,16 +361,18 @@
 
         year_list = ee.List(list(year_gen(start_dt, end_dt)))
 
         def agg_annual(agg_start_date):
             return aggregate_image(
                 agg_start_date=agg_start_date,
                 agg_end_date=ee.Date(agg_start_date).advance(1, 'year'),
-                date_format='YYYY')
+                date_format='YYYY',
+            )
 
         return ee.ImageCollection(year_list.map(agg_annual))
 
     elif t_interval.lower() == 'custom':
         # Returning an ImageCollection to be consistent
         return ee.ImageCollection(aggregate_image(
             agg_start_date=start_date, agg_end_date=end_date,
-            date_format='YYYYMMdd'))
+            date_format='YYYYMMdd',
+        ))
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/ipytest.py` & `openet-ssebop-0.2.8/openet/ssebop/ipytest.py`

 * *Files identical despite different names*

### Comparing `openet-ssebop-0.2.6/openet/ssebop/landsat.py` & `openet-ssebop-0.2.8/openet/ssebop/landsat.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,36 +20,39 @@
         Remote Sensing of Environment, 90(4), 434-440.
         https://doi.org/10.1016/j.rse.2004.02.003
 
     """
     ndvi_img = ndvi(landsat_image)
     Pv = ndvi_img.expression('((ndvi - 0.2) / 0.3) ** 2', {'ndvi': ndvi_img})
     # ndviRangevalue = ndvi_image.where(
-    #     ndvi_image.gte(0.2).And(ndvi_image.lte(0.5)), ndvi_image)
+    #     ndvi_image.gte(0.2).And(ndvi_image.lte(0.5)), ndvi_image
+    # )
     # Pv = ndviRangevalue.expression(
     #     '(((ndviRangevalue - 0.2) / 0.3) ** 2',
-    #     {'ndviRangevalue':ndviRangevalue})
+    #     {'ndviRangevalue':ndviRangevalue}
+    # )
 
     # Assuming typical Soil Emissivity of 0.97 and Veg Emissivity of 0.99
     #   and shape Factor mean value of 0.553
     dE = Pv.expression(
-        '(1 - 0.97) * (1 - Pv) * (0.55 * 0.99)', {'Pv': Pv})
+        '(1 - 0.97) * (1 - Pv) * (0.55 * 0.99)', {'Pv': Pv}
+    )
     RangeEmiss = dE.expression(
-        '(0.99 * Pv) + (0.97 * (1 - Pv)) + dE', {'Pv': Pv, 'dE': dE})
+        '(0.99 * Pv) + (0.97 * (1 - Pv)) + dE', {'Pv': Pv, 'dE': dE}
+    )
 
-    # RangeEmiss = 0.989 # dE.expression(
-    #  '((0.99 * Pv) + (0.97 * (1 - Pv)) + dE)', {'Pv':Pv, 'dE':dE})
-    return ndvi_img\
-        .where(ndvi_img.lt(0), 0.985)\
-        .where(ndvi_img.gte(0).And(ndvi_img.lt(0.2)), 0.977)\
-        .where(ndvi_img.gt(0.5), 0.99)\
-        .where(ndvi_img.gte(0.2).And(ndvi_img.lte(0.5)), RangeEmiss)\
-        .clamp(0.977, 0.99)\
+    return (
+        ndvi_img
+        .where(ndvi_img.lt(0), 0.985)
+        .where(ndvi_img.gte(0).And(ndvi_img.lt(0.2)), 0.977)
+        .where(ndvi_img.gt(0.5), 0.99)
+        .where(ndvi_img.gte(0.2).And(ndvi_img.lte(0.5)), RangeEmiss)
+        .clamp(0.977, 0.99)
         .rename(['emissivity'])
-
+    )
 
 
 def lst(landsat_image):
     """Emissivity corrected land surface temperature (LST) from brightness Ts.
 
     Parameters
     ----------
@@ -89,26 +92,29 @@
     ts_brightness = ee.Image(landsat_image).select(['tir'])
     emissivity_img = emissivity(landsat_image)
 
     # First back out radiance from brightness temperature
     # Then recalculate emissivity corrected Ts
     thermal_rad_toa = ts_brightness.expression(
         'k1 / (exp(k2 / ts_brightness) - 1)',
-        {'ts_brightness': ts_brightness, 'k1': k1, 'k2': k2})
+        {'ts_brightness': ts_brightness, 'k1': k1, 'k2': k2}
+    )
 
     rc = thermal_rad_toa.expression(
         '((thermal_rad_toa - rp) / tnb) - ((1 - emiss) * rsky)',
         {
             'thermal_rad_toa': thermal_rad_toa,
             'emiss': emissivity_img,
             'rp': 0.91, 'tnb': 0.866, 'rsky': 1.32,
-        })
+        }
+    )
     lst = rc.expression(
         'k2 / log(emiss * k1 / rc + 1)',
-        {'emiss': emissivity_img, 'rc': rc, 'k1': k1, 'k2': k2})
+        {'emiss': emissivity_img, 'rc': rc, 'k1': k1, 'k2': k2}
+    )
 
     return lst.rename(['lst'])
 
 
 def ndvi(landsat_image):
     """Normalized difference vegetation index
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/model.py` & `openet-ssebop-0.2.8/openet/ssebop/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,20 +29,23 @@
     -----
     Clamping function assumes this is an alfalfa fraction.
 
     """
 
     et_fraction = lst.expression(
         '(lst * (-1) + tmax * tcorr + dt) / dt',
-        {'tmax': tmax, 'dt': dt, 'lst': lst, 'tcorr': tcorr})
+        {'tmax': tmax, 'dt': dt, 'lst': lst, 'tcorr': tcorr}
+    )
 
-    return et_fraction\
-        .updateMask(et_fraction.lte(2.0))\
-        .clamp(0, 1.0)\
+    return (
+        et_fraction
+        .updateMask(et_fraction.lte(2.0))
+        .clamp(0, 1.0)
         .rename(['et_fraction'])
+    )
 
 
 def dt(tmax, tmin, elev, doy, lat=None, rs=None, ea=None):
     """Temperature difference between hot/dry ground and cold/wet canopy
 
     Parameters
     ----------
@@ -91,22 +94,22 @@
     # Convert latitude to radians
     phi = lat.multiply(math.pi / 180)
 
     # Make a DOY image from the DOY number
     doy = tmax.multiply(0).add(doy)
 
     # Extraterrestrial radiation (Ra) (FAO56 Eqns 24, 25, 23, 21)
-    delta = doy.multiply(2 * math.pi / 365).subtract(1.39).sin()\
-        .multiply(0.409)
+    delta = doy.multiply(2 * math.pi / 365).subtract(1.39).sin().multiply(0.409)
     ws = phi.tan().multiply(-1).multiply(delta.tan()).acos()
     dr = doy.multiply(2 * math.pi / 365).cos().multiply(0.033).add(1)
-    ra = ws.multiply(phi.sin()).multiply(delta.sin())\
-        .add(phi.cos().multiply(delta.cos()).multiply(ws.sin()))\
-        .multiply(dr)\
-        .multiply((1367.0 / math.pi) * 0.0820)
+    ra = (
+        ws.multiply(phi.sin()).multiply(delta.sin())
+        .add(phi.cos().multiply(delta.cos()).multiply(ws.sin()))
+        .multiply(dr).multiply((1367.0 / math.pi) * 0.0820)
+    )
 
     # Simplified clear sky solar formulation (Rso) [MJ m-2 d-1] (Eqn 37)
     rso = elev.multiply(2E-5).add(0.75).multiply(ra)
 
     # Derive cloudiness fraction from Rs and Rso (see FAO56 Eqn 39)
     # Use Rso for Rs if not set
     if rs is None:
@@ -117,32 +120,35 @@
         # fcd = rs.divide(rso).clamp(0.3, 1).multiply(1.35).subtract(0.35)
 
     # Net shortwave radiation [MJ m-2 d-1] (FAO56 Eqn 38)
     rns = rs.multiply(1 - 0.23)
 
     # Actual vapor pressure [kPa] (FAO56 Eqn 14)
     if ea is None:
-        ea = tmin.subtract(273.15).multiply(17.27)\
-            .divide(tmin.subtract(273.15).add(237.3)).exp().multiply(0.6108)
+        ea = (
+            tmin.subtract(273.15).multiply(17.27)
+            .divide(tmin.subtract(273.15).add(237.3))
+            .exp().multiply(0.6108)
+        )
 
     # Net longwave radiation [MJ m-2 d-1] (FAO56 Eqn 39)
-    rnl = tmax.pow(4).add(tmin.pow(4))\
-        .multiply(ea.sqrt().multiply(-0.14).add(0.34))\
+    rnl = (
+        tmax.pow(4).add(tmin.pow(4))
+        .multiply(ea.sqrt().multiply(-0.14).add(0.34))
         .multiply(4.901E-9 * 0.5).multiply(fcd)
+    )
 
     # Net radiation [MJ m-2 d-1] (FAO56 Eqn 40)
     rn = rns.subtract(rnl)
 
     # Air pressure [kPa] (FAO56 Eqn 7)
-    pair = elev.multiply(-0.0065).add(293.0).divide(293.0).pow(5.26)\
-        .multiply(101.3)
+    pair = elev.multiply(-0.0065).add(293.0).divide(293.0).pow(5.26).multiply(101.3)
 
     # Air density [Kg m-3] (Senay2018 A.11 & A.13)
-    den = tmax.add(tmin).multiply(0.5).pow(-1).multiply(pair)\
-        .multiply(3.486 / 1.01)
+    den = tmax.add(tmin).multiply(0.5).pow(-1).multiply(pair).multiply(3.486 / 1.01)
 
     # Temperature difference [K] (Senay2018 A.5)
     dt = rn.divide(den).multiply(110.0 / ((1.013 / 1000) * 86400))
 
     return dt
 
 
@@ -161,18 +167,17 @@
     Returns
     -------
     ee.Image
 
     """
     elr_adjust = ee.Image(temperature).expression(
         '(temperature - (0.003 * (elev - threshold)))',
-        {
-            'temperature': temperature, 'elev': elev,
-            'threshold': lapse_threshold
-        })
+        {'temperature': temperature, 'elev': elev, 'threshold': lapse_threshold}
+    )
+
     return ee.Image(temperature).where(elev.gt(lapse_threshold), elr_adjust)
 
 
 def elr_adjust(temperature, elevation, radius=80):
     """Elevation Lapse Rate (ELR) adjusted temperature [K]
 
     Parameters
@@ -205,19 +210,20 @@
     elev_tmax_fine = elev_img.reproject(crs=tmax_projection)
     # elev_tmax_fine = elev_img.resample('bilinear').reproject(crs=tmax_projection)
     # elev_tmax_fine = elev_img\
     #     .reduceResolution(reducer=ee.Reducer.median(), maxPixels=65536)\
     #     .reproject(crs=tmax_projection)
 
     # Then generate the smoothed elevation image
-    elev_tmax_smoothed = elev_tmax_fine\
+    elev_tmax_smoothed = (
+        elev_tmax_fine
         .reduceNeighborhood(reducer=ee.Reducer.median(),
-                            kernel=ee.Kernel.square(radius=radius,
-                                                    units='pixels'))\
+                            kernel=ee.Kernel.square(radius=radius, units='pixels'))
         .reproject(crs=tmax_projection)
+    )
 
     # Final ELR mask: (DEM-(medDEM.add(100)).gt(0))
     elev_diff = elev_tmax_fine.subtract(elev_tmax_smoothed.add(100))
     elr_mask = elev_diff.gt(0)
 
     # temperature - (0.005 * (elr_layer))
     elr_adjust = tmax_img.subtract(elev_diff.multiply(0.005))
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/tests/conftest.py` & `openet-ssebop-0.2.8/openet/ssebop/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openet-ssebop-0.2.6/openet/ssebop/tests/test_a_utils.py` & `openet-ssebop-0.2.8/openet/ssebop/tests/test_a_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,25 @@
 import openet.ssebop.utils as utils
 
 
 def test_getinfo():
     assert utils.getinfo(ee.Number(1)) == 1
 
 
+def test_getinfo_exception():
+    with pytest.raises(Exception):
+        utils.getinfo('deadbeef')
+
+
+# # CGM - Not sure how to trigger an EEException to test that the output is None
+# #   This fails before it is sent to the getinfo function
+# def test_getinfo_eeexception():
+#     assert utils.getinfo(ee.Number('deadbeef')) is None
+
+
 def test_constant_image_value(tol=0.000001):
     expected = 10.123456789
     input_img = ee.Image.constant(expected)
     output = utils.constant_image_value(input_img)
     assert abs(output['constant'] - expected) <= tol
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/tests/test_b_landsat.py` & `openet-ssebop-0.2.8/openet/ssebop/tests/test_b_landsat.py`

 * *Files identical despite different names*

### Comparing `openet-ssebop-0.2.6/openet/ssebop/tests/test_b_model.py` & `openet-ssebop-0.2.8/openet/ssebop/tests/test_b_model.py`

 * *Files identical despite different names*

### Comparing `openet-ssebop-0.2.6/openet/ssebop/tests/test_c_image.py` & `openet-ssebop-0.2.8/openet/ssebop/tests/test_c_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -273,16 +273,14 @@
     output = utils.point_image_value(ee.Image(m.dt), xy)
     assert abs(output['dt'] - expected) <= tol
 
 
 @pytest.mark.parametrize(
     'dt_source, doy, xy, expected',
     [
-        ['DAYMET_MEDIAN_V0', SCENE_DOY, TEST_POINT, 19.4612],
-        ['DAYMET_MEDIAN_V0', 194, [-120.113, 36.336], 19.262],
         ['DAYMET_MEDIAN_V1', SCENE_DOY, TEST_POINT, 18],
         ['DAYMET_MEDIAN_V1', 194, [-120.113, 36.336], 18],
         ['DAYMET_MEDIAN_V1', 194, [-119.0, 37.5], 21],
         ['DAYMET_MEDIAN_V2', SCENE_DOY, TEST_POINT, 19.5982],
         ['DAYMET_MEDIAN_V2', 194, [-120.113, 36.336], 19.4762],
         ['DAYMET_MEDIAN_V2', 194, [-119.0, 37.5], 25],
     ]
@@ -294,16 +292,14 @@
     output = utils.point_image_value(ee.Image(m.dt), xy)
     assert abs(output['dt'] - expected) <= tol
 
 
 @pytest.mark.parametrize(
     'dt_source, doy, xy, expected',
     [
-        ['DAYMET_MEDIAN_V0', 1, [-120.113, 36.336], 5],
-        ['DAYMET_MEDIAN_V0', 194, [-119.0, 37.5], 25],
         ['DAYMET_MEDIAN_V1', 1, [-120.113, 36.336], 5],
         # ['DAYMET_MEDIAN_V1', 194, [-119.0, 37.5], 25],
         ['DAYMET_MEDIAN_V2', 1, [-96.6255, 43.7359], 5],
         ['DAYMET_MEDIAN_V2', 194, [-119.0, 37.5], 25],
     ]
 )
 def test_Image_dt_source_clamping(dt_source, doy, xy, expected, tol=0.001):
@@ -424,24 +420,20 @@
         ['DAYMET_MEDIAN_V2', TEST_POINT, 310.15],
         ['CIMIS', [-120.113, 36.336], 307.725],
         ['DAYMET_V3', [-120.113, 36.336], 308.150],
         ['DAYMET_V4', [-120.113, 36.336], 308.500],
         ['GRIDMET', [-120.113, 36.336], 306.969],
         # ['TOPOWX', [-120.113, 36.336], 301.67],
         ['CIMIS_MEDIAN_V1', [-120.113, 36.336], 308.946],
-        ['DAYMET_MEDIAN_V0', [-120.113, 36.336], 310.150],
         ['DAYMET_MEDIAN_V1', [-120.113, 36.336], 310.150],
         ['DAYMET_MEDIAN_V2', [-120.113, 36.336], 310.150],
         # Added extra test point where DAYMET median values differ
         # TEST_POINT, [-119.0, 37.5], [-122.1622, 39.1968], [-106.03249, 37.17777]
-        ['DAYMET_MEDIAN_V0', [-122.1622, 39.1968], 308.15],
         ['DAYMET_MEDIAN_V1', [-122.1622, 39.1968], 308.4],
         ['DAYMET_MEDIAN_V2', [-122.1622, 39.1968], 308.65],
-        ['GRIDMET_MEDIAN_V1', [-120.113, 36.336], 310.436],
-        ['TOPOWX_MEDIAN_V0', [-120.113, 36.336], 310.430],
         # Check string/float constant values
         ['305', [-120.113, 36.336], 305],
         [305, [-120.113, 36.336], 305],
     ]
 )
 def test_Image_tmax_source_values(tmax_source, xy, expected, tol=0.001):
     """Test getting Tmax values for a single date at a real point"""
@@ -475,19 +467,16 @@
         ['projects/usgs-ssebop/tmax/daymet_v4_median_1980_2019', {}],
         ['CIMIS', {}],
         ['DAYMET_V3', {}],
         ['DAYMET_V4', {}],
         ['GRIDMET', {}],
         # ['TOPOWX', {}],
         ['CIMIS_MEDIAN_V1', {}],
-        ['DAYMET_MEDIAN_V0', {}],
         ['DAYMET_MEDIAN_V1', {}],
         ['DAYMET_MEDIAN_V2', {}],
-        ['GRIDMET_MEDIAN_V1', {}],
-        ['TOPOWX_MEDIAN_V0', {}],
         ['305', {'tmax_source': 'custom_305'}],
         [305, {'tmax_source': 'custom_305'}],
     ]
 )
 def test_Image_tmax_properties(tmax_source, expected):
     """Test if properties are set on the Tmax image"""
     output = utils.getinfo(default_image_obj(tmax_source=tmax_source).tmax)
@@ -781,22 +770,14 @@
     assert output['tcorr_count'] == count
 
 
 # NOTE: These values seem to change by small amounts for no reason
 @pytest.mark.parametrize(
     'image_id, tmax_source, expected',
     [
-        # TOPOWX_MEDIAN_V0
-        ['LANDSAT/LC08/C01/T1_TOA/LC08_044033_20170716', 'TOPOWX_MEDIAN_V0',
-         {'tcorr_value': 0.9914826142535333, 'tcorr_count': 457876}],
-        ['LANDSAT/LE07/C01/T1_TOA/LE07_044033_20170708', 'TOPOWX_MEDIAN_V0',
-         {'tcorr_value': 0.9810607908548545, 'tcorr_count': 21852}],
-        ['LANDSAT/LT05/C01/T1_TOA/LT05_044033_20110716', 'TOPOWX_MEDIAN_V0',
-         {'tcorr_value': 0.9571767539172935, 'tcorr_count': 872}],
-
         # DAYMET_MEDIAN_V2
         ['LANDSAT/LC08/C01/T1_TOA/LC08_042035_20150713', 'DAYMET_MEDIAN_V2',
          {'tcorr_value': 0.9730285325301501, 'tcorr_count': 152720}],
         ['LANDSAT/LC08/C01/T1_TOA/LC08_044033_20170716', 'DAYMET_MEDIAN_V2',
          {'tcorr_value': 0.9856133291233087, 'tcorr_count': 457876}],
         ['LANDSAT/LE07/C01/T1_TOA/LE07_044033_20170708', 'DAYMET_MEDIAN_V2',
          {'tcorr_value': 0.9798477638345092, 'tcorr_count': 21852}],
@@ -963,20 +944,14 @@
 
 
 # TODO: Modify these tests for the DYNAMIC tcorr source
 #   to check that the monthly and annual fallback collections are used
 # @pytest.mark.parametrize(
 #     'tcorr_source, tmax_source, scene_id, expected',
 #     [
-#         # TOPOWX_MEDIAN_V0
-#         ['IMAGE', 'TOPOWX_MEDIAN_V0', 'LC08_042035_20150713', [0.9752, 0]],
-#         ['IMAGE_DAILY', 'TOPOWX_MEDIAN_V0', 'LC08_042035_20150713', [0.9752, 0]],
-#         ['IMAGE_MONTHLY', 'TOPOWX_MEDIAN_V0', 'LC08_042035_20150713', [0.9723, 1]],
-#         ['IMAGE_ANNUAL', 'TOPOWX_MEDIAN_V0', 'LC08_042035_20150713', [0.9786, 2]],
-#         ['IMAGE_DEFAULT', 'TOPOWX_MEDIAN_V0', 'LC08_042035_20150713', [0.978, 3]],
 #         # DAYMET_MEDIAN_V2
 #         ['IMAGE', 'DAYMET_MEDIAN_V2', 'LC08_042035_20150713', [0.9744, 0]],
 #         ['IMAGE_DAILY', 'DAYMET_MEDIAN_V2', 'LC08_042035_20150713', [0.9744, 0]],
 #         ['IMAGE_MONTHLY', 'DAYMET_MEDIAN_V2', 'LC08_042035_20150713', [0.9756, 1]],
 #         ['IMAGE_ANNUAL', 'DAYMET_MEDIAN_V2', 'LC08_042035_20150713', [0.9829, 2]],
 #         ['IMAGE_DEFAULT', 'DAYMET_MEDIAN_V2', 'LC08_042035_20150713', [0.978, 3]],
 #     ]
@@ -1589,14 +1564,17 @@
 @pytest.mark.parametrize(
     'source, band, factor, xy, expected',
     [
         ['IDAHO_EPSCOR/GRIDMET', 'etr', 1, TEST_POINT, 9.5730],
         ['IDAHO_EPSCOR/GRIDMET', 'etr', 0.85, TEST_POINT, 9.5730 * 0.85],
         ['projects/earthengine-legacy/assets/projects/climate-engine/cimis/daily',
          'ETr_ASCE', 1, TEST_POINT, 10.0220],
+        # CGM - Why are these not the same?
+        ['projects/earthengine-legacy/assets/projects/openet/reference_et/cimis/daily',
+         'etr_asce', 1, TEST_POINT, 10.0760],
         [10, 'FOO', 1, TEST_POINT, 10.0],
         [10, 'FOO', 0.85, TEST_POINT, 8.5],
     ]
 )
 def test_Image_et_reference_source(source, band, factor, xy, expected,
                                    tol=0.001):
     """Test getting reference ET values for a single date at a real point"""
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/tests/test_d_collection.py` & `openet-ssebop-0.2.8/openet/ssebop/tests/test_d_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,14 +407,22 @@
     """Default t_interval should be custom"""
     output = utils.getinfo(default_coll_obj().interpolate())
     assert output['type'] == 'ImageCollection'
     assert parse_scene_id(output) == ['20170701']
     assert {y['id'] for x in output['features'] for y in x['bands']} == VARIABLES
 
 
+@pytest.mark.parametrize('use_joins', [True, False])
+def test_Collection_interpolate_use_joins(use_joins):
+    """Only checking if the parameter is accepted and runs for now"""
+    output = utils.getinfo(default_coll_obj().interpolate(use_joins=use_joins))
+    assert output['type'] == 'ImageCollection'
+    assert parse_scene_id(output) == ['20170701']
+
+
 def test_Collection_interpolate_variables_custom():
     output = utils.getinfo(default_coll_obj().interpolate(variables=['et']))
     assert [y['id'] for x in output['features'] for y in x['bands']] == ['et']
 
 
 def test_Collection_interpolate_t_interval_daily():
     """Test if the daily time interval parameter works
@@ -434,15 +442,15 @@
     output = utils.getinfo(default_coll_obj().interpolate(t_interval='monthly'))
     assert output['type'] == 'ImageCollection'
     assert parse_scene_id(output) == ['201707']
     assert {y['id'] for x in output['features'] for y in x['bands']} == VARIABLES
 
 
 # CGM - Commenting out since it takes a really long time to run
-#   This function could probably be be tested for a shorter time period
+#   This function could probably be tested for a shorter time period
 # def test_Collection_interpolate_t_interval_annual():
 #     """Test if the annual time interval parameter works"""
 #     coll_obj = default_coll_obj(start_date='2017-01-01', end_date='2018-01-01')
 #     output = utils.getinfo(coll_obj.interpolate(t_interval='annual'))
 #     assert output['type'] == 'ImageCollection'
 #     assert parse_scene_id(output) == ['2017']
 #     assert {y['id'] for x in output['features'] for y in x['bands']} == VARIABLES
@@ -603,22 +611,25 @@
 
 
 def test_Collection_interpolate_daily_et_reference_date_type_doy(tol=0.01):
     """Test interpolating a daily collection using a reference ET climatology"""
     output_coll = default_coll_obj(
         collections=['LANDSAT/LC08/C02/T1_L2'],
         geometry=ee.Geometry.Point(TEST_POINT),
-        start_date=START_DATE, end_date=END_DATE,
+        # CGM - Testing the full month returns a memory error
+        start_date='2017-07-01', end_date='2017-07-10',
+        # start_date=START_DATE, end_date=END_DATE,
         variables=['et_reference'],
         et_reference_source='projects/usgs-ssebop/pet/gridmet_median_v1',
         et_reference_band='etr', et_reference_factor=1.0,
         et_reference_resample='nearest', et_reference_date_type='doy',
         ).interpolate(t_interval='daily')
     output = utils.point_coll_value(output_coll, TEST_POINT, scale=10)
-    assert abs(output['et_reference'][START_DATE] - 8.75) <= tol
+    assert abs(output['et_reference']['2017-07-01'] - 8.75) <= tol
+    # assert abs(output['et_reference'][START_DATE] - 8.75) <= tol
 
 
 def test_Collection_interpolate_monthly_et_reference_date_type_doy(tol=0.01):
     """Test interpolating a monthly collection using a reference ET climatology"""
     output_coll = default_coll_obj(
         collections=['LANDSAT/LC08/C02/T1_L2'],
         geometry=ee.Geometry.Point(TEST_POINT),
```

### Comparing `openet-ssebop-0.2.6/openet/ssebop/tests/test_d_interpolate.py` & `openet-ssebop-0.2.8/openet/ssebop/tests/test_d_interpolate.py`

 * *Files identical despite different names*

### Comparing `openet-ssebop-0.2.6/openet/ssebop/utils.py` & `openet-ssebop-0.2.8/openet/ssebop/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 def getinfo(ee_obj, n=4):
     """Make an exponential back off getInfo call on an Earth Engine object"""
     output = None
     for i in range(1, n):
         try:
             output = ee_obj.getInfo()
         except ee.ee_exception.EEException as e:
-            logging.info('    Resending query ({}/10)'.format(i))
-            logging.debug('    {}'.format(e))
+            logging.info(f'    Resending query ({i}/{n})')
+            logging.debug(f'    {e}')
             sleep(i ** 2)
             # if ('Earth Engine memory capacity exceeded' in str(e) or
             #         'Earth Engine capacity exceeded' in str(e)):
-            #     logging.info('    Resending query ({}/10)'.format(i))
-            #     logging.debug('    {}'.format(e))
+            #     logging.info(f'    Resending query ({i}/{n})')
+            #     logging.debug(f'    {e}')
             #     sleep(i ** 2)
             # else:
             #     raise e
+        except Exception as e:
+            logging.exception('Unhandled exception on getInfo call')
+            raise e
 
         if output:
             break
 
-    # output = ee_obj.getInfo()
     return output
 
 
 # TODO: Import from common.utils
 # Should these be test fixtures instead?
 # I'm not sure how to make them fixtures and allow input parameters
 def constant_image_value(image, crs='EPSG:32613', scale=1):
```

### Comparing `openet-ssebop-0.2.6/openet_ssebop.egg-info/PKG-INFO` & `openet-ssebop-0.2.8/openet_ssebop.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: openet-ssebop
-Version: 0.2.6
+Version: 0.2.8
 Summary: Earth Engine based SSEBop Model
 Home-page: https://github.com/Open-ET/openet-ssebop
+Download-URL: https://github.com/Open-ET/openet-ssebop/archive/v0.2.8.tar.gz
 Author: Gabe Parrish, Mac Friedrichs, Gabriel Senay
 Author-email: gparrish@contractor.usgs.gov
 License: Apache
-Download-URL: https://github.com/Open-ET/openet-ssebop/archive/v0.2.6.tar.gz
 Keywords: SSEBop OpenET Evapotranspiration Earth Engine
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 ===============
 OpenET - SSEBop
 ===============
 
-|version| |build| |codecov|
+|version| |build|
 
 **WARNING: This code is in development, is being provided without support, and is subject to change at any time without notification**
 
 This repository provides `Google Earth Engine <https://earthengine.google.com/>`__ Python API based implementation of the SSEBop ET model.
 
 The Operational Simplified Surface Energy Balance (SSEBop) model computes daily total actual evapotranspiration (ETa) using land surface temperature (Ts), maximum air temperature (Ta) and reference ET (ETr or ETo).
 The SSEBop model does not solve all the energy balance terms explicitly; rather, it defines the limiting conditions based on "gray-sky" net radiation balance principles and an air temperature parameter.
-This approach predefines unique sets of "hot/dry" and "cold/wet" limiting values for each pixel, allowing an operational model setup and a relatively shorter compute time.
+This approach predefines unique sets of "hot/dry" and "cold/wet" limiting values for each pixel, allowing an operational model setup and a relatively shorter compute time. More information on the GEE implementation of SSEBop is published in Senay2022_ and Senay2023_ with additional details and model assessment.
 
 *Basic SSEBop model implementation in Earth Engine:*
 
 .. image:: docs/SSEBop_GEE_diagram.jpg
 
 Model Design
 ============
@@ -40,37 +39,39 @@
 The primary component of the SSEBop model is the Image() class.  The Image class can be used to compute a single fraction of reference ET (ETf) image from a single input image.  The Image class should generally be instantiated from an Earth Engine Landsat image using the collection specific methods listed below.  ET image collections can be built by computing ET in a function that is mapped over a collection of input images.  Please see the `Example Notebooks`_ for more details.
 
 Input Collections
 =================
 
 SSEBop ET can currently be computed for Landsat Collection 2 Level 2 (SR/ST) images and Landsat Collection 1 Top-Of-Atmosphere (TOA) images from the following Earth Engine image collections:
 
+ * LANDSAT/LC09/C02/T1_L2
  * LANDSAT/LC08/C02/T1_L2
  * LANDSAT/LE07/C02/T1_L2
  * LANDSAT/LT05/C02/T1_L2
  * LANDSAT/LC08/C01/T1_TOA or LANDSAT/LC08/C01/T1_RT_TOA
  * LANDSAT/LE07/C01/T1_TOA or LANDSAT/LE07/C01/T1_RT_TOA
  * LANDSAT/LT05/C01/T1_TOA
 
 
-**Note:** Users are encouraged to prioritize use of Collection 2 data where available. Collection 1 will be produced by USGS until 2022-01-01, and maintained by Earth Engine until 2023-01-01. [`More Information <https://developers.google.com/earth-engine/guides/landsat#landsat-collection-status>`__]
+**Note:** Users are encouraged to prioritize use of Collection 2 data where available. Collection 1 was produced by USGS until 2022-01-01, and maintained by Earth Engine until 2023-01-01. [`More Information <https://developers.google.com/earth-engine/guides/landsat#landsat-collection-status>`__]
 
 Landsat Collection 2 SR/ST Input Image
 --------------------------------------
 
 To instantiate the class for a Landsat Collection 2 SR/ST image, use the Image.from_landsat_c2_sr method.
 
 The input Landsat image must have the following bands and properties:
 
 =================  ======================================
 SPACECRAFT_ID      Band Names
 =================  ======================================
 LANDSAT_5          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B7, ST_B6, QA_PIXEL
 LANDSAT_7          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B7, ST_B6, QA_PIXEL
 LANDSAT_8          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B6, SR_B7, ST_B10, QA_PIXEL
+LANDSAT_9          SR_B1, SR_B2, SR_B3, SR_B4, SR_B5, SR_B6, SR_B7, ST_B10, QA_PIXEL
 =================  ======================================
 
 Landsat Collection 1 TOA Input Image
 ------------------------------------
 
 To instantiate the class for a Landsat Collection 1 TOA image, use the Image.from_landsat_c1_toa() method.
 
@@ -85,15 +86,15 @@
 =================  ======================================
 
 =================  =============================================
 Property           Description
 =================  =============================================
 system:index       - Landsat Scene ID
                    - Must be in the Earth Engine format (e.g. LC08_044033_20170716)
-                   - Used to lookup the scene specific c-factor
+                   - Used to lookup the scene specific c-factor (DEPRECATED)
 system:time_start  Image datetime in milliseconds since 1970
 SPACECRAFT_ID      - Used to determine which Landsat type
                    - Must be: LANDSAT_5, LANDSAT_7, or LANDSAT_8
 =================  =============================================
 
 Model Output
 ------------
@@ -145,56 +146,49 @@
 ==================
 
 Maximum Daily Air Temperature (Tmax)
 ------------------------------------
 The daily maximum air temperature (Tmax) is essential for establishing the maximum ET limit (cold boundary) as explained in Senay2017_.
 Support for source options includes CIMIS, GRIDMET, DAYMET, and other custom Image Collections. See the model Image class docstrings for more information.
 
-Default Asset ID: *projects/usgs-ssebop/tmax/daymet_median_v2* (Daily median from 1980-2018)
+Default Asset ID: *projects/usgs-ssebop/tmax/daymet_v4_mean_1981_2010* (Daily median from 1981-2010)
 
 Land Surface Temperature (LST)
 ------------------------------
 Land Surface Temperature is currently calculated in the SSEBop approach two ways:
 
 * Landsat Collection 2 Level-2 (ST band) images directly. More information can be found at: `USGS Landsat Collection 2 Level-2 Science Products <https://www.usgs.gov/core-science-systems/nli/landsat/landsat-collection-2-level-2-science-products>`__
 
 * Landsat Collection 1 Top-of-Atmosphere images by including an on-the-fly function for calibration steps and atmospheric correction techniques. These include calculations for: (1) spectral radiance conversion to the at-sensor brightness temperature; (2) atmospheric absorption and re-emission value; and (3) surface emissivity. For additional information, users can refer to section 3.2 of the Methodology in Senay2016_.
 
 Temperature Difference (dT)
 ---------------------------
 The SSEBop ET model uses dT as a predefined temperature difference between Thot and Tcold for each pixel.
 In SSEBop formulation, hot and cold limits are defined on the same pixel; therefore, dT actually represents the vertical temperature difference between the surface temperature of a theoretical bare/dry condition of a given pixel and the air temperature at the canopy level of the same pixel as explained in Senay2018_. The input dT is calculated under "gray-sky" conditions and assumed not to change from year to year, but is unique for each day and location.
 
-Default Asset ID: *projects/usgs-ssebop/dt/daymet_median_v2*
-
-Elevation
----------
-The default elevation dataset is the USGS SRTM global image asset.
-
-Default Asset ID: `USGS/SRTMGL1_003 <https://developers.google.com/earth-engine/datasets/catalog/USGS_SRTMGL1_003>`__
-
-The elevation parameter will accept any Earth Engine image.
+Default Asset ID: *projects/usgs-ssebop/dt/daymet_median_v6*
 
 Temperature Correction (*c factor*)
 -----------------------------------
-In order to correspond the maximum air temperature with cold/wet limiting environmental conditions, the SSEBop model uses a temperature correction coefficient (*c factor*, sometimes labeled interchangeably as Tcorr) uniquely calculated for each Landsat scene from well-watered/vegetated pixels.
-This temperature correction component is based on a ratio of Tmax and LST that has passed through several conditions such as NDVI limits. The SSEBop model utilizes the *c factor* as a function of the maximum air temperature, so the data source of the *c factor* collection needs to match the data source of the air temperature. **Note:** *Tcorr* refers to the pixel-based ratio of LST_cold and Tmax while *c factor* is a statistical value that represents a region such as a 5-km grid or scene-wide value.
+In order to correspond the maximum air temperature with cold/wet limiting environmental conditions, the SSEBop model uses a temperature correction coefficient (*c factor*, sometimes labeled interchangeably as Tcorr) uniquely calculated for each Landsat scene.
+This temperature correction component is uniquely developed for SSEBop using a Forcing and Normalizing Operation (FANO) method featuring a linear relation between a normalized land surface temperature difference and NDVI difference using the dT parameter and a proportionality constant.
 
-.. image:: docs/GriddedCfactor_example.png
+ **Note:** *Tcorr* refers to the pixel-based ratio of LST_cold and Tmax while *c factor* is a statistical value that represents a region such as a 5-km grid size (or larger) value.
 
-This parameter can be implemented dynamically as a scene-based single *c factor* (this is the default) or using precomputed spatially varying Image Assets where a gridded *c factor* is generated for every 5-km (advanced setting).
+More information on parameter design and model improvements using the FANO method can be found in Senay2023_. Additional SSEBop model algorithm theoretical basis documentation can be found `here <https://www.usgs.gov/media/files/landsat-4-9-collection-2-level-3-provisional-actual-evapotranspiration-algorithm>`__.
 
-* Using either DYNAMIC or SCENE_GRIDDED settings, the *c factor* parameter is read from precomputed Earth Engine image collections based on the Landsat scene ID (from the system:index property). Monthly/annual climatology values are used if Tcorr cannot be determined for a given Landsat scene. If fallback values have not been computed for the target path/row, a default value of 0.978 will be used.
-* Currently, SCENE_GRIDDED is only supported for Landsat Collection 2 across CONUS (since model version 0.1.5x) and requires a matching Tmax source. See `this example notebook <examples/tcorr_gridded.ipynb>`__ for more information.
+The 'FANO' parameter (default) can be implemented dynamically for each Landsat scene within the SSEBop Image object using the following Tcorr source:
 
-Default Asset IDs
+.. code-block:: python
 
-Scene ID: projects/usgs-ssebop/tcorr_scene/daymet_median_v2_scene
+    model_obj = model.Image.from_landsat_c2_sr(
+        tcorr_source='FANO',
+        )
 
-Monthly ID: projects/usgs-ssebop/tcorr_scene/daymet_median_v2_monthly
+The FANO parameterization allows the establishment of the cold boundary condition regardless of vegetation cover density, improving the performance and operational implementation of the SSEBop ET model in sparsely vegetated landscapes, dynamic growing seasons, and varying locations around the world.
 
 Installation
 ============
 
 The OpenET SSEBop python module can be installed via pip:
 
 .. code-block:: console
@@ -238,21 +232,22 @@
 .. [Senay2018]
  | Senay, G. (2018). Satellite Psychrometric Formulation of the Operational Simplified Surface Energy Balance (SSEBop) Model for Quantifying and Mapping Evapotranspiration. *Applied Engineering in Agriculture*, 34(3).
  | `https://doi.org/10.13031/aea.12614 <https://doi.org/10.13031/aea.12614>`__
 .. [Senay2019]
  | Senay, G., Schauer, M., Velpuri, N.M., Singh, R.K., Kagone, S., Friedrichs, M., Litvak, M.E., Douglas-Mankin, K.R. (2019). Long-Term (1986–2015) Crop Water Use Characterization over the Upper Rio Grande Basin of United States and Mexico Using Landsat-Based Evapotranspiration. *Remote Sensing*, 11(13):1587.
  | `https://doi.org/10.3390/rs11131587 <https://doi.org/10.3390/rs11131587>`__
 .. [Schauer2019]
- | Schauer, M.,Senay, G. (2019). Characterizing Crop Water Use Dynamics in the Central Valley of California Using Landsat-Derived Evapotranspiration. *Remote Sensing*, 11(15):1782.
+ | Schauer, M., Senay, G. (2019). Characterizing Crop Water Use Dynamics in the Central Valley of California Using Landsat-Derived Evapotranspiration. *Remote Sensing*, 11(15):1782.
  | `https://doi.org/10.3390/rs11151782 <https://doi.org/10.3390/rs11151782>`__
+.. [Senay2022]
+ | Senay, G.B., Friedrichs, M., Morton, C., Parrish, G. E., Schauer, M., Khand, K., ... & Huntington, J. (2022). Mapping actual evapotranspiration using Landsat for the conterminous United States: Google Earth Engine implementation and assessment of the SSEBop model. *Remote Sensing of Environment*, 275, 113011
+ | `https://doi.org/10.1016/j.rse.2022.113011 <https://doi.org/10.1016/j.rse.2022.113011>`__
+.. [Senay2023]
+ | Senay, G.B., Parrish, G. E., Schauer, M., Friedrichs, M., Khand, K., Boiko, O., Kagone, S., Dittmeier, R., Arab, S., Ji, L. (2023). Improving the Operational Simplified Surface Energy Balance evapotranspiration model using the Forcing and Normalizing Operation. *Remote Sensing*, 15(1):260.
+ | `https://doi.org/10.3390/rs15010260 <https://doi.org/10.3390/rs15010260>`__
 
 .. |build| image:: https://github.com/Open-ET/openet-ssebop/workflows/build/badge.svg
    :alt: Build status
    :target: https://github.com/Open-ET/openet-ssebop
 .. |version| image:: https://badge.fury.io/py/openet-ssebop.svg
    :alt: Latest version on PyPI
    :target: https://badge.fury.io/py/openet-ssebop
-.. |codecov| image:: https://codecov.io/gh/Open-ET/openet-ssebop/branch/main/graphs/badge.svg
-   :alt: Coverage Status
-   :target: https://codecov.io/gh/Open-ET/openet-ssebop
-
-
```

### Comparing `openet-ssebop-0.2.6/openet_ssebop.egg-info/SOURCES.txt` & `openet-ssebop-0.2.8/openet_ssebop.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-openet/.DS_Store
 openet/__init__.py
 openet/ssebop/__init__.py
 openet/ssebop/collection.py
 openet/ssebop/image.py
 openet/ssebop/interpolate.py
 openet/ssebop/ipytest.py
 openet/ssebop/landsat.py
```

### Comparing `openet-ssebop-0.2.6/setup.py` & `openet-ssebop-0.2.8/setup.py`

 * *Files identical despite different names*

