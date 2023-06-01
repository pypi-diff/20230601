# Comparing `tmp/caf.space-1.2.2.tar.gz` & `tmp/caf.space-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caf.space-1.2.2.tar", last modified: Mon Apr 24 12:13:05 2023, max compression
+gzip compressed data, was "caf.space-1.3.0.tar", last modified: Thu Jun  1 10:37:44 2023, max compression
```

## Comparing `caf.space-1.2.2.tar` & `caf.space-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.554793 caf.space-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 12:12:49.000000 caf.space-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-24 12:13:05.554793 caf.space-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-24 12:12:49.000000 caf.space-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-24 12:12:49.000000 caf.space-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 12:13:05.554793 caf.space-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-24 12:12:49.000000 caf.space-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.550794 caf.space-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.550794 caf.space-1.2.2/src/caf/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.554793 caf.space-1.2.2/src/caf/space/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-24 12:13:05.554793 caf.space-1.2.2/src/caf/space/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/weighted_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/zone_correspondence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/zone_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.554793 caf.space-1.2.2/src/caf.space.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.554793 caf.space-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-24 12:12:49.000000 caf.space-1.2.2/tests/test_weighted_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-04-24 12:12:49.000000 caf.space-1.2.2/tests/test_zone_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:37:44.164983 caf.space-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 10:37:31.000000 caf.space-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-01 10:37:44.164983 caf.space-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-06-01 10:37:31.000000 caf.space-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-01 10:37:31.000000 caf.space-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-01 10:37:44.164983 caf.space-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-01 10:37:31.000000 caf.space-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:37:44.160983 caf.space-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:37:44.160983 caf.space-1.3.0/src/caf/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:37:44.164983 caf.space-1.3.0/src/caf/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 10:37:44.164983 caf.space-1.3.0/src/caf/space/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/weighted_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/zone_correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-01 10:37:31.000000 caf.space-1.3.0/src/caf/space/zone_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:37:44.160983 caf.space-1.3.0/src/caf.space.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-01 10:37:44.000000 caf.space-1.3.0/src/caf.space.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-01 10:37:44.000000 caf.space-1.3.0/src/caf.space.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:37:44.000000 caf.space-1.3.0/src/caf.space.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 10:37:44.000000 caf.space-1.3.0/src/caf.space.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 10:37:44.000000 caf.space-1.3.0/src/caf.space.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 10:37:44.000000 caf.space-1.3.0/src/caf.space.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:37:44.164983 caf.space-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-01 10:37:31.000000 caf.space-1.3.0/tests/test_weighted_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-01 10:37:31.000000 caf.space-1.3.0/tests/test_zone_translation.py
```

### Comparing `caf.space-1.2.2/LICENSE` & `caf.space-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/PKG-INFO` & `caf.space-1.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: caf.space
-Version: 1.2.2
-Summary: Easily generate translations between transport zoning systems
-Home-page: https://github.com/Transport-for-the-North/caf.space
-Author: Transport for the North
-Maintainer: Transport for the North
-License: GPL-3.0
-Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.space/issues
-Project-URL: Source, https://github.com/Transport-for-the-North/caf.space
-Project-URL: Documentation, https://cafspcae.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 ![Transport for the North Logo](https://github.com/Transport-for-the-North/caf.toolkit/blob/main/docs/TFN_Landscape_Colour_CMYK.png)
 
 <h1 align="center">CAF.Space</h1>
 
 <p align="center">
 <a href="https://www.gnu.org/licenses/gpl-3.0.en.html"><img alt="License: GNU GPL v3.0" src="https://img.shields.io/badge/license-GPLv3-blueviolet.svg"></a>
 <a href="https://github.com/PyCQA/pylint"><img alt="linting: pylint" src="https://img.shields.io/badge/linting-pylint-yellowgreen"></a>
@@ -32,14 +14,28 @@
 translations in .csv format describing how to convert between different zoning systems.
 The aim is to free tools up from directly having to do their own geo-processing, and    
 instead have a single source of truth to get them from! For more info see https://cafspcae.readthedocs.io/en/latest/.
 
 <u><h3> Tool info </h3></u>
 The tool has two main options for running a translation, either a purely spatial translation (where overlapping zones are split by area), or a weighted translation where overlapping zones are split by some other type of weighting data like population or employment data. For most purposes a weighted translation will be more accurate, and it is up to the user to decide the most appropriate weighting data to use. For both types of translation the tool runs from a set of parameters within a config class. If you are using the GUI then provide parameters in the first tab. If you are not using the GUI a instance of inputs.ZoningTranslationInputs is required. This can either be loaded from a yaml file, or initialised in the code.
 
+<u><h3> Command Line Tool </h3></u>
+The tool can be run from command line, with the command:
+
+<b> python -m caf.space </b>
+
+This can be run with no arguments, which will launch the GUI, but there are also 3 arguments for running in different modes.:
+* <b> mode: --mode</b> must be either "GUI" (default value), "spatial", or "weighted". "Gui" launches the GUI and the other two produce spatial or weighted zone translations respectively.
+* <b> config_path: --config</b> must be provided if mode is either "spatial" or "weighted". This is a path to the config file containing parameters for that translation.
+* <b> out_path: --out_path</b> must be provided if either "spatial" or "weighted". This is the directory you want your translation saved to. This directory must exist and will not be generated internally.
+
+Running with all three arguments would look like:
+
+<b> python -m caf.space --mode "spatial" --config "path/to/config.yml" --out_path "path/to/output/folder" </b>
+
 <u><h4> Spatial Correspondence </h4></u>
 For a spatial correspondence, the only user inputs needed are shapefiles for the two zone systems you want a translation between. The parameters required for a spatial translation are as follows:
 
 * <b> zone_1:</b><br>
     <b>name:</b> The name of the first zone system you are providing. This should be as simple as possible, so for an MSOA shapefile, name should simply be MSOA.<br>
     <b>shapefile:</b> A file path to the shapefile you want a translation for.<br>
     <b>id_col:</b> The name of the unique ID column in your chosen shapefile. This can be any column as long as it is unique for each zone in the shapefile.<br>
```

#### html2text {}

```diff
@@ -1,19 +1,9 @@
-Metadata-Version: 2.1 Name: caf.space Version: 1.2.2 Summary: Easily generate
-translations between transport zoning systems Home-page: https://github.com/
-Transport-for-the-North/caf.space Author: Transport for the North Maintainer:
-Transport for the North License: GPL-3.0 Project-URL: Bug Tracker, https://
-github.com/Transport-for-the-North/caf.space/issues Project-URL: Source, https:
-//github.com/Transport-for-the-North/caf.space Project-URL: Documentation,
-https://cafspcae.readthedocs.io/en/latest/ Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9 Requires-
-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra: testing
-License-File: LICENSE ![Transport for the North Logo](https://github.com/
-Transport-for-the-North/caf.toolkit/blob/main/docs/
-TFN_Landscape_Colour_CMYK.png)
+![Transport for the North Logo](https://github.com/Transport-for-the-North/
+caf.toolkit/blob/main/docs/TFN_Landscape_Colour_CMYK.png)
                             ****** CAF.Space ******
  [License:_GNU_GPL_v3.0] [linting:_pylint] [code_format:_Google_Style_Guide]
                               [code_style:_black]
 Common Analytical Framework (CAF) Space contains geo-processing functionality
 useful for transport planners. Primarily it is a tool for generating standard
 weighting translations in .csv format describing how to convert between
 different zoning systems. The aim is to free tools up from directly having to
@@ -26,14 +16,27 @@
 data like population or employment data. For most purposes a weighted
 translation will be more accurate, and it is up to the user to decide the most
 appropriate weighting data to use. For both types of translation the tool runs
 from a set of parameters within a config class. If you are using the GUI then
 provide parameters in the first tab. If you are not using the GUI a instance of
 inputs.ZoningTranslationInputs is required. This can either be loaded from a
 yaml file, or initialised in the code.
+**** Command Line Tool ****
+ The tool can be run from command line, with the command: python -m caf.space
+This can be run with no arguments, which will launch the GUI, but there are
+also 3 arguments for running in different modes.: * mode: --mode must be either
+"GUI" (default value), "spatial", or "weighted". "Gui" launches the GUI and the
+other two produce spatial or weighted zone translations respectively. *
+config_path: --config must be provided if mode is either "spatial" or
+"weighted". This is a path to the config file containing parameters for that
+translation. * out_path: --out_path must be provided if either "spatial" or
+"weighted". This is the directory you want your translation saved to. This
+directory must exist and will not be generated internally. Running with all
+three arguments would look like: python -m caf.space --mode "spatial" --config
+"path/to/config.yml" --out_path "path/to/output/folder"
 *** Spatial Correspondence ***
  For a spatial correspondence, the only user inputs needed are shapefiles for
 the two zone systems you want a translation between. The parameters required
 for a spatial translation are as follows: * zone_1:
 name: The name of the first zone system you are providing. This should be as
 simple as possible, so for an MSOA shapefile, name should simply be MSOA.
 shapefile: A file path to the shapefile you want a translation for.
```

### Comparing `caf.space-1.2.2/pyproject.toml` & `caf.space-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/setup.cfg` & `caf.space-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/src/caf/space/inputs.py` & `caf.space-1.3.0/src/caf/space/inputs.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,30 +10,34 @@
 ##### IMPORTS #####
 from __future__ import annotations
 
 # Standard imports
 # pylint: disable=import-error
 import logging
 import datetime
+import dataclasses
 import fiona
 import os
 from pathlib import Path
 import pandas as pd
 from typing import Optional
 from pydantic import validator
+from enum import Enum
 
 # Third party imports
 from caf.toolkit import BaseConfig
+import argparse
 
 # pylint: enable=import-error
 # Local imports
 
 ##### CONSTANTS #####
 LOG = logging.getLogger(__name__)
 CACHE_PATH = "I:/Data/Zone Translations/cache"
+MODES = ("spatial", "weighted", "GUI")
 
 
 class ZoneSystemInfo(BaseConfig):
     """Base class for storing information about a shapefile input.
 
     Parameters
     ----------
@@ -153,14 +157,67 @@
     def _valid_data_col(cls, v, values):
         cols = pd.read_csv(values["weight_data"], nrows=1).columns
         if v not in cols:
             raise ValueError(f"The given col, {v}, does not appear in the weight data.")
         return v
 
 
+@dataclasses.dataclass
+class SpaceArguments:
+    """Command Line arguments for running space."""
+
+    config_path: Path
+    mode: str
+    out_path: Path
+
+    @classmethod
+    def parse(cls) -> SpaceArguments:
+        """Parse command line argument."""
+        parser = argparse.ArgumentParser(
+            description=__doc__, formatter_class=argparse.ArgumentDefaultsHelpFormatter
+        )
+        parser.add_argument(
+            "--mode",
+            type=str,
+            help="Mode to run translation in; spatial, weighted or GUI.",
+            default="GUI",
+            required=False,
+        )
+        parser.add_argument(
+            "--config",
+            type=Path,
+            help="path to config file containing parameters",
+            default=None,
+            required=False,
+        )
+        parser.add_argument(
+            "--out_path",
+            type=Path,
+            help="Path the translation will be saved in.",
+            default=None,
+            required=False,
+        )
+
+        parsed_args = parser.parse_args()
+        return SpaceArguments(parsed_args.config, parsed_args.mode, parsed_args.out_path)
+
+    def validate(self):
+        """Raise error for invalid input."""
+        if self.config_path:
+            if not self.config_path.is_file():
+                raise FileNotFoundError(f"config file doesn't exist: {self.config_path}")
+
+        if self.out_path:
+            if not self.out_path.is_dir():
+                raise FileNotFoundError(f"{self.out_path} does not exist.")
+
+        if self.mode not in MODES:
+            raise ValueError(f"{self.mode} is not a valid mode for caf.space to run in.")
+
+
 class ZoningTranslationInputs(BaseConfig):
     """
     Class for storing and reading input parameters for `ZoneTranslation`.
 
     Parameters
     ----------
     zone_1: TransZoneSystemInfo
```

### Comparing `caf.space-1.2.2/src/caf/space/metadata.py` & `caf.space-1.3.0/src/caf/space/metadata.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/src/caf/space/ui.py` & `caf.space-1.3.0/src/caf/space/ui.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/src/caf/space/utils.py` & `caf.space-1.3.0/src/caf/space/utils.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/src/caf/space/weighted_funcs.py` & `caf.space-1.3.0/src/caf/space/weighted_funcs.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/src/caf/space/zone_correspondence.py` & `caf.space-1.3.0/src/caf/space/zone_correspondence.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/src/caf/space/zone_translation.py` & `caf.space-1.3.0/src/caf/space/zone_translation.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/src/caf.space.egg-info/PKG-INFO` & `caf.space-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.space
-Version: 1.2.2
+Version: 1.3.0
 Summary: Easily generate translations between transport zoning systems
 Home-page: https://github.com/Transport-for-the-North/caf.space
 Author: Transport for the North
 Maintainer: Transport for the North
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.space/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.space
@@ -32,14 +32,28 @@
 translations in .csv format describing how to convert between different zoning systems.
 The aim is to free tools up from directly having to do their own geo-processing, and    
 instead have a single source of truth to get them from! For more info see https://cafspcae.readthedocs.io/en/latest/.
 
 <u><h3> Tool info </h3></u>
 The tool has two main options for running a translation, either a purely spatial translation (where overlapping zones are split by area), or a weighted translation where overlapping zones are split by some other type of weighting data like population or employment data. For most purposes a weighted translation will be more accurate, and it is up to the user to decide the most appropriate weighting data to use. For both types of translation the tool runs from a set of parameters within a config class. If you are using the GUI then provide parameters in the first tab. If you are not using the GUI a instance of inputs.ZoningTranslationInputs is required. This can either be loaded from a yaml file, or initialised in the code.
 
+<u><h3> Command Line Tool </h3></u>
+The tool can be run from command line, with the command:
+
+<b> python -m caf.space </b>
+
+This can be run with no arguments, which will launch the GUI, but there are also 3 arguments for running in different modes.:
+* <b> mode: --mode</b> must be either "GUI" (default value), "spatial", or "weighted". "Gui" launches the GUI and the other two produce spatial or weighted zone translations respectively.
+* <b> config_path: --config</b> must be provided if mode is either "spatial" or "weighted". This is a path to the config file containing parameters for that translation.
+* <b> out_path: --out_path</b> must be provided if either "spatial" or "weighted". This is the directory you want your translation saved to. This directory must exist and will not be generated internally.
+
+Running with all three arguments would look like:
+
+<b> python -m caf.space --mode "spatial" --config "path/to/config.yml" --out_path "path/to/output/folder" </b>
+
 <u><h4> Spatial Correspondence </h4></u>
 For a spatial correspondence, the only user inputs needed are shapefiles for the two zone systems you want a translation between. The parameters required for a spatial translation are as follows:
 
 * <b> zone_1:</b><br>
     <b>name:</b> The name of the first zone system you are providing. This should be as simple as possible, so for an MSOA shapefile, name should simply be MSOA.<br>
     <b>shapefile:</b> A file path to the shapefile you want a translation for.<br>
     <b>id_col:</b> The name of the unique ID column in your chosen shapefile. This can be any column as long as it is unique for each zone in the shapefile.<br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.space Version: 1.2.2 Summary: Easily generate
+Metadata-Version: 2.1 Name: caf.space Version: 1.3.0 Summary: Easily generate
 translations between transport zoning systems Home-page: https://github.com/
 Transport-for-the-North/caf.space Author: Transport for the North Maintainer:
 Transport for the North License: GPL-3.0 Project-URL: Bug Tracker, https://
 github.com/Transport-for-the-North/caf.space/issues Project-URL: Source, https:
 //github.com/Transport-for-the-North/caf.space Project-URL: Documentation,
 https://cafspcae.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9 Requires-
@@ -26,14 +26,27 @@
 data like population or employment data. For most purposes a weighted
 translation will be more accurate, and it is up to the user to decide the most
 appropriate weighting data to use. For both types of translation the tool runs
 from a set of parameters within a config class. If you are using the GUI then
 provide parameters in the first tab. If you are not using the GUI a instance of
 inputs.ZoningTranslationInputs is required. This can either be loaded from a
 yaml file, or initialised in the code.
+**** Command Line Tool ****
+ The tool can be run from command line, with the command: python -m caf.space
+This can be run with no arguments, which will launch the GUI, but there are
+also 3 arguments for running in different modes.: * mode: --mode must be either
+"GUI" (default value), "spatial", or "weighted". "Gui" launches the GUI and the
+other two produce spatial or weighted zone translations respectively. *
+config_path: --config must be provided if mode is either "spatial" or
+"weighted". This is a path to the config file containing parameters for that
+translation. * out_path: --out_path must be provided if either "spatial" or
+"weighted". This is the directory you want your translation saved to. This
+directory must exist and will not be generated internally. Running with all
+three arguments would look like: python -m caf.space --mode "spatial" --config
+"path/to/config.yml" --out_path "path/to/output/folder"
 *** Spatial Correspondence ***
  For a spatial correspondence, the only user inputs needed are shapefiles for
 the two zone systems you want a translation between. The parameters required
 for a spatial translation are as follows: * zone_1:
 name: The name of the first zone system you are providing. This should be as
 simple as possible, so for an MSOA shapefile, name should simply be MSOA.
 shapefile: A file path to the shapefile you want a translation for.
```

### Comparing `caf.space-1.2.2/src/caf.space.egg-info/SOURCES.txt` & `caf.space-1.3.0/src/caf.space.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/caf.space.egg-info/PKG-INFO
 src/caf.space.egg-info/SOURCES.txt
 src/caf.space.egg-info/dependency_links.txt
 src/caf.space.egg-info/namespace_packages.txt
 src/caf.space.egg-info/requires.txt
 src/caf.space.egg-info/top_level.txt
 src/caf/space/__init__.py
+src/caf/space/__main__.py
 src/caf/space/_version.py
 src/caf/space/inputs.py
 src/caf/space/metadata.py
 src/caf/space/ui.py
 src/caf/space/utils.py
 src/caf/space/weighted_funcs.py
 src/caf/space/zone_correspondence.py
```

### Comparing `caf.space-1.2.2/tests/test_weighted_funcs.py` & `caf.space-1.3.0/tests/test_weighted_funcs.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.2/tests/test_zone_translation.py` & `caf.space-1.3.0/tests/test_zone_translation.py`

 * *Files identical despite different names*

