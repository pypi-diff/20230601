# Comparing `tmp/interpret-core-0.4.1.tar.gz` & `tmp/interpret-core-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpret-core-0.4.1.tar", last modified: Tue May 16 23:05:36 2023, max compression
+gzip compressed data, was "interpret-core-0.4.2.tar", last modified: Thu Jun  1 03:28:15 2023, max compression
```

## Comparing `interpret-core-0.4.1.tar` & `interpret-core-0.4.2.tar`

### file list

```diff
@@ -1,343 +1,343 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.833345 interpret-core-0.4.1/
--rw-r--r--   0 vsts      (1001) docker     (122)      275 2023-05-16 23:00:07.000000 interpret-core-0.4.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-05-16 23:05:36.833345 interpret-core-0.4.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.713344 interpret-core-0.4.1/interpret/
--rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.713344 interpret-core-0.4.1/interpret/api/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2543 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/api/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6294 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/api/templates.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.717344 interpret-core-0.4.1/interpret/blackbox/
--rw-r--r--   0 vsts      (1001) docker     (122)      381 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6145 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_lime.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8611 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_partialdependence.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10275 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_permutationimportance.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10783 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_sensitivity.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/blackbox/_shap.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.721344 interpret-core-0.4.1/interpret/data/
--rw-r--r--   0 vsts      (1001) docker     (122)      158 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15905 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/data/_response.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6307 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/develop.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.721344 interpret-core-0.4.1/interpret/ext/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.721344 interpret-core-0.4.1/interpret/ext/blackbox/
--rw-r--r--   0 vsts      (1001) docker     (122)      366 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/blackbox/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.721344 interpret-core-0.4.1/interpret/ext/data/
--rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3314 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/extension.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2955 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/extension_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/ext/glassbox/
--rw-r--r--   0 vsts      (1001) docker     (122)      366 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/glassbox/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/ext/greybox/
--rw-r--r--   0 vsts      (1001) docker     (122)      362 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/greybox/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/ext/perf/
--rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/perf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/ext/provider/
--rw-r--r--   0 vsts      (1001) docker     (122)      340 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/ext/provider/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.725344 interpret-core-0.4.1/interpret/glassbox/
--rw-r--r--   0 vsts      (1001) docker     (122)      500 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20235 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_decisiontree.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.729344 interpret-core-0.4.1/interpret/glassbox/_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9550 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_bin.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6500 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_boost.py
--rw-r--r--   0 vsts      (1001) docker     (122)   139474 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_ebm.py
--rw-r--r--   0 vsts      (1001) docker     (122)    33662 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_merge_ebms.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4461 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_multiclass.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.729344 interpret-core-0.4.1/interpret/glassbox/_ebm/_research/
--rw-r--r--   0 vsts      (1001) docker     (122)      537 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_research/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10237 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_research/_group_importance.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4136 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_research/_purify.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5423 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_tensor.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17903 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_ebm/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17093 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14262 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/glassbox/_skoperules.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.733344 interpret-core-0.4.1/interpret/greybox/
--rw-r--r--   0 vsts      (1001) docker     (122)      202 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/greybox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/greybox/_shaptree.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5420 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/greybox/_treeinterpreter.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.737344 interpret-core-0.4.1/interpret/lib/
--rw-r--r--   0 vsts      (1001) docker     (122)  4182080 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret/lib/interpret-inline.js
--rw-r--r--   0 vsts      (1001) docker     (122)     2580 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret/lib/interpret-inline.js.LICENSE.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.741344 interpret-core-0.4.1/interpret/perf/
--rw-r--r--   0 vsts      (1001) docker     (122)      192 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/perf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10362 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/perf/_curve.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/perf/_regression.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.741344 interpret-core-0.4.1/interpret/privacy/
--rw-r--r--   0 vsts      (1001) docker     (122)      269 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/privacy/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.741344 interpret-core-0.4.1/interpret/provider/
--rw-r--r--   0 vsts      (1001) docker     (122)      316 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      777 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/provider/_compute.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4704 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/provider/_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8375 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/provider/_visualize.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.745344 interpret-core-0.4.1/interpret/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)     2900 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_SPOTgreedy.py
--rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14758 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_clean_simple.py
--rw-r--r--   0 vsts      (1001) docker     (122)    82828 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_clean_x.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4613 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_compressed_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6217 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_explanation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2369 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_histogram.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1412 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_link.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9852 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_measure_interactions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    61653 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_native.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23690 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_preprocessor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5556 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_privacy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1623 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_rank_interactions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2611 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_seed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3790 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_shap_common.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3274 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_unify_data.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5003 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/utils/_unify_predict.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.745344 interpret-core-0.4.1/interpret/visual/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8094 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/_inline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7582 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/_interactive.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32140 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/_udash.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.745344 interpret-core-0.4.1/interpret/visual/assets/
--rw-r--r--   0 vsts      (1001) docker     (122)    15406 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/assets/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (122)    15857 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/assets/udash.css
--rw-r--r--   0 vsts      (1001) docker     (122)      599 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/assets/udash.js
--rw-r--r--   0 vsts      (1001) docker     (122)    13340 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/dashboard.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26837 2023-05-16 23:00:07.000000 interpret-core-0.4.1/interpret/visual/plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.753344 interpret-core-0.4.1/interpret_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    11667 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      717 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-05-16 23:05:36.000000 interpret-core-0.4.1/interpret_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-16 23:05:36.833345 interpret-core-0.4.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     8880 2023-05-16 23:00:07.000000 interpret-core-0.4.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.753344 interpret-core-0.4.1/symbolic/
--rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-05-16 23:00:15.000000 interpret-core-0.4.1/symbolic/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)    34327 2023-05-16 23:00:15.000000 interpret-core-0.4.1/symbolic/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1565 2023-05-16 23:00:15.000000 interpret-core-0.4.1/symbolic/build.bat
--rw-r--r--   0 vsts      (1001) docker     (122)    40976 2023-05-16 23:00:15.000000 interpret-core-0.4.1/symbolic/build.sh
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.705344 interpret-core-0.4.1/symbolic/shared/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.781345 interpret-core-0.4.1/symbolic/shared/libebm/
--rw-r--r--   0 vsts      (1001) docker     (122)    25251 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/ApplyTermUpdate.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    10588 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BinSumsBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    15618 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BinSumsInteraction.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    30951 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BoosterCore.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7155 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BoosterCore.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    19842 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BoosterShell.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     5691 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/BoosterShell.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     8866 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CODING_STYLE.md
--rw-r--r--   0 vsts      (1001) docker     (122)    18718 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CalcInteractionStrength.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)   179547 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CutQuantile.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    32876 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CutUniform.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    20952 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/CutWinsorized.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    27635 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DataSetBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3161 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DataSetBoosting.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    14037 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DataSetInteraction.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3075 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DataSetInteraction.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/DetermineLinkFunction.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    60544 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Discretize.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4162 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Feature.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    19457 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/GaussianDistribution.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    42347 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/GenerateTermUpdate.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    17492 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/IMPORTANT.md
--rw-r--r--   0 vsts      (1001) docker     (122)     4536 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InitializeGradientsAndHessians.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    10200 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InnerBag.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2783 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InnerBag.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    20298 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InteractionCore.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4133 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InteractionCore.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     9050 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InteractionShell.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/InteractionShell.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    35081 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/PartitionOneDimensionalBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    32143 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/PartitionRandomBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    42726 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/PartitionTwoDimensionalBoosting.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    25557 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/PartitionTwoDimensionalInteraction.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7387 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/RandomDeterministic.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    11402 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/RandomDeterministic.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4656 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/RandomNondeterministic.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4417 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/SplitPosition.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    36064 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Tensor.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13659 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Tensor.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    46171 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/TensorTotalsBuild.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    18160 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/TensorTotalsSum.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     1843 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Term.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4546 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Term.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4849 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/Transpose.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    10239 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/TreeNode.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.781345 interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/
--rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/bridge_c.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1371 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/zones.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.781345 interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/
--rw-r--r--   0 vsts      (1001) docker     (122)    13743 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/Bin.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     8442 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/GradientPair.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     8200 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/bridge_cpp.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.785344 interpret-core-0.4.1/symbolic/shared/libebm/common_c/
--rw-r--r--   0 vsts      (1001) docker     (122)     3037 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_c/common_c.c
--rw-r--r--   0 vsts      (1001) docker     (122)     8476 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_c/common_c.h
--rw-r--r--   0 vsts      (1001) docker     (122)     6580 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_c/logging.c
--rw-r--r--   0 vsts      (1001) docker     (122)    10001 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_c/logging.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.785344 interpret-core-0.4.1/symbolic/shared/libebm/common_cpp/
--rw-r--r--   0 vsts      (1001) docker     (122)    45433 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/common_cpp/common_cpp.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.789345 interpret-core-0.4.1/symbolic/shared/libebm/compute/
--rw-r--r--   0 vsts      (1001) docker     (122)      553 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Directory.Build.targets
--rw-r--r--   0 vsts      (1001) docker     (122)     6427 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Objective.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    35870 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Objective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     6723 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Registration.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13194 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/Registration.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    50721 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/approximate_math.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.793345 interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)      257 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/avx512_32.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13706 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)      477 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj.filters
--rw-r--r--   0 vsts      (1001) docker     (122)     4386 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/compute.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    61597 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/compute_stats.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.793345 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)      254 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_32.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7447 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_64.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13427 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)      593 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj.filters
--rw-r--r--   0 vsts      (1001) docker     (122)     8950 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/sse2_32.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/sse2_64.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.793345 interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)    11435 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_32.cu
--rw-r--r--   0 vsts      (1001) docker     (122)    14658 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)      505 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj.filters
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.797345 interpret-core-0.4.1/symbolic/shared/libebm/compute/metrics/
--rw-r--r--   0 vsts      (1001) docker     (122)      177 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/metrics/AucMetric.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.797345 interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)      630 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_32.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    13332 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)      478 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj.filters
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.801345 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/
--rw-r--r--   0 vsts      (1001) docker     (122)      432 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/CrossEntropyBinaryObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3630 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassMultitaskObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4464 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/ExampleRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3033 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/GammaDevianceRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)      770 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossBinaryMultitaskObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     7535 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossBinaryObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     9437 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossMulticlassObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4596 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/PoissonDevianceRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4226 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/PseudoHuberRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3409 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseLogLinkRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseRegressionMultitaskObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     9112 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4842 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/TweedieDevianceRegressionObjective.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     3245 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/objective_registrations.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)      267 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/precompiled_header_cpp.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2301 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/registration_exceptions.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.801345 interpret-core-0.4.1/symbolic/shared/libebm/compute/special/
--rw-r--r--   0 vsts      (1001) docker     (122)      164 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/special/precompiled_header_cpp.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2366 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_c_functions.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     1068 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_c_functions.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_cpp_functions.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2800 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/compute_accessors.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    99988 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/dataset_shared.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2242 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/dataset_shared.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    20943 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/debug_ebm.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     8264 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/ebm_internal.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    41443 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/ebm_stats.hpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.801345 interpret-core-0.4.1/symbolic/shared/libebm/inc/
--rw-r--r--   0 vsts      (1001) docker     (122)    20435 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/inc/libebm.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3650 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/include_ordering.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    13166 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/interpret.sln
--rw-r--r--   0 vsts      (1001) docker     (122)    77375 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/interpretable_numerics.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    24095 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)     5242 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj.filters
--rw-r--r--   0 vsts      (1001) docker     (122)      994 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/libebm_exports.def
--rw-r--r--   0 vsts      (1001) docker     (122)     1257 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/libebm_exports.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/precompiled_header_cpp.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)     6007 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/random.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    26424 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/sampling.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.801345 interpret-core-0.4.1/symbolic/shared/libebm/special/
--rw-r--r--   0 vsts      (1001) docker     (122)     2874 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/special/linux_wrap_functions.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      164 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/special/precompiled_header_cpp.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      790 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/special/windows_DllMain.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.809345 interpret-core-0.4.1/symbolic/shared/libebm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)    46248 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/CutQuantileTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    12964 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/CutUniformTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    24882 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/CutWinsorizedTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/DiscretizeTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     6935 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/RandomStreamTest.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    11983 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/SuggestGraphBoundsTest.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     6816 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/bit_packing_extremes.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    68182 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/boosting_unusual_inputs.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    17110 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/dataset_shared_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     2740 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/include_c.c
--rw-r--r--   0 vsts      (1001) docker     (122)    15959 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/interaction_unusual_inputs.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     1931 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.bat
--rw-r--r--   0 vsts      (1001) docker     (122)    41676 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)    14654 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    38501 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.sh
--rw-r--r--   0 vsts      (1001) docker     (122)    15718 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.vcxproj
--rw-r--r--   0 vsts      (1001) docker     (122)     1636 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.vcxproj.filters
--rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/precompiled_header_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      298 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/precompiled_header_test.hpp
--rw-r--r--   0 vsts      (1001) docker     (122)    12851 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/random_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)     4893 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/tests/rehydrate_booster.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      564 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/libebm/vs_python_setup.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.813345 interpret-core-0.4.1/symbolic/shared/vis/
--rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/.babelrc
--rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/.eslintrc.json
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (122)      238 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1472 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/package.json
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.813345 interpret-core-0.4.1/symbolic/shared/vis/src/
--rw-r--r--   0 vsts      (1001) docker     (122)     4433 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/src/index.js
--rw-r--r--   0 vsts      (1001) docker     (122)     1469 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/src/styles.scss
--rw-r--r--   0 vsts      (1001) docker     (122)      757 2023-05-16 23:00:07.000000 interpret-core-0.4.1/symbolic/shared/vis/webpack.config.js
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.817345 interpret-core-0.4.1/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.817345 interpret-core-0.4.1/tests/api/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1895 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/api/test_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.821345 interpret-core-0.4.1/tests/blackbox/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/blackbox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1435 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/blackbox/test_permutationimportance.py
--rw-r--r--   0 vsts      (1001) docker     (122)      477 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/blackbox/test_sensitivity.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.821345 interpret-core-0.4.1/tests/ext/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/ext/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2502 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/ext/test_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.821345 interpret-core-0.4.1/tests/glassbox/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.825345 interpret-core-0.4.1/tests/glassbox/ebm/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.825345 interpret-core-0.4.1/tests/glassbox/ebm/research/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/research/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8067 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/research/test_group_importance.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8414 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/research/test_purify.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4105 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_bin.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28189 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_ebm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5551 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_ebm_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5393 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_merge_ebms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      790 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/ebm/test_multiclass.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2055 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/test_decisiontree.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3499 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/glassbox/test_linear.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.825345 interpret-core-0.4.1/tests/greybox/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/greybox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1459 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/greybox/test_treeinterpreter.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.825345 interpret-core-0.4.1/tests/provider/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      470 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/provider/test_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2257 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/provider/test_providers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_develop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_example_notebooks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3215 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_explainers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2702 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_ext.py
--rw-r--r--   0 vsts      (1001) docker     (122)      691 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_extension_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1108 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_mli_interop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9489 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/test_selenium.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8241 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/tutils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.829345 interpret-core-0.4.1/tests/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1099 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_SPOTgreedy.py
--rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_clean_simple.py
--rw-r--r--   0 vsts      (1001) docker     (122)   113135 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_clean_x.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3041 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_compressed_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1453 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_explanation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8683 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_measure_interactions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2888 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/utils/test_native.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:36.833345 interpret-core-0.4.1/tests/visual/
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      369 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/test_dashboard.py
--rw-r--r--   0 vsts      (1001) docker     (122)      898 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/test_inline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/test_interactive.py
--rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-05-16 23:00:07.000000 interpret-core-0.4.1/tests/visual/test_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.774153 interpret-core-0.4.2/
+-rw-r--r--   0 vsts      (1001) docker     (122)      275 2023-06-01 03:23:28.000000 interpret-core-0.4.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-06-01 03:28:15.774153 interpret-core-0.4.2/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.710152 interpret-core-0.4.2/interpret/
+-rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.710152 interpret-core-0.4.2/interpret/api/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2543 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/api/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6294 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/api/templates.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/blackbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      381 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/blackbox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6145 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/blackbox/_lime.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8611 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/blackbox/_partialdependence.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10275 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/blackbox/_permutationimportance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10783 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/blackbox/_sensitivity.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/blackbox/_shap.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/data/
+-rw-r--r--   0 vsts      (1001) docker     (122)      158 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15905 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/data/_response.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6307 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/develop.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/ext/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/ext/blackbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      366 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/blackbox/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/ext/data/
+-rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3314 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/extension.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2955 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/extension_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/ext/glassbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      366 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/glassbox/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/ext/greybox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      362 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/greybox/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/ext/perf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/perf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/ext/provider/
+-rw-r--r--   0 vsts      (1001) docker     (122)      340 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/ext/provider/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.714152 interpret-core-0.4.2/interpret/glassbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      500 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20235 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_decisiontree.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.718152 interpret-core-0.4.2/interpret/glassbox/_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9550 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_bin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7004 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_boost.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   141941 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_ebm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    33635 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_merge_ebms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4461 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_multiclass.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.718152 interpret-core-0.4.2/interpret/glassbox/_ebm/_research/
+-rw-r--r--   0 vsts      (1001) docker     (122)      537 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_research/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10237 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_research/_group_importance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4136 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_research/_purify.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2908 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_tensor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17903 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_ebm/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17093 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14262 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/glassbox/_skoperules.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.718152 interpret-core-0.4.2/interpret/greybox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      202 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/greybox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/greybox/_shaptree.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5420 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/greybox/_treeinterpreter.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.726152 interpret-core-0.4.2/interpret/lib/
+-rw-r--r--   0 vsts      (1001) docker     (122)  4182747 2023-06-01 03:28:15.000000 interpret-core-0.4.2/interpret/lib/interpret-inline.js
+-rw-r--r--   0 vsts      (1001) docker     (122)     2580 2023-06-01 03:28:15.000000 interpret-core-0.4.2/interpret/lib/interpret-inline.js.LICENSE.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.726152 interpret-core-0.4.2/interpret/perf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      192 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/perf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10362 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/perf/_curve.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/perf/_regression.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.726152 interpret-core-0.4.2/interpret/privacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)      269 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/privacy/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.726152 interpret-core-0.4.2/interpret/provider/
+-rw-r--r--   0 vsts      (1001) docker     (122)      316 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      777 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/provider/_compute.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4704 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/provider/_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8375 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/provider/_visualize.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.730152 interpret-core-0.4.2/interpret/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2900 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_SPOTgreedy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14758 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_clean_simple.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    82828 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_clean_x.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4565 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_compressed_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6217 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_explanation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2369 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1412 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_link.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9938 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_measure_interactions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    60622 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_native.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24882 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_preprocessor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6169 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_privacy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1768 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_rank_interactions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2611 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_seed.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3790 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_shap_common.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3274 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_unify_data.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5003 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/utils/_unify_predict.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.730152 interpret-core-0.4.2/interpret/visual/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8094 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/_inline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7582 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/_interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32140 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/_udash.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.730152 interpret-core-0.4.2/interpret/visual/assets/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15406 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/assets/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (122)    15857 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/assets/udash.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      599 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/assets/udash.js
+-rw-r--r--   0 vsts      (1001) docker     (122)    13340 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/dashboard.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26837 2023-06-01 03:23:28.000000 interpret-core-0.4.2/interpret/visual/plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.734152 interpret-core-0.4.2/interpret_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-06-01 03:28:15.000000 interpret-core-0.4.2/interpret_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    11667 2023-06-01 03:28:15.000000 interpret-core-0.4.2/interpret_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-01 03:28:15.000000 interpret-core-0.4.2/interpret_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-06-01 03:28:15.000000 interpret-core-0.4.2/interpret_core.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      717 2023-06-01 03:28:15.000000 interpret-core-0.4.2/interpret_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-06-01 03:28:15.000000 interpret-core-0.4.2/interpret_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-06-01 03:28:15.774153 interpret-core-0.4.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     8880 2023-06-01 03:23:28.000000 interpret-core-0.4.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.734152 interpret-core-0.4.2/symbolic/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-06-01 03:23:34.000000 interpret-core-0.4.2/symbolic/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)    34669 2023-06-01 03:23:34.000000 interpret-core-0.4.2/symbolic/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1565 2023-06-01 03:23:34.000000 interpret-core-0.4.2/symbolic/build.bat
+-rw-r--r--   0 vsts      (1001) docker     (122)    40922 2023-06-01 03:23:34.000000 interpret-core-0.4.2/symbolic/build.sh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.710152 interpret-core-0.4.2/symbolic/shared/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.746152 interpret-core-0.4.2/symbolic/shared/libebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)    25237 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/ApplyTermUpdate.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    10588 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/BinSumsBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    15618 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/BinSumsInteraction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    31739 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/BoosterCore.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7155 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/BoosterCore.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    19919 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/BoosterShell.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5691 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/BoosterShell.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8866 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/CODING_STYLE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)    18709 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/CalcInteractionStrength.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)   180748 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/CutQuantile.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    32876 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/CutUniform.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    20952 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/CutWinsorized.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    27647 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/DataSetBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3161 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/DataSetBoosting.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14037 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/DataSetInteraction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3075 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/DataSetInteraction.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5709 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/DetermineLinkFunction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    60544 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/Discretize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4162 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/Feature.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    19457 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/GaussianDistribution.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    42362 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/GenerateTermUpdate.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    17492 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/IMPORTANT.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     4536 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/InitializeGradientsAndHessians.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    10200 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/InnerBag.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2783 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/InnerBag.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    20527 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/InteractionCore.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4133 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/InteractionCore.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9050 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/InteractionShell.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/InteractionShell.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    34955 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/PartitionOneDimensionalBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    32082 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/PartitionRandomBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    42786 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/PartitionTwoDimensionalBoosting.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    25557 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/PartitionTwoDimensionalInteraction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7387 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/RandomDeterministic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    11402 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/RandomDeterministic.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4656 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/RandomNondeterministic.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4417 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/SplitPosition.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    36017 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/Tensor.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13455 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/Tensor.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    46171 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/TensorTotalsBuild.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    18160 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/TensorTotalsSum.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1843 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/Term.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4682 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/Term.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7143 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/Transpose.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    10239 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/TreeNode.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.746152 interpret-core-0.4.2/symbolic/shared/libebm/bridge_c/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/bridge_c/bridge_c.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1203 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/bridge_c/zones.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.750152 interpret-core-0.4.2/symbolic/shared/libebm/bridge_cpp/
+-rw-r--r--   0 vsts      (1001) docker     (122)    13743 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/bridge_cpp/Bin.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8442 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/bridge_cpp/GradientPair.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8200 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/bridge_cpp/bridge_cpp.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.750152 interpret-core-0.4.2/symbolic/shared/libebm/common_c/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3037 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/common_c/common_c.c
+-rw-r--r--   0 vsts      (1001) docker     (122)     8476 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/common_c/common_c.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6580 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/common_c/logging.c
+-rw-r--r--   0 vsts      (1001) docker     (122)    10001 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/common_c/logging.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.750152 interpret-core-0.4.2/symbolic/shared/libebm/common_cpp/
+-rw-r--r--   0 vsts      (1001) docker     (122)    45433 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/common_cpp/common_cpp.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.754152 interpret-core-0.4.2/symbolic/shared/libebm/compute/
+-rw-r--r--   0 vsts      (1001) docker     (122)      553 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/Directory.Build.targets
+-rw-r--r--   0 vsts      (1001) docker     (122)     6382 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/Objective.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    35870 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/Objective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6723 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/Registration.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13194 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/Registration.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    50721 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/approximate_math.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.754152 interpret-core-0.4.2/symbolic/shared/libebm/compute/avx512_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      257 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/avx512_ebm/avx512_32.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13706 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)      477 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj.filters
+-rw-r--r--   0 vsts      (1001) docker     (122)     4386 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/compute.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    61597 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/compute_stats.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.754152 interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      254 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/cpu_32.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7447 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/cpu_64.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13427 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)      593 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj.filters
+-rw-r--r--   0 vsts      (1001) docker     (122)     8950 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/sse2_32.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/sse2_64.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.754152 interpret-core-0.4.2/symbolic/shared/libebm/compute/cuda_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11435 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cuda_ebm/cuda_32.cu
+-rw-r--r--   0 vsts      (1001) docker     (122)    14658 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)      505 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj.filters
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.754152 interpret-core-0.4.2/symbolic/shared/libebm/compute/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (122)      177 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/metrics/AucMetric.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.754152 interpret-core-0.4.2/symbolic/shared/libebm/compute/no_cuda_ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      630 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_32.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13332 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)      478 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj.filters
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.758152 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/
+-rw-r--r--   0 vsts      (1001) docker     (122)      432 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/CrossEntropyBinaryObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3630 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassMultitaskObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4464 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/ExampleRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3033 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/GammaDevianceRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      770 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/LogLossBinaryMultitaskObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7535 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/LogLossBinaryObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9437 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/LogLossMulticlassObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4596 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/PoissonDevianceRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4226 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/PseudoHuberRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3409 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/RmseLogLinkRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/RmseRegressionMultitaskObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9112 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/RmseRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4842 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/TweedieDevianceRegressionObjective.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3245 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/objective_registrations.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      267 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/precompiled_header_cpp.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2301 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/registration_exceptions.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.758152 interpret-core-0.4.2/symbolic/shared/libebm/compute/special/
+-rw-r--r--   0 vsts      (1001) docker     (122)      164 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/special/precompiled_header_cpp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2331 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/zoned_bridge_c_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/zoned_bridge_c_functions.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute/zoned_bridge_cpp_functions.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2800 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/compute_accessors.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)   101153 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/dataset_shared.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2242 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/dataset_shared.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    25788 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/debug_ebm.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8264 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/ebm_internal.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    41443 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/ebm_stats.hpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.758152 interpret-core-0.4.2/symbolic/shared/libebm/inc/
+-rw-r--r--   0 vsts      (1001) docker     (122)    20429 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/inc/libebm.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3650 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/include_ordering.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    13166 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/interpret.sln
+-rw-r--r--   0 vsts      (1001) docker     (122)    77375 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/interpretable_numerics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    24091 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/libebm.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)     5242 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/libebm.vcxproj.filters
+-rw-r--r--   0 vsts      (1001) docker     (122)      994 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/libebm_exports.def
+-rw-r--r--   0 vsts      (1001) docker     (122)     1257 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/libebm_exports.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/precompiled_header_cpp.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6007 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/random.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    25518 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/sampling.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.758152 interpret-core-0.4.2/symbolic/shared/libebm/special/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2874 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/special/linux_wrap_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      164 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/special/precompiled_header_cpp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      790 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/special/windows_DllMain.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.766152 interpret-core-0.4.2/symbolic/shared/libebm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)    46248 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/CutQuantileTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    12964 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/CutUniformTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    24882 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/CutWinsorizedTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/DiscretizeTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6935 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/RandomStreamTest.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    11983 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/SuggestGraphBoundsTest.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7580 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/bit_packing_extremes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    68448 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/boosting_unusual_inputs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    17142 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/dataset_shared_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2740 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/include_c.c
+-rw-r--r--   0 vsts      (1001) docker     (122)    16012 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/interaction_unusual_inputs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1931 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.bat
+-rw-r--r--   0 vsts      (1001) docker     (122)    41934 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14919 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    38501 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.sh
+-rw-r--r--   0 vsts      (1001) docker     (122)    15718 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.vcxproj
+-rw-r--r--   0 vsts      (1001) docker     (122)     1636 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.vcxproj.filters
+-rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/precompiled_header_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      298 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/precompiled_header_test.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    12851 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/random_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4893 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/tests/rehydrate_booster.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      564 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/libebm/vs_python_setup.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.766152 interpret-core-0.4.2/symbolic/shared/vis/
+-rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/vis/.babelrc
+-rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/vis/.eslintrc.json
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/vis/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)      238 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/vis/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1472 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/vis/package.json
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.766152 interpret-core-0.4.2/symbolic/shared/vis/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4433 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/vis/src/index.js
+-rw-r--r--   0 vsts      (1001) docker     (122)     1469 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/vis/src/styles.scss
+-rw-r--r--   0 vsts      (1001) docker     (122)      757 2023-06-01 03:23:28.000000 interpret-core-0.4.2/symbolic/shared/vis/webpack.config.js
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.766152 interpret-core-0.4.2/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.766152 interpret-core-0.4.2/tests/api/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1895 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/api/test_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.770152 interpret-core-0.4.2/tests/blackbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/blackbox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1435 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/blackbox/test_permutationimportance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      477 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/blackbox/test_sensitivity.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.770152 interpret-core-0.4.2/tests/ext/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/ext/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2502 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/ext/test_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.770152 interpret-core-0.4.2/tests/glassbox/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.770152 interpret-core-0.4.2/tests/glassbox/ebm/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.770152 interpret-core-0.4.2/tests/glassbox/ebm/research/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/research/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8067 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/research/test_group_importance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8414 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/research/test_purify.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4105 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/test_bin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    29387 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/test_ebm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5551 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/test_ebm_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5393 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/test_merge_ebms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      790 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/ebm/test_multiclass.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2055 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/test_decisiontree.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3499 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/glassbox/test_linear.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.770152 interpret-core-0.4.2/tests/greybox/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/greybox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1459 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/greybox/test_treeinterpreter.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.774153 interpret-core-0.4.2/tests/provider/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      470 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/provider/test_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2257 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/provider/test_providers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/test_develop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/test_example_notebooks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3215 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/test_explainers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2702 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/test_ext.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      691 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/test_extension_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1108 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/test_mli_interop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9489 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/test_selenium.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8241 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/tutils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.774153 interpret-core-0.4.2/tests/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1099 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/utils/test_SPOTgreedy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/utils/test_clean_simple.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   113135 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/utils/test_clean_x.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3041 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/utils/test_compressed_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1453 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/utils/test_explanation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8683 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/utils/test_measure_interactions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2888 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/utils/test_native.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-01 03:28:15.774153 interpret-core-0.4.2/tests/visual/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/visual/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      369 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/visual/test_dashboard.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      898 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/visual/test_inline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5223 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/visual/test_interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-06-01 03:23:28.000000 interpret-core-0.4.2/tests/visual/test_plot.py
```

### Comparing `interpret-core-0.4.1/PKG-INFO` & `interpret-core-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret-core
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fit interpretable models. Explain blackbox machine learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `interpret-core-0.4.1/interpret/api/base.py` & `interpret-core-0.4.2/interpret/api/base.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/api/templates.py` & `interpret-core-0.4.2/interpret/api/templates.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/blackbox/_lime.py` & `interpret-core-0.4.2/interpret/blackbox/_lime.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/blackbox/_partialdependence.py` & `interpret-core-0.4.2/interpret/blackbox/_partialdependence.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/blackbox/_permutationimportance.py` & `interpret-core-0.4.2/interpret/blackbox/_permutationimportance.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/blackbox/_sensitivity.py` & `interpret-core-0.4.2/interpret/blackbox/_sensitivity.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/blackbox/_shap.py` & `interpret-core-0.4.2/interpret/blackbox/_shap.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/data/_response.py` & `interpret-core-0.4.2/interpret/data/_response.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/develop.py` & `interpret-core-0.4.2/interpret/develop.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/ext/examples.py` & `interpret-core-0.4.2/interpret/ext/examples.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/ext/extension.py` & `interpret-core-0.4.2/interpret/ext/extension.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/ext/extension_utils.py` & `interpret-core-0.4.2/interpret/ext/extension_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_decisiontree.py` & `interpret-core-0.4.2/interpret/glassbox/_decisiontree.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_bin.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_bin.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_boost.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_boost.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,149 +30,153 @@
     noise_scale,
     bin_weights,
     rng,
     is_private,
     objective,
     experimental_params=None,
 ):
-    episode_index = 0
-    with Booster(
-        dataset,
-        bag,
-        init_scores,
-        term_features,
-        n_inner_bags,
-        rng,
-        is_private,
-        objective,
-        experimental_params,
-    ) as booster:
-        # the first round is alwasy cyclic since we need to get the initial gains
-        greedy_portion = 0.0
-
-        min_metric = np.inf
-        no_change_run_length = 0
-        bp_metric = np.inf
-        _log.info("Start boosting")
-        native = Native.get_native_singleton()
-
-        for episode_index in range(max_rounds):
-            if episode_index % 10 == 0:
-                _log.debug("Sweep Index {0}".format(episode_index))
-                _log.debug("Metric: {0}".format(min_metric))
-
-            if greedy_portion < 1.0:
-                # we're doing a cyclic round
-                heap = []
-
-            boost_flags_local = boost_flags
-            if 0 < smoothing_rounds:
-                # modify some of our parameters temporarily
-                boost_flags_local |= (
-                    Native.BoostFlags_DisableNewtonGain
-                    | Native.BoostFlags_DisableNewtonUpdate
-                    | Native.BoostFlags_RandomSplits
-                )
-
-            for term_idx in range(len(term_features)):
-                if 1.0 <= greedy_portion:
-                    # we're being greedy, so select something from our
-                    # queue and overwrite the term_idx we'll work on
-                    _, term_idx = heapq.heappop(heap)
-
-                avg_gain = booster.generate_term_update(
-                    term_idx=term_idx,
-                    boost_flags=boost_flags_local,
-                    learning_rate=learning_rate,
-                    min_samples_leaf=min_samples_leaf,
-                    max_leaves=max_leaves,
-                )
+    try:
+        episode_index = 0
+        with Booster(
+            dataset,
+            bag,
+            init_scores,
+            term_features,
+            n_inner_bags,
+            rng,
+            is_private,
+            objective,
+            experimental_params,
+        ) as booster:
+            # the first round is alwasy cyclic since we need to get the initial gains
+            greedy_portion = 0.0
+
+            min_metric = np.inf
+            no_change_run_length = 0
+            bp_metric = np.inf
+            _log.info("Start boosting")
+            native = Native.get_native_singleton()
+
+            for episode_index in range(max_rounds):
+                if episode_index % 10 == 0:
+                    _log.debug("Sweep Index {0}".format(episode_index))
+                    _log.debug("Metric: {0}".format(min_metric))
+
+                if greedy_portion < 1.0:
+                    # we're doing a cyclic round
+                    heap = []
+
+                boost_flags_local = boost_flags
+                if 0 < smoothing_rounds:
+                    # modify some of our parameters temporarily
+                    boost_flags_local |= (
+                        Native.BoostFlags_DisableNewtonGain
+                        | Native.BoostFlags_DisableNewtonUpdate
+                        | Native.BoostFlags_RandomSplits
+                    )
 
-                heapq.heappush(heap, (-avg_gain, term_idx))
+                for term_idx in range(len(term_features)):
+                    if 1.0 <= greedy_portion:
+                        # we're being greedy, so select something from our
+                        # queue and overwrite the term_idx we'll work on
+                        _, term_idx = heapq.heappop(heap)
+
+                    avg_gain = booster.generate_term_update(
+                        rng,
+                        term_idx=term_idx,
+                        boost_flags=boost_flags_local,
+                        learning_rate=learning_rate,
+                        min_samples_leaf=min_samples_leaf,
+                        max_leaves=max_leaves,
+                    )
 
-                if noise_scale:  # Differentially private updates
-                    splits = booster.get_term_update_splits()[0]
+                    heapq.heappush(heap, (-avg_gain, term_idx))
 
-                    term_update_tensor = booster.get_term_update()
-                    noisy_update_tensor = term_update_tensor.copy()
+                    if noise_scale:  # Differentially private updates
+                        splits = booster.get_term_update_splits()[0]
 
-                    # Make splits iteration friendly
-                    splits_iter = [0] + list(splits + 1) + [len(term_update_tensor)]
+                        term_update_tensor = booster.get_term_update()
+                        noisy_update_tensor = term_update_tensor.copy()
 
-                    n_sections = len(splits_iter) - 1
-                    noises = native.generate_gaussian_random(
-                        rng, noise_scale, n_sections
-                    )
+                        # Make splits iteration friendly
+                        splits_iter = [0] + list(splits) + [len(term_update_tensor)]
 
-                    # Loop through all random splits and add noise before updating
-                    for f, s, noise in zip(splits_iter[:-1], splits_iter[1:], noises):
-                        if s == 1:
-                            # Skip cuts that fall on 0th (missing value) bin -- missing values not supported in DP
-                            continue
-
-                        noisy_update_tensor[f:s] = term_update_tensor[f:s] + noise
-
-                        # Native code will be returning sums of residuals in slices, not averages.
-                        # Compute noisy average by dividing noisy sum by noisy bin weights
-                        region_weight = np.sum(bin_weights[term_idx][f:s])
-                        noisy_update_tensor[f:s] = (
-                            noisy_update_tensor[f:s] / region_weight
+                        n_sections = len(splits_iter) - 1
+                        noises = native.generate_gaussian_random(
+                            rng, noise_scale, n_sections
                         )
 
-                    # Invert gradients before updates
-                    noisy_update_tensor = -noisy_update_tensor
-                    booster.set_term_update(term_idx, noisy_update_tensor)
-
-                cur_metric = booster.apply_term_update()
-
-                min_metric = min(cur_metric, min_metric)
-
-            # TODO PK this early_stopping_tolerance is a little inconsistent
-            #      since it triggers intermittently and only re-triggers if the
-            #      threshold is re-passed, but not based on a smooth windowed set
-            #      of checks.  We can do better by keeping a list of the last
-            #      number of measurements to have a consistent window of values.
-            #      If we only cared about the metric at the start and end of the epoch
-            #      window a circular buffer would be best choice with O(1).
-            if no_change_run_length == 0:
-                bp_metric = min_metric
-
-            # TODO: PK, I think this is a bug and the first iteration no_change_run_length
-            # get incremented to 1, so if early_stopping_rounds is 1 it will always
-            # exit on the first round? I haven't changed it since it's just going to affect 1
-            # and changing it would change the results so I need to benchmark update it
-            if min_metric + early_stopping_tolerance < bp_metric:
-                no_change_run_length = 0
-            else:
-                no_change_run_length += 1
-
-            if 1.0 <= greedy_portion:
-                greedy_portion -= 1.0
+                        # Loop through all random splits and add noise before updating
+                        for f, s, noise in zip(
+                            splits_iter[:-1], splits_iter[1:], noises
+                        ):
+                            noisy_update_tensor[f:s] = term_update_tensor[f:s] + noise
+
+                            # Native code will be returning sums of residuals in slices, not averages.
+                            # Compute noisy average by dividing noisy sum by noisy bin weights
+                            region_weight = np.sum(
+                                bin_weights[term_features[term_idx][0]][f:s]
+                            )
+                            noisy_update_tensor[f:s] = (
+                                noisy_update_tensor[f:s] / region_weight
+                            )
+
+                        # Invert gradients before updates
+                        noisy_update_tensor = -noisy_update_tensor
+                        booster.set_term_update(term_idx, noisy_update_tensor)
+
+                    cur_metric = booster.apply_term_update()
+
+                    min_metric = min(cur_metric, min_metric)
+
+                # TODO PK this early_stopping_tolerance is a little inconsistent
+                #      since it triggers intermittently and only re-triggers if the
+                #      threshold is re-passed, but not based on a smooth windowed set
+                #      of checks.  We can do better by keeping a list of the last
+                #      number of measurements to have a consistent window of values.
+                #      If we only cared about the metric at the start and end of the epoch
+                #      window a circular buffer would be best choice with O(1).
+                if no_change_run_length == 0:
+                    bp_metric = min_metric
+
+                # TODO: PK, I think this is a bug and the first iteration no_change_run_length
+                # get incremented to 1, so if early_stopping_rounds is 1 it will always
+                # exit on the first round? I haven't changed it since it's just going to affect 1
+                # and changing it would change the results so I need to benchmark update it
+                if min_metric + early_stopping_tolerance < bp_metric:
+                    no_change_run_length = 0
+                else:
+                    no_change_run_length += 1
 
-            if 0 < smoothing_rounds:
-                # disable early stopping progress during the smoothing rounds since
-                # cuts are chosen randomly, which will lead to high variance on the
-                # validation metric
-                no_change_run_length = 0
-                smoothing_rounds -= 1
-            else:
-                # do not progress into greedy rounds until we're done with the smoothing_rounds
-                greedy_portion += greediness
+                if 1.0 <= greedy_portion:
+                    greedy_portion -= 1.0
 
-            if (
-                early_stopping_rounds > 0
-                and no_change_run_length >= early_stopping_rounds
-            ):
-                break
-
-        _log.info(
-            "End boosting, Best Metric: {0}, Num Rounds: {1}".format(
-                min_metric, episode_index
+                if 0 < smoothing_rounds:
+                    # disable early stopping progress during the smoothing rounds since
+                    # cuts are chosen randomly, which will lead to high variance on the
+                    # validation metric
+                    no_change_run_length = 0
+                    smoothing_rounds -= 1
+                else:
+                    # do not progress into greedy rounds until we're done with the smoothing_rounds
+                    greedy_portion += greediness
+
+                if (
+                    early_stopping_rounds > 0
+                    and no_change_run_length >= early_stopping_rounds
+                ):
+                    break
+
+            _log.info(
+                "End boosting, Best Metric: {0}, Num Rounds: {1}".format(
+                    min_metric, episode_index
+                )
             )
-        )
 
-        if early_stopping_rounds > 0:
-            model_update = booster.get_best_model()
-        else:
-            model_update = booster.get_current_model()
+            if early_stopping_rounds > 0:
+                model_update = booster.get_best_model()
+            else:
+                model_update = booster.get_current_model()
 
-    return model_update, episode_index, rng
+        return None, model_update, episode_index, rng
+    except Exception as e:
+        return e, None, None, None
```

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_ebm.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_ebm.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,20 +36,15 @@
 
 from ._bin import (
     eval_terms,
     ebm_decision_function,
     ebm_decision_function_and_explain,
     make_bin_weights,
 )
-from ._tensor import (
-    make_boosting_weights,
-    after_boosting,
-    remove_last,
-    trim_tensor,
-)
+from ._tensor import remove_last, trim_tensor
 from ...utils._native import Native
 from ...api.base import ExplainerMixin
 from ...api.templates import FeatureValueExplanation
 from ...provider import JobLibProvider
 from ...utils._explanation import (
     gen_name_from_class,
     gen_global_selector,
@@ -373,21 +368,25 @@
             if random_state is not None:
                 warn(
                     f"Privacy violation: using a fixed random_state of {random_state} "
                     "will cause deterministic noise additions. This capability is only "
                     "for debugging/testing. Set random_state to None to remove this warning."
                 )
 
-    def fit(self, X, y, sample_weight=None, init_score=None):  # noqa: C901
+    def fit(self, X, y, sample_weight=None, bags=None, init_score=None):  # noqa: C901
         """Fits model to provided samples.
 
         Args:
             X: Numpy array for training samples.
             y: Numpy array as training labels.
             sample_weight: Optional array of weights per sample. Should be same length as X and y.
+            bags: Optional bag definitions. The first dimension should have length equal to the number of outer_bags.
+                The second dimension should have length equal to the number of samples. The contents should be
+                +1 for training, -1 for validation, and 0 if not included in the bag. Numbers other than 1 indicate
+                how many times to include the sample in the training or validation sets.
             init_score: Optional. Either a model that can generate scores or per-sample initialization score.
                 If samples scores it should be the same length as X.
 
         Returns:
             Itself.
         """
 
@@ -399,14 +398,20 @@
             _log.error(msg)
             raise ValueError(msg)
         elif self.outer_bags < 1:
             msg = "outer_bags must be 1 or greater. Did you mean to set: outer_bags=1, validation_size=0?"
             _log.error(msg)
             raise ValueError(msg)
 
+        if bags is not None:
+            if len(bags) != self.outer_bags:
+                msg = f"bags has {len(bags)} bags and self.outer_bags is {self.outer_bags} bags"
+                _log.error(msg)
+                raise ValueError(msg)
+
         if not isinstance(self.validation_size, int) and not isinstance(
             self.validation_size, float
         ):
             msg = "validation_size must be an integer or float"
             _log.error(msg)
             raise ValueError(msg)
         elif self.validation_size <= 0:
@@ -676,14 +681,79 @@
         elif exclude == "mains":
             exclude = set()
             term_features = []
         else:
             exclude = _clean_exclude(exclude, feature_map)
             term_features = [(x,) for x in range(n_features_in) if (x,) not in exclude]
 
+        rng = native.create_rng(init_random_state)
+        # branch it so we have no correlation to the binning rng that uses the same seed
+        rng = native.branch_rng(rng)
+        used_seeds = set()
+        rngs = []
+        internal_bags = []
+        for idx in range(self.outer_bags):
+            while True:
+                bagged_rng = native.branch_rng(rng)
+                seed = native.generate_seed(bagged_rng)
+                # we really really do not want identical bags. branch_rng is pretty good but it can lead to
+                # collisions, so check with a 32-bit seed if we possibly have a collision and regenerate if so
+                if seed not in used_seeds:
+                    break
+            # we do not need used_seeds if the rng is None, but it does not hurt anything
+            used_seeds.add(seed)
+
+            if bags is None:
+                bag = make_bag(
+                    y,
+                    self.validation_size,
+                    bagged_rng,
+                    is_classifier(self) and not is_differential_privacy,
+                )
+                # we bag within the same proces, so bagged_rng will progress inside make_bag
+            else:
+                bag = bags[idx]
+                if not isinstance(bag, np.ndarray):
+                    bag = np.array(bag)
+                if bag.ndim != 1:
+                    msg = "bags must be 2-dimensional"
+                    _log.error(msg)
+                    raise ValueError(msg)
+                if len(y) != len(bag):
+                    msg = f"y has {len(y)} samples and bags has {len(bag)} samples"
+                    _log.error(msg)
+                    raise ValueError(msg)
+                if (127 < bag).any() or (bag < -128).any():
+                    msg = "A value in bags is outside the valid range -128 to 127"
+                    _log.error(msg)
+                    raise ValueError(msg)
+                if bag.flags.c_contiguous:
+                    bag = bag.astype(np.int8, copy=False)
+                else:
+                    bag = bag.astype(np.int8, copy=True)
+
+            rngs.append(bagged_rng)
+            internal_bags.append(bag)
+
+        bag_weights = []
+        for bag in internal_bags:
+            if bag is None:
+                if sample_weight is None:
+                    bag_weights.append(n_samples)
+                else:
+                    bag_weights.append(sample_weight.sum())
+            else:
+                keep = 0 < bag
+                if sample_weight is None:
+                    bag_weights.append(bag[keep].sum())
+                else:
+                    bag_weights.append((bag[keep] * sample_weight[keep]).sum())
+                del keep
+        bag_weights = np.array(bag_weights, np.float64)
+
         if is_differential_privacy:
             # [DP] Calculate how much noise will be applied to each iteration of the algorithm
             domain_size = 1 if is_classifier(self) else max_target - min_target
             max_weight = 1 if sample_weight is None else np.max(sample_weight)
             training_eps = self.epsilon - bin_eps
             training_delta = self.delta - bin_delta
             if self.composition == "classic":
@@ -706,15 +776,15 @@
                 # Alg Line 17
                 noise_scale_boosting *= domain_size * self.learning_rate * max_weight
             else:
                 raise NotImplementedError(
                     f"Unknown composition method provided: {self.composition}. Please use 'gdp' or 'classic'."
                 )
 
-            bin_data_weights = make_boosting_weights(main_bin_weights)
+            bin_data_weights = main_bin_weights
             boost_flags = (
                 Native.BoostFlags_GradientSums | Native.BoostFlags_RandomSplits
             )
             inner_bags = 0
             greediness = 0.0
             smoothing_rounds = 0
             early_stopping_rounds = 0
@@ -729,54 +799,14 @@
             greediness = self.greediness
             smoothing_rounds = self.smoothing_rounds
             early_stopping_rounds = self.early_stopping_rounds
             early_stopping_tolerance = self.early_stopping_tolerance
             min_samples_leaf = self.min_samples_leaf
             interactions = self.interactions
 
-        rng = native.create_rng(init_random_state)
-        # branch it so we have no correlation to the binning rng that uses the same seed
-        rng = native.branch_rng(rng)
-        used_seeds = set()
-        rngs = []
-        bag_weights = []
-        bags = []
-        for _ in range(self.outer_bags):
-            while True:
-                bagged_rng = native.branch_rng(rng)
-                seed = native.generate_seed(bagged_rng)
-                # we really really do not want identical bags. branch_rng is pretty good but it can lead to
-                # collisions, so check with a 32-bit seed if we possibly have a collision and regenerate if so
-                if seed not in used_seeds:
-                    break
-            # we do not need used_seeds if the rng is None, but it does not hurt anything
-            used_seeds.add(seed)
-
-            bag = make_bag(
-                y,
-                self.validation_size,
-                bagged_rng,
-                is_classifier(self) and not is_differential_privacy,
-            )
-            # we bag within the same proces, so bagged_rng will progress inside make_bag
-            rngs.append(bagged_rng)
-            bags.append(bag)
-            if bag is None:
-                if sample_weight is None:
-                    bag_weights.append(n_samples)
-                else:
-                    bag_weights.append(sample_weight.sum())
-            else:
-                keep = 0 < bag
-                if sample_weight is None:
-                    bag_weights.append(bag[keep].sum())
-                else:
-                    bag_weights.append((bag[keep] * sample_weight[keep]).sum())
-        bag_weights = np.array(bag_weights, np.float64)
-
         if n_classes == 1:
             warn(
                 "Only 1 class detected for classification. The model will predict 1.0 whenever predict_proba is called."
             )
 
             breakpoint_iteration = [[]]
             models = []
@@ -811,24 +841,35 @@
                 feature_names_in,
                 feature_types_in,
             )
 
             parallel_args = []
             for idx in range(self.outer_bags):
                 early_stopping_rounds_local = early_stopping_rounds
-                if bags[idx] is None or (0 <= bags[idx]).all():
+                bag = internal_bags[idx]
+                if bag is None or (0 <= bag).all():
                     # if there are no validation samples, turn off early stopping
                     # because the validation metric cannot improve each round
                     early_stopping_rounds_local = 0
 
+                init_score_local = init_score
+                if (
+                    init_score_local is not None
+                    and bag is not None
+                    and np.count_nonzero(bag) != len(bag)
+                ):
+                    # TODO: instead of making these copies we should
+                    # put init_score into the native shared dataframe
+                    init_score_local = init_score_local[bag != 0]
+
                 parallel_args.append(
                     (
                         dataset,
-                        bags[idx],
-                        init_score,
+                        bag,
+                        init_score_local,
                         term_features,
                         inner_bags,
                         boost_flags,
                         self.learning_rate,
                         min_samples_leaf,
                         self.max_leaves,
                         greediness,
@@ -850,17 +891,19 @@
             # let python reclaim the dataset memory via reference counting
             del parallel_args  # parallel_args holds references to dataset, so must be deleted
             del dataset
 
             breakpoint_iteration = [[]]
             models = []
             rngs = []
-            for model, bag_breakpoint_iteration, bagged_rng in results:
+            for exception, model, bag_breakpoint_iteration, bagged_rng in results:
+                if exception is not None:
+                    raise exception
                 breakpoint_iteration[-1].append(bag_breakpoint_iteration)
-                models.append(after_boosting(term_features, model, main_bin_weights))
+                models.append(model)
                 # retrieve our rng state since this was used outside of our process
                 rngs.append(bagged_rng)
 
             while True:  # this isn't for looping. Just for break statements to exit
                 if interactions is None:
                     break
 
@@ -904,30 +947,31 @@
                             "if you know what you are doing."
                         )
 
                 initial_intercept = np.zeros(
                     Native.get_count_scores_c(n_classes), np.float64
                 )
                 scores_bags = []
-                for model in models:
+                for model, bag in zip(models, internal_bags):
                     # TODO: instead of going back to the original data in X, we
                     # could use the compressed and already binned data in dataset
-                    scores_bags.append(
-                        ebm_decision_function(
-                            X,
-                            n_samples,
-                            feature_names_in,
-                            feature_types_in,
-                            bins,
-                            initial_intercept,
-                            model,
-                            term_features,
-                            init_score,
-                        )
+                    scores = ebm_decision_function(
+                        X,
+                        n_samples,
+                        feature_names_in,
+                        feature_types_in,
+                        bins,
+                        initial_intercept,
+                        model,
+                        term_features,
+                        init_score,
                     )
+                    if bag is not None and np.count_nonzero(bag) != len(bag):
+                        scores = scores[bag != 0]
+                    scores_bags.append(scores)
 
                 dataset = bin_native_by_dimension(
                     n_classes,
                     2,
                     bins,
                     X,
                     y,
@@ -942,15 +986,15 @@
 
                     parallel_args = []
                     for idx in range(self.outer_bags):
                         # TODO: the combinations below should be selected from the non-excluded features
                         parallel_args.append(
                             (
                                 dataset,
-                                bags[idx],
+                                internal_bags[idx],
                                 scores_bags[idx],
                                 combinations(range(n_features_in), 2),
                                 exclude,
                                 Native.InteractionFlags_Default,
                                 max_cardinality,
                                 min_samples_leaf,
                                 is_differential_privacy,
@@ -959,22 +1003,25 @@
                             )
                         )
 
                     bagged_ranked_interaction = provider.parallel(
                         rank_interactions, parallel_args
                     )
 
-                    # this holds references to dataset, bags, and scores_bags which we want python to reclaim later
+                    # this holds references to dataset, internal_bags, and scores_bags which we want python to reclaim later
                     del parallel_args
 
                     # Select merged pairs
                     pair_ranks = {}
                     for n, interaction_strengths_and_indices in enumerate(
                         bagged_ranked_interaction
                     ):
+                        if isinstance(interaction_strengths_and_indices, Exception):
+                            raise interaction_strengths_and_indices
+
                         interaction_indices = list(
                             map(
                                 operator.itemgetter(1),
                                 interaction_strengths_and_indices,
                             )
                         )
                         for rank, indices in enumerate(interaction_indices):
@@ -1022,23 +1069,23 @@
                             "global explanations. Local explanations are still "
                             "available and exact."
                         )
 
                 parallel_args = []
                 for idx in range(self.outer_bags):
                     early_stopping_rounds_local = early_stopping_rounds
-                    if bags[idx] is None or (0 <= bags[idx]).all():
+                    if internal_bags[idx] is None or (0 <= internal_bags[idx]).all():
                         # if there are no validation samples, turn off early stopping
                         # because the validation metric cannot improve each round
                         early_stopping_rounds_local = 0
 
                     parallel_args.append(
                         (
                             dataset,
-                            bags[idx],
+                            internal_bags[idx],
                             scores_bags[idx],
                             boost_groups,
                             inner_bags,
                             boost_flags,
                             self.learning_rate,
                             min_samples_leaf,
                             self.max_leaves,
@@ -1061,19 +1108,19 @@
                 # allow python to reclaim these big memory items via reference counting
                 del parallel_args  # this holds references to dataset, scores_bags, and bags
                 del dataset
                 del scores_bags
 
                 breakpoint_iteration.append([])
                 for idx in range(self.outer_bags):
-                    breakpoint_iteration[-1].append(results[idx][1])
-                    models[idx].extend(
-                        after_boosting(boost_groups, results[idx][0], main_bin_weights)
-                    )
-                    rngs[idx] = results[idx][2]
+                    if results[idx][0] is not None:
+                        raise results[idx][0]
+                    breakpoint_iteration[-1].append(results[idx][2])
+                    models[idx].extend(results[idx][1])
+                    rngs[idx] = results[idx][3]
 
                 term_features.extend(boost_groups)
 
                 break  # do not loop!
 
         breakpoint_iteration = np.array(breakpoint_iteration, np.int64)
```

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_merge_ebms.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_merge_ebms.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,15 +566,15 @@
         if hasattr(model, "bagged_scores_"):
             if 0 < len(model.bagged_scores_):
                 n_outer_bags = len(model.bagged_scores_[0])
 
         model_bag_weights = getattr(model, "bag_weights_", None)
         if model_bag_weights is None:
             # this model wasn't the result of a merge, so get the total weight for the model
-            # every feature group in a model should have the same weight, but perhaps the user edited
+            # every term in a model should have the same weight, but perhaps the user edited
             # the model weights and they don't agree.  We handle these by taking the average
             model_bag_weights = [avg_weight] * n_outer_bags
         elif len(model_bag_weights) != n_outer_bags:
             raise Exception(
                 "self.bagged_weights_ should have the same length as n_outer_bags."
             )
 
@@ -592,15 +592,15 @@
         ]
         fg_dicts.append(dict(zip(fg_sorted, count())))
         all_fg.update(fg_sorted)
 
     sorted_fgs = order_terms(list(all_fg))
 
     # TODO: in the future we might at this point try and figure out the most
-    #       common feature ordering within the feature groups.  Take the mode first
+    #       common feature ordering within the terms.  Take the mode first
     #       and amonst the orderings that tie, choose the one that's best sorted by
     #       feature indexes
     ebm.term_features_ = sorted_fgs
 
     ebm.bin_weights_ = []
     ebm.bagged_scores_ = []
     for sorted_fg in sorted_fgs:
@@ -651,15 +651,15 @@
                     old_bins[model_idx],
                     old_mapping[model_idx],
                     model.bin_weights_[term_idx],
                     None,
                 )
                 bin_weight_percentages.append(fixed_tensor * model_weight)
 
-        # use this when we don't have a feature group in a model as a reasonable
+        # use this when we don't have a term in a model as a reasonable
         # set of guesses for the distribution of the weight of the model
         bin_weight_percentages = np.sum(bin_weight_percentages, axis=0)
         bin_weight_percentages = bin_weight_percentages / bin_weight_percentages.sum()
 
         additive_shape = bin_weight_percentages.shape
         if 2 < n_classes:
             additive_shape = tuple(list(additive_shape) + [n_classes])
```

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_multiclass.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_multiclass.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_research/__init__.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_research/__init__.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_research/_group_importance.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_research/_group_importance.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_research/_purify.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_research/_purify.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_ebm/_utils.py` & `interpret-core-0.4.2/interpret/glassbox/_ebm/_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_linear.py` & `interpret-core-0.4.2/interpret/glassbox/_linear.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/glassbox/_skoperules.py` & `interpret-core-0.4.2/interpret/glassbox/_skoperules.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/greybox/_shaptree.py` & `interpret-core-0.4.2/interpret/greybox/_shaptree.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/greybox/_treeinterpreter.py` & `interpret-core-0.4.2/interpret/greybox/_treeinterpreter.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/lib/interpret-inline.js` & `interpret-core-0.4.2/interpret/lib/interpret-inline.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1025,146 +1025,149 @@
                         function Jt(t) {
                             return t instanceof Xt(t).Node
                         }
 
                         function $t(t) {
                             return Jt(t) ? (t.nodeName || "").toLowerCase() : ""
                         }
-                        let Qt;
 
-                        function te(t) {
+                        function Qt(t) {
                             return t instanceof Xt(t).HTMLElement
                         }
 
-                        function ee(t) {
+                        function te(t) {
                             return t instanceof Xt(t).Element
                         }
 
-                        function re(t) {
+                        function ee(t) {
                             return "undefined" != typeof ShadowRoot && (t instanceof Xt(t).ShadowRoot || t instanceof ShadowRoot)
                         }
 
-                        function ne(t) {
+                        function re(t) {
                             const {
                                 overflow: e,
                                 overflowX: r,
                                 overflowY: n,
                                 display: i
                             } = Kt(t);
                             return /auto|scroll|overlay|hidden|clip/.test(e + n + r) && !["inline", "contents"].includes(i)
-                        }
-
-                        function ie() {
-                            return /^((?!chrome|android).)*safari/i.test(function() {
-                                if (Qt) return Qt;
-                                const t = navigator.userAgentData;
-                                return t && Array.isArray(t.brands) ? (Qt = t.brands.map((t => t.brand + "/" + t.version)).join(" "), Qt) : navigator.userAgent
-                            }())
                         } ["top", "right", "bottom", "left"].reduce(((t, e) => t.concat(e, e + "-start", e + "-end")), []), Math.min, Math.max;
-                        const ae = Math.round;
+                        const ne = Math.round;
 
-                        function oe(t) {
-                            return ee(t) ? t : t.contextElement
+                        function ie(t) {
+                            return te(t) ? t : t.contextElement
                         }
-                        const se = {
+                        const ae = {
                             x: 1,
                             y: 1
                         };
 
-                        function le(t) {
-                            const e = oe(t);
-                            if (!te(e)) return se;
+                        function oe(t) {
+                            const e = ie(t);
+                            if (!Qt(e)) return ae;
                             const r = e.getBoundingClientRect(),
                                 {
                                     width: n,
                                     height: i,
                                     fallback: a
                                 } = function(t) {
                                     const e = Kt(t);
                                     let r = parseFloat(e.width) || 0,
                                         n = parseFloat(e.height) || 0;
-                                    const i = te(t),
+                                    const i = Qt(t),
                                         a = i ? t.offsetWidth : r,
                                         o = i ? t.offsetHeight : n,
-                                        s = ae(r) !== a || ae(n) !== o;
+                                        s = ne(r) !== a || ne(n) !== o;
                                     return s && (r = a, n = o), {
                                         width: r,
                                         height: n,
                                         fallback: s
                                     }
                                 }(e);
-                            let o = (a ? ae(r.width) : r.width) / n,
-                                s = (a ? ae(r.height) : r.height) / i;
+                            let o = (a ? ne(r.width) : r.width) / n,
+                                s = (a ? ne(r.height) : r.height) / i;
                             return o && Number.isFinite(o) || (o = 1), s && Number.isFinite(s) || (s = 1), {
                                 x: o,
                                 y: s
                             }
                         }
+                        const se = {
+                            x: 0,
+                            y: 0
+                        };
+
+                        function le(t, e, r) {
+                            var n, i;
+                            if (void 0 === e && (e = !0), "undefined" == typeof CSS || !CSS.supports || !CSS.supports("-webkit-backdrop-filter", "none")) return se;
+                            const a = t ? Xt(t) : window;
+                            return !r || e && r !== a ? se : {
+                                x: (null == (n = a.visualViewport) ? void 0 : n.offsetLeft) || 0,
+                                y: (null == (i = a.visualViewport) ? void 0 : i.offsetTop) || 0
+                            }
+                        }
 
                         function ue(t, e, r, n) {
-                            var i, a;
                             void 0 === e && (e = !1), void 0 === r && (r = !1);
-                            const o = t.getBoundingClientRect(),
-                                s = oe(t);
-                            let l = se;
-                            e && (n ? ee(n) && (l = le(n)) : l = le(t));
-                            const u = s ? Xt(s) : window,
-                                c = ie() && r;
-                            let f = (o.left + (c && (null == (i = u.visualViewport) ? void 0 : i.offsetLeft) || 0)) / l.x,
-                                h = (o.top + (c && (null == (a = u.visualViewport) ? void 0 : a.offsetTop) || 0)) / l.y,
-                                p = o.width / l.x,
-                                d = o.height / l.y;
-                            if (s) {
-                                const t = Xt(s),
-                                    e = n && ee(n) ? Xt(n) : n;
+                            const i = t.getBoundingClientRect(),
+                                a = ie(t);
+                            let o = ae;
+                            e && (n ? te(n) && (o = oe(n)) : o = oe(t));
+                            const s = le(a, r, n);
+                            let l = (i.left + s.x) / o.x,
+                                u = (i.top + s.y) / o.y,
+                                c = i.width / o.x,
+                                f = i.height / o.y;
+                            if (a) {
+                                const t = Xt(a),
+                                    e = n && te(n) ? Xt(n) : n;
                                 let r = t.frameElement;
                                 for (; r && n && e !== t;) {
-                                    const t = le(r),
+                                    const t = oe(r),
                                         e = r.getBoundingClientRect(),
                                         n = getComputedStyle(r);
-                                    e.x += (r.clientLeft + parseFloat(n.paddingLeft)) * t.x, e.y += (r.clientTop + parseFloat(n.paddingTop)) * t.y, f *= t.x, h *= t.y, p *= t.x, d *= t.y, f += e.x, h += e.y, r = Xt(r).frameElement
+                                    e.x += (r.clientLeft + parseFloat(n.paddingLeft)) * t.x, e.y += (r.clientTop + parseFloat(n.paddingTop)) * t.y, l *= t.x, u *= t.y, c *= t.x, f *= t.y, l += e.x, u += e.y, r = Xt(r).frameElement
                                 }
                             }
-                            return v = {
-                                width: p,
-                                height: d,
-                                x: f,
-                                y: h
+                            return h = {
+                                width: c,
+                                height: f,
+                                x: l,
+                                y: u
                             }, {
-                                ...v,
-                                top: v.y,
-                                left: v.x,
-                                right: v.x + v.width,
-                                bottom: v.y + v.height
+                                ...h,
+                                top: h.y,
+                                left: h.x,
+                                right: h.x + h.width,
+                                bottom: h.y + h.height
                             };
-                            var v
+                            var h
                         }
 
                         function ce(t) {
                             if ("html" === $t(t)) return t;
-                            const e = t.assignedSlot || t.parentNode || re(t) && t.host || function(t) {
+                            const e = t.assignedSlot || t.parentNode || ee(t) && t.host || function(t) {
                                 return ((Jt(t) ? t.ownerDocument : t.document) || window.document).documentElement
                             }(t);
-                            return re(e) ? e.host : e
+                            return ee(e) ? e.host : e
                         }
 
                         function fe(t) {
                             const e = ce(t);
                             return function(t) {
                                 return ["html", "body", "#document"].includes($t(t))
-                            }(e) ? e.ownerDocument.body : te(e) && ne(e) ? e : fe(e)
+                            }(e) ? e.ownerDocument.body : Qt(e) && re(e) ? e : fe(e)
                         }
 
                         function he(t, e) {
                             var r;
                             void 0 === e && (e = []);
                             const n = fe(t),
                                 i = n === (null == (r = t.ownerDocument) ? void 0 : r.body),
                                 a = Xt(n);
-                            return i ? e.concat(a, a.visualViewport || [], ne(n) ? n : []) : e.concat(n, he(n))
+                            return i ? e.concat(a, a.visualViewport || [], re(n) ? n : []) : e.concat(n, he(n))
                         }
                         const pe = n.useLayoutEffect;
                         var de = ["className", "clearValue", "cx", "getStyles", "getClassNames", "getValue", "hasValue", "isMulti", "isRtl", "options", "selectOption", "selectProps", "setValue", "theme"],
                             ve = function() {};
 
                         function ge(t, e) {
                             return e ? "-" === e[0] ? t + e : t + "__" + e : t
@@ -1731,25 +1734,25 @@
                                         "function" == typeof c.current && (c.current(), c.current = null), i && u.current && (c.current = function(t, e, r, n) {
                                             void 0 === n && (n = {});
                                             const {
                                                 ancestorScroll: i = !0,
                                                 ancestorResize: a = !0,
                                                 elementResize: o = !0,
                                                 animationFrame: s = !1
-                                            } = n, l = i || a ? [...ee(t) ? he(t) : t.contextElement ? he(t.contextElement) : [], ...he(e)] : [];
+                                            } = n, l = i || a ? [...te(t) ? he(t) : t.contextElement ? he(t.contextElement) : [], ...he(e)] : [];
                                             l.forEach((t => {
-                                                const e = !ee(t) && t.toString().includes("V");
+                                                const e = !te(t) && t.toString().includes("V");
                                                 !i || s && !e || t.addEventListener("scroll", r, {
                                                     passive: !0
                                                 }), a && t.addEventListener("resize", r)
                                             }));
                                             let u, c = null;
                                             o && (c = new ResizeObserver((() => {
                                                 r()
-                                            })), ee(t) && !s && c.observe(t), ee(t) || !t.contextElement || s || c.observe(t.contextElement), c.observe(e));
+                                            })), te(t) && !s && c.observe(t), te(t) || !t.contextElement || s || c.observe(t.contextElement), c.observe(e));
                                             let f = s ? ue(t) : null;
                                             return s && function e() {
                                                 const n = ue(t);
                                                 !f || n.x === f.x && n.y === f.y && n.width === f.width && n.height === f.height || r(), f = n, u = requestAnimationFrame(e)
                                             }(), r(), () => {
                                                 var t;
                                                 l.forEach((t => {
@@ -11948,15 +11951,15 @@
                                 textOverflowWrap: {
                                     enums: ["whitespace", "anywhere"]
                                 },
                                 textBackgroundShape: {
                                     enums: ["rectangle", "roundrectangle", "round-rectangle"]
                                 },
                                 nodeShape: {
-                                    enums: ["rectangle", "roundrectangle", "round-rectangle", "cutrectangle", "cut-rectangle", "bottomroundrectangle", "bottom-round-rectangle", "barrel", "ellipse", "triangle", "round-triangle", "square", "pentagon", "round-pentagon", "hexagon", "round-hexagon", "concavehexagon", "concave-hexagon", "heptagon", "round-heptagon", "octagon", "round-octagon", "tag", "round-tag", "star", "diamond", "round-diamond", "vee", "rhomboid", "polygon"]
+                                    enums: ["rectangle", "roundrectangle", "round-rectangle", "cutrectangle", "cut-rectangle", "bottomroundrectangle", "bottom-round-rectangle", "barrel", "ellipse", "triangle", "round-triangle", "square", "pentagon", "round-pentagon", "hexagon", "round-hexagon", "concavehexagon", "concave-hexagon", "heptagon", "round-heptagon", "octagon", "round-octagon", "tag", "round-tag", "star", "diamond", "round-diamond", "vee", "rhomboid", "right-rhomboid", "polygon"]
                                 },
                                 overlayShape: {
                                     enums: ["roundrectangle", "round-rectangle", "ellipse"]
                                 },
                                 compoundIncludeLabels: {
                                     enums: ["include", "exclude"]
                                 },
@@ -14236,76 +14239,76 @@
                             return this
                         }, Ja.prototype.stop = function() {
                             return this.stopped = !0, this.thread && this.thread.stop(), this.emit("layoutstop"), this
                         }, Ja.prototype.destroy = function() {
                             return this.thread && this.thread.stop(), this
                         };
                         var $a = function(t, e, r) {
-                                for (var n = r.eles.edges(), i = r.eles.nodes(), a = {
+                                for (var n = r.eles.edges(), i = r.eles.nodes(), a = de(r.boundingBox ? r.boundingBox : {
+                                        x1: 0,
+                                        y1: 0,
+                                        w: t.width(),
+                                        h: t.height()
+                                    }), o = {
                                         isCompound: t.hasCompoundNodes(),
                                         layoutNodes: [],
                                         idToIndex: {},
                                         nodeSize: i.size(),
                                         graphSet: [],
                                         indexToGraph: [],
                                         layoutEdges: [],
                                         edgeSize: n.size(),
                                         temperature: r.initialTemp,
-                                        clientWidth: t.width(),
-                                        clientHeight: t.width(),
-                                        boundingBox: de(r.boundingBox ? r.boundingBox : {
-                                            x1: 0,
-                                            y1: 0,
-                                            w: t.width(),
-                                            h: t.height()
-                                        })
-                                    }, o = r.eles.components(), s = {}, l = 0; l < o.length; l++)
-                                    for (var u = o[l], c = 0; c < u.length; c++) s[u[c].id()] = l;
-                                for (l = 0; l < a.nodeSize; l++) {
-                                    var f = (g = i[l]).layoutDimensions(r);
-                                    (I = {}).isLocked = g.locked(), I.id = g.data("id"), I.parentId = g.data("parent"), I.cmptId = s[g.id()], I.children = [], I.positionX = g.position("x"), I.positionY = g.position("y"), I.offsetX = 0, I.offsetY = 0, I.height = f.w, I.width = f.h, I.maxX = I.positionX + I.width / 2, I.minX = I.positionX - I.width / 2, I.maxY = I.positionY + I.height / 2, I.minY = I.positionY - I.height / 2, I.padLeft = parseFloat(g.style("padding")), I.padRight = parseFloat(g.style("padding")), I.padTop = parseFloat(g.style("padding")), I.padBottom = parseFloat(g.style("padding")), I.nodeRepulsion = C(r.nodeRepulsion) ? r.nodeRepulsion(g) : r.nodeRepulsion, a.layoutNodes.push(I), a.idToIndex[I.id] = l
-                                }
-                                var h = [],
-                                    p = 0,
-                                    d = -1,
-                                    v = [];
-                                for (l = 0; l < a.nodeSize; l++) {
-                                    var g, y = (g = a.layoutNodes[l]).parentId;
-                                    null != y ? a.layoutNodes[a.idToIndex[y]].children.push(g.id) : (h[++d] = g.id, v.push(g.id))
-                                }
-                                for (a.graphSet.push(v); p <= d;) {
-                                    var m = h[p++],
-                                        x = a.idToIndex[m],
-                                        b = a.layoutNodes[x].children;
-                                    if (b.length > 0)
-                                        for (a.graphSet.push(b), l = 0; l < b.length; l++) h[++d] = b[l]
-                                }
-                                for (l = 0; l < a.graphSet.length; l++) {
-                                    var _ = a.graphSet[l];
-                                    for (c = 0; c < _.length; c++) {
-                                        var w = a.idToIndex[_[c]];
-                                        a.indexToGraph[w] = l
-                                    }
-                                }
-                                for (l = 0; l < a.edgeSize; l++) {
-                                    var k = n[l],
-                                        T = {};
-                                    T.id = k.data("id"), T.sourceId = k.data("source"), T.targetId = k.data("target");
-                                    var M = C(r.idealEdgeLength) ? r.idealEdgeLength(k) : r.idealEdgeLength,
-                                        A = C(r.edgeElasticity) ? r.edgeElasticity(k) : r.edgeElasticity,
-                                        S = a.idToIndex[T.sourceId],
-                                        E = a.idToIndex[T.targetId];
-                                    if (a.indexToGraph[S] != a.indexToGraph[E]) {
-                                        for (var L = Qa(T.sourceId, T.targetId, a), P = a.graphSet[L], O = 0, I = a.layoutNodes[S]; - 1 === P.indexOf(I.id);) I = a.layoutNodes[a.idToIndex[I.parentId]], O++;
-                                        for (I = a.layoutNodes[E]; - 1 === P.indexOf(I.id);) I = a.layoutNodes[a.idToIndex[I.parentId]], O++;
-                                        M *= O * r.nestingFactor
+                                        clientWidth: a.w,
+                                        clientHeight: a.h,
+                                        boundingBox: a
+                                    }, s = r.eles.components(), l = {}, u = 0; u < s.length; u++)
+                                    for (var c = s[u], f = 0; f < c.length; f++) l[c[f].id()] = u;
+                                for (u = 0; u < o.nodeSize; u++) {
+                                    var h = (y = i[u]).layoutDimensions(r);
+                                    (D = {}).isLocked = y.locked(), D.id = y.data("id"), D.parentId = y.data("parent"), D.cmptId = l[y.id()], D.children = [], D.positionX = y.position("x"), D.positionY = y.position("y"), D.offsetX = 0, D.offsetY = 0, D.height = h.w, D.width = h.h, D.maxX = D.positionX + D.width / 2, D.minX = D.positionX - D.width / 2, D.maxY = D.positionY + D.height / 2, D.minY = D.positionY - D.height / 2, D.padLeft = parseFloat(y.style("padding")), D.padRight = parseFloat(y.style("padding")), D.padTop = parseFloat(y.style("padding")), D.padBottom = parseFloat(y.style("padding")), D.nodeRepulsion = C(r.nodeRepulsion) ? r.nodeRepulsion(y) : r.nodeRepulsion, o.layoutNodes.push(D), o.idToIndex[D.id] = u
+                                }
+                                var p = [],
+                                    d = 0,
+                                    v = -1,
+                                    g = [];
+                                for (u = 0; u < o.nodeSize; u++) {
+                                    var y, m = (y = o.layoutNodes[u]).parentId;
+                                    null != m ? o.layoutNodes[o.idToIndex[m]].children.push(y.id) : (p[++v] = y.id, g.push(y.id))
+                                }
+                                for (o.graphSet.push(g); d <= v;) {
+                                    var x = p[d++],
+                                        b = o.idToIndex[x],
+                                        _ = o.layoutNodes[b].children;
+                                    if (_.length > 0)
+                                        for (o.graphSet.push(_), u = 0; u < _.length; u++) p[++v] = _[u]
+                                }
+                                for (u = 0; u < o.graphSet.length; u++) {
+                                    var w = o.graphSet[u];
+                                    for (f = 0; f < w.length; f++) {
+                                        var k = o.idToIndex[w[f]];
+                                        o.indexToGraph[k] = u
+                                    }
+                                }
+                                for (u = 0; u < o.edgeSize; u++) {
+                                    var T = n[u],
+                                        M = {};
+                                    M.id = T.data("id"), M.sourceId = T.data("source"), M.targetId = T.data("target");
+                                    var A = C(r.idealEdgeLength) ? r.idealEdgeLength(T) : r.idealEdgeLength,
+                                        S = C(r.edgeElasticity) ? r.edgeElasticity(T) : r.edgeElasticity,
+                                        E = o.idToIndex[M.sourceId],
+                                        L = o.idToIndex[M.targetId];
+                                    if (o.indexToGraph[E] != o.indexToGraph[L]) {
+                                        for (var P = Qa(M.sourceId, M.targetId, o), O = o.graphSet[P], I = 0, D = o.layoutNodes[E]; - 1 === O.indexOf(D.id);) D = o.layoutNodes[o.idToIndex[D.parentId]], I++;
+                                        for (D = o.layoutNodes[L]; - 1 === O.indexOf(D.id);) D = o.layoutNodes[o.idToIndex[D.parentId]], I++;
+                                        A *= I * r.nestingFactor
                                     }
-                                    T.idealLength = M, T.elasticity = A, a.layoutEdges.push(T)
+                                    M.idealLength = A, M.elasticity = S, o.layoutEdges.push(M)
                                 }
-                                return a
+                                return o
                             },
                             Qa = function(t, e, r) {
                                 var n = to(t, e, 0, r);
                                 return 2 > n.count ? 0 : n.graph
                             },
                             to = function t(e, r, n, i) {
                                 var a = i.graphSet[n];
@@ -17537,15 +17540,15 @@
                                     var n = new Array(20),
                                         i = Ne(5, 0),
                                         a = Ne(5, Math.PI / 5),
                                         o = .5 * (3 - Math.sqrt(5));
                                     o *= 1.57;
                                     for (var s = 0; s < a.length / 2; s++) a[2 * s] *= o, a[2 * s + 1] *= o;
                                     for (s = 0; s < 5; s++) n[4 * s] = i[2 * s], n[4 * s + 1] = i[2 * s + 1], n[4 * s + 2] = a[2 * s], n[4 * s + 3] = a[2 * s + 1];
-                                    n = Be(n), this.generatePolygon("star", n), this.generatePolygon("vee", [-1, -1, 0, -.333, 1, -1, 0, 1]), this.generatePolygon("rhomboid", [-1, -1, .333, -1, 1, 1, -.333, 1]), this.nodeShapes.concavehexagon = this.generatePolygon("concave-hexagon", [-1, -.95, -.75, 0, -1, .95, 1, .95, .75, 0, 1, -.95]);
+                                    n = Be(n), this.generatePolygon("star", n), this.generatePolygon("vee", [-1, -1, 0, -.333, 1, -1, 0, 1]), this.generatePolygon("rhomboid", [-1, -1, .333, -1, 1, 1, -.333, 1]), this.generatePolygon("right-rhomboid", [-.333, -1, 1, -1, .333, 1, -1, 1]), this.nodeShapes.concavehexagon = this.generatePolygon("concave-hexagon", [-1, -.95, -.75, 0, -1, .95, 1, .95, .75, 0, 1, -.95]);
                                     var l = [-1, -1, .25, -1, 1, 0, .25, 1, -1, 1];
                                     this.generatePolygon("tag", l), this.generateRoundPolygon("round-tag", l), t.makePolygon = function(t) {
                                         var r, n = "polygon-" + t.join("$");
                                         return (r = this[n]) ? r : e.generatePolygon(n, t)
                                     }
                                 }
                             },
@@ -17605,15 +17608,15 @@
                                 var n = _.document,
                                     i = n.head,
                                     a = "__________cytoscape_stylesheet",
                                     o = "__________cytoscape_container",
                                     s = null != n.getElementById(a);
                                 if (r.className.indexOf(o) < 0 && (r.className = (r.className || "") + " " + o), !s) {
                                     var l = n.createElement("style");
-                                    l.id = a, l.innerHTML = "." + o + " { position: relative; }", i.insertBefore(l, i.children[0])
+                                    l.id = a, l.textContent = "." + o + " { position: relative; }", i.insertBefore(l, i.children[0])
                                 }
                                 "static" === _.getComputedStyle(r).getPropertyValue("position") && St("A Cytoscape container has style position:static and so can not use UI extensions properly")
                             }
                             e.selection = [void 0, void 0, void 0, void 0, 0], e.bezierProjPcts = [.05, .225, .4, .5, .6, .775, .95], e.hoverData = {
                                 down: null,
                                 last: null,
                                 downTime: null,
@@ -19745,15 +19748,15 @@
                             return void 0 === t && (t = {}), P(t) ? new Ba(t) : E(t) ? Js.apply(Js, arguments) : void 0
                         };
                         tl.use = function(t) {
                             var e = Array.prototype.slice.call(arguments, 1);
                             return e.unshift(tl), t.apply(null, e), this
                         }, tl.warnings = function(t) {
                             return At(t)
-                        }, tl.version = "3.24.0", tl.stylesheet = tl.Stylesheet = $s, t.exports = tl
+                        }, tl.version = "3.25.0", tl.stylesheet = tl.Stylesheet = $s, t.exports = tl
                     },
                     4485: (t, e, r) => {
                         t.exports = r(2894)
                     },
                     2894: function(t, e) {
                         var r, n, i;
                         (function() {
@@ -30602,15 +30605,15 @@
                                             g = r(30477),
                                             y = r(21459),
                                             m = r(42359),
                                             x = r(51873).clearOutline,
                                             b = r(60165),
                                             _ = b.handleEllipse,
                                             w = b.readPaths,
-                                            k = r(90551),
+                                            k = r(90551).newShapes,
                                             T = r(35855),
                                             M = r(32485).activateLastSelection,
                                             A = r(71828),
                                             S = A.sorterAsc,
                                             E = r(61082),
                                             C = r(79990),
                                             L = r(41675).getFromId,
@@ -31131,46 +31134,53 @@
                                                     yt = vt._length,
                                                     mt = gt._length,
                                                     xt = t.altKey && !(p(i) && y);
                                                 Y(t, T, n), c && (H = z([
                                                     [F, B]
                                                 ], I.BENDPX));
                                                 var bt = E.selectAll("path.select-outline-" + P.id).data([1]),
-                                                    _t = x ? M.newshape : M.newselection,
-                                                    wt = x && !y ? _t.fillcolor : "rgba(0,0,0,0)",
+                                                    _t = x ? M.newshape : M.newselection;
+                                                x && (n.hasText = _t.label.text || _t.label.texttemplate);
+                                                var wt = x && !y ? _t.fillcolor : "rgba(0,0,0,0)",
                                                     kt = _t.line.color || (u ? s.contrast(T._fullLayout.plot_bgcolor) : "#7f7f7f");
                                                 bt.enter().append("path").attr("class", "select-outline select-outline-" + P.id).style({
                                                     opacity: x ? _t.opacity / 2 : 1,
                                                     "stroke-dasharray": o(_t.line.dash, _t.line.width),
                                                     "stroke-width": _t.line.width + "px",
                                                     "shape-rendering": "crispEdges"
                                                 }).call(s.stroke, kt).call(s.fill, wt).attr("fill-rule", "evenodd").classed("cursor-move", !!x).attr("transform", O).attr("d", dt + "Z");
                                                 var Tt = E.append("path").attr("class", "zoombox-corners").style({
-                                                        fill: s.background,
-                                                        stroke: s.defaultLine,
-                                                        "stroke-width": 1
-                                                    }).attr("transform", O).attr("d", "M0,0Z"),
-                                                    Mt = M._uid + I.SELECTID,
-                                                    At = [],
-                                                    St = X(T, n.xaxes, n.yaxes, n.subplot);
+                                                    fill: s.background,
+                                                    stroke: s.defaultLine,
+                                                    "stroke-width": 1
+                                                }).attr("transform", O).attr("d", "M0,0Z");
+                                                if (x && n.hasText) {
+                                                    var Mt = E.select(".label-temp");
+                                                    Mt.empty() && (Mt = E.append("g").classed("label-temp", !0).classed("select-outline", !0).style({
+                                                        opacity: .8
+                                                    }))
+                                                }
+                                                var At = M._uid + I.SELECTID,
+                                                    St = [],
+                                                    Et = X(T, n.xaxes, n.yaxes, n.subplot);
                                                 S && !t.shiftKey && (n._clearSubplotSelections = function() {
                                                     if (u) {
                                                         var t = vt._id,
                                                             e = gt._id;
-                                                        it(T, t, e, St);
+                                                        it(T, t, e, Et);
                                                         for (var r = (T.layout || {}).selections || [], n = [], i = !1, o = 0; o < r.length; o++) {
                                                             var s = M.selections[o];
                                                             s.xref !== t || s.yref !== e ? n.push(r[o]) : i = !0
                                                         }
                                                         i && (T._fullLayout._noEmitSelectedAtStart = !0, a.call("_guiRelayout", T, {
                                                             selections: n
                                                         }))
                                                     }
                                                 });
-                                                var Et = function(t) {
+                                                var Ct = function(t) {
                                                     return t.plotinfo.fillRangeItems || ct(t.xaxes.concat(t.yaxes))
                                                 }(n);
                                                 n.moveFn = function(t, e) {
                                                     n._clearSubplotSelections && (n._clearSubplotSelections(), n._clearSubplotSelections = void 0), lt = Math.max(0, Math.min(yt, ot * t + F)), pt = Math.max(0, Math.min(mt, st * e + B));
                                                     var r = Math.abs(lt - F),
                                                         i = Math.abs(pt - B);
                                                     if (g) {
@@ -31214,38 +31224,38 @@
                                                             [lt, pt],
                                                             [lt, B]
                                                         ]).xmin = Math.min(F, lt), K.xmax = Math.max(F, lt), K.ymin = Math.min(B, pt), K.ymax = Math.max(B, pt), Tt.attr("d", "M0,0Z"))
                                                     } else c && (H.addPt([lt, pt]), K = H.filtered);
                                                     if (n.selectionDefs && n.selectionDefs.length ? (Z = Q(n.mergedPolygons, K, xt), K.subtract = xt, q = G(n.selectionDefs.concat([K]))) : (Z = [K], q = R(K)), m(et(Z, y), bt, n), b) {
                                                         var u, f = nt(T, !1),
                                                             h = f.eventData ? f.eventData.points.slice() : [];
-                                                        f = nt(T, !1, q, St, n), q = f.selectionTesters, at = f.eventData, u = H ? H.filtered : ut(Z), C.throttle(Mt, I.SELECTDELAY, (function() {
-                                                            for (var t = (At = rt(q, St)).slice(), e = 0; e < h.length; e++) {
+                                                        f = nt(T, !1, q, Et, n), q = f.selectionTesters, at = f.eventData, u = H ? H.filtered : ut(Z), C.throttle(At, I.SELECTDELAY, (function() {
+                                                            for (var t = (St = rt(q, Et)).slice(), e = 0; e < h.length; e++) {
                                                                 for (var r = h[e], n = !1, i = 0; i < t.length; i++)
                                                                     if (t[i].curveNumber === r.curveNumber && t[i].pointNumber === r.pointNumber) {
                                                                         n = !0;
                                                                         break
                                                                     } n || t.push(r)
                                                             }
-                                                            t.length && (at || (at = {}), at.points = t), Et(at, u),
+                                                            t.length && (at || (at = {}), at.points = t), Ct(at, u),
                                                                 function(t, e) {
                                                                     t.emit("plotly_selecting", e)
                                                                 }(T, at)
                                                         }))
                                                     }
                                                 }, n.clickFn = function(t, e) {
                                                     if (Tt.remove(), T._fullLayout._activeShapeIndex >= 0) T._fullLayout._deactivateShape(T);
                                                     else if (!x) {
                                                         var r = M.clickmode;
-                                                        C.done(Mt).then((function() {
-                                                            if (C.clear(Mt), 2 === t) {
-                                                                for (bt.remove(), J = 0; J < St.length; J++)(tt = St[J])._module.selectPoints(tt, !1);
-                                                                if ($(T, St), W(n), ht(T), St.length) {
-                                                                    var i = St[0].xaxis,
-                                                                        o = St[0].yaxis;
+                                                        C.done(At).then((function() {
+                                                            if (C.clear(At), 2 === t) {
+                                                                for (bt.remove(), J = 0; J < Et.length; J++)(tt = Et[J])._module.selectPoints(tt, !1);
+                                                                if ($(T, Et), W(n), ht(T), Et.length) {
+                                                                    var i = Et[0].xaxis,
+                                                                        o = Et[0].yaxis;
                                                                     if (i && o) {
                                                                         for (var s = [], u = T._fullLayout.selections, c = 0; c < u.length; c++) {
                                                                             var f = u[c];
                                                                             f && (f.xref === i._id && f.yref === o._id || s.push(f))
                                                                         }
                                                                         s.length < u.length && (T._fullLayout._noEmitSelectedAtStart = !0, a.call("_guiRelayout", T, {
                                                                             selections: s
@@ -31253,16 +31263,16 @@
                                                                     }
                                                                 }
                                                             } else r.indexOf("select") > -1 && V(e, T, n.xaxes, n.yaxes, n.subplot, n, bt), "event" === r && ft(T, void 0);
                                                             l.click(T, e)
                                                         })).catch(A.error)
                                                     }
                                                 }, n.doneFn = function() {
-                                                    Tt.remove(), C.done(Mt).then((function() {
-                                                        C.clear(Mt), !S && K && n.selectionDefs && (K.subtract = xt, n.selectionDefs.push(K), n.mergedPolygons.length = 0, [].push.apply(n.mergedPolygons, Z)), (S || x) && W(n, S), n.doneFnCompleted && n.doneFnCompleted(At), b && ft(T, at)
+                                                    Tt.remove(), C.done(At).then((function() {
+                                                        C.clear(At), !S && K && n.selectionDefs && (K.subtract = xt, n.selectionDefs.push(K), n.mergedPolygons.length = 0, [].push.apply(n.mergedPolygons, Z)), (S || x) && W(n, S), n.doneFnCompleted && n.doneFnCompleted(St), b && ft(T, at)
                                                     })).catch(A.error)
                                                 }
                                             },
                                             clearOutline: x,
                                             clearSelectionsCache: W,
                                             selectOnClick: V
                                         }
@@ -31625,14 +31635,126 @@
                                         t.exports = function(t, e) {
                                             a(t, e, {
                                                 name: "shapes",
                                                 handleItemDefaults: l
                                             })
                                         }
                                     },
+                                    48100: function(t, e, r) {
+                                        "use strict";
+                                        var n = r(71828),
+                                            i = r(89298),
+                                            a = r(63893),
+                                            o = r(91424),
+                                            s = r(60165).readPaths,
+                                            l = r(30477),
+                                            u = l.getPathString,
+                                            c = r(37281),
+                                            f = r(18783).FROM_TL;
+                                        t.exports = function(t, e, r, h) {
+                                            if (h.selectAll(".shape-label").remove(), r.label.text || r.label.texttemplate) {
+                                                var p;
+                                                if (r.label.texttemplate) {
+                                                    var d = {};
+                                                    if ("path" !== r.type) {
+                                                        var v = i.getFromId(t, r.xref),
+                                                            g = i.getFromId(t, r.yref);
+                                                        for (var y in c) {
+                                                            var m = c[y](r, v, g);
+                                                            void 0 !== m && (d[y] = m)
+                                                        }
+                                                    }
+                                                    p = n.texttemplateStringForShapes(r.label.texttemplate, {}, t._fullLayout._d3locale, d)
+                                                } else p = r.label.text;
+                                                var x, b, _, w, k = {
+                                                        "data-index": e
+                                                    },
+                                                    T = r.label.font,
+                                                    M = h.append("g").attr(k).classed("shape-label", !0).append("text").attr({
+                                                        "data-notex": 1
+                                                    }).classed("shape-label-text", !0).text(p);
+                                                if (r.path) {
+                                                    var A = u(t, r),
+                                                        S = s(A, t);
+                                                    x = 1 / 0, _ = 1 / 0, b = -1 / 0, w = -1 / 0;
+                                                    for (var E = 0; E < S.length; E++)
+                                                        for (var C = 0; C < S[E].length; C++)
+                                                            for (var L = S[E][C], P = 1; P < L.length; P += 2) {
+                                                                var O = L[P],
+                                                                    I = L[P + 1];
+                                                                x = Math.min(x, O), b = Math.max(b, O), _ = Math.min(_, I), w = Math.max(w, I)
+                                                            }
+                                                } else {
+                                                    var D = i.getFromId(t, r.xref),
+                                                        z = i.getRefType(r.xref),
+                                                        R = i.getFromId(t, r.yref),
+                                                        F = i.getRefType(r.yref),
+                                                        B = l.getDataToPixel(t, D, !1, z),
+                                                        N = l.getDataToPixel(t, R, !0, F);
+                                                    x = B(r.x0), b = B(r.x1), _ = N(r.y0), w = N(r.y1)
+                                                }
+                                                var j = r.label.textangle;
+                                                "auto" === j && (j = "line" === r.type ? function(t, e, r, n) {
+                                                    var i, a;
+                                                    return a = Math.abs(r - t), i = r >= t ? e - n : n - e, -180 / Math.PI * Math.atan2(i, a)
+                                                }(x, _, b, w) : 0), M.call((function(e) {
+                                                    return e.call(o.font, T).attr({}), a.convertToTspans(e, t), e
+                                                }));
+                                                var U = function(t, e, r, n, i, a, o) {
+                                                        var s, l, u, c, h = i.label.textposition,
+                                                            p = i.label.textangle,
+                                                            d = i.label.padding,
+                                                            v = i.type,
+                                                            g = Math.PI / 180 * a,
+                                                            y = Math.sin(g),
+                                                            m = Math.cos(g),
+                                                            x = i.label.xanchor,
+                                                            b = i.label.yanchor;
+                                                        if ("line" === v) {
+                                                            "start" === h ? (s = t, l = e) : "end" === h ? (s = r, l = n) : (s = (t + r) / 2, l = (e + n) / 2), "auto" === x && (x = "start" === h ? "auto" === p ? r > t ? "left" : r < t ? "right" : "center" : r > t ? "right" : r < t ? "left" : "center" : "end" === h ? "auto" === p ? r > t ? "right" : r < t ? "left" : "center" : r > t ? "left" : r < t ? "right" : "center" : "center");
+                                                            var _ = {
+                                                                bottom: -1,
+                                                                middle: 0,
+                                                                top: 1
+                                                            };
+                                                            if ("auto" === p) {
+                                                                var w = _[b];
+                                                                u = -d * y * w, c = d * m * w
+                                                            } else u = d * {
+                                                                left: 1,
+                                                                center: 0,
+                                                                right: -1
+                                                            } [x], c = d * _[b];
+                                                            s += u, l += c
+                                                        } else u = d + 3, -1 !== h.indexOf("right") ? (s = Math.max(t, r) - u, "auto" === x && (x = "right")) : -1 !== h.indexOf("left") ? (s = Math.min(t, r) + u, "auto" === x && (x = "left")) : (s = (t + r) / 2, "auto" === x && (x = "center")), l = -1 !== h.indexOf("top") ? Math.min(e, n) : -1 !== h.indexOf("bottom") ? Math.max(e, n) : (e + n) / 2, c = d, "bottom" === b ? l -= c : "top" === b && (l += c);
+                                                        var k = f[b],
+                                                            T = i.label.font.size,
+                                                            M = o.height;
+                                                        return {
+                                                            textx: s + (M * k - T) * y,
+                                                            texty: l + -(M * k - T) * m,
+                                                            xanchor: x
+                                                        }
+                                                    }(x, _, b, w, r, j, o.bBox(M.node())),
+                                                    V = U.textx,
+                                                    H = U.texty,
+                                                    q = U.xanchor;
+                                                M.attr({
+                                                    "text-anchor": {
+                                                        left: "start",
+                                                        center: "middle",
+                                                        right: "end"
+                                                    } [q],
+                                                    y: H,
+                                                    x: V,
+                                                    transform: "rotate(" + j + "," + V + "," + H + ")"
+                                                }).call(a.positionText, V, H)
+                                            }
+                                        }
+                                    },
                                     42359: function(t, e, r) {
                                         "use strict";
                                         var n = r(71828).strTranslate,
                                             i = r(28569),
                                             a = r(64505),
                                             o = a.drawMode,
                                             s = a.selectMode,
@@ -31644,103 +31766,165 @@
                                             p = c.i180,
                                             d = c.i270,
                                             v = r(51873).clearOutlineControllers,
                                             g = r(60165),
                                             y = g.pointsOnRectangle,
                                             m = g.pointsOnEllipse,
                                             x = g.writePaths,
-                                            b = r(90551),
-                                            _ = r(35855);
+                                            b = r(90551).newShapes,
+                                            _ = r(90551).createShapeObj,
+                                            w = r(35855),
+                                            k = r(48100);
 
-                                        function w(t, e) {
+                                        function T(t, e) {
                                             var r, n, i, a = t[e][1],
                                                 o = t[e][2],
                                                 s = t.length;
                                             return n = t[r = (e + 1) % s][1], i = t[r][2], n === a && i === o && (n = t[r = (e + 2) % s][1], i = t[r][2]), [r, n, i]
                                         }
                                         t.exports = function t(e, r, a, c) {
                                             c || (c = 0);
                                             var g = a.gd;
 
-                                            function k() {
-                                                t(e, r, a, c++), (m(e[0]) || a.hasText) && T({
+                                            function M() {
+                                                t(e, r, a, c++), (m(e[0]) || a.hasText) && A({
                                                     redrawing: !0
                                                 })
                                             }
 
-                                            function T(t) {
+                                            function A(t) {
                                                 var e = {};
-                                                void 0 !== a.isActiveShape && (a.isActiveShape = !1, e = b(r, a)), void 0 !== a.isActiveSelection && (a.isActiveSelection = !1, e = _(r, a), g._fullLayout._reselect = !0), Object.keys(e).length && l.call((t || {}).redrawing ? "relayout" : "_guiRelayout", g, e)
+                                                void 0 !== a.isActiveShape && (a.isActiveShape = !1, e = b(r, a)), void 0 !== a.isActiveSelection && (a.isActiveSelection = !1, e = w(r, a), g._fullLayout._reselect = !0), Object.keys(e).length && l.call((t || {}).redrawing ? "relayout" : "_guiRelayout", g, e)
+                                            }
+                                            var S, E, C, L, P, O = g._fullLayout._zoomlayer,
+                                                I = a.dragmode,
+                                                D = o(I),
+                                                z = s(I);
+                                            if ((D || z) && (g._fullLayout._outlining = !0), v(g), r.attr("d", x(e)), c || !a.isActiveShape && !a.isActiveSelection || (P = function(t, e) {
+                                                    for (var r = 0; r < e.length; r++) {
+                                                        var n = e[r];
+                                                        t[r] = [];
+                                                        for (var i = 0; i < n.length; i++) {
+                                                            t[r][i] = [];
+                                                            for (var a = 0; a < n[i].length; a++) t[r][i][a] = n[i][a]
+                                                        }
+                                                    }
+                                                    return t
+                                                }([], e), function(t) {
+                                                    S = [];
+                                                    for (var r = 0; r < e.length; r++) {
+                                                        var o = e[r],
+                                                            s = y(o),
+                                                            l = !s && m(o);
+                                                        S[r] = [];
+                                                        for (var c = o.length, v = 0; v < c; v++)
+                                                            if ("Z" !== o[v][0] && (!l || v === f || v === h || v === p || v === d)) {
+                                                                var x, b = s && a.isActiveSelection;
+                                                                b && (x = T(o, v));
+                                                                var _ = o[v][1],
+                                                                    w = o[v][2],
+                                                                    k = t.append(b ? "rect" : "circle").attr("data-i", r).attr("data-j", v).style({
+                                                                        fill: u.background,
+                                                                        stroke: u.defaultLine,
+                                                                        "stroke-width": 1,
+                                                                        "shape-rendering": "crispEdges"
+                                                                    });
+                                                                if (b) {
+                                                                    var M = x[1] - _,
+                                                                        A = x[2] - w,
+                                                                        E = A ? 5 : Math.max(Math.min(25, Math.abs(M) - 5), 5),
+                                                                        C = M ? 5 : Math.max(Math.min(25, Math.abs(A) - 5), 5);
+                                                                    k.classed(A ? "cursor-ew-resize" : "cursor-ns-resize", !0).attr("width", E).attr("height", C).attr("x", _ - E / 2).attr("y", w - C / 2).attr("transform", n(M / 2, A / 2))
+                                                                } else k.classed("cursor-grab", !0).attr("r", 5).attr("cx", _).attr("cy", w);
+                                                                S[r][v] = {
+                                                                    element: k.node(),
+                                                                    gd: g,
+                                                                    prepFn: B,
+                                                                    doneFn: j,
+                                                                    clickFn: U
+                                                                }, i.init(S[r][v])
+                                                            }
+                                                    }
+                                                }(O.append("g").attr("class", "outline-controllers")), function() {
+                                                    if (E = [], e.length) {
+                                                        E[0] = {
+                                                            element: r[0][0],
+                                                            gd: g,
+                                                            prepFn: H,
+                                                            doneFn: q,
+                                                            clickFn: G
+                                                        }, i.init(E[0])
+                                                    }
+                                                }()), D && a.hasText) {
+                                                var R = O.select(".label-temp"),
+                                                    F = _(r, a, a.dragmode);
+                                                k(g, "label-temp", F, R)
                                             }
-                                            var M, A, S, E, C, L = g._fullLayout._zoomlayer,
-                                                P = a.dragmode,
-                                                O = o(P),
-                                                I = s(P);
 
-                                            function D(t) {
-                                                S = +t.srcElement.getAttribute("data-i"), E = +t.srcElement.getAttribute("data-j"), M[S][E].moveFn = z
+                                            function B(t) {
+                                                C = +t.srcElement.getAttribute("data-i"), L = +t.srcElement.getAttribute("data-j"), S[C][L].moveFn = N
                                             }
 
-                                            function z(t, r) {
+                                            function N(t, r) {
                                                 if (e.length) {
-                                                    var n = C[S][E][1],
-                                                        i = C[S][E][2],
-                                                        o = e[S],
+                                                    var n = P[C][L][1],
+                                                        i = P[C][L][2],
+                                                        o = e[C],
                                                         s = o.length;
                                                     if (y(o)) {
                                                         var l = t,
                                                             u = r;
-                                                        a.isActiveSelection && (w(o, E)[1] === o[E][1] ? u = 0 : l = 0);
+                                                        a.isActiveSelection && (T(o, L)[1] === o[L][1] ? u = 0 : l = 0);
                                                         for (var c = 0; c < s; c++)
-                                                            if (c !== E) {
+                                                            if (c !== L) {
                                                                 var f = o[c];
-                                                                f[1] === o[E][1] && (f[1] = n + l), f[2] === o[E][2] && (f[2] = i + u)
-                                                            } if (o[E][1] = n + l, o[E][2] = i + u, !y(o))
+                                                                f[1] === o[L][1] && (f[1] = n + l), f[2] === o[L][2] && (f[2] = i + u)
+                                                            } if (o[L][1] = n + l, o[L][2] = i + u, !y(o))
                                                             for (var h = 0; h < s; h++)
-                                                                for (var p = 0; p < o[h].length; p++) o[h][p] = C[S][h][p]
-                                                    } else o[E][1] = n + t, o[E][2] = i + r;
-                                                    k()
+                                                                for (var p = 0; p < o[h].length; p++) o[h][p] = P[C][h][p]
+                                                    } else o[L][1] = n + t, o[L][2] = i + r;
+                                                    M()
                                                 }
                                             }
 
-                                            function R() {
-                                                T()
+                                            function j() {
+                                                A()
                                             }
 
-                                            function F(t, r) {
+                                            function U(t, r) {
                                                 if (2 === t) {
-                                                    S = +r.srcElement.getAttribute("data-i"), E = +r.srcElement.getAttribute("data-j");
-                                                    var n = e[S];
+                                                    C = +r.srcElement.getAttribute("data-i"), L = +r.srcElement.getAttribute("data-j");
+                                                    var n = e[C];
                                                     y(n) || m(n) || function() {
-                                                        if (e.length && e[S] && e[S].length) {
-                                                            for (var t = [], r = 0; r < e[S].length; r++) r !== E && t.push(e[S][r]);
-                                                            t.length > 1 && (2 !== t.length || "Z" !== t[1][0]) && (0 === E && (t[0][0] = "M"), e[S] = t, k(), T())
+                                                        if (e.length && e[C] && e[C].length) {
+                                                            for (var t = [], r = 0; r < e[C].length; r++) r !== L && t.push(e[C][r]);
+                                                            t.length > 1 && (2 !== t.length || "Z" !== t[1][0]) && (0 === L && (t[0][0] = "M"), e[C] = t, M(), A())
                                                         }
                                                     }()
                                                 }
                                             }
 
-                                            function B(t, r) {
+                                            function V(t, r) {
                                                 ! function(t, r) {
                                                     if (e.length)
                                                         for (var n = 0; n < e.length; n++)
                                                             for (var i = 0; i < e[n].length; i++)
-                                                                for (var a = 0; a + 2 < e[n][i].length; a += 2) e[n][i][a + 1] = C[n][i][a + 1] + t, e[n][i][a + 2] = C[n][i][a + 2] + r
-                                                }(t, r), k()
+                                                                for (var a = 0; a + 2 < e[n][i].length; a += 2) e[n][i][a + 1] = P[n][i][a + 1] + t, e[n][i][a + 2] = P[n][i][a + 2] + r
+                                                }(t, r), M()
                                             }
 
-                                            function N(t) {
-                                                (S = +t.srcElement.getAttribute("data-i")) || (S = 0), A[S].moveFn = B
+                                            function H(t) {
+                                                (C = +t.srcElement.getAttribute("data-i")) || (C = 0), E[C].moveFn = V
                                             }
 
-                                            function j() {
-                                                T()
+                                            function q() {
+                                                A()
                                             }
 
-                                            function U(t) {
+                                            function G(t) {
                                                 2 === t && function(t) {
                                                     if (s(t._fullLayout.dragmode)) {
                                                         v(t);
                                                         var e = t._fullLayout._activeSelectionIndex,
                                                             r = (t.layout || {}).selections || [];
                                                         if (e < r.length) {
                                                             for (var n = [], i = 0; i < r.length; i++) i !== e && n.push(r[i]);
@@ -31751,158 +31935,101 @@
                                                                 yref: a.yref
                                                             }, l.call("_guiRelayout", t, {
                                                                 selections: n
                                                             })
                                                         }
                                                     }
                                                 }(g)
-                                            }(O || I) && (g._fullLayout._outlining = !0), v(g), r.attr("d", x(e)), c || !a.isActiveShape && !a.isActiveSelection || (C = function(t, e) {
-                                                for (var r = 0; r < e.length; r++) {
-                                                    var n = e[r];
-                                                    t[r] = [];
-                                                    for (var i = 0; i < n.length; i++) {
-                                                        t[r][i] = [];
-                                                        for (var a = 0; a < n[i].length; a++) t[r][i][a] = n[i][a]
-                                                    }
-                                                }
-                                                return t
-                                            }([], e), function(t) {
-                                                M = [];
-                                                for (var r = 0; r < e.length; r++) {
-                                                    var o = e[r],
-                                                        s = y(o),
-                                                        l = !s && m(o);
-                                                    M[r] = [];
-                                                    for (var c = o.length, v = 0; v < c; v++)
-                                                        if ("Z" !== o[v][0] && (!l || v === f || v === h || v === p || v === d)) {
-                                                            var x, b = s && a.isActiveSelection;
-                                                            b && (x = w(o, v));
-                                                            var _ = o[v][1],
-                                                                k = o[v][2],
-                                                                T = t.append(b ? "rect" : "circle").attr("data-i", r).attr("data-j", v).style({
-                                                                    fill: u.background,
-                                                                    stroke: u.defaultLine,
-                                                                    "stroke-width": 1,
-                                                                    "shape-rendering": "crispEdges"
-                                                                });
-                                                            if (b) {
-                                                                var A = x[1] - _,
-                                                                    S = x[2] - k,
-                                                                    E = S ? 5 : Math.max(Math.min(25, Math.abs(A) - 5), 5),
-                                                                    C = A ? 5 : Math.max(Math.min(25, Math.abs(S) - 5), 5);
-                                                                T.classed(S ? "cursor-ew-resize" : "cursor-ns-resize", !0).attr("width", E).attr("height", C).attr("x", _ - E / 2).attr("y", k - C / 2).attr("transform", n(A / 2, S / 2))
-                                                            } else T.classed("cursor-grab", !0).attr("r", 5).attr("cx", _).attr("cy", k);
-                                                            M[r][v] = {
-                                                                element: T.node(),
-                                                                gd: g,
-                                                                prepFn: D,
-                                                                doneFn: R,
-                                                                clickFn: F
-                                                            }, i.init(M[r][v])
-                                                        }
-                                                }
-                                            }(L.append("g").attr("class", "outline-controllers")), function() {
-                                                if (A = [], e.length) {
-                                                    A[0] = {
-                                                        element: r[0][0],
-                                                        gd: g,
-                                                        prepFn: N,
-                                                        doneFn: j,
-                                                        clickFn: U
-                                                    }, i.init(A[0])
-                                                }
-                                            }())
+                                            }
                                         }
                                     },
                                     34031: function(t, e, r) {
                                         "use strict";
                                         var n = r(39898),
                                             i = r(73972),
                                             a = r(71828),
                                             o = r(89298),
                                             s = r(60165).readPaths,
                                             l = r(42359),
-                                            u = r(51873).clearOutlineControllers,
-                                            c = r(7901),
-                                            f = r(91424),
-                                            h = r(44467).arrayEditor,
-                                            p = r(28569),
-                                            d = r(6964),
-                                            v = r(63893),
+                                            u = r(48100),
+                                            c = r(51873).clearOutlineControllers,
+                                            f = r(7901),
+                                            h = r(91424),
+                                            p = r(44467).arrayEditor,
+                                            d = r(28569),
+                                            v = r(6964),
                                             g = r(21459),
                                             y = r(30477),
-                                            m = y.getPathString,
-                                            x = r(37281),
-                                            b = r(18783).FROM_TL;
+                                            m = y.getPathString;
 
-                                        function _(t) {
+                                        function x(t) {
                                             var e = t._fullLayout;
                                             for (var r in e._shapeUpperLayer.selectAll("path").remove(), e._shapeLowerLayer.selectAll("path").remove(), e._shapeUpperLayer.selectAll("text").remove(), e._shapeLowerLayer.selectAll("text").remove(), e._plots) {
                                                 var n = e._plots[r].shapelayer;
                                                 n && (n.selectAll("path").remove(), n.selectAll("text").remove())
                                             }
-                                            for (var i = 0; i < e.shapes.length; i++) e.shapes[i].visible && T(t, i)
+                                            for (var i = 0; i < e.shapes.length; i++) e.shapes[i].visible && w(t, i)
                                         }
 
-                                        function w(t) {
+                                        function b(t) {
                                             return !!t._fullLayout._outlining
                                         }
 
-                                        function k(t) {
+                                        function _(t) {
                                             return !t._context.edits.shapePosition
                                         }
 
-                                        function T(t, e) {
+                                        function w(t, e) {
                                             t._fullLayout._paperdiv.selectAll('.shapelayer [data-index="' + e + '"]').remove();
                                             var r = y.makeShapesOptionsAndPlotinfo(t, e),
-                                                u = r.options,
-                                                v = r.plotinfo;
+                                                c = r.options,
+                                                w = r.plotinfo;
 
-                                            function x(r) {
-                                                var x = m(t, u),
-                                                    b = {
+                                            function A(r) {
+                                                var A = m(t, c),
+                                                    S = {
                                                         "data-index": e,
-                                                        "fill-rule": u.fillrule,
-                                                        d: x
+                                                        "fill-rule": c.fillrule,
+                                                        d: A
                                                     },
-                                                    T = u.opacity,
-                                                    C = u.fillcolor,
-                                                    L = u.line.width ? u.line.color : "rgba(0,0,0,0)",
-                                                    P = u.line.width,
-                                                    O = u.line.dash;
-                                                P || !0 !== u.editable || (P = 5, O = "solid");
-                                                var I = "Z" !== x[x.length - 1],
-                                                    D = k(t) && u.editable && t._fullLayout._activeShapeIndex === e;
-                                                D && (C = I ? "rgba(0,0,0,0)" : t._fullLayout.activeshape.fillcolor, T = t._fullLayout.activeshape.opacity);
+                                                    E = c.opacity,
+                                                    C = c.fillcolor,
+                                                    L = c.line.width ? c.line.color : "rgba(0,0,0,0)",
+                                                    P = c.line.width,
+                                                    O = c.line.dash;
+                                                P || !0 !== c.editable || (P = 5, O = "solid");
+                                                var I = "Z" !== A[A.length - 1],
+                                                    D = _(t) && c.editable && t._fullLayout._activeShapeIndex === e;
+                                                D && (C = I ? "rgba(0,0,0,0)" : t._fullLayout.activeshape.fillcolor, E = t._fullLayout.activeshape.opacity);
                                                 var z, R = r.append("g").classed("shape-group", !0).attr({
                                                         "data-index": e
                                                     }),
-                                                    F = R.append("path").attr(b).style("opacity", T).call(c.stroke, L).call(c.fill, C).call(f.dashLine, O, P);
-                                                if (M(R, t, u), A(t, e, u, R), (D || t._context.edits.shapePosition) && (z = h(t.layout, "shapes", u)), D) {
+                                                    F = R.append("path").attr(S).style("opacity", E).call(f.stroke, L).call(f.fill, C).call(h.dashLine, O, P);
+                                                if (k(R, t, c), u(t, e, c, R), (D || t._context.edits.shapePosition) && (z = p(t.layout, "shapes", c)), D) {
                                                     F.style({
                                                         cursor: "move"
                                                     });
                                                     var B = {
                                                             element: F.node(),
-                                                            plotinfo: v,
+                                                            plotinfo: w,
                                                             gd: t,
                                                             editHelpers: z,
-                                                            hasText: u.label.text || u.label.texttemplate,
+                                                            hasText: c.label.text || c.label.texttemplate,
                                                             isActiveShape: !0
                                                         },
-                                                        N = s(x, t);
+                                                        N = s(A, t);
                                                     l(N, F, B)
-                                                } else t._context.edits.shapePosition ? function(t, e, r, s, l, u) {
-                                                    var c, h, v, x, b, _, k, T, E, C, L, P, O, I, D, z, R = 10,
+                                                } else t._context.edits.shapePosition ? function(t, e, r, s, l, c) {
+                                                    var f, p, x, _, w, M, A, S, E, C, L, P, O, I, D, z, R = 10,
                                                         F = 10,
                                                         B = "pixel" === r.xsizemode,
                                                         N = "pixel" === r.ysizemode,
                                                         j = "line" === r.type,
                                                         U = "path" === r.type,
-                                                        V = u.modifyItem,
+                                                        V = c.modifyItem,
                                                         H = n.select(e.node().parentNode),
                                                         q = o.getFromId(t, r.xref),
                                                         G = o.getRefType(r.xref),
                                                         Y = o.getFromId(t, r.yref),
                                                         W = o.getRefType(r.yref),
                                                         Z = y.getDataToPixel(t, q, !1, G),
                                                         X = y.getDataToPixel(t, Y, !0, W),
@@ -31933,98 +32060,98 @@
                                                                 r: o
                                                             }).style(a).classed("cursor-grab", !0), i
                                                         }() : e,
                                                         Q = {
                                                             element: $.node(),
                                                             gd: t,
                                                             prepFn: function(n) {
-                                                                w(t) || (B && (b = Z(r.xanchor)), N && (_ = X(r.yanchor)), "path" === r.type ? D = r.path : (c = B ? r.x0 : Z(r.x0), h = N ? r.y0 : X(r.y0), v = B ? r.x1 : Z(r.x1), x = N ? r.y1 : X(r.y1)), c < v ? (E = c, O = "x0", C = v, I = "x1") : (E = v, O = "x1", C = c, I = "x0"), !N && h < x || N && h > x ? (k = h, L = "y0", T = x, P = "y1") : (k = x, L = "y1", T = h, P = "y0"), tt(n), nt(l, r), function(t, e, r) {
+                                                                b(t) || (B && (w = Z(r.xanchor)), N && (M = X(r.yanchor)), "path" === r.type ? D = r.path : (f = B ? r.x0 : Z(r.x0), p = N ? r.y0 : X(r.y0), x = B ? r.x1 : Z(r.x1), _ = N ? r.y1 : X(r.y1)), f < x ? (E = f, O = "x0", C = x, I = "x1") : (E = x, O = "x1", C = f, I = "x0"), !N && p < _ || N && p > _ ? (A = p, L = "y0", S = _, P = "y1") : (A = _, L = "y1", S = p, P = "y0"), tt(n), nt(l, r), function(t, e, r) {
                                                                     var n = e.xref,
                                                                         i = e.yref,
                                                                         a = o.getFromId(r, n),
                                                                         s = o.getFromId(r, i),
                                                                         l = "";
-                                                                    "paper" === n || a.autorange || (l += n), "paper" === i || s.autorange || (l += i), f.setClipUrl(t, l ? "clip" + r._fullLayout._uid + l : null, r)
+                                                                    "paper" === n || a.autorange || (l += n), "paper" === i || s.autorange || (l += i), h.setClipUrl(t, l ? "clip" + r._fullLayout._uid + l : null, r)
                                                                 }(e, r, t), Q.moveFn = "move" === z ? et : rt, Q.altKey = n.altKey)
                                                             },
                                                             doneFn: function() {
-                                                                w(t) || (d(e), it(l), M(e, t, r), i.call("_guiRelayout", t, u.getUpdateObj()))
+                                                                b(t) || (v(e), it(l), k(e, t, r), i.call("_guiRelayout", t, c.getUpdateObj()))
                                                             },
                                                             clickFn: function() {
-                                                                w(t) || it(l)
+                                                                b(t) || it(l)
                                                             }
                                                         };
 
                                                     function tt(r) {
-                                                        if (w(t)) z = null;
+                                                        if (b(t)) z = null;
                                                         else if (j) z = "path" === r.target.tagName ? "move" : "start-point" === r.target.attributes["data-line-point"].value ? "resize-over-start-point" : "resize-over-end-point";
                                                         else {
                                                             var n = Q.element.getBoundingClientRect(),
                                                                 i = n.right - n.left,
                                                                 a = n.bottom - n.top,
                                                                 o = r.clientX - n.left,
                                                                 s = r.clientY - n.top,
-                                                                l = !U && i > R && a > F && !r.shiftKey ? p.getCursor(o / i, 1 - s / a) : "move";
-                                                            d(e, l), z = l.split("-")[0]
+                                                                l = !U && i > R && a > F && !r.shiftKey ? d.getCursor(o / i, 1 - s / a) : "move";
+                                                            v(e, l), z = l.split("-")[0]
                                                         }
                                                     }
 
                                                     function et(n, i) {
                                                         if ("path" === r.type) {
                                                             var a = function(t) {
                                                                     return t
                                                                 },
                                                                 o = a,
-                                                                u = a;
-                                                            B ? V("xanchor", r.xanchor = K(b + n)) : (o = function(t) {
+                                                                c = a;
+                                                            B ? V("xanchor", r.xanchor = K(w + n)) : (o = function(t) {
                                                                 return K(Z(t) + n)
-                                                            }, q && "date" === q.type && (o = y.encodeDate(o))), N ? V("yanchor", r.yanchor = J(_ + i)) : (u = function(t) {
+                                                            }, q && "date" === q.type && (o = y.encodeDate(o))), N ? V("yanchor", r.yanchor = J(M + i)) : (c = function(t) {
                                                                 return J(X(t) + i)
-                                                            }, Y && "date" === Y.type && (u = y.encodeDate(u))), V("path", r.path = S(D, o, u))
-                                                        } else B ? V("xanchor", r.xanchor = K(b + n)) : (V("x0", r.x0 = K(c + n)), V("x1", r.x1 = K(v + n))), N ? V("yanchor", r.yanchor = J(_ + i)) : (V("y0", r.y0 = J(h + i)), V("y1", r.y1 = J(x + i)));
-                                                        e.attr("d", m(t, r)), nt(l, r), A(t, s, r, H)
+                                                            }, Y && "date" === Y.type && (c = y.encodeDate(c))), V("path", r.path = T(D, o, c))
+                                                        } else B ? V("xanchor", r.xanchor = K(w + n)) : (V("x0", r.x0 = K(f + n)), V("x1", r.x1 = K(x + n))), N ? V("yanchor", r.yanchor = J(M + i)) : (V("y0", r.y0 = J(p + i)), V("y1", r.y1 = J(_ + i)));
+                                                        e.attr("d", m(t, r)), nt(l, r), u(t, s, r, H)
                                                     }
 
                                                     function rt(n, i) {
                                                         if (U) {
                                                             var a = function(t) {
                                                                     return t
                                                                 },
                                                                 o = a,
-                                                                u = a;
-                                                            B ? V("xanchor", r.xanchor = K(b + n)) : (o = function(t) {
+                                                                c = a;
+                                                            B ? V("xanchor", r.xanchor = K(w + n)) : (o = function(t) {
                                                                 return K(Z(t) + n)
-                                                            }, q && "date" === q.type && (o = y.encodeDate(o))), N ? V("yanchor", r.yanchor = J(_ + i)) : (u = function(t) {
+                                                            }, q && "date" === q.type && (o = y.encodeDate(o))), N ? V("yanchor", r.yanchor = J(M + i)) : (c = function(t) {
                                                                 return J(X(t) + i)
-                                                            }, Y && "date" === Y.type && (u = y.encodeDate(u))), V("path", r.path = S(D, o, u))
+                                                            }, Y && "date" === Y.type && (c = y.encodeDate(c))), V("path", r.path = T(D, o, c))
                                                         } else if (j) {
                                                             if ("resize-over-start-point" === z) {
-                                                                var f = c + n,
-                                                                    p = N ? h - i : h + i;
-                                                                V("x0", r.x0 = B ? f : K(f)), V("y0", r.y0 = N ? p : J(p))
+                                                                var h = f + n,
+                                                                    d = N ? p - i : p + i;
+                                                                V("x0", r.x0 = B ? h : K(h)), V("y0", r.y0 = N ? d : J(d))
                                                             } else if ("resize-over-end-point" === z) {
-                                                                var d = v + n,
-                                                                    g = N ? x - i : x + i;
-                                                                V("x1", r.x1 = B ? d : K(d)), V("y1", r.y1 = N ? g : J(g))
+                                                                var v = x + n,
+                                                                    g = N ? _ - i : _ + i;
+                                                                V("x1", r.x1 = B ? v : K(v)), V("y1", r.y1 = N ? g : J(g))
                                                             }
                                                         } else {
-                                                            var w = function(t) {
+                                                            var b = function(t) {
                                                                     return -1 !== z.indexOf(t)
                                                                 },
-                                                                M = w("n"),
-                                                                G = w("s"),
-                                                                W = w("w"),
-                                                                $ = w("e"),
-                                                                Q = M ? k + i : k,
-                                                                tt = G ? T + i : T,
+                                                                k = b("n"),
+                                                                G = b("s"),
+                                                                W = b("w"),
+                                                                $ = b("e"),
+                                                                Q = k ? A + i : A,
+                                                                tt = G ? S + i : S,
                                                                 et = W ? E + n : E,
                                                                 rt = $ ? C + n : C;
-                                                            N && (M && (Q = k - i), G && (tt = T - i)), (!N && tt - Q > F || N && Q - tt > F) && (V(L, r[L] = N ? Q : J(Q)), V(P, r[P] = N ? tt : J(tt))), rt - et > R && (V(O, r[O] = B ? et : K(et)), V(I, r[I] = B ? rt : K(rt)))
+                                                            N && (k && (Q = A - i), G && (tt = S - i)), (!N && tt - Q > F || N && Q - tt > F) && (V(L, r[L] = N ? Q : J(Q)), V(P, r[P] = N ? tt : J(tt))), rt - et > R && (V(O, r[O] = B ? et : K(et)), V(I, r[I] = B ? rt : K(rt)))
                                                         }
-                                                        e.attr("d", m(t, r)), nt(l, r), A(t, s, r, H)
+                                                        e.attr("d", m(t, r)), nt(l, r), u(t, s, r, H)
                                                     }
 
                                                     function nt(t, e) {
                                                         (B || N) && function() {
                                                             var r = "path" !== e.type,
                                                                 n = t.selectAll(".visual-cue").data([0]);
                                                             n.enter().append("path").attr({
@@ -32047,170 +32174,69 @@
                                                             }
                                                         }()
                                                     }
 
                                                     function it(t) {
                                                         t.selectAll(".visual-cue").remove()
                                                     }
-                                                    p.init(Q), $.node().onmousemove = tt
-                                                }(t, F, u, e, r, z) : !0 === u.editable && F.style("pointer-events", I || c.opacity(C) * T <= .5 ? "stroke" : "all");
+                                                    d.init(Q), $.node().onmousemove = tt
+                                                }(t, F, c, e, r, z) : !0 === c.editable && F.style("pointer-events", I || f.opacity(C) * E <= .5 ? "stroke" : "all");
                                                 F.node().addEventListener("click", (function() {
                                                     return function(t, e) {
-                                                        if (k(t)) {
+                                                        if (_(t)) {
                                                             var r = +e.node().getAttribute("data-index");
                                                             if (r >= 0) {
-                                                                if (r === t._fullLayout._activeShapeIndex) return void E(t);
-                                                                t._fullLayout._activeShapeIndex = r, t._fullLayout._deactivateShape = E, _(t)
+                                                                if (r === t._fullLayout._activeShapeIndex) return void M(t);
+                                                                t._fullLayout._activeShapeIndex = r, t._fullLayout._deactivateShape = M, x(t)
                                                             }
                                                         }
                                                     }(t, F)
                                                 }))
                                             }
-                                            u._input && !1 !== u.visible && ("below" !== u.layer ? x(t._fullLayout._shapeUpperLayer) : "paper" === u.xref || "paper" === u.yref ? x(t._fullLayout._shapeLowerLayer) : v._hadPlotinfo ? x((v.mainplotinfo || v).shapelayer) : x(t._fullLayout._shapeLowerLayer))
+                                            c._input && !1 !== c.visible && ("below" !== c.layer ? A(t._fullLayout._shapeUpperLayer) : "paper" === c.xref || "paper" === c.yref ? A(t._fullLayout._shapeLowerLayer) : w._hadPlotinfo ? A((w.mainplotinfo || w).shapelayer) : A(t._fullLayout._shapeLowerLayer))
                                         }
 
-                                        function M(t, e, r) {
+                                        function k(t, e, r) {
                                             var n = (r.xref + r.yref).replace(/paper/g, "").replace(/[xyz][1-9]* *domain/g, "");
-                                            f.setClipUrl(t, n ? "clip" + e._fullLayout._uid + n : null, e)
+                                            h.setClipUrl(t, n ? "clip" + e._fullLayout._uid + n : null, e)
                                         }
 
-                                        function A(t, e, r, n) {
-                                            if (n.selectAll(".shape-label").remove(), r.label.text || r.label.texttemplate) {
-                                                var i;
-                                                if (r.label.texttemplate) {
-                                                    var l = {};
-                                                    if ("path" !== r.type) {
-                                                        var u = o.getFromId(t, r.xref),
-                                                            c = o.getFromId(t, r.yref);
-                                                        for (var h in x) {
-                                                            var p = x[h](r, u, c);
-                                                            void 0 !== p && (l[h] = p)
-                                                        }
-                                                    }
-                                                    i = a.texttemplateStringForShapes(r.label.texttemplate, {}, t._fullLayout._d3locale, l)
-                                                } else i = r.label.text;
-                                                var d, g, _, w, k = {
-                                                        "data-index": e
-                                                    },
-                                                    T = r.label.font,
-                                                    M = n.append("g").attr(k).classed("shape-label", !0).append("text").attr({
-                                                        "data-notex": 1
-                                                    }).classed("shape-label-text", !0).text(i);
-                                                if (r.path) {
-                                                    var A = m(t, r),
-                                                        S = s(A, t);
-                                                    d = 1 / 0, _ = 1 / 0, g = -1 / 0, w = -1 / 0;
-                                                    for (var E = 0; E < S.length; E++)
-                                                        for (var C = 0; C < S[E].length; C++)
-                                                            for (var L = S[E][C], P = 1; P < L.length; P += 2) {
-                                                                var O = L[P],
-                                                                    I = L[P + 1];
-                                                                d = Math.min(d, O), g = Math.max(g, O), _ = Math.min(_, I), w = Math.max(w, I)
-                                                            }
-                                                } else {
-                                                    var D = o.getFromId(t, r.xref),
-                                                        z = o.getRefType(r.xref),
-                                                        R = o.getFromId(t, r.yref),
-                                                        F = o.getRefType(r.yref),
-                                                        B = y.getDataToPixel(t, D, !1, z),
-                                                        N = y.getDataToPixel(t, R, !0, F);
-                                                    d = B(r.x0), g = B(r.x1), _ = N(r.y0), w = N(r.y1)
-                                                }
-                                                var j = r.label.textangle;
-                                                "auto" === j && (j = "line" === r.type ? function(t, e, r, n) {
-                                                    var i, a;
-                                                    return a = Math.abs(r - t), i = r >= t ? e - n : n - e, -180 / Math.PI * Math.atan2(i, a)
-                                                }(d, _, g, w) : 0), M.call((function(e) {
-                                                    return e.call(f.font, T).attr({}), v.convertToTspans(e, t), e
-                                                }));
-                                                var U = function(t, e, r, n, i, a, o) {
-                                                        var s, l, u, c, f = i.label.textposition,
-                                                            h = i.label.textangle,
-                                                            p = i.label.padding,
-                                                            d = i.type,
-                                                            v = Math.PI / 180 * a,
-                                                            g = Math.sin(v),
-                                                            y = Math.cos(v),
-                                                            m = i.label.xanchor,
-                                                            x = i.label.yanchor;
-                                                        if ("line" === d) {
-                                                            "start" === f ? (s = t, l = e) : "end" === f ? (s = r, l = n) : (s = (t + r) / 2, l = (e + n) / 2), "auto" === m && (m = "start" === f ? "auto" === h ? r > t ? "left" : r < t ? "right" : "center" : r > t ? "right" : r < t ? "left" : "center" : "end" === f ? "auto" === h ? r > t ? "right" : r < t ? "left" : "center" : r > t ? "left" : r < t ? "right" : "center" : "center");
-                                                            var _ = {
-                                                                bottom: -1,
-                                                                middle: 0,
-                                                                top: 1
-                                                            };
-                                                            if ("auto" === h) {
-                                                                var w = _[x];
-                                                                u = -p * g * w, c = p * y * w
-                                                            } else u = p * {
-                                                                left: 1,
-                                                                center: 0,
-                                                                right: -1
-                                                            } [m], c = p * _[x];
-                                                            s += u, l += c
-                                                        } else u = p + 3, -1 !== f.indexOf("right") ? (s = Math.max(t, r) - u, "auto" === m && (m = "right")) : -1 !== f.indexOf("left") ? (s = Math.min(t, r) + u, "auto" === m && (m = "left")) : (s = (t + r) / 2, "auto" === m && (m = "center")), l = -1 !== f.indexOf("top") ? Math.min(e, n) : -1 !== f.indexOf("bottom") ? Math.max(e, n) : (e + n) / 2, c = p, "bottom" === x ? l -= c : "top" === x && (l += c);
-                                                        var k = b[x],
-                                                            T = i.label.font.size,
-                                                            M = o.height;
-                                                        return {
-                                                            textx: s + (M * k - T) * g,
-                                                            texty: l + -(M * k - T) * y,
-                                                            xanchor: m
-                                                        }
-                                                    }(d, _, g, w, r, j, f.bBox(M.node())),
-                                                    V = U.textx,
-                                                    H = U.texty,
-                                                    q = U.xanchor;
-                                                M.attr({
-                                                    "text-anchor": {
-                                                        left: "start",
-                                                        center: "middle",
-                                                        right: "end"
-                                                    } [q],
-                                                    y: H,
-                                                    x: V,
-                                                    transform: "rotate(" + j + "," + V + "," + H + ")"
-                                                }).call(v.positionText, V, H)
-                                            }
-                                        }
-
-                                        function S(t, e, r) {
+                                        function T(t, e, r) {
                                             return t.replace(g.segmentRE, (function(t) {
                                                 var n = 0,
                                                     i = t.charAt(0),
                                                     a = g.paramIsX[i],
                                                     o = g.paramIsY[i],
                                                     s = g.numParams[i];
                                                 return i + t.substr(1).replace(g.paramRE, (function(t) {
                                                     return n >= s || (a[n] ? t = e(t) : o[n] && (t = r(t)), n++), t
                                                 }))
                                             }))
                                         }
 
-                                        function E(t) {
-                                            k(t) && t._fullLayout._activeShapeIndex >= 0 && (u(t), delete t._fullLayout._activeShapeIndex, _(t))
+                                        function M(t) {
+                                            _(t) && t._fullLayout._activeShapeIndex >= 0 && (c(t), delete t._fullLayout._activeShapeIndex, x(t))
                                         }
                                         t.exports = {
-                                            draw: _,
-                                            drawOne: T,
+                                            draw: x,
+                                            drawOne: w,
                                             eraseActiveShape: function(t) {
-                                                if (k(t)) {
-                                                    u(t);
+                                                if (_(t)) {
+                                                    c(t);
                                                     var e = t._fullLayout._activeShapeIndex,
                                                         r = (t.layout || {}).shapes || [];
                                                     if (e < r.length) {
                                                         for (var n = [], a = 0; a < r.length; a++) a !== e && n.push(r[a]);
                                                         delete t._fullLayout._activeShapeIndex, i.call("_guiRelayout", t, {
                                                             shapes: n
                                                         })
                                                     }
                                                 }
                                             },
-                                            drawLabel: A
+                                            drawLabel: u
                                         }
                                     },
                                     29241: function(t, e, r) {
                                         "use strict";
                                         var n = r(41940),
                                             i = r(79952).P,
                                             a = r(1426).extendFlat,
@@ -32535,105 +32561,113 @@
                                             v = p.r2p,
                                             g = r(51873).clearOutline,
                                             y = r(60165),
                                             m = y.readPaths,
                                             x = y.writePaths,
                                             b = y.ellipseOver,
                                             _ = y.fixDatesForPaths;
-                                        t.exports = function(t, e) {
-                                            if (t.length) {
-                                                var r = t[0][0];
-                                                if (r) {
-                                                    var n = r.getAttribute("d"),
-                                                        o = e.gd,
-                                                        p = o._fullLayout.newshape,
-                                                        y = e.plotinfo,
-                                                        w = y.xaxis,
-                                                        k = y.yaxis,
-                                                        T = !!y.domain || !y.xaxis,
-                                                        M = !!y.domain || !y.yaxis,
-                                                        A = e.isActiveShape,
-                                                        S = e.dragmode,
-                                                        E = (o.layout || {}).shapes || [];
-                                                    if (!i(S) && void 0 !== A) {
-                                                        var C = o._fullLayout._activeShapeIndex;
-                                                        if (C < E.length) switch (o._fullLayout.shapes[C].type) {
+
+                                        function w(t, e, r) {
+                                            var n, i = t[0][0],
+                                                o = e.gd,
+                                                p = i.getAttribute("d"),
+                                                g = o._fullLayout.newshape,
+                                                y = e.plotinfo,
+                                                w = e.isActiveShape,
+                                                k = y.xaxis,
+                                                T = y.yaxis,
+                                                M = !!y.domain || !y.xaxis,
+                                                A = !!y.domain || !y.yaxis,
+                                                S = a(r),
+                                                E = m(p, o, y, w),
+                                                C = {
+                                                    editable: !0,
+                                                    label: g.label,
+                                                    xref: M ? "paper" : k._id,
+                                                    yref: A ? "paper" : T._id,
+                                                    layer: g.layer,
+                                                    opacity: g.opacity,
+                                                    line: {
+                                                        color: g.line.color,
+                                                        width: g.line.width,
+                                                        dash: g.line.dash
+                                                    }
+                                                };
+                                            if (S || (C.fillcolor = g.fillcolor, C.fillrule = g.fillrule), 1 === E.length && (n = E[0]), n && 5 === n.length && "drawrect" === r) C.type = "rect", C.x0 = n[0][1], C.y0 = n[0][2], C.x1 = n[2][1], C.y1 = n[2][2];
+                                            else if (n && "drawline" === r) C.type = "line", C.x0 = n[0][1], C.y0 = n[0][2], C.x1 = n[1][1], C.y1 = n[1][2];
+                                            else if (n && "drawcircle" === r) {
+                                                C.type = "circle";
+                                                var L = n[s][1],
+                                                    P = n[l][1],
+                                                    O = n[u][1],
+                                                    I = n[c][1],
+                                                    D = n[s][2],
+                                                    z = n[l][2],
+                                                    R = n[u][2],
+                                                    F = n[c][2],
+                                                    B = y.xaxis && ("date" === y.xaxis.type || "log" === y.xaxis.type),
+                                                    N = y.yaxis && ("date" === y.yaxis.type || "log" === y.yaxis.type);
+                                                B && (L = v(y.xaxis, L), P = v(y.xaxis, P), O = v(y.xaxis, O), I = v(y.xaxis, I)), N && (D = v(y.yaxis, D), z = v(y.yaxis, z), R = v(y.yaxis, R), F = v(y.yaxis, F));
+                                                var j = (P + I) / 2,
+                                                    U = (D + R) / 2,
+                                                    V = b({
+                                                        x0: j,
+                                                        y0: U,
+                                                        x1: j + (I - P + O - L) / 2 * f,
+                                                        y1: U + (F - z + R - D) / 2 * h
+                                                    });
+                                                B && (V.x0 = d(y.xaxis, V.x0), V.x1 = d(y.xaxis, V.x1)), N && (V.y0 = d(y.yaxis, V.y0), V.y1 = d(y.yaxis, V.y1)), C.x0 = V.x0, C.y0 = V.y0, C.x1 = V.x1, C.y1 = V.y1
+                                            } else C.type = "path", k && T && _(E, k, T), C.path = x(E), n = null;
+                                            return C
+                                        }
+                                        t.exports = {
+                                            newShapes: function(t, e) {
+                                                if (t.length && t[0][0]) {
+                                                    var r = e.gd,
+                                                        n = e.isActiveShape,
+                                                        a = e.dragmode,
+                                                        o = (r.layout || {}).shapes || [];
+                                                    if (!i(a) && void 0 !== n) {
+                                                        var s = r._fullLayout._activeShapeIndex;
+                                                        if (s < o.length) switch (r._fullLayout.shapes[s].type) {
                                                             case "rect":
-                                                                S = "drawrect";
+                                                                a = "drawrect";
                                                                 break;
                                                             case "circle":
-                                                                S = "drawcircle";
+                                                                a = "drawcircle";
                                                                 break;
                                                             case "line":
-                                                                S = "drawline";
+                                                                a = "drawline";
                                                                 break;
                                                             case "path":
-                                                                var L = E[C].path || "";
-                                                                S = "Z" === L[L.length - 1] ? "drawclosedpath" : "drawopenpath"
+                                                                var l = o[s].path || "";
+                                                                a = "Z" === l[l.length - 1] ? "drawclosedpath" : "drawopenpath"
                                                         }
                                                     }
-                                                    var P, O = a(S),
-                                                        I = m(n, o, y, A),
-                                                        D = {
-                                                            editable: !0,
-                                                            label: p.label,
-                                                            xref: T ? "paper" : w._id,
-                                                            yref: M ? "paper" : k._id,
-                                                            layer: p.layer,
-                                                            opacity: p.opacity,
-                                                            line: {
-                                                                color: p.line.color,
-                                                                width: p.line.width,
-                                                                dash: p.line.dash
-                                                            }
-                                                        };
-                                                    if (O || (D.fillcolor = p.fillcolor, D.fillrule = p.fillrule), 1 === I.length && (P = I[0]), P && 5 === P.length && "drawrect" === S) D.type = "rect", D.x0 = P[0][1], D.y0 = P[0][2], D.x1 = P[2][1], D.y1 = P[2][2];
-                                                    else if (P && "drawline" === S) D.type = "line", D.x0 = P[0][1], D.y0 = P[0][2], D.x1 = P[1][1], D.y1 = P[1][2];
-                                                    else if (P && "drawcircle" === S) {
-                                                        D.type = "circle";
-                                                        var z = P[s][1],
-                                                            R = P[l][1],
-                                                            F = P[u][1],
-                                                            B = P[c][1],
-                                                            N = P[s][2],
-                                                            j = P[l][2],
-                                                            U = P[u][2],
-                                                            V = P[c][2],
-                                                            H = y.xaxis && ("date" === y.xaxis.type || "log" === y.xaxis.type),
-                                                            q = y.yaxis && ("date" === y.yaxis.type || "log" === y.yaxis.type);
-                                                        H && (z = v(y.xaxis, z), R = v(y.xaxis, R), F = v(y.xaxis, F), B = v(y.xaxis, B)), q && (N = v(y.yaxis, N), j = v(y.yaxis, j), U = v(y.yaxis, U), V = v(y.yaxis, V));
-                                                        var G = (R + B) / 2,
-                                                            Y = (N + U) / 2,
-                                                            W = b({
-                                                                x0: G,
-                                                                y0: Y,
-                                                                x1: G + (B - R + F - z) / 2 * f,
-                                                                y1: Y + (V - j + U - N) / 2 * h
-                                                            });
-                                                        H && (W.x0 = d(y.xaxis, W.x0), W.x1 = d(y.xaxis, W.x1)), q && (W.y0 = d(y.yaxis, W.y0), W.y1 = d(y.yaxis, W.y1)), D.x0 = W.x0, D.y0 = W.y0, D.x1 = W.x1, D.y1 = W.y1
-                                                    } else D.type = "path", w && k && _(I, w, k), D.path = x(I), P = null;
-                                                    g(o);
-                                                    for (var Z = e.editHelpers, X = (Z || {}).modifyItem, K = [], J = 0; J < E.length; J++) {
-                                                        var $ = o._fullLayout.shapes[J];
-                                                        if (K[J] = $._input, void 0 !== A && J === o._fullLayout._activeShapeIndex) {
-                                                            var Q = D;
-                                                            switch ($.type) {
+                                                    var u = w(t, e, a);
+                                                    g(r);
+                                                    for (var c = e.editHelpers, f = (c || {}).modifyItem, h = [], p = 0; p < o.length; p++) {
+                                                        var d = r._fullLayout.shapes[p];
+                                                        if (h[p] = d._input, void 0 !== n && p === r._fullLayout._activeShapeIndex) {
+                                                            var v = u;
+                                                            switch (d.type) {
                                                                 case "line":
                                                                 case "rect":
                                                                 case "circle":
-                                                                    X("x0", Q.x0), X("x1", Q.x1), X("y0", Q.y0), X("y1", Q.y1);
+                                                                    f("x0", v.x0), f("x1", v.x1), f("y0", v.y0), f("y1", v.y1);
                                                                     break;
                                                                 case "path":
-                                                                    X("path", Q.path)
+                                                                    f("path", v.path)
                                                             }
                                                         }
                                                     }
-                                                    return void 0 === A ? (K.push(D), K) : Z ? Z.getUpdateObj() : {}
+                                                    return void 0 === n ? (h.push(u), h) : c ? c.getUpdateObj() : {}
                                                 }
-                                            }
+                                            },
+                                            createShapeObj: w
                                         }
                                     },
                                     51873: function(t) {
                                         "use strict";
                                         t.exports = {
                                             clearOutlineControllers: function(t) {
                                                 var e = t._fullLayout._zoomlayer;
@@ -36902,28 +36936,29 @@
                                         "use strict";
                                         var n = r(32396),
                                             i = r(91424),
                                             a = r(71828),
                                             o = null;
                                         t.exports = function() {
                                             if (null !== o) return o;
-                                            if (a.isIE()) o = !1;
-                                            else {
-                                                var t = Array.from(n.CSS_DECLARATIONS).reverse(),
-                                                    e = window.CSS && window.CSS.supports || window.supportsCSS;
-                                                if ("function" == typeof e) o = t.some((function(t) {
-                                                    return e.apply(null, t)
+                                            o = !1;
+                                            var t = a.isIE() || a.isSafari() || a.isIOS();
+                                            if (window.navigator.userAgent && !t) {
+                                                var e = Array.from(n.CSS_DECLARATIONS).reverse(),
+                                                    r = window.CSS && window.CSS.supports || window.supportsCSS;
+                                                if ("function" == typeof r) o = e.some((function(t) {
+                                                    return r.apply(null, t)
                                                 }));
                                                 else {
-                                                    var r = i.tester.append("image"),
-                                                        s = window.getComputedStyle(r.node());
-                                                    r.attr("style", n.STYLE), o = t.some((function(t) {
+                                                    var s = i.tester.append("image").attr("style", n.STYLE),
+                                                        l = window.getComputedStyle(s.node()).imageRendering;
+                                                    o = e.some((function(t) {
                                                         var e = t[1];
-                                                        return s.imageRendering === e || s.imageRendering === e.toLowerCase()
-                                                    })), r.remove()
+                                                        return l === e || l === e.toLowerCase()
+                                                    })), s.remove()
                                                 }
                                             }
                                             return o
                                         }
                                     },
                                     63893: function(t, e, r) {
                                         "use strict";
@@ -82845,15 +82880,15 @@
                                                     r._indexToPoints = v, e._length = u
                                                 }
                                             }
                                         }
                                     },
                                     11506: function(t, e) {
                                         "use strict";
-                                        e.version = "2.23.0"
+                                        e.version = "2.23.2"
                                     },
                                     9330: function(t, e, r) {
                                         var n, i = r(90386);
                                         self, n = function() {
                                             return function() {
                                                 var t = {
                                                     7386: function(t, e, r) {
```

### Comparing `interpret-core-0.4.1/interpret/lib/interpret-inline.js.LICENSE.txt` & `interpret-core-0.4.2/interpret/lib/interpret-inline.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/perf/_curve.py` & `interpret-core-0.4.2/interpret/perf/_curve.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/perf/_regression.py` & `interpret-core-0.4.2/interpret/perf/_regression.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/provider/_compute.py` & `interpret-core-0.4.2/interpret/provider/_compute.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/provider/_environment.py` & `interpret-core-0.4.2/interpret/provider/_environment.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/provider/_visualize.py` & `interpret-core-0.4.2/interpret/provider/_visualize.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_SPOTgreedy.py` & `interpret-core-0.4.2/interpret/utils/_SPOTgreedy.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_clean_simple.py` & `interpret-core-0.4.2/interpret/utils/_clean_simple.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_clean_x.py` & `interpret-core-0.4.2/interpret/utils/_clean_x.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_compressed_dataset.py` & `interpret-core-0.4.2/interpret/utils/_compressed_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,22 +53,21 @@
 
         if not X_col.flags.c_contiguous:
             # X_col could be a slice that has a stride.  We need contiguous for caling into C
             X_col = X_col.copy()
 
         if isinstance(feature_bins, dict):
             # categorical feature
-            n_bins = 1 if len(feature_bins) == 0 else (max(feature_bins.values()) + 1)
+            n_bins = 2 if len(feature_bins) == 0 else (max(feature_bins.values()) + 2)
         else:
             # continuous feature
             X_col = native.discretize(X_col, feature_bins)
-            n_bins = len(feature_bins) + 2
+            n_bins = len(feature_bins) + 3
 
         if bad is not None:
-            n_bins += 1
             X_col[bad != _none_ndarray] = n_bins - 1
 
         n_bytes += native.measure_feature(
             n_bins,
             np.count_nonzero(X_col) != len(X_col),
             bad is not None,
             feature_types_in[feature_idx] == "nominal",
@@ -98,22 +97,21 @@
 
         if not X_col.flags.c_contiguous:
             # X_col could be a slice that has a stride.  We need contiguous for caling into C
             X_col = X_col.copy()
 
         if isinstance(feature_bins, dict):
             # categorical feature
-            n_bins = 1 if len(feature_bins) == 0 else (max(feature_bins.values()) + 1)
+            n_bins = 2 if len(feature_bins) == 0 else (max(feature_bins.values()) + 2)
         else:
             # continuous feature
             X_col = native.discretize(X_col, feature_bins)
-            n_bins = len(feature_bins) + 2
+            n_bins = len(feature_bins) + 3
 
         if bad is not None:
-            n_bins += 1
             X_col[bad != _none_ndarray] = n_bins - 1
 
         native.fill_feature(
             n_bins,
             np.count_nonzero(X_col) != len(X_col),
             bad is not None,
             feature_types_in[feature_idx] == "nominal",
```

### Comparing `interpret-core-0.4.1/interpret/utils/_explanation.py` & `interpret-core-0.4.2/interpret/utils/_explanation.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_histogram.py` & `interpret-core-0.4.2/interpret/utils/_histogram.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_link.py` & `interpret-core-0.4.2/interpret/utils/_link.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_measure_interactions.py` & `interpret-core-0.4.2/interpret/utils/_measure_interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,8 +256,11 @@
         min_samples_leaf=min_samples_leaf,
         is_private=is_differential_privacy,
         objective=objective,
         experimental_params=None,
         n_output_interactions=n_output_interactions,
     )
 
+    if isinstance(ranked_interactions, Exception):
+        raise ranked_interactions
+
     return list(map(tuple, map(reversed, ranked_interactions)))
```

### Comparing `interpret-core-0.4.1/interpret/utils/_native.py` & `interpret-core-0.4.2/interpret/utils/_native.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,31 +51,37 @@
         return Native._native
 
     @staticmethod
     def _make_pointer(array, dtype, ndim=1, is_null_allowed=False):
         # using ndpointer creates cyclic garbage references which could clog up
         # our memory and require extra garbage collections.  This function avoids that
 
+        # array MUST be an object with a reference that will remain valid for the duration
+        # of the pointer's use. We do not create a new reference to array
+
         if array is None:
             if not is_null_allowed:  # pragma: no cover
                 raise ValueError("array cannot be None")
             return None
 
         if not isinstance(array, np.ndarray):  # pragma: no cover
             raise ValueError("array should be an ndarray")
 
         if array.dtype.type is not dtype:  # pragma: no cover
             raise ValueError(f"array should be an ndarray of type {dtype}")
 
+        # if the data is transposed, Fortran ordered, or has strides, we can't use it
         if not array.flags.c_contiguous:  # pragma: no cover
             raise ValueError("array should be a contiguous ndarray")
 
         if array.ndim != ndim:  # pragma: no cover
             raise ValueError(f"array should have {ndim} dimensions")
 
+        # ctypes.data will return an interor pointer when given an array that is sliced,
+        # so arr[1:-1] will return a pointer to the 1st element within arr.
         return array.ctypes.data
 
     @staticmethod
     def _get_native_exception(error_code, native_function):  # pragma: no cover
         if error_code == -1:
             return Exception(f"Out of memory in {native_function}")
         elif error_code == -2:
@@ -107,15 +113,15 @@
         elif error_code == -19:
             return Exception("Differential Privacy not supported by the objective")
         elif error_code == -20:
             return Exception(
                 "Differential Privacy not supported by an objective parameter value"
             )
         elif error_code == -21:
-            return Exception("Illegal target value for the objective")
+            return Exception("Illegal value in y for the objective")
         else:
             return Exception(
                 f"Unrecognized native return code {error_code} in {native_function}"
             )
 
     @staticmethod
     def get_count_scores_c(n_classes):
@@ -1088,15 +1094,15 @@
         self._unsafe.GetTermUpdateSplits.argtypes = [
             # void * boosterHandle
             ct.c_void_p,
             # int64_t indexDimension
             ct.c_int64,
             # int64_t * countSplitsInOut
             ct.POINTER(ct.c_int64),
-            # int64_t * splitIndexesOut
+            # int64_t * splitsOut
             ct.c_void_p,
         ]
         self._unsafe.GetTermUpdateSplits.restype = ct.c_int32
 
         self._unsafe.GetTermUpdate.argtypes = [
             # void * boosterHandle
             ct.c_void_p,
@@ -1263,15 +1269,14 @@
 
         self._term_shapes = None
         if 0 < n_class_scores:
             bin_counts = native.extract_bin_counts(self.dataset, n_features)
             self._term_shapes = []
             for feature_idxs in self.term_features:
                 dimensions = [bin_counts[feature_idx] for feature_idx in feature_idxs]
-                dimensions.reverse()
 
                 # Array returned for multiclass is one higher dimension
                 if 1 < n_class_scores:
                     dimensions.append(n_class_scores)
 
                 self._term_shapes.append(tuple(dimensions))
 
@@ -1331,14 +1336,15 @@
             self._booster_handle = None
             native._unsafe.FreeBooster(booster_handle)
 
         _log.info("Deallocation boosting end")
 
     def generate_term_update(
         self,
+        rng,
         term_idx,
         boost_flags,
         learning_rate,
         min_samples_leaf,
         max_leaves,
     ):
         """Generates a boosting step update per feature
@@ -1362,15 +1368,15 @@
         native = Native.get_native_singleton()
 
         avg_gain = ct.c_double(0.0)
         n_features = len(self.term_features[term_idx])
         max_leaves_arr = np.full(n_features, max_leaves, dtype=ct.c_int64, order="C")
 
         return_code = native._unsafe.GenerateTermUpdate(
-            Native._make_pointer(self.rng, np.ubyte, is_null_allowed=True),
+            Native._make_pointer(rng, np.ubyte, is_null_allowed=True),
             self._booster_handle,
             term_idx,
             boost_flags,
             learning_rate,
             min_samples_leaf,
             Native._make_pointer(max_leaves_arr, np.int64),
             ct.byref(avg_gain),
@@ -1435,18 +1441,18 @@
             splits_dimension = self._get_term_update_splits_dimension(dimension_idx)
             splits.append(splits_dimension)
 
         return splits
 
     def _get_best_term_scores(self, term_idx):
         """Returns best model/function according to validation set
-            for a given feature group.
+            for a given term.
 
         Args:
-            term_idx: The index for the feature group.
+            term_idx: The index for the term.
 
         Returns:
             An ndarray that represents the model.
         """
 
         if self._term_shapes is None:  # pragma: no cover
             # if there is only one legal state for a classification problem, then we know with 100%
@@ -1463,29 +1469,22 @@
             self._booster_handle,
             term_idx,
             Native._make_pointer(term_scores, np.float64, len(shape)),
         )
         if return_code:  # pragma: no cover
             raise Native._get_native_exception(return_code, "GetBestTermScores")
 
-        n_dimensions = len(self.term_features[term_idx])
-        temp_transpose = [*range(n_dimensions - 1, -1, -1)]
-        if len(shape) != n_dimensions:  # multiclass
-            temp_transpose.append(len(temp_transpose))
-        term_scores = np.ascontiguousarray(
-            np.transpose(term_scores, tuple(temp_transpose))
-        )
         return term_scores
 
     def _get_current_term_scores(self, term_idx):
         """Returns current model/function according to validation set
-            for a given feature group.
+            for a given term.
 
         Args:
-            term_idx: The index for the feature group.
+            term_idx: The index for the term.
 
         Returns:
             An ndarray that represents the model.
         """
 
         if self._term_shapes is None:  # pragma: no cover
             # if there is only one legal state for a classification problem, then we know with 100%
@@ -1502,21 +1501,14 @@
             self._booster_handle,
             term_idx,
             Native._make_pointer(term_scores, np.float64, len(shape)),
         )
         if return_code:  # pragma: no cover
             raise Native._get_native_exception(return_code, "GetCurrentTermScores")
 
-        n_dimensions = len(self.term_features[term_idx])
-        temp_transpose = [*range(n_dimensions - 1, -1, -1)]
-        if len(shape) != n_dimensions:  # multiclass
-            temp_transpose.append(len(temp_transpose))
-        term_scores = np.ascontiguousarray(
-            np.transpose(term_scores, tuple(temp_transpose))
-        )
         return term_scores
 
     def _get_term_update_splits_dimension(self, dimension_index):
         if self._term_shapes is None:  # pragma: no cover
             # if there is only one legal state for a classification problem, then we know with 100%
             # certainty what the result will be, and our model has no information since we always predict
             # the only output
@@ -1560,21 +1552,14 @@
         return_code = native._unsafe.GetTermUpdate(
             self._booster_handle,
             Native._make_pointer(update_scores, np.float64, len(shape)),
         )
         if return_code:  # pragma: no cover
             raise Native._get_native_exception(return_code, "GetTermUpdate")
 
-        n_dimensions = len(self.term_features[self._term_idx])
-        temp_transpose = [*range(n_dimensions - 1, -1, -1)]
-        if len(shape) != n_dimensions:  # multiclass
-            temp_transpose.append(len(temp_transpose))
-        update_scores = np.ascontiguousarray(
-            np.transpose(update_scores, tuple(temp_transpose))
-        )
         return update_scores
 
     def set_term_update(self, term_idx, update_scores):
         self._term_idx = -1
 
         if self._term_shapes is None:  # pragma: no cover
             if update_scores is None:  # pragma: no cover
@@ -1582,22 +1567,14 @@
                 return
             raise ValueError(
                 "a tensor with 1 class or less would be empty since the predictions would always be the same"
             )
 
         shape = self._term_shapes[term_idx]
 
-        n_dimensions = len(self.term_features[term_idx])
-        temp_transpose = [*range(n_dimensions - 1, -1, -1)]
-        if len(shape) != n_dimensions:  # multiclass
-            temp_transpose.append(len(temp_transpose))
-        update_scores = np.ascontiguousarray(
-            np.transpose(update_scores, tuple(temp_transpose))
-        )
-
         if shape != update_scores.shape:  # pragma: no cover
             raise ValueError("incorrect tensor shape in call to set_term_update")
 
         native = Native.get_native_singleton()
         return_code = native._unsafe.SetTermUpdate(
             self._booster_handle,
             term_idx,
```

### Comparing `interpret-core-0.4.1/interpret/utils/_preprocessor.py` & `interpret-core-0.4.2/interpret/utils/_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,21 +143,29 @@
                 _log.error(msg)
                 raise ValueError(msg)
             n_samples = len(sample_weight)
             sample_weight = sample_weight.astype(np.float64, copy=False)
 
             # NaN values are guaranteed to be the min if they exist
             min_weight = sample_weight.min()
-            # TODO: for now weights of zero are illegal, but in the future accept them
-            if (
-                math.isnan(min_weight)
-                or min_weight <= 0
-                or math.isinf(sample_weight.max())
-            ):
-                msg = "illegal sample_weight value"
+            if math.isnan(min_weight):
+                msg = "illegal NaN sample_weight value"
+                _log.error(msg)
+                raise ValueError(msg)
+            if math.isinf(sample_weight.max()):
+                msg = "illegal +infinity sample_weight value"
+                _log.error(msg)
+                raise ValueError(msg)
+            if min_weight < 0:
+                msg = "illegal negative sample_weight value"
+                _log.error(msg)
+                raise ValueError(msg)
+            if min_weight == 0:
+                # TODO: for now weights of zero are illegal, but in the future accept them
+                msg = "illegal sample_weight value of zero"
                 _log.error(msg)
                 raise ValueError(msg)
 
         X, n_samples = preclean_X(
             X,
             self.feature_names,
             self.feature_types,
@@ -284,14 +292,17 @@
                         is_privacy_bounds_warning = True
                         min_feature_val = np.nanmin(X_col)
 
                     if math.isnan(max_feature_val):
                         is_privacy_bounds_warning = True
                         max_feature_val = np.nanmax(X_col)
 
+                    # TODO: instead of passing in "max_bins - 1" should we be passing in "max_bins - 2"?
+                    #       It's not a big deal since it doesn't cause an error, and I don't want to
+                    #       change the results right now, but clean this up eventually
                     cuts, feature_bin_weights = private_numeric_binning(
                         X_col,
                         sample_weight,
                         noise_scale,
                         max_bins - 1,
                         min_feature_val,
                         max_feature_val,
@@ -355,14 +366,17 @@
                         raise ValueError(msg)
 
                     if feature_type_given is None:
                         # if auto-detected then we need to show a privacy warning
                         is_privacy_types_warning = True
 
                     # TODO: clean up this hack that uses strings of the indexes
+                    # TODO: instead of passing in "max_bins - 1" should we be passing in "max_bins - 2"?
+                    #       It's not a big deal since it doesn't cause an error, and I don't want to
+                    #       change the results right now, but clean this up eventually
                     keep_bins, old_feature_bin_weights = private_categorical_binning(
                         X_col, sample_weight, noise_scale, max_bins - 1, rng
                     )
                     unknown_weight = 0
                     if keep_bins[-1] == "DPOther":
                         unknown_weight = old_feature_bin_weights[-1]
                         keep_bins = keep_bins[:-1]
@@ -473,14 +487,19 @@
 
                     if not X_col.flags.c_contiguous:
                         # X_col could be a slice that has a stride.  We need contiguous for caling into C
                         X_col = X_col.copy()
 
                     X_col = native.discretize(X_col, bins)
 
+                if np.count_nonzero(X_col) != len(X_col):
+                    msg = "missing values in X not supported in transform"
+                    _log.error(msg)
+                    raise ValueError(msg)
+
                 X_binned[:, feature_idx] = X_col
 
         return X_binned
 
     def fit_transform(self, X, y=None, sample_weight=None):
         """Fits and Transform on provided samples.
```

### Comparing `interpret-core-0.4.1/interpret/utils/_privacy.py` & `interpret-core-0.4.2/interpret/utils/_privacy.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,14 +51,22 @@
     sample_weight,
     noise_scale,
     max_bins,
     min_feature_val,
     max_feature_val,
     rng=None,
 ):
+    # TODO: a few ways to improve this function:
+    #   - it prefers the leftmost bin since it starts from there and accumulates
+    #   - we are not guaranteed max_bins bins.  We could have more or less.  If for example all the
+    #     noise were positive by chance, more could be above target_weight than planned. On the opposite
+    #     side we could have badly placed weights and collapse more than required. The noisy bin weights
+    #     are public information after the noise has been added, so we can use much more aggressively optimizing
+    #     algorithms to more evently distribute the weight
+
     native = Native.get_native_singleton()
     uniform_weights, uniform_edges = np.histogram(
         X_col,
         bins=max_bins * 2,
         range=(min_feature_val, max_feature_val),
         weights=sample_weight,
     )
```

### Comparing `interpret-core-0.4.1/interpret/utils/_rank_interactions.py` & `interpret-core-0.4.2/interpret/utils/_rank_interactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,31 +24,34 @@
     max_cardinality,
     min_samples_leaf,
     is_private,
     objective,
     experimental_params=None,
     n_output_interactions=0,
 ):
-    interaction_strengths = []
-    with InteractionDetector(
-        dataset, bag, init_scores, is_private, objective, experimental_params
-    ) as interaction_detector:
-        for feature_idxs in iter_term_features:
-            if tuple(sorted(feature_idxs)) in exclude:
-                continue
-            strength = interaction_detector.calc_interaction_strength(
-                feature_idxs,
-                interaction_flags,
-                max_cardinality,
-                min_samples_leaf,
-            )
-            item = (strength, feature_idxs)
-            if n_output_interactions <= 0:
-                interaction_strengths.append(item)
-            else:
-                if len(interaction_strengths) == n_output_interactions:
-                    heapq.heappushpop(interaction_strengths, item)
+    try:
+        interaction_strengths = []
+        with InteractionDetector(
+            dataset, bag, init_scores, is_private, objective, experimental_params
+        ) as interaction_detector:
+            for feature_idxs in iter_term_features:
+                if tuple(sorted(feature_idxs)) in exclude:
+                    continue
+                strength = interaction_detector.calc_interaction_strength(
+                    feature_idxs,
+                    interaction_flags,
+                    max_cardinality,
+                    min_samples_leaf,
+                )
+                item = (strength, feature_idxs)
+                if n_output_interactions <= 0:
+                    interaction_strengths.append(item)
                 else:
-                    heapq.heappush(interaction_strengths, item)
+                    if len(interaction_strengths) == n_output_interactions:
+                        heapq.heappushpop(interaction_strengths, item)
+                    else:
+                        heapq.heappush(interaction_strengths, item)
 
-    interaction_strengths.sort(reverse=True)
-    return interaction_strengths
+        interaction_strengths.sort(reverse=True)
+        return interaction_strengths
+    except Exception as e:
+        return e
```

### Comparing `interpret-core-0.4.1/interpret/utils/_seed.py` & `interpret-core-0.4.2/interpret/utils/_seed.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_shap_common.py` & `interpret-core-0.4.2/interpret/utils/_shap_common.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_unify_data.py` & `interpret-core-0.4.2/interpret/utils/_unify_data.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/utils/_unify_predict.py` & `interpret-core-0.4.2/interpret/utils/_unify_predict.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/visual/_inline.py` & `interpret-core-0.4.2/interpret/visual/_inline.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/visual/_interactive.py` & `interpret-core-0.4.2/interpret/visual/_interactive.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/visual/_udash.py` & `interpret-core-0.4.2/interpret/visual/_udash.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/visual/assets/favicon.ico` & `interpret-core-0.4.2/interpret/visual/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/visual/assets/udash.css` & `interpret-core-0.4.2/interpret/visual/assets/udash.css`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/visual/assets/udash.js` & `interpret-core-0.4.2/interpret/visual/assets/udash.js`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/visual/dashboard.py` & `interpret-core-0.4.2/interpret/visual/dashboard.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret/visual/plot.py` & `interpret-core-0.4.2/interpret/visual/plot.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret_core.egg-info/PKG-INFO` & `interpret-core-0.4.2/interpret_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret-core
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fit interpretable models. Explain blackbox machine learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `interpret-core-0.4.1/interpret_core.egg-info/SOURCES.txt` & `interpret-core-0.4.2/interpret_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret_core.egg-info/entry_points.txt` & `interpret-core-0.4.2/interpret_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/interpret_core.egg-info/requires.txt` & `interpret-core-0.4.2/interpret_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/setup.py` & `interpret-core-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from distutils.command.install import install
 
 from setuptools import setup, find_packages
 from setuptools.command.sdist import sdist
 
 name = "interpret-core"
 # NOTE: Version is replaced by a regex script.
-version = "0.4.1"
+version = "0.4.2"
 long_description = """
 Core system for the interpret package.
 
 https://github.com/interpretml/interpret
 """
 
 entry_points = {
```

### Comparing `interpret-core-0.4.1/symbolic/LICENSE` & `interpret-core-0.4.2/symbolic/LICENSE`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/README.md` & `interpret-core-0.4.2/symbolic/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -620,15 +620,17 @@
 - [Targeting resources efficiently and justifiably by combining causal machine learning and theory](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9768181/pdf/frai-05-1015604.pdf)
 - [Extractive Text Summarization Using Generalized Additive Models with Interactions for Sentence Selection](https://arxiv.org/pdf/2212.10707.pdf)
 - [Death by Round Numbers: Glass-Box Machine Learning Uncovers Biases in Medical Practice](https://www.medrxiv.org/content/medrxiv/early/2022/11/28/2022.04.30.22274520.full.pdf)
 - [Post-Hoc Interpretation of Transformer Hyperparameters with Explainable Boosting Machines](https://www.cs.jhu.edu/~xzhan138/papers/BLACK2022.pdf)
 - [Interpretable machine learning for predicting pathologic complete response in patients treated with chemoradiation therapy for rectal adenocarcinoma](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9771385/pdf/frai-05-1059033.pdf)
 - [Exploring the Balance between Interpretability and Performance with carefully designed Constrainable Neural Additive Models](https://deliverypdf.ssrn.com/delivery.php?ID=998105006000069122073098120102102121021040051018055094125029122011041003059093125102072122106122077081069015087124028097016003127095087091028087010007035098086102086081014043013113004081117108011028041097095064071100112069081100069120077067116088100069070097093080074087115080072064086111126&EXT=pdf&INDEX=TRUE)
 - [Estimating Discontinuous Time-Varying Risk Factors and Treatment Benefits for COVID-19 with Interpretable ML](https://arxiv.org/pdf/2211.08991.pdf)
+- [Extending Explainable Boosting Machines to Scientific Image Data](https://arxiv.org/pdf/2305.16526.pdf)
 - [Pest Presence Prediction Using Interpretable Machine Learning](https://arxiv.org/pdf/2205.07723.pdf)
+- [Key Thresholds and Relative Contributions of Knee Geometry, Anteroposterior Laxity, and Body Weight as Risk Factors for Noncontact ACL Injury](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10184233/pdf/10.1177_23259671231163627.pdf)
 - [epitope1D: Accurate Taxonomy-Aware B-Cell Linear Epitope Prediction](https://www.biorxiv.org/content/10.1101/2022.10.17.512613v1.full.pdf)
 - [Explainable Boosting Machines for Slope Failure Spatial Predictive Modeling](https://www.mdpi.com/2072-4292/13/24/4991/htm)
 - [Micromodels for Efficient, Explainable, and Reusable Systems: A Case Study on Mental Health](https://arxiv.org/pdf/2109.13770.pdf)
 - [Identifying main and interaction effects of risk factors to predict intensive care admission in patients hospitalized with COVID-19](https://www.medrxiv.org/content/10.1101/2020.06.30.20143651v1.full.pdf)
 - [Comparing the interpretability of machine learning classifiers for brain tumour survival prediction](https://deliverypdf.ssrn.com/delivery.php?ID=760122118067103094108090123091079011028032009009023085005014014002123105085114025022024005047078031019089073120012025117073002064031071072113006066035001068125027021087087083085026100009018045107092063001023068071002124070107120120007014102094103069089119026110104107005031095001092090&EXT=pdf&INDEX=TRUE)
 - [Using Interpretable Machine Learning to Predict Maternal and Fetal Outcomes](https://arxiv.org/pdf/2207.05322.pdf)
 - [Calibrate: Interactive Analysis of Probabilistic Model Output](https://arxiv.org/pdf/2207.13770.pdf)
```

#### html2text {}

```diff
@@ -443,26 +443,31 @@
 chemoradiation therapy for rectal adenocarcinoma](https://www.ncbi.nlm.nih.gov/
 pmc/articles/PMC9771385/pdf/frai-05-1059033.pdf) - [Exploring the Balance
 between Interpretability and Performance with carefully designed Constrainable
 Neural Additive Models](https://deliverypdf.ssrn.com/
 delivery.php?ID=998105006000069122073098120102102121021040051018055094125029122011041003059093125102072122106122077081069015087124028097016003127095087091028087010007035098086102086081014043013113004081117108011028041097095064071100112069081100069120077067116088100069070097093080074087115080072064086111126&EXT=pdf&INDEX=TRUE)
 - [Estimating Discontinuous Time-Varying Risk Factors and Treatment Benefits
 for COVID-19 with Interpretable ML](https://arxiv.org/pdf/2211.08991.pdf) -
-[Pest Presence Prediction Using Interpretable Machine Learning](https://
-arxiv.org/pdf/2205.07723.pdf) - [epitope1D: Accurate Taxonomy-Aware B-Cell
-Linear Epitope Prediction](https://www.biorxiv.org/content/10.1101/
-2022.10.17.512613v1.full.pdf) - [Explainable Boosting Machines for Slope
-Failure Spatial Predictive Modeling](https://www.mdpi.com/2072-4292/13/24/4991/
-htm) - [Micromodels for Efficient, Explainable, and Reusable Systems: A Case
-Study on Mental Health](https://arxiv.org/pdf/2109.13770.pdf) - [Identifying
-main and interaction effects of risk factors to predict intensive care
-admission in patients hospitalized with COVID-19](https://www.medrxiv.org/
-content/10.1101/2020.06.30.20143651v1.full.pdf) - [Comparing the
-interpretability of machine learning classifiers for brain tumour survival
-prediction](https://deliverypdf.ssrn.com/
+[Extending Explainable Boosting Machines to Scientific Image Data](https://
+arxiv.org/pdf/2305.16526.pdf) - [Pest Presence Prediction Using Interpretable
+Machine Learning](https://arxiv.org/pdf/2205.07723.pdf) - [Key Thresholds and
+Relative Contributions of Knee Geometry, Anteroposterior Laxity, and Body
+Weight as Risk Factors for Noncontact ACL Injury](https://www.ncbi.nlm.nih.gov/
+pmc/articles/PMC10184233/pdf/10.1177_23259671231163627.pdf) - [epitope1D:
+Accurate Taxonomy-Aware B-Cell Linear Epitope Prediction](https://
+www.biorxiv.org/content/10.1101/2022.10.17.512613v1.full.pdf) - [Explainable
+Boosting Machines for Slope Failure Spatial Predictive Modeling](https://
+www.mdpi.com/2072-4292/13/24/4991/htm) - [Micromodels for Efficient,
+Explainable, and Reusable Systems: A Case Study on Mental Health](https://
+arxiv.org/pdf/2109.13770.pdf) - [Identifying main and interaction effects of
+risk factors to predict intensive care admission in patients hospitalized with
+COVID-19](https://www.medrxiv.org/content/10.1101/
+2020.06.30.20143651v1.full.pdf) - [Comparing the interpretability of machine
+learning classifiers for brain tumour survival prediction](https://
+deliverypdf.ssrn.com/
 delivery.php?ID=760122118067103094108090123091079011028032009009023085005014014002123105085114025022024005047078031019089073120012025117073002064031071072113006066035001068125027021087087083085026100009018045107092063001023068071002124070107120120007014102094103069089119026110104107005031095001092090&EXT=pdf&INDEX=TRUE)
 - [Using Interpretable Machine Learning to Predict Maternal and Fetal Outcomes]
 (https://arxiv.org/pdf/2207.05322.pdf) - [Calibrate: Interactive Analysis of
 Probabilistic Model Output](https://arxiv.org/pdf/2207.13770.pdf) - [Neural
 Additive Models: Interpretable Machine Learning with Neural Nets](https://
 arxiv.org/pdf/2004.13912.pdf) - [NODE-GAM: Neural Generalized Additive Model
 for Interpretable Deep Learning](https://arxiv.org/pdf/2106.01613.pdf) -
```

### Comparing `interpret-core-0.4.1/symbolic/build.bat` & `interpret-core-0.4.2/symbolic/build.bat`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/build.sh` & `interpret-core-0.4.2/symbolic/build.sh`

 * *Files 2% similar despite different names*

```diff
@@ -264,53 +264,53 @@
    printf "%s\n" "CFLAGS=${CFLAGS}"
    printf "%s\n" "CXXFLAGS=${CXXFLAGS}"
 
    printf "%s\n" "LDFLAGS=${LDFLAGS}"
    printf "%s\n" "LOADLIBES=${LOADLIBES}"
    printf "%s\n" "LDLIBS=${LDLIBS}"
 
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/ApplyTermUpdate.cpp" -o "$tmp_path/ApplyTermUpdate.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/BinSumsBoosting.cpp" -o "$tmp_path/BinSumsBoosting.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/BinSumsInteraction.cpp" -o "$tmp_path/BinSumsInteraction.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/BoosterCore.cpp" -o "$tmp_path/BoosterCore.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/BoosterShell.cpp" -o "$tmp_path/BoosterShell.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/CalcInteractionStrength.cpp" -o "$tmp_path/CalcInteractionStrength.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/CutQuantile.cpp" -o "$tmp_path/CutQuantile.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/CutUniform.cpp" -o "$tmp_path/CutUniform.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/CutWinsorized.cpp" -o "$tmp_path/CutWinsorized.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/dataset_shared.cpp" -o "$tmp_path/dataset_shared.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/DataSetBoosting.cpp" -o "$tmp_path/DataSetBoosting.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/DataSetInteraction.cpp" -o "$tmp_path/DataSetInteraction.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/DetermineLinkFunction.cpp" -o "$tmp_path/DetermineLinkFunction.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/debug_ebm.cpp" -o "$tmp_path/debug_ebm.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/Discretize.cpp" -o "$tmp_path/Discretize.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/Term.cpp" -o "$tmp_path/Term.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/GenerateTermUpdate.cpp" -o "$tmp_path/GenerateTermUpdate.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/InitializeGradientsAndHessians.cpp" -o "$tmp_path/InitializeGradientsAndHessians.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/InteractionCore.cpp" -o "$tmp_path/InteractionCore.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/InteractionShell.cpp" -o "$tmp_path/InteractionShell.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/interpretable_numerics.cpp" -o "$tmp_path/interpretable_numerics.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/PartitionOneDimensionalBoosting.cpp" -o "$tmp_path/PartitionOneDimensionalBoosting.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/PartitionRandomBoosting.cpp" -o "$tmp_path/PartitionRandomBoosting.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/PartitionTwoDimensionalBoosting.cpp" -o "$tmp_path/PartitionTwoDimensionalBoosting.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/PartitionTwoDimensionalInteraction.cpp" -o "$tmp_path/PartitionTwoDimensionalInteraction.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/RandomDeterministic.cpp" -o "$tmp_path/RandomDeterministic.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/random.cpp" -o "$tmp_path/random.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/sampling.cpp" -o "$tmp_path/sampling.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/InnerBag.cpp" -o "$tmp_path/InnerBag.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/Tensor.cpp" -o "$tmp_path/Tensor.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/TensorTotalsBuild.cpp" -o "$tmp_path/TensorTotalsBuild.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/compute/Objective.cpp" -o "$tmp_path/Objective.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/compute/Registration.cpp" -o "$tmp_path/Registration.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/compute/zoned_bridge_c_functions.cpp" -o "$tmp_path/zoned_bridge_c_functions.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/compute/cpu_ebm/cpu_32.cpp" -o "$tmp_path/cpu_32.o"
-   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_main "$code_path/compute/cpu_ebm/cpu_64.cpp" -o "$tmp_path/cpu_64.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/ApplyTermUpdate.cpp" -o "$tmp_path/ApplyTermUpdate.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/BinSumsBoosting.cpp" -o "$tmp_path/BinSumsBoosting.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/BinSumsInteraction.cpp" -o "$tmp_path/BinSumsInteraction.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/BoosterCore.cpp" -o "$tmp_path/BoosterCore.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/BoosterShell.cpp" -o "$tmp_path/BoosterShell.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/CalcInteractionStrength.cpp" -o "$tmp_path/CalcInteractionStrength.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/CutQuantile.cpp" -o "$tmp_path/CutQuantile.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/CutUniform.cpp" -o "$tmp_path/CutUniform.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/CutWinsorized.cpp" -o "$tmp_path/CutWinsorized.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/dataset_shared.cpp" -o "$tmp_path/dataset_shared.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/DataSetBoosting.cpp" -o "$tmp_path/DataSetBoosting.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/DataSetInteraction.cpp" -o "$tmp_path/DataSetInteraction.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/DetermineLinkFunction.cpp" -o "$tmp_path/DetermineLinkFunction.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/debug_ebm.cpp" -o "$tmp_path/debug_ebm.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/Discretize.cpp" -o "$tmp_path/Discretize.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/Term.cpp" -o "$tmp_path/Term.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/GenerateTermUpdate.cpp" -o "$tmp_path/GenerateTermUpdate.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/InitializeGradientsAndHessians.cpp" -o "$tmp_path/InitializeGradientsAndHessians.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/InteractionCore.cpp" -o "$tmp_path/InteractionCore.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/InteractionShell.cpp" -o "$tmp_path/InteractionShell.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/interpretable_numerics.cpp" -o "$tmp_path/interpretable_numerics.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/PartitionOneDimensionalBoosting.cpp" -o "$tmp_path/PartitionOneDimensionalBoosting.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/PartitionRandomBoosting.cpp" -o "$tmp_path/PartitionRandomBoosting.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/PartitionTwoDimensionalBoosting.cpp" -o "$tmp_path/PartitionTwoDimensionalBoosting.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/PartitionTwoDimensionalInteraction.cpp" -o "$tmp_path/PartitionTwoDimensionalInteraction.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/RandomDeterministic.cpp" -o "$tmp_path/RandomDeterministic.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/random.cpp" -o "$tmp_path/random.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/sampling.cpp" -o "$tmp_path/sampling.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/InnerBag.cpp" -o "$tmp_path/InnerBag.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/Tensor.cpp" -o "$tmp_path/Tensor.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/TensorTotalsBuild.cpp" -o "$tmp_path/TensorTotalsBuild.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/compute/Objective.cpp" -o "$tmp_path/Objective.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/compute/Registration.cpp" -o "$tmp_path/Registration.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/compute/zoned_bridge_c_functions.cpp" -o "$tmp_path/zoned_bridge_c_functions.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/compute/cpu_ebm/cpu_32.cpp" -o "$tmp_path/cpu_32.o"
+   ${CXX} -c ${CPPFLAGS} ${CXXFLAGS} ${extras} -DZONE_cpu "$code_path/compute/cpu_ebm/cpu_64.cpp" -o "$tmp_path/cpu_64.o"
 
-   ${CC} -c ${CPPFLAGS} ${CFLAGS} ${extras} -DZONE_main "$code_path/common_c/common_c.c" -o "$tmp_path/common_c.o"
-   ${CC} -c ${CPPFLAGS} ${CFLAGS} ${extras} -DZONE_main "$code_path/common_c/logging.c" -o "$tmp_path/logging.o"
+   ${CC} -c ${CPPFLAGS} ${CFLAGS} ${extras} -DZONE_cpu "$code_path/common_c/common_c.c" -o "$tmp_path/common_c.o"
+   ${CC} -c ${CPPFLAGS} ${CFLAGS} ${extras} -DZONE_cpu "$code_path/common_c/logging.c" -o "$tmp_path/logging.o"
 
    ${CXX} ${LDFLAGS} -shared \
    "$tmp_path/ApplyTermUpdate.o" \
    "$tmp_path/BinSumsBoosting.o" \
    "$tmp_path/BinSumsInteraction.o" \
    "$tmp_path/BoosterCore.o" \
    "$tmp_path/BoosterShell.o" \
@@ -504,15 +504,15 @@
    
       g_all_object_files_sanitized=""
       g_compile_out_full=""
 
       make_initial_paths_simple "$obj_path_unsanitized" "$bin_path_unsanitized"
       compile_directory_c "$c_compiler" "$c_args_specific $common_args" "$src_path_unsanitized/common_c" "$obj_path_unsanitized" "$is_asm" "C"
       compile_directory_c "$c_compiler" "$c_args_specific $bridge_args" "$src_path_unsanitized/bridge_c" "$obj_path_unsanitized" "$is_asm" "C"
-      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_main" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "main"
+      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_cpu" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "avx512"
       compile_file "$cpp_compiler" "$cpp_args_specific" "$src_path_unsanitized"/special/linux_wrap_functions.cpp "$obj_path_unsanitized" "$is_asm" "NONE"
       link_file "$cpp_compiler" "$link_args_specific" "$bin_path_unsanitized" "$bin_file"
       printf "%s\n" "$g_compile_out_full"
       printf "%s\n" "$g_compile_out_full" > "$g_log_file_unsanitized"
       copy_bin_files "$bin_path_unsanitized" "$bin_file" "$python_lib_unsanitized" "$staging_path_unsanitized"
@@ -535,15 +535,15 @@
    
       g_all_object_files_sanitized=""
       g_compile_out_full=""
 
       make_initial_paths_simple "$obj_path_unsanitized" "$bin_path_unsanitized"
       compile_directory_c "$c_compiler" "$c_args_specific $common_args" "$src_path_unsanitized/common_c" "$obj_path_unsanitized" 0 "C"
       compile_directory_c "$c_compiler" "$c_args_specific $bridge_args" "$src_path_unsanitized/bridge_c" "$obj_path_unsanitized" 0 "C"
-      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_main" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "main"
+      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_cpu" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "avx512"
       compile_file "$cpp_compiler" "$cpp_args_specific" "$src_path_unsanitized"/special/linux_wrap_functions.cpp "$obj_path_unsanitized" 0 "NONE"
       link_file "$cpp_compiler" "$link_args_specific" "$bin_path_unsanitized" "$bin_file"
       printf "%s\n" "$g_compile_out_full"
       printf "%s\n" "$g_compile_out_full" > "$g_log_file_unsanitized"
       copy_bin_files "$bin_path_unsanitized" "$bin_file" "$python_lib_unsanitized" "$staging_path_unsanitized"
@@ -566,15 +566,15 @@
       g_all_object_files_sanitized=""
       g_compile_out_full=""
 
       make_initial_paths_simple "$obj_path_unsanitized" "$bin_path_unsanitized"
       check_install "$tmp_path_unsanitized" "g++-multilib"
       compile_directory_c "$c_compiler" "$c_args_specific $common_args" "$src_path_unsanitized/common_c" "$obj_path_unsanitized" 0 "C"
       compile_directory_c "$c_compiler" "$c_args_specific $bridge_args" "$src_path_unsanitized/bridge_c" "$obj_path_unsanitized" 0 "C"
-      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_main" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "main"
+      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_cpu" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "avx512"
       compile_file "$cpp_compiler" "$cpp_args_specific" "$src_path_unsanitized"/special/linux_wrap_functions.cpp "$obj_path_unsanitized" 0 "NONE"
       link_file "$cpp_compiler" "$link_args_specific" "$bin_path_unsanitized" "$bin_file"
       printf "%s\n" "$g_compile_out_full"
       printf "%s\n" "$g_compile_out_full" > "$g_log_file_unsanitized"
       copy_bin_files "$bin_path_unsanitized" "$bin_file" "$python_lib_unsanitized" "$staging_path_unsanitized"
@@ -597,15 +597,15 @@
       g_all_object_files_sanitized=""
       g_compile_out_full=""
 
       make_initial_paths_simple "$obj_path_unsanitized" "$bin_path_unsanitized"
       check_install "$tmp_path_unsanitized" "g++-multilib"
       compile_directory_c "$c_compiler" "$c_args_specific $common_args" "$src_path_unsanitized/common_c" "$obj_path_unsanitized" 0 "C"
       compile_directory_c "$c_compiler" "$c_args_specific $bridge_args" "$src_path_unsanitized/bridge_c" "$obj_path_unsanitized" 0 "C"
-      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_main" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "main"
+      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_cpu" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "avx512"
       compile_file "$cpp_compiler" "$cpp_args_specific" "$src_path_unsanitized"/special/linux_wrap_functions.cpp "$obj_path_unsanitized" 0 "NONE"
       link_file "$cpp_compiler" "$link_args_specific" "$bin_path_unsanitized" "$bin_file"
       printf "%s\n" "$g_compile_out_full"
       printf "%s\n" "$g_compile_out_full" > "$g_log_file_unsanitized"
       copy_bin_files "$bin_path_unsanitized" "$bin_file" "$python_lib_unsanitized" "$staging_path_unsanitized"
@@ -655,15 +655,15 @@
    
       g_all_object_files_sanitized=""
       g_compile_out_full=""
 
       make_initial_paths_simple "$obj_path_unsanitized" "$bin_path_unsanitized"
       compile_directory_c "$c_compiler" "$c_args_specific $common_args" "$src_path_unsanitized/common_c" "$obj_path_unsanitized" "$is_asm" "C"
       compile_directory_c "$c_compiler" "$c_args_specific $bridge_args" "$src_path_unsanitized/bridge_c" "$obj_path_unsanitized" "$is_asm" "C"
-      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_main" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "main"
+      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_cpu" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "avx512"
       link_file "$cpp_compiler" "$link_args_specific" "$bin_path_unsanitized" "$bin_file"
       printf "%s\n" "$g_compile_out_full"
       printf "%s\n" "$g_compile_out_full" > "$g_log_file_unsanitized"
       copy_bin_files "$bin_path_unsanitized" "$bin_file" "$python_lib_unsanitized" "$staging_path_unsanitized"
       copy_asm_files "$obj_path_unsanitized" "$tmp_path_unsanitized" "$staging_path_unsanitized/$bin_file" "asm_release_64" "$is_asm"
@@ -685,15 +685,15 @@
    
       g_all_object_files_sanitized=""
       g_compile_out_full=""
 
       make_initial_paths_simple "$obj_path_unsanitized" "$bin_path_unsanitized"
       compile_directory_c "$c_compiler" "$c_args_specific $common_args" "$src_path_unsanitized/common_c" "$obj_path_unsanitized" 0 "C"
       compile_directory_c "$c_compiler" "$c_args_specific $bridge_args" "$src_path_unsanitized/bridge_c" "$obj_path_unsanitized" 0 "C"
-      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_main" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "main"
+      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_cpu" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "avx512"
       link_file "$cpp_compiler" "$link_args_specific" "$bin_path_unsanitized" "$bin_file"
       printf "%s\n" "$g_compile_out_full"
       printf "%s\n" "$g_compile_out_full" > "$g_log_file_unsanitized"
       copy_bin_files "$bin_path_unsanitized" "$bin_file" "$python_lib_unsanitized" "$staging_path_unsanitized"
    fi
@@ -714,15 +714,15 @@
    
       g_all_object_files_sanitized=""
       g_compile_out_full=""
 
       make_initial_paths_simple "$obj_path_unsanitized" "$bin_path_unsanitized"
       compile_directory_c "$c_compiler" "$c_args_specific $common_args" "$src_path_unsanitized/common_c" "$obj_path_unsanitized" "$is_asm" "C"
       compile_directory_c "$c_compiler" "$c_args_specific $bridge_args" "$src_path_unsanitized/bridge_c" "$obj_path_unsanitized" "$is_asm" "C"
-      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_main" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "main"
+      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_cpu" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" "$is_asm" "cpu"
       link_file "$cpp_compiler" "$link_args_specific" "$bin_path_unsanitized" "$bin_file"
       printf "%s\n" "$g_compile_out_full"
       printf "%s\n" "$g_compile_out_full" > "$g_log_file_unsanitized"
       copy_bin_files "$bin_path_unsanitized" "$bin_file" "$python_lib_unsanitized" "$staging_path_unsanitized"
       copy_asm_files "$obj_path_unsanitized" "$tmp_path_unsanitized" "$staging_path_unsanitized/$bin_file" "asm_release_arm" "$is_asm"
    fi
@@ -743,15 +743,15 @@
    
       g_all_object_files_sanitized=""
       g_compile_out_full=""
 
       make_initial_paths_simple "$obj_path_unsanitized" "$bin_path_unsanitized"
       compile_directory_c "$c_compiler" "$c_args_specific $common_args" "$src_path_unsanitized/common_c" "$obj_path_unsanitized" 0 "C"
       compile_directory_c "$c_compiler" "$c_args_specific $bridge_args" "$src_path_unsanitized/bridge_c" "$obj_path_unsanitized" 0 "C"
-      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_main" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "main"
+      compile_directory_cpp "$cpp_compiler" "$cpp_args_specific $main_args -DZONE_cpu" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       compile_compute "$cpp_compiler" "$cpp_args_specific $compute_args" "$src_path_sanitized" "$src_path_unsanitized" "$obj_path_unsanitized" 0 "cpu"
       link_file "$cpp_compiler" "$link_args_specific" "$bin_path_unsanitized" "$bin_file"
       printf "%s\n" "$g_compile_out_full"
       printf "%s\n" "$g_compile_out_full" > "$g_log_file_unsanitized"
       copy_bin_files "$bin_path_unsanitized" "$bin_file" "$python_lib_unsanitized" "$staging_path_unsanitized"
    fi
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/ApplyTermUpdate.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/ApplyTermUpdate.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 #include <stddef.h> // size_t, ptrdiff_t
 #include <string.h> // memcpy
 
 #include "libebm.h" // ErrorEbm
 #include "logging.h" // EBM_ASSERT
 #include "zones.h"
 
-#include "Transpose.hpp"
-
 #include "Feature.hpp"
 #include "Term.hpp"
+#include "Transpose.hpp"
 #include "Tensor.hpp"
 #include "BoosterCore.hpp"
 #include "BoosterShell.hpp"
 
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
 #error DEFINED_ZONE_NAME must be defined
@@ -136,15 +135,15 @@
    if(0 != pBoosterCore->GetTrainingSet()->GetCountSamples()) {
       ApplyUpdateBridge data;
       data.m_cScores = GetCountScores(pBoosterCore->GetCountClasses());
       data.m_cPack = pTerm->GetTermBitPack();
       data.m_bHessianNeeded = EBM_TRUE;
       data.m_bCalcMetric = false;
       data.m_aMulticlassMidwayTemp = pBoosterShell->GetMulticlassMidwayTemp();
-      data.m_aUpdateTensorScores = pBoosterShell->GetTermUpdate()->GetTensorScoresPointer();
+      data.m_aUpdateTensorScores = aUpdateScores;
       data.m_cSamples = pBoosterCore->GetTrainingSet()->GetCountSamples();
       data.m_aPacked = pBoosterCore->GetTrainingSet()->GetInputDataPointer(iTerm);
       data.m_aTargets = pBoosterCore->GetTrainingSet()->GetTargetDataPointer();
       data.m_aWeights = nullptr;
       data.m_aSampleScores = pBoosterCore->GetTrainingSet()->GetSampleScores();
       data.m_aGradientsAndHessians = pBoosterCore->GetTrainingSet()->GetGradientsAndHessiansPointer();
       error = pBoosterCore->ObjectiveApplyUpdate(&data);
@@ -168,15 +167,15 @@
 
       ApplyUpdateBridge data;
       data.m_cScores = GetCountScores(pBoosterCore->GetCountClasses());
       data.m_cPack = pTerm->GetTermBitPack();
       data.m_bHessianNeeded = EBM_TRUE;
       data.m_bCalcMetric = true;
       data.m_aMulticlassMidwayTemp = pBoosterShell->GetMulticlassMidwayTemp();
-      data.m_aUpdateTensorScores = pBoosterShell->GetTermUpdate()->GetTensorScoresPointer();
+      data.m_aUpdateTensorScores = aUpdateScores;
       data.m_cSamples = pBoosterCore->GetValidationSet()->GetCountSamples();
       data.m_aPacked = pBoosterCore->GetValidationSet()->GetInputDataPointer(iTerm);
       data.m_aTargets = pBoosterCore->GetValidationSet()->GetTargetDataPointer();
       data.m_aWeights = pBoosterCore->GetValidationWeights();
       data.m_aSampleScores = pBoosterCore->GetValidationSet()->GetSampleScores();
       data.m_aGradientsAndHessians = pBoosterCore->GetValidationSet()->GetGradientsAndHessiansPointer();
       error = pBoosterCore->ObjectiveApplyUpdate(&data);
@@ -261,30 +260,30 @@
 // times than desired, but we can live with that
 static int g_cLogGetTermUpdateSplits = 10;
 
 EBM_API_BODY ErrorEbm EBM_CALLING_CONVENTION GetTermUpdateSplits(
    BoosterHandle boosterHandle,
    IntEbm indexDimension,
    IntEbm * countSplitsInOut,
-   IntEbm * splitIndexesOut
+   IntEbm * splitsOut
 ) {
    LOG_COUNTED_N(
       &g_cLogGetTermUpdateSplits,
       Trace_Info,
       Trace_Verbose,
       "GetTermUpdateSplits: "
       "boosterHandle=%p, "
       "indexDimension=%" IntEbmPrintf ", "
       "countSplitsInOut=%p"
-      "splitIndexesOut=%p"
+      "splitsOut=%p"
       ,
       static_cast<void *>(boosterHandle),
       indexDimension, 
       static_cast<void *>(countSplitsInOut),
-      static_cast<void *>(splitIndexesOut)
+      static_cast<void *>(splitsOut)
    );
 
    if(nullptr == countSplitsInOut) {
       LOG_0(Trace_Error, "ERROR GetTermUpdateSplits countSplitsInOut cannot be nullptr");
       return Error_IllegalParamVal;
    }
 
@@ -315,63 +314,70 @@
    if(static_cast<IntEbm>(pTerm->GetCountDimensions()) <= indexDimension) {
       *countSplitsInOut = IntEbm { 0 };
       LOG_0(Trace_Error, "ERROR GetTermUpdateSplits indexDimension above the number of dimensions that we have");
       return Error_IllegalParamVal;
    }
    const size_t iDimension = static_cast<size_t>(indexDimension);
 
-   size_t cBins = pTerm->GetFeatures()[iDimension]->GetCountBins();
+   size_t cBins = pTerm->GetTermFeatures()[iDimension].m_pFeature->GetCountBins();
+   const bool bMissing = pTerm->GetTermFeatures()[iDimension].m_pFeature->IsMissing();
+   const bool bUnknown = pTerm->GetTermFeatures()[iDimension].m_pFeature->IsUnknown();
+   cBins += bMissing ? size_t { 0 } : size_t { 1 };
+   cBins += bUnknown ? size_t { 0 } : size_t { 1 };
    cBins = size_t { 0 } == cBins ? size_t { 1 } : cBins; // for our purposes here, 0 bins means 0 splits
 
    // cBins started from IntEbm, so we should be able to convert back safely
    if(*countSplitsInOut != static_cast<IntEbm>(cBins - size_t { 1 })) {
       *countSplitsInOut = IntEbm { 0 };
       LOG_0(Trace_Error, "ERROR GetTermUpdateSplits bad split array length");
       return Error_IllegalParamVal;
    }
 
    if(ptrdiff_t { 0 } == pBoosterCore->GetCountClasses() || ptrdiff_t { 1 } == pBoosterCore->GetCountClasses()) {
       // if we have 0 or 1 classes then there is no tensor, so return now
       *countSplitsInOut = 0;
-      LOG_0(Trace_Warning, "ERROR GetTermUpdateSplits ptrdiff_t { 0 } == pBoosterCore->GetCountClasses() || ptrdiff_t { 1 } == pBoosterCore->GetCountClasses()");
+      LOG_0(Trace_Warning, "WARNING GetTermUpdateSplits ptrdiff_t { 0 } == pBoosterCore->GetCountClasses() || ptrdiff_t { 1 } == pBoosterCore->GetCountClasses()");
       return Error_None;
    }
    EBM_ASSERT(nullptr != pBoosterShell->GetTermUpdate());
 
    if(size_t { 0 } == pTerm->GetCountTensorBins()) {
       // if we have zero samples and one of the dimensions has 0 bins then there is no tensor, so return now
 
       // if GetCountTensorBins is 0, then pBoosterShell->GetTermUpdate() does not contain valid data
 
       *countSplitsInOut = 0;
-      LOG_0(Trace_Warning, "ERROR GetTermUpdateSplits size_t { 0 } == pTerm->GetCountTensorBins()");
+      LOG_0(Trace_Warning, "WARNING GetTermUpdateSplits size_t { 0 } == pTerm->GetCountTensorBins()");
       return Error_None;
    }
 
-   const size_t cSplits = pBoosterShell->GetTermUpdate()->GetCountSplits(iDimension);
+   const size_t cSplits = pBoosterShell->GetTermUpdate()->GetCountSlices(iDimension) - 1;
    EBM_ASSERT(cSplits < cBins);
    if(0 != cSplits) {
-      if(nullptr == splitIndexesOut) {
+      if(nullptr == splitsOut) {
          *countSplitsInOut = IntEbm { 0 };
-         LOG_0(Trace_Error, "ERROR GetTermUpdateSplits splitIndexesOut cannot be nullptr");
+         LOG_0(Trace_Error, "ERROR GetTermUpdateSplits splitsOut cannot be nullptr");
          return Error_IllegalParamVal;
       }
 
-      const ActiveDataType * pSplitIndexesFrom = pBoosterShell->GetTermUpdate()->GetSplitPointer(iDimension);
-      IntEbm * pSplitIndexesTo = splitIndexesOut;
-      IntEbm * pSplitIndexesToEnd = splitIndexesOut + cSplits;
+      const ActiveDataType indexEdgeAdd = bMissing ? size_t { 0 } : size_t { 1 };
+
+      const ActiveDataType * pFrom = pBoosterShell->GetTermUpdate()->GetSplitPointer(iDimension);
+      IntEbm * pTo = splitsOut;
+      IntEbm * pToEnd = splitsOut + cSplits;
       do {
-         const ActiveDataType indexSplit = *pSplitIndexesFrom;
-         ++pSplitIndexesFrom;
+         // if the missing bin was eliminated, we need to increment our split indexes
+         const ActiveDataType indexEdge = *pFrom + indexEdgeAdd;
+         ++pFrom;
 
-         EBM_ASSERT(!IsConvertError<IntEbm>(indexSplit)); // the total count works so the index should too
-         *pSplitIndexesTo = static_cast<IntEbm>(indexSplit);
+         EBM_ASSERT(!IsConvertError<IntEbm>(indexEdge)); // the total count works so the index should too
+         *pTo = static_cast<IntEbm>(indexEdge);
 
-         ++pSplitIndexesTo;
-      } while(pSplitIndexesToEnd != pSplitIndexesTo);
+         ++pTo;
+      } while(pToEnd != pTo);
    }
    EBM_ASSERT(!IsConvertError<IntEbm>(cSplits)); // cSplits originally came from an IntEbm
    *countSplitsInOut = static_cast<IntEbm>(cSplits);
    return Error_None;
 }
 
 // we made this a global because if we had put this variable inside the BoosterCore object, then we would need to dereference that before 
@@ -419,35 +425,33 @@
    }
    EBM_ASSERT(nullptr != pBoosterShell->GetTermUpdate());
 
    const Term * const pTerm = pBoosterCore->GetTerms()[iTerm];
 
    size_t cTensorScores = pTerm->GetCountTensorBins();
    if(size_t { 0 } == cTensorScores) {
-      // if we have zero samples and one of the dimensions has 0 bins then there is no tensor, so return now
+      // If we have zero samples and one of the dimensions has 0 bins then there is no tensor, so return now
+      // In theory it might be better to zero out the caller's tensor cells (2 ^ n_dimensions), but this condition
+      // is almost an error already, so don't try reading/writing memory. We just define this situation as
+      // having a zero sized tensor result. The caller can zero their own memory if they want it zero
 
       // if GetCountTensorBins is 0, then pBoosterShell->GetTermUpdate() does not contain valid data
 
+      LOG_0(Trace_Warning, "WARNING GetTermUpdate size_t { 0 } == cTensorScores");
       return Error_None;
    }
 
    error = pBoosterShell->GetTermUpdate()->Expand(pTerm);
    if(Error_None != error) {
       return error;
    }
 
-   EBM_ASSERT(!IsMultiplyError(cTensorScores, GetCountScores(pBoosterCore->GetCountClasses())));
-   cTensorScores *= GetCountScores(pBoosterCore->GetCountClasses());
+   FloatFast * const aUpdateScores = pBoosterShell->GetTermUpdate()->GetTensorScoresPointer();
+   Transpose<true>(pTerm, GetCountScores(pBoosterCore->GetCountClasses()), updateScoresTensorOut, aUpdateScores);
 
-   const FloatFast * const aUpdateScores = pBoosterShell->GetTermUpdate()->GetTensorScoresPointer();
-   // we've allocated this memory, so it should be reachable, so these numbers should multiply
-   EBM_ASSERT(!IsMultiplyError(sizeof(*updateScoresTensorOut), cTensorScores));
-   EBM_ASSERT(!IsMultiplyError(sizeof(*aUpdateScores), cTensorScores));
-   static_assert(sizeof(*updateScoresTensorOut) == sizeof(*aUpdateScores), "float mismatch");
-   memcpy(updateScoresTensorOut, aUpdateScores, sizeof(*aUpdateScores) * cTensorScores);
    return Error_None;
 }
 
 // we made this a global because if we had put this variable inside the BoosterCore object, then we would need to dereference that before 
 // getting the count.  By making this global we can send a log message incase a bad BoosterCore object is sent into us
 // we only decrease the count if the count is non-zero, so at worst if there is a race condition then we'll output this log message more 
 // times than desired, but we can live with that
@@ -493,15 +497,15 @@
       // we wouldn't have allowed the creation of an feature set larger than size_t
       LOG_0(Trace_Error, "ERROR SetTermUpdate indexTerm is too high to index");
       return Error_IllegalParamVal;
    }
    const size_t iTerm = static_cast<size_t>(indexTerm);
    if(pBoosterCore->GetCountTerms() <= iTerm) {
       pBoosterShell->SetTermIndex(BoosterShell::k_illegalTermIndex);
-      LOG_0(Trace_Error, "ERROR SetTermUpdate indexTerm above the number of feature groups that we have");
+      LOG_0(Trace_Error, "ERROR SetTermUpdate indexTerm above the number of terms that we have");
       return Error_IllegalParamVal;
    }
 
    if(ptrdiff_t { 0 } == pBoosterCore->GetCountClasses() || ptrdiff_t { 1 } == pBoosterCore->GetCountClasses()) {
       pBoosterShell->SetTermIndex(iTerm);
       return Error_None;
    }
@@ -509,18 +513,19 @@
 
    // pBoosterCore->GetTerms() can be null if 0 == pBoosterCore->m_cTerms, but we checked that condition above
    EBM_ASSERT(nullptr != pBoosterCore->GetTerms());
    const Term * const pTerm = pBoosterCore->GetTerms()[iTerm];
 
    size_t cTensorScores = pTerm->GetCountTensorBins();
    if(size_t { 0 } == cTensorScores) {
-      // if we have zero samples and one of the dimensions has 0 bins then there is no tensor, so return now
+      // If we have zero samples and one of the dimensions has 0 bins then there is no tensor, so return now
 
-      // if GetCountTensorBins is 0, then we leave pBoosterShell->GetTermUpdate() with invalid data since
-      // out Tensor class does not support tensors of zero elements
+      // if GetCountTensorBins is 0, then pBoosterShell->GetTermUpdate() does not contain valid data
+
+      LOG_0(Trace_Warning, "WARNING SetTermUpdate size_t { 0 } == cTensorScores");
 
       pBoosterShell->SetTermIndex(iTerm);
       return Error_None;
    }
 
    pBoosterShell->GetTermUpdate()->SetCountDimensions(pTerm->GetCountDimensions());
    pBoosterShell->GetTermUpdate()->Reset();
@@ -528,22 +533,18 @@
    error = pBoosterShell->GetTermUpdate()->Expand(pTerm);
    if(Error_None != error) {
       // already logged
       pBoosterShell->SetTermIndex(BoosterShell::k_illegalTermIndex);
       return error;
    }
 
-   EBM_ASSERT(!IsMultiplyError(cTensorScores, GetCountScores(pBoosterCore->GetCountClasses())));
-   cTensorScores *= GetCountScores(pBoosterCore->GetCountClasses());
-
    FloatFast * const aUpdateScores = pBoosterShell->GetTermUpdate()->GetTensorScoresPointer();
-   EBM_ASSERT(!IsMultiplyError(sizeof(*aUpdateScores), cTensorScores));
-   EBM_ASSERT(!IsMultiplyError(sizeof(*updateScoresTensor), cTensorScores));
-   static_assert(sizeof(*updateScoresTensor) == sizeof(*aUpdateScores), "float mismatch");
-   memcpy(aUpdateScores, updateScoresTensor, sizeof(*aUpdateScores) * cTensorScores);
+   // *updateScoresTensor is const, but Transpose can go either way.  When bCopyToIncrement is false like it
+   // is below, then Transpose will treat updateScoresTensor as const
+   Transpose<false>(pTerm, GetCountScores(pBoosterCore->GetCountClasses()), const_cast<double *>(updateScoresTensor), aUpdateScores);
 
    pBoosterShell->SetTermIndex(iTerm);
 
    return Error_None;
 }
 
 } // DEFINED_ZONE_NAME
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/BinSumsBoosting.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/BinSumsBoosting.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/BinSumsInteraction.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/BinSumsInteraction.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/BoosterCore.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/BoosterCore.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,15 @@
    }
    LOG_0(Trace_Info, "BoosterCore::Create done feature processing");
 
    size_t cFastBinsMax = 0;
    size_t cBigBinsMax = 0;
    size_t cSingleDimensionBinsMax = 0;
 
-   LOG_0(Trace_Info, "BoosterCore::Create starting feature group processing");
+   LOG_0(Trace_Info, "BoosterCore::Create starting term processing");
    if(0 != cTerms) {
       pBoosterCore->m_cTerms = cTerms;
       pBoosterCore->m_apTerms = Term::AllocateTerms(cTerms);
       if(UNLIKELY(nullptr == pBoosterCore->m_apTerms)) {
          LOG_0(Trace_Warning, "WARNING BoosterCore::Create 0 != m_cTerms && nullptr == m_apTerms");
          return Error_OutOfMemory;
       }
@@ -355,15 +355,15 @@
       do {
          const IntEbm countDimensions = acTermDimensions[iTerm];
          if(countDimensions < IntEbm { 0 }) {
             LOG_0(Trace_Error, "ERROR BoosterCore::Create countDimensions cannot be negative");
             return Error_IllegalParamVal;
          }
          if(IntEbm { k_cDimensionsMax } < countDimensions) {
-            LOG_0(Trace_Error, "WARNING BoosterCore::Create countDimensions too large and would cause out of memory condition");
+            LOG_0(Trace_Warning, "WARNING BoosterCore::Create countDimensions too large and would cause out of memory condition");
             return Error_OutOfMemory;
          }
          const size_t cDimensions = static_cast<size_t>(countDimensions);
          Term * const pTerm = Term::Allocate(cDimensions);
          if(nullptr == pTerm) {
             LOG_0(Trace_Warning, "WARNING BoosterCore::Create nullptr == pTerm");
             return Error_OutOfMemory;
@@ -374,26 +374,30 @@
          pTerm->SetCountAuxillaryBins(0); // we only use these for pairs, so otherwise it gets left as zero
 
          size_t cAuxillaryBinsForBuildFastTotals = 0;
          size_t cRealDimensions = 0;
          ptrdiff_t cItemsPerBitPack = k_cItemsPerBitPackNone;
          size_t cTensorBins = 1;
          if(UNLIKELY(0 == cDimensions)) {
-            LOG_0(Trace_Info, "INFO BoosterCore::Create empty feature group");
+            LOG_0(Trace_Info, "INFO BoosterCore::Create empty term");
 
             cFastBinsMax = EbmMax(cFastBinsMax, size_t { 1 });
             cBigBinsMax = EbmMax(cBigBinsMax, size_t { 1 });
          } else {
             if(nullptr == piTermFeature) {
                LOG_0(Trace_Error, "ERROR BoosterCore::Create aiTermFeatures is null when there are Terms with non-zero numbers of features");
                return Error_IllegalParamVal;
             }
             size_t cSingleDimensionBins = 0;
-            const FeatureBoosting ** ppFeature = pTerm->GetFeatures();
-            const FeatureBoosting * const * const ppFeaturesEnd = &ppFeature[cDimensions];
+            TermFeature * pTermFeature = pTerm->GetTermFeatures();
+            const TermFeature * const pTermFeaturesEnd = &pTermFeature[cDimensions];
+            // TODO: Ideally we would flip our input dimensions so that we're aligned with the output ordering
+            //       and thus not need a transpose when transfering data to the caller. We're doing it this way
+            //       for now to test the transpose ability and also to maintain the same results as before for comparison
+            size_t iTranspose = cDimensions - 1;
             do {
                const IntEbm indexFeature = *piTermFeature;
                if(indexFeature < 0) {
                   LOG_0(Trace_Error, "ERROR BoosterCore::Create aiTermFeatures value cannot be negative");
                   return Error_IllegalParamVal;
                }
                if(IsConvertError<size_t>(indexFeature)) {
@@ -407,15 +411,17 @@
                   return Error_IllegalParamVal;
                }
 
                EBM_ASSERT(1 <= cFeatures); // since our iFeature is valid and index 0 would mean cFeatures == 1
                EBM_ASSERT(nullptr != pBoosterCore->m_aFeatures);
 
                const FeatureBoosting * const pInputFeature = &pBoosterCore->m_aFeatures[iFeature];
-               *ppFeature = pInputFeature;
+               pTermFeature->m_pFeature = pInputFeature;
+               pTermFeature->m_cStride = cTensorBins;
+               pTermFeature->m_iTranspose = iTranspose; // TODO: no tranposition yet, but move it from python to C
 
                const size_t cBins = pInputFeature->GetCountBins();
                if(LIKELY(size_t { 1 } < cBins)) {
                   // if we have only 1 bin, then we can eliminate the feature from consideration since the resulting tensor loses one dimension but is 
                   // otherwise indistinquishable from the original data
                   ++cRealDimensions;
 
@@ -432,23 +438,24 @@
 
                   // since cBins must be 2 or more, cAuxillaryBinsForBuildFastTotals must grow slower than 
                   // cTensorBins, and we checked above that cTensorBins would not overflow
                   EBM_ASSERT(!IsAddError(cAuxillaryBinsForBuildFastTotals, cTensorBins));
 
                   cAuxillaryBinsForBuildFastTotals += cTensorBins;
                } else {
-                  LOG_0(Trace_Info, "INFO BoosterCore::Create feature group with no useful features");
+                  LOG_0(Trace_Info, "INFO BoosterCore::Create term with no useful features");
                }
                cTensorBins *= cBins;
                // same reasoning as above: cAuxillaryBinsForBuildFastTotals grows slower than cTensorBins
                EBM_ASSERT(0 == cTensorBins || cAuxillaryBinsForBuildFastTotals < cTensorBins);
 
+               --iTranspose;
                ++piTermFeature;
-               ++ppFeature;
-            } while(ppFeaturesEnd != ppFeature);
+               ++pTermFeature;
+            } while(pTermFeaturesEnd != pTermFeature);
 
             if(LIKELY(size_t { 0 } != cTensorBins)) {
                cFastBinsMax = EbmMax(cFastBinsMax, cTensorBins);
 
                size_t cTotalBigBins = cTensorBins;
                if(LIKELY(size_t { 1 } != cTensorBins)) {
                   EBM_ASSERT(1 <= cRealDimensions);
@@ -495,15 +502,15 @@
          pTerm->SetCountRealDimensions(cRealDimensions);
          pTerm->SetBitPack(cItemsPerBitPack);
          pTerm->SetCountTensorBins(cTensorBins);
 
          ++iTerm;
       } while(iTerm < cTerms);
    }
-   LOG_0(Trace_Info, "BoosterCore::Create finished feature group processing");
+   LOG_0(Trace_Info, "BoosterCore::Create finished term processing");
 
    EBM_ASSERT(nullptr == pBoosterCore->m_apInnerBags);
    if(0 != cTrainingSamples) {
       FloatFast * aWeights = nullptr;
       if(0 != cWeights) {
          error = ExtractWeights(
             pDataSetShared,
@@ -570,40 +577,43 @@
 
    // having 1 class means that all predictions are perfect. In the C interface we reduce this into having 0 scores, 
    // which means that we do not write anything to our upper level callers, and we don't need a bunch of things
    // since they have zero memory allocated to them. Having 0 classes means there are also 0 samples.
    if(ptrdiff_t { 0 } != cClasses && ptrdiff_t { 1 } != cClasses) {
       const size_t cScores = GetCountScores(cClasses);
 
+      LOG_0(Trace_Info, "INFO BoosterCore::Create determining Objective");
       Config config;
       config.cOutputs = cScores;
       config.isDifferentiallyPrivate = EBM_FALSE != isDifferentiallyPrivate ? EBM_TRUE : EBM_FALSE;
       error = GetObjective(&config, sObjective, &pBoosterCore->m_objective);
       if (Error_None != error) {
          // already logged
          return error;
       }
+      LOG_0(Trace_Info, "INFO BoosterCore::Create Objective determined");
 
       const OutputType outputType = GetOutputType(pBoosterCore->m_objective.m_linkFunction);
       if(IsClassification(cClasses)) {
          if(outputType < OutputType_GeneralClassification) {
-            LOG_0(Trace_Warning, "ERROR BoosterCore::Create mismatch in objective class model type");
+            LOG_0(Trace_Error, "ERROR BoosterCore::Create mismatch in objective class model type");
             return Error_IllegalParamVal;
          }
       } else {
          if(OutputType_Regression != outputType) {
-            LOG_0(Trace_Warning, "ERROR BoosterCore::Create mismatch in objective class model type");
+            LOG_0(Trace_Error, "ERROR BoosterCore::Create mismatch in objective class model type");
             return Error_IllegalParamVal;
          }
       }
 
       if(EBM_FALSE != pBoosterCore->CheckTargets(cSamples, aTargets)) {
-         LOG_0(Trace_Warning, "ERROR BoosterCore::Create invalid target value");
+         LOG_0(Trace_Warning, "WARNING BoosterCore::Create invalid target value");
          return Error_ObjectiveIllegalTarget;
       }
+      LOG_0(Trace_Info, "INFO BoosterCore::Create Targets verified");
 
       const bool bHessian = pBoosterCore->IsHessian();
 
       if(IsOverflowBinSize<FloatFast>(bHessian, cScores) || IsOverflowBinSize<FloatBig>(bHessian, cScores)) {
          LOG_0(Trace_Warning, "WARNING BoosterCore::Create bin size overflow");
          return Error_OutOfMemory;
       }
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/BoosterCore.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/BoosterCore.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/BoosterShell.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/BoosterShell.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 
 #include <stdlib.h> // free
 #include <stddef.h> // size_t, ptrdiff_t
 #include <string.h> // memcpy
 
 #include "RandomDeterministic.hpp" // RandomDeterministic
 
-#include "Transpose.hpp"
-
 #include "Feature.hpp" // Feature
 #include "Term.hpp" // Term
+#include "Transpose.hpp"
 #include "Tensor.hpp" // Tensor
 
 #include "BoosterCore.hpp" // BoosterCore
 #include "BoosterShell.hpp"
 
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
@@ -204,15 +203,15 @@
    }
    const size_t cTerms = static_cast<size_t>(countTerms);
 
    if(nullptr == dimensionCounts && size_t { 0 } != cTerms) {
       LOG_0(Trace_Error, "ERROR CreateBooster dimensionCounts cannot be null if 0 < countTerms");
       return Error_IllegalParamVal;
    }
-   // it's legal for featureIndexes to be null if there are no features indexed by our feature groups
+   // it's legal for featureIndexes to be null if there are no features indexed by our terms
    // dimensionCounts can have zero features, so it could be legal for this to be null even if 0 < countTerms
 
    if(IsConvertError<size_t>(countInnerBags)) {
       // this is just a warning since the caller doesn't pass us anything material, but if it's this high
       // then our allocation would fail since it can't even in pricipal fit into memory
       LOG_0(Trace_Warning, "WARNING CreateBooster IsConvertError<size_t>(countInnerBags)");
       return Error_OutOfMemory;
@@ -380,15 +379,15 @@
       LOG_0(Trace_Error, "ERROR GetBestTermScores indexTerm is too high to index");
       return Error_IllegalParamVal;
    }
    size_t iTerm = static_cast<size_t>(indexTerm);
 
    BoosterCore * const pBoosterCore = pBoosterShell->GetBoosterCore();
    if(pBoosterCore->GetCountTerms() <= iTerm) {
-      LOG_0(Trace_Error, "ERROR GetBestTermScores indexTerm above the number of feature groups that we have");
+      LOG_0(Trace_Error, "ERROR GetBestTermScores indexTerm above the number of terms that we have");
       return Error_IllegalParamVal;
    }
 
    if(ptrdiff_t { 0 } == pBoosterCore->GetCountClasses() || ptrdiff_t { 1 } == pBoosterCore->GetCountClasses()) {
       // for classification, if there is only 1 possible target class, then the probability of that class is 100%.  
       // If there were logits in this model, they'd all be infinity, but you could alternatively think of this 
       // model as having no logits, since the number of logits can be one less than the number of target classes.
@@ -399,38 +398,38 @@
    EBM_ASSERT(nullptr != pBoosterCore->GetBestModel());
    EBM_ASSERT(nullptr != pBoosterCore->GetTerms());
 
    const Term * const pTerm = pBoosterCore->GetTerms()[iTerm];
 
    size_t cTensorScores = pTerm->GetCountTensorBins();
    if(size_t { 0 } == cTensorScores) {
-      // if one of the dimensions has zero bins then the tensor has zero tensor bins and there is nothing to do
+      // If we have zero samples and one of the dimensions has 0 bins then there is no tensor, so return now
+      // In theory it might be better to zero out the caller's tensor cells (2 ^ n_dimensions), but this condition
+      // is almost an error already, so don't try reading/writing memory. We just define this situation as
+      // having a zero sized tensor result. The caller can zero their own memory if they want it zero
+
+      // if GetCountTensorBins is 0, then pBoosterCore->GetBestModel()[iTerm] does not contain valid data
+
       LOG_0(Trace_Warning, "WARNING GetBestTermScores feature with zero bins");
       return Error_None;
    }
    EBM_ASSERT(nullptr != pBoosterCore->GetBestModel()[iTerm]);
 
    if(nullptr == termScoresTensorOut) {
       LOG_0(Trace_Error, "ERROR GetBestTermScores termScoresTensorOut cannot be nullptr");
       return Error_IllegalParamVal;
    }
 
-   EBM_ASSERT(!IsMultiplyError(cTensorScores, GetCountScores(pBoosterCore->GetCountClasses())));
-   cTensorScores *= GetCountScores(pBoosterCore->GetCountClasses());
-
    Tensor * const pTensor = pBoosterCore->GetBestModel()[iTerm];
    EBM_ASSERT(nullptr != pTensor);
    EBM_ASSERT(pTensor->GetExpanded()); // the tensor should have been expanded at startup
    FloatFast * const aTermScores = pTensor->GetTensorScoresPointer();
    EBM_ASSERT(nullptr != aTermScores);
 
-   EBM_ASSERT(!IsMultiplyError(sizeof(*termScoresTensorOut), cTensorScores));
-   EBM_ASSERT(!IsMultiplyError(sizeof(*aTermScores), cTensorScores));
-   static_assert(sizeof(*termScoresTensorOut) == sizeof(*aTermScores), "float mismatch");
-   memcpy(termScoresTensorOut, aTermScores, sizeof(*aTermScores) * cTensorScores);
+   Transpose<true>(pTerm, GetCountScores(pBoosterCore->GetCountClasses()), termScoresTensorOut, aTermScores);
 
    LOG_0(Trace_Info, "Exited GetBestTermScores");
    return Error_None;
 }
 
 EBM_API_BODY ErrorEbm EBM_CALLING_CONVENTION GetCurrentTermScores(
    BoosterHandle boosterHandle,
@@ -460,15 +459,15 @@
       LOG_0(Trace_Error, "ERROR GetCurrentTermScores indexTerm is too high to index");
       return Error_IllegalParamVal;
    }
    size_t iTerm = static_cast<size_t>(indexTerm);
 
    BoosterCore * const pBoosterCore = pBoosterShell->GetBoosterCore();
    if(pBoosterCore->GetCountTerms() <= iTerm) {
-      LOG_0(Trace_Error, "ERROR GetCurrentTermScores indexTerm above the number of feature groups that we have");
+      LOG_0(Trace_Error, "ERROR GetCurrentTermScores indexTerm above the number of terms that we have");
       return Error_IllegalParamVal;
    }
 
    if(ptrdiff_t { 0 } == pBoosterCore->GetCountClasses() || ptrdiff_t { 1 } == pBoosterCore->GetCountClasses()) {
       // for classification, if there is only 1 possible target class, then the probability of that class is 100%.  
       // If there were logits in this model, they'd all be infinity, but you could alternatively think of this 
       // model as having no logits, since the number of logits can be one less than the number of target classes.
@@ -479,38 +478,38 @@
    EBM_ASSERT(nullptr != pBoosterCore->GetCurrentModel());
    EBM_ASSERT(nullptr != pBoosterCore->GetTerms());
 
    const Term * const pTerm = pBoosterCore->GetTerms()[iTerm];
 
    size_t cTensorScores = pTerm->GetCountTensorBins();
    if(size_t { 0 } == cTensorScores) {
-      // if one of the dimensions has zero bins then the tensor has zero tensor bins and there is nothing to do
+      // If we have zero samples and one of the dimensions has 0 bins then there is no tensor, so return now
+      // In theory it might be better to zero out the caller's tensor cells (2 ^ n_dimensions), but this condition
+      // is almost an error already, so don't try reading/writing memory. We just define this situation as
+      // having a zero sized tensor result. The caller can zero their own memory if they want it zero
+
+      // if GetCountTensorBins is 0, then pBoosterCore->GetCurrentModel()[iTerm] does not contain valid data
+
       LOG_0(Trace_Warning, "WARNING GetCurrentTermScores feature with zero bins");
       return Error_None;
    }
    EBM_ASSERT(nullptr != pBoosterCore->GetCurrentModel()[iTerm]);
 
    if(nullptr == termScoresTensorOut) {
       LOG_0(Trace_Error, "ERROR GetCurrentTermScores termScoresTensorOut cannot be nullptr");
       return Error_IllegalParamVal;
    }
 
-   EBM_ASSERT(!IsMultiplyError(cTensorScores, GetCountScores(pBoosterCore->GetCountClasses())));
-   cTensorScores *= GetCountScores(pBoosterCore->GetCountClasses());
-
    Tensor * const pTensor = pBoosterCore->GetCurrentModel()[iTerm];
    EBM_ASSERT(nullptr != pTensor);
    EBM_ASSERT(pTensor->GetExpanded()); // the tensor should have been expanded at startup
    FloatFast * const aTermScores = pTensor->GetTensorScoresPointer();
    EBM_ASSERT(nullptr != aTermScores);
 
-   EBM_ASSERT(!IsMultiplyError(sizeof(*termScoresTensorOut), cTensorScores));
-   EBM_ASSERT(!IsMultiplyError(sizeof(*aTermScores), cTensorScores));
-   static_assert(sizeof(*termScoresTensorOut) == sizeof(*aTermScores), "float mismatch");
-   memcpy(termScoresTensorOut, aTermScores, sizeof(*aTermScores) * cTensorScores);
+   Transpose<true>(pTerm, GetCountScores(pBoosterCore->GetCountClasses()), termScoresTensorOut, aTermScores);
 
    LOG_0(Trace_Info, "Exited GetCurrentTermScores");
    return Error_None;
 }
 
 EBM_API_BODY void EBM_CALLING_CONVENTION FreeBooster(
    BoosterHandle boosterHandle
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/BoosterShell.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/BoosterShell.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/CODING_STYLE.md` & `interpret-core-0.4.2/symbolic/shared/libebm/CODING_STYLE.md`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/CalcInteractionStrength.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/CalcInteractionStrength.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
       }
       const size_t iFeature = static_cast<size_t>(indexFeature);
 
       const FeatureInteraction * const pFeature = &aFeatures[iFeature];
 
       const size_t cBins = pFeature->GetCountBins();
       if(UNLIKELY(cBins <= size_t { 1 })) {
-         LOG_0(Trace_Info, "INFO CalcInteractionStrength feature group contains a feature with only 1 or 0 bins");
+         LOG_0(Trace_Info, "INFO CalcInteractionStrength term contains a feature with only 1 or 0 bins");
          if(nullptr != avgInteractionStrengthOut) {
             *avgInteractionStrengthOut = 0.0;
          }
          return Error_None;
       }
       binSums.m_acBins[iDimension] = cBins;
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/CutQuantile.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/CutQuantile.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -976,14 +976,27 @@
          EBM_ASSERT(cRangesLowModification <= k_cutExploreDistance);
          EBM_ASSERT(-pCutBest->m_cPredeterminedMovementOnCut < static_cast<ptrdiff_t>(cRangesLowModification));
 
          EBM_ASSERT(double { 0 } <= pCutLowModificationExclusiveBoundary->m_iValAspirationalFloat);
 
          // this should be exact, since we would have set it like this
          EBM_ASSERT(!pCutLowModificationExclusiveBoundary->IsCut() || pCutLowModificationExclusiveBoundary->m_iValAspirationalFloat == static_cast<double>(pCutLowModificationExclusiveBoundary->m_iVal));
+         // TODO: We've gotten a report of this assert triggering from this issue:
+         // https://github.com/interpretml/interpret/issues/430
+         // I think I need to add "k_valNotLegal == pCutLowModificationExclusiveBoundary->m_iVal || " but I cannot
+         // figure out what realistic situation m_iVal would end up with k_valNotLegal at a distance of exactly
+         // k_cutExploreDistance since k_valNotLegal gets generated when potential cuts are pushed into a corner
+         // but you would think that would mean that there would be a valid cut separating a potential cut
+         // from the set of illegal cuts and we wouldn't be able to have k_cutExploreDistance uncut potential
+         // cuts with the k_valNotLegal located exactly at distance k_cutExploreDistance.
+         // This also applies to the assert below that checks:
+         // "pCutBest->m_iVal <= pCutHighModificationExclusiveBoundary->m_iVal"
+         // I do not believe this condition creates an issue in the release build, but I'm leaving the assert
+         // here without modification until we can find a valid case where this occurs to preclude the scenario
+         // that there is an unknown bug.
          EBM_ASSERT(pCutLowModificationExclusiveBoundary->m_iVal <= pCutBest->m_iVal);
          EBM_ASSERT(pCutLowModificationExclusiveBoundary->m_iValAspirationalFloat < pCutBest->m_iValAspirationalFloat);
 
          CutPoint * pCutHighModificationExclusiveBoundary = pCutBest;
          size_t cRangesHighModification = k_cutExploreDistance;
          ptrdiff_t cPredeterminedMovementOnCutHighHigh;
          do {
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/CutUniform.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/CutUniform.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/CutWinsorized.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/CutWinsorized.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/DataSetBoosting.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/DataSetBoosting.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -330,22 +330,22 @@
             goto free_all;
          }
          *paInputDataTo = pInputDataTo;
          ++paInputDataTo;
 
          const StorageDataType * const pInputDataToEnd = pInputDataTo + cDataUnitsTo;
 
-         const FeatureBoosting * const * ppFeature = pTerm->GetFeatures();
+         const TermFeature * pTermFeature = pTerm->GetTermFeatures();
          EBM_ASSERT(1 <= pTerm->GetCountDimensions());
-         const FeatureBoosting * const * const ppFeaturesEnd = &ppFeature[pTerm->GetCountDimensions()];
+         const TermFeature * const pTermFeaturesEnd = &pTermFeature[pTerm->GetCountDimensions()];
 
          InputDataPointerAndCountBins dimensionInfo[k_cDimensionsMax];
          InputDataPointerAndCountBins * pDimensionInfoInit = &dimensionInfo[0];
          do {
-            const FeatureBoosting * const pFeature = *ppFeature;
+            const FeatureBoosting * const pFeature = pTermFeature->m_pFeature;
             const size_t cBins = pFeature->GetCountBins();
             EBM_ASSERT(size_t { 1 } <= cBins); // we don't construct datasets on empty training sets
             if(size_t { 1 } < cBins) {
                const IntEbm indexFeature = *piTermFeatures;
                EBM_ASSERT(!IsConvertError<size_t>(indexFeature)); // we converted it previously
                const size_t iFeature = static_cast<size_t>(indexFeature);
 
@@ -404,16 +404,16 @@
                pDimensionInfoInit->m_cBitsPerItemMaxFrom = cBitsPerItemMaxFrom;
                pDimensionInfoInit->m_maskBitsFrom = maskBitsFrom;
                pDimensionInfoInit->m_iShiftFrom = static_cast<ptrdiff_t>((cSharedSamples - 1) % cItemsPerBitPackFrom);
 
                ++pDimensionInfoInit;
             }
             ++piTermFeatures;
-            ++ppFeature;
-         } while(ppFeaturesEnd != ppFeature);
+            ++pTermFeature;
+         } while(pTermFeaturesEnd != pTermFeature);
          EBM_ASSERT(pDimensionInfoInit == &dimensionInfo[pTerm->GetCountRealDimensions()]);
 
          EBM_ASSERT(nullptr != aBag || isLoopTraining); // if aBag is nullptr then we have no validation samples
          const BagEbm * pSampleReplication = aBag;
          BagEbm replication = 0;
          StorageDataType iTensor;
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/DataSetBoosting.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/DataSetBoosting.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/DataSetInteraction.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/DataSetInteraction.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/DataSetInteraction.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/DataSetInteraction.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/DetermineLinkFunction.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/DetermineLinkFunction.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -19,22 +19,38 @@
 
 EBM_API_BODY ErrorEbm EBM_CALLING_CONVENTION DetermineLinkFunction(
    BoolEbm isDifferentiallyPrivate,
    const char * objective,
    LinkEbm * linkOut,
    double * linkParamOut
 ) {
+   LOG_N(
+      Trace_Info,
+      "Entered DetermineLinkFunction: "
+      "isDifferentiallyPrivate=%s, "
+      "objective=%p, "
+      "linkOut=%p, "
+      "linkParamOut=%p"
+      ,
+      ObtainTruth(isDifferentiallyPrivate),
+      static_cast<const void *>(objective),
+      static_cast<void *>(linkOut),
+      static_cast<void *>(linkParamOut)
+   );
+
    ObjectiveWrapper objectiveWrapper;
    InitializeObjectiveWrapperUnfailing(&objectiveWrapper);
 
    Config config;
    config.cOutputs = 1; // this is kind of cheating, but it should work
    config.isDifferentiallyPrivate = EBM_FALSE != isDifferentiallyPrivate ? EBM_TRUE : EBM_FALSE;
    const ErrorEbm error = GetObjective(&config, objective, &objectiveWrapper);
    if(Error_None != error) {
+      LOG_0(Trace_Error, "ERROR DetermineLinkFunction GetObjective failed");
+
       if(nullptr != linkOut) {
          *linkOut = Link_ERROR;
       }
       if(nullptr != linkParamOut) {
          *linkParamOut = std::numeric_limits<double>::quiet_NaN();
       }
       return error;
@@ -45,14 +61,17 @@
 
    if(nullptr != linkOut) {
       *linkOut = objectiveWrapper.m_linkFunction;
    }
    if(nullptr != linkParamOut) {
       *linkParamOut = objectiveWrapper.m_linkParam;
    }
+
+   LOG_0(Trace_Info, "Exited DetermineLinkFunction");
+
    return Error_None;
 }
 
 static const char g_sCustomRegression[] = "custom_regression";
 static const char g_sCustomClassification[] = "custom_classification";
 static const char g_sCustomRanking[] = "custom_ranking";
 static const char g_sPower[] = "power";
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/Discretize.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/Discretize.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/Feature.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/Feature.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/GaussianDistribution.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/GaussianDistribution.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/GenerateTermUpdate.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/GenerateTermUpdate.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -295,26 +295,26 @@
 
    const size_t cTensorBins = pTerm->GetCountTensorBins();
    EBM_ASSERT(1 <= cTensorBins);
 
    size_t acBins[k_cDimensionsMax];
    size_t * pcBins = acBins;
 
-   const FeatureBoosting * const * ppFeature = pTerm->GetFeatures();
-   const FeatureBoosting * const * const ppFeaturesEnd = &ppFeature[pTerm->GetCountDimensions()];
+   const TermFeature * pTermFeature = pTerm->GetTermFeatures();
+   const TermFeature * const pTermFeaturesEnd = &pTermFeature[pTerm->GetCountDimensions()];
    do {
-      const FeatureBoosting * pFeature = *ppFeature;
+      const FeatureBoosting * pFeature = pTermFeature->m_pFeature;
       const size_t cBins = pFeature->GetCountBins();
       EBM_ASSERT(size_t { 1 } <= cBins); // we don't boost on empty training sets
       if(size_t { 1 } < cBins) {
          *pcBins = cBins;
          ++pcBins;
       }
-      ++ppFeature;
-   } while(ppFeaturesEnd != ppFeature);
+      ++pTermFeature;
+   } while(pTermFeaturesEnd != pTermFeature);
 
    const size_t cScores = GetCountScores(pBoosterCore->GetCountClasses());
 
    EBM_ASSERT(!IsOverflowBinSize<FloatFast>(pBoosterCore->IsHessian(), cScores)); // we check in CreateBooster 
    const size_t cBytesPerFastBin = GetBinSize<FloatFast>(pBoosterCore->IsHessian(), cScores);
    EBM_ASSERT(!IsMultiplyError(cBytesPerFastBin, cTensorBins));
 
@@ -692,15 +692,15 @@
       return Error_IllegalParamVal;
    }
 
    BoosterCore * const pBoosterCore = pBoosterShell->GetBoosterCore();
    EBM_ASSERT(nullptr != pBoosterCore);
 
    if(static_cast<IntEbm>(pBoosterCore->GetCountTerms()) <= indexTerm) {
-      LOG_0(Trace_Error, "ERROR GenerateTermUpdate indexTerm above the number of feature groups that we have");
+      LOG_0(Trace_Error, "ERROR GenerateTermUpdate indexTerm above the number of terms that we have");
       return Error_IllegalParamVal;
    }
    size_t iTerm = static_cast<size_t>(indexTerm);
 
    // this is true because 0 < pBoosterCore->m_cTerms since our caller needs to pass in a valid indexTerm to this function
    EBM_ASSERT(nullptr != pBoosterCore->GetTerms());
    Term * const pTerm = pBoosterCore->GetTerms()[iTerm];
@@ -788,19 +788,19 @@
    size_t iDimensionImportant = 0;
    if(nullptr == leavesMax) {
       LOG_0(Trace_Warning, "WARNING GenerateTermUpdate leavesMax was null, so there won't be any splits");
    } else {
       if(0 != cRealDimensions) {
          size_t iDimensionInit = 0;
          const IntEbm * pLeavesMax = leavesMax;
-         const FeatureBoosting * const * ppFeature = pTerm->GetFeatures();
+         const TermFeature * pTermFeature = pTerm->GetTermFeatures();
          EBM_ASSERT(1 <= cDimensions);
-         const FeatureBoosting * const * const ppFeaturesEnd = &ppFeature[cDimensions];
+         const TermFeature * const pTermFeaturesEnd = &pTermFeature[cDimensions];
          do {
-            const FeatureBoosting * const pFeature = *ppFeature;
+            const FeatureBoosting * const pFeature = pTermFeature->m_pFeature;
             const size_t cBins = pFeature->GetCountBins();
             if(size_t { 1 } < cBins) {
                // if there is only 1 dimension then this is our first time here and lastDimensionLeavesMax must be zero
                EBM_ASSERT(size_t { 2 } <= cRealDimensions || IntEbm { 0 } == lastDimensionLeavesMax);
 
                iDimensionImportant = iDimensionInit;
                cSignificantBinCount = cBins;
@@ -811,16 +811,16 @@
                } else {
                   // keep iteration even once we find this so that we output logs for any bins of 1
                   lastDimensionLeavesMax = countLeavesMax;
                }
             }
             ++iDimensionInit;
             ++pLeavesMax;
-            ++ppFeature;
-         } while(ppFeaturesEnd != ppFeature);
+            ++pTermFeature;
+         } while(pTermFeaturesEnd != pTermFeature);
 
          EBM_ASSERT(size_t { 2 } <= cSignificantBinCount);
       }
    }
 
    pBoosterShell->GetTermUpdate()->SetCountDimensions(cDimensions);
    pBoosterShell->GetTermUpdate()->Reset();
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/IMPORTANT.md` & `interpret-core-0.4.2/symbolic/shared/libebm/IMPORTANT.md`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/InitializeGradientsAndHessians.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/InitializeGradientsAndHessians.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/InnerBag.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/InnerBag.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/InnerBag.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/InnerBag.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/InteractionCore.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/InteractionCore.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -206,40 +206,43 @@
       return Error_IllegalParamVal;
    }
    pInteractionCore->m_cClasses = cClasses;
 
    if(ptrdiff_t { 0 } != cClasses && ptrdiff_t { 1 } != cClasses) {
       const size_t cScores = GetCountScores(cClasses);
 
+      LOG_0(Trace_Info, "INFO InteractionCore::Create determining Objective");
       Config config;
       config.cOutputs = cScores;
       config.isDifferentiallyPrivate = EBM_FALSE != isDifferentiallyPrivate ? EBM_TRUE : EBM_FALSE;
       error = GetObjective(&config, sObjective, &pInteractionCore->m_objective);
       if(Error_None != error) {
          // already logged
          return error;
       }
+      LOG_0(Trace_Info, "INFO InteractionCore::Create Objective determined");
 
       const OutputType outputType = GetOutputType(pInteractionCore->m_objective.m_linkFunction);
       if(IsClassification(cClasses)) {
          if(outputType < OutputType_GeneralClassification) {
-            LOG_0(Trace_Warning, "ERROR InteractionCore::Create mismatch in objective class model type");
+            LOG_0(Trace_Error, "ERROR InteractionCore::Create mismatch in objective class model type");
             return Error_IllegalParamVal;
          }
       } else {
          if(OutputType_Regression != outputType) {
-            LOG_0(Trace_Warning, "ERROR InteractionCore::Create mismatch in objective class model type");
+            LOG_0(Trace_Error, "ERROR InteractionCore::Create mismatch in objective class model type");
             return Error_IllegalParamVal;
          }
       }
 
       if(EBM_FALSE != pInteractionCore->CheckTargets(cSamples, aTargets)) {
-         LOG_0(Trace_Warning, "ERROR InteractionCore::Create invalid target value");
+         LOG_0(Trace_Warning, "WARNING InteractionCore::Create invalid target value");
          return Error_ObjectiveIllegalTarget;
       }
+      LOG_0(Trace_Info, "INFO InteractionCore::Create Targets verified");
 
       const bool bHessian = pInteractionCore->IsHessian();
 
       if(IsOverflowBinSize<FloatFast>(bHessian, cScores) || IsOverflowBinSize<FloatBig>(bHessian, cScores)) {
          LOG_0(Trace_Warning, "WARNING InteractionCore::Create IsOverflowBinSize overflow");
          return Error_OutOfMemory;
       }
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/InteractionCore.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/InteractionCore.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/InteractionShell.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/InteractionShell.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/InteractionShell.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/InteractionShell.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/PartitionOneDimensionalBoosting.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/PartitionOneDimensionalBoosting.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -102,59 +102,58 @@
 
 // do not inline this.  Not inlining it makes fewer versions that can be called from the more templated functions
 template<bool bHessian>
 static ErrorEbm Flatten(
    BoosterShell * const pBoosterShell,
    const size_t iDimension,
    const size_t cBins,
-   const size_t cSplits
+   const size_t cSlices
 ) {
    LOG_0(Trace_Verbose, "Entered Flatten");
 
    EBM_ASSERT(nullptr != pBoosterShell);
    EBM_ASSERT(iDimension <= k_cDimensionsMax);
-   EBM_ASSERT(cSplits < cBins);
+   EBM_ASSERT(cSlices <= cBins);
    
    ErrorEbm error;
 
    Tensor * const pInnerTermUpdate = pBoosterShell->GetInnerTermUpdate();
 
-   error = pInnerTermUpdate->SetCountSplits(iDimension, cSplits);
+   error = pInnerTermUpdate->SetCountSlices(iDimension, cSlices);
    if(UNLIKELY(Error_None != error)) {
       // already logged
       return error;
    }
 
    const BoosterCore * const pBoosterCore = pBoosterShell->GetBoosterCore();
    const size_t cScores = GetCountScores(pBoosterCore->GetCountClasses());
 
-   // we checked during init that cScores * cBins can be allocated, so cSplits + 1 must work too
-   EBM_ASSERT(!IsMultiplyError(cScores, cSplits + size_t { 1 }));
-   error = pInnerTermUpdate->EnsureTensorScoreCapacity(cScores * (cSplits + size_t { 1 }));
+   EBM_ASSERT(!IsMultiplyError(cScores, cSlices));
+   error = pInnerTermUpdate->EnsureTensorScoreCapacity(cScores * cSlices);
    if(UNLIKELY(Error_None != error)) {
       // already logged
       return error;
    }
 
-   ActiveDataType * pSplits = pInnerTermUpdate->GetSplitPointer(iDimension);
+   ActiveDataType * pSplit = pInnerTermUpdate->GetSplitPointer(iDimension);
    FloatFast * pUpdateScore = pInnerTermUpdate->GetTensorScoresPointer();
 
    EBM_ASSERT(!IsOverflowBinSize<FloatBig>(bHessian, cScores)); // we're accessing allocated memory
    const size_t cBytesPerBin = GetBinSize<FloatBig>(bHessian, cScores);
 
    EBM_ASSERT(!IsOverflowTreeNodeSize(bHessian, cScores)); // we're accessing allocated memory
    const size_t cBytesPerTreeNode = GetTreeNodeSize(bHessian, cScores);
 
    const auto * const aBins = pBoosterShell->GetBoostingBigBins()->Specialize<FloatBig, bHessian>();
    const auto * const pBinsEnd = IndexBin(aBins, cBytesPerBin * cBins);
 
    auto * pTreeNode = pBoosterShell->GetTreeNodesTemp<bHessian>();
 
    TreeNode<bHessian> * pParent = nullptr;
-   size_t iSplit;
+   size_t iEdge;
    while(true) {
 
    moved_down:;
       if(UNPREDICTABLE(pTreeNode->AFTER_IsSplit())) {
 #ifndef NDEBUG
          pTreeNode->SetDebugProgression(2);
 #endif // NDEBUG
@@ -176,15 +175,15 @@
             const auto * const pRightChild = GetRightNode(pTreeNode->AFTER_GetChildren(), cBytesPerTreeNode);
             pBinLastOrChildren = pRightChild->BEFORE_GetBinLast();
          }
          const auto * const pBinLast = reinterpret_cast<const Bin<FloatBig, bHessian> *>(pBinLastOrChildren);
 
          EBM_ASSERT(aBins <= pBinLast);
          EBM_ASSERT(pBinLast < pBinsEnd);
-         iSplit = CountBins(pBinLast, aBins, cBytesPerBin);
+         iEdge = CountBins(pBinLast, aBins, cBytesPerBin) + 1;
             
          const auto * aGradientPair = pTreeNode->GetGradientPairs();
          size_t iScore = 0;
          do {
             FloatBig updateScore;
             if(bHessian) {
                updateScore = EbmStats::ComputeSinglePartitionUpdate(
@@ -206,16 +205,16 @@
          }
          break; // this can only happen if our tree has zero splits, but we need to check it
       }
 
    moved_up:;
       auto * pChildren = pTreeNode->AFTER_GetChildren();
       if(nullptr != pChildren) {
-         *pSplits = iSplit;
-         ++pSplits;
+         *pSplit = iEdge;
+         ++pSplit;
 
          pParent = pTreeNode;
          pTreeNode->AFTER_SetChildren(nullptr);
          pTreeNode = GetRightNode(pChildren, cBytesPerTreeNode);
          goto moved_down;
       } else {
          pTreeNode = pTreeNode->DECONSTRUCT_GetParent();
@@ -704,15 +703,15 @@
             // calling anything inside nodeGainRanking can throw exceptions
             LOG_0(Trace_Warning, "WARNING PartitionOneDimensionalBoosting exception");
             return Error_UnexpectedInternal;
          }
       }
       *pTotalGain = static_cast<double>(totalGain);
       const size_t cSplits = cSplitsMax - cSplitsRemaining;
-      return Flatten<bHessian>(pBoosterShell, iDimension, cBins, cSplits);
+      return Flatten<bHessian>(pBoosterShell, iDimension, cBins, cSplits + 1);
    }
 };
 
 extern ErrorEbm PartitionOneDimensionalBoosting(
    RandomDeterministic * const pRng,
    BoosterShell * const pBoosterShell,
    const size_t cBins,
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/PartitionRandomBoosting.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/PartitionRandomBoosting.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 
       EBM_ASSERT(1 <= pTerm->GetCountRealDimensions());
       EBM_ASSERT(1 <= pTerm->GetCountDimensions());
 
       Tensor * const pInnerTermUpdate = pBoosterShell->GetInnerTermUpdate();
 
       const IntEbm * pLeavesMax1 = aLeavesMax;
-      const FeatureBoosting * const * ppFeature1 = pTerm->GetFeatures();
-      const FeatureBoosting * const * const ppFeaturesEnd = &ppFeature1[pTerm->GetCountDimensions()];
+      const TermFeature * pTermFeature1 = pTerm->GetTermFeatures();
+      const TermFeature * const pTermFeaturesEnd = &pTermFeature1[pTerm->GetCountDimensions()];
       size_t cSlicesTotal = 0;
       size_t cSlicesPlusRandomMax = 0;
       size_t cCollapsedTensorCells = 1;
       do {
          size_t cLeavesMax;
          if(nullptr == pLeavesMax1) {
             cLeavesMax = size_t { 1 };
@@ -86,15 +86,15 @@
                   // we can never exceed a size_t number of leaves, so let's just set it to the maximum if we 
                   // were going to overflow because it will generate the same results as if we used the true number
                   cLeavesMax = std::numeric_limits<size_t>::max();
                }
             }
          }
 
-         const FeatureBoosting * const pFeature = *ppFeature1;
+         const FeatureBoosting * const pFeature = pTermFeature1->m_pFeature;
          const size_t cBins = pFeature->GetCountBins();
          EBM_ASSERT(size_t { 1 } <= cBins); // we don't boost on empty training sets
          const size_t cSlices = EbmMin(cLeavesMax, cBins);
          EBM_ASSERT(1 <= cSlices);
 
          const size_t cPossibleSplitLocations = cBins - size_t { 1 };
          if(size_t { 0 } != cPossibleSplitLocations) {
@@ -113,16 +113,16 @@
             // multiplication, so we can conclude that addition won't overflow since the multiplication didn't
             EBM_ASSERT(!IsAddError(cSlicesTotal, cSlices));
             cSlicesTotal += cSlices;
 
             EBM_ASSERT(!IsMultiplyError(cCollapsedTensorCells, cSlices)); // our allocated histogram is bigger
             cCollapsedTensorCells *= cSlices;
          }
-         ++ppFeature1;
-      } while(ppFeaturesEnd != ppFeature1);
+         ++pTermFeature1;
+      } while(pTermFeaturesEnd != pTermFeature1);
 
       // since we subtract 1 from cPossibleSplitLocations, we need to check that our final slice length isn't longer
       cSlicesPlusRandomMax = EbmMax(cSlicesPlusRandomMax, cSlicesTotal);
 
       if(IsMultiplyError(sizeof(size_t), cSlicesPlusRandomMax)) {
          LOG_0(Trace_Warning, "WARNING PartitionRandomBoostingInternal IsMultiplyError(sizeof(size_t), cSlicesPlusRandomMax)");
          return Error_OutOfMemory;
@@ -163,15 +163,15 @@
          LOG_0(Trace_Warning, "WARNING PartitionRandomBoostingInternal nullptr == pBuffer");
          return Error_OutOfMemory;
       }
       size_t * const acItemsInNextSliceOrBytesInCurrentSlice = reinterpret_cast<size_t *>(pBuffer);
 
       const IntEbm * pLeavesMax2 = aLeavesMax;
       size_t * pcItemsInNextSliceOrBytesInCurrentSlice2 = acItemsInNextSliceOrBytesInCurrentSlice;
-      const FeatureBoosting * const * ppFeature2 = pTerm->GetFeatures();
+      const TermFeature * pTermFeature2 = pTerm->GetTermFeatures();
       do {
          size_t cTreeSplitsMax;
          if(nullptr == pLeavesMax2) {
             cTreeSplitsMax = size_t { 0 };
          } else {
             const IntEbm countLeavesMax = *pLeavesMax2;
             ++pLeavesMax2;
@@ -183,29 +183,29 @@
                   // we can never exceed a size_t number of leaves, so let's just set it to the maximum if we 
                   // were going to overflow because it will generate the same results as if we used the true number
                   cTreeSplitsMax = std::numeric_limits<size_t>::max() - size_t { 1 };
                }
             }
          }
 
-         const FeatureBoosting * const pFeature = *ppFeature2;
+         const FeatureBoosting * const pFeature = pTermFeature2->m_pFeature;
          const size_t cBins = pFeature->GetCountBins();
          EBM_ASSERT(size_t { 1 } <= cBins); // we don't boost on empty training sets
          size_t cPossibleSplitLocations = cBins - size_t { 1 };
          if(size_t { 0 } != cPossibleSplitLocations) {
             // drop any dimensions with 1 bin since the tensor is the same without the extra dimension
 
             if(size_t { 0 } != cTreeSplitsMax) {
                size_t * pFillIndexes = pcItemsInNextSliceOrBytesInCurrentSlice2;
-               size_t iPossibleSplitLocations = cPossibleSplitLocations; // 1 means split between bin 0 and bin 1
+               size_t iEdge = cPossibleSplitLocations; // 1 means split between bin 0 and bin 1
                do {
-                  *pFillIndexes = iPossibleSplitLocations;
+                  *pFillIndexes = iEdge;
                   ++pFillIndexes;
-                  --iPossibleSplitLocations;
-               } while(size_t { 0 } != iPossibleSplitLocations);
+                  --iEdge;
+               } while(size_t { 0 } != iEdge);
 
                size_t * pOriginal = pcItemsInNextSliceOrBytesInCurrentSlice2;
 
                const size_t cSplits = EbmMin(cTreeSplitsMax, cPossibleSplitLocations);
                EBM_ASSERT(1 <= cSplits);
                const size_t * const pcItemsInNextSliceOrBytesInCurrentSliceEnd = pcItemsInNextSliceOrBytesInCurrentSlice2 + cSplits;
                do {
@@ -219,24 +219,24 @@
                } while(pcItemsInNextSliceOrBytesInCurrentSliceEnd != pcItemsInNextSliceOrBytesInCurrentSlice2);
 
                std::sort(pOriginal, pcItemsInNextSliceOrBytesInCurrentSlice2);
             }
             *pcItemsInNextSliceOrBytesInCurrentSlice2 = cBins; // index 1 past the last item
             ++pcItemsInNextSliceOrBytesInCurrentSlice2;
          }
-         ++ppFeature2;
-      } while(ppFeaturesEnd != ppFeature2);
+         ++pTermFeature2;
+      } while(pTermFeaturesEnd != pTermFeature2);
 
       const IntEbm * pLeavesMax3 = aLeavesMax;
       const size_t * pcBytesInSliceEnd;
-      const FeatureBoosting * const * ppFeature3 = pTerm->GetFeatures();
+      const TermFeature * pTermFeature3 = pTerm->GetTermFeatures();
       size_t * pcItemsInNextSliceOrBytesInCurrentSlice3 = acItemsInNextSliceOrBytesInCurrentSlice;
       size_t cBytesCollapsedTensor3;
       while(true) {
-         EBM_ASSERT(ppFeature3 < ppFeaturesEnd);
+         EBM_ASSERT(pTermFeature3 < pTermFeaturesEnd);
 
          size_t cLeavesMax;
          if(nullptr == pLeavesMax3) {
             cLeavesMax = size_t { 1 };
          } else {
             const IntEbm countLeavesMax = *pLeavesMax3;
             ++pLeavesMax3;
@@ -249,16 +249,16 @@
                   // were going to overflow because it will generate the same results as if we used the true number
                   cLeavesMax = std::numeric_limits<size_t>::max();
                }
             }
          }
 
          // the first dimension is special.  we put byte until next item into it instead of counts remaining
-         const FeatureBoosting * const pFeature = *ppFeature3;
-         ++ppFeature3;
+         const FeatureBoosting * const pFeature = pTermFeature3->m_pFeature;
+         ++pTermFeature3;
          const size_t cBins = pFeature->GetCountBins();
          EBM_ASSERT(size_t { 1 } <= cBins); // we don't boost on empty training sets
          if(size_t { 1 } < cBins) {
             // drop any dimensions with 1 bin since the tensor is the same without the extra dimension
 
             const size_t cFirstSlices = EbmMin(cLeavesMax, cBins);
             cBytesCollapsedTensor3 = cBytesPerBin * cFirstSlices;
@@ -295,15 +295,15 @@
 
          const size_t * m_pcItemsInNextSlice;
          const size_t * m_pcItemsInNextSliceEnd;
       };
       RandomSplitState randomSplitState[k_cDimensionsMax - size_t { 1 }]; // the first dimension is special cased
       RandomSplitState * pStateInit = &randomSplitState[0];
 
-      for(; ppFeaturesEnd != ppFeature3; ++ppFeature3) {
+      for(; pTermFeaturesEnd != pTermFeature3; ++pTermFeature3) {
          size_t cLeavesMax;
          if(nullptr == pLeavesMax3) {
             cLeavesMax = size_t { 1 };
          } else {
             const IntEbm countLeavesMax = *pLeavesMax3;
             ++pLeavesMax3;
             if(countLeavesMax <= IntEbm { 1 }) {
@@ -314,15 +314,15 @@
                   // we can never exceed a size_t number of leaves, so let's just set it to the maximum if we 
                   // were going to overflow because it will generate the same results as if we used the true number
                   cLeavesMax = std::numeric_limits<size_t>::max();
                }
             }
          }
 
-         const FeatureBoosting * const pFeature = *ppFeature3;
+         const FeatureBoosting * const pFeature = pTermFeature3->m_pFeature;
          const size_t cBins = pFeature->GetCountBins();
          EBM_ASSERT(size_t { 1 } <= cBins); // we don't boost on empty training sets
          if(size_t { 1 } < cBins) {
             // drop any dimensions with 1 bin since the tensor is the same without the extra dimension
 
             size_t cSlices = EbmMin(cLeavesMax, cBins);
 
@@ -432,80 +432,80 @@
       //      bin from which we can calculate the parent and subtract the best child from the parent.
       
       //FloatBig gain;
       //FloatBig gainParent = FloatBig { 0 };
       FloatBig gain = 0;
 
 
-      const FeatureBoosting * const * ppFeature4 = pTerm->GetFeatures();
+      const TermFeature * pTermFeature4 = pTerm->GetTermFeatures();
       size_t iDimensionWrite = ~size_t { 0 }; // this is -1, but without the compiler warning
       size_t cBinsWrite;
       do {
-         const FeatureBoosting * const pFeature = *ppFeature4;
+         const FeatureBoosting * const pFeature = pTermFeature4->m_pFeature;
          cBinsWrite = pFeature->GetCountBins();
          ++iDimensionWrite;
-         ++ppFeature4;
+         ++pTermFeature4;
       } while(cBinsWrite <= size_t { 1 });
 
-      const size_t * const pcBytesInSliceLast = pcBytesInSliceEnd - size_t { 1 };
-      EBM_ASSERT(acItemsInNextSliceOrBytesInCurrentSlice <= pcBytesInSliceLast);
-      const size_t cFirstSplits = pcBytesInSliceLast - acItemsInNextSliceOrBytesInCurrentSlice;
+      EBM_ASSERT(acItemsInNextSliceOrBytesInCurrentSlice < pcBytesInSliceEnd);
+      const size_t cFirstSlices = pcBytesInSliceEnd - acItemsInNextSliceOrBytesInCurrentSlice;
       // 3 items in the acItemsInNextSliceOrBytesInCurrentSlice means 2 splits and 
       // one last item to indicate the termination point
-      error = pInnerTermUpdate->SetCountSplits(iDimensionWrite, cFirstSplits);
+      error = pInnerTermUpdate->SetCountSlices(iDimensionWrite, cFirstSlices);
       if(UNLIKELY(Error_None != error)) {
          // already logged
          free(pBuffer);
          return error;
       }
       const size_t * pcBytesInSlice2 = acItemsInNextSliceOrBytesInCurrentSlice;
-      if(LIKELY(size_t { 0 } != cFirstSplits)) {
+      if(LIKELY(size_t { 1 } < cFirstSlices)) {
+         const size_t * const pcBytesInSliceLast = pcBytesInSliceEnd - size_t { 1 };
          ActiveDataType * pSplitFirst = pInnerTermUpdate->GetSplitPointer(iDimensionWrite);
-         // converting negative to positive number is defined behavior in C++ and uses twos compliment
-         size_t iSplitFirst = static_cast<size_t>(ptrdiff_t { -1 });
+         size_t iEdgeFirst = 0;
          do {
             EBM_ASSERT(pcBytesInSlice2 < pcBytesInSliceLast);
             EBM_ASSERT(0 != *pcBytesInSlice2);
             EBM_ASSERT(0 == *pcBytesInSlice2 % cBytesPerBin);
-            iSplitFirst += *pcBytesInSlice2 / cBytesPerBin;
-            *pSplitFirst = iSplitFirst;
+            iEdgeFirst += *pcBytesInSlice2 / cBytesPerBin;
+            *pSplitFirst = iEdgeFirst;
             ++pSplitFirst;
             ++pcBytesInSlice2;
             // the last one is the distance to the end, which we don't include in the update
          } while(LIKELY(pcBytesInSliceLast != pcBytesInSlice2));
       }
 
       RandomSplitState * pState = randomSplitState;
       if(PREDICTABLE(pStateInit != pState)) {
          do {
             do {
-               const FeatureBoosting * const pFeature = *ppFeature4;
+               const FeatureBoosting * const pFeature = pTermFeature4->m_pFeature;
                cBinsWrite = pFeature->GetCountBins();
                ++iDimensionWrite;
-               ++ppFeature4;
+               ++pTermFeature4;
             } while(cBinsWrite <= size_t { 1 });
 
             ++pcBytesInSlice2; // we have one less split than we have slices, so move to the next one
 
-            const size_t * pcItemsInNextSliceLast = pState->m_pcItemsInNextSliceEnd - size_t { 1 };
-            error = pInnerTermUpdate->SetCountSplits(iDimensionWrite, pcItemsInNextSliceLast - pcBytesInSlice2);
+            const size_t * pcItemsInNextSliceEnd = pState->m_pcItemsInNextSliceEnd;
+            error = pInnerTermUpdate->SetCountSlices(iDimensionWrite, pcItemsInNextSliceEnd - pcBytesInSlice2);
             if(Error_None != error) {
                // already logged
                free(pBuffer);
                return error;
             }
+            const size_t * pcItemsInNextSliceLast = pcItemsInNextSliceEnd - size_t { 1 };
             if(pcItemsInNextSliceLast != pcBytesInSlice2) {
                ActiveDataType * pSplit = pInnerTermUpdate->GetSplitPointer(iDimensionWrite);
-               size_t iSplit2 = *pcItemsInNextSliceLast - size_t { 1 };
-               *pSplit = iSplit2;
+               size_t iEdge2 = *pcItemsInNextSliceLast;
+               *pSplit = iEdge2;
                --pcItemsInNextSliceLast;
                while(pcItemsInNextSliceLast != pcBytesInSlice2) {
-                  iSplit2 += *pcBytesInSlice2;
+                  iEdge2 += *pcBytesInSlice2;
                   ++pSplit;
-                  *pSplit = iSplit2;
+                  *pSplit = iEdge2;
                   ++pcBytesInSlice2;
                }
                // increment it once more because our indexes are shifted such that the first one was the last item
                ++pcBytesInSlice2;
             }
             ++pState;
          } while(PREDICTABLE(pStateInit != pState));
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/PartitionTwoDimensionalBoosting.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/PartitionTwoDimensionalBoosting.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -221,33 +221,33 @@
       EBM_ASSERT(2 == pTerm->GetCountRealDimensions());
       EBM_ASSERT(2 <= pTerm->GetCountDimensions());
       size_t iDimensionLoop = 0;
       size_t iDimension1 = 0;
       size_t iDimension2 = 0;
       size_t cBinsDimension1 = 0;
       size_t cBinsDimension2 = 0;
-      const FeatureBoosting * const * ppFeature = pTerm->GetFeatures();
-      const FeatureBoosting * const * const ppFeaturesEnd = &ppFeature[pTerm->GetCountDimensions()];
+      const TermFeature * pTermFeature = pTerm->GetTermFeatures();
+      const TermFeature * const pTermFeaturesEnd = &pTermFeature[pTerm->GetCountDimensions()];
       do {
-         const FeatureBoosting * const pFeature = *ppFeature;
+         const FeatureBoosting * const pFeature = pTermFeature->m_pFeature;
          const size_t cBins = pFeature->GetCountBins();
          EBM_ASSERT(size_t { 1 } <= cBins); // we don't boost on empty training sets
          if(size_t { 1 } < cBins) {
             EBM_ASSERT(0 == cBinsDimension2);
             if(0 == cBinsDimension1) {
                iDimension1 = iDimensionLoop;
                cBinsDimension1 = cBins;
             } else {
                iDimension2 = iDimensionLoop;
                cBinsDimension2 = cBins;
             }
          }
          ++iDimensionLoop;
-         ++ppFeature;
-      } while(ppFeaturesEnd != ppFeature);
+         ++pTermFeature;
+      } while(pTermFeaturesEnd != pTermFeature);
       EBM_ASSERT(2 <= cBinsDimension1);
       EBM_ASSERT(2 <= cBinsDimension2);
 
       FloatBig bestGain = k_illegalGainFloat;
 
       size_t splitFirst1Best;
       size_t splitFirst1LowBest;
@@ -483,60 +483,60 @@
                EBM_ASSERT(k_epsilonNegativeGainAllowed <= bestGain);
 
                *pTotalGain = 0;
                if(LIKELY(k_gainMin <= bestGain)) {
                   *pTotalGain = static_cast<double>(bestGain);
                   if(bSplitFirst2) {
                      // if bSplitFirst2 is true, then there definetly was a split, so we don't have to check for zero splits
-                     error = pInnerTermUpdate->SetCountSplits(iDimension2, 1);
+                     error = pInnerTermUpdate->SetCountSlices(iDimension2, 2);
                      if(Error_None != error) {
                         // already logged
                         return error;
                      }
-                     pInnerTermUpdate->GetSplitPointer(iDimension2)[0] = splitFirst2Best;
+                     pInnerTermUpdate->GetSplitPointer(iDimension2)[0] = splitFirst2Best + 1;
 
                      if(splitFirst2LowBest < splitFirst2HighBest) {
                         error = pInnerTermUpdate->EnsureTensorScoreCapacity(cScores * 6);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
-                        error = pInnerTermUpdate->SetCountSplits(iDimension1, 2);
+                        error = pInnerTermUpdate->SetCountSlices(iDimension1, 3);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
-                        pInnerTermUpdate->GetSplitPointer(iDimension1)[0] = splitFirst2LowBest;
-                        pInnerTermUpdate->GetSplitPointer(iDimension1)[1] = splitFirst2HighBest;
+                        pInnerTermUpdate->GetSplitPointer(iDimension1)[0] = splitFirst2LowBest + 1;
+                        pInnerTermUpdate->GetSplitPointer(iDimension1)[1] = splitFirst2HighBest + 1;
                      } else if(splitFirst2HighBest < splitFirst2LowBest) {
                         error = pInnerTermUpdate->EnsureTensorScoreCapacity(cScores * 6);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
-                        error = pInnerTermUpdate->SetCountSplits(iDimension1, 2);
+                        error = pInnerTermUpdate->SetCountSlices(iDimension1, 3);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
-                        pInnerTermUpdate->GetSplitPointer(iDimension1)[0] = splitFirst2HighBest;
-                        pInnerTermUpdate->GetSplitPointer(iDimension1)[1] = splitFirst2LowBest;
+                        pInnerTermUpdate->GetSplitPointer(iDimension1)[0] = splitFirst2HighBest + 1;
+                        pInnerTermUpdate->GetSplitPointer(iDimension1)[1] = splitFirst2LowBest + 1;
                      } else {
-                        error = pInnerTermUpdate->SetCountSplits(iDimension1, 1);
+                        error = pInnerTermUpdate->SetCountSlices(iDimension1, 2);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
 
                         error = pInnerTermUpdate->EnsureTensorScoreCapacity(cScores * 4);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
-                        pInnerTermUpdate->GetSplitPointer(iDimension1)[0] = splitFirst2LowBest;
+                        pInnerTermUpdate->GetSplitPointer(iDimension1)[0] = splitFirst2LowBest + 1;
                      }
 
                      auto * const pGradientPairTotals2LowLowBest = pTotals2LowLowBest->GetGradientPairs();
                      auto * const pGradientPairTotals2LowHighBest = pTotals2LowHighBest->GetGradientPairs();
                      auto * const pGradientPairTotals2HighLowBest = pTotals2HighLowBest->GetGradientPairs();
                      auto * const pGradientPairTotals2HighHighBest = pTotals2HighHighBest->GetGradientPairs();
                      for(size_t iScore = 0; iScore < cScores; ++iScore) {
@@ -600,68 +600,68 @@
                            aUpdateScores[0 * cScores + iScore] = SafeConvertFloat<FloatFast>(predictionLowLow);
                            aUpdateScores[1 * cScores + iScore] = SafeConvertFloat<FloatFast>(predictionLowHigh);
                            aUpdateScores[2 * cScores + iScore] = SafeConvertFloat<FloatFast>(predictionHighLow);
                            aUpdateScores[3 * cScores + iScore] = SafeConvertFloat<FloatFast>(predictionHighHigh);
                         }
                      }
                   } else {
-                     error = pInnerTermUpdate->SetCountSplits(iDimension1, 1);
+                     error = pInnerTermUpdate->SetCountSlices(iDimension1, 2);
                      if(Error_None != error) {
                         // already logged
                         return error;
                      }
 
                      // The Clang static analyzer believes that splitFirst1Best could contain uninitialized garbage
                      // We can only reach here if bSplitFirst2 is false and if k_illegalGainFloat != bestGain
                      // Since bestGain is only set in two places, and since in one of those bSplitFirst2 is set to true
                      // our code path above must have gone through the section that set both bestGain and 
                      // splitFirst1Best.  The Clang static analyzer does not seem to recognize this, so stop it
                      StopClangAnalysis();
-                     pInnerTermUpdate->GetSplitPointer(iDimension1)[0] = splitFirst1Best;
+                     pInnerTermUpdate->GetSplitPointer(iDimension1)[0] = splitFirst1Best + 1;
 
                      if(splitFirst1LowBest < splitFirst1HighBest) {
                         error = pInnerTermUpdate->EnsureTensorScoreCapacity(cScores * 6);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
 
-                        error = pInnerTermUpdate->SetCountSplits(iDimension2, 2);
+                        error = pInnerTermUpdate->SetCountSlices(iDimension2, 3);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
-                        pInnerTermUpdate->GetSplitPointer(iDimension2)[0] = splitFirst1LowBest;
-                        pInnerTermUpdate->GetSplitPointer(iDimension2)[1] = splitFirst1HighBest;
+                        pInnerTermUpdate->GetSplitPointer(iDimension2)[0] = splitFirst1LowBest + 1;
+                        pInnerTermUpdate->GetSplitPointer(iDimension2)[1] = splitFirst1HighBest + 1;
                      } else if(splitFirst1HighBest < splitFirst1LowBest) {
                         error = pInnerTermUpdate->EnsureTensorScoreCapacity(cScores * 6);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
 
-                        error = pInnerTermUpdate->SetCountSplits(iDimension2, 2);
+                        error = pInnerTermUpdate->SetCountSlices(iDimension2, 3);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
-                        pInnerTermUpdate->GetSplitPointer(iDimension2)[0] = splitFirst1HighBest;
-                        pInnerTermUpdate->GetSplitPointer(iDimension2)[1] = splitFirst1LowBest;
+                        pInnerTermUpdate->GetSplitPointer(iDimension2)[0] = splitFirst1HighBest + 1;
+                        pInnerTermUpdate->GetSplitPointer(iDimension2)[1] = splitFirst1LowBest + 1;
                      } else {
-                        error = pInnerTermUpdate->SetCountSplits(iDimension2, 1);
+                        error = pInnerTermUpdate->SetCountSlices(iDimension2, 2);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
                         error = pInnerTermUpdate->EnsureTensorScoreCapacity(cScores * 4);
                         if(Error_None != error) {
                            // already logged
                            return error;
                         }
-                        pInnerTermUpdate->GetSplitPointer(iDimension2)[0] = splitFirst1LowBest;
+                        pInnerTermUpdate->GetSplitPointer(iDimension2)[0] = splitFirst1LowBest + 1;
                      }
 
                      auto * const pGradientPairTotals1LowLowBest = pTotals1LowLowBest->GetGradientPairs();
                      auto * const pGradientPairTotals1LowHighBest = pTotals1LowHighBest->GetGradientPairs();
                      auto * const pGradientPairTotals1HighLowBest = pTotals1HighLowBest->GetGradientPairs();
                      auto * const pGradientPairTotals1HighHighBest = pTotals1HighHighBest->GetGradientPairs();
                      for(size_t iScore = 0; iScore < cScores; ++iScore) {
@@ -740,22 +740,22 @@
          EBM_ASSERT(!std::isnan(bestGain));
       }
 
       // there were no good splits found
 #ifndef NDEBUG
       const ErrorEbm errorDebug1 =
 #endif // NDEBUG
-         pInnerTermUpdate->SetCountSplits(iDimension1, 0);
+         pInnerTermUpdate->SetCountSlices(iDimension1, 1);
       // we can't fail since we're setting this to zero, so no allocations.  We don't in fact need the split array at all
       EBM_ASSERT(Error_None == errorDebug1);
 
 #ifndef NDEBUG
       const ErrorEbm errorDebug2 =
 #endif // NDEBUG
-         pInnerTermUpdate->SetCountSplits(iDimension2, 0);
+         pInnerTermUpdate->SetCountSlices(iDimension2, 1);
       // we can't fail since we're setting this to zero, so no allocations.  We don't in fact need the split array at all
       EBM_ASSERT(Error_None == errorDebug2);
 
       // we don't need to call pInnerTermUpdate->EnsureTensorScoreCapacity, 
       // since our value capacity would be 1, which is pre-allocated
 
       for(size_t iScore = 0; iScore < cScores; ++iScore) {
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/PartitionTwoDimensionalInteraction.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/PartitionTwoDimensionalInteraction.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/RandomDeterministic.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/RandomDeterministic.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/RandomDeterministic.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/RandomDeterministic.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/RandomNondeterministic.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/RandomNondeterministic.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/SplitPosition.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/SplitPosition.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/Tensor.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/Tensor.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -58,25 +58,25 @@
    // we check elsewhere that IEEE754 is used, so bit zeroing is making zeroed floats
    memset(aTensorScores, 0, sizeof(*aTensorScores) * cScores);
 
    if(0 != cDimensionsMax) {
       DimensionInfo * pDimension = pTensor->GetDimensions();
       size_t iDimension = 0;
       do {
-         pDimension->m_cSplits = 0;
-         pDimension->m_cSplitCapacity = k_initialSplitCapacity;
+         pDimension->m_cSlices = 1;
+         pDimension->m_cSliceCapacity = k_initialSliceCapacity;
          pDimension->m_aSplits = nullptr;
          ++pDimension;
          ++iDimension;
       } while(iDimension < cDimensionsMax);
 
       pDimension = pTensor->GetDimensions();
       iDimension = 0;
       do {
-         ActiveDataType * const aSplits = static_cast<ActiveDataType *>(malloc(sizeof(ActiveDataType) * k_initialSplitCapacity));
+         ActiveDataType * const aSplits = static_cast<ActiveDataType *>(malloc(sizeof(ActiveDataType) * (k_initialSliceCapacity - 1)));
          if(UNLIKELY(nullptr == aSplits)) {
             LOG_0(Trace_Warning, "WARNING Allocate nullptr == aSplits");
             Free(pTensor); // free everything!
             return nullptr;
          }
          pDimension->m_aSplits = aSplits;
          ++pDimension;
@@ -100,32 +100,33 @@
       free(pTensor);
    }
 }
 
 void Tensor::Reset() {
    DimensionInfo * pDimensionInfo = GetDimensions();
    for(size_t iDimension = 0; iDimension < m_cDimensions; ++iDimension) {
-      pDimensionInfo[iDimension].m_cSplits = 0;
+      pDimensionInfo[iDimension].m_cSlices = 1;
    }
    // we only need to set the base case to zero
    // this can't overflow since we previously allocated this memory
    for(size_t i = 0; i < m_cScores; ++i) {
       m_aTensorScores[i] = 0;
    }
    m_bExpanded = false;
 }
 
-ErrorEbm Tensor::SetCountSplits(const size_t iDimension, const size_t cSplits) {
+ErrorEbm Tensor::SetCountSlices(const size_t iDimension, const size_t cSlices) {
    EBM_ASSERT(iDimension < m_cDimensions);
    DimensionInfo * const pDimension = &GetDimensions()[iDimension];
    // we shouldn't be able to expand our length after we're been expanded since expanded should be the maximum size already
-   EBM_ASSERT(!m_bExpanded || cSplits <= pDimension->m_cSplits);
-   if(UNLIKELY(pDimension->m_cSplitCapacity < cSplits)) {
+   EBM_ASSERT(!m_bExpanded || cSlices <= pDimension->m_cSlices);
+   if(UNLIKELY(pDimension->m_cSliceCapacity < cSlices)) {
       EBM_ASSERT(!m_bExpanded); // we shouldn't be able to expand our length after we're been expanded since expanded should be the maximum size already
 
+      size_t cSplits = cSlices - 1;
       if(IsAddError(cSplits, cSplits >> 1)) {
          LOG_0(Trace_Warning, "WARNING SetCountSplits IsAddError(cSplits, cSplits >> 1)");
          return Error_OutOfMemory;
       }
       // just increase it by 50% since we don't expect to grow our splits often after an initial period, 
       // and realloc takes some of the cost of growing away
       size_t cNewSplitCapacity = cSplits + (cSplits >> 1);
@@ -140,17 +141,17 @@
       if(UNLIKELY(nullptr == aNewSplits)) {
          // according to the realloc spec, if realloc fails to allocate the new memory, it returns nullptr BUT the old memory is valid.
          // we leave m_aThreadByteBuffer1 alone in this instance and will free that memory later in the destructor
          LOG_0(Trace_Warning, "WARNING SetCountSplits nullptr == aNewSplits");
          return Error_OutOfMemory;
       }
       pDimension->m_aSplits = aNewSplits;
-      pDimension->m_cSplitCapacity = cNewSplitCapacity;
+      pDimension->m_cSliceCapacity = cNewSplitCapacity + 1;
    } // never shrink our array unless the user chooses to Trim()
-   pDimension->m_cSplits = cSplits;
+   pDimension->m_cSlices = cSlices;
    return Error_None;
 }
 
 ErrorEbm Tensor::EnsureTensorScoreCapacity(const size_t cTensorScores) {
    if(UNLIKELY(m_cTensorScoreCapacity < cTensorScores)) {
       EBM_ASSERT(!m_bExpanded); // we shouldn't be able to expand our length after we're been expanded since expanded should be the maximum size already
 
@@ -187,24 +188,24 @@
 
    const DimensionInfo * pThisDimensionInfo = GetDimensions();
    const DimensionInfo * pRhsDimensionInfo = rhs.GetDimensions();
 
    size_t cTensorScores = m_cScores;
    for(size_t iDimension = 0; iDimension < m_cDimensions; ++iDimension) {
       const DimensionInfo * const pDimension = &pRhsDimensionInfo[iDimension];
-      size_t cSplits = pDimension->m_cSplits;
-      EBM_ASSERT(!IsMultiplyError(cTensorScores, cSplits + 1)); // we're copying this memory, so multiplication can't overflow
-      cTensorScores *= (cSplits + 1);
-      error = SetCountSplits(iDimension, cSplits);
+      size_t cSlices = pDimension->m_cSlices;
+      EBM_ASSERT(!IsMultiplyError(cTensorScores, cSlices)); // we're copying this memory, so multiplication can't overflow
+      cTensorScores *= cSlices;
+      error = SetCountSlices(iDimension, cSlices);
       if(UNLIKELY(Error_None != error)) {
-         LOG_0(Trace_Warning, "WARNING Copy SetCountSplits(iDimension, cSplits)");
+         LOG_0(Trace_Warning, "WARNING Copy SetCountSlices(iDimension, cSlices)");
          return error;
       }
-      EBM_ASSERT(!IsMultiplyError(sizeof(ActiveDataType), cSplits)); // we're copying this memory, so multiplication can't overflow
-      memcpy(pThisDimensionInfo[iDimension].m_aSplits, pDimension->m_aSplits, sizeof(ActiveDataType) * cSplits);
+      EBM_ASSERT(!IsMultiplyError(sizeof(ActiveDataType), cSlices - 1)); // we're copying this memory, so multiplication can't overflow
+      memcpy(pThisDimensionInfo[iDimension].m_aSplits, pDimension->m_aSplits, sizeof(ActiveDataType) * (cSlices - 1));
    }
    error = EnsureTensorScoreCapacity(cTensorScores);
    if(UNLIKELY(Error_None != error)) {
       // already logged
       return error;
    }
    EBM_ASSERT(!IsMultiplyError(sizeof(FloatFast), cTensorScores)); // we're copying this memory, so multiplication can't overflow
@@ -216,16 +217,16 @@
 bool Tensor::MultiplyAndCheckForIssues(const double v) {
    const FloatFast vFloat = SafeConvertFloat<FloatFast>(v);
    const DimensionInfo * pThisDimensionInfo = GetDimensions();
 
    size_t cTensorScores = m_cScores;
    for(size_t iDimension = 0; iDimension < m_cDimensions; ++iDimension) {
       // we're accessing existing memory, so it can't overflow
-      EBM_ASSERT(!IsMultiplyError(cTensorScores, pThisDimensionInfo[iDimension].m_cSplits + 1));
-      cTensorScores *= pThisDimensionInfo[iDimension].m_cSplits + 1;
+      EBM_ASSERT(!IsMultiplyError(cTensorScores, pThisDimensionInfo[iDimension].m_cSlices));
+      cTensorScores *= pThisDimensionInfo[iDimension].m_cSlices;
    }
 
    FloatFast * pCur = &m_aTensorScores[0];
    FloatFast * pEnd = &m_aTensorScores[cTensorScores];
    int bBad = 0;
    // we always have 1 score, even if we have zero splits
    do {
@@ -255,47 +256,46 @@
       LOG_0(Trace_Verbose, "Exited Expand");
       return Error_None;
    }
 
    EBM_ASSERT(nullptr != pTerm);
    const size_t cDimensions = pTerm->GetCountDimensions();
    if(size_t { 0 } != cDimensions) {
-      const FeatureBoosting * const * ppFeature1 = pTerm->GetFeatures();
-      const FeatureBoosting * const * const ppFeaturesEnd = &ppFeature1[cDimensions];
+      const TermFeature * pTermFeature1 = pTerm->GetTermFeatures();
+      const TermFeature * const pTermFeaturesEnd = &pTermFeature1[cDimensions];
       DimensionInfoStackExpand aDimensionInfoStackExpand[k_cDimensionsMax];
       DimensionInfoStackExpand * pDimensionInfoStackFirst = aDimensionInfoStackExpand;
       const DimensionInfo * pDimensionFirst1 = GetDimensions();
       size_t cTensorScores1 = m_cScores;
 #ifndef NDEBUG
       size_t cNewTensorScoresDebug = m_cScores;
 #endif // NDEBUG
       // first, get basic counts of how many splits and scores we'll have in our final result
       do {
-         const FeatureBoosting * const pFeature = *ppFeature1;
+         const FeatureBoosting * const pFeature = pTermFeature1->m_pFeature;
          const size_t cBins = pFeature->GetCountBins();
 
 #ifndef NDEBUG
          cNewTensorScoresDebug *= cBins;
 #endif // NDEBUG
 
-         const size_t cSplits1 = pDimensionFirst1->m_cSplits;
+         const size_t cSlices1 = pDimensionFirst1->m_cSlices;
 
-         EBM_ASSERT(!IsMultiplyError(cTensorScores1, cSplits1 + 1)); // this is accessing existing memory, so it can't overflow
-         cTensorScores1 *= cSplits1 + 1;
+         EBM_ASSERT(!IsMultiplyError(cTensorScores1, cSlices1)); // this is accessing existing memory, so it can't overflow
+         cTensorScores1 *= cSlices1;
 
-         pDimensionInfoStackFirst->m_pSplit1 = &pDimensionFirst1->m_aSplits[cSplits1];
+         pDimensionInfoStackFirst->m_pSplit1 = &pDimensionFirst1->m_aSplits[cSlices1 - 1];
 
-         const size_t cSplits = cBins - size_t { 1 };
-         pDimensionInfoStackFirst->m_iSplit2 = cSplits;
-         pDimensionInfoStackFirst->m_cNewSplits = cSplits;
+         pDimensionInfoStackFirst->m_iEdge2 = cBins;
+         pDimensionInfoStackFirst->m_cNewSlices = cBins;
 
          ++pDimensionFirst1;
          ++pDimensionInfoStackFirst;
-         ++ppFeature1;
-      } while(ppFeaturesEnd != ppFeature1);
+         ++pTermFeature1;
+      } while(pTermFeaturesEnd != pTermFeature1);
 
       EBM_ASSERT(!IsMultiplyError(m_cScores, pTerm->GetCountTensorBins()));
       const size_t cNewTensorScores = m_cScores * pTerm->GetCountTensorBins();
       EBM_ASSERT(cNewTensorScoresDebug == cNewTensorScores);
       EBM_ASSERT(1 <= cNewTensorScores);
 
       // call EnsureTensorScoreCapacity before using the m_aTensorScores pointer since m_aTensorScores might change inside EnsureTensorScoreCapacity
@@ -339,107 +339,107 @@
          DimensionInfoStackExpand * pDimensionInfoStackSecond = aDimensionInfoStackExpand;
          const DimensionInfo * pDimensionSecond1 = aDimension1;
 
          size_t multiplication1 = m_cScores;
 
          while(true) {
             const ActiveDataType * const pSplit1 = pDimensionInfoStackSecond->m_pSplit1;
-            size_t iSplit2 = pDimensionInfoStackSecond->m_iSplit2;
+            size_t iEdge2 = pDimensionInfoStackSecond->m_iEdge2;
 
             ActiveDataType * const aSplits1 = pDimensionSecond1->m_aSplits;
 
-            EBM_ASSERT(static_cast<size_t>(pSplit1 - aSplits1) <= iSplit2);
+            EBM_ASSERT(static_cast<size_t>(pSplit1 - aSplits1) < iEdge2);
             if(UNPREDICTABLE(aSplits1 < pSplit1)) {
-               EBM_ASSERT(0 < iSplit2);
+               EBM_ASSERT(1 < iEdge2);
 
                const ActiveDataType * const pSplit1MinusOne = pSplit1 - 1;
 
                const size_t d1 = static_cast<size_t>(*pSplit1MinusOne);
 
-               --iSplit2;
+               --iEdge2;
 
-               const bool bMove = UNPREDICTABLE(iSplit2 <= d1);
+               const bool bMove = UNPREDICTABLE(iEdge2 <= d1);
                pDimensionInfoStackSecond->m_pSplit1 = bMove ? pSplit1MinusOne : pSplit1;
                pTensorScore1 = bMove ? pTensorScore1 - multiplication1 : pTensorScore1;
 
-               pDimensionInfoStackSecond->m_iSplit2 = iSplit2;
+               pDimensionInfoStackSecond->m_iEdge2 = iEdge2;
                break;
             } else {
-               if(UNPREDICTABLE(0 < iSplit2)) {
-                  pDimensionInfoStackSecond->m_iSplit2 = iSplit2 - 1;
+               if(UNPREDICTABLE(1 < iEdge2)) {
+                  pDimensionInfoStackSecond->m_iEdge2 = iEdge2 - 1;
                   break;
                } else {
                   pTensorScore1 -= multiplication1; // put us before the beginning.  We'll add the full row first
 
-                  const size_t cSplits1 = pDimensionSecond1->m_cSplits;
+                  const size_t cSlices1 = pDimensionSecond1->m_cSlices;
 
                   // we're already allocated scores, so this is accessing what we've already allocated, so it must not overflow
-                  EBM_ASSERT(!IsMultiplyError(multiplication1, 1 + cSplits1));
-                  multiplication1 *= 1 + cSplits1;
+                  EBM_ASSERT(!IsMultiplyError(multiplication1, cSlices1));
+                  multiplication1 *= cSlices1;
 
                   // go to the last valid entry back to where we started.  If we don't move down a set, then we re-do this set of numbers
                   pTensorScore1 += multiplication1;
 
-                  pDimensionInfoStackSecond->m_pSplit1 = &aSplits1[cSplits1];
-                  pDimensionInfoStackSecond->m_iSplit2 = pDimensionInfoStackSecond->m_cNewSplits;
+                  pDimensionInfoStackSecond->m_pSplit1 = &aSplits1[cSlices1 - 1];
+                  pDimensionInfoStackSecond->m_iEdge2 = pDimensionInfoStackSecond->m_cNewSlices;
 
                   ++pDimensionSecond1;
                   ++pDimensionInfoStackSecond;
                   continue;
                }
             }
          }
       }
 
       EBM_ASSERT(pTensorScoreTop == m_aTensorScores);
       EBM_ASSERT(pTensorScore1 == m_aTensorScores + m_cScores);
 
-      const FeatureBoosting * const * ppFeature2 = pTerm->GetFeatures();
+      const TermFeature * pTermFeature2 = pTerm->GetTermFeatures();
       size_t iDimension = 0;
       do {
-         const FeatureBoosting * const pFeature = *ppFeature2;
+         const FeatureBoosting * const pFeature = pTermFeature2->m_pFeature;
          const size_t cBins = pFeature->GetCountBins();
          EBM_ASSERT(size_t { 1 } <= cBins); // we exited above on tensors with zero bins in any dimension
-         const size_t cSplits = cBins - size_t { 1 };
+         const size_t cSlices = cBins;
          const DimensionInfo * const pDimension = &aDimension1[iDimension];
-         if(cSplits != pDimension->m_cSplits) {
-            error = SetCountSplits(iDimension, cSplits);
+         if(cSlices != pDimension->m_cSlices) {
+            error = SetCountSlices(iDimension, cSlices);
             if(UNLIKELY(Error_None != error)) {
                // already logged
                return error;
             }
 
-            // if cSplits is zero then pDimension->m_cSplits must be zero and we'd be filtered out above
-            EBM_ASSERT(size_t { 1 } <= cSplits);
+            // if cSlices is 1 then pDimension->m_cSlices must be 1 and we'd be filtered out above
+            EBM_ASSERT(size_t { 2 } <= cSlices);
 
             ActiveDataType * const aSplit = pDimension->m_aSplits;
-            size_t iSplit = 0;
+            size_t iEdge = 1;
             do {
-               aSplit[iSplit] = iSplit;
-               ++iSplit;
-            } while(cSplits != iSplit);
+               aSplit[iEdge - 1] = iEdge;
+               ++iEdge;
+            } while(cSlices != iEdge);
          }
          ++iDimension;
-         ++ppFeature2;
-      } while(ppFeaturesEnd != ppFeature2);
+         ++pTermFeature2;
+      } while(pTermFeaturesEnd != pTermFeature2);
    }
    m_bExpanded = true;
    
    LOG_0(Trace_Verbose, "Exited Expand");
    return Error_None;
 }
 
 void Tensor::AddExpandedWithBadValueProtection(const FloatFast * const aFromScores) {
    EBM_ASSERT(m_bExpanded);
    size_t cItems = m_cScores;
 
    const DimensionInfo * const aDimension = GetDimensions();
    for(size_t iDimension = 0; iDimension < m_cDimensions; ++iDimension) {
       // this can't overflow since we've already allocated them!
-      cItems *= aDimension[iDimension].m_cSplits + 1;
+      cItems *= aDimension[iDimension].m_cSlices;
    }
 
    const FloatFast * pFromScore = aFromScores;
    FloatFast * pToScore = m_aTensorScores;
    const FloatFast * const pToScoresEnd = m_aTensorScores + cItems;
    do {
       // if we get a NaN value, then just consider it a no-op zero
@@ -506,57 +506,57 @@
    size_t cTensorScores1 = m_cScores;
    size_t cTensorScores2 = m_cScores;
    size_t cNewTensorScores = m_cScores;
 
    EBM_ASSERT(1 <= m_cDimensions);
    // first, get basic counts of how many splits and values we'll have in our final result
    do {
-      const size_t cSplits1 = pDimensionFirst1->m_cSplits;
+      const size_t cSlices1 = pDimensionFirst1->m_cSlices;
       ActiveDataType * p1Cur = pDimensionFirst1->m_aSplits;
-      const size_t cSplits2 = pDimensionFirst2->m_cSplits;
+      const size_t cSlices2 = pDimensionFirst2->m_cSlices;
       ActiveDataType * p2Cur = pDimensionFirst2->m_aSplits;
 
-      cTensorScores1 *= cSplits1 + 1; // this can't overflow since we're counting existing allocated memory
-      cTensorScores2 *= cSplits2 + 1; // this can't overflow since we're counting existing allocated memory
+      cTensorScores1 *= cSlices1; // this can't overflow since we're counting existing allocated memory
+      cTensorScores2 *= cSlices2; // this can't overflow since we're counting existing allocated memory
 
-      ActiveDataType * const p1End = &p1Cur[cSplits1];
-      ActiveDataType * const p2End = &p2Cur[cSplits2];
+      ActiveDataType * const p1End = &p1Cur[cSlices1 - 1];
+      ActiveDataType * const p2End = &p2Cur[cSlices2 - 1];
 
       pDimensionInfoStackFirst->m_pSplit1 = p1End;
       pDimensionInfoStackFirst->m_pSplit2 = p2End;
 
-      size_t cNewSingleDimensionSplits = 0;
+      size_t cNewSingleDimensionSlices = 1;
 
       // processing forwards here is slightly faster in terms of cache fetch efficiency.  We'll then be guaranteed to have the splits at least
       // in the cache, which will be benefitial when traversing backwards later below
       while(true) {
          if(UNLIKELY(p2End == p2Cur)) {
             // check the other array first.  Most of the time the other array will be shorter since we'll be adding
             // a sequence of sliced lines and our main line will be in *this, and there will be more slices in general for
             // a line that is added to a lot
-            cNewSingleDimensionSplits += static_cast<size_t>(p1End - p1Cur);
+            cNewSingleDimensionSlices += static_cast<size_t>(p1End - p1Cur);
             break;
          }
          if(UNLIKELY(p1End == p1Cur)) {
-            cNewSingleDimensionSplits += static_cast<size_t>(p2End - p2Cur);
+            cNewSingleDimensionSlices += static_cast<size_t>(p2End - p2Cur);
             break;
          }
-         ++cNewSingleDimensionSplits; // if we move one or both pointers, we just added annother unique one
+         ++cNewSingleDimensionSlices; // if we move one or both pointers, we just added annother unique one
 
          const ActiveDataType d1 = *p1Cur;
          const ActiveDataType d2 = *p2Cur;
 
          p1Cur = UNPREDICTABLE(d1 <= d2) ? p1Cur + 1 : p1Cur;
          p2Cur = UNPREDICTABLE(d2 <= d1) ? p2Cur + 1 : p2Cur;
       }
-      pDimensionInfoStackFirst->m_cNewSplits = cNewSingleDimensionSplits;
+      pDimensionInfoStackFirst->m_cNewSlices = cNewSingleDimensionSlices;
       // we check for simple multiplication overflow from m_cBins in Booster::Initialize when we unpack featureIndexes and in 
       // CalcInteractionStrength for interactions
-      EBM_ASSERT(!IsMultiplyError(cNewTensorScores, cNewSingleDimensionSplits + 1));
-      cNewTensorScores *= cNewSingleDimensionSplits + 1;
+      EBM_ASSERT(!IsMultiplyError(cNewTensorScores, cNewSingleDimensionSlices));
+      cNewTensorScores *= cNewSingleDimensionSlices;
 
       ++pDimensionFirst1;
       ++pDimensionFirst2;
 
       ++pDimensionInfoStackFirst;
    } while(pDimensionInfoStackEnd != pDimensionInfoStackFirst);
 
@@ -640,29 +640,29 @@
                pTensorScore2 -= multiplication2;
                pDimensionInfoStackSecond->m_pSplit2 = pSplit2 - 1;
                break;
             } else {
                pTensorScore1 -= multiplication1; // put us before the beginning.  We'll add the full row first
                pTensorScore2 -= multiplication2; // put us before the beginning.  We'll add the full row first
 
-               const size_t cSplits1 = pDimensionSecond1->m_cSplits;
-               const size_t cSplits2 = pDimensionSecond2->m_cSplits;
+               const size_t cSlices1 = pDimensionSecond1->m_cSlices;
+               const size_t cSlices2 = pDimensionSecond2->m_cSlices;
 
-               EBM_ASSERT(!IsMultiplyError(multiplication1, 1 + cSplits1)); // we're accessing allocated memory, so it can't overflow
-               multiplication1 *= 1 + cSplits1;
-               EBM_ASSERT(!IsMultiplyError(multiplication2, 1 + cSplits2)); // we're accessing allocated memory, so it can't overflow
-               multiplication2 *= 1 + cSplits2;
+               EBM_ASSERT(!IsMultiplyError(multiplication1, cSlices1)); // we're accessing allocated memory, so it can't overflow
+               multiplication1 *= cSlices1;
+               EBM_ASSERT(!IsMultiplyError(multiplication2, cSlices2)); // we're accessing allocated memory, so it can't overflow
+               multiplication2 *= cSlices2;
 
                // go to the last valid entry back to where we started.  If we don't move down a set, then we re-do this set of numbers
                pTensorScore1 += multiplication1;
                // go to the last valid entry back to where we started.  If we don't move down a set, then we re-do this set of numbers
                pTensorScore2 += multiplication2;
 
-               pDimensionInfoStackSecond->m_pSplit1 = &aSplits1[cSplits1];
-               pDimensionInfoStackSecond->m_pSplit2 = &aSplits2[cSplits2];
+               pDimensionInfoStackSecond->m_pSplit1 = &aSplits1[cSlices1 - 1];
+               pDimensionInfoStackSecond->m_pSplit2 = &aSplits2[cSlices2 - 1];
                ++pDimensionSecond1;
                ++pDimensionSecond2;
                ++pDimensionInfoStackSecond;
                continue;
             }
          }
       }
@@ -675,29 +675,29 @@
    // now finally do the splits
 
    const DimensionInfoStack * pDimensionInfoStackCur = dimensionStack;
    const DimensionInfo * pDimension1Cur = aDimension1;
    const DimensionInfo * pDimension2Cur = aDimension2;
    size_t iDimension = 0;
    do {
-      const size_t cNewSplits = pDimensionInfoStackCur->m_cNewSplits;
-      const size_t cOriginalSplitsBeforeSetting = pDimension1Cur->m_cSplits;
+      const size_t cNewSlices = pDimensionInfoStackCur->m_cNewSlices;
+      const size_t cOriginalSlicesBeforeSetting = pDimension1Cur->m_cSlices;
 
       // this will increase our capacity, if required.  It will also change m_cSplits, so we get that before calling it.  
       // SetCountSplits might change m_aTensorScoresAndSplits, so we need to actually keep it here after getting m_cSplits but 
       // before set set all our pointers
-      error = SetCountSplits(iDimension, cNewSplits);
+      error = SetCountSlices(iDimension, cNewSlices);
       if(UNLIKELY(Error_None != error)) {
          // already logged
          return error;
       }
 
-      const ActiveDataType * p1Cur = &pDimension1Cur->m_aSplits[cOriginalSplitsBeforeSetting];
-      const ActiveDataType * p2Cur = &pDimension2Cur->m_aSplits[pDimension2Cur->m_cSplits];
-      ActiveDataType * pTopCur = &pDimension1Cur->m_aSplits[cNewSplits];
+      const ActiveDataType * p1Cur = &pDimension1Cur->m_aSplits[cOriginalSlicesBeforeSetting - 1];
+      const ActiveDataType * p2Cur = &pDimension2Cur->m_aSplits[pDimension2Cur->m_cSlices - 1];
+      ActiveDataType * pTopCur = &pDimension1Cur->m_aSplits[cNewSlices - 1];
 
       // traverse in reverse so that we can put our results at the higher order indexes where we are guaranteed not to overwrite our existing scores
       // which we still need to copy
       while(true) {
          EBM_ASSERT(pDimension1Cur->m_aSplits <= pTopCur);
          EBM_ASSERT(pDimension1Cur->m_aSplits <= p1Cur);
          EBM_ASSERT(pDimension2Cur->m_aSplits <= p2Cur);
@@ -754,26 +754,26 @@
    const DimensionInfo * pRhsDimensionInfo = rhs.GetDimensions();
 
    size_t cTensorScores = m_cScores;
    for(size_t iDimension = 0; iDimension < m_cDimensions; ++iDimension) {
       const DimensionInfo * const pDimension1 = &pThisDimensionInfo[iDimension];
       const DimensionInfo * const pDimension2 = &pRhsDimensionInfo[iDimension];
 
-      size_t cSplits = pDimension1->m_cSplits;
-      if(cSplits != pDimension2->m_cSplits) {
+      size_t cSlices = pDimension1->m_cSlices;
+      if(cSlices != pDimension2->m_cSlices) {
          return false;
       }
 
-      if(0 != cSplits) {
-         EBM_ASSERT(!IsMultiplyError(cTensorScores, cSplits + 1)); // we're accessing allocated memory, so it can't overflow
-         cTensorScores *= cSplits + 1;
+      if(1 < cSlices) {
+         EBM_ASSERT(!IsMultiplyError(cTensorScores, cSlices)); // we're accessing allocated memory, so it can't overflow
+         cTensorScores *= cSlices;
 
          const ActiveDataType * pD1Cur = pDimension1->m_aSplits;
          const ActiveDataType * pD2Cur = pDimension2->m_aSplits;
-         const ActiveDataType * const pD1End = pD1Cur + cSplits;
+         const ActiveDataType * const pD1End = pD1Cur + cSlices - 1;
          do {
             if(UNLIKELY(*pD1Cur != *pD2Cur)) {
                return false;
             }
             ++pD1Cur;
             ++pD2Cur;
          } while(LIKELY(pD1End != pD1Cur));
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/Tensor.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/Tensor.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
 #error DEFINED_ZONE_NAME must be defined
 #endif // DEFINED_ZONE_NAME
 
 class Term;
 
+// Terminology:
+// bin - features are binned in the caller. A feature has a set number of bins
+// slice - one or more adjacent bins grouped together
+// edge - the outer boundaries of the bins. Edges include the point before the first bin and the point after the
+//        last bin. If there are 2 bins, there are 3 edges. The number of edges is fixed for a feature after binning
+// split - an edge that is used to separate slices appart from one another. There are between 0 and n_bins - 1 splits
+
 // TODO: we need to radically change this data structure so that we can efficiently pass it between machines in a 
 // cluster AND within/between a GPU/CPU.  This stucture should be:
 //
 // IntEbm m_cBytes; // our caller can fetch the memory size of this Tensor and memcpy it over the network
 //// The first thing our caller should do is call into the C++ to fix the endian nature of this struct
 //// 0x3333333333333333 non-expanded, big endian
 //// 0x2222222222222222 non-expanded, little endian
@@ -39,21 +46,17 @@
 // UIntEbm m_endianAndIsExpanded;
 // NO m_cTensorScoreCapacity -> we have a function that calculates the maximum capacity and we allocate it all at the start
 // NO m_cTensorScores -> we don't need to pass this arround from process to process since it's global info and can be passed to the individual functions
 // NO m_cDimensionsMax -> we pre-determine the maximum size and always allocate the max max size
 // NO m_cDimensions; -> we can pass in the Term object to know the # of dimensions
 // FloatFast m_aTensorScores[]; // a space for our values
 // UIntEbm DIMENSION_1_SPLIT_POINTS
-// UIntEbm DIMENSION_1_BIN_COUNT -> we find this by traversing the 0th dimension items
+// UIntEbm DIMENSION_1_SLICE_COUNT -> we find this by traversing the 0th dimension items
 // UIntEbm DIMENSION_0_SPLIT_POINTS -> we travel backwards by the count
-// UIntEbm DIMENSION_0_BIN_COUNT -> we find this using m_cBytes to find the end, then subtract sizeof(UIntEbm)
-//
-// - use SLICE_COUNT instead of SPLIT_COUNT because then we can express tensors with zero bins AND we can still
-//   get to the End pointer because our slices don't and split points are both 64 bit numbers, so subtracting from
-//   the current pointer gets us to the next BIN_COUNT value since a bin count of 1 means zero splits, so subtract 1
+// UIntEbm DIMENSION_0_SLICE_COUNT -> we find this using m_cBytes to find the end, then subtract sizeof(UIntEbm)
 //
 // Reasons:
 //   - our super-parallel algorithm needs to split up the data and have separate processing cores process their data
 //     their outputs will be partial histograms. After a single cores does the tree buiding, that core will need to 
 //     push the term score updates to all the children nodes
 //   - in an MPI environment, or a Spark cluster, or in a GPU, we'll need to pass this data structure between nodes, 
 //     so it will need to be memcopy-able, which means no pointers (use 64-bit offsets), and it means that the data 
@@ -95,15 +98,15 @@
       DimensionInfoStack() = default; // preserve our POD status
       ~DimensionInfoStack() = default; // preserve our POD status
       void * operator new(std::size_t) = delete; // we only use malloc/free in this library
       void operator delete (void *) = delete; // we only use malloc/free in this library
 
       const ActiveDataType * m_pSplit1;
       const ActiveDataType * m_pSplit2;
-      size_t m_cNewSplits;
+      size_t m_cNewSlices;
    };
    static_assert(std::is_standard_layout<DimensionInfoStack>::value,
       "We use the struct hack in several places, so disallow non-standard_layout types in general");
    static_assert(std::is_trivial<DimensionInfoStack>::value,
       "We use memcpy in several places, so disallow non-trivial types in general");
    static_assert(std::is_pod<DimensionInfoStack>::value,
       "We use a lot of C constructs, so disallow non-POD types in general");
@@ -111,59 +114,56 @@
    struct DimensionInfoStackExpand final {
       DimensionInfoStackExpand() = default; // preserve our POD status
       ~DimensionInfoStackExpand() = default; // preserve our POD status
       void * operator new(std::size_t) = delete; // we only use malloc/free in this library
       void operator delete (void *) = delete; // we only use malloc/free in this library
 
       const ActiveDataType * m_pSplit1;
-      size_t m_iSplit2;
-      size_t m_cNewSplits;
+      size_t m_iEdge2;
+      size_t m_cNewSlices;
    };
    static_assert(std::is_standard_layout<DimensionInfoStackExpand>::value,
       "We use the struct hack in several places, so disallow non-standard_layout types in general");
    static_assert(std::is_trivial<DimensionInfoStackExpand>::value,
       "We use memcpy in several places, so disallow non-trivial types in general");
    static_assert(std::is_pod<DimensionInfoStackExpand>::value,
       "We use a lot of C constructs, so disallow non-POD types in general");
 
    struct DimensionInfo final {
       DimensionInfo() = default; // preserve our POD status
       ~DimensionInfo() = default; // preserve our POD status
       void * operator new(std::size_t) = delete; // we only use malloc/free in this library
       void operator delete (void *) = delete; // we only use malloc/free in this library
 
-      // TODO : change m_cSplits to m_cSlices to fit the rest of our framework where we always use bin/slices, but also
-      //        to represent tensors with slices that are 0 (truely empty without even 1 bin), and because we need
-      //        to multiply by cSlices, when calculating the tensor volume, so we can never get away or optimize the
-      //        need away for cSlicess, unlike perhaps cSplits which might in some cases allow for tricks to optimize
-      size_t m_cSplits;
+      size_t m_cSlices;
       ActiveDataType * m_aSplits;
-      size_t m_cSplitCapacity;
+      size_t m_cSliceCapacity;
    };
    static_assert(std::is_standard_layout<DimensionInfo>::value,
       "We use the struct hack in several places, so disallow non-standard_layout types in general");
    static_assert(std::is_trivial<DimensionInfo>::value,
       "We use memcpy in several places, so disallow non-trivial types in general");
    static_assert(std::is_pod<DimensionInfo>::value,
       "We use a lot of C constructs, so disallow non-POD types in general");
 
    // TODO : is this still required after we do tree splitting by pairs??
    // we always allocate our array because we don't want to Require Add(...) to check for the null pointer
    // always allocate one so that we never have to check if we have sufficient storage when we call Reset with one split and two values
-   static constexpr size_t k_initialSplitCapacity = 1;
+   static constexpr size_t k_initialSliceCapacity = 2;
    static constexpr size_t k_initialTensorCapacity = 2;
 
    size_t m_cTensorScoreCapacity;
    size_t m_cScores;
    size_t m_cDimensionsMax;
    size_t m_cDimensions;
    FloatFast * m_aTensorScores;
    bool m_bExpanded;
 
    // IMPORTANT: m_aDimensions must be in the last position for the struct hack and this must be standard layout
+   // TODO: make this length k_cDimensionsMax and reduce allocations as needed, so that we do not need the struct hack
    DimensionInfo m_aDimensions[1];
 
    inline const DimensionInfo * GetDimensions() const {
       return ArrayToPointer(m_aDimensions);
    }
    inline DimensionInfo * GetDimensions() {
       return ArrayToPointer(m_aDimensions);
@@ -180,23 +180,23 @@
    // a node in a distributed system.  After each node calculates it's term score update (represented by this
    // Tensor class), we'll need to reduce them accross all nodes, before adding together all the
    // Tensor classes and sending back a full update to the Nodes.  Since we'll be ferrying info
    // back and forth, we'll want to keep it in a more compressed format keeping split and not expanding
    // to a direct indexable tensor until after recieved by the nodes.  We'll NEED to keep the entire strucutre
    // as a single continuous chunk of memory.  At the very start will be our regular struct (containing the
    // full size of the data region at the top (64 bit since we don't know what processor we'll be on)
-   // We know the number of dimensions for an feature group at allocation, so we can put the values right below
+   // We know the number of dimensions for each term at allocation, so we can put the values right below
    // that.  When we find ourselves expanding dimensions, we can first figure out how much all the values and dimension
    // need to grow and then we can directly move each dimension pointed to object without needing to move the full
    // values array.
 
    static void Free(Tensor * const pTensor);
    static Tensor * Allocate(const size_t cDimensionsMax, const size_t cScores);
    void Reset();
-   ErrorEbm SetCountSplits(const size_t iDimension, const size_t cSplits);
+   ErrorEbm SetCountSlices(const size_t iDimension, const size_t cSlices);
    ErrorEbm EnsureTensorScoreCapacity(const size_t cTensorScores);
    ErrorEbm Copy(const Tensor & rhs);
    bool MultiplyAndCheckForIssues(const double v);
    ErrorEbm Expand(const Term * const pTerm);
    void AddExpandedWithBadValueProtection(const FloatFast * const aFromValues);
    ErrorEbm Add(const Tensor & rhs);
 
@@ -214,17 +214,17 @@
    }
 
    inline ActiveDataType * GetSplitPointer(const size_t iDimension) {
       EBM_ASSERT(iDimension < m_cDimensions);
       return GetDimensions()[iDimension].m_aSplits;
    }
 
-   inline size_t GetCountSplits(const size_t iDimension) {
+   inline size_t GetCountSlices(const size_t iDimension) {
       EBM_ASSERT(iDimension < m_cDimensions);
-      return GetDimensions()[iDimension].m_cSplits;
+      return GetDimensions()[iDimension].m_cSlices;
    }
 
    inline FloatFast * GetTensorScoresPointer() {
       return m_aTensorScores;
    }
 };
 static_assert(std::is_standard_layout<Tensor>::value,
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/TensorTotalsBuild.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/TensorTotalsBuild.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/TensorTotalsSum.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/TensorTotalsSum.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/Term.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/Term.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/Term.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/Term.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -15,37 +15,43 @@
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
 #error DEFINED_ZONE_NAME must be defined
 #endif // DEFINED_ZONE_NAME
 
 class FeatureBoosting;
 
+struct TermFeature {
+   const FeatureBoosting * m_pFeature;
+   size_t                  m_cStride;
+   size_t                  m_iTranspose;
+};
+
 class Term final {
    ptrdiff_t m_cItemsPerBitPack;
    size_t m_cDimensions;
    size_t m_cRealDimensions;
    size_t m_cTensorBins;
    size_t m_cAuxillaryBins;
    int m_cLogEnterGenerateTermUpdateMessages;
    int m_cLogExitGenerateTermUpdateMessages;
    int m_cLogEnterApplyTermUpdateMessages;
    int m_cLogExitApplyTermUpdateMessages;
 
    // IMPORTANT: m_apFeature must be in the last position for the struct hack and this must be standard layout
-   const FeatureBoosting * m_apFeature[k_cDimensionsMax];
+   TermFeature m_aTermFeatures[k_cDimensionsMax];
 
 public:
 
    Term() = default; // preserve our POD status
    ~Term() = default; // preserve our POD status
    void * operator new(std::size_t) = delete; // we only use malloc/free in this library
    void operator delete (void *) = delete; // we only use malloc/free in this library
 
    inline static size_t GetTermCountBytes(const size_t cDimensions) noexcept {
-      return offsetof(Term, m_apFeature) + sizeof(Term::m_apFeature[0]) * cDimensions;
+      return offsetof(Term, m_aTermFeatures) + sizeof(Term::m_aTermFeatures[0]) * cDimensions;
    }
 
    inline static void Free(Term * const pTerm) noexcept {
       free(pTerm);
    }
 
    inline void Initialize(const size_t cDimensions) noexcept {
@@ -97,19 +103,19 @@
       return m_cAuxillaryBins;
    }
 
    inline void SetCountAuxillaryBins(const size_t cAuxillaryBins) noexcept {
       m_cAuxillaryBins = cAuxillaryBins;
    }
 
-   inline const FeatureBoosting * const * GetFeatures() const noexcept {
-      return ArrayToPointer(m_apFeature);
+   inline const TermFeature * GetTermFeatures() const noexcept {
+      return ArrayToPointer(m_aTermFeatures);
    }
-   inline const FeatureBoosting ** GetFeatures() noexcept {
-      return ArrayToPointer(m_apFeature);
+   inline TermFeature * GetTermFeatures() noexcept {
+      return ArrayToPointer(m_aTermFeatures);
    }
 
    inline int * GetPointerCountLogEnterGenerateTermUpdateMessages() noexcept {
       return &m_cLogEnterGenerateTermUpdateMessages;
    }
 
    inline int * GetPointerCountLogExitGenerateTermUpdateMessages() noexcept {
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/TreeNode.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/TreeNode.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/bridge_c.h` & `interpret-core-0.4.2/symbolic/shared/libebm/bridge_c/bridge_c.h`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/bridge_c/zones.h` & `interpret-core-0.4.2/symbolic/shared/libebm/bridge_c/zones.h`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,22 @@
 #ifndef ZONES_H
 #define ZONES_H
 
 #ifdef __cplusplus
 extern "C" {
 #endif // __cplusplus
 
-#if defined(ZONE_main)
-#define DEFINED_ZONE_NAME      NAMESPACE_MAIN
-#elif defined(ZONE_cpu)
-#define DEFINED_ZONE_NAME      NAMESPACE_COMPUTE_CPU
+#if defined(ZONE_cpu)
+#define DEFINED_ZONE_NAME      NAMESPACE_CPU
 #elif defined(ZONE_avx512)
-#define DEFINED_ZONE_NAME      NAMESPACE_COMPUTE_AVX512
+#define DEFINED_ZONE_NAME      NAMESPACE_AVX512
 #elif defined(ZONE_cuda)
-#define DEFINED_ZONE_NAME      NAMESPACE_COMPUTE_CUDA
+#define DEFINED_ZONE_NAME      NAMESPACE_CUDA
 #elif defined(ZONE_no_cuda)
-#define DEFINED_ZONE_NAME      NAMESPACE_COMPUTE_NO_CUDA
-#elif defined(ZONE_R)
-#define DEFINED_ZONE_NAME      NAMESPACE_R
+#define DEFINED_ZONE_NAME      NAMESPACE_NO_CUDA
 #else
 #error ZONE not recognized
 #endif
 
 // we need to nest twice to get the defined value into the token pasted operation:
 // https://stackoverflow.com/questions/1597007/creating-c-macro-with-and-line-token-concatenation-with-positioning-macr
 #define MAKE_ZONED_C_FUNCTION_NAME_INTERNAL1(__zone_name, __function_name) __zone_name ## _ ## __function_name
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/Bin.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/bridge_cpp/Bin.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/GradientPair.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/bridge_cpp/GradientPair.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/bridge_cpp/bridge_cpp.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/bridge_cpp/bridge_cpp.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/common_c/common_c.c` & `interpret-core-0.4.2/symbolic/shared/libebm/common_c/common_c.c`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/common_c/common_c.h` & `interpret-core-0.4.2/symbolic/shared/libebm/common_c/common_c.h`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/common_c/logging.c` & `interpret-core-0.4.2/symbolic/shared/libebm/common_c/logging.c`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/common_c/logging.h` & `interpret-core-0.4.2/symbolic/shared/libebm/common_c/logging.h`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/common_cpp/common_cpp.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/common_cpp/common_cpp.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/Directory.Build.targets` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/Directory.Build.targets`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/Objective.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/Objective.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,21 @@
       pObjectiveWrapperOut->m_pFunctionPointersCpp = pFunctionPointersCpp;
       try {
          const std::vector<std::shared_ptr<const Registration>> registrations = (*registerObjectivesFunction)();
          const bool bFailed = Registration::CreateRegistrable(pConfig, sObjective, sObjectiveEnd, pObjectiveWrapperOut, registrations);
          if(!bFailed) {
             EBM_ASSERT(nullptr != pObjectiveWrapperOut->m_pObjective);
             pObjectiveWrapperOut->m_pApplyUpdateC = MAKE_ZONED_C_FUNCTION_NAME(ApplyUpdate);
-#if defined(ZONE_cpu) || defined(ZONE_R)
+#ifdef ZONE_cpu
             pObjectiveWrapperOut->m_pFinishMetricC = MAKE_ZONED_C_FUNCTION_NAME(FinishMetric);
             pObjectiveWrapperOut->m_pCheckTargetsC = MAKE_ZONED_C_FUNCTION_NAME(CheckTargets);
-#else // ZONE_cpu || ZONE_R
+#else // ZONE_cpu
             pObjectiveWrapperOut->m_pFinishMetricC = nullptr;
             pObjectiveWrapperOut->m_pCheckTargetsC = nullptr;
-#endif // ZONE_cpu || ZONE_R
+#endif // ZONE_cpu
 
             LOG_0(Trace_Info, "Exited Objective::CreateObjective");
             return Error_None;
          }
          EBM_ASSERT(nullptr == pObjectiveWrapperOut->m_pObjective);
          LOG_0(Trace_Info, "Exited Objective::CreateObjective unknown objective");
          error = Error_ObjectiveUnknown;
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/Objective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/Objective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/Registration.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/Registration.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/Registration.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/Registration.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/approximate_math.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/approximate_math.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/avx512_ebm/avx512_ebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/compute.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/compute.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/compute_stats.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/compute_stats.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_64.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/cpu_64.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj.filters` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/cpu_ebm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/cpu_ebm/sse2_32.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/cpu_ebm/sse2_32.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_32.cu` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/cuda_ebm/cuda_32.cu`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/cuda_ebm/cuda_ebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_32.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_32.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/no_cuda_ebm/no_cuda_ebm.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassMultitaskObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/CrossEntropyMulticlassMultitaskObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/ExampleRegressionObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/ExampleRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/GammaDevianceRegressionObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/GammaDevianceRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossBinaryMultitaskObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/LogLossBinaryMultitaskObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossBinaryObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/LogLossBinaryObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/LogLossMulticlassObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/LogLossMulticlassObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/PoissonDevianceRegressionObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/PoissonDevianceRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/PseudoHuberRegressionObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/PseudoHuberRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseLogLinkRegressionObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/RmseLogLinkRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/RmseRegressionObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/RmseRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/TweedieDevianceRegressionObjective.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/TweedieDevianceRegressionObjective.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/objectives/objective_registrations.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/objectives/objective_registrations.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/registration_exceptions.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/registration_exceptions.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_c_functions.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/zoned_bridge_c_functions.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ) {
    const Objective * const pObjective = static_cast<const Objective *>(pObjectiveWrapper->m_pObjective);
    const APPLY_UPDATE_CPP pApplyUpdateCpp = 
       (static_cast<FunctionPointersCpp *>(pObjectiveWrapper->m_pFunctionPointersCpp))->m_pApplyUpdateCpp;
    return (*pApplyUpdateCpp)(pObjective, pData);
 }
 
-#if defined(ZONE_cpu) || defined(ZONE_R)
+#ifdef ZONE_cpu
 INTERNAL_IMPORT_EXPORT_BODY double MAKE_ZONED_C_FUNCTION_NAME(FinishMetric) (
    const ObjectiveWrapper * const pObjectiveWrapper,
    const double metricSum
 ) {
    const Objective * const pObjective = static_cast<const Objective *>(pObjectiveWrapper->m_pObjective);
    const FINISH_METRIC_CPP pFinishMetricCpp =
       (static_cast<const FunctionPointersCpp *>(pObjectiveWrapper->m_pFunctionPointersCpp))->m_pFinishMetricCpp;
@@ -52,10 +52,10 @@
    const void * const aTargets
 ) {
    const Objective * const pObjective = static_cast<const Objective *>(pObjectiveWrapper->m_pObjective);
    const CHECK_TARGETS_CPP pCheckTargetsCpp =
       (static_cast<const FunctionPointersCpp *>(pObjectiveWrapper->m_pFunctionPointersCpp))->m_pCheckTargetsCpp;
    return (*pCheckTargetsCpp)(pObjective, c, aTargets);
 }
-#endif // ZONE_cpu || ZONE_R
+#endif // ZONE_cpu
 
 } // DEFINED_ZONE_NAME
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_c_functions.h` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/zoned_bridge_c_functions.h`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 #endif // __cplusplus
 
 INTERNAL_IMPORT_EXPORT_INCLUDE ErrorEbm MAKE_ZONED_C_FUNCTION_NAME(ApplyUpdate)(
    const ObjectiveWrapper * const pObjectiveWrapper,
    ApplyUpdateBridge * const pData
 );
 
-#if defined(ZONE_cpu) || defined(ZONE_R)
+#ifdef ZONE_cpu
 INTERNAL_IMPORT_EXPORT_INCLUDE double MAKE_ZONED_C_FUNCTION_NAME(FinishMetric) (
    const ObjectiveWrapper * const pObjectiveWrapper,
    const double metricSum
 );
 INTERNAL_IMPORT_EXPORT_INCLUDE BoolEbm MAKE_ZONED_C_FUNCTION_NAME(CheckTargets) (
    const ObjectiveWrapper * const pObjectiveWrapper,
    const size_t c, 
    const void * const aTargets
 );
-#endif // ZONE_cpu || ZONE_R
+#endif // ZONE_cpu
 
 
 #ifdef __cplusplus
 }
 #endif // __cplusplus
 
 #endif // ZONED_BRIDGE_C_FUNCTIONS_H
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute/zoned_bridge_cpp_functions.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute/zoned_bridge_cpp_functions.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/compute_accessors.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/compute_accessors.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/dataset_shared.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/dataset_shared.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1021,26 +1021,31 @@
       countSamples,
       static_cast<const void *>(binIndexes),
       cBytesAllocated,
       static_cast<void *>(pFillMem)
    );
 
    {
+      if(countBins <= IntEbm { 1 }) {
+         LOG_0(Trace_Error, "ERROR AppendFeature countBins must be 2 or larger");
+         goto return_bad;
+      }
       // we do not need to access memory based on the value of countBins, so we do not need to check if fits into size_t
       if(IsConvertError<SharedStorageDataType>(countBins)) {
          LOG_0(Trace_Error, "ERROR AppendFeature countBins is outside the range of a valid index");
          goto return_bad;
       }
-      const SharedStorageDataType cBins = static_cast<SharedStorageDataType>(countBins);
+      SharedStorageDataType cBins = static_cast<SharedStorageDataType>(countBins);
+      cBins -= EBM_FALSE != isMissing ? SharedStorageDataType { 0 } : SharedStorageDataType { 1 };
+      cBins -= EBM_FALSE != isUnknown ? SharedStorageDataType { 0 } : SharedStorageDataType { 1 };
 
       if(EBM_FALSE != isMissing && EBM_TRUE != isMissing) {
          LOG_0(Trace_Error, "ERROR AppendFeature isMissing is not EBM_FALSE or EBM_TRUE");
          goto return_bad;
       }
-
       if(EBM_FALSE != isUnknown && EBM_TRUE != isUnknown) {
          LOG_0(Trace_Error, "ERROR AppendFeature isUnknown is not EBM_FALSE or EBM_TRUE");
          goto return_bad;
       }
       if(EBM_FALSE != isNominal && EBM_TRUE != isNominal) {
          LOG_0(Trace_Error, "ERROR AppendFeature isNominal is not EBM_FALSE or EBM_TRUE");
          goto return_bad;
@@ -1152,25 +1157,34 @@
             }
             const IntEbm * pBinIndex = binIndexes;
             const IntEbm * const pBinIndexsEnd = binIndexes + cSamples;
             SharedStorageDataType * pFillData = reinterpret_cast<SharedStorageDataType *>(pFillMem + iByteCur);
 
             ptrdiff_t cShift = static_cast<ptrdiff_t>((cSamples - size_t { 1 }) % cItemsPerBitPack * cBitsPerItemMax);
             const ptrdiff_t cShiftReset = static_cast<ptrdiff_t>((cItemsPerBitPack - size_t { 1 }) * cBitsPerItemMax);
+            const IntEbm indexBinIllegal = countBins - (EBM_FALSE != isUnknown ? IntEbm { 0 } : IntEbm { 1 });
             do {
                SharedStorageDataType bits = 0;
                do {
-                  const IntEbm indexBin = *pBinIndex;
-                  if(indexBin < IntEbm { 0 }) {
-                     LOG_0(Trace_Error, "ERROR AppendFeature indexBin can't be negative");
+                  IntEbm indexBin = *pBinIndex;
+                  if(indexBinIllegal <= indexBin) {
+                     LOG_0(Trace_Error, "ERROR AppendFeature indexBinIllegal <= indexBin");
                      goto return_bad;
                   }
-                  if(countBins <= indexBin) {
-                     LOG_0(Trace_Error, "ERROR AppendFeature countBins <= indexBin");
-                     goto return_bad;
+                  if(EBM_FALSE != isMissing) {
+                     if(indexBin < IntEbm { 0 }) {
+                        LOG_0(Trace_Error, "ERROR AppendFeature indexBin can't be negative");
+                        goto return_bad;
+                     }
+                  } else {
+                     if(indexBin <= IntEbm { 0 }) {
+                        LOG_0(Trace_Error, "ERROR AppendFeature indexBin <= IntEbm { 0 }");
+                        goto return_bad;
+                     }
+                     --indexBin;
                   }
                   ++pBinIndex;
 
                   // since countBins can be converted to these, so now can indexBin
                   EBM_ASSERT(!IsConvertError<SharedStorageDataType>(indexBin));
 
                   EBM_ASSERT(0 <= cShift);
@@ -2106,15 +2120,18 @@
          const size_t iOffsetCur = static_cast<size_t>(indexOffsetCur);
 
          const FeatureDataSetShared * pFeatureDataSetShared =
             reinterpret_cast<const FeatureDataSetShared *>(static_cast<const char *>(dataSet) + iOffsetCur);
 
          EBM_ASSERT(IsFeature(pFeatureDataSetShared->m_id));
 
-         const SharedStorageDataType countBins = pFeatureDataSetShared->m_cBins;
+         SharedStorageDataType countBins = pFeatureDataSetShared->m_cBins;
+         // countBins originally fit into SharedStorageDataType so it should still with these additions
+         countBins += IsMissingFeature(pFeatureDataSetShared->m_id) ? SharedStorageDataType { 0 } : SharedStorageDataType { 1 };
+         countBins += IsUnknownFeature(pFeatureDataSetShared->m_id) ? SharedStorageDataType { 0 } : SharedStorageDataType { 1 };
          if(IsConvertError<IntEbm>(countBins)) {
             LOG_0(Trace_Error, "ERROR ExtractBinCounts IsConvertError<IntEbm>(countBins)");
             return Error_IllegalParamVal;
          }
 
          *pcBins = static_cast<IntEbm>(countBins);
          ++pcBins;
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/dataset_shared.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/dataset_shared.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/debug_ebm.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/debug_ebm.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -17,28 +17,170 @@
 
 #include "libebm.h"
 #include "logging.h"
 #include "zones.h"
 
 //#include "approximate_math.hpp"
 
+#include "Feature.hpp"
+#include "Term.hpp"
+#include "Transpose.hpp"
+
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
 #error DEFINED_ZONE_NAME must be defined
 #endif // DEFINED_ZONE_NAME
 
+
 //#define INCLUDE_TESTS_IN_RELEASE
+//#define ENABLE_TRANSPOSE
 //#define ENABLE_TEST_LOG_SUM_ERRORS
 //#define ENABLE_TEST_EXP_SUM_ERRORS
 //#define ENABLE_TEST_SOFTMAX_SUM_ERRORS
 //#define ENABLE_PRINTF
 
 #if !defined(NDEBUG) || defined(INCLUDE_TESTS_IN_RELEASE)
 
 
+
+#ifdef ENABLE_TRANSPOSE
+static double TestTranspose() {
+   double debugRet = 0; // this just prevents the optimizer from eliminating this code
+
+   std::mt19937 testRandom(52);
+   std::uniform_int_distribution<> dimensionsDistributions(1, 5);
+
+   FeatureBoosting features[5];
+   Term term;
+
+   double original[20000];
+   double transposed[20000];
+   double restored[20000];
+
+   for(int iTest = 0; iTest < 100000; ++iTest) {
+      const int cDimensions = dimensionsDistributions(testRandom);
+
+      debugRet += cDimensions; // just to ensure this code gets run
+
+      term.Initialize(cDimensions);
+      term.SetCountRealDimensions(cDimensions);
+
+      TermFeature * aTermFeatures = term.GetTermFeatures();
+      size_t cTensorBins = 1;
+      for(int iDimension = 0; iDimension < cDimensions; ++iDimension) {
+         aTermFeatures[iDimension].m_iTranspose = iDimension;
+         aTermFeatures[iDimension].m_pFeature = &features[iDimension];
+         aTermFeatures[iDimension].m_cStride = cTensorBins;
+
+         int cBins;
+         bool bMissing;
+         bool bUnknown;
+         int cExpandedBins;
+         do {
+            cBins = dimensionsDistributions(testRandom);
+            bMissing = 4 <= dimensionsDistributions(testRandom);
+            bUnknown = 4 <= dimensionsDistributions(testRandom);
+            cExpandedBins = cBins + (bMissing ? 0 : 1) + (bUnknown ? 0 : 1);
+         } while(cExpandedBins < 2);
+
+         features[iDimension].Initialize(cBins, bMissing, bUnknown, EBM_FALSE);
+
+         cTensorBins *= cBins;
+      }
+
+      for(int iDimension = 0; iDimension < cDimensions; ++iDimension) {
+         std::uniform_int_distribution<> shuffleDistribution(iDimension, cDimensions - 1);
+         int iShuffle = shuffleDistribution(testRandom);
+         size_t temp = aTermFeatures[iShuffle].m_iTranspose;
+         aTermFeatures[iShuffle].m_iTranspose = aTermFeatures[iDimension].m_iTranspose;
+         aTermFeatures[iDimension].m_iTranspose = temp;
+      }
+
+      for(int i = 0; i < 20000; ++i) {
+         original[i] = i;
+      }
+
+      Transpose<false>(&term, 1, original, transposed);
+      Transpose<true>(&term, 1, restored, transposed);
+
+      size_t indexIncrement[5];
+      indexIncrement[0] = 0;
+      indexIncrement[1] = 0;
+      indexIncrement[2] = 0;
+      indexIncrement[3] = 0;
+      indexIncrement[4] = 0;
+      size_t indexCorrected[5];
+
+      while(true) {
+         for(int iDimension = 0; iDimension < cDimensions; ++iDimension) {
+            const FeatureBoosting * pFeature = aTermFeatures[aTermFeatures[iDimension].m_iTranspose].m_pFeature;
+            bool bMissing = pFeature->IsMissing();
+            bool bUnknown = pFeature->IsUnknown();
+            size_t cBins = pFeature->GetCountBins();
+            cBins = cBins + (bMissing ? 0 : 1) + (bUnknown ? 0 : 1);
+            size_t i = indexIncrement[iDimension];
+
+            if(i == cBins - 1 && !bUnknown) {
+               --i;
+            }
+            if(i == 0 && !bMissing) {
+               ++i;
+            }
+
+            indexCorrected[iDimension] = i;
+         }
+
+         cTensorBins = 1;
+         size_t iFlatIncrement = 0;
+         size_t iFlatCorrected = 0;
+         for(int iDimension = 0; iDimension < cDimensions; ++iDimension) {
+            const FeatureBoosting * pFeature = aTermFeatures[aTermFeatures[iDimension].m_iTranspose].m_pFeature;
+            bool bMissing = pFeature->IsMissing();
+            bool bUnknown = pFeature->IsUnknown();
+            size_t cBins = pFeature->GetCountBins();
+            cBins = cBins + (bMissing ? 0 : 1) + (bUnknown ? 0 : 1);
+
+            iFlatIncrement += indexIncrement[iDimension] * cTensorBins;
+            iFlatCorrected += indexCorrected[iDimension] * cTensorBins;
+
+            cTensorBins *= cBins;
+         }
+
+         EBM_ASSERT(original[iFlatCorrected] == restored[iFlatIncrement]);
+
+         int iDimension;
+         for(iDimension = 0; iDimension < cDimensions; ++iDimension) {
+            const FeatureBoosting * pFeature = aTermFeatures[aTermFeatures[iDimension].m_iTranspose].m_pFeature;
+            bool bMissing = pFeature->IsMissing();
+            bool bUnknown = pFeature->IsUnknown();
+            size_t cBins = pFeature->GetCountBins();
+            cBins = cBins + (bMissing ? 0 : 1) + (bUnknown ? 0 : 1);
+            size_t i = indexIncrement[iDimension];
+            ++i;
+            indexIncrement[iDimension] = i;
+            if(i != cBins) {
+               break;
+            }
+            indexIncrement[iDimension] = 0;
+         }
+
+         if(iDimension == cDimensions) {
+            break;
+         }
+      }
+   }
+
+   return debugRet;
+}
+
+// this is just to prevent the compiler for optimizing our code away on release
+extern double g_TestTranspose = TestTranspose();
+#endif
+
+
 #ifdef ENABLE_TEST_LOG_SUM_ERRORS
 static double TestLogSumErrors() {
    double debugRet = 0; // this just prevents the optimizer from eliminating this code
 
    // check that our outputs match that of the std::log function
    EBM_ASSERT(std::isnan(std::log(std::numeric_limits<float>::quiet_NaN())));
    EBM_ASSERT(std::isnan(std::log(-std::numeric_limits<float>::infinity())));
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/ebm_internal.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/ebm_internal.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/ebm_stats.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/ebm_stats.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/inc/libebm.h` & `interpret-core-0.4.2/symbolic/shared/libebm/inc/libebm.h`

 * *Files 0% similar despite different names*

```diff
@@ -443,15 +443,15 @@
    double * avgGainOut
 );
 // GetTermUpdateSplits must be called before calls to GetTermUpdate/SetTermUpdate
 EBM_API_INCLUDE ErrorEbm EBM_CALLING_CONVENTION GetTermUpdateSplits(
    BoosterHandle boosterHandle,
    IntEbm indexDimension,
    IntEbm * countSplitsInOut,
-   IntEbm * splitIndexesOut
+   IntEbm * splitsOut
 );
 EBM_API_INCLUDE ErrorEbm EBM_CALLING_CONVENTION GetTermUpdate(
    BoosterHandle boosterHandle,
    double * updateScoresTensorOut
 );
 EBM_API_INCLUDE ErrorEbm EBM_CALLING_CONVENTION SetTermUpdate(
    BoosterHandle boosterHandle,
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/include_ordering.txt` & `interpret-core-0.4.2/symbolic/shared/libebm/include_ordering.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 
 // main side include files
 #include "compute_accessors.hpp"
 #include "ebm_internal.hpp" // GENERAL include file in the non-compute zones.  Almost all the below depend on it
 #include "RandomDeterministic.hpp"
 #include "RandomNondeterministic.hpp"
 #include "GaussianDistribution.hpp" // implicitly depends on RandomDeterministic.hpp and RandomNondeterministic.hpp but the dependency is templated away
-#include "Transpose.hpp"
 #include "approximate_math.hpp"
 #include "ebm_stats.hpp" // depends on approximate_math.hpp
 #include "Feature.hpp" // ONLY zones.h
 #include "Term.hpp" // ONLY zones.h and Feature.hpp
+#include "Transpose.hpp"
 #include "dataset_shared.hpp"
 #include "DataSetBoosting.hpp" // depends on dataset_shared.hpp, Feature.hpp, Term.hpp
 #include "DataSetInteraction.hpp" // depends on dataset_shared.hpp
 #include "InnerBag.hpp" // depends on RandomDeterministic.hpp
 #include "Tensor.hpp" // depends on Term.hpp and Feature.hpp
 #include "GradientPair.hpp"
 #include "Bin.hpp" // depends on GradientPair.hpp
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/interpret.sln` & `interpret-core-0.4.2/symbolic/shared/libebm/interpret.sln`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/interpretable_numerics.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/interpretable_numerics.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj` & `interpret-core-0.4.2/symbolic/shared/libebm/libebm.vcxproj`

 * *Files 0% similar despite different names*

#### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj` & `interpret-core-0.4.2/symbolic/shared/libebm/libebm.vcxproj`

```diff
@@ -94,15 +94,15 @@
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
       <PrecompiledHeader>Use</PrecompiledHeader>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
       <SDLCheck>true</SDLCheck>
-      <PreprocessorDefinitions>ZONE_main;LIBEBM_EXPORTS;_WINDOWS;_USRDLL;_DEBUG;WIN32;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>ZONE_cpu;LIBEBM_EXPORTS;_WINDOWS;_USRDLL;_DEBUG;WIN32;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <ConformanceMode>true</ConformanceMode>
       <PrecompiledHeaderFile>precompiled_header_cpp.hpp</PrecompiledHeaderFile>
       <AdditionalIncludeDirectories>$(ProjectDir)inc;$(ProjectDir)common_c;$(ProjectDir)bridge_c;$(ProjectDir)common_cpp;$(ProjectDir)bridge_cpp;$(ProjectDir);</AdditionalIncludeDirectories>
       <InlineFunctionExpansion>AnySuitable</InlineFunctionExpansion>
       <RuntimeLibrary>MultiThreadedDebug</RuntimeLibrary>
       <StringPooling>true</StringPooling>
       <ControlFlowGuard>Guard</ControlFlowGuard>
@@ -139,15 +139,15 @@
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
       <PrecompiledHeader>Use</PrecompiledHeader>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
       <SDLCheck>true</SDLCheck>
-      <PreprocessorDefinitions>ZONE_main;LIBEBM_EXPORTS;_WINDOWS;_USRDLL;_DEBUG;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>ZONE_cpu;LIBEBM_EXPORTS;_WINDOWS;_USRDLL;_DEBUG;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <ConformanceMode>true</ConformanceMode>
       <PrecompiledHeaderFile>precompiled_header_cpp.hpp</PrecompiledHeaderFile>
       <AdditionalIncludeDirectories>$(ProjectDir)inc;$(ProjectDir)common_c;$(ProjectDir)bridge_c;$(ProjectDir)common_cpp;$(ProjectDir)bridge_cpp;$(ProjectDir);</AdditionalIncludeDirectories>
       <InlineFunctionExpansion>AnySuitable</InlineFunctionExpansion>
       <RuntimeLibrary>MultiThreadedDebug</RuntimeLibrary>
       <OmitFramePointers>false</OmitFramePointers>
       <StringPooling>true</StringPooling>
@@ -186,15 +186,15 @@
     <ClCompile>
       <PrecompiledHeader>Use</PrecompiledHeader>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
       <SDLCheck>false</SDLCheck>
-      <PreprocessorDefinitions>ZONE_main;LIBEBM_EXPORTS;_WINDOWS;_USRDLL;NDEBUG;WIN32;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>ZONE_cpu;LIBEBM_EXPORTS;_WINDOWS;_USRDLL;NDEBUG;WIN32;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <ConformanceMode>true</ConformanceMode>
       <PrecompiledHeaderFile>precompiled_header_cpp.hpp</PrecompiledHeaderFile>
       <AdditionalIncludeDirectories>$(ProjectDir)inc;$(ProjectDir)common_c;$(ProjectDir)bridge_c;$(ProjectDir)common_cpp;$(ProjectDir)bridge_cpp;$(ProjectDir);</AdditionalIncludeDirectories>
       <InlineFunctionExpansion>AnySuitable</InlineFunctionExpansion>
       <FavorSizeOrSpeed>Speed</FavorSizeOrSpeed>
       <RuntimeLibrary>MultiThreaded</RuntimeLibrary>
       <OmitFramePointers>true</OmitFramePointers>
@@ -236,15 +236,15 @@
     <ClCompile>
       <PrecompiledHeader>Use</PrecompiledHeader>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
       <SDLCheck>false</SDLCheck>
-      <PreprocessorDefinitions>ZONE_main;LIBEBM_EXPORTS;_WINDOWS;_USRDLL;NDEBUG;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>ZONE_cpu;LIBEBM_EXPORTS;_WINDOWS;_USRDLL;NDEBUG;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <ConformanceMode>true</ConformanceMode>
       <PrecompiledHeaderFile>precompiled_header_cpp.hpp</PrecompiledHeaderFile>
       <AdditionalIncludeDirectories>$(ProjectDir)inc;$(ProjectDir)common_c;$(ProjectDir)bridge_c;$(ProjectDir)common_cpp;$(ProjectDir)bridge_cpp;$(ProjectDir);</AdditionalIncludeDirectories>
       <InlineFunctionExpansion>AnySuitable</InlineFunctionExpansion>
       <FavorSizeOrSpeed>Speed</FavorSizeOrSpeed>
       <RuntimeLibrary>MultiThreaded</RuntimeLibrary>
       <OmitFramePointers>true</OmitFramePointers>
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/libebm.vcxproj.filters` & `interpret-core-0.4.2/symbolic/shared/libebm/libebm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/libebm_exports.def` & `interpret-core-0.4.2/symbolic/shared/libebm/libebm_exports.def`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/libebm_exports.txt` & `interpret-core-0.4.2/symbolic/shared/libebm/libebm_exports.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/precompiled_header_cpp.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/precompiled_header_cpp.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/random.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/random.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/sampling.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/sampling.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,22 @@
 #include "dataset_shared.hpp" // GetDataSetSharedWeight
 
 namespace DEFINED_ZONE_NAME {
 #ifndef DEFINED_ZONE_NAME
 #error DEFINED_ZONE_NAME must be defined
 #endif // DEFINED_ZONE_NAME
 
-// we don't care if an extra log message is outputted due to the non-atomic nature of the decrement to this value
-static int g_cLogEnterSampleWithoutReplacement = 5;
-static int g_cLogExitSampleWithoutReplacement = 5;
-
 EBM_API_BODY ErrorEbm EBM_CALLING_CONVENTION SampleWithoutReplacement(
    void * rng,
    IntEbm countTrainingSamples,
    IntEbm countValidationSamples,
    BagEbm * bagOut
 ) {
-   LOG_COUNTED_N(
-      &g_cLogEnterSampleWithoutReplacement,
+   LOG_N(
       Trace_Info,
-      Trace_Verbose,
       "Entered SampleWithoutReplacement: "
       "rng=%p, "
       "countTrainingSamples=%" IntEbmPrintf ", "
       "countValidationSamples=%" IntEbmPrintf ", "
       "bagOut=%p"
       ,
       rng,
@@ -58,20 +52,15 @@
 
    if(UNLIKELY(IsAddError(cTrainingSamples, cValidationSamples))) {
       LOG_0(Trace_Error, "ERROR SampleWithoutReplacement IsAddError(cTrainingSamples, cValidationSamples)");
       return Error_IllegalParamVal;
    }
    size_t cSamplesRemaining = cTrainingSamples + cValidationSamples;
    if(UNLIKELY(size_t { 0 } == cSamplesRemaining)) {
-      LOG_COUNTED_0(
-         &g_cLogExitSampleWithoutReplacement,
-         Trace_Info,
-         Trace_Verbose,
-         "Exited SampleWithoutReplacement with zero elements"
-      );
+      LOG_0(Trace_Info, "Exited SampleWithoutReplacement with zero elements");
       return Error_None;
    }
    if(UNLIKELY(IsMultiplyError(sizeof(*bagOut), cSamplesRemaining))) {
       LOG_0(Trace_Error, "ERROR SampleWithoutReplacement IsMultiplyError(sizeof(*bagOut), cSamplesRemaining)");
       return Error_IllegalParamVal;
    }
 
@@ -114,45 +103,33 @@
       } catch(...) {
          LOG_0(Trace_Warning, "WARNING SampleWithoutReplacement Unknown error in std::random_device");
          return Error_UnexpectedInternal;
       }
    }
    EBM_ASSERT(0 == cTrainingRemaining); // this should be all used up too now
 
-   LOG_COUNTED_0(
-      &g_cLogExitSampleWithoutReplacement,
-      Trace_Info,
-      Trace_Verbose,
-      "Exited SampleWithoutReplacement"
-   );
+   LOG_0(Trace_Info, "Exited SampleWithoutReplacement");
    return Error_None;
 }
 
-
-static int g_cLogEnterSampleWithoutReplacementStratified = 5;
-static int g_cLogExitSampleWithoutReplacementStratified = 5;
-
-
 EBM_API_BODY ErrorEbm EBM_CALLING_CONVENTION SampleWithoutReplacementStratified(
    void * rng,
    IntEbm countClasses,
    IntEbm countTrainingSamples,
    IntEbm countValidationSamples,
    const IntEbm * targets,
    BagEbm * bagOut
 ) {
    struct TargetClass {
       size_t m_cTrainingSamples;
       size_t m_cSamples;
    };
 
-   LOG_COUNTED_N(
-      &g_cLogEnterSampleWithoutReplacementStratified,
+   LOG_N(
       Trace_Info,
-      Trace_Verbose,
       "Entered SampleWithoutReplacementStratified: "
       "rng=%p, "
       "countClasses=%" IntEbmPrintf ", "
       "countTrainingSamples=%" IntEbmPrintf ", "
       "countValidationSamples=%" IntEbmPrintf ", "
       "targets=%p, "
       "bagOut=%p"
@@ -180,20 +157,15 @@
    if(UNLIKELY(IsAddError(cTrainingSamples, cValidationSamples))) {
       LOG_0(Trace_Error, "ERROR SampleWithoutReplacementStratified IsAddError(countTrainingSamples, countValidationSamples))");
       return Error_IllegalParamVal;
    }
 
    const size_t cSamples = cTrainingSamples + cValidationSamples;
    if(UNLIKELY(size_t { 0 } == cSamples)) {
-      LOG_COUNTED_0(
-         &g_cLogExitSampleWithoutReplacementStratified,
-         Trace_Info,
-         Trace_Verbose,
-         "Exited SampleWithoutReplacementStratified with zero samples"
-      );
+      LOG_0(Trace_Info, "Exited SampleWithoutReplacementStratified with zero samples");
       return Error_None;
    }
 
    if(UNLIKELY(IsMultiplyError(EbmMax(sizeof(*targets), sizeof(*bagOut)), cSamples))) {
       LOG_0(Trace_Error, "ERROR SampleWithoutReplacementStratified IsMultiplyError(EbmMax(sizeof(*targets), sizeof(*bagOut)), cSamples)");
       return Error_IllegalParamVal;
    }
@@ -445,20 +417,15 @@
       EBM_ASSERT(0 == aTargetClasses[iClassDebug].m_cSamples);
    }
 #endif
 
    free(aTargetClasses);
    free(apMostImprovedClasses);
 
-   LOG_COUNTED_0(
-      &g_cLogExitSampleWithoutReplacementStratified,
-      Trace_Info,
-      Trace_Verbose,
-      "Exited SampleWithoutReplacementStratified"
-   );
+   LOG_0(Trace_Info, "Exited SampleWithoutReplacementStratified");
 
    return Error_None;
 }
 
 extern ErrorEbm Unbag(
    const size_t cSamples,
    const BagEbm * const aBag,
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/special/linux_wrap_functions.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/special/linux_wrap_functions.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/special/windows_DllMain.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/special/windows_DllMain.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/CutQuantileTest.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/CutQuantileTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/CutUniformTest.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/CutUniformTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/CutWinsorizedTest.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/CutWinsorizedTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/DiscretizeTest.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/DiscretizeTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/RandomStreamTest.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/RandomStreamTest.hpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/SuggestGraphBoundsTest.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/SuggestGraphBoundsTest.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/bit_packing_extremes.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/bit_packing_extremes.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,17 @@
       // if we set the number of bins to be exponential, then we'll be just under a bit packing boundary.  4 bins means bits packs 00, 01, 10, and 11
       for(IntEbm iRange = IntEbm { -1 }; iRange <= IntEbm { 1 }; ++iRange) {
          IntEbm cBins = exponential + iRange; // check one less than the tight fit, the tight fit, and one above the tight fit
          // try everything from 0 samples to 65 samples because for bitpacks with 1 bit, we can have up to 64 packed into a single data value on a 
          // 64 bit machine
          for(size_t cSamples = 1; cSamples < 66; ++cSamples) {
             TestApi test = TestApi(OutputType_Regression);
-            test.AddFeatures({ FeatureTest(cBins) });
+            // add one to the bins because our interface needs missing and unknown bins but 
+            // internally drop the unknown bin to make it possible to have 1 bin
+            test.AddFeatures({ FeatureTest(cBins + 1, true, false) });
             test.AddTerms({ { 0 } });
 
             std::vector<TestSample> trainingSamples;
             std::vector<TestSample> validationSamples;
             for(size_t iSample = 0; iSample < cSamples; ++iSample) {
                trainingSamples.push_back(TestSample({ cBins - 1 }, 7));
                validationSamples.push_back(TestSample({ cBins - 1 }, 8));
@@ -47,15 +49,17 @@
       // if we set the number of bins to be exponential, then we'll be just under a bit packing boundary.  4 bins means bits packs 00, 01, 10, and 11
       for(IntEbm iRange = IntEbm { -1 }; iRange <= IntEbm { 1 }; ++iRange) {
          IntEbm cBins = exponential + iRange; // check one less than the tight fit, the tight fit, and one above the tight fit
          // try everything from 0 samples to 65 samples because for bitpacks with 1 bit, we can have up to 64 packed into a single data value on 
          // a 64 bit machine
          for(size_t cSamples = 1; cSamples < 66; ++cSamples) {
             TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
-            test.AddFeatures({ FeatureTest(cBins) });
+            // add one to the bins because our interface needs missing and unknown bins but 
+            // internally drop the unknown bin to make it possible to have 1 bin
+            test.AddFeatures({ FeatureTest(cBins + 1, true, false) });
             test.AddTerms({ { 0 } });
 
             std::vector<TestSample> trainingSamples;
             std::vector<TestSample> validationSamples;
             for(size_t iSample = 0; iSample < cSamples; ++iSample) {
                trainingSamples.push_back(TestSample({ cBins - 1 }, 0));
                validationSamples.push_back(TestSample({ cBins - 1 }, 1));
@@ -83,15 +87,17 @@
       // if we set the number of bins to be exponential, then we'll be just under a bit packing boundary.  4 bins means bits packs 00, 01, 10, and 11
       for(IntEbm iRange = IntEbm { -1 }; iRange <= IntEbm { 1 }; ++iRange) {
          IntEbm cBins = exponential + iRange; // check one less than the tight fit, the tight fit, and one above the tight fit
          // try everything from 0 samples to 65 samples because for bitpacks with 1 bit, we can have up to 64 packed into a single data value on 
          // a 64 bit machine
          for(size_t cSamples = 1; cSamples < 66; ++cSamples) {
             TestApi test = TestApi(OutputType_Regression);
-            test.AddFeatures({ FeatureTest(2), FeatureTest(cBins) });
+            // add one to the bins because our interface needs missing and unknown bins but 
+            // internally drop the unknown bin to make it possible to have 1 bin
+            test.AddFeatures({ FeatureTest(2), FeatureTest(cBins + 1, true, false) });
 
             std::vector<TestSample> samples;
             for(size_t iSample = 0; iSample < cSamples; ++iSample) {
                samples.push_back(TestSample({ 0, cBins - 1 }, 7));
             }
             test.AddInteractionSamples(samples);
             test.InitializeInteraction();
@@ -109,15 +115,17 @@
       // if we set the number of bins to be exponential, then we'll be just under a bit packing boundary.  4 bins means bits packs 00, 01, 10, and 11
       for(IntEbm iRange = IntEbm { -1 }; iRange <= IntEbm { 1 }; ++iRange) {
          IntEbm cBins = exponential + iRange; // check one less than the tight fit, the tight fit, and one above the tight fit
          // try everything from 0 samples to 65 samples because for bitpacks with 1 bit, we can have up to 64 packed into a single data value on 
          // a 64 bit machine
          for(size_t cSamples = 1; cSamples < 66; ++cSamples) {
             TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
-            test.AddFeatures({ FeatureTest(2), FeatureTest(cBins) });
+            // add one to the bins because our interface needs missing and unknown bins but 
+            // internally drop the unknown bin to make it possible to have 1 bin
+            test.AddFeatures({ FeatureTest(2), FeatureTest(cBins + 1, true, false) });
 
             std::vector<TestSample> samples;
             for(size_t iSample = 0; iSample < cSamples; ++iSample) {
                samples.push_back(TestSample({ 0, cBins - 1 }, 1));
             }
             test.AddInteractionSamples(samples);
             test.InitializeInteraction();
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/boosting_unusual_inputs.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/boosting_unusual_inputs.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -775,18 +775,20 @@
       CHECK_APPROX(termScore, test.GetBestTermScore(0, { 1 }, 1));
       termScore = test.GetBestTermScore(0, { 0 }, 2);
       CHECK(0 == termScore);
       CHECK_APPROX(termScore, test.GetBestTermScore(0, { 1 }, 2));
    }
 }
 
+// TODO: reinstate this AFTER we have moved missing value handling into C++
+#ifdef NEVER
 TEST_CASE("features with 0 states, boosting") {
    // for there to be zero states, there can't be an training data or testing data since then those would be required to have a value for the state
    TestApi test = TestApi(OutputType_Regression);
-   test.AddFeatures({ FeatureTest(0) });
+   test.AddFeatures({ FeatureTest(2, false, false) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({});
    test.AddValidationSamples({});
    test.InitializeBoosting();
 
    double validationMetric = test.Boost(0).validationMetric;
    CHECK(std::numeric_limits<double>::infinity() == validationMetric);
@@ -798,44 +800,45 @@
    termScores[0] = 9.99;
    test.GetBestTermScoresRaw(0, termScores);
    CHECK(9.99 == termScores[0]); // the term is a tensor with zero values since one of the dimensions is non-existant
    termScores[0] = 9.99;
    test.GetCurrentTermScoresRaw(0, termScores);
    CHECK(9.99 == termScores[0]); // the term is a tensor with zero values since one of the dimensions is non-existant
 }
+#endif
 
 
 TEST_CASE("features with 1 state in various positions, boosting") {
    TestApi test0 = TestApi(OutputType_Regression);
    test0.AddFeatures({
-      FeatureTest(1),
+      FeatureTest(2, true, false),
       FeatureTest(2),
       FeatureTest(2)
       });
    test0.AddTerms({ { 0 }, { 1 }, { 2 } });
    test0.AddTrainingSamples({ TestSample({ 0, 1, 1 }, 10) });
    test0.AddValidationSamples({ TestSample({ 0, 1, 1 }, 12) });
    test0.InitializeBoosting();
 
    TestApi test1 = TestApi(OutputType_Regression);
    test1.AddFeatures({
       FeatureTest(2),
-      FeatureTest(1),
+      FeatureTest(2, true, false),
       FeatureTest(2)
       });
    test1.AddTerms({ { 0 }, { 1 }, { 2 } });
    test1.AddTrainingSamples({ TestSample({ 1, 0, 1 }, 10) });
    test1.AddValidationSamples({ TestSample({ 1, 0, 1 }, 12) });
    test1.InitializeBoosting();
 
    TestApi test2 = TestApi(OutputType_Regression);
    test2.AddFeatures({
       FeatureTest(2),
       FeatureTest(2),
-      FeatureTest(1)
+      FeatureTest(2, true, false)
       });
    test2.AddTerms({ { 0 }, { 1 }, { 2 } });
    test2.AddTrainingSamples({ TestSample({ 1, 1, 0 }, 10) });
    test2.AddValidationSamples({ TestSample({ 1, 1, 0 }, 12) });
    test2.InitializeBoosting();
 
    for(int iEpoch = 0; iEpoch < 1000; ++iEpoch) {
@@ -1033,15 +1036,15 @@
    testZeroDimensions.AddFeatures({});
    testZeroDimensions.AddTerms({ {} });
    testZeroDimensions.AddTrainingSamples({ TestSample({}, 10) });
    testZeroDimensions.AddValidationSamples({ TestSample({}, 12) });
    testZeroDimensions.InitializeBoosting();
 
    TestApi testOneState = TestApi(OutputType_Regression);
-   testOneState.AddFeatures({ FeatureTest(1) });
+   testOneState.AddFeatures({ FeatureTest(2, true, false) });
    testOneState.AddTerms({ { 0 } });
    testOneState.AddTrainingSamples({ TestSample({ 0 }, 10) });
    testOneState.AddValidationSamples({ TestSample({ 0 }, 12) });
    testOneState.InitializeBoosting();
 
    TestApi testTwoStates = TestApi(OutputType_Regression);
    testTwoStates.AddFeatures({ FeatureTest(2) });
@@ -1074,15 +1077,15 @@
    testZeroDimensions.AddFeatures({});
    testZeroDimensions.AddTerms({ {} });
    testZeroDimensions.AddTrainingSamples({ TestSample({}, 0) });
    testZeroDimensions.AddValidationSamples({ TestSample({}, 0) });
    testZeroDimensions.InitializeBoosting();
 
    TestApi testOneState = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
-   testOneState.AddFeatures({ FeatureTest(1) });
+   testOneState.AddFeatures({ FeatureTest(2, true, false) });
    testOneState.AddTerms({ { 0 } });
    testOneState.AddTrainingSamples({ TestSample({ 0 }, 0) });
    testOneState.AddValidationSamples({ TestSample({ 0 }, 0) });
    testOneState.InitializeBoosting();
 
    TestApi testTwoStates = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
    testTwoStates.AddFeatures({ FeatureTest(2) });
@@ -1121,15 +1124,15 @@
    testZeroDimensions.AddFeatures({});
    testZeroDimensions.AddTerms({ {} });
    testZeroDimensions.AddTrainingSamples({ TestSample({}, 0) });
    testZeroDimensions.AddValidationSamples({ TestSample({}, 0) });
    testZeroDimensions.InitializeBoosting();
 
    TestApi testOneState = TestApi(3);
-   testOneState.AddFeatures({ FeatureTest(1) });
+   testOneState.AddFeatures({ FeatureTest(2, true, false) });
    testOneState.AddTerms({ { 0 } });
    testOneState.AddTrainingSamples({ TestSample({ 0 }, 0) });
    testOneState.AddValidationSamples({ TestSample({ 0 }, 0) });
    testOneState.InitializeBoosting();
 
    TestApi testTwoStates = TestApi(3);
    testTwoStates.AddFeatures({ FeatureTest(2) });
@@ -1167,39 +1170,39 @@
          CHECK_APPROX(termScoreZeroDimensions2, termScoreTwoStates2);
       }
    }
 }
 
 TEST_CASE("3 dimensional term with one dimension reduced in different ways, boosting, regression") {
    TestApi test0 = TestApi(OutputType_Regression);
-   test0.AddFeatures({ FeatureTest(1), FeatureTest(2), FeatureTest(2) });
+   test0.AddFeatures({ FeatureTest(2, true, false), FeatureTest(2), FeatureTest(2) });
    test0.AddTerms({ { 0, 1, 2 } });
    test0.AddTrainingSamples({
       TestSample({ 0, 0, 0 }, 9),
       TestSample({ 0, 1, 0 }, 10),
       TestSample({ 0, 0, 1 }, 11),
       TestSample({ 0, 1, 1 }, 12),
       });
    test0.AddValidationSamples({ TestSample({ 0, 1, 0 }, 12) });
    test0.InitializeBoosting();
 
    TestApi test1 = TestApi(OutputType_Regression);
-   test1.AddFeatures({ FeatureTest(2), FeatureTest(1), FeatureTest(2) });
+   test1.AddFeatures({ FeatureTest(2), FeatureTest(2, true, false), FeatureTest(2) });
    test1.AddTerms({ { 0, 1, 2 } });
    test1.AddTrainingSamples({
       TestSample({ 0, 0, 0 }, 9),
       TestSample({ 0, 0, 1 }, 10),
       TestSample({ 1, 0, 0 }, 11),
       TestSample({ 1, 0, 1 }, 12),
       });
    test1.AddValidationSamples({ TestSample({ 0, 0, 1 }, 12) });
    test1.InitializeBoosting();
 
    TestApi test2 = TestApi(OutputType_Regression);
-   test2.AddFeatures({ FeatureTest(2), FeatureTest(2), FeatureTest(1) });
+   test2.AddFeatures({ FeatureTest(2), FeatureTest(2), FeatureTest(2, true, false) });
    test2.AddTerms({ { 0, 1, 2 } });
    test2.AddTrainingSamples({
       TestSample({ 0, 0, 0 }, 9),
       TestSample({ 1, 0, 0 }, 10),
       TestSample({ 0, 1, 0 }, 11),
       TestSample({ 1, 1, 0 }, 12),
       });
@@ -1213,31 +1216,31 @@
          double validationMetric0 = test0.Boost(iTerm).validationMetric;
          double validationMetric1 = test1.Boost(iTerm).validationMetric;
          CHECK_APPROX(validationMetric0, validationMetric1);
          double validationMetric2 = test2.Boost(iTerm).validationMetric;
          CHECK_APPROX(validationMetric0, validationMetric2);
 
          double termScore01 = test0.GetCurrentTermScore(iTerm, { 0, 0, 0 }, 0);
-         double termScore02 = test0.GetCurrentTermScore(iTerm, { 0, 0, 1 }, 0);
+         double termScore02 = test0.GetCurrentTermScore(iTerm, { 1, 0, 0 }, 0);
          double termScore03 = test0.GetCurrentTermScore(iTerm, { 0, 1, 0 }, 0);
-         double termScore04 = test0.GetCurrentTermScore(iTerm, { 0, 1, 1 }, 0);
+         double termScore04 = test0.GetCurrentTermScore(iTerm, { 1, 1, 0 }, 0);
 
          double termScore11 = test1.GetCurrentTermScore(iTerm, { 0, 0, 0 }, 0);
-         double termScore12 = test1.GetCurrentTermScore(iTerm, { 1, 0, 0 }, 0);
-         double termScore13 = test1.GetCurrentTermScore(iTerm, { 0, 0, 1 }, 0);
+         double termScore12 = test1.GetCurrentTermScore(iTerm, { 0, 0, 1 }, 0);
+         double termScore13 = test1.GetCurrentTermScore(iTerm, { 1, 0, 0 }, 0);
          double termScore14 = test1.GetCurrentTermScore(iTerm, { 1, 0, 1 }, 0);
          CHECK_APPROX(termScore11, termScore01);
          CHECK_APPROX(termScore12, termScore02);
          CHECK_APPROX(termScore13, termScore03);
          CHECK_APPROX(termScore14, termScore04);
 
          double termScore21 = test2.GetCurrentTermScore(iTerm, { 0, 0, 0 }, 0);
          double termScore22 = test2.GetCurrentTermScore(iTerm, { 0, 1, 0 }, 0);
-         double termScore23 = test2.GetCurrentTermScore(iTerm, { 1, 0, 0 }, 0);
-         double termScore24 = test2.GetCurrentTermScore(iTerm, { 1, 1, 0 }, 0);
+         double termScore23 = test2.GetCurrentTermScore(iTerm, { 0, 0, 1 }, 0);
+         double termScore24 = test2.GetCurrentTermScore(iTerm, { 0, 1, 1 }, 0);
          CHECK_APPROX(termScore21, termScore01);
          CHECK_APPROX(termScore22, termScore02);
          CHECK_APPROX(termScore23, termScore03);
          CHECK_APPROX(termScore24, termScore04);
       }
    }
 }
@@ -1320,15 +1323,15 @@
    static const std::vector<IntEbm> k_leavesMax = {
       IntEbm { 3 },
       IntEbm { 3 },
       IntEbm { 3 }
    };
 
    TestApi test = TestApi(3);
-   test.AddFeatures({ FeatureTest(cStates), FeatureTest(1), FeatureTest(cStates) });
+   test.AddFeatures({ FeatureTest(cStates), FeatureTest(2, true, false), FeatureTest(cStates) });
    test.AddTerms({ { 0, 1, 2 } });
    std::vector<TestSample> samples;
    for(IntEbm i0 = 0; i0 < cStates; ++i0) {
       for(IntEbm i2 = 0; i2 < cStates; ++i2) {
          // create a few zero spaces where we have no data
          if(i0 != i2) {
             if(i0 < i2) {
@@ -1556,15 +1559,15 @@
 
 TEST_CASE("Random splitting, no splits, binary, sums") {
    static const std::vector<IntEbm> k_leavesMax = {
       IntEbm { 3 }
    };
 
    TestApi test = TestApi(OutputType_BinaryClassification);
-   test.AddFeatures({ FeatureTest(1) });
+   test.AddFeatures({ FeatureTest(2, true, false) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({
       TestSample({ 0 }, 0),
       TestSample({ 0 }, 0),
       TestSample({ 0 }, 1),
       TestSample({ 0 }, 1),
       TestSample({ 0 }, 1),
@@ -1645,15 +1648,15 @@
    double gainAvg2 = test2.Boost(0).gainAvg;
 
    CHECK_APPROX(gainAvg1, gainAvg2);
 }
 
 TEST_CASE("tweedie, boosting") {
    TestApi test = TestApi(OutputType_Regression, EBM_FALSE, "tweedie_deviance:variance_power=1.3");
-   test.AddFeatures({ FeatureTest(1) });
+   test.AddFeatures({ FeatureTest(2, true, false) });
    test.AddTerms({ { 0 } });
    test.AddTrainingSamples({ TestSample({ 0 }, 10) });
    test.AddValidationSamples({ TestSample({ 0 }, 12) });
    test.InitializeBoosting();
 
    double validationMetric = double { std::numeric_limits<double>::quiet_NaN() };
    double termScore = double { std::numeric_limits<double>::quiet_NaN() };
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/dataset_shared_test.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/dataset_shared_test.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -66,34 +66,34 @@
    IntEbm part;
    ErrorEbm error;
 
    part = MeasureDataSetHeader(2, 0, 1);
    CHECK(0 <= part);
    sum += part;
 
-   part = MeasureFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr);
+   part = MeasureFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
-   part = MeasureFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr);
+   part = MeasureFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
    part = MeasureRegressionTarget(0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
    std::vector<char> buffer(static_cast<size_t>(sum) + 1, 77);
    buffer[static_cast<size_t>(sum)] = 99;
 
    error = FillDataSetHeader(2, 0, 1, sum, &buffer[0]);
    CHECK(Error_None == error);
-   error = FillFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
+   error = FillFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
-   error = FillFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
+   error = FillFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
    error = FillRegressionTarget(0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
 
    CHECK(99 == buffer[static_cast<size_t>(sum)]);
 }
 
@@ -192,34 +192,34 @@
    IntEbm part;
    ErrorEbm error;
 
    part = MeasureDataSetHeader(2, 0, 1);
    CHECK(0 <= part);
    sum += part;
 
-   part = MeasureFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr);
+   part = MeasureFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
-   part = MeasureFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr);
+   part = MeasureFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
    part = MeasureClassificationTarget(0, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
    std::vector<char> buffer(static_cast<size_t>(sum) + 1, 77);
    buffer[static_cast<size_t>(sum)] = 99;
 
    error = FillDataSetHeader(2, 0, 1, sum, &buffer[0]);
    CHECK(Error_None == error);
-   error = FillFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
+   error = FillFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
-   error = FillFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
+   error = FillFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
    error = FillClassificationTarget(0, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
 
    CHECK(99 == buffer[static_cast<size_t>(sum)]);
 }
 
@@ -339,34 +339,34 @@
    CHECK(0 <= part);
    sum += part;
 
    part = MeasureWeight(0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
-   part = MeasureFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr);
+   part = MeasureFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
-   part = MeasureFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr);
+   part = MeasureFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
    part = MeasureRegressionTarget(0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
    std::vector<char> buffer(static_cast<size_t>(sum) + 1, 77);
    buffer[static_cast<size_t>(sum)] = 99;
 
    error = FillDataSetHeader(2, 1, 1, sum, &buffer[0]);
    CHECK(Error_None == error);
-   error = FillFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
+   error = FillFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
-   error = FillFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
+   error = FillFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
    error = FillWeight(0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
    error = FillRegressionTarget(0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
 
    CHECK(99 == buffer[static_cast<size_t>(sum)]);
@@ -487,19 +487,19 @@
    IntEbm part;
    ErrorEbm error;
 
    part = MeasureDataSetHeader(2, 1, 1);
    CHECK(0 <= part);
    sum += part;
 
-   part = MeasureFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr);
+   part = MeasureFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
-   part = MeasureFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr);
+   part = MeasureFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
    part = MeasureWeight(0, nullptr);
    CHECK(0 <= part);
    sum += part;
 
@@ -508,17 +508,17 @@
    sum += part;
 
    std::vector<char> buffer(static_cast<size_t>(sum) + 1, 77);
    buffer[static_cast<size_t>(sum)] = 99;
 
    error = FillDataSetHeader(2, 1, 1, sum, &buffer[0]);
    CHECK(Error_None == error);
-   error = FillFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
+   error = FillFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
-   error = FillFeature(0, EBM_TRUE, EBM_TRUE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
+   error = FillFeature(2, EBM_FALSE, EBM_FALSE, EBM_FALSE, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
    error = FillWeight(0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
    error = FillClassificationTarget(0, 0, nullptr, sum, &buffer[0]);
    CHECK(Error_None == error);
 
    CHECK(99 == buffer[static_cast<size_t>(sum)]);
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/include_c.c` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/include_c.c`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/interaction_unusual_inputs.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/interaction_unusual_inputs.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
    double validationMetric = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == validationMetric);
 }
 
 TEST_CASE("features with 0 states, interaction") {
    TestApi test = TestApi(OutputType_Regression);
-   test.AddFeatures({ FeatureTest(0) });
+   test.AddFeatures({ FeatureTest(2, false, false) });
    test.AddInteractionSamples({});
    test.InitializeInteraction();
 
    double validationMetric = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == validationMetric);
 }
 
@@ -94,33 +94,33 @@
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({});
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("Term with one feature with one state, interaction, regression") {
    TestApi test = TestApi(OutputType_Regression);
-   test.AddFeatures({ FeatureTest(1) });
+   test.AddFeatures({ FeatureTest(2, true, false) });
    test.AddInteractionSamples({ TestSample({ 0 }, 10) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("Term with one feature with one state, interaction, binary") {
    TestApi test = TestApi(OutputType_BinaryClassification, EBM_FALSE, nullptr, 0);
-   test.AddFeatures({ FeatureTest(1) });
+   test.AddFeatures({ FeatureTest(2, true, false) });
    test.AddInteractionSamples({ TestSample({ 0 }, 0) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("Term with one feature with one state, interaction, multiclass") {
    TestApi test = TestApi(3);
-   test.AddFeatures({ FeatureTest(1) });
+   test.AddFeatures({ FeatureTest(2, true, false) });
    test.AddInteractionSamples({ TestSample({ 0 }, 0) });
    test.InitializeInteraction();
    double metricReturn = test.TestCalcInteractionStrength({ 0 });
    CHECK(0 == metricReturn);
 }
 
 TEST_CASE("weights are proportional, interaction, regression") {
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.bat` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.bat`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,16 @@
 
 void TestApi::AddFeatures(const std::vector<FeatureTest> features) {
    if(Stage::Beginning != m_stage) {
       exit(1);
    }
 
    for(const FeatureTest & oneFeature : features) {
+      m_featureMissings.push_back(oneFeature.m_bMissing ? EBM_TRUE : EBM_FALSE);
+      m_featureUnknowns.push_back(oneFeature.m_bUnknown ? EBM_TRUE : EBM_FALSE);
       m_featureNominals.push_back(oneFeature.m_bNominal ? EBM_TRUE : EBM_FALSE);
       m_featureBinCounts.push_back(oneFeature.m_countBins);
    }
 
    m_stage = Stage::FeaturesAdded;
 }
 
@@ -583,15 +585,15 @@
    for(size_t i = 0; i < cFeatures; ++i) {
       std::vector<IntEbm> trainingFeatures(m_trainingBinIndexes.begin() + i * cTrainingSamples, m_trainingBinIndexes.begin() + i * cTrainingSamples + cTrainingSamples);
       std::vector<IntEbm> validationFeatures(m_validationBinIndexes.begin() + i * cValidationSamples, m_validationBinIndexes.begin() + i * cValidationSamples + cValidationSamples);
 
       std::vector<IntEbm> allFeatures(trainingFeatures);
       allFeatures.insert(allFeatures.end(), validationFeatures.begin(), validationFeatures.end());
 
-      size += MeasureFeature(m_featureBinCounts[i], EBM_TRUE, EBM_TRUE, m_featureNominals[i], allFeatures.size(), 0 == allFeatures.size() ? nullptr : &allFeatures[0]);
+      size += MeasureFeature(m_featureBinCounts[i], m_featureMissings[i], m_featureUnknowns[i], m_featureNominals[i], allFeatures.size(), 0 == allFeatures.size() ? nullptr : &allFeatures[0]);
    }
 
    std::vector<double> allWeights(m_trainingWeights);
    allWeights.insert(allWeights.end(), m_validationWeights.begin(), m_validationWeights.end());
    size += MeasureWeight(allWeights.size(), 0 == allWeights.size() ? nullptr : &allWeights[0]);
 
    if(IsClassification(m_cClasses)) {
@@ -611,15 +613,15 @@
    for(size_t i = 0; i < cFeatures; ++i) {
       std::vector<IntEbm> trainingFeatures(m_trainingBinIndexes.begin() + i * cTrainingSamples, m_trainingBinIndexes.begin() + i * cTrainingSamples + cTrainingSamples);
       std::vector<IntEbm> validationFeatures(m_validationBinIndexes.begin() + i * cValidationSamples, m_validationBinIndexes.begin() + i * cValidationSamples + cValidationSamples);
 
       std::vector<IntEbm> allFeatures(trainingFeatures);
       allFeatures.insert(allFeatures.end(), validationFeatures.begin(), validationFeatures.end());
 
-      error = FillFeature(m_featureBinCounts[i], EBM_TRUE, EBM_TRUE, m_featureNominals[i], allFeatures.size(), 0 == allFeatures.size() ? nullptr : &allFeatures[0], size, pDataSet);
+      error = FillFeature(m_featureBinCounts[i], m_featureMissings[i], m_featureUnknowns[i], m_featureNominals[i], allFeatures.size(), 0 == allFeatures.size() ? nullptr : &allFeatures[0], size, pDataSet);
    }
 
    error = FillWeight(allWeights.size(), 0 == allWeights.size() ? nullptr : &allWeights[0], size, pDataSet);
 
    if(IsClassification(m_cClasses)) {
       std::vector<IntEbm> allTargets(m_trainingClassificationTargets);
       allTargets.insert(allTargets.end(), m_validationClassificationTargets.begin(), m_validationClassificationTargets.end());
@@ -992,15 +994,15 @@
    if(m_bNullInteractionWeights) {
       m_interactionWeights.resize(cSamples);
    }
 
    IntEbm size = MeasureDataSetHeader(cFeatures, 1, 1);
    for(size_t i = 0; i < cFeatures; ++i) {
       std::vector<IntEbm> allFeatures(m_interactionBinIndexes.begin() + i * cSamples, m_interactionBinIndexes.begin() + i * cSamples + cSamples);
-      size += MeasureFeature(m_featureBinCounts[i], EBM_TRUE, EBM_TRUE, m_featureNominals[i], allFeatures.size(), 0 == allFeatures.size() ? nullptr : &allFeatures[0]);
+      size += MeasureFeature(m_featureBinCounts[i], m_featureMissings[i], m_featureUnknowns[i], m_featureNominals[i], allFeatures.size(), 0 == allFeatures.size() ? nullptr : &allFeatures[0]);
    }
 
    size += MeasureWeight(m_interactionWeights.size(), 0 == m_interactionWeights.size() ? nullptr : &m_interactionWeights[0]);
 
    if(IsClassification(m_cClasses)) {
       size += MeasureClassificationTarget(m_cClasses, cSamples, 0 == cSamples ? nullptr : &m_interactionClassificationTargets[0]);
    } else {
@@ -1009,15 +1011,15 @@
 
    void * pDataSet = malloc(static_cast<size_t>(size));
 
    error = FillDataSetHeader(cFeatures, 1, 1, size, pDataSet);
 
    for(size_t i = 0; i < cFeatures; ++i) {
       std::vector<IntEbm> allFeatures(m_interactionBinIndexes.begin() + i * cSamples, m_interactionBinIndexes.begin() + i * cSamples + cSamples);
-      error = FillFeature(m_featureBinCounts[i], EBM_TRUE, EBM_TRUE, m_featureNominals[i], allFeatures.size(), 0 == allFeatures.size() ? nullptr : &allFeatures[0], size, pDataSet);
+      error = FillFeature(m_featureBinCounts[i], m_featureMissings[i], m_featureUnknowns[i], m_featureNominals[i], allFeatures.size(), 0 == allFeatures.size() ? nullptr : &allFeatures[0], size, pDataSet);
    }
 
    error = FillWeight(m_interactionWeights.size(), 0 == m_interactionWeights.size() ? nullptr : &m_interactionWeights[0], size, pDataSet);
 
    if(IsClassification(m_cClasses)) {
       error = FillClassificationTarget(m_cClasses, cSamples, 0 == cSamples ? nullptr : &m_interactionClassificationTargets[0], size, pDataSet);
    } else {
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.hpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -149,23 +149,30 @@
 }
 
 static constexpr SeedEbm k_seed = SeedEbm { -42 };
 
 class FeatureTest final {
 public:
 
-   const bool m_bNominal;
    const IntEbm m_countBins;
+   const bool m_bMissing;
+   const bool m_bUnknown;
+   const bool m_bNominal;
 
    inline FeatureTest(
       const IntEbm countBins, 
+      const bool bMissing = true,
+      const bool bUnknown = true,
       const bool bNominal = false
    ) :
-      m_bNominal(bNominal),
-      m_countBins(countBins) {
+      m_countBins(countBins),
+      m_bMissing(bMissing),
+      m_bUnknown(bUnknown),
+      m_bNominal(bNominal)
+   {
       if(countBins < 0) {
          exit(1);
       }
    }
 };
 
 class TestSample final {
@@ -293,14 +300,16 @@
    Stage m_stage;
    const OutputType m_cClasses;
    const ptrdiff_t m_iZeroClassificationLogit;
 
    BoolEbm m_bDifferentiallyPrivate;
    const char * m_sObjective;
 
+   std::vector<BoolEbm> m_featureMissings;
+   std::vector<BoolEbm> m_featureUnknowns;
    std::vector<BoolEbm> m_featureNominals;
    std::vector<IntEbm> m_featureBinCounts;
    std::vector<IntEbm> m_dimensionCounts;
    std::vector<IntEbm> m_featureIndexes;
 
    std::vector<std::vector<size_t>> m_termBinCounts;
```

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.sh` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.sh`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.vcxproj` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.vcxproj`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/libebm_test.vcxproj.filters` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/libebm_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/random_test.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/random_test.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/tests/rehydrate_booster.cpp` & `interpret-core-0.4.2/symbolic/shared/libebm/tests/rehydrate_booster.cpp`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/libebm/vs_python_setup.txt` & `interpret-core-0.4.2/symbolic/shared/libebm/vs_python_setup.txt`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/vis/package.json` & `interpret-core-0.4.2/symbolic/shared/vis/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.4.2'"}*

```diff
@@ -43,9 +43,9 @@
     },
     "scripts": {
         "build-dev": "webpack --mode development",
         "build-prod": "webpack --mode production",
         "clean": "rm dist/interpret-inline.js",
         "start": "webpack-dev-server --hot --mode development"
     },
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `interpret-core-0.4.1/symbolic/shared/vis/src/index.js` & `interpret-core-0.4.2/symbolic/shared/vis/src/index.js`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/vis/src/styles.scss` & `interpret-core-0.4.2/symbolic/shared/vis/src/styles.scss`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/symbolic/shared/vis/webpack.config.js` & `interpret-core-0.4.2/symbolic/shared/vis/webpack.config.js`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/api/test_base.py` & `interpret-core-0.4.2/tests/api/test_base.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/blackbox/test_permutationimportance.py` & `interpret-core-0.4.2/tests/blackbox/test_permutationimportance.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/ext/test_examples.py` & `interpret-core-0.4.2/tests/ext/test_examples.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/glassbox/ebm/research/test_group_importance.py` & `interpret-core-0.4.2/tests/glassbox/ebm/research/test_group_importance.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/glassbox/ebm/research/test_purify.py` & `interpret-core-0.4.2/tests/glassbox/ebm/research/test_purify.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/glassbox/ebm/test_bin.py` & `interpret-core-0.4.2/tests/glassbox/ebm/test_bin.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/glassbox/ebm/test_ebm.py` & `interpret-core-0.4.2/tests/glassbox/ebm/test_ebm.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     clf = ExplainableBoostingClassifier()
     clf.fit(X, y)
 
     intercept = clf.intercept_
     clf.monotonize(0, increasing=True)
     clf.monotonize(1, increasing=False)
     clf.monotonize(2, increasing="auto")
+    clf.monotonize(3)
 
     valid_ebm(clf)
 
     assert np.all(np.diff(clf.term_features_[0]) >= 0)
     assert np.all(np.diff(clf.term_features_[1]) <= 0)
     diff = np.diff(clf.term_features_[2])
     assert np.all(diff >= 0) or np.all(diff <= 0)
@@ -761,14 +762,59 @@
     clf = ExplainableBoostingClassifier()
     clf.fit(X, y)
     clf.predict(X_test)
 
     valid_ebm(clf)
 
 
+def test_bags():
+    data = synthetic_regression()
+    X = data["full"]["X"]
+    y = data["full"]["y"]
+
+    n_samples = X.shape[0]
+
+    init_score = np.full(n_samples, 3.0)
+    sample_weight = np.full(n_samples, 99.0)
+
+    bags = np.zeros((1, n_samples), np.int8)
+    for idx in range(n_samples - 2, -1, -2):
+        bags[0, idx] = 1
+        init_score[idx] = -0.5 * idx - 0.25
+        sample_weight[idx] = 0.25 * idx + 0.5
+
+    keep = bags[0] != 0
+
+    X0 = X[keep]
+    y0 = y[keep]
+    init_score0 = init_score[keep]
+    sample_weight0 = sample_weight[keep]
+
+    clf = ExplainableBoostingRegressor(
+        max_bins=n_samples + 2,
+        max_interaction_bins=n_samples + 2,
+        max_rounds=100,
+        outer_bags=1,
+        validation_size=0,
+    )
+    clf.fit(X0, y0, sample_weight=sample_weight0, init_score=init_score0)
+    pred0 = clf.predict(X0)
+
+    clf = ExplainableBoostingRegressor(
+        max_bins=n_samples + 2,
+        max_interaction_bins=n_samples + 2,
+        max_rounds=100,
+        outer_bags=1,
+    )
+    clf.fit(X, y, sample_weight=sample_weight, bags=bags, init_score=init_score)
+    pred1 = clf.predict(X0)
+
+    assert np.allclose(pred0, pred1)
+
+
 @pytest.mark.skip(
     reason="can't run this test reliably until we depend on scikit-learn 0.22"
 )
 def test_scikit_learn_compatibility():
     """Run scikit-learn compatibility tests"""
 
     # sklearn tests in:
```

### Comparing `interpret-core-0.4.1/tests/glassbox/ebm/test_ebm_utils.py` & `interpret-core-0.4.2/tests/glassbox/ebm/test_ebm_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/glassbox/ebm/test_merge_ebms.py` & `interpret-core-0.4.2/tests/glassbox/ebm/test_merge_ebms.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/glassbox/ebm/test_multiclass.py` & `interpret-core-0.4.2/tests/glassbox/ebm/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/glassbox/test_decisiontree.py` & `interpret-core-0.4.2/tests/glassbox/test_decisiontree.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/glassbox/test_linear.py` & `interpret-core-0.4.2/tests/glassbox/test_linear.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/greybox/test_treeinterpreter.py` & `interpret-core-0.4.2/tests/greybox/test_treeinterpreter.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/provider/test_providers.py` & `interpret-core-0.4.2/tests/provider/test_providers.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/test_develop.py` & `interpret-core-0.4.2/tests/test_develop.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/test_example_notebooks.py` & `interpret-core-0.4.2/tests/test_example_notebooks.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/test_explainers.py` & `interpret-core-0.4.2/tests/test_explainers.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/test_ext.py` & `interpret-core-0.4.2/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/test_extension_utils.py` & `interpret-core-0.4.2/tests/test_extension_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/test_mli_interop.py` & `interpret-core-0.4.2/tests/test_mli_interop.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/test_selenium.py` & `interpret-core-0.4.2/tests/test_selenium.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/tutils.py` & `interpret-core-0.4.2/tests/tutils.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/utils/test_SPOTgreedy.py` & `interpret-core-0.4.2/tests/utils/test_SPOTgreedy.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/utils/test_clean_simple.py` & `interpret-core-0.4.2/tests/utils/test_clean_simple.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/utils/test_clean_x.py` & `interpret-core-0.4.2/tests/utils/test_clean_x.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/utils/test_compressed_dataset.py` & `interpret-core-0.4.2/tests/utils/test_compressed_dataset.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/utils/test_explanation.py` & `interpret-core-0.4.2/tests/utils/test_explanation.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/utils/test_measure_interactions.py` & `interpret-core-0.4.2/tests/utils/test_measure_interactions.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/utils/test_native.py` & `interpret-core-0.4.2/tests/utils/test_native.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/visual/test_inline.py` & `interpret-core-0.4.2/tests/visual/test_inline.py`

 * *Files identical despite different names*

### Comparing `interpret-core-0.4.1/tests/visual/test_interactive.py` & `interpret-core-0.4.2/tests/visual/test_interactive.py`

 * *Files identical despite different names*

