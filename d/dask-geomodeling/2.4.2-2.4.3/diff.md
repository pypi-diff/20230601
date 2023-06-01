# Comparing `tmp/dask-geomodeling-2.4.2.tar.gz` & `tmp/dask-geomodeling-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-geomodeling-2.4.2.tar", last modified: Wed May 31 11:50:01 2023, max compression
+gzip compressed data, was "dask-geomodeling-2.4.3.tar", last modified: Thu Jun  1 10:07:35 2023, max compression
```

## Comparing `dask-geomodeling-2.4.2.tar` & `dask-geomodeling-2.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.532863 dask-geomodeling-2.4.2/
--rw-rw-r--   0 casper    (1000) casper    (1000)    19228 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/CHANGES.rst
--rw-rw-r--   0 casper    (1000) casper    (1000)     1503 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/LICENSE
--rw-rw-r--   0 casper    (1000) casper    (1000)       59 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/MANIFEST.in
--rw-rw-r--   0 casper    (1000) casper    (1000)    21098 2023-05-31 11:50:01.532863 dask-geomodeling-2.4.2/PKG-INFO
--rw-rw-r--   0 casper    (1000) casper    (1000)     1240 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/README.rst
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.528863 dask-geomodeling-2.4.2/dask_geomodeling/
--rw-rw-r--   0 casper    (1000) casper    (1000)      228 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)      318 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/config.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.528863 dask-geomodeling-2.4.2/dask_geomodeling/core/
--rw-rw-r--   0 casper    (1000) casper    (1000)       30 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/core/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    11147 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/core/graphs.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.528863 dask-geomodeling-2.4.2/dask_geomodeling/geometry/
--rw-rw-r--   0 casper    (1000) casper    (1000)      337 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    23024 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/aggregate.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    10953 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/base.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/constructive.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    24495 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/field_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     1492 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/geom_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     5351 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/merge.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     3458 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/parallelize.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4978 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/set_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    10587 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/sinks.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     9096 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/sources.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4138 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/text.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4987 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/ipyleaflet_plugin.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4796 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/measurements.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.532863 dask-geomodeling-2.4.2/dask_geomodeling/raster/
--rw-rw-r--   0 casper    (1000) casper    (1000)      291 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/base.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    16996 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/combine.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    25032 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/elemwise.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    26079 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/misc.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4450 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/parallelize.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     8124 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/reduction.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    17971 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/sources.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    26435 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/spatial.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    33321 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/temporal.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    31545 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/utils.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.528863 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/
--rw-rw-r--   0 casper    (1000) casper    (1000)    21098 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/PKG-INFO
--rw-rw-r--   0 casper    (1000) casper    (1000)     1341 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/SOURCES.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/dependency_links.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/not-zip-safe
--rw-rw-r--   0 casper    (1000) casper    (1000)      112 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/requires.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)       17 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/top_level.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)      324 2023-05-31 11:50:01.532863 dask-geomodeling-2.4.2/setup.cfg
--rw-rw-r--   0 casper    (1000) casper    (1000)     1670 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/setup.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-06-01 10:07:35.766711 dask-geomodeling-2.4.3/
+-rw-rw-r--   0 casper    (1000) casper    (1000)    19358 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/CHANGES.rst
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1503 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/LICENSE
+-rw-rw-r--   0 casper    (1000) casper    (1000)       59 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/MANIFEST.in
+-rw-rw-r--   0 casper    (1000) casper    (1000)    21228 2023-06-01 10:07:35.766711 dask-geomodeling-2.4.3/PKG-INFO
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1240 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/README.rst
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-06-01 10:07:35.762711 dask-geomodeling-2.4.3/dask_geomodeling/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      228 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)      318 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/config.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-06-01 10:07:35.762711 dask-geomodeling-2.4.3/dask_geomodeling/core/
+-rw-rw-r--   0 casper    (1000) casper    (1000)       30 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/core/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    11147 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/core/graphs.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-06-01 10:07:35.762711 dask-geomodeling-2.4.3/dask_geomodeling/geometry/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      337 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    23024 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/aggregate.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    10953 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/base.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/constructive.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    24495 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/field_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1492 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/geom_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     5351 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/merge.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     3458 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/parallelize.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4978 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/set_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    10587 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/sinks.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     9096 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/sources.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4138 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/geometry/text.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4987 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/ipyleaflet_plugin.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4796 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/measurements.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-06-01 10:07:35.766711 dask-geomodeling-2.4.3/dask_geomodeling/raster/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      291 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/base.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    16996 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/combine.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    25032 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/elemwise.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    26079 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/misc.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4450 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/parallelize.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     8124 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/reduction.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    17971 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/sources.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    26435 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/spatial.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    33452 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/raster/temporal.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    31545 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling/utils.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-06-01 10:07:35.762711 dask-geomodeling-2.4.3/dask_geomodeling.egg-info/
+-rw-rw-r--   0 casper    (1000) casper    (1000)    21228 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling.egg-info/PKG-INFO
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1341 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling.egg-info/SOURCES.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling.egg-info/dependency_links.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling.egg-info/not-zip-safe
+-rw-rw-r--   0 casper    (1000) casper    (1000)      112 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling.egg-info/requires.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)       17 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/dask_geomodeling.egg-info/top_level.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)      324 2023-06-01 10:07:35.766711 dask-geomodeling-2.4.3/setup.cfg
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1670 2023-06-01 10:07:35.000000 dask-geomodeling-2.4.3/setup.py
```

### Comparing `dask-geomodeling-2.4.2/CHANGES.rst` & `dask-geomodeling-2.4.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.3 (2023-06-01)
+------------------
+
+- Fixed an edge case in TemporalAggregate / Cumulative for month start ("MS") frequency.
+
+
 2.4.2 (2023-05-31)
 ------------------
 
 - Fixed TemporalAggregate and Cumulative for month start ("MS") frequency.
 
 
 2.4.1 (2023-04-18)
```

### Comparing `dask-geomodeling-2.4.2/LICENSE` & `dask-geomodeling-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/PKG-INFO` & `dask-geomodeling-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-geomodeling
-Version: 2.4.2
+Version: 2.4.3
 Summary: On-the-fly operations on geographical maps.
 Home-page: https://github.com/nens/dask-geomodeling
 Author: Casper van der Wel
 Author-email: casper.vanderwel@nelen-schuurmans.nl
 License: BSD 3-Clause License
 Keywords: dask
 Classifier: Development Status :: 4 - Beta
@@ -43,14 +43,20 @@
 
 `Read the docs <https://dask-geomodeling.readthedocs.org/>`_ for further information.
 
 
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.3 (2023-06-01)
+------------------
+
+- Fixed an edge case in TemporalAggregate / Cumulative for month start ("MS") frequency.
+
+
 2.4.2 (2023-05-31)
 ------------------
 
 - Fixed TemporalAggregate and Cumulative for month start ("MS") frequency.
 
 
 2.4.1 (2023-04-18)
```

### Comparing `dask-geomodeling-2.4.2/README.rst` & `dask-geomodeling-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/core/graphs.py` & `dask-geomodeling-2.4.3/dask_geomodeling/core/graphs.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/aggregate.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/aggregate.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/base.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/base.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/constructive.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/constructive.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/field_operations.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/field_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/geom_operations.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/geom_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/merge.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/merge.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/parallelize.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/parallelize.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/set_operations.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/set_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/sinks.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/sinks.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/sources.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/sources.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/geometry/text.py` & `dask-geomodeling-2.4.3/dask_geomodeling/geometry/text.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/ipyleaflet_plugin.py` & `dask-geomodeling-2.4.3/dask_geomodeling/ipyleaflet_plugin.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/measurements.py` & `dask-geomodeling-2.4.3/dask_geomodeling/measurements.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/base.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/base.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/combine.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/combine.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/elemwise.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/elemwise.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/misc.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/misc.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/parallelize.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/parallelize.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/reduction.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/reduction.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/sources.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/sources.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/spatial.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/spatial.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/raster/temporal.py` & `dask-geomodeling-2.4.3/dask_geomodeling/raster/temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,19 +259,22 @@
 
 
 def _get_bin_label(dt, frequency, closed, label, timezone):
     """Returns the label of the bin the input dt belongs to.
 
     :type dt: datetime.datetime without timezone.
     """
-    # go through resample, this is the only function that supports 'closed'
+    # the strategy is leveraging pandas.Series.resample to put the dt in a bin
+    # while there is only 1 sample here, there might be multiple (empty) bins
+    # in some cases (see test_issue_5917)
     series = pd.Series([0], index=[_dt_to_ts(dt, timezone)])
-    resampled = series.resample(frequency, closed=closed, label=label, kind="timestamp")
-    snapped = resampled.first().index[0]
-    return _ts_to_dt(snapped, timezone)
+    for label, bin in series.resample(frequency, closed=closed, label=label, kind="timestamp"):
+        if len(bin) != 0:
+            break
+    return _ts_to_dt(label, timezone)
 
 
 def _get_bin_period(dt, frequency, closed, label, timezone):
     """Returns the label of the bin the input dt belongs to.
 
     :type dt: datetime.datetime without timezone.
     """
```

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling/utils.py` & `dask-geomodeling-2.4.3/dask_geomodeling/utils.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling.egg-info/PKG-INFO` & `dask-geomodeling-2.4.3/dask_geomodeling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-geomodeling
-Version: 2.4.2
+Version: 2.4.3
 Summary: On-the-fly operations on geographical maps.
 Home-page: https://github.com/nens/dask-geomodeling
 Author: Casper van der Wel
 Author-email: casper.vanderwel@nelen-schuurmans.nl
 License: BSD 3-Clause License
 Keywords: dask
 Classifier: Development Status :: 4 - Beta
@@ -43,14 +43,20 @@
 
 `Read the docs <https://dask-geomodeling.readthedocs.org/>`_ for further information.
 
 
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.3 (2023-06-01)
+------------------
+
+- Fixed an edge case in TemporalAggregate / Cumulative for month start ("MS") frequency.
+
+
 2.4.2 (2023-05-31)
 ------------------
 
 - Fixed TemporalAggregate and Cumulative for month start ("MS") frequency.
 
 
 2.4.1 (2023-04-18)
```

### Comparing `dask-geomodeling-2.4.2/dask_geomodeling.egg-info/SOURCES.txt` & `dask-geomodeling-2.4.3/dask_geomodeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.2/setup.py` & `dask-geomodeling-2.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = '2.4.2'
+version = '2.4.3'
 
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read()])
 
 install_requires = (
     [
         "dask[delayed]>=0.20",
         "pandas>=0.23",
```

