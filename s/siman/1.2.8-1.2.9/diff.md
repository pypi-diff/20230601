# Comparing `tmp/siman-1.2.8.tar.gz` & `tmp/siman-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.2.8.tar", last modified: Fri May 12 13:35:10 2023, max compression
+gzip compressed data, was "dist/siman-1.2.9.tar", last modified: Thu Jun  1 10:25:57 2023, max compression
```

## Comparing `siman-1.2.8.tar` & `siman-1.2.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.774413 siman-1.2.8/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.2.8/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.2.8/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-05-12 13:35:10.774413 siman-1.2.8/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.2.8/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-05-12 13:35:10.774413 siman-1.2.8/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-05-12 13:35:04.000000 siman-1.2.8/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.771413 siman-1.2.8/siman/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.2.8/siman/3d_plot.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.2.8/siman/SSHTools.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.2.8/siman/__init__.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49532 2022-09-29 10:57:16.000000 siman-1.2.8/siman/analysis.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.2.8/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.772413 siman-1.2.8/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.8/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.2.8/siman/analyze/segregation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.2.8/siman/approximation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.2.8/siman/bands.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   125759 2023-05-12 13:34:11.000000 siman-1.2.8/siman/calc_manage.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.2.8/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.772413 siman-1.2.8/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-04-04 10:46:17.000000 siman-1.2.8/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.772413 siman-1.2.8/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.2.8/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.2.8/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.2.8/siman/chg/vasputil_chgarith_module.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.2.8/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.773413 siman-1.2.8/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.8/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53303 2023-04-04 10:20:35.000000 siman-1.2.8/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.2.8/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.2.8/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.2.8/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.2.8/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118077 2023-04-18 16:31:52.000000 siman-1.2.8/siman/core/structure.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20209 2022-12-15 17:24:44.000000 siman-1.2.8/siman/database.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.2.8/siman/default_project_conf.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.2.8/siman/dev_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.2.8/siman/dos_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.2.8/siman/fit_hex.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28019 2022-09-20 15:22:50.000000 siman-1.2.8/siman/functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.2.8/siman/geo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14496 2023-01-30 17:40:21.000000 siman-1.2.8/siman/header.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.2.8/siman/helper_for_writing_beatiful_code.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.2.8/siman/impurity.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80434 2022-09-29 10:57:16.000000 siman-1.2.8/siman/inout.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.2.8/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.774413 siman-1.2.8/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.8/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.2.8/siman/mat_prop/mat_prop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.2.8/siman/matproj_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.2.8/siman/monte.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.2.8/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.2.8/siman/neb.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.2.8/siman/pairs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.2.8/siman/picture_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.2.8/siman/plot_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4434 2023-04-06 13:23:01.000000 siman-1.2.8/siman/polaron.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.2.8/siman/polaron_hop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.2.8/siman/polaron_mod.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.2.8/siman/project_funcs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.2.8/siman/properties_2d.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.2.8/siman/properties_energy.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.2.8/siman/properties_lattice.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-04-04 10:53:58.000000 siman-1.2.8/siman/set_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.2.8/siman/simanrc.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.2.8/siman/small_classes.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.2.8/siman/small_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.2.8/siman/structure_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.2.8/siman/table_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.2.8/siman/thermo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.2.8/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.772413 siman-1.2.8/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.138047 siman-1.2.9/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.2.9/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.2.9/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-06-01 10:25:57.138047 siman-1.2.9/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.2.9/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-06-01 10:25:57.139047 siman-1.2.9/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-06-01 10:25:51.000000 siman-1.2.9/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.136047 siman-1.2.9/siman/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.2.9/siman/3d_plot.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.2.9/siman/SSHTools.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.2.9/siman/__init__.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49532 2022-09-29 10:57:16.000000 siman-1.2.9/siman/analysis.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.2.9/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.136047 siman-1.2.9/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.9/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.2.9/siman/analyze/segregation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.2.9/siman/approximation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.2.9/siman/bands.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   125775 2023-05-22 16:36:10.000000 siman-1.2.9/siman/calc_manage.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.2.9/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.137047 siman-1.2.9/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-04-04 10:46:17.000000 siman-1.2.9/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.137047 siman-1.2.9/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.2.9/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.2.9/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.2.9/siman/chg/vasputil_chgarith_module.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.2.9/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.138047 siman-1.2.9/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.9/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53303 2023-04-04 10:20:35.000000 siman-1.2.9/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.2.9/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.2.9/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.2.9/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.2.9/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118077 2023-04-18 16:31:52.000000 siman-1.2.9/siman/core/structure.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20209 2022-12-15 17:24:44.000000 siman-1.2.9/siman/database.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.2.9/siman/default_project_conf.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.2.9/siman/dev_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.2.9/siman/dos_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.2.9/siman/fit_hex.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-05-24 11:04:51.000000 siman-1.2.9/siman/functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.2.9/siman/geo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14499 2023-06-01 09:41:19.000000 siman-1.2.9/siman/header.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.2.9/siman/helper_for_writing_beatiful_code.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.2.9/siman/impurity.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80434 2022-09-29 10:57:16.000000 siman-1.2.9/siman/inout.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.2.9/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.138047 siman-1.2.9/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.9/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.2.9/siman/mat_prop/mat_prop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.2.9/siman/matproj_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.2.9/siman/monte.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.2.9/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.2.9/siman/neb.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.2.9/siman/pairs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.2.9/siman/picture_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.2.9/siman/plot_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4434 2023-04-06 13:23:01.000000 siman-1.2.9/siman/polaron.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.2.9/siman/polaron_hop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.2.9/siman/polaron_mod.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.2.9/siman/project_funcs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.2.9/siman/properties_2d.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.2.9/siman/properties_energy.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.2.9/siman/properties_lattice.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-04-04 10:53:58.000000 siman-1.2.9/siman/set_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.2.9/siman/simanrc.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.2.9/siman/small_classes.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.2.9/siman/small_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.2.9/siman/structure_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.2.9/siman/table_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.2.9/siman/thermo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.2.9/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.136047 siman-1.2.9/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/top_level.txt
```

### Comparing `siman-1.2.8/LICENSE` & `siman-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/PKG-INFO` & `siman-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.2.8
+Version: 1.2.9
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.2.8/setup.py` & `siman-1.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.2.8",
+    version="1.2.9",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.2.8/siman/3d_plot.py` & `siman-1.2.9/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/SSHTools.py` & `siman-1.2.9/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/analysis.py` & `siman-1.2.9/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/analysis_functions.py` & `siman-1.2.9/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/analyze/segregation.py` & `siman-1.2.9/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/approximation.py` & `siman-1.2.9/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/bands.py` & `siman-1.2.9/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/calc_manage.py` & `siman-1.2.9/siman/calc_manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -922,20 +922,20 @@
                 st1_vis = copy.deepcopy(st1)
                 st2_vis = copy.deepcopy(st2)
 
 
             else:
                 if existing:
                     st1 = copy.deepcopy(input_st)
-                    st2 = input_st.localize_polaron(pm['iend'], am)
-                    st2 = st2.localize_polaron(pm['istart'], -am) # return back existing polaron to normal
+                    st2 = input_st.localize_polaron(pm['iend'], am, nn)
+                    st2 = st2.localize_polaron(pm['istart'], -am, nn) # return back existing polaron to normal
 
                 else:
-                    st1 = input_st.localize_polaron(pm['istart'],  am)
-                    st2 = input_st.localize_polaron(pm['iend'], am)
+                    st1 = input_st.localize_polaron(pm['istart'],  am, nn)
+                    st2 = input_st.localize_polaron(pm['iend'], am, nn)
 
 
 
                 st1_vis = st1.replace_atoms([pm['istart']], 'U')
                 st2_vis = st2.replace_atoms([pm['iend']], 'U')
             st1_vis.write_poscar('xyz/'+it+'/1.POSCAR')
             st2_vis.write_poscar('xyz/'+it+'/100.POSCAR')
```

### Comparing `siman-1.2.8/siman/calcul.py` & `siman-1.2.9/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/calculators/aims.py` & `siman-1.2.9/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/calculators/gaussian.py` & `siman-1.2.9/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/calculators/qe.py` & `siman-1.2.9/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/calculators/vasp.py` & `siman-1.2.9/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/calculators/vasp_old.py` & `siman-1.2.9/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/chg/chg_func.py` & `siman-1.2.9/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/chg/vasputil_chgarith_module.py` & `siman-1.2.9/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/classes.py` & `siman-1.2.9/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/core/calculation.py` & `siman-1.2.9/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/core/calculation_old.py` & `siman-1.2.9/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/core/cluster_batch_script.py` & `siman-1.2.9/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/core/cluster_run_script.py` & `siman-1.2.9/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/core/molecule.py` & `siman-1.2.9/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/core/structure.py` & `siman-1.2.9/siman/core/structure.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/database.py` & `siman-1.2.9/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/default_project_conf.py` & `siman-1.2.9/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/dev_functions.py` & `siman-1.2.9/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/dos_functions.py` & `siman-1.2.9/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/fit_hex.py` & `siman-1.2.9/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/functions.py` & `siman-1.2.9/siman/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         if algo = 'my'
             n of 10-15 is good
     """
     algo = 'gaus'
     # algo = 'my'
 
     if algo == 'my':
+        #average on interval
         x_smooth = []
         L = len(x)
         store = np.zeros((n,1),float)
         for u in range(L-n):
           for v in range(n):
                store[v] = x[u+v]
           av = float(sum(store)) / n
```

### Comparing `siman-1.2.8/siman/geo.py` & `siman-1.2.9/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/header.py` & `siman-1.2.9/siman/header.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,21 @@
     # sys.path.append('/home/dim/Simulation_wrapper/ase') #
     # plt = None
 except:
     mpl = None
     plt = None
     print('Warning! matplotlib is not installed! Some functions will not work!')
 
+try:
+    import matplotlib.pyplot as plt
+except:
+    plt = None
+
+
+
 history = []
 
 #Defaults to some project_conf values
 PBS_PROCS = False # if true than #PBS -l procs="+str(number_cores) is used
 WALLTIME_LIMIT = False # now only for PBS if True 72 hours limit is used
 CIF2CELL = False
 
@@ -102,18 +109,14 @@
 
 
 
 
 
 
 
-try:
-    import matplotlib.pyplot as plt
-except:
-    plt = None
 
 calc_database = 'only_calc.gdbm3'
 
 class CalcDict(dict):
     def __getitem__(self, key):
         # print(self)
         if type(key) == str:
```

### Comparing `siman-1.2.8/siman/impurity.py` & `siman-1.2.9/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/inout.py` & `siman-1.2.9/siman/inout.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/kpoints_functions.py` & `siman-1.2.9/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/mat_prop/mat_prop.py` & `siman-1.2.9/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/matproj_functions.py` & `siman-1.2.9/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/monte.py` & `siman-1.2.9/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/monte_functions.py` & `siman-1.2.9/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/neb.py` & `siman-1.2.9/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/pairs.py` & `siman-1.2.9/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/picture_functions.py` & `siman-1.2.9/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/plot_functions.py` & `siman-1.2.9/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/polaron.py` & `siman-1.2.9/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/polaron_hop.py` & `siman-1.2.9/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/polaron_mod.py` & `siman-1.2.9/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/project_funcs.py` & `siman-1.2.9/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/properties_2d.py` & `siman-1.2.9/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/properties_energy.py` & `siman-1.2.9/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/properties_lattice.py` & `siman-1.2.9/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/set_functions.py` & `siman-1.2.9/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/simanrc.py` & `siman-1.2.9/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/small_functions.py` & `siman-1.2.9/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/structure_functions.py` & `siman-1.2.9/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/table_functions.py` & `siman-1.2.9/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/thermo.py` & `siman-1.2.9/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman/workflow_utilities.py` & `siman-1.2.9/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.8/siman.egg-info/PKG-INFO` & `siman-1.2.9/siman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.2.8
+Version: 1.2.9
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.2.8/siman.egg-info/SOURCES.txt` & `siman-1.2.9/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

