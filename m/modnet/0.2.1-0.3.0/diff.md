# Comparing `tmp/modnet-0.2.1.tar.gz` & `tmp/modnet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modnet-0.2.1.tar", last modified: Thu Feb  9 15:38:43 2023, max compression
+gzip compressed data, was "dist/modnet-0.3.0.tar", last modified: Thu Jun  1 14:29:47 2023, max compression
```

## Comparing `modnet-0.2.1.tar` & `modnet-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.2.1/LICENSE.md
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.2.1/MANIFEST.in
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     5983 2023-02-09 15:38:43.000000 modnet-0.2.1/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4139 2023-02-09 15:34:41.000000 modnet-0.2.1/README.md
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2023-02-09 15:34:49.000000 modnet-0.2.1/modnet/__init__.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/data/
--rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.2.1/modnet/data/Features_cross
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.2.1/modnet/ext_data.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/featurizers/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.2.1/modnet/featurizers/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    10893 2023-02-07 16:34:07.000000 modnet-0.2.1/modnet/featurizers/featurizers.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/featurizers/presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      736 2023-01-23 13:07:39.000000 modnet-0.2.1/modnet/featurizers/presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9990 2023-01-23 13:07:39.000000 modnet-0.2.1/modnet/featurizers/presets/debreuck_2020.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     8222 2023-01-23 13:07:39.000000 modnet-0.2.1/modnet/featurizers/presets/matminer_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      492 2021-09-08 13:24:57.000000 modnet-0.2.1/modnet/featurizers/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/hyper_opt/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.2.1/modnet/hyper_opt/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    24201 2023-01-23 13:07:39.000000 modnet-0.2.1/modnet/hyper_opt/fit_genetic.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/matbench/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.2.1/modnet/matbench/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    11627 2022-02-08 11:33:52.000000 modnet-0.2.1/modnet/matbench/benchmark.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/model_presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.2.1/modnet/model_presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.2.1/modnet/model_presets/presets.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/models/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      190 2022-05-10 12:28:41.000000 modnet-0.2.1/modnet/models/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    15042 2022-08-30 16:25:35.000000 modnet-0.2.1/modnet/models/bayesian.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17296 2023-02-07 16:34:07.000000 modnet-0.2.1/modnet/models/ensemble.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    32356 2023-02-09 15:34:41.000000 modnet-0.2.1/modnet/models/vanilla.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    40770 2023-01-23 13:07:39.000000 modnet-0.2.1/modnet/preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6345 2022-05-19 13:18:13.000000 modnet-0.2.1/modnet/sklearn.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet/tests/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.2.1/modnet/tests/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3410 2023-01-23 13:07:39.000000 modnet-0.2.1/modnet/tests/conftest.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-01-23 13:07:39.000000 modnet-0.2.1/modnet/tests/test_benchmark.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.2.1/modnet/tests/test_ext_data.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      770 2022-01-12 21:23:06.000000 modnet-0.2.1/modnet/tests/test_hyper_opt.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9497 2023-01-23 13:07:39.000000 modnet-0.2.1/modnet/tests/test_model.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17841 2023-02-09 15:34:41.000000 modnet-0.2.1/modnet/tests/test_preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.2.1/modnet/tests/test_sklearn.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.2.1/modnet/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet.egg-info/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     5983 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet.egg-info/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1062 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet.egg-info/SOURCES.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet.egg-info/dependency_links.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      192 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet.egg-info/requires.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2023-02-09 15:38:43.000000 modnet-0.2.1/modnet.egg-info/top_level.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2023-02-09 15:38:43.000000 modnet-0.2.1/setup.cfg
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1961 2023-02-09 15:34:41.000000 modnet-0.2.1/setup.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.3.0/LICENSE.md
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.3.0/MANIFEST.in
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6122 2023-06-01 14:29:47.000000 modnet-0.3.0/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4238 2023-05-08 13:57:20.000000 modnet-0.3.0/README.md
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2023-06-01 14:27:20.000000 modnet-0.3.0/modnet/__init__.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/data/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.3.0/modnet/data/Features_cross
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.3.0/modnet/ext_data.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/featurizers/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.3.0/modnet/featurizers/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    12289 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/featurizers/featurizers.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/featurizers/presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/featurizers/presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9990 2023-01-23 13:07:39.000000 modnet-0.3.0/modnet/featurizers/presets/debreuck_2020.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9213 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/featurizers/presets/matminer_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    15893 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/featurizers/presets/matminer_all_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      492 2021-09-08 13:24:57.000000 modnet-0.3.0/modnet/featurizers/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/hyper_opt/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.3.0/modnet/hyper_opt/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    27252 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/hyper_opt/fit_genetic.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/matbench/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.3.0/modnet/matbench/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-06-01 13:18:02.000000 modnet-0.3.0/modnet/matbench/benchmark.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/model_presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.3.0/modnet/model_presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.3.0/modnet/model_presets/presets.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/models/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      190 2022-05-10 12:28:41.000000 modnet-0.3.0/modnet/models/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    15042 2022-08-30 16:25:35.000000 modnet-0.3.0/modnet/models/bayesian.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    17880 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/models/ensemble.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    39117 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/models/vanilla.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    41703 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6345 2022-05-19 13:18:13.000000 modnet-0.3.0/modnet/sklearn.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/tests/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.3.0/modnet/tests/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3410 2023-01-23 13:07:39.000000 modnet-0.3.0/modnet/tests/conftest.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-01-23 13:07:39.000000 modnet-0.3.0/modnet/tests/test_benchmark.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.3.0/modnet/tests/test_ext_data.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/tests/test_hyper_opt.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9497 2023-01-23 13:07:39.000000 modnet-0.3.0/modnet/tests/test_model.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    18202 2023-06-01 13:18:02.000000 modnet-0.3.0/modnet/tests/test_preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.3.0/modnet/tests/test_sklearn.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.3.0/modnet/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6122 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/SOURCES.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/dependency_links.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      192 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/requires.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/top_level.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2023-06-01 14:29:47.000000 modnet-0.3.0/setup.cfg
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1961 2023-02-09 15:34:41.000000 modnet-0.3.0/setup.py
```

### Comparing `modnet-0.2.1/LICENSE.md` & `modnet-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/PKG-INFO` & `modnet-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.2.1
+Version: 0.3.0
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
 Description: # MODNet: Material Optimal Descriptor Network
         
         [![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
         
+        <p align="center">
+            <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
+            <br>
+        </p>
+        
         <a name="introduction"></a>
         ## Introduction
         This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
         It is a supervised machine learning framework for **learning material properties** from
         either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
         and can be used for learning *multiple* properties together by using **joint learning**.
```

### Comparing `modnet-0.2.1/README.md` & `modnet-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # MODNet: Material Optimal Descriptor Network
 
 [![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
 
+<p align="center">
+    <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
+    <br>
+</p>
+
 <a name="introduction"></a>
 ## Introduction
 This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
 It is a supervised machine learning framework for **learning material properties** from
 either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
 and can be used for learning *multiple* properties together by using **joint learning**.
```

### Comparing `modnet-0.2.1/modnet/data/Features_cross` & `modnet-0.3.0/modnet/data/Features_cross`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/ext_data.py` & `modnet-0.3.0/modnet/ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/featurizers/featurizers.py` & `modnet-0.3.0/modnet/featurizers/featurizers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 from typing import Optional, Iterable, Tuple, Dict
 
 import pandas as pd
+from pymatgen.core import Composition
 
 from matminer.featurizers.base import MultipleFeaturizer, BaseFeaturizer
 from matminer.featurizers.structure import SiteStatsFingerprint
 from matminer.featurizers.conversions import CompositionToOxidComposition
 
 from modnet.utils import LOG
 
@@ -200,22 +201,49 @@
                 mode=self.featurizer_mode,
             )
             df = df.rename(columns={"Input Data": ""})
             df.columns = df.columns.map("|".join).str.strip("|")
 
         if self.oxid_composition_featurizers:
             LOG.info("Applying oxidation state featurizers...")
+            # Get integer composition if some are not
+            col_comp = "composition"
+            if not all(
+                all(amt == int(amt) for amt in comp.values())
+                for comp in df["composition"].values
+            ):
+                LOG.info(
+                    "There are non-integer compositions in the dataset, and featurizers that need them. "
+                    "Computing..."
+                )
+                df["integer_composition"] = [
+                    Composition(
+                        comp.get_integer_formula_and_factor(
+                            max_denominator=10
+                            if getattr(self, "fast_oxid", False)
+                            else 100
+                        )[0]
+                    )
+                    for comp in df["composition"].values
+                ]
+                # df["integer_composition"] = df["composition"].apply(
+                # lambda c: c.get_integer_formula_and_factor(
+                #         max_denominator=10 if getattr(self, "fast_oxid", False) else 100
+                #     )[0]
+                # )
+
+                col_comp = "integer_composition"
             if getattr(self, "fast_oxid", False):
                 df = CompositionToOxidComposition(
                     all_oxi_states=False, max_sites=-1
-                ).featurize_dataframe(df, "composition")
+                ).featurize_dataframe(df, col_id=col_comp)
             else:
-                df = CompositionToOxidComposition().featurize_dataframe(
-                    df, "composition"
-                )
+                df = CompositionToOxidComposition(
+                    max_sites=-1 if getattr(self, "continuous_only", False) else None
+                ).featurize_dataframe(df, col_id=col_comp, ignore_errors=True)
             df = self._fit_apply_featurizers(
                 df,
                 self.oxid_composition_featurizers,
                 "composition_oxid",
                 mode=self.featurizer_mode,
             )
             df = df.rename(columns={"Input Data": ""})
@@ -267,22 +295,24 @@
 
         LOG.info("Applying site featurizers...")
 
         df = df.copy()
         df.columns = ["Input data|" + x for x in df.columns]
 
         for fingerprint in self.site_featurizers:
+            fingerprint_name = fingerprint.__class__.__name__
+            if fingerprint_name == "SOAP":
+                fingerprint.fit(df["Input data|structure"])
             site_stats_fingerprint = SiteStatsFingerprint(
                 fingerprint, stats=self.site_stats
             )
             df = site_stats_fingerprint.featurize_dataframe(
                 df, "Input data|structure", multiindex=False, ignore_errors=True
             )
 
-            fingerprint_name = fingerprint.__class__.__name__
             if aliases:
                 fingerprint_name = aliases.get(fingerprint_name, fingerprint_name)
             if "|" not in fingerprint_name:
                 fingerprint_name += "|"
             df.columns = [
                 f"{fingerprint_name}{x}" if "|" not in x else x for x in df.columns
             ]
```

### Comparing `modnet-0.2.1/modnet/featurizers/presets/debreuck_2020.py` & `modnet-0.3.0/modnet/featurizers/presets/debreuck_2020.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/featurizers/presets/matminer_2023.py` & `modnet-0.3.0/modnet/featurizers/presets/matminer_2023.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 
     Follows the same philosophy and featurizer list as the `DeBreuck2020Featurizer`
     but with with many features changing their underlying matminer implementation,
     definition and behaviour since the creation of the former featurizer.
 
     """
 
-    def __init__(self, fast_oxid: bool = False):
+    def __init__(self, fast_oxid: bool = False, continuous_only: bool = False):
         """Creates the featurizer and imports all featurizer functions.
 
         Parameters:
             fast_oxid: Whether to use the accelerated oxidation state parameters within
                 pymatgen when constructing features that constrain oxidation states such
                 that all sites with the same species in a structure will have the same
                 oxidation state (recommended if featurizing any structure
                 with large unit cells).
 
         """
 
         super().__init__()
-        self.load_featurizers()
+        self.continuous_only = continuous_only
         self.fast_oxid = fast_oxid
+        self.load_featurizers()
 
     def load_featurizers(self):
         with contextlib.redirect_stdout(None):
             from pymatgen.analysis.local_env import VoronoiNN
             from matminer.featurizers.composition import (
                 AtomicOrbitals,
                 AtomicPackingEfficiency,
@@ -78,27 +79,41 @@
                 GaussianSymmFunc,
                 GeneralizedRadialDistributionFunction,
                 LocalPropertyDifference,
                 OPSiteFingerprint,
                 VoronoiFingerprint,
             )
 
-            self.composition_featurizers = (
-                AtomicOrbitals(),
-                AtomicPackingEfficiency(),
-                BandCenter(),
-                ElementFraction(),
-                ElementProperty.from_preset("magpie"),
-                IonProperty(),
-                Miedema(),
-                Stoichiometry(),
-                TMetalFraction(),
-                ValenceOrbital(),
-                YangSolidSolution(),
-            )
+            if self.continuous_only:
+                magpie_featurizer = ElementProperty.from_preset("magpie")
+                magpie_featurizer.stats = ["mean", "avg_dev"]
+
+                self.composition_featurizers = (
+                    BandCenter(),
+                    ElementFraction(),
+                    magpie_featurizer,
+                    IonProperty(fast=self.fast_oxid),
+                    Stoichiometry(p_list=[2, 3, 5, 7, 10]),
+                    TMetalFraction(),
+                    ValenceOrbital(props=["frac"]),
+                )
+            else:
+                self.composition_featurizers = (
+                    AtomicOrbitals(),
+                    AtomicPackingEfficiency(),
+                    BandCenter(),
+                    ElementFraction(),
+                    ElementProperty.from_preset("magpie"),
+                    IonProperty(),
+                    Miedema(),
+                    Stoichiometry(),
+                    TMetalFraction(),
+                    ValenceOrbital(),
+                    YangSolidSolution(),
+                )
 
             self.oxid_composition_featurizers = (
                 ElectronegativityDiff(),
                 OxidationStates(),
             )
 
             self.structure_featurizers = (
@@ -141,28 +156,32 @@
         renames some fields and cleans the output dataframe.
 
         """
         from pymatgen.core.periodic_table import Element
 
         df = super().featurize_composition(df)
 
-        _orbitals = {"s": 1, "p": 2, "d": 3, "f": 4}
-        df["AtomicOrbitals|HOMO_character"] = df["AtomicOrbitals|HOMO_character"].map(
-            _orbitals
-        )
-        df["AtomicOrbitals|LUMO_character"] = df["AtomicOrbitals|LUMO_character"].map(
-            _orbitals
-        )
-
-        df["AtomicOrbitals|HOMO_element"] = df["AtomicOrbitals|HOMO_element"].apply(
-            lambda x: -1 if not isinstance(x, str) else Element(x).Z
-        )
-        df["AtomicOrbitals|LUMO_element"] = df["AtomicOrbitals|LUMO_element"].apply(
-            lambda x: -1 if not isinstance(x, str) else Element(x).Z
-        )
+        if not self.continuous_only:
+            _orbitals = {"s": 1, "p": 2, "d": 3, "f": 4}
+            df["AtomicOrbitals|HOMO_character"] = df[
+                "AtomicOrbitals|HOMO_character"
+            ].map(_orbitals)
+            df["AtomicOrbitals|LUMO_character"] = df[
+                "AtomicOrbitals|LUMO_character"
+            ].map(_orbitals)
+
+            df["AtomicOrbitals|HOMO_element"] = df["AtomicOrbitals|HOMO_element"].apply(
+                lambda x: -1 if not isinstance(x, str) else Element(x).Z
+            )
+            df["AtomicOrbitals|LUMO_element"] = df["AtomicOrbitals|LUMO_element"].apply(
+                lambda x: -1 if not isinstance(x, str) else Element(x).Z
+            )
+
+        else:
+            df.drop(columns=["IonProperty|max ionic char"], inplace=True)
 
         return modnet.featurizers.clean_df(df)
 
     def featurize_structure(self, df):
         """Applies the preset structural featurizers to the input dataframe,
         renames some fields and cleans the output dataframe.
 
@@ -220,12 +239,12 @@
     """This subclass simply disables structure and site-level features
     from the main `Matminer2023Featurizer` class.
 
     This should yield identical results to the original 2020 version.
 
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, continuous_only: bool = False, fast_oxid: bool = False):
+        super().__init__(fast_oxid=fast_oxid, continuous_only=continuous_only)
         self.oxid_composition_featurizers = ()
         self.structure_featurizers = ()
         self.site_featurizers = ()
```

### Comparing `modnet-0.2.1/modnet/hyper_opt/fit_genetic.py` & `modnet-0.3.0/modnet/hyper_opt/fit_genetic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import random
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Union, Callable
 import numpy as np
 import tensorflow as tf
 from sklearn.model_selection import train_test_split
 from modnet.preprocessing import MODData
 from modnet.models import MODNetModel, EnsembleMODNetModel
 from modnet.utils import LOG
 import multiprocessing
@@ -16,46 +16,61 @@
     """Class representing a set of hyperparameters for the genetic algorithm."""
 
     def __init__(
         self,
         max_feat: int,
         num_classes: dict,
         multi_label: bool,
+        loss: Union[str, Callable] = "mae",
         targets: List = None,
         weights: Dict[str, float] = None,
+        **fit_params,
     ) -> Individual:
         """
         Args:
             max_feat (int): Maximum number of features
             num_classes (dict): MODData num_classes parameter.Used for distinguishing between regression and classification.
             multi_label (bool): whether the task is a classification multi-label problem.
+            loss: The built-in tf.keras loss to pass to `compile(...)`.
             targets (List): Optional (for joint learning only). A nested list of targets names that defines the hierarchy
                 of the output layers.
             weights (Dict[str, float]): Optional (for joint learning only). The relative loss weights to apply for each target.
+            fit_params: Any additional parameters to pass to `MODNetModel.fit(...)`,
         """
 
+        self.act = "elu"
+        self.loss = loss
+        self.n_neurons_first_layer = 32 * random.randint(1, 10)
         self.max_feat = max_feat
         self.num_classes = num_classes
         self.multi_label = multi_label
         self.targets = targets
         self.weights = weights
+        self.fit_params = fit_params
 
         self.xscale_list = ["minmax", "standard"]
+        self.impute_missing_list = [0, "mean"]
+        self.xscale_before_impute = True
         self.lr_list = [0.1, 0.01, 0.005, 0.001]
         self.batch_size_list = [32, 64, 128, 256]
         self.fraction_list = [1, 0.75, 0.5, 0.25]
 
+        if fit_params:
+            self.__dict__.update(fit_params)
+
         self.genes = {
-            "act": "elu",
-            "loss": "mae",
-            "n_neurons_first_layer": 32 * random.randint(1, 10),
+            "act": self.act,
+            "loss": self.loss,
+            "n_neurons_first_layer": self.n_neurons_first_layer,
             "fraction1": random.choice(self.fraction_list),
             "fraction2": random.choice(self.fraction_list),
             "fraction3": random.choice(self.fraction_list),
             "xscale": random.choice(self.xscale_list),
+            "impute_missing": random.choice(self.impute_missing_list),
+            "xscale_before_impute": self.xscale_before_impute,
             "lr": random.choice(self.lr_list),
             "batch_size": random.choice(self.batch_size_list),
             "n_feat": 0,
         }
 
         if max_feat <= 100:
             b = int(max_feat / 2)
@@ -73,28 +88,29 @@
         Args:
             partner (Individual): Partner individual.
         Returns:
             Individual: Child.
         """
 
         genes_from_mother = random.sample(
-            range(10), k=5
-        )  # creates indices to take randomly 5 genes from one parent, and 5 genes from the other
+            range(len(self.genes)), k=len(self.genes) // 2
+        )  # creates indices to take randomly half the genes from one parent, and half the genes from the other
 
         child_genes = {
             list(self.genes.keys())[i]: list(self.genes.values())[i]
             if i in genes_from_mother
             else list(partner.genes.values())[i]
-            for i in range(10)
+            for i in range(len(self.genes))
         }
 
         child = Individual(
             max_feat=self.max_feat,
             num_classes=self.num_classes,
             multi_label=self.multi_label,
+            loss=self.genes["loss"],
             targets=self.targets,
             weights=self.weights,
         )
         child.genes = child_genes
         return child
 
     def mutation(self, prob_mut: float) -> None:
@@ -107,14 +123,15 @@
         """
 
         if np.random.rand() < prob_mut:
             individual = Individual(
                 max_feat=self.max_feat,
                 num_classes=self.num_classes,
                 multi_label=self.multi_label,
+                loss=self.genes["loss"],
                 targets=self.targets,
                 weights=self.weights,
             )
             # modification of the number of features in a [-10%, +10%] range
             self.genes["n_feat"] = np.absolute(
                 int(
                     self.genes["n_feat"]
@@ -197,25 +214,32 @@
                     )
                 ],
             ],
             act=self.genes["act"],
             num_classes=self.num_classes,
             multi_label=self.multi_label,
         )
-
+        if "custom_data" in train_data.df_targets.columns:
+            custom_data = np.array(list(train_data.df_targets["custom_data"].values))
+        else:
+            custom_data = None
         model.fit(
             train_data,
+            custom_data=custom_data,
             val_data=val_data,
             loss=self.genes["loss"],
             lr=self.genes["lr"],
             epochs=800 if not fast else 1,
             batch_size=self.genes["batch_size"],
             xscale=self.genes["xscale"],
+            impute_missing=self.genes["impute_missing"],
+            xscale_before_impute=self.genes["xscale_before_impute"],
             callbacks=callbacks,
             verbose=0,
+            **self.fit_params,
         )
 
         self.val_loss = model.evaluate(val_data)
         self.model = model
 
     def refit_model(self, data: MODData, n_models=10, n_jobs=1, fast: bool = False):
         """Refit inner model on specified data.
@@ -258,60 +282,83 @@
                     )
                 ],
             ],
             act=self.genes["act"],
             num_classes=self.num_classes,
             multi_label=self.multi_label,
         )
-
+        if "custom_data" in data.df_targets.columns:
+            custom_data = np.array(list(data.df_targets["custom_data"].values))
+        else:
+            custom_data = None
         model.fit(
             data,
+            custom_data=custom_data,
             n_jobs=n_jobs,
             val_fraction=0,
             loss=self.genes["loss"],
             lr=self.genes["lr"],
             epochs=800 if not fast else 1,
             batch_size=self.genes["batch_size"],
             xscale=self.genes["xscale"],
+            impute_missing=self.genes["impute_missing"],
+            xscale_before_impute=self.genes["xscale_before_impute"],
             callbacks=callbacks,
             verbose=0,
+            **self.fit_params,
         )
 
         self.model = model
         return self.model
 
 
 class FitGenetic:
     """Class optimizing the model parameters using a genetic algorithm."""
 
     def __init__(
         self,
         data: MODData,
+        custom_data: Optional[np.ndarray] = None,
         targets: List = None,
         weights: Dict[str, float] = None,
         sample_threshold: int = 5000,
+        ignore_names: Optional[List] = [],
     ):
         """Genetic algorithm hyperparameter optimization for MODNet.
 
         Args:
             data (MODData): Training MODData
+            custom_data (np.ndarray): Optional array of shape (n_sampels, n_custom_props) that will be appended to the targets (columns wise).
+                This can be useful for defining custom loss functions.
             targets (List): Optional (for joint learning only). A nested list of targets names that defines the hierarchy
                 of the output layers.
             weights (Dict[str, float]): Optional (for joint learning only). The relative loss weights to apply for each target.
             sample_threshold (int, optional): If the dataset size exceeds this threshold, individuals are
                 trained on sampled subsets of this size. Defaults to 5000.
+            ignore_names (List): Optional list of property names to ignore during feature selection.
+                Feature selection will be performed w.r.t. all properties except the ones in ignore_names.
+
         """
+        for n in ignore_names:
+            if n not in data.names:
+                raise RuntimeError(
+                    f"Names provided in ignore_names should be part of {data.names}. {n} was not found."
+                )
+
         self.data = data
+        if custom_data is not None:
+            self.data.df_targets["custom_data"] = [list(x) for x in custom_data]
         subset_ids = np.random.permutation(len(data.df_featurized))[:sample_threshold]
         self.train_data, _ = data.split((subset_ids, []))
         self.num_classes = data.num_classes
+        t_names = list(set(data.names).difference(set(ignore_names)))
         if targets is None:
-            targets = [[data.target_names]]
+            targets = [[t_names]]
         if weights is None:
-            weights = {n: 1 for n in data.target_names}
+            weights = {n: 1 for n in t_names}
         self.targets = targets
         self.weights = weights
 
         LOG.info("Targets:")
         for i, (k, v) in enumerate(self.num_classes.items()):
             if v >= 2:
                 type = "classification"
@@ -330,30 +377,40 @@
             )
         )
 
     def _end_run(self):
         self.pool.close()
         self.pool.join()
 
-    def initialization_population(self, size_pop: int, multi_label: bool) -> None:
+    def initialization_population(
+        self,
+        size_pop: int,
+        multi_label: bool,
+        loss: Union[str, Callable] = "mae",
+        **fit_params,
+    ) -> None:
         """Initializes the initial population (Generation 0).
 
         Args:
             size_pop (int): Size of population.
             multi_label: Whether the problem (if classification) is multi-label.
                 In this case the softmax output-activation is replaced by a sigmoid.
+            loss: The built-in tf.keras loss to pass to `compile(...)`.
+            fit_params: Any additional parameters to pass to `MODNetModel.fit(...)`,
         """
 
         self.pop = [
             Individual(
                 max_feat=len(self.train_data.get_optimal_descriptors()),
                 num_classes=self.train_data.num_classes,
                 multi_label=multi_label,
+                loss=loss,
                 targets=self.targets,
                 weights=self.weights,
+                **fit_params,
             )
             for _ in range(size_pop)
         ]
 
     def function_fitness(
         self,
         pop: List[Individual],
@@ -436,17 +493,15 @@
         ):
             individual, individual_id, fold_id = res
             individual.model._restore_model()
             val_losses[individual_id, fold_id] = individual.val_loss
             individuals[individual_id] = individual
             models[individual_id][fold_id] = individual.model
 
-        models = [
-            EnsembleMODNetModel(modnet_models=inner_models) for inner_models in models
-        ]
+        models = [EnsembleMODNetModel(models=inner_models) for inner_models in models]
         val_loss_per_individual = np.mean(val_losses, axis=1)
         res_str = "Loss per individual: "
         for ind, vl in enumerate(val_loss_per_individual):
             res_str += "ind {}: {:.3f} \t".format(ind, vl)
         LOG.info(res_str)
 
         os.environ["TF_CPP_MIN_LOG_LEVEL"] = "0"  # reset
@@ -456,46 +511,53 @@
     def run(
         self,
         size_pop: int = 20,
         num_generations: int = 10,
         prob_mut: Optional[int] = None,
         nested: Optional[int] = 5,
         multi_label: bool = False,
+        loss: Union[str, Callable] = "mae",
         n_jobs: Optional[int] = None,
         early_stopping: Optional[int] = 4,
         refit: Optional[int] = 5,
         fast=False,
+        **fit_params,
     ) -> EnsembleMODNetModel:
         """Run the GA and return best model.
 
         Args:
             size_pop (int, optional): Size of the population per generation.. Defaults to 20.
             num_generations (int, optional): Size of the population per generation. Defaults to 10.
             prob_mut (Optional[int], optional): Probability of mutation. Defaults to None.
             nested (Optional[int], optional): CV fold size. Use <=0 for hold-out validation. Defaults to 5.
             multi_label: Whether the problem (if classification) is multi-label.
                 In this case the softmax output-activation is replaced by a sigmoid.
+            loss: The built-in tf.keras loss to pass to `compile(...)`.
             n_jobs (Optional[int], optional): Number of jobs to parallelize on. Defaults to None.
             early_stopping (Optional[int], optional): Number of successive generations without improvement before stopping. Defaults to 4.
-            refit (Optional[int], optional): Wether to refit (>0) the best hyperparameters on the whole dataset or use the best Individual instead (=0).
-                The amount corresponds the the number of models used in the ensemble. Defaults to 0.
+            refit (Optional[int], optional): Whether to refit (>0) the best hyperparameters on the whole dataset or use the best Individual instead (=0).
+                The amount corresponds to the number of models used in the ensemble. Defaults to 0.
             fast (bool, optional): Use only for debugging and testing. A fast GA run with small number of epochs, generations, individuals and folds.
                 Overrides the size_pop, num_generation and nested arguments.. Defaults to False.
+            fit_params: Any additional parameters to pass to `MODNetModel.fit(...)`,
 
         Returns:
             EnsembleMODNetModel: Fitted model with best hyperparameters
         """
         self._init_run(n_jobs=n_jobs)
 
         if fast:
             size_pop, num_generations, nested = 2, 2, 2
 
         LOG.info("Generation number 0")
         self.initialization_population(
-            size_pop, multi_label=multi_label
+            size_pop,
+            multi_label=multi_label,
+            loss=loss,
+            **fit_params,
         )  # initialization of the population
         val_loss, models, individuals = self.function_fitness(
             pop=self.pop,
             nested=nested,
             n_jobs=n_jobs,
             multi_label=multi_label,
             fast=fast,
@@ -584,25 +646,25 @@
                 self.pool.imap_unordered(_map_refit_individual, tasks, chunksize=1),
                 total=len(tasks),
             ):
                 model = res
                 model._restore_model()
                 ensemble.append(model)
 
-            self.best_model = EnsembleMODNetModel(modnet_models=ensemble)
+            self.best_model = EnsembleMODNetModel(models=ensemble)
             """
             self.best_model = self.best_individual.refit_model(
-                self.data, n_models=refit, n_jobs=n_jobs, fast=fast
+                self.data, n_models=refit, n_jobs=n_jobs or 1, fast=fast
             )
 
         else:
             ensemble = []
-            for m in models[ranking[:10]]:
+            for m in models[ranking[:refit]]:
                 ensemble += m.model
-            self.best_model = EnsembleMODNetModel(modnet_models=ensemble)
+            self.best_model = EnsembleMODNetModel(models=ensemble)
 
         self.results = self.best_individual.genes
 
         return self.best_model
 
 
 def _map_evaluate_individual(kwargs):
```

### Comparing `modnet-0.2.1/modnet/matbench/benchmark.py` & `modnet-0.3.0/modnet/matbench/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ):
 
         def _mapArrayToInt(a):
             return np.array(a).dot(2 ** np.arange(len(a)))
 
         ycv = data.df_targets.iloc[:, 0].map(_mapArrayToInt)
     else:
-        ycv = data.df_targets
+        ycv = data.df_targets.values[:, 0]
 
     kf = KFold(n_splits=n_splits, shuffle=True, random_state=MATBENCH_SEED)
     kf_splits = kf.split(data.df_featurized, y=ycv)
     return kf_splits
 
 
 def matbench_benchmark(
```

### Comparing `modnet-0.2.1/modnet/model_presets/presets.py` & `modnet-0.3.0/modnet/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/models/bayesian.py` & `modnet-0.3.0/modnet/models/bayesian.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/models/ensemble.py` & `modnet-0.3.0/modnet/models/ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,39 +37,48 @@
             was trained for.
 
     """
 
     can_return_uncertainty = True
 
     def __init__(
-        self, *args, n_models=100, bootstrap=True, modnet_models=None, **kwargs
+        self,
+        *args,
+        n_models=100,
+        bootstrap=True,
+        models=None,
+        modnet_models=None,
+        **kwargs,
     ):
         """
         Args:
             *args: See MODNetModel
             n_models: number of inner MODNetModels, each model has the same architecture defined by the args nd kwargs.
             bootstrap: whether to bootstrap the samples for each inner MODNet fit.
-            modnet_models: List of user provided MODNetModels. Enables to have different architectures. n_models is discarded in this case.
+            models: List of user provided MODNetModels. Enables to have different architectures. n_models is discarded in this case.
+            modnet_model: Deprecated. Same argument as models. For backward compatibility only.
             **kwargs: See MODNetModel
         """
         self.__modnet_version__ = __version__
         self.bootstrap = bootstrap
-        if modnet_models is None:
-            self.model = []
+        if modnet_models is not None and models is None:
+            models = modnet_models
+        if models is None:
+            self.models = []
             self.n_models = n_models
             for i in range(self.n_models):
-                self.model.append(MODNetModel(*args, **kwargs))
+                self.models.append(MODNetModel(*args, **kwargs))
         else:
-            self.model = modnet_models
-            self.n_models = len(modnet_models)
+            self.models = models
+            self.n_models = len(models)
 
-        self.targets = self.model[0].targets
-        self.weights = self.model[0].weights
-        self.num_classes = self.model[0].num_classes
-        self.out_act = self.model[0].out_act
+        self.targets = self.models[0].targets
+        self.weights = self.models[0].weights
+        self.num_classes = self.models[0].num_classes
+        self.out_act = self.models[0].out_act
 
     def fit(
         self,
         training_data: MODData,
         n_jobs=1,
         **kwargs,
     ) -> None:
@@ -95,26 +104,26 @@
             ]
         else:
             train_datas = [training_data for _ in range(self.n_models)]
 
         if n_jobs <= 1:
             for i in range(self.n_models):
                 LOG.info(f"Bootstrap fitting model #{i + 1}/{self.n_models}")
-                self.model[i].fit(train_datas[i], **kwargs)
+                self.models[i].fit(train_datas[i], **kwargs)
                 model_summary = ""
-                for k in self.model[i].history.keys():
+                for k in self.models[i].history.keys():
                     model_summary += "{}: {:.4f}\t".format(
-                        k, self.model[i].history[k][-1]
+                        k, self.models[i].history[k][-1]
                     )
                 LOG.info(model_summary)
         else:
             ctx = multiprocessing.get_context("spawn")
             pool = ctx.Pool(processes=n_jobs)
             tasks = []
-            for i, m in enumerate(self.model):
+            for i, m in enumerate(self.models):
                 m._make_picklable()
                 tasks.append(
                     {
                         "model": m,
                         "training_data": train_datas[i],
                         "model_id": i,
                         **kwargs,
@@ -122,15 +131,15 @@
                 )
             for res in tqdm.tqdm(
                 pool.imap_unordered(_map_fit_MODNet, tasks, chunksize=1),
                 total=self.n_models,
             ):
                 model, model_id = res
                 model._restore_model()
-                self.model[model_id] = model
+                self.models[model_id] = model
                 model_summary = f"Model #{model_id}\t"
                 for k in model.history.keys():
                     model_summary += "{}: {:.4f}\t".format(k, model.history[k][-1])
                 LOG.info(model_summary)
             pool.close()
             pool.join()
 
@@ -138,27 +147,27 @@
         self, test_data: MODData, return_unc=False, return_prob=False
     ) -> pd.DataFrame:
         """Predict the target values for the passed MODData.
 
         Parameters:
             test_data: A featurized and feature-selected `MODData`
                 object containing the descriptors used in training.
-            return_prob: For a classification tasks only: whether to return the probability of each
+            return_prob: For a classification task only: whether to return the probability of each
                 class OR only return the most probable class.
-            return_unc: wheter to return a second dataframe containing the uncertainties
+            return_unc: whether to return a second dataframe containing the uncertainties
 
         Returns:
             A `pandas.DataFrame` containing the predicted values of the targets.
 
 
         """
 
         all_predictions = []
         for i in range(self.n_models):
-            p = self.model[i].predict(test_data, return_prob=return_prob)
+            p = self.models[i].predict(test_data, return_prob=return_prob)
             all_predictions.append(p.values)
 
         p_mean = np.array(all_predictions).mean(axis=0)
         p_std = np.array(all_predictions).std(axis=0)
 
         df_mean = pd.DataFrame(p_mean, index=p.index, columns=p.columns)
         df_std = pd.DataFrame(p_std, index=p.index, columns=p.columns)
@@ -176,15 +185,15 @@
                 object containing the descriptors used in training.
 
 
         Returns:
             Loss score
         """
         all_losses = np.zeros(self.n_models)
-        for i, m in enumerate(self.model):
+        for i, m in enumerate(self.models):
             all_losses[i] = m.evaluate(test_data)
 
         return all_losses.mean()
 
     def fit_preset(
         self,
         data: MODData,
@@ -209,15 +218,15 @@
         This function implements the "inner loop" of a cross-validation workflow. By
         modifying the `nested` argument, it can be run in full nested mode (i.e.
         train n_fold * n_preset models) or just with a simple random hold-out set.
 
         The data is first fitted on several well working MODNet presets
         with a validation set (10% of the furnished data by default).
 
-        Sets the `self.model` attribute to the model with the lowest mean validation loss across
+        Sets the `self.models` attribute to the model with the lowest mean validation loss across
         all folds.
 
         Note: Inner models (presets) are 5-model bootstraps. The final (refit) model will be a self.n_model bootstrap.
 
         Args:
             data: MODData object contain training and validation samples.
             presets: A list of dictionaries containing custom presets.
@@ -272,16 +281,14 @@
             )
 
         if fast and len(presets) >= 2:
             presets = presets[:2]
             for k, _ in enumerate(presets):
                 presets[k]["epochs"] = 5
 
-        val_losses = 1e20 * np.ones((len(presets),))
-
         num_nested_folds = 5
         if nested:
             num_nested_folds = nested
         if num_nested_folds <= 1:
             num_nested_folds = 5
 
         # create tasks
@@ -413,25 +420,38 @@
         return models, val_losses, best_learning_curve, learning_curves, best_preset
 
     def _make_picklable(self):
         """
         transforms inner keras model to jsons so that the MODNet object becomes picklable.
         """
 
-        for m in self.model:
+        for m in self.models:
             m._make_picklable()
 
     def _restore_model(self):
         """
         restore inner keras model after running make_picklable
         """
 
-        for m in self.model:
+        for m in self.models:
             m._restore_model()
 
+    def _get_param_names(self):
+        possible_params = [
+            "n_models",
+            "bootstrap",
+            "models",
+        ]
+        return possible_params
+
+    @property
+    def model(self) -> List[MODNetModel]:
+        """Returns the inner MODNet models. For Backward compatability only."""
+        return self.models
+
 
 def _validate_ensemble_model(
     train_data=None,
     val_data=None,
     targets=None,
     weights=None,
     n_models=5,
@@ -441,14 +461,15 @@
     lr=0.1,
     batch_size=64,
     epochs=100,
     loss="mse",
     act="relu",
     out_act="linear",
     xscale="minmax",
+    impute_missing=-1,
     callbacks=[],
     preset_id=None,
     fold_id=None,
     verbose=0,
 ):
 
     model = EnsembleMODNetModel(
@@ -465,14 +486,15 @@
     model.fit(
         train_data,
         learning_rate=lr,
         epochs=epochs,
         batch_size=batch_size,
         loss=loss,
         xscale=xscale,
+        impute_missing=impute_missing,
         callbacks=callbacks,
         verbose=verbose,
         val_fraction=0,
         val_data=val_data,
     )
 
     learning_curves = [m.history["val_loss"] for m in model.model]
```

### Comparing `modnet-0.2.1/modnet/models/vanilla.py` & `modnet-0.3.0/modnet/models/vanilla.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """This submodule defines the "vanilla" `MODNetModel`, i.e. a single
 model with deterministic weights and outputs.
 
 """
+from collections import defaultdict
+from typing import List, Tuple, Dict, Optional, Callable, Any, Union
 
-from typing import List, Tuple, Dict, Optional, Callable, Any
 from pathlib import Path
 import multiprocessing
 
 import pandas as pd
 import numpy as np
+import warnings
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import mean_absolute_error, roc_auc_score
+from sklearn.impute import SimpleImputer
+from sklearn.pipeline import Pipeline
 import tensorflow as tf
 
 from modnet.preprocessing import MODData
 from modnet.utils import LOG
 from modnet import __version__
 
 import tqdm
@@ -83,15 +87,19 @@
         self.weights = weights
         self.num_classes = num_classes
         self.multi_label = multi_label
         self.num_neurons = num_neurons
         self.act = act
         self.out_act = out_act
 
+        self.xscale = None
         self._scaler = None
+        self._imputer = None
+        self.impute_missing = None
+        self._scale_impute = None
         self.optimal_descriptors = None
         self.target_names = None
         self.targets = targets
         self.model = None
 
         f_temp = [x for subl in targets for x in subl]
         self.targets_flatten = [x for subl in f_temp for x in subl]
@@ -203,44 +211,60 @@
                     final_out.append(out)
 
         return tf.keras.models.Model(inputs=f_input, outputs=final_out)
 
     def fit(
         self,
         training_data: MODData,
+        custom_data: Optional[np.ndarray] = None,
         val_fraction: float = 0.0,
         val_key: Optional[str] = None,
         val_data: Optional[MODData] = None,
         lr: float = 0.001,
         epochs: int = 200,
         batch_size: int = 128,
         xscale: Optional[str] = "minmax",
+        impute_missing: Optional[Union[float, str]] = 0,
+        xscale_before_impute: bool = True,
         metrics: List[str] = ["mae"],
         callbacks: List[Callable] = None,
         verbose: int = 0,
-        loss: str = "mse",
+        loss: str = None,
         **fit_params,
     ) -> None:
         """Train the model on the passed training `MODData` object.
 
         Parameters:
             training_data: A `MODData` that has been featurized and
                 feature selected. The first `self.n_feat` entries in
                 `training_data.get_optimal_descriptors()` will be used
                 for training.
+            custom_data (np.ndarray): Optional array of shape (n_sampels, n_custom_props) that will be appended to the targets (columns wise).
+                This can be useful for defining custom loss functions.
             val_fraction: The fraction of the training data to use as a
                 validation set for tracking model performance during
                 training.
             val_key: The target name to track on the validation set
                 during training, if performing multi-target learning.
             lr: The learning rate.
             epochs: The maximum number of epochs to train for.
             batch_size: The batch size to use for training.
             xscale: The feature scaler to use, either `None`,
                 `'minmax'` or `'standard'`.
+            impute_missing: Determines how the NaN features are treated.
+                If str, defines the strategy used in the scikit-learn SimpleImputer,
+                e.g., "mean" sets the NaNs to the mean of their feature column.
+                If a float is provided, and if xscale_before_impute is False, this
+                float is used to replace NaNs in the original dataset.
+                If a float is provided but xscale_before_impute is True, the float
+                is not used and standard values are used.
+                If you want to do something more sophisticated, make your own
+                modifications to MODData.df_featurized before fitting the model.
+            xscale_before_impute: whether to first scale the input and then impute values, or
+                first impute values and then scale the inputs.
             metrics: A list of tf.keras metrics to pass to `compile(...)`.
             loss: The built-in tf.keras loss to pass to `compile(...)`.
             fit_params: Any additional parameters to pass to `fit(...)`,
                 these will be overwritten by the explicit keyword
                 arguments above.
 
         """
@@ -248,14 +272,15 @@
         if self.n_feat > len(training_data.get_optimal_descriptors()):
             raise RuntimeError(
                 "The model requires more features than computed in data. "
                 f"Please reduce n_feat below or equal to {len(training_data.get_optimal_descriptors())}"
             )
 
         self.xscale = xscale
+        self.impute_missing = impute_missing
         self.target_names = list(self.weights.keys())
         self.optimal_descriptors = training_data.get_optimal_descriptors()
 
         x = training_data.get_featurized_df()[
             self.optimal_descriptors[: self.n_feat]
         ].values
 
@@ -268,49 +293,90 @@
             self.targets_flatten = list(training_data.df_targets.columns)
 
         y = []
         for targ in self.targets_flatten:
             if self.num_classes[targ] >= 2:  # Classification
                 if self.multi_label:
                     y_inner = np.stack(training_data.df_targets[targ].values)
-                    loss = "binary_crossentropy"
+                    if loss is None:
+                        loss = "binary_crossentropy"
                 else:
                     y_inner = tf.keras.utils.to_categorical(
                         training_data.df_targets[targ].values,
                         num_classes=self.num_classes[targ],
                     )
-                    loss = "categorical_crossentropy"
+                    if loss is None:
+                        loss = "categorical_crossentropy"
             else:
                 y_inner = training_data.df_targets[targ].values.astype(
                     np.float64, copy=False
                 )
+            if custom_data is not None:
+                val_data = None
+                val_fraction = 0
+                metrics = []
+                y_inner = np.hstack(
+                    (
+                        np.reshape(y_inner, (len(y_inner), -1)),
+                        custom_data.reshape((len(custom_data), -1)),
+                    )
+                )
             y.append(y_inner)
 
-        # Scale the input features:
+        # Define the scaler
         if self.xscale == "minmax":
             self._scaler = MinMaxScaler(feature_range=(-0.5, 0.5))
 
         elif self.xscale == "standard":
             self._scaler = StandardScaler()
 
-        x = self._scaler.fit_transform(x)
-        x = np.nan_to_num(x, nan=-1)
+        # Define the imputer
+        if isinstance(impute_missing, str):
+            self._imputer = SimpleImputer(
+                missing_values=np.nan, strategy=impute_missing
+            )
+        else:
+            if self.xscale == "minmax":
+                impute_missing = -1 if xscale_before_impute else impute_missing
+            elif self.xscale == "standard":
+                impute_missing = (
+                    10 * np.max(np.nan_to_num(StandardScaler().fit_transform(x)))
+                    if xscale_before_impute
+                    else impute_missing
+                )
+            self.impute_missing = impute_missing
+
+            self._imputer = SimpleImputer(
+                missing_values=np.nan, strategy="constant", fill_value=impute_missing
+            )
+
+        # Scale and impute input features in the desired order
+        if xscale_before_impute:
+            self._scale_impute = Pipeline(
+                [("scaler", self._scaler), ("imputer", self._imputer)]
+            )
+        else:
+            self._scale_impute = Pipeline(
+                [("imputer", self._imputer), ("scaler", self._scaler)]
+            )
+
+        x = self._scale_impute.fit_transform(x)
 
         if val_data is not None:
             val_x = val_data.get_featurized_df()[
                 self.optimal_descriptors[: self.n_feat]
             ].values
-            val_x = self._scaler.transform(val_x)
-            val_x = np.nan_to_num(val_x, nan=-1)
+            val_x = self._scale_impute.transform(val_x)
             val_y = []
             for targ in self.targets_flatten:
                 if self.num_classes[targ] >= 2:  # Classification
                     if self.multi_label:
                         y_inner = np.stack(val_data.df_targets[targ].values)
-                        loss = "binary_crossentropy"
+                        if loss is None:
+                            loss = "binary_crossentropy"
                     else:
                         y_inner = tf.keras.utils.to_categorical(
                             val_data.df_targets[targ].values,
                             num_classes=self.num_classes[targ],
                         )
                 else:
                     y_inner = val_data.df_targets[targ].values.astype(
@@ -348,25 +414,29 @@
                 )
 
             if callbacks is None:
                 callbacks = [print_callback]
             else:
                 callbacks.append(print_callback)
 
-        fit_params = {
+        fit_params_kw = {
             "x": x,
             "y": y,
             "epochs": epochs,
             "batch_size": batch_size,
             "verbose": 0,
             "validation_split": val_fraction,
             "validation_data": validation_data,
             "callbacks": callbacks,
         }
 
+        fit_params.update(fit_params_kw)
+
+        if loss is None:
+            loss = "mse"
         self.model.compile(
             loss=loss,
             optimizer=tf.keras.optimizers.legacy.Adam(learning_rate=lr),
             metrics=metrics,
             loss_weights=self.weights,
         )
         history = self.model.fit(**fit_params)
@@ -380,14 +450,15 @@
         verbose: int = 0,
         classification: bool = False,
         refit: bool = True,
         fast: bool = False,
         nested: int = 5,
         callbacks: List[Any] = None,
         n_jobs=None,
+        **fit_params,
     ) -> Tuple[
         List[List[Any]],
         np.ndarray,
         Optional[List[float]],
         List[List[float]],
         Dict[str, Any],
     ]:
@@ -572,19 +643,22 @@
                 val_fraction=0,
                 lr=best_preset["lr"],
                 epochs=best_preset["epochs"],
                 batch_size=best_preset["batch_size"],
                 loss=best_preset["loss"],
                 callbacks=callbacks,
                 verbose=verbose,
+                **fit_params,
             )
         else:
             self.n_feat = best_model.n_feat
             self.model = best_model.model
             self._scaler = best_model._scaler
+            self._imputer = best_model._imputer
+            self._scale_impute = best_model._scale_impute
 
         os.environ["TF_CPP_MIN_LOG_LEVEL"] = "0"  # reset
 
         return models, val_losses, best_learning_curve, learning_curves, best_preset
 
     def predict(self, test_data: MODData, return_prob=False) -> pd.DataFrame:
         """Predict the target values for the passed MODData.
@@ -599,25 +673,21 @@
             A `pandas.DataFrame` containing the predicted values of the targets.
 
 
         """
         # prevents Nan predictions if some features are inf
         x = (
             test_data.get_featurized_df()
-            .replace([np.inf, -np.inf, np.nan], 0)[
-                self.optimal_descriptors[: self.n_feat]
-            ]
+            .replace([np.inf, -np.inf], np.nan)[self.optimal_descriptors[: self.n_feat]]
             .values
         )
 
-        # Scale the input features:
-        x = np.nan_to_num(x)
-        if self._scaler is not None:
-            x = self._scaler.transform(x)
-            x = np.nan_to_num(x, nan=-1)
+        # Scale and impute input features:
+        if self._scale_impute is not None:
+            x = self._scale_impute.transform(x)
 
         p = np.array(self.model.predict(x))
 
         if len(p.shape) == 2:
             p = np.array([p])
 
         # post-process based on training data
@@ -665,25 +735,21 @@
 
         Returns:
             Score defined hereabove.
         """
         # prevents Nan predictions if some features are inf
         x = (
             test_data.get_featurized_df()
-            .replace([np.inf, -np.inf, np.nan], 0)[
-                self.optimal_descriptors[: self.n_feat]
-            ]
+            .replace([np.inf, -np.inf], np.nan)[self.optimal_descriptors[: self.n_feat]]
             .values
         )
 
-        # Scale the input features:
-        x = np.nan_to_num(x)
-        if self._scaler is not None:
-            x = self._scaler.transform(x)
-            x = np.nan_to_num(x, nan=-1)
+        # Scale and impute input features:
+        if self._scale_impute is not None:
+            x = self._scale_impute.transform(x)
 
         y_pred = np.array(self.model.predict(x))
         if len(y_pred.shape) == 2:
             y_pred = np.array([y_pred])
         score = []
         for i, targ in enumerate(self.targets_flatten):
             if self.num_classes[targ] >= 2:  # Classification
@@ -790,14 +856,117 @@
             return pickled_data
 
         raise ValueError(
             f"File {filename} did not contain compatible data to create a MODNetModel object, "
             f"instead found {pickled_data.__class__.__name__}."
         )
 
+    def _get_param_names(self):
+        possible_params = [
+            "targets",
+            "weights",
+            "num_neurons",
+            "num_classes",
+            "multi_label",
+            "n_feat",
+            "act",
+            "out_act",
+        ]
+        return possible_params
+
+    def get_params(self, deep=True):
+        """
+        Get parameters for this estimator.
+        Taken from sklearn.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            If True, will return the parameters for this estimator and
+            contained subobjects that are estimators.
+
+        Returns
+        -------
+        params : dict
+            Parameter names mapped to their values.
+        """
+        out = dict()
+
+        for key in self._get_param_names():
+            value = getattr(self, key)
+            if deep and hasattr(value, "get_params") and not isinstance(value, type):
+                deep_items = value.get_params().items()
+                out.update((key + "__" + k, val) for k, val in deep_items)
+            out[key] = value
+        return out
+
+    def set_params(self, **params):
+        """Set the parameters of this estimator.
+
+        The method works on simple estimators as well as on nested objects
+        (such as :class:`~sklearn.pipeline.Pipeline`). The latter have
+        parameters of the form ``<component>__<parameter>`` so that it's
+        possible to update each component of a nested object.
+        Taken from sklearn.
+
+        Parameters
+        ----------
+        **params : dict
+            Estimator parameters.
+
+        Returns
+        -------
+        self : estimator instance
+            Estimator instance.
+        """
+        if not params:
+            # Simple optimization to gain speed (inspect is slow)
+            return self
+        valid_params = self.get_params(deep=True)
+
+        nested_params = defaultdict(dict)  # grouped by prefix
+        for key, value in params.items():
+            key, delim, sub_key = key.partition("__")
+            if key not in valid_params:
+                local_valid_params = self._get_param_names()
+                raise ValueError(
+                    f"Invalid parameter {key!r} for estimator {self}. "
+                    f"Valid parameters are: {local_valid_params!r}."
+                )
+
+            if delim:
+                nested_params[key][sub_key] = value
+            else:
+                setattr(self, key, value)
+                valid_params[key] = value
+
+        for key, sub_params in nested_params.items():
+            # TODO(1.4): remove specific handling of "base_estimator".
+            # The "base_estimator" key is special. It was deprecated and
+            # renamed to "estimator" for several estimators. This means we
+            # need to translate it here and set sub-parameters on "estimator",
+            # but only if the user did not explicitly set a value for
+            # "base_estimator".
+            if (
+                key == "base_estimator"
+                and valid_params[key] == "deprecated"
+                and self.__module__.startswith("sklearn.")
+            ):
+                warnings.warn(
+                    f"Parameter 'base_estimator' of {self.__class__.__name__} is"
+                    " deprecated in favor of 'estimator'. See"
+                    f" {self.__class__.__name__}'s docstring for more details.",
+                    FutureWarning,
+                    stacklevel=2,
+                )
+                key = "estimator"
+            valid_params[key].set_params(**sub_params)
+
+        return self
+
 
 def validate_model(
     train_data=None,
     val_data=None,
     targets=None,
     weights=None,
     num_classes=None,
```

### Comparing `modnet-0.2.1/modnet/preprocessing.py` & `modnet-0.3.0/modnet/preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from sklearn.preprocessing import MinMaxScaler
 
 import pandas as pd
 import numpy as np
 import tqdm
 from multiprocessing import Pool
 
-from modnet.featurizers import MODFeaturizer
+from modnet.featurizers import MODFeaturizer, clean_df
 from modnet import __version__
 from modnet.utils import LOG
 
 
 DATABASE = pd.DataFrame([])
 
 
@@ -66,14 +66,15 @@
 
 
 def nmi_target(
     df_feat: pd.DataFrame,
     df_target: pd.DataFrame,
     task_type: str = "regression",
     drop_constant_features: bool = True,
+    drop_duplicate_features: bool = True,
     **kwargs,
 ) -> pd.DataFrame:
     """
     Computes the Normalized Mutual Information (NMI) between a list of
     input features and a target variable.
 
     Args:
@@ -81,14 +82,16 @@
             which the NMI with the target variable is to be computed.
         df_target (pandas.DataFrame): Dataframe containing the target variable.
             This DataFrame should contain only one column and have the same
             size as `df_feat`.
         task_type (integer): 0 for regression, 1 for classification
         drop_constant_features (bool): If True, the features that are constant
             across the entire data set will be dropped.
+        drop_duplicate_features (bool): If True, the features that have exactly the same
+            values across the entire data set will be dropped.
         **kwargs: Keyword arguments to be passed down to the
             :py:func:`mutual_info_regression` function from scikit-learn. This
             can be useful e.g. for testing purposes.
 
     Returns:
         pandas.DataFrame: Dataframe containing the NMI between each of
             the input features and the target variable.
@@ -111,19 +114,21 @@
 
     if len(df_feat) != len(df_target):
         raise ValueError(
             "The input features DataFrame and the target variable DataFrame "
             "should contain the same number of data points."
         )
 
+    # Drop features that are duplicates across the entire data set
+    if drop_duplicate_features:
+        df_feat = df_feat.T.drop_duplicates().T
+
     # Drop features which have the same value for the entire data set
     if drop_constant_features:
-        frange = df_feat.max(axis=0) - df_feat.min(axis=0)
-        to_drop = frange[frange == 0].index
-        df_feat = df_feat.drop(to_drop, axis=1)
+        df_feat = df_feat.loc[:, (df_feat != df_feat.iloc[0]).any()]
 
     # preprocess the input matrix
     if (
         df_feat.isna().any().any()
     ):  # only preprocess if nans are present to preserve past behaviour
         scaler = MinMaxScaler(feature_range=(-0.5, 0.5))
         x = df_feat.values
@@ -658,15 +663,18 @@
         if self.featurizer is not None:
             LOG.info(f"Loaded {self.featurizer.__class__.__name__} featurizer.")
 
         if target_names is not None:
             if np.shape(targets)[-1] != len(target_names):
                 raise ValueError("Target names must be supplied for every target.")
         elif targets is not None:
-            target_names = ["prop" + str(i) for i in range(len(targets))]
+            if len(np.shape(targets)) == 1:
+                target_names = ["prop0"]
+            else:
+                target_names = ["prop" + str(i) for i in range(np.shape(targets)[1])]
 
         if structure_ids is not None:
             # for backwards compat, always store the *passed* list of
             # IDs, so they can be used when loading from a database file
             # check ids are unique
             if len(set(structure_ids)) != len(structure_ids):
                 raise ValueError(
@@ -765,26 +773,29 @@
             else:
                 df_final = df_done
 
         # otherwise, no structures were loaded, so we need to compute all
         else:
             df_final = self.featurizer.featurize(self.df_structure)
 
-        df_final = df_final.replace([np.inf, -np.inf, np.nan], 0)
+        # replace infinite values by nan that are handled during the fit
+        df_final = clean_df(df_final)
 
         self.df_featurized = df_final
         LOG.info("Data has successfully been featurized!")
 
     def feature_selection(
         self,
         n: int = 1500,
         cross_nmi: Optional[pd.DataFrame] = None,
         use_precomputed_cross_nmi: bool = False,
         n_samples=6000,
+        drop_thr: float = 0.2,
         n_jobs: int = None,
+        ignore_names: Optional[List] = [],
     ):
         """Compute the mutual information between features and targets,
         then apply relevance-redundancy rankings to choose the top `n`
         features.
 
         Sets the `self.optimal_features` attribute to a list of feature
         names.
@@ -793,32 +804,38 @@
             n: number of desired features.
             cross_nmi: specify the cross NMI between features as a
                 dataframe.
             use_precomputed_cross_nmi: Whether or not to use the cross NMI
                 that was computed on Materials Project features, instead of
                 precomputing.
             n_jobs: max. number of processes to use when calculating cross NMI.
+            ignore_names (List): Optional list of property names to ignore during feature selection.
+                Feature selection will be performed w.r.t. all properties except the ones in ignore_names.
 
         """
         if getattr(self, "df_featurized", None) is None:
             raise RuntimeError(
-                "Mutual information feature selection requiresd featurized data, please call `.featurize()`"
+                "Mutual information feature selection requires featurized data, please call `.featurize()`"
             )
         if getattr(self, "df_targets", None) is None:
             raise RuntimeError(
                 "Mutual information feature selection requires target properties"
             )
 
+        for na in ignore_names:
+            if na not in self.names:
+                raise RuntimeError(
+                    f"Names provided in ignore_names should be part of {self.names}. {na} was not found."
+                )
+
         ranked_lists = []
         optimal_features_by_target = {}
 
         if cross_nmi is not None:
             self.cross_nmi = cross_nmi
-        elif getattr(self, "cross_nmi", None) is None:
-            self.cross_nmi = None
 
         # Loading mutual information between features
         if use_precomputed_cross_nmi:
             LOG.info("Loading cross NMI from 'Features_cross' file.")
             from modnet.ext_data import load_ext_dataset
 
             cnmi_path = load_ext_dataset("MP_2018.6_CROSS_NMI", "cross_nmi")
@@ -833,24 +850,25 @@
 
         if self.cross_nmi is None:
             if len(self.df_featurized) > n_samples:
                 df = self.df_featurized.sample(n=n_samples, random_state=12)
             else:
                 df = self.df_featurized.copy()
             self.cross_nmi, self.feature_entropy = get_cross_nmi(
-                df, return_entropy=True, n_jobs=n_jobs
+                df, return_entropy=True, drop_thr=drop_thr, n_jobs=n_jobs
             )
 
         if self.cross_nmi.isna().sum().sum() > 0:
-            raise RuntimeError(
-                "Cross NMI (`moddata.cross_nmi`) contains NaN values, consider setting them to zero."
-            )
+            raise RuntimeError("Cross NMI (`moddata.cross_nmi`) contains NaN values.")
 
-        for i, name in enumerate(self.names):
-            LOG.info(f"Starting target {i + 1}/{len(self.names)}: {self.names[i]} ...")
+        selection_names = list(set(self.names).difference(set(ignore_names)))
+        for i, name in enumerate(selection_names):
+            LOG.info(
+                f"Starting target {i + 1}/{len(selection_names)}: {selection_names[i]} ..."
+            )
 
             # Computing mutual information with target
             LOG.info("Computing mutual information between features and target...")
             if getattr(self, "num_classes", None) and self.num_classes[name] >= 2:
                 task_type = "classification"
             else:
                 task_type = "regression"
```

### Comparing `modnet-0.2.1/modnet/sklearn.py` & `modnet-0.3.0/modnet/sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/tests/conftest.py` & `modnet-0.3.0/modnet/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/tests/test_benchmark.py` & `modnet-0.3.0/modnet/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/tests/test_ext_data.py` & `modnet-0.3.0/modnet/tests/test_ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/tests/test_hyper_opt.py` & `modnet-0.3.0/modnet/tests/test_hyper_opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,8 @@
         refit=1,
         fast=True,
     )
 
     from modnet.models import EnsembleMODNetModel
 
     assert type(model) is EnsembleMODNetModel
-    assert len(model.model) == 1
+    assert len(model.models) == 1
```

### Comparing `modnet-0.2.1/modnet/tests/test_model.py` & `modnet-0.3.0/modnet/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/tests/test_preprocessing.py` & `modnet-0.3.0/modnet/tests/test_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,25 @@
             error_cols.add(col)
 
     # Unfortuanately there are some columns we cannot control, e.g.,
     # default symmetry tolerance changing in pymatgen leading to a
     # different number of symm ops being detected.
 
     # We need a mechanism to allow these discrepancies through in certain cases:
-    allowed_bad_columns = ["GlobalSymmetryFeatures|n_symmetry_ops"]
+    allowed_bad_columns = [
+        "GlobalSymmetryFeatures|n_symmetry_ops",
+        "GlobalSymmetryFeatures|crystal_system",
+        "YangSolidSolution|Yang delta",
+        "Miedema|Miedema_deltaH_inter",
+        "AtomicPackingEfficiency|mean simul. packing efficiency",
+        "Miedema|Miedema_deltaH_amor",
+        "AtomicPackingEfficiency|mean abs simul. packing efficiency",
+        "Miedema|Miedema_deltaH_ss_min",
+    ]
+
     for col in allowed_bad_columns:
         if col in error_cols:
             error_cols.remove(col)
 
     assert not error_cols, f"Some columns contained errors: {error_cols}"
```

### Comparing `modnet-0.2.1/modnet/tests/test_sklearn.py` & `modnet-0.3.0/modnet/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet/utils.py` & `modnet-0.3.0/modnet/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.2.1/modnet.egg-info/PKG-INFO` & `modnet-0.3.0/modnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.2.1
+Version: 0.3.0
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
 Description: # MODNet: Material Optimal Descriptor Network
         
         [![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
         
+        <p align="center">
+            <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
+            <br>
+        </p>
+        
         <a name="introduction"></a>
         ## Introduction
         This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
         It is a supervised machine learning framework for **learning material properties** from
         either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
         and can be used for learning *multiple* properties together by using **joint learning**.
```

### Comparing `modnet-0.2.1/modnet.egg-info/SOURCES.txt` & `modnet-0.3.0/modnet.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 modnet/data/Features_cross
 modnet/featurizers/__init__.py
 modnet/featurizers/featurizers.py
 modnet/featurizers/utils.py
 modnet/featurizers/presets/__init__.py
 modnet/featurizers/presets/debreuck_2020.py
 modnet/featurizers/presets/matminer_2023.py
+modnet/featurizers/presets/matminer_all_2023.py
 modnet/hyper_opt/__init__.py
 modnet/hyper_opt/fit_genetic.py
 modnet/matbench/__init__.py
 modnet/matbench/benchmark.py
 modnet/model_presets/__init__.py
 modnet/model_presets/presets.py
 modnet/models/__init__.py
```

### Comparing `modnet-0.2.1/setup.py` & `modnet-0.3.0/setup.py`

 * *Files identical despite different names*

