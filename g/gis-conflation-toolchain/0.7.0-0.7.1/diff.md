# Comparing `tmp/gis-conflation-toolchain-0.7.0.tar.gz` & `tmp/gis-conflation-toolchain-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gis-conflation-toolchain-0.7.0.tar", last modified: Fri Apr 28 11:18:53 2023, max compression
+gzip compressed data, was "gis-conflation-toolchain-0.7.1.tar", last modified: Thu Jun  1 03:56:34 2023, max compression
```

## Comparing `gis-conflation-toolchain-0.7.0.tar` & `gis-conflation-toolchain-0.7.1.tar`

### file list

```diff
@@ -1,28 +1,41 @@
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1211 2023-04-25 04:34:54.000000 gis-conflation-toolchain-0.7.0/LICENSE
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2682 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/PKG-INFO
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2047 2023-04-28 11:18:17.000000 gis-conflation-toolchain-0.7.0/README.md
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      104 2023-04-25 05:51:41.000000 gis-conflation-toolchain-0.7.0/pyproject.toml
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1044 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/setup.cfg
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/src/
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/src/csv2excel/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 07:23:36.000000 gis-conflation-toolchain-0.7.0/src/csv2excel/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     5490 2023-04-26 12:06:05.000000 gis-conflation-toolchain-0.7.0/src/csv2excel/csv2excel.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/src/csv2geojson/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 07:17:51.000000 gis-conflation-toolchain-0.7.0/src/csv2geojson/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    23044 2023-04-25 08:57:32.000000 gis-conflation-toolchain-0.7.0/src/csv2geojson/csv2geojson.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/src/geojsondiff/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      168 2023-04-25 05:57:16.000000 gis-conflation-toolchain-0.7.0/src/geojsondiff/__init__.py
--rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    40955 2023-04-27 17:25:44.000000 gis-conflation-toolchain-0.7.0/src/geojsondiff/geojsondiff.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/src/gis_conflation_toolchain.egg-info/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2682 2023-04-28 11:18:53.000000 gis-conflation-toolchain-0.7.0/src/gis_conflation_toolchain.egg-info/PKG-INFO
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      596 2023-04-28 11:18:53.000000 gis-conflation-toolchain-0.7.0/src/gis_conflation_toolchain.egg-info/SOURCES.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        1 2023-04-28 11:18:53.000000 gis-conflation-toolchain-0.7.0/src/gis_conflation_toolchain.egg-info/dependency_links.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      278 2023-04-28 11:18:53.000000 gis-conflation-toolchain-0.7.0/src/gis_conflation_toolchain.egg-info/entry_points.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       48 2023-04-28 11:18:53.000000 gis-conflation-toolchain-0.7.0/src/gis_conflation_toolchain.egg-info/top_level.txt
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/src/gisconflation/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 09:07:58.000000 gis-conflation-toolchain-0.7.0/src/gisconflation/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2511 2023-04-28 09:55:54.000000 gis-conflation-toolchain-0.7.0/src/gisconflation/osmf2geojson.py
--rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)     5508 2023-04-28 09:46:28.000000 gis-conflation-toolchain-0.7.0/src/gisconflation/overpassql2osmf.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-04-28 11:18:53.510393 gis-conflation-toolchain-0.7.0/tests/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      580 2023-04-25 08:13:46.000000 gis-conflation-toolchain-0.7.0/tests/test_main.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    34522 2023-05-06 01:44:35.000000 gis-conflation-toolchain-0.7.1/LICENSE
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     3173 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/PKG-INFO
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2486 2023-06-01 03:52:52.000000 gis-conflation-toolchain-0.7.1/README.md
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      104 2023-05-06 19:31:41.000000 gis-conflation-toolchain-0.7.1/pyproject.toml
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1739 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/setup.cfg
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.951835 gis-conflation-toolchain-0.7.1/src/
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.951835 gis-conflation-toolchain-0.7.1/src/csv2excel/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 07:23:36.000000 gis-conflation-toolchain-0.7.1/src/csv2excel/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     5490 2023-04-26 12:06:05.000000 gis-conflation-toolchain-0.7.1/src/csv2excel/csv2excel.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.951835 gis-conflation-toolchain-0.7.1/src/csv2geojson/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 07:17:51.000000 gis-conflation-toolchain-0.7.1/src/csv2geojson/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    26048 2023-05-09 03:45:20.000000 gis-conflation-toolchain-0.7.1/src/csv2geojson/csv2geojson.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.951835 gis-conflation-toolchain-0.7.1/src/geojsondiff/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      168 2023-04-25 05:57:16.000000 gis-conflation-toolchain-0.7.1/src/geojsondiff/__init__.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    44861 2023-05-07 23:02:01.000000 gis-conflation-toolchain-0.7.1/src/geojsondiff/geojsondiff.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     3173 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/PKG-INFO
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1016 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        1 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      828 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/entry_points.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       56 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/requires.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       48 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/top_level.txt
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/src/gisconflation/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 09:07:58.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    24308 2023-05-06 22:34:03.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/csv2gecodedcsv.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    14609 2023-05-09 05:18:51.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/csvedit.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10344 2023-05-08 21:49:46.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/dictionarybuilder.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     5727 2023-05-08 21:50:20.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/dictionarymerger.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)     7111 2023-06-01 03:54:51.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonconcat.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    10629 2023-05-07 01:45:11.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonedit.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    14364 2023-06-01 02:16:30.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonmerger.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     6639 2023-05-07 00:35:41.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/json2csv.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/src/gisconflation/lib/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-29 17:52:00.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/lib/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      503 2023-04-29 18:03:53.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/lib/language.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2511 2023-04-28 09:55:54.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/osmf2geojson.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)     5820 2023-05-08 01:21:04.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/overpassql2osmf.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     8661 2023-05-06 22:48:52.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/util.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/tests/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      580 2023-04-25 08:13:46.000000 gis-conflation-toolchain-0.7.1/tests/test_main.py
```

### Comparing `gis-conflation-toolchain-0.7.0/PKG-INFO` & `gis-conflation-toolchain-0.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,88 @@
 Metadata-Version: 2.1
 Name: gis-conflation-toolchain
-Version: 0.7.0
+Version: 0.7.1
 Summary: gis-conflation-toolchain
 Home-page: https://github.com/fititnt/spatial-data-conflation-open-toolchain
 Author: Emerson Rocha
 Author-email: rocha@ieee.org
 Project-URL: Bug Tracker, https://github.com/fititnt/spatial-data-conflation-open-toolchain/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: extras
 License-File: LICENSE
 
 # spatial-data-conflation-open-toolchain
 **[EARLY DRAFT] Open, free to use, toolchain for geospatial data conflation. Command-line interface for file manipulation.** _See geojson-diff.py from <https://github.com/fititnt/openstreetmap-vs-dados-abertos-brasil>._
 
 [![GitHub](https://img.shields.io/badge/GitHub-fititnt%20spatial--data--conflation--open--toolchain-lightgrey?logo=github&style=social[fititnt/geojson-diff] "GitHub")](https://github.com/fititnt/spatial-data-conflation-open-toolchain)
 
 [![Pypi: gis-conflation-toolchain](https://img.shields.io/badge/python%20pypi-gis--conflation--toolchain-brightgreen[Python] 
  "Pypi: gis-conflation-toolchain")](https://pypi.org/project/gis-conflation-toolchain)
 
 
 ## Installing
 
 ```bash
-# @TODO release this as pip package
-pip install --upgrade git+https://github.com/fititnt/spatial-data-conflation-open-toolchain.git#egg=gis-conflation-toolchain
+pip install --upgrade gis-conflation-toolchain
 ```
 
 <!--
 -  Saalfield, Alan. Conflation: Automated Map Compilation. BUREAU OF THE CENSUS STATISTICAL RESEARCH DIVISION REPORT SERIES, SRD Research Report Number: Census/SRD/RR-87124
   - https://www.census.gov/content/dam/Census/library/working-papers/1987/adrm/rr87-24.pdf
 - Lynch, M. and A. Saalfeld, 1985, "Conflation: Automated Map Compilation, a Video Game Approach", Proceedings, Auto-Carto VII
   - https://cartogis.org/docs/proceedings/archive/auto-carto-7/pdf/conflation-automated-map-compilation-a-video-game-approach.pdf
 -->
 
 ## Toolchain
 
+<!--
+Rebuld documentation with
+    ./generate-help-markdown.sh
+-->
+
 ### csv2excel
 - [doc/csv2excel-help.md](doc/csv2excel-help.md)
 
-### csv2geojson
-- [doc/csv2geojson-help.md](doc/csv2geojson-help.md)
+### csvedit
+- [doc/csvedit-help.md](doc/csvedit-help.md)
+
+### dictionarybuilder
+- [doc/dictionarybuilder-help.md](doc/dictionarybuilder-help.md)
 
 ### geojsondiff
 - [doc/geojsondiff-help.md](doc/geojsondiff-help.md)
 
+### geojsonconcat
+- [doc/geojsonconcat-help.md](doc/geojsonconcat-help.md)
+
+### geojsonedit
+- [doc/geojsonedit-help.md](doc/geojsonedit-help.md)
+
+### geojsonmerger
+- [doc/geojsonmerger-help.md](doc/geojsonmerger-help.md)
+
+### csv2geojson
+- [doc/csv2geojson-help.md](doc/csv2geojson-help.md)
+
+### json2csv
+- [doc/json2csv-help.md](doc/json2csv-help.md)
+
+### overpassql2osmf
+- [doc/overpassql2osmf-help.md](doc/overpassql2osmf-help.md)
+
 <!--
 
 osmf2geojson
 osmf2geojson tests/data/test2.osm
 
 # https://docs.osmcode.org/osmium/latest/osmium-sort.html
 osmium sort -o tests/data/test2-v2.osm tests/data/test2.osm
 osmium sort -o tests/data/test1-v2.osm tests/data/test1.osm
 osmf2geojson tests/data/test2-v2.osm > tests/temp/test2-v2.geojson
 osmf2geojson tests/data/test1-v2.osm > tests/temp/test1-v2.geojson
 -->
-
-## License
-
-Public domain
```

### Comparing `gis-conflation-toolchain-0.7.0/README.md` & `gis-conflation-toolchain-0.7.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,65 @@
 [![Pypi: gis-conflation-toolchain](https://img.shields.io/badge/python%20pypi-gis--conflation--toolchain-brightgreen[Python] 
  "Pypi: gis-conflation-toolchain")](https://pypi.org/project/gis-conflation-toolchain)
 
 
 ## Installing
 
 ```bash
-# @TODO release this as pip package
-pip install --upgrade git+https://github.com/fititnt/spatial-data-conflation-open-toolchain.git#egg=gis-conflation-toolchain
+pip install --upgrade gis-conflation-toolchain
 ```
 
 <!--
 -  Saalfield, Alan. Conflation: Automated Map Compilation. BUREAU OF THE CENSUS STATISTICAL RESEARCH DIVISION REPORT SERIES, SRD Research Report Number: Census/SRD/RR-87124
   - https://www.census.gov/content/dam/Census/library/working-papers/1987/adrm/rr87-24.pdf
 - Lynch, M. and A. Saalfeld, 1985, "Conflation: Automated Map Compilation, a Video Game Approach", Proceedings, Auto-Carto VII
   - https://cartogis.org/docs/proceedings/archive/auto-carto-7/pdf/conflation-automated-map-compilation-a-video-game-approach.pdf
 -->
 
 ## Toolchain
 
+<!--
+Rebuld documentation with
+    ./generate-help-markdown.sh
+-->
+
 ### csv2excel
 - [doc/csv2excel-help.md](doc/csv2excel-help.md)
 
-### csv2geojson
-- [doc/csv2geojson-help.md](doc/csv2geojson-help.md)
+### csvedit
+- [doc/csvedit-help.md](doc/csvedit-help.md)
+
+### dictionarybuilder
+- [doc/dictionarybuilder-help.md](doc/dictionarybuilder-help.md)
 
 ### geojsondiff
 - [doc/geojsondiff-help.md](doc/geojsondiff-help.md)
 
+### geojsonconcat
+- [doc/geojsonconcat-help.md](doc/geojsonconcat-help.md)
+
+### geojsonedit
+- [doc/geojsonedit-help.md](doc/geojsonedit-help.md)
+
+### geojsonmerger
+- [doc/geojsonmerger-help.md](doc/geojsonmerger-help.md)
+
+### csv2geojson
+- [doc/csv2geojson-help.md](doc/csv2geojson-help.md)
+
+### json2csv
+- [doc/json2csv-help.md](doc/json2csv-help.md)
+
+### overpassql2osmf
+- [doc/overpassql2osmf-help.md](doc/overpassql2osmf-help.md)
+
 <!--
 
 osmf2geojson
 osmf2geojson tests/data/test2.osm
 
 # https://docs.osmcode.org/osmium/latest/osmium-sort.html
 osmium sort -o tests/data/test2-v2.osm tests/data/test2.osm
 osmium sort -o tests/data/test1-v2.osm tests/data/test1.osm
 osmf2geojson tests/data/test2-v2.osm > tests/temp/test2-v2.geojson
 osmf2geojson tests/data/test1-v2.osm > tests/temp/test1-v2.geojson
 -->
-
-## License
-
-Public domain
```

### Comparing `gis-conflation-toolchain-0.7.0/src/csv2excel/csv2excel.py` & `gis-conflation-toolchain-0.7.1/src/csv2excel/csv2excel.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.0/src/csv2geojson/csv2geojson.py` & `gis-conflation-toolchain-0.7.1/src/gisconflation/csv2gecodedcsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,60 @@
 #!/usr/bin/env python3
 # ==============================================================================
 #
-#          FILE:  csv2geojson.py
+#          FILE:  csv2gecodedcsv.py
 #
-#         USAGE:  ./scripts/csv2geojson.py
-#                 ./scripts/csv2geojson.py --help
+#         USAGE:  ./scripts/csv2gecodedcsv.py
+#                 ./scripts/csv2gecodedcsv.py --help
 #
-#   DESCRIPTION:  ---
+#   DESCRIPTION:  [DRAFT, not usable yet]
 #
 #       OPTIONS:  ---
 #
 #  REQUIREMENTS:  - python3
 #          BUGS:  ---
 #         NOTES:  ---
 #       AUTHORS:  Emerson Rocha <rocha[at]ieee.org>
 # COLLABORATORS:  ---
 #
 #       COMPANY:  EticaAI
-#       LICENSE:  Public Domain dedication or Zero-Clause BSD
-#                 SPDX-License-Identifier: Unlicense OR 0BSD
-#       VERSION:  v1.1.0
-#       CREATED:  2023-04-11 18:13 BRT
-#      REVISION:  2023-04-20 01:20 BRT v1.1 --contain-and-in
+#       LICENSE:  GNU Affero General Public License v3.0 or later
+#                 SPDX-License-Identifier: AGPL-3.0-or-later
+#       VERSION:  v0.5.0
+#       CREATED:  2023-05-06 16:54 BRT started, based on csv2geojson.py
+#      REVISION:  --
 # ==============================================================================
 
 
 # import geopandas
 # import os
 import argparse
 import csv
 import json
 import re
 import sys
 import string
 
+from gisconflation.util import parse_argument_values
 
-__VERSION__ = "1.1.0"
-PROGRAM = "csv2geojson"
+try:
+    import geocoder
+except ImportError:
+    raise ImportError("Dependency not found. Please: pip install geocoder")
+
+# https://geocoder.readthedocs.io/providers/OpenStreetMap.html
+print(geocoder.osm('Mountain View, CA'))
+
+# geocode 'New York city' --provider osm --out geojson | jq .
+
+__VERSION__ = "0.5.0"
+PROGRAM = "csv2gecodedcsv"
 DESCRIPTION = """
 ------------------------------------------------------------------------------
-CSV to GeoJSON
+[DRAFT, not usable yet] CSV to Geocoded CSV
 
 ------------------------------------------------------------------------------
 """.format(
     PROGRAM, __VERSION__
 )
 
 # https://www.rfc-editor.org/rfc/rfc7946
@@ -144,14 +155,26 @@
             help="the name of the longitude column",
             dest="lon",
             required=True,
             nargs="?",
         )
 
         parser.add_argument(
+            "--filter-contain",
+            help="Filter one or more fields for contain a string"
+            "Use '|||' to divide the field and the string. "
+            "Accept multiple values. "
+            "Example: "
+            "--filter-contain='name|||hospital'",
+            dest="filter_contain",
+            nargs="?",
+            action="append",
+        )
+
+        parser.add_argument(
             "--contain-or",
             help="If defined, only results that match at least one clause"
             " will appear on output. Accept multiple values."
             "--contain-or=tag1=value1 --contain-or=tag2=value2",
             dest="contain_or",
             nargs="?",
             action="append",
@@ -375,14 +398,15 @@
                 line_num += 1
 
                 if not geojson_item_contain(
                     row,
                     contain_or=_contain_or,
                     contain_and=_contain_and,
                     contain_and_in=_contain_and_in,
+                    filter_contain=parse_argument_values(pyargs.filter_contain),
                 ):
                     continue
 
                 formated_row = row_item_cast(
                     row,
                     line_num=line_num,
                     cast_integer=pyargs.cast_integer,
@@ -482,15 +506,19 @@
 
     result["properties"] = geojsom_item_properties(row, _ignore)
 
     return result
 
 
 def geojson_item_contain(
-    item, contain_or: list = None, contain_and: list = None, contain_and_in: list = None
+    item,
+    contain_or: list = None,
+    contain_and: list = None,
+    contain_and_in: list = None,
+    filter_contain: list = None,
 ) -> bool:
     if not item:
         return False
 
     if not contain_or and not contain_and and not contain_and_in:
         return True
 
@@ -528,14 +556,25 @@
         if _key not in item:
             raise SyntaxError(f"key {_key} not in {item}")
             # return False
 
         if _val is not True and _val != item[_key]:
             return False
 
+    if filter_contain:
+        for _key, _val in filter_contain.items():
+            _val = _val.lower()
+
+            if _key not in item:
+                raise SyntaxError(f"key {_key} not in {item}")
+                # return False
+
+            if _val is not True and item[_key].lower().find(_val) == -1:
+                return False
+
     return True
 
 
 def geojsom_item_properties(row: dict, ignore: list):
     result = {}
 
     for key, value in row.items():
```

### Comparing `gis-conflation-toolchain-0.7.0/src/geojsondiff/geojsondiff.py` & `gis-conflation-toolchain-0.7.1/src/geojsondiff/geojsondiff.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,24 +32,27 @@
 import argparse
 import csv
 import dataclasses
 import json
 import sys
 import logging
 from typing import List, Type
+import Levenshtein
 from haversine import haversine, Unit
 
 # from shapely.geometry import Polygon, Point
 from shapely.geometry import Polygon
 from xml.sax.saxutils import escape
 
+from gisconflation.util import LevenshteinHelper
+
 
 __VERSION__ = "0.6.1"
 
-PROGRAM = "geojson-diff"
+PROGRAM = "geojsondiff"
 DESCRIPTION = """
 ------------------------------------------------------------------------------
 GeoJSON++ diff
 
 ------------------------------------------------------------------------------
 """.format(
     __file__
@@ -192,14 +195,27 @@
             "Example: "
             "--pivot-attr-2='contact:email'",
             dest="pivot_attr_2",
             nargs="?",
             action="append",
         )
 
+        pivot.add_argument(
+            "--pivot-alias",
+            help="A weak (like name or description) attribute to order the matches. "
+            "Impefect. Never will return perfect match, even if exact the same. "
+            "Use '||' if attribute on A is not the same on the B. "
+            "Accept multiple values. "
+            "Example: "
+            "--pivot-alias'COMPANY_NAME||name' --pivot-alias'COMPANY_NAME||alt_name'",
+            dest="pivot_alias",
+            nargs="?",
+            action="append",
+        )
+
         prefilter = parser.add_argument_group("Pre-filter data before processing")
 
         prefilter.add_argument(
             "--prefilter-a-contain",
             help="Prefilter (e.g. before processing) a filed in A for a string"
             "Use '||' to divide the field and the string. "
             "Accept multiple values. "
@@ -312,14 +328,15 @@
         # print('oi', pyargs.pivot_key_main, pks_dict)
 
         crules = ConflationRules(
             distance_okay=int(pyargs.tdist),
             # pivot_key_main=parse_argument_values(pyargs.pivot_key_main),
             pivot_key_main=pivot_key_main,
             pivot_attr_2=parse_argument_values(pyargs.pivot_attr_2),
+            pivot_alias=parse_argument_values(pyargs.pivot_alias),
         )
 
         cfilters = ConflationFilters(
             filter_ab_dist_min=pyargs.filter_ab_dist_min,
             filter_ab_dist_max=pyargs.filter_ab_dist_max,
             filter_matched_key=pyargs.filter_matched_key,
             filter_matched_key_not=pyargs.filter_matched_key_not,
@@ -492,18 +509,20 @@
 
 class ConflationRules:
     def __init__(
         self,
         distance_okay: int = None,
         pivot_key_main: list = None,
         pivot_attr_2: list = None,
+        pivot_alias: list = None,
     ) -> None:
         self.distance_okay = distance_okay
         self.pivot_key_main = pivot_key_main
         self.pivot_attr_2 = pivot_attr_2
+        self.pivot_alias = pivot_alias
 
 
 class DatasetInMemory:
     def __init__(
         self,
         alias: str,
         group: str,
@@ -527,17 +546,18 @@
 
     def add_item(self, item: dict):
         self.index += 1
         # self.items.append(None)
 
         if (
             not item
+            or not isinstance(item, dict)
             or "geometry" not in item
+            or not item["geometry"]
             or "coordinates" not in item["geometry"]
-            or "type" not in item
         ):
             # Really bad input item (we still count on index)
             self.items.append(False)
             return False
 
         _properties = item["properties"] if "properties" in item else None
 
@@ -707,14 +727,16 @@
 
         return result.strip()
 
     def compute(self):
         """compute difference of B against A"""
         # for item in self.a.items:
 
+        levenshtein = LevenshteinHelper()
+
         if len(self.a.items) > 0:
             for index in range(0, len(self.a.items)):
                 if not self.a.items[index] or not self.a.items[index][1]:
                     continue
 
                 if (
                     "id" in self.a.items[index][1]
@@ -764,14 +786,15 @@
             # print(f"    > teste A i{index_a}", self.a.items[index_a])
             found = False
             # if not self.a.items[index_a]:
             #     self.matrix.append(None)
             # else:
             if self.a.items[index_a]:
                 candidates = []
+                candidates_aliases = []
                 for index_b in range(0, len(self.b.items)):
                     # print("oibb", len(self.b.items))
                     # print('a', self.a.items[index_a])
                     # print('b', self.b.items[index_b][0])
 
                     # Try perfect match (including tags)
                     if (
@@ -811,19 +834,51 @@
                             unit=Unit.METERS,
                         )
                         # print(f"        >> teste A i{index_a} vs B i{index_b}", dist)
                         if dist <= self.distance_okay:
                             # TODO sort by near
                             candidates.append((dist, index_b))
                             # self.matrix.append((index_b, MATCH_NEAR, round(dist, 2)))
+
+                            _aliasgroup = []
+                            if self.crules.pivot_alias:
+                                for refkey, altkey in self.crules.pivot_alias.items():
+                                    if altkey is True:
+                                        altkey = refkey
+                                if altkey in self.b.items[index_b][1]:
+                                    _aliasgroup.append(self.b.items[index_b][1][altkey])
+                                else:
+                                    # _aliasgroup.append(None)
+                                    # _aliasgroup.append('')
+                                    pass
+                            # print(_aliasgroup)
+                            candidates_aliases.append(_aliasgroup)
                             found = True
                         # break
 
             if found == True and len(candidates) > 0:
-                it = ItemMatcher(self.a.items[index_a], candidates, self.crules)
+                # candidates_aliases = []
+                item_aliases = []
+                if self.crules.pivot_alias:
+                    for refkey, _altkey in self.crules.pivot_alias.items():
+                        if refkey in self.a.items[index_a][1]:
+                            item_aliases.append(self.a.items[index_a][1][refkey])
+                        else:
+                            # item_aliases.append(None)
+                            item_aliases.append("")
+                # print(item_aliases)
+
+                it = ItemMatcher(
+                    self.a.items[index_a],
+                    item_aliases,
+                    candidates,
+                    candidates_aliases,
+                    self.crules,
+                    levenshtein,
+                )
                 self.matrix.append(it.result())
 
                 _temp = it.result()
                 if _temp is None:
                     self.matrix_v2.append(None)
                 else:
                     self.matrix_v2.append(
@@ -856,17 +911,24 @@
         # print("dataset a", self.a.items)
         print(self.b)
         # print("dataset b", self.b.items)
         print("matrix", self.matrix)
 
     def diff_geojson_full(self):
         dataobj = {"type": "FeatureCollection", "features": []}
+
+        _repeatcheck = {}
+
         for index_a in range(0, len(self.a.items)):
             _item_a = self.a.items[index_a]
 
+            if not _item_a:
+                # Skip very bad input (invalid geometry)
+                continue
+
             _matrix = self.matrix[index_a]
 
             final_properties = {}
             pointer = None
 
             # print("_item_a", _item_a)
             if _item_a[2] is not None:
@@ -938,14 +1000,30 @@
             #     final_properties["action"] = "retag"
             #     final_properties["marker-color"] = "#660000"
             # else:
             #     # 'move':   '#110055',  # moving an existing node
             #     final_properties["action"] = "move"
             #     final_properties["marker-color"] = "#110055"
 
+            _hash = str(hash(str(final_geometry)))
+            if _hash not in _repeatcheck:
+                _repeatcheck[_hash] = 0
+            else:
+                _repeatcheck[_hash] += 1
+                if final_geometry["type"] == "Point":
+                    final_properties["__coordinates_original"] = final_geometry[
+                        "coordinates"
+                    ]
+                    final_geometry["coordinates"][0] = final_geometry["coordinates"][
+                        0
+                    ] + (_repeatcheck[_hash] * 0.0001)
+                    final_geometry["coordinates"][1] = final_geometry["coordinates"][
+                        1
+                    ] - (_repeatcheck[_hash] * 0.0001)
+
             res = {
                 "geometry": final_geometry,
                 "properties": final_properties,
                 "type": "Feature",
                 # "_debug": f"_item_a {_item_a}",
                 # "_original": _item_a,
             }
@@ -1061,14 +1139,17 @@
             "desc_b",
             "near_a",
         ]
         data = []
 
         for index_a in range(0, len(self.a.items)):
             _item_a = self.a.items[index_a]
+            if not _item_a:
+                # Skip very bad input (invalid geometry)
+                continue
 
             _matrix = self.matrix[index_a]
 
             # print(_item_a, _matrix)
             # print(_item_a[1], _matrix)
             # # print(_item_a[1])
             # print('aa', _matrix)
@@ -1141,28 +1222,44 @@
         data.insert(0, header)
 
         # return data.insert(0, header)
         return data
 
 
 class ItemMatcher:
-    def __init__(self, item, candidates: list, crules: Type[ConflationRules]) -> None:
+    def __init__(
+        self,
+        item,
+        item_aliases: list,
+        candidates: list,
+        candidates_aliases: list,
+        crules: Type["ConflationRules"],
+        levenshtein: Type["LevenshteinHelper"],
+    ) -> None:
         self.item = item
         # self.candidates = candidates
         ## Improve this part
         self.candidates_valid = None
         self.automacher = None
         self.crules = crules
+        self.levenshtein = levenshtein
 
-        self.compute(candidates)
+        self.compute(item_aliases, candidates_aliases, candidates)
 
-    def compute(self, candidates):
+    def compute(self, item_aliases, candidates_aliases, candidates):
         # candidates = self.candidates
 
-        candidates_sorted = sorted(candidates, key=lambda tup: tup[0])
+        # print(self.item, candidates)
+        _ext = []
+        for idx, item in enumerate(candidates):
+            _ext.append((item[0], item[1], item_aliases, candidates_aliases[idx]))
+        # candidates_sorted = sorted(candidates, key=lambda tup: tup[0])
+        candidates_sorted = sorted(
+            _ext, key=lambda tup: Levenshtein.setratio(tup[2], tup[3]), reverse=True
+        )
 
         # Improve this part
         self.candidates_valid = candidates_sorted
 
         dist = candidates_sorted[0][0]
         index_b = candidates_sorted[0][1]
         skiped = None
```

### Comparing `gis-conflation-toolchain-0.7.0/src/gis_conflation_toolchain.egg-info/PKG-INFO` & `gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,88 @@
 Metadata-Version: 2.1
 Name: gis-conflation-toolchain
-Version: 0.7.0
+Version: 0.7.1
 Summary: gis-conflation-toolchain
 Home-page: https://github.com/fititnt/spatial-data-conflation-open-toolchain
 Author: Emerson Rocha
 Author-email: rocha@ieee.org
 Project-URL: Bug Tracker, https://github.com/fititnt/spatial-data-conflation-open-toolchain/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: extras
 License-File: LICENSE
 
 # spatial-data-conflation-open-toolchain
 **[EARLY DRAFT] Open, free to use, toolchain for geospatial data conflation. Command-line interface for file manipulation.** _See geojson-diff.py from <https://github.com/fititnt/openstreetmap-vs-dados-abertos-brasil>._
 
 [![GitHub](https://img.shields.io/badge/GitHub-fititnt%20spatial--data--conflation--open--toolchain-lightgrey?logo=github&style=social[fititnt/geojson-diff] "GitHub")](https://github.com/fititnt/spatial-data-conflation-open-toolchain)
 
 [![Pypi: gis-conflation-toolchain](https://img.shields.io/badge/python%20pypi-gis--conflation--toolchain-brightgreen[Python] 
  "Pypi: gis-conflation-toolchain")](https://pypi.org/project/gis-conflation-toolchain)
 
 
 ## Installing
 
 ```bash
-# @TODO release this as pip package
-pip install --upgrade git+https://github.com/fititnt/spatial-data-conflation-open-toolchain.git#egg=gis-conflation-toolchain
+pip install --upgrade gis-conflation-toolchain
 ```
 
 <!--
 -  Saalfield, Alan. Conflation: Automated Map Compilation. BUREAU OF THE CENSUS STATISTICAL RESEARCH DIVISION REPORT SERIES, SRD Research Report Number: Census/SRD/RR-87124
   - https://www.census.gov/content/dam/Census/library/working-papers/1987/adrm/rr87-24.pdf
 - Lynch, M. and A. Saalfeld, 1985, "Conflation: Automated Map Compilation, a Video Game Approach", Proceedings, Auto-Carto VII
   - https://cartogis.org/docs/proceedings/archive/auto-carto-7/pdf/conflation-automated-map-compilation-a-video-game-approach.pdf
 -->
 
 ## Toolchain
 
+<!--
+Rebuld documentation with
+    ./generate-help-markdown.sh
+-->
+
 ### csv2excel
 - [doc/csv2excel-help.md](doc/csv2excel-help.md)
 
-### csv2geojson
-- [doc/csv2geojson-help.md](doc/csv2geojson-help.md)
+### csvedit
+- [doc/csvedit-help.md](doc/csvedit-help.md)
+
+### dictionarybuilder
+- [doc/dictionarybuilder-help.md](doc/dictionarybuilder-help.md)
 
 ### geojsondiff
 - [doc/geojsondiff-help.md](doc/geojsondiff-help.md)
 
+### geojsonconcat
+- [doc/geojsonconcat-help.md](doc/geojsonconcat-help.md)
+
+### geojsonedit
+- [doc/geojsonedit-help.md](doc/geojsonedit-help.md)
+
+### geojsonmerger
+- [doc/geojsonmerger-help.md](doc/geojsonmerger-help.md)
+
+### csv2geojson
+- [doc/csv2geojson-help.md](doc/csv2geojson-help.md)
+
+### json2csv
+- [doc/json2csv-help.md](doc/json2csv-help.md)
+
+### overpassql2osmf
+- [doc/overpassql2osmf-help.md](doc/overpassql2osmf-help.md)
+
 <!--
 
 osmf2geojson
 osmf2geojson tests/data/test2.osm
 
 # https://docs.osmcode.org/osmium/latest/osmium-sort.html
 osmium sort -o tests/data/test2-v2.osm tests/data/test2.osm
 osmium sort -o tests/data/test1-v2.osm tests/data/test1.osm
 osmf2geojson tests/data/test2-v2.osm > tests/temp/test2-v2.geojson
 osmf2geojson tests/data/test1-v2.osm > tests/temp/test1-v2.geojson
 -->
-
-## License
-
-Public domain
```

### Comparing `gis-conflation-toolchain-0.7.0/src/gisconflation/osmf2geojson.py` & `gis-conflation-toolchain-0.7.1/src/gisconflation/osmf2geojson.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.0/src/gisconflation/overpassql2osmf.py` & `gis-conflation-toolchain-0.7.1/src/gisconflation/overpassql2osmf.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #                   - pip install pandas (https://pandas.pydata.org/)
 #          BUGS:  ---
 #         NOTES:  ---
 #       AUTHORS:  Emerson Rocha <rocha[at]ieee.org>
 # COLLABORATORS:  ---
 #
 #       COMPANY:  EticaAI
-#       LICENSE:  Public Domain dedication or Zero-Clause BSD
-#                 SPDX-License-Identifier: Unlicense OR 0BSD
+#       LICENSE:  GNU Affero General Public License v3.0 or later
+#                 SPDX-License-Identifier: AGPL-3.0-or-later
 #       VERSION:  v0.2.0
 #       CREATED:  2023-04-26 01:04 BRT
 #      REVISION:  ---
 # ==============================================================================
 
 # ./src/gisconflation/overpassql2osmf.py --help
 # ./src/gisconflation/overpassql2osmf.py tests/data/cnes.overpassql > tests/temp/cnes.osm.json
@@ -56,15 +56,21 @@
     PROGRAM, __VERSION__
 )
 
 __EPILOGUM__ = """
 ------------------------------------------------------------------------------
                             EXEMPLŌRUM GRATIĀ
 ------------------------------------------------------------------------------
-    {0} input.csv output.xlsx
+Input file contains Overpass query . . . . . . . . . . . . . . . . . . . . . .
+    {0} tests/data/cnes.overpassql > tests/temp/cnes.osm
+
+CSV Output (requires special Overpass query) . . . . . . . . . . . . . . . . .
+
+    {0} '[out:csv(::id,::type,"name")]; area[name="Bonn"]; nwr(area)[railway=station]; out;' \
+> tests/temp/bonn.osm.csv
 ------------------------------------------------------------------------------
                             EXEMPLŌRUM GRATIĀ
 ------------------------------------------------------------------------------
 """.format(
     PROGRAM
 )
```

### Comparing `gis-conflation-toolchain-0.7.0/tests/test_main.py` & `gis-conflation-toolchain-0.7.1/tests/test_main.py`

 * *Files identical despite different names*

