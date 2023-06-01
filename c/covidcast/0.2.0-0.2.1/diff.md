# Comparing `tmp/covidcast-0.2.0.tar.gz` & `tmp/covidcast-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covidcast-0.2.0.tar", last modified: Tue May 23 16:52:19 2023, max compression
+gzip compressed data, was "covidcast-0.2.1.tar", last modified: Thu Jun  1 18:29:10 2023, max compression
```

## Comparing `covidcast-0.2.0.tar` & `covidcast-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.300094 covidcast-0.2.0/
--rw-r--r--   0 krivard  (12134) users      (100)     1277 2023-05-23 16:52:19.300094 covidcast-0.2.0/PKG-INFO
--rw-r--r--   0 krivard  (12134) users      (100)      680 2020-12-16 14:58:59.000000 covidcast-0.2.0/README.md
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.288094 covidcast-0.2.0/covidcast/
--rw-r--r--   0 krivard  (12134) users      (100)      739 2023-05-22 19:15:07.000000 covidcast-0.2.0/covidcast/__init__.py
--rw-r--r--   0 krivard  (12134) users      (100)    24797 2023-05-22 19:15:07.000000 covidcast-0.2.0/covidcast/covidcast.py
--rw-r--r--   0 krivard  (12134) users      (100)      182 2020-12-16 14:58:59.000000 covidcast-0.2.0/covidcast/errors.py
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.292094 covidcast-0.2.0/covidcast/geo_mappings/
--rw-r--r--   0 krivard  (12134) users      (100)  3674419 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/geo_mappings/county_census.csv
--rw-r--r--   0 krivard  (12134) users      (100)  1299191 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/geo_mappings/msa_census.csv
--rw-r--r--   0 krivard  (12134) users      (100)     2854 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/geo_mappings/state_census.csv
--rw-r--r--   0 krivard  (12134) users      (100)    17755 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/geography.py
--rw-r--r--   0 krivard  (12134) users      (100)     3426 2023-03-27 18:00:04.000000 covidcast-0.2.0/covidcast/make_reference_plots.py
--rw-r--r--   0 krivard  (12134) users      (100)    26627 2023-03-29 14:35:17.000000 covidcast-0.2.0/covidcast/plotting.py
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.288094 covidcast-0.2.0/covidcast/shapefiles/
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.296094 covidcast-0.2.0/covidcast/shapefiles/county/
--rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.cpg
--rw-r--r--   0 krivard  (12134) users      (100)   527301 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.dbf
--rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.prj
--rw-r--r--   0 krivard  (12134) users      (100)  3662752 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp
--rwxr-xr-x   0 krivard  (12134) users      (100)    21754 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.ea.iso.xml
--rwxr-xr-x   0 krivard  (12134) users      (100)    34190 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.iso.xml
--rw-r--r--   0 krivard  (12134) users      (100)    25964 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shx
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.296094 covidcast-0.2.0/covidcast/shapefiles/hrr/
--rw-r--r--   0 krivard  (12134) users      (100)   236891 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.dbf
--rw-r--r--   0 krivard  (12134) users      (100)      212 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.prj
--rw-r--r--   0 krivard  (12134) users      (100)  1734200 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shp
--rw-r--r--   0 krivard  (12134) users      (100)     2548 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shx
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.300094 covidcast-0.2.0/covidcast/shapefiles/msa/
--rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.cpg
--rw-r--r--   0 krivard  (12134) users      (100)   148494 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.dbf
--rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.prj
--rw-r--r--   0 krivard  (12134) users      (100)  1494264 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp
--rwxr-xr-x   0 krivard  (12134) users      (100)    16594 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.ea.iso.xml
--rwxr-xr-x   0 krivard  (12134) users      (100)    32493 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.iso.xml
--rw-r--r--   0 krivard  (12134) users      (100)     7604 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shx
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.300094 covidcast-0.2.0/covidcast/shapefiles/state/
--rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.cpg
--rw-r--r--   0 krivard  (12134) users      (100)     9058 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.dbf
--rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.prj
--rw-r--r--   0 krivard  (12134) users      (100)  1394376 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp
--rwxr-xr-x   0 krivard  (12134) users      (100)    17903 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.ea.iso.xml
--rwxr-xr-x   0 krivard  (12134) users      (100)    31536 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.iso.xml
--rw-r--r--   0 krivard  (12134) users      (100)      548 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shx
-drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.288094 covidcast-0.2.0/covidcast.egg-info/
--rw-r--r--   0 krivard  (12134) users      (100)     1277 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/PKG-INFO
--rw-r--r--   0 krivard  (12134) users      (100)     1874 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/SOURCES.txt
--rw-r--r--   0 krivard  (12134) users      (100)        1 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/dependency_links.txt
--rw-r--r--   0 krivard  (12134) users      (100)      115 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/requires.txt
--rw-r--r--   0 krivard  (12134) users      (100)       10 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/top_level.txt
--rw-r--r--   0 krivard  (12134) users      (100)       38 2023-05-23 16:52:19.300094 covidcast-0.2.0/setup.cfg
--rw-r--r--   0 krivard  (12134) users      (100)     1056 2023-05-22 19:17:23.000000 covidcast-0.2.0/setup.py
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.371330 covidcast-0.2.1/
+-rw-r--r--   0 krivard  (12134) users      (100)     1277 2023-06-01 18:29:10.371330 covidcast-0.2.1/PKG-INFO
+-rw-r--r--   0 krivard  (12134) users      (100)      680 2020-12-16 14:58:59.000000 covidcast-0.2.1/README.md
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.359330 covidcast-0.2.1/covidcast/
+-rw-r--r--   0 krivard  (12134) users      (100)      739 2023-05-22 19:15:07.000000 covidcast-0.2.1/covidcast/__init__.py
+-rw-r--r--   0 krivard  (12134) users      (100)    24833 2023-06-01 14:47:34.000000 covidcast-0.2.1/covidcast/covidcast.py
+-rw-r--r--   0 krivard  (12134) users      (100)      182 2020-12-16 14:58:59.000000 covidcast-0.2.1/covidcast/errors.py
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.363330 covidcast-0.2.1/covidcast/geo_mappings/
+-rw-r--r--   0 krivard  (12134) users      (100)  3674419 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/geo_mappings/county_census.csv
+-rw-r--r--   0 krivard  (12134) users      (100)  1299191 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/geo_mappings/msa_census.csv
+-rw-r--r--   0 krivard  (12134) users      (100)     2854 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/geo_mappings/state_census.csv
+-rw-r--r--   0 krivard  (12134) users      (100)    17755 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/geography.py
+-rw-r--r--   0 krivard  (12134) users      (100)     3426 2023-03-27 18:00:04.000000 covidcast-0.2.1/covidcast/make_reference_plots.py
+-rw-r--r--   0 krivard  (12134) users      (100)    26627 2023-03-29 14:35:17.000000 covidcast-0.2.1/covidcast/plotting.py
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.359330 covidcast-0.2.1/covidcast/shapefiles/
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.367330 covidcast-0.2.1/covidcast/shapefiles/county/
+-rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.cpg
+-rw-r--r--   0 krivard  (12134) users      (100)   527301 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.dbf
+-rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.prj
+-rw-r--r--   0 krivard  (12134) users      (100)  3662752 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.shp
+-rwxr-xr-x   0 krivard  (12134) users      (100)    21754 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.ea.iso.xml
+-rwxr-xr-x   0 krivard  (12134) users      (100)    34190 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.iso.xml
+-rw-r--r--   0 krivard  (12134) users      (100)    25964 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.shx
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.367330 covidcast-0.2.1/covidcast/shapefiles/hrr/
+-rw-r--r--   0 krivard  (12134) users      (100)   236891 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.dbf
+-rw-r--r--   0 krivard  (12134) users      (100)      212 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.prj
+-rw-r--r--   0 krivard  (12134) users      (100)  1734200 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shp
+-rw-r--r--   0 krivard  (12134) users      (100)     2548 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shx
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.371330 covidcast-0.2.1/covidcast/shapefiles/msa/
+-rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.cpg
+-rw-r--r--   0 krivard  (12134) users      (100)   148494 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.dbf
+-rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.prj
+-rw-r--r--   0 krivard  (12134) users      (100)  1494264 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp
+-rwxr-xr-x   0 krivard  (12134) users      (100)    16594 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.ea.iso.xml
+-rwxr-xr-x   0 krivard  (12134) users      (100)    32493 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.iso.xml
+-rw-r--r--   0 krivard  (12134) users      (100)     7604 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shx
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.371330 covidcast-0.2.1/covidcast/shapefiles/state/
+-rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.cpg
+-rw-r--r--   0 krivard  (12134) users      (100)     9058 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.dbf
+-rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.prj
+-rw-r--r--   0 krivard  (12134) users      (100)  1394376 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.shp
+-rwxr-xr-x   0 krivard  (12134) users      (100)    17903 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.ea.iso.xml
+-rwxr-xr-x   0 krivard  (12134) users      (100)    31536 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.iso.xml
+-rw-r--r--   0 krivard  (12134) users      (100)      548 2020-12-16 14:59:00.000000 covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.shx
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-06-01 18:29:10.359330 covidcast-0.2.1/covidcast.egg-info/
+-rw-r--r--   0 krivard  (12134) users      (100)     1277 2023-06-01 18:29:10.000000 covidcast-0.2.1/covidcast.egg-info/PKG-INFO
+-rw-r--r--   0 krivard  (12134) users      (100)     1874 2023-06-01 18:29:10.000000 covidcast-0.2.1/covidcast.egg-info/SOURCES.txt
+-rw-r--r--   0 krivard  (12134) users      (100)        1 2023-06-01 18:29:10.000000 covidcast-0.2.1/covidcast.egg-info/dependency_links.txt
+-rw-r--r--   0 krivard  (12134) users      (100)      114 2023-06-01 18:29:10.000000 covidcast-0.2.1/covidcast.egg-info/requires.txt
+-rw-r--r--   0 krivard  (12134) users      (100)       10 2023-06-01 18:29:10.000000 covidcast-0.2.1/covidcast.egg-info/top_level.txt
+-rw-r--r--   0 krivard  (12134) users      (100)       38 2023-06-01 18:29:10.371330 covidcast-0.2.1/setup.cfg
+-rw-r--r--   0 krivard  (12134) users      (100)     1055 2023-06-01 14:44:57.000000 covidcast-0.2.1/setup.py
```

### Comparing `covidcast-0.2.0/PKG-INFO` & `covidcast-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covidcast
-Version: 0.2.0
+Version: 0.2.1
 Summary: Access COVID-19 data through the Delphi COVIDcast API
 Home-page: https://cmu-delphi.github.io/covidcast/covidcast-py/html/
 Author: Alex Reinhart
 Author-email: areinhar@stat.cmu.edu
 License: UNKNOWN
 Description: # COVIDcast API client
```

### Comparing `covidcast-0.2.0/README.md` & `covidcast-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/__init__.py` & `covidcast-0.2.1/covidcast/__init__.py`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/covidcast.py` & `covidcast-0.2.1/covidcast/covidcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     :param key: String containing the API key for you and/or your group.
 
     Anyone may access the Epidata API anonymously without providing an API key.
     Anonymous API access is currently rate-limited and with a maximum of two of
     the requested parameters having multiple selections (signals, dates, issues,
     regions, etc). To be exempt from these limits, use this function to apply an
     API key to all subsequent queries. You can register for an API key at
-    <https://forms.gle/hkBr5SfQgxguAfEt7>.
+    <https://api.delphi.cmu.edu/epidata/admin/registration_form>.
 
     Consult the `API documentation
     <https://cmu-delphi.github.io/delphi-epidata/api/api_keys.html>`_
     for details on our API key policies.
     """
-    Epidata.auth = key
+    Epidata.auth = ("epidata", key)
 
 def signal(data_source: str,
            signal: str,  # pylint: disable=W0621
            start_day: date = None,
            end_day: date = None,
            geo_type: str = "county",
            geo_values: Union[str, Iterable[str]] = "*",
```

### Comparing `covidcast-0.2.0/covidcast/geo_mappings/county_census.csv` & `covidcast-0.2.1/covidcast/geo_mappings/county_census.csv`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/geo_mappings/msa_census.csv` & `covidcast-0.2.1/covidcast/geo_mappings/msa_census.csv`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/geo_mappings/state_census.csv` & `covidcast-0.2.1/covidcast/geo_mappings/state_census.csv`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/geography.py` & `covidcast-0.2.1/covidcast/geography.py`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/make_reference_plots.py` & `covidcast-0.2.1/covidcast/make_reference_plots.py`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/plotting.py` & `covidcast-0.2.1/covidcast/plotting.py`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.dbf` & `covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.dbf`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp` & `covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.shp`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.ea.iso.xml` & `covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.ea.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.iso.xml` & `covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shx` & `covidcast-0.2.1/covidcast/shapefiles/county/cb_2019_us_county_5m.shx`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.dbf` & `covidcast-0.2.1/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.dbf`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shp` & `covidcast-0.2.1/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shp`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shx` & `covidcast-0.2.1/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shx`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.dbf` & `covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.dbf`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp` & `covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.ea.iso.xml` & `covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.ea.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.iso.xml` & `covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shx` & `covidcast-0.2.1/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shx`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.dbf` & `covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.dbf`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp` & `covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.shp`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.ea.iso.xml` & `covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.ea.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.iso.xml` & `covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shx` & `covidcast-0.2.1/covidcast/shapefiles/state/cb_2019_us_state_5m.shx`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/covidcast.egg-info/PKG-INFO` & `covidcast-0.2.1/covidcast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covidcast
-Version: 0.2.0
+Version: 0.2.1
 Summary: Access COVID-19 data through the Delphi COVIDcast API
 Home-page: https://cmu-delphi.github.io/covidcast/covidcast-py/html/
 Author: Alex Reinhart
 Author-email: areinhar@stat.cmu.edu
 License: UNKNOWN
 Description: # COVIDcast API client
```

### Comparing `covidcast-0.2.0/covidcast.egg-info/SOURCES.txt` & `covidcast-0.2.1/covidcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covidcast-0.2.0/setup.py` & `covidcast-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covidcast",
-    version="0.2.0",  # also update in docs/conf.py
+    version="0.2.1",  # also update in docs/conf.py
     author="Alex Reinhart",
     author_email="areinhar@stat.cmu.edu",
     description="Access COVID-19 data through the Delphi COVIDcast API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://cmu-delphi.github.io/covidcast/covidcast-py/html/",
     packages=setuptools.find_packages(),
@@ -18,15 +18,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
         "pandas<2",
         "requests",
-        "delphi-epidata>=0.0.11",
+        "delphi-epidata>=4.1.1",
         "geopandas",
         "matplotlib",
         "numpy",
         "descartes",
         "imageio-ffmpeg",
         "imageio",
         "tqdm",
```

