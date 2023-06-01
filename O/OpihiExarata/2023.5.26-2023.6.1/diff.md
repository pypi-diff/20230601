# Comparing `tmp/OpihiExarata-2023.5.26.tar.gz` & `tmp/OpihiExarata-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpihiExarata-2023.5.26.tar", last modified: Fri May 26 05:19:56 2023, max compression
+gzip compressed data, was "OpihiExarata-2023.6.1.tar", last modified: Thu Jun  1 04:57:35 2023, max compression
```

## Comparing `OpihiExarata-2023.5.26.tar` & `OpihiExarata-2023.6.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 05:19:39.000000 OpihiExarata-2023.5.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-26 05:19:39.000000 OpihiExarata-2023.5.26/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.795427 OpihiExarata-2023.5.26/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.799427 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.799427 OpihiExarata-2023.5.26/src/opihiexarata/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.799427 OpihiExarata-2023.5.26/src/opihiexarata/astrometry/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/astrometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/astrometry/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/astrometry/webclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/configuration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.803427 OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/jplhorizons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.803427 OpihiExarata-2023.5.26/src/opihiexarata/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)   128567 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.807427 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/automatic.ui
--rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
--rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
--rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/old_manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    17432 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/selector.ui
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/window_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    50479 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.807427 OpihiExarata-2023.5.26/src/opihiexarata/library/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/mpcrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/phototable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/tcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/src/opihiexarata/opihi/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/opihi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42391 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/opihi/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/opihi/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/opihi/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/src/opihiexarata/orbit/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/orbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/orbit/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/orbit/orbfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/orbit/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/src/opihiexarata/photometry/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/photometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/photometry/panstarrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/photometry/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/src/opihiexarata/propagate/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/propagate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/propagate/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/propagate/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/tests/test_global.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 04:57:17.000000 OpihiExarata-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-01 04:57:17.000000 OpihiExarata-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.333420 OpihiExarata-2023.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.337420 OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-01 04:57:35.000000 OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-01 04:57:35.000000 OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 04:57:35.000000 OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 04:57:35.000000 OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-01 04:57:35.000000 OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 04:57:35.000000 OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.337420 OpihiExarata-2023.6.1/src/opihiexarata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.337420 OpihiExarata-2023.6.1/src/opihiexarata/astrometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/astrometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/astrometry/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/astrometry/webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/configuration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.337420 OpihiExarata-2023.6.1/src/opihiexarata/ephemeris/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/ephemeris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/ephemeris/jplhorizons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/ephemeris/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.337420 OpihiExarata-2023.6.1/src/opihiexarata/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128567 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.341421 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/automatic.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
+-rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/old_manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    17432 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/qtui_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/qtui_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/qtui_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/selector.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/window_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50479 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/gui/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/src/opihiexarata/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/mpcrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/phototable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/tcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/library/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/src/opihiexarata/opihi/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/opihi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42391 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/opihi/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/opihi/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/opihi/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/src/opihiexarata/orbit/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/orbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/orbit/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/orbit/orbfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/orbit/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/src/opihiexarata/photometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/photometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/photometry/panstarrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/photometry/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/src/opihiexarata/propagate/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/propagate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/propagate/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/propagate/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/src/opihiexarata/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:57:35.345420 OpihiExarata-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 04:57:18.000000 OpihiExarata-2023.6.1/tests/test_global.py
```

### Comparing `OpihiExarata-2023.5.26/LICENSE` & `OpihiExarata-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/PKG-INFO` & `OpihiExarata-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.5.26
+Version: 2023.6.1
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.5.26/README.md` & `OpihiExarata-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/setup.py` & `OpihiExarata-2023.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/PKG-INFO` & `OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.5.26
+Version: 2023.6.1
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/SOURCES.txt` & `OpihiExarata-2023.6.1/src/OpihiExarata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/__init__.py` & `OpihiExarata-2023.6.1/src/opihiexarata/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/__main__.py` & `OpihiExarata-2023.6.1/src/opihiexarata/__main__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/astrometry/solution.py` & `OpihiExarata-2023.6.1/src/opihiexarata/astrometry/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/astrometry/webclient.py` & `OpihiExarata-2023.6.1/src/opihiexarata/astrometry/webclient.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/configuration.yaml` & `OpihiExarata-2023.6.1/src/opihiexarata/configuration.yaml`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/jplhorizons.py` & `OpihiExarata-2023.6.1/src/opihiexarata/ephemeris/jplhorizons.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/solution.py` & `OpihiExarata-2023.6.1/src/opihiexarata/ephemeris/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/__init__.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/automatic.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/functions.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/functions.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/manual.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/manual.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/name.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/name.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/automatic.ui` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/automatic.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/manual.ui` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/old_manual.ui` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/old_manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_automatic.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/qtui_automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_manual.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/qtui_manual.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_selector.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/qtui_selector.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/selector.ui` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/selector.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/window_icon.png` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/qtui/window_icon.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/gui/selector.py` & `OpihiExarata-2023.6.1/src/opihiexarata/gui/selector.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/__init__.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/config.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/config.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/conversion.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/conversion.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/engine.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/engine.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/error.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/error.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/fits.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/fits.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/hint.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/hint.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/http.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/http.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/image.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/image.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/json.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/json.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/mpcrecord.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/mpcrecord.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/path.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/path.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/phototable.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/phototable.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/tcs.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/tcs.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/library/temporary.py` & `OpihiExarata-2023.6.1/src/opihiexarata/library/temporary.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/opihi/database.py` & `OpihiExarata-2023.6.1/src/opihiexarata/opihi/database.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/opihi/preprocess.py` & `OpihiExarata-2023.6.1/src/opihiexarata/opihi/preprocess.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/opihi/solution.py` & `OpihiExarata-2023.6.1/src/opihiexarata/opihi/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/orbit/custom.py` & `OpihiExarata-2023.6.1/src/opihiexarata/orbit/custom.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/orbit/orbfit.py` & `OpihiExarata-2023.6.1/src/opihiexarata/orbit/orbfit.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/orbit/solution.py` & `OpihiExarata-2023.6.1/src/opihiexarata/orbit/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/photometry/panstarrs.py` & `OpihiExarata-2023.6.1/src/opihiexarata/photometry/panstarrs.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/photometry/solution.py` & `OpihiExarata-2023.6.1/src/opihiexarata/photometry/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/propagate/polynomial.py` & `OpihiExarata-2023.6.1/src/opihiexarata/propagate/polynomial.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.26/src/opihiexarata/propagate/solution.py` & `OpihiExarata-2023.6.1/src/opihiexarata/propagate/solution.py`

 * *Files identical despite different names*

