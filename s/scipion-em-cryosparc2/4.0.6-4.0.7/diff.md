# Comparing `tmp/scipion-em-cryosparc2-4.0.6.tar.gz` & `tmp/scipion-em-cryosparc2-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryosparc2-4.0.6.tar", last modified: Fri May 26 16:04:54 2023, max compression
+gzip compressed data, was "scipion-em-cryosparc2-4.0.7.tar", last modified: Thu Jun  1 12:14:06 2023, max compression
```

## Comparing `scipion-em-cryosparc2-4.0.6.tar` & `scipion-em-cryosparc2-4.0.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.766321 scipion-em-cryosparc2-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-26 16:04:54.766321 scipion-em-cryosparc2-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.758321 scipion-em-cryosparc2-4.0.6/cryosparc2/
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)    32630 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.762321 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/cs2Start.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/cryosparc2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.762321 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryorefine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23442 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
--rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
--rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_ab.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23634 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23794 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    20831 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_sharppening.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.762321 scipion-em-cryosparc2-4.0.6/cryosparc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/tests/test_protocols_cryosparc2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34295 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.762321 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_2Dclassify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_partsubtract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.766321 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:04:54.766321 scipion-em-cryosparc2-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:14:06.865212 scipion-em-cryosparc2-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-01 12:14:06.865212 scipion-em-cryosparc2-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:14:06.861212 scipion-em-cryosparc2-4.0.7/cryosparc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32573 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:14:06.861212 scipion-em-cryosparc2-4.0.7/cryosparc2/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28297 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/convert/cs2Start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/cryosparc2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:14:06.865212 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryorefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23502 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24121 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_ab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23634 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23794 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_sharppening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:14:06.865212 scipion-em-cryosparc2-4.0.7/cryosparc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47395 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/tests/test_protocols_cryosparc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34295 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:14:06.865212 scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/viewer_2Dclassify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/viewer_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/viewer_partsubtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/viewer_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/cryosparc2/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:14:06.865212 scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-01 12:14:06.000000 scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-01 12:14:06.000000 scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:14:06.000000 scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 12:14:06.000000 scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 12:14:06.000000 scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 12:14:06.000000 scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:14:06.865212 scipion-em-cryosparc2-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-01 12:12:11.000000 scipion-em-cryosparc2-4.0.7/setup.py
```

### Comparing `scipion-em-cryosparc2-4.0.6/LICENSE` & `scipion-em-cryosparc2-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/PKG-INFO` & `scipion-em-cryosparc2-4.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.6
+Version: 4.0.7
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -34,19 +34,20 @@
         * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
         * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
         * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
         
         **Latest plugin version**
         ==========================
         
-        **v4.0.6**
+        **v4.0.7**
         -----------
         * **new**     :  Compatibility with cryoSPARC v4.2.1
         * **new**        Plugin operation in a cluster
         * **fixed**      Fixed an installation error
+        * **fixed**      Fixed an error related with the calculation of the particles shifts
         
         **Installing the plugin**
         =========================
         
         In order to install the plugin follow these instructions:
         
         1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.6/README.rst` & `scipion-em-cryosparc2-4.0.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
 * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
 * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
 
 **Latest plugin version**
 ==========================
 
-**v4.0.6**
+**v4.0.7**
 -----------
 * **new**     :  Compatibility with cryoSPARC v4.2.1
 * **new**        Plugin operation in a cluster
 * **fixed**      Fixed an installation error
+* **fixed**      Fixed an error related with the calculation of the particles shifts
 
 **Installing the plugin**
 =========================
 
 In order to install the plugin follow these instructions:
 
 1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/__init__.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 import os
 import pwem as em
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
-__version__ = '4.0.6'
+__version__ = '4.0.7'
 _references = ['Punjani2017', 'Brubaker2017', 'daniel_asarnow_2019_3576630']
 _logo = 'cryosparc2_logo.png'
 
 
 class Plugin(em.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-cryosparc2"
     _homeVar = CRYOSPARC_HOME
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/bibtex.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/constants.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # *
 # **************************************************************************
 import enum
 from pwem.constants import (
     SYM_CYCLIC, SYM_TETRAHEDRAL, SYM_OCTAHEDRAL, SYM_I222,
     SYM_I222r)
 
-
 from pwem.constants import SYM_DIHEDRAL_Y
+
 # Root folder where cryosparc is installed, we will look here for the client
 CRYOSPARC_HOME = 'CRYOSPARC_HOME'
 CRYOSPARC_DIR = 'CRYOSPARC_DIR'  # Legacy, replaced by CRYOSPARC_HOME
 # Optional: Folder where cryosparc projects will be created
 CRYO_PROJECTS_DIR = 'CRYO_PROJECTS_DIR'
 CRYOSPARC_USER = 'CRYOSPARC_USER'
 CRYOSPARC_USE_SSD = 'CRYOSPARC_USE_SSD'
@@ -42,23 +42,25 @@
 CRYOSPARC_STANDALONE_INSTALLATION = 'CRYOSPARC_STANDALONE_INSTALLATION'
 CRYOSPARC_DEFAULT_LANE = 'CRYOSPARC_DEFAULT_LANE'
 CRYOSPARC_VERSION_FILE = 'version'
 CRYOSPARC_CONFIG_FILE = 'config.sh'
 CRYOSPARC_LICENSE_ID_VARIABLE = 'CRYOSPARC_LICENSE_ID'
 CRYOSPARC_CS2STAR_SCRIPT = 'cs2Start.py'
 
+
 def getPyemEnvName(version):
     return 'pyem-%s' % version
 
+
 # pyem environment variables
 PYEM_VERSION = '23.01.25'  # This is our made up version
 PYEM_ACTIVATION_CMD = 'conda activate %s' % (getPyemEnvName(PYEM_VERSION))
 
 # Supported versions:
-V_UNKNOWN ='v0.0.0'
+V_UNKNOWN = 'v0.0.0'
 V3_0_0 = 'v3.0.0'
 V3_0_1 = 'v3.0.1'
 V3_1_0 = 'v3.1.0'
 V3_2_0 = 'v3.2.0'
 V3_3_0 = 'v3.3.0'
 V3_3_1 = 'v3.3.1'
 V3_3_2 = 'V3.3.2'
@@ -85,16 +87,16 @@
                        'white',
                        'coloured']
 REFINE_MASK_CHOICES = ['dynamic',
                        'static',
                        'null']
 
 REFINE_FILTER_TYPE = ['butterworth',
-                     'rect',
-                     'gaussian']
+                      'rect',
+                      'gaussian']
 
 REFINE_FULCRUM_LOCATION = ['mask_center',
                            'box_center']
 
 COMPUTE_FACILITY_CHOICES = ['GPU',
                             'CPU']
 
@@ -116,15 +118,14 @@
 LAST_ITER = 0
 ALL_ITERS = 1
 SELECTED_ITERS = 2
 
 ANGDIST_2DPLOT = 0
 ANGDIST_CHIMERA = 1
 
-
 # VOLUME_SLICES = 0
 VOLUME_CHIMERA = 1
 VOLUME_CRYOSPARC = 0
 DATA_VIEWER = 0
 
 fscValues = dict()
 fscValues['fsc_nomask'] = 'No mask'
@@ -147,64 +148,67 @@
 OBJCMD_PROJS = 'Show only projections'
 OBJCMD_INITVOL = 'Show initial random volume'
 
 
 # METADATA
 
 class RELIONCOLUMNS(enum.Enum):
-    rlnOriginX = 'rlnOriginX'                        # RLN_ORIENT_ORIGIN_X
-    rlnOriginY = 'rlnOriginY'                        # RLN_ORIENT_ORIGIN_Y
-    rlnAngleRot = 'rlnAngleRot'                      # RLN_ORIENT_ROT
-    rlnAnglePsi = 'rlnAnglePsi'                      # RLN_ORIENT_PSI
-    rlnOriginZ = 'rlnOriginZ'                        # RLN_ORIENT_ORIGIN_Z
-    rlnClassNumber = 'rlnClassNumber'                # RLN_PARTICLE_CLASS
-    rlnImageName = 'rlnImageName'                    # RLN_IMAGE_NAME
-    rlnRandomSubset = 'rlnRandomSubset'              # RLN_PARTICLE_RANDOM_SUBSET
-    rlnAngleTilt = 'rlnAngleTilt'                    # RLN_ORIENT_TILT
-    rlnDefocusU = 'rlnDefocusU'                      # RLN_CTF_DEFOCUSU
-    rlnDefocusV = 'rlnDefocusV'                      # RLN_CTF_DEFOCUSV
-    rlnDefocusAngle = 'rlnDefocusAngle'              # RLN_CTF_DEFOCUS_ANGLE
-    rlnPhaseShift = 'rlnPhaseShift'                  # RLN_CTF_PHASESHIFT
-    rlnBfactor = 'rlnBfactor'                        # RLN_CTF_BFACTOR
+    rlnOriginX = 'rlnOriginX'  # RLN_ORIENT_ORIGIN_X
+    rlnOriginY = 'rlnOriginY'  # RLN_ORIENT_ORIGIN_Y
+    rlnAngleRot = 'rlnAngleRot'  # RLN_ORIENT_ROT
+    rlnAnglePsi = 'rlnAnglePsi'  # RLN_ORIENT_PSI
+    rlnOriginZ = 'rlnOriginZ'  # RLN_ORIENT_ORIGIN_Z
+    rlnOriginXAngst = 'rlnOriginXAngst'  # RLN_ORIENT_ORIGIN_X IN ANGSTROM
+    rlnOriginYAngst = 'rlnOriginYAngst'  # RLN_ORIENT_ORIGIN_Y IN ANGSTROM
+    rlnOriginZAngst = 'rlnOriginZAngst'  # RLN_ORIENT_ORIGIN_Z IN ANGSTROM
+
+    rlnClassNumber = 'rlnClassNumber'  # RLN_PARTICLE_CLASS
+    rlnImageName = 'rlnImageName'  # RLN_IMAGE_NAME
+    rlnRandomSubset = 'rlnRandomSubset'  # RLN_PARTICLE_RANDOM_SUBSET
+    rlnAngleTilt = 'rlnAngleTilt'  # RLN_ORIENT_TILT
+    rlnDefocusU = 'rlnDefocusU'  # RLN_CTF_DEFOCUSU
+    rlnDefocusV = 'rlnDefocusV'  # RLN_CTF_DEFOCUSV
+    rlnDefocusAngle = 'rlnDefocusAngle'  # RLN_CTF_DEFOCUS_ANGLE
+    rlnPhaseShift = 'rlnPhaseShift'  # RLN_CTF_PHASESHIFT
+    rlnBfactor = 'rlnBfactor'  # RLN_CTF_BFACTOR
     rlnOpticsGroup = 'rlnOpticsGroup'
-    rlnVoltage = 'rlnVoltage'                        # RLN_CTF_VOLTAGE
+    rlnVoltage = 'rlnVoltage'  # RLN_CTF_VOLTAGE
     rlnSphericalAberration = 'rlnSphericalAberration'  # RLN_CTF_CS
-    rlnAmplitudeContrast = 'rlnAmplitudeContrast'    # RLN_CTF_Q0
-    rlnImageSize = 'rlnImageSize'                    # RLN_IMAGE_SIZE
-    rlnEnabled = 'rlnEnabled'                        # RLN_IMAGE_ENABLED
-    rlnCtfFigureOfMerit = 'rlnCtfFigureOfMerit'     # RLN_CTF_FOM
-    rlnMagnification = 'rlnMagnification'           # RLN_CTF_MAGNIFICATION
-    rlnDetectorPixelSize = 'rlnDetectorPixelSize'    # RLN_CTF_DETECTOR_PIXEL_SIZE
+    rlnAmplitudeContrast = 'rlnAmplitudeContrast'  # RLN_CTF_Q0
+    rlnImageSize = 'rlnImageSize'  # RLN_IMAGE_SIZE
+    rlnEnabled = 'rlnEnabled'  # RLN_IMAGE_ENABLED
+    rlnCtfFigureOfMerit = 'rlnCtfFigureOfMerit'  # RLN_CTF_FOM
+    rlnMagnification = 'rlnMagnification'  # RLN_CTF_MAGNIFICATION
+    rlnDetectorPixelSize = 'rlnDetectorPixelSize'  # RLN_CTF_DETECTOR_PIXEL_SIZE
     rlnCtfImage = 'rlnCtfImage'
-    rlnAreaId = 'rlnAreaId'                        # RLN_AREA_ID
-    rlnAreaName = 'rlnAreaName'                    # RLN_AREA_NAME
-    rlnCtfScalefactor = 'rlnCtfScalefactor'         # RLN_CTF_SCALEFACTOR\
+    rlnAreaId = 'rlnAreaId'  # RLN_AREA_ID
+    rlnAreaName = 'rlnAreaName'  # RLN_AREA_NAME
+    rlnCtfScalefactor = 'rlnCtfScalefactor'  # RLN_CTF_SCALEFACTOR\
     rlnChromaticAberration = 'rlnChromaticAberration'  # RLN_CTF_CA
-    rlnEnergyLoss = 'rlnEnergyLoss'                   # RLN_CTF_ENERGY_LOSS
-    rlnLensStability = 'rlnLensStability'             # RLN_CTF_LENS_STABILITY
-    rlnCtfMaxResolution = 'rlnCtfMaxResolution'       # RLN_CTF_MAXRES
-    rlnConvergenceCone = 'rlnConvergenceCone'         # RLN_CTF_CONVERGENCE_CONE
+    rlnEnergyLoss = 'rlnEnergyLoss'  # RLN_CTF_ENERGY_LOSS
+    rlnLensStability = 'rlnLensStability'  # RLN_CTF_LENS_STABILITY
+    rlnCtfMaxResolution = 'rlnCtfMaxResolution'  # RLN_CTF_MAXRES
+    rlnConvergenceCone = 'rlnConvergenceCone'  # RLN_CTF_CONVERGENCE_CONE
     rlnLongitudinalDisplacement = 'rlnLongitudinalDisplacement'  # RLN_CTF_LONGITUDINAL_DISPLACEMENT
     rlnTransversalDisplacement = 'rlnTransversalDisplacement'  # RLN_CTF_TRANSVERSAL_DISPLACEMENT
-    rlnCtfValidationScore = 'rlnCtfValidationScore'       # RLN_CTF_VALIDATIONSCORE
-    rlnCtfValue = 'rlnCtfValue'                      # RLN_CTF_VALUE
+    rlnCtfValidationScore = 'rlnCtfValidationScore'  # RLN_CTF_VALIDATIONSCORE
+    rlnCtfValue = 'rlnCtfValue'  # RLN_CTF_VALUE
     rlnReconstructImageName = 'rlnReconstructImageName'  # RLN_IMAGE_RECONSTRUCT_NAME
-    rlnImageId = 'rlnImageId'           # RLN_IMAGE_ID
-    rlnDataType = 'rlnDataType'         # RLN_IMAGE_DATATYPE
-    rlnAutopickFigureOfMerit = 'rlnAutopickFigureOfMerit'   # RLN_PARTICLE_AUTOPICK_FOM
-    rlnCoordinateX = 'rlnCoordinateX'     # RLN_IMAGE_COORD_X
-    rlnCoordinateY = 'rlnCoordinateY'     # RLN_IMAGE_COORD_Y
-    rlnCoordinateZ = 'rlnCoordinateZ'     # RLN_IMAGE_COORD_Z
-    rlnMicrographName = 'rlnMicrographName' # RLN_MICROGRAPH_NAME
+    rlnImageId = 'rlnImageId'  # RLN_IMAGE_ID
+    rlnDataType = 'rlnDataType'  # RLN_IMAGE_DATATYPE
+    rlnAutopickFigureOfMerit = 'rlnAutopickFigureOfMerit'  # RLN_PARTICLE_AUTOPICK_FOM
+    rlnCoordinateX = 'rlnCoordinateX'  # RLN_IMAGE_COORD_X
+    rlnCoordinateY = 'rlnCoordinateY'  # RLN_IMAGE_COORD_Y
+    rlnCoordinateZ = 'rlnCoordinateZ'  # RLN_IMAGE_COORD_Z
+    rlnMicrographName = 'rlnMicrographName'  # RLN_MICROGRAPH_NAME
     rlnParticleSelectZScore = 'rlnParticleSelectZScore'  # RLN_SELECT_PARTICLES_ZSCORE
     rlnMovieFrameNumber = 'rlnMovieFrameNumber'  # RLN_IMAGE_FRAME_NR
-    rlnReferenceImage = 'rlnReferenceImage'     # RLN_MLMODEL_REF_IMAGE
-    rlnMicrographId = 'rlnMicrographId'          # RLN_MICROGRAPH_ID
-    rlnParticleId = 'rlnParticleId'      # RLN_PARTICLE_ID
-
+    rlnReferenceImage = 'rlnReferenceImage'  # RLN_MLMODEL_REF_IMAGE
+    rlnMicrographId = 'rlnMicrographId'  # RLN_MICROGRAPH_ID
+    rlnParticleId = 'rlnParticleId'  # RLN_PARTICLE_ID
 
 
 """
         // Label rlnImageDimensionality is originally rlnDataDimensionality, which is
         // duplicated for other label. A relion bug???
         MDL::addLabel(RLN_IMAGE_DIMENSIONALITY, LABEL_INT, "rlnImageDimensionality");
         MDL::addLabel(RLN_IMAGE_BEAMTILT_X, LABEL_DOUBLE, "rlnBeamTiltX");
@@ -470,15 +474,15 @@
         MDL::addLabelAlias(RLN_CTF_BFACTOR, "rlnCtfBfactor"); //Relion-2.0
 
 """
 
 COOR_EXTRA_LABELS = [RELIONCOLUMNS.rlnAutopickFigureOfMerit.value,
                      RELIONCOLUMNS.rlnClassNumber.value,
                      RELIONCOLUMNS.rlnAnglePsi.value
-]
+                     ]
 
 # COOR_EXTRA_LABELS = [ # Additional autopicking-related metadata
 #     md.RLN_PARTICLE_AUTOPICK_FOM,
 #     md.RLN_PARTICLE_CLASS,
 #     md.RLN_ORIENT_PSI
 # ]
 
@@ -515,10 +519,11 @@
 
 ALIGNMENT_DICT = {
     "_rlnOriginX": RELIONCOLUMNS.rlnOriginX.value,
     "_rlnOriginY": RELIONCOLUMNS.rlnOriginY.value,
     "_rlnOriginZ": RELIONCOLUMNS.rlnOriginZ.value,
     "_rlnAngleRot": RELIONCOLUMNS.rlnAngleRot.value,
     "_rlnAngleTilt": RELIONCOLUMNS.rlnAngleTilt.value,
-    "_rlnAnglePsi": RELIONCOLUMNS.rlnAnglePsi.value}
-
-
+    "_rlnAnglePsi": RELIONCOLUMNS.rlnAnglePsi.value,
+    "_rlnOriginXAngst": RELIONCOLUMNS.rlnOriginXAngst.value,
+    "_rlnOriginYAngst": RELIONCOLUMNS.rlnOriginYAngst.value,
+    "_rlnOriginZAngst": RELIONCOLUMNS.rlnOriginZAngst.value}
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/convert/__init__.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/convert/convert.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/convert/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,46 +370,42 @@
     else:
         fn = vol.getFileName()
     return fn
 
 
 def createItemMatrix(item, row, align):
     item.setCTF(rowToCtfModel(row))
-    item.setTransform(rowToAlignment(row, alignType=align))
+    pixelSize = item.getSamplingRate()
+    item.setTransform(rowToAlignment(row, align, pixelSize))
 
 
-def rowToAlignment(alignmentRow, alignType):
+def rowToAlignment(alignmentRow, alignType, pixelSize=1.0):
     """
     is2D == True-> matrix is 2D (2D images alignment)
             otherwise matrix is 3D (3D volume alignment or projection)
     invTransform == True  -> for xmipp implies projection
     """
     if alignType == ALIGN_3D:
         raise Exception("3D alignment conversion for Relion not implemented.")
 
     is2D = alignType == ALIGN_2D
     inverseTransform = alignType == ALIGN_PROJ
     if alignmentRow.hasAnyColumn(ALIGNMENT_DICT.values()):
         alignment = Transform()
         angles = np.zeros(3)
         shifts = np.zeros(3)
-        shifts[0] = alignmentRow.get(RELIONCOLUMNS.rlnOriginX.value, default=0.)
-        shifts[1] = alignmentRow.get(RELIONCOLUMNS.rlnOriginY.value, default=0.)
+        shifts[0] = alignmentRow.get(RELIONCOLUMNS.rlnOriginXAngst.value, default=0.)/pixelSize
+        shifts[1] = alignmentRow.get(RELIONCOLUMNS.rlnOriginYAngst.value, default=0.)/pixelSize
         if not is2D:
-            angles[0] = alignmentRow.get(RELIONCOLUMNS.rlnAngleRot.value,
-                                         default=0.)
-            angles[1] = alignmentRow.get(RELIONCOLUMNS.rlnAngleTilt.value,
-                                         default=0.)
-            angles[2] = alignmentRow.get(RELIONCOLUMNS.rlnAnglePsi.value,
-                                         default=0.)
-            shifts[2] = alignmentRow.get(RELIONCOLUMNS.rlnOriginZ.value,
-                                         default=0.)
+            angles[0] = alignmentRow.get(RELIONCOLUMNS.rlnAngleRot.value, default=0.)
+            angles[1] = alignmentRow.get(RELIONCOLUMNS.rlnAngleTilt.value, default=0.)
+            angles[2] = alignmentRow.get(RELIONCOLUMNS.rlnAnglePsi.value, default=0.)
+            shifts[2] = alignmentRow.get(RELIONCOLUMNS.rlnOriginZAngst.value, default=0.)/pixelSize
         else:
-            angles[2] = - alignmentRow.get(RELIONCOLUMNS.rlnAnglePsi.value,
-                                           default=0.)
+            angles[2] = - alignmentRow.get(RELIONCOLUMNS.rlnAnglePsi.value, default=0.)
         M = matrixFromGeometry(shifts, angles, inverseTransform)
         alignment.setMatrix(M)
     else:
         alignment = None
 
     return alignment
 
@@ -533,27 +529,25 @@
     return filesDict
 
 
 def writeSetOfParticles(imgSet, fileName, extraPath):
     args = {'outputDir': extraPath,
             'fillMagnification': True,
             'fillRandomSubset': True}
-
-    if imgSet.hasAlignmentProj() and imgSet.getAttributeValue(
-            "_rlnRandomSubset") is None:
-        args['postprocessImageRow'] = addRandomSubset
     try:
         logger.info('Trying to generate the star file with Relion convert...')
         from relion import convert
         alignType = ALIGN_PROJ if imgSet.hasAlignmentProj() else ALIGN_NONE
         args['alignType'] = alignType
         args['incompatibleExtensions'] = ['hdf', 'stk']
         convert.writeSetOfParticles(imgSet, fileName, **args)
         logger.info('The star file was generate successfully ...')
     except Exception:
+        if imgSet.hasAlignmentProj() and imgSet.getAttributeValue("_rlnRandomSubset") is None:
+            args['postprocessImageRow'] = addRandomSubset
         logger.info('The star file generation with Relion convert failed ...')
         logger.info('Trying to generate the star file with cryoSPARC convert ...')
         cryosPARCwriteSetOfParticles(imgSet, fileName, **args)
         logger.info('The star file was generate successfully ...')
 
 
 def cryosPARCwriteSetOfParticles(imgSet, starFile, outputDir, **kwargs):
@@ -659,15 +653,16 @@
         img.setCTF(rowToCtfModel(partRow))
 
     # alignment is mandatory at this point, it should be check
     # and detected defaults if not passed at readSetOf.. level
     alignType = kwargs.get('alignType')
 
     if alignType != ALIGN_NONE:
-        img.setTransform(rowToAlignment(partRow, alignType))
+        samplingRate = kwargs.get('samplingRate')
+        img.setTransform(rowToAlignment(partRow, alignType, samplingRate))
 
     if kwargs.get('readAcquisition', True):
         img.setAcquisition(rowToAcquisition(partRow))
 
     if kwargs.get('magnification', None):
         img.getAcquisition().setMagnification(kwargs.get("magnification"))
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/convert/cs2Start.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/convert/cs2Start.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import argparse
 import sys
-import re
 import json
 import os
 
 
 def cs2Star(args):
     from glob import glob
     import pandas as pd
@@ -66,15 +65,15 @@
                     [f for f in fields if f in data_general]])
             return 0
 
         try:
             df = metadata.parse_cryosparc_2_cs(cs, passthroughs=args.input[1:],
                                                minphic=args.minphic,
                                                boxsize=args.boxsize,
-                                               swapxy=args.swapxy,
+                                               swapxy=args.noswapxy,
                                                invertx=args.invertx,
                                                inverty=args.inverty)
         except (KeyError, ValueError) as e:
             log.error(e, exc_info=True)
             log.error("Required fields could not be mapped. Are you using the "
                       "right input file(s)?")
             return 1
@@ -92,26 +91,27 @@
         df = star.select_classes(df, args.cls)
 
     if args.flipy:
         log.info("Flipping refined shifts in Y")
         df[star.Relion.ORIGINY] = -df[star.Relion.ORIGINY]
         log.info("Flipping particle orientation through XZ plane")
         df = star.transform_star(df,
-                                 np.array([[1, 0, 0], [0, -1, 0], [0, 0, -1]]))
+                                 np.array([[1, 0, 0], [0, -1, 0], [0, 0, -1]]),
+                                 leftmult=True)
 
     if args.strip_uid is not None:
         df = star.strip_path_uids(df, inplace=True, count=args.strip_uid)
 
     if args.copy_micrograph_coordinates is not None:
         df = star.augment_star_ucsf(df, inplace=True)
         coord_star = pd.concat(
             (star.parse_star(inp, keep_index=False, augment=True) for inp in
              glob(args.copy_micrograph_coordinates)), join="inner")
         key = star.merge_key(df, coord_star, threshold=0)
-        if key is None:
+        if key is None and not args.strip_uid:
             log.debug("Merge key not found, removing leading UIDs")
             df = star.strip_path_uids(df, inplace=True)
             key = star.merge_key(df, coord_star)
         log.debug("Coordinates merge key: %s" % key)
         if args.cached or key == star.Relion.IMAGE_NAME:
             fields = star.Relion.MICROGRAPH_COORDS
         else:
@@ -128,15 +128,18 @@
         df = star.replace_micrograph_path(df, args.micrograph_path,
                                           inplace=True)
 
     if args.transform is not None:
         r = np.array(json.loads(args.transform))
         df = star.transform_star(df, r, inplace=True)
 
-    #df = star.check_defaults(df, inplace=True)
+    try:
+        df = star.check_defaults(df, inplace=True)
+    except Exception as e:
+        print(e)
 
     if args.relion2:
         df = star.remove_new_relion31(df, inplace=True)
         star.write_star(args.output, df, resort_records=True, optics=False)
     else:
         df = star.remove_deprecated_relion2(df, inplace=True)
         # Changing NaN values. These values denote erroneous coordinates
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/convert/dataimport.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/convert/dataimport.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
             raise Exception("The .cs file has not been imported: %s" % e)
 
 
     def _fillDataFromIter(self, imgSet):
         outImgsFn = 'particles@' + self.protocol._getFileName('out_particles')
         readSetOfParticles(outImgsFn, imgSet,
                            postprocessImageRow=self._updateItem,
-                           alignType=ALIGN_PROJ)
+                           alignType=ALIGN_PROJ,
+                           samplingRate=imgSet.getSamplingRate())
 
     def _updateItem(self, item, row):
         index, file = item.getLocation()
         binaryPath = self.findImagesFrom(self._csFile, file)
         item.setLocation(index, binaryPath)
         item.setSamplingRate(self._pixelSize)
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/cryosparc2_logo.png` & `scipion-em-cryosparc2-4.0.7/cryosparc2/cryosparc2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/__init__.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_base.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryorefine.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryorefine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc2d.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,15 +355,16 @@
         clsSet.classifyItems(updateItemCallback=self._updateParticle,
                              updateClassCallback=self._updateClass,
                              itemDataIterator=emtable.Table.iterRows(
                                  xmpMd))  # relion style
 
     def _updateParticle(self, item, row):
         item.setClassId(row.get(RELIONCOLUMNS.rlnClassNumber.value))
-        item.setTransform(rowToAlignment(row, ALIGN_2D))
+        samplingRate = item.getSamplingRate()
+        item.setTransform(rowToAlignment(row, ALIGN_2D, samplingRate))
 
     def _updateClass(self, class2D):
         classId = class2D.getObjId()
         if classId in self._classesInfo:
             index, fn, row = self._classesInfo[classId]
             class2D.setAlignment2D()
             class2Drep = class2D.getRepresentative()
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_classification.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3D_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,16 @@
         clsSet.classifyItems(updateItemCallback=self._updateParticle,
                              updateClassCallback=self._updateClass,
                              itemDataIterator=emtable.Table.iterRows(xmpMd))
 
     def _updateParticle(self, item, row):
         if row.get(RELIONCOLUMNS.rlnAnglePsi.value):
             item.setClassId(row.get(RELIONCOLUMNS.rlnClassNumber.value))
-            item.setTransform(rowToAlignment(row, ALIGN_PROJ))
+            samplingRate = item.getSamplingRate()
+            item.setTransform(rowToAlignment(row, ALIGN_PROJ, samplingRate))
         else:
             item._appendItem = False
 
     def _updateClass(self, item):
         classId = item.getObjId()
         if classId in self._classesInfo:
             index, fn, row = self._classesInfo[classId]
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3d_variability.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3d_variability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_ab.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_ab.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,16 @@
                              itemDataIterator=emtable.Table.iterRows(outImgsFn))
 
     def _updateParticle(self, item, row):
         if row.hasColumn(RELIONCOLUMNS.rlnClassNumber.value):
             item.setClassId(row.get(RELIONCOLUMNS.rlnClassNumber.value))
         else:
             item.setClassId(1)
-        item.setTransform(rowToAlignment(row, ALIGN_PROJ))
+        samplingRate = item.getSamplingRate()
+        item.setTransform(rowToAlignment(row, ALIGN_PROJ, samplingRate))
 
     def _updateClass(self, item):
         classId = item.getObjId()
         if classId in self._classesInfo:
             index, fn, row = self._classesInfo[classId]
             fixVolume(fn)
             item.setAlignmentProj()
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,16 @@
         clsSet.classifyItems(updateItemCallback=self._updateParticle,
                              updateClassCallback=self._updateClass,
                              itemDataIterator=emtable.Table.iterRows(xmpMd))
 
     def _updateParticle(self, item, row):
         if row.get(RELIONCOLUMNS.rlnAnglePsi.value):
             item.setClassId(row.get(RELIONCOLUMNS.rlnClassNumber.value))
-            item.setTransform(rowToAlignment(row, ALIGN_PROJ))
+            samplingRate = item.getSamplingRate()
+            item.setTransform(rowToAlignment(row, ALIGN_PROJ, samplingRate))
         else:
             item._appendItem = False
 
     def _updateClass(self, item):
         classId = item.getObjId()
         if classId in self._classesInfo:
             index, fn, row = self._classesInfo[classId]
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,14 +261,16 @@
                                                      imgSet.getSamplingRate(),
                                                      imgSet.getDim()))
         vol.setHalfMaps([half1, half2])
 
         outImgSet = self._createSetOfParticles()
         outImgSet.copyInfo(imgSet)
         self._fillDataFromIter(outImgSet)
+        import time
+        time.sleep(10)
 
         self._defineOutputs(outputVolume=vol)
         self._defineSourceRelation(self.inputParticles.get(), vol)
         self._defineOutputs(outputParticles=outImgSet)
         self._defineTransformRelation(self.inputParticles.get(), outImgSet)
         self.createFSC(idd, imgSet, vol)
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_part_subtract.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_part_subtract.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,16 @@
 
         outImgsFn = 'particles@' + self._getFileName('out_particles')
         hasCtf = imgSet.hasCTF()
         hasAcquisition = True  # I think this is alway present ROB
         readSetOfParticles(outImgsFn, imgSet,
                            postprocessImageRow=self._updateItem,
                            alignType=ALIGN_PROJ, readCtf=hasCtf, 
-                           readAcquisition= hasAcquisition)
+                           readAcquisition=hasAcquisition,
+                           samplingRate=imgSet.getSamplingRate())
 
     def _updateItem(self, item, row):
         newFn = row.get(RELIONCOLUMNS.rlnImageName.value)
         index, file = cryosparcToLocation(newFn)
         item.setLocation((index, self._getExtraPath(file)))
         item.setSamplingRate(calculateNewSamplingRate(item.getDim(),
                                                       self._getInputParticles().getSamplingRate(),
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_sharppening.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_sharppening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,15 +138,16 @@
         self._defineOutputs(outputParticles=outImgSet)
         self._defineTransformRelation(imgSet, outImgSet)
 
     def _fillDataFromIter(self, imgSet):
         outImgsFn = 'particles@' + self._getFileName('out_particles')
         readSetOfParticles(outImgsFn, imgSet,
                            postprocessImageRow=self.updateParticlePath,
-                           alignType=imgSet.getAlignment())
+                           alignType=imgSet.getAlignment(),
+                           samplingRate=imgSet.getSamplingRate())
 
     # --------------------------- INFO functions -------------------------------
 
     def _validate(self):
         """ Should be overwritten in subclasses to
             return summary message for NORMAL EXECUTION.
         """
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols.conf` & `scipion-em-cryosparc2-4.0.7/cryosparc2/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/tests/__init__.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/tests/test_protocols_cryosparc2.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/tests/test_protocols_cryosparc2.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,17 +521,26 @@
             protNonUniform3DRefinement1.symmetryGroup.set(SYM_CYCLIC)
             protNonUniform3DRefinement1.symmetryOrder.set(1)
             protNonUniform3DRefinement1.compute_use_ssd.set(False)
             protNonUniform3DRefinement1.setObjLabel("protNonUniform3DRefinement_2")
             self.launchProtocol(protNonUniform3DRefinement1)
             self.assertIsNotNone(protNonUniform3DRefinement1.outputVolume)
 
+            unionProt = self.newProtocol(ProtUnionSet)
+            # Set the input volumes
+            unionProt.inputSets.append(protNonUniform3DRefinement.outputParticles)
+            unionProt.inputSets.append(protNonUniform3DRefinement1.outputParticles)
+            unionProt.setObjLabel("Single particles union")
+            self.launchProtocol(unionProt)
+            self.assertSetSize(unionProt.outputSet, 746,
+                               msg="Union of 2 set of particles does not work.")
+
             # Launch a 3D Heterogeneous Refinement protocol
             prot3DHeterogeneousRefinement = self.newProtocol(ProtCryoSparc3DClassification)
-            prot3DHeterogeneousRefinement.inputParticles.set(protNonUniform3DRefinement.outputParticles)
+            prot3DHeterogeneousRefinement.inputParticles.set(unionProt.outputSet)
             volumes = PointerList()
             volumes.append(protNonUniform3DRefinement.outputVolume)
             volumes.append(protNonUniform3DRefinement1.outputVolume)
             prot3DHeterogeneousRefinement.refVolumes.set(volumes)
             prot3DHeterogeneousRefinement.compute_use_ssd.set(False)
             self.launchProtocol(prot3DHeterogeneousRefinement)
 
@@ -592,16 +601,14 @@
             protParticlesSubtract.inputParticles.set(prot3DRefinement.outputParticles)
             protParticlesSubtract.refVolume.set(prot3DRefinement.outputVolume)
             protParticlesSubtract.refMask.set(protXmippCreate3DMask.outputMask)
             protParticlesSubtract.compute_use_ssd.set(False)
             self.launchProtocol(protParticlesSubtract)
 
             self.assertIsNotNone(protParticlesSubtract.outputParticles)
-            self.assertEqual(protParticlesSubtract.outputParticles.getSize(),
-                             prot3DRefinement.outputParticles.getSize())
 
         _runCryosparctestParticlesSubtract(label="Cryosparc Subtract projection")
 
 
 class TestCryosparcSharppening(TestCryosparcBase):
 
     @classmethod
@@ -856,15 +863,19 @@
             protLocalRefine.compute_use_ssd.set(False)
             self.launchProtocol(protLocalRefine)
 
             return protLocalRefine
 
         def _checkAsserts(cryosparcProt):
             self.assertIsNotNone(cryosparcProt.outputParticles,
-                                 "There was a problem with Cryosparc subtract projection")
+                                 "There was a problem with Cryosparc local refine")
+            transform = cryosparcProt.outputParticles.getFirstItem().getTransform()
+            shifts = transform.getShifts()
+            shiftsCeros = shifts[0] == shifts[1] == shifts[2] == 0
+            self.assertFalse(shiftsCeros, "The transform matrix must have shifts")
 
         cryosparcProtGpu = _runCryosparctestLocalRefine(label="Cryosparc Local Refine")
         _checkAsserts(cryosparcProtGpu)
 
 
 class TestCryosparcHomogeneousReconstruction(TestCryosparcBase):
 
@@ -895,15 +906,15 @@
             protHomogeneousReconst.refMask.set(self.protXmippCreate3DMask.outputMask)
             self.launchProtocol(protHomogeneousReconst)
 
             return protHomogeneousReconst
 
         def _checkAsserts(cryosparcProt):
             self.assertIsNotNone(cryosparcProt.outputParticles,
-                                 "There was a problem with Cryosparc subtract projection")
+                                 "There was a problem with Cryosparc Homogeneous Reconstruction")
 
         cryosparcProtGpu = _runCryosparctestHomogeneousReconstruction(label="Cryosparc Homogeneous Reconstruction")
         _checkAsserts(cryosparcProtGpu)
 
 
 class TestCryosparc3DClassification(TestCryosparcBase):
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/tests/test_utils.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import getpass
 import unittest
 from unittest.mock import patch
 
-from cryosparc2 import V_UNKNOWN
+from cryosparc2 import V_UNKNOWN, V3_0_0
 from cryosparc2.utils import (cryosparcValidate, cryosparcExists,
                               isCryosparcRunning, calculateNewSamplingRate,
                               getProjectName, getCryosparcVersion)
 
 import cryosparc2.utils as csutils
 
 class TestUtils(unittest.TestCase):
@@ -68,15 +68,15 @@
 
                     # Low version
                     getVersion.return_value = "1.0.0"
                     result = cryosparcValidate()
                     self.assertTrue('not compatible' in result[0], "Validation did not detect CS low version")
 
                     # Supported version
-                    getVersion.return_value = V2_14_2
+                    getVersion.return_value = V3_0_0
                     result = cryosparcValidate()
                     self.assertEqual(0, len(result), "Validation did not detectCS correct version.")
 
                     # Patch printing Warning function--> redStr
                     with patch('pyworkflow.utils.yellowStr') as yellowStr:
                         # Higher version
                         highV = "100.1.1"
```

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/utils.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/__init__.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_2Dclassify.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/viewer_2Dclassify.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_initialmodel.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/viewer_initialmodel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_partsubtract.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/viewer_partsubtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_refinement.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/viewers/viewer_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/cryosparc2/wizards.py` & `scipion-em-cryosparc2-4.0.7/cryosparc2/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/PKG-INFO` & `scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.6
+Version: 4.0.7
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -34,19 +34,20 @@
         * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
         * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
         * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
         
         **Latest plugin version**
         ==========================
         
-        **v4.0.6**
+        **v4.0.7**
         -----------
         * **new**     :  Compatibility with cryoSPARC v4.2.1
         * **new**        Plugin operation in a cluster
         * **fixed**      Fixed an installation error
+        * **fixed**      Fixed an error related with the calculation of the particles shifts
         
         **Installing the plugin**
         =========================
         
         In order to install the plugin follow these instructions:
         
         1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/SOURCES.txt` & `scipion-em-cryosparc2-4.0.7/scipion_em_cryosparc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.6/setup.py` & `scipion-em-cryosparc2-4.0.7/setup.py`

 * *Files identical despite different names*

