# Comparing `tmp/sdcflows-2.4.3.tar.gz` & `tmp/sdcflows-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdcflows-2.4.3.tar", last modified: Mon Apr 24 13:11:49 2023, max compression
+gzip compressed data, was "sdcflows-2.5.0.tar", last modified: Thu Jun  1 18:35:06 2023, max compression
```

## Comparing `sdcflows-2.4.3.tar` & `sdcflows-2.5.0.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/.maint/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1594 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/CONTRIBUTORS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/FORMER.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1146 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/MAINTAINERS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/PIs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/ROADMAP.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9457 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/update_authors.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1174 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/update_requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22205 2023-04-24 13:11:30.000000 sdcflows-2.4.3/CHANGES.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-04-24 13:11:30.000000 sdcflows-2.4.3/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-04-24 13:11:30.000000 sdcflows-2.4.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-04-24 13:11:30.000000 sdcflows-2.4.3/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-04-24 13:11:30.000000 sdcflows-2.4.3/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-24 13:11:49.588117 sdcflows-2.4.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2023-04-24 13:11:30.000000 sdcflows-2.4.3/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      218 2023-04-24 13:11:30.000000 sdcflows-2.4.3/min-requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-04-24 13:11:30.000000 sdcflows-2.4.3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-04-24 13:11:30.000000 sdcflows-2.4.3/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/sdcflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      502 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/sdcflows/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3266 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/cli/find_estimators.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/sdcflows/cli/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/cli/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3464 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/cli/tests/test_find_estimators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3011 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.536116 sdcflows-2.4.3/sdcflows/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/affine.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.536116 sdcflows-2.4.3/sdcflows/data/flirtsch/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_1.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_2.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_4.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_quick.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/fmap-any_registration.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/fmap-any_registration_testing.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)  5801500 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/fmap_atlas.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/fmap_atlas_2_MNI152NLin2009cAsym_affine.mat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      960 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/sd_syn.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/sd_syn_sloppy.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/translation_rigid.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17569 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/fieldmaps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.540116 sdcflows-2.4.3/sdcflows/interfaces/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/brainmask.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23807 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/bspline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4440 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/epi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6852 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/fmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5483 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/reportlets.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.540116 sdcflows-2.4.3/sdcflows/interfaces/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4506 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_bspline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1482 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_epi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_fmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1770 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_reportlets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4243 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18032 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.544116 sdcflows-2.4.3/sdcflows/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.544116 sdcflows-2.4.3/sdcflows/tests/data/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.548116 sdcflows-2.4.3/sdcflows/tests/data/dsA/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.520116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.548116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/anat/sub-01_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.552116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.556116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.560116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.560116 sdcflows-2.4.3/sdcflows/tests/data/dsB/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      270 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.520116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.520116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.560116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.564116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.568116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      317 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.568116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.568116 sdcflows-2.4.3/sdcflows/tests/data/dsC/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.524116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.568116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/anat/sub-01_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.572116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.580116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.580116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/task-rest_bold.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1954195 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/field-coeff-tests.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29820 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/topup-coeff-fixed.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29726 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/topup-coeff.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)  2210404 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/topup-field.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11243 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/test_fieldmaps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6003 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/test_transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2110 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/test_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16934 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/transform.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.580116 sdcflows-2.4.3/sdcflows/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6762 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/bimap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10294 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/epimanip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5069 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/phasemanip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.580116 sdcflows-2.4.3/sdcflows/utils/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1460 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/test_misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/test_phasemanip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1214 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/test_tools.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7232 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/test_wrangler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7852 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tools.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21284 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/wrangler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.584117 sdcflows-2.4.3/sdcflows/viz/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/viz/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4092 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/viz/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.584117 sdcflows-2.4.3/sdcflows/workflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3747 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/ancillary.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.584117 sdcflows-2.4.3/sdcflows/workflows/apply/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6544 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/correction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/registration.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.584117 sdcflows-2.4.3/sdcflows/workflows/apply/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30980 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5277 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/tests/test_correction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4362 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/tests/test_registration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6275 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/sdcflows/workflows/fit/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13253 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/fieldmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16449 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/pepolar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24995 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/syn.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/sdcflows/workflows/fit/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1727 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_fit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_pepolar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3946 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_phdiff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6807 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_syn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9632 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/outputs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/sdcflows/workflows/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/tests/test_ancillary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/tests/test_base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/sdcflows.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10864 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2336 2023-04-24 13:11:49.592116 sdcflows-2.4.3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-04-24 13:11:30.000000 sdcflows-2.4.3/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/tools/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-04-24 13:11:30.000000 sdcflows-2.4.3/tools/cache_templateflow.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.055788 sdcflows-2.5.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.007788 sdcflows-2.5.0/.maint/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1594 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/CONTRIBUTORS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/FORMER.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/MAINTAINERS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/PIs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/ROADMAP.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9457 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/update_authors.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1174 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/update_requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23275 2023-06-01 18:34:46.000000 sdcflows-2.5.0/CHANGES.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-06-01 18:34:46.000000 sdcflows-2.5.0/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-01 18:34:46.000000 sdcflows-2.5.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-06-01 18:34:46.000000 sdcflows-2.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-06-01 18:34:46.000000 sdcflows-2.5.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-06-01 18:35:06.055788 sdcflows-2.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2023-06-01 18:34:46.000000 sdcflows-2.5.0/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      218 2023-06-01 18:34:46.000000 sdcflows-2.5.0/min-requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-06-01 18:34:46.000000 sdcflows-2.5.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-06-01 18:34:46.000000 sdcflows-2.5.0/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.007788 sdcflows-2.5.0/sdcflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      502 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.007788 sdcflows-2.5.0/sdcflows/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3266 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/cli/find_estimators.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.011788 sdcflows-2.5.0/sdcflows/cli/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/cli/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3464 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/cli/tests/test_find_estimators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3011 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.015788 sdcflows-2.5.0/sdcflows/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/affine.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.019788 sdcflows-2.5.0/sdcflows/data/flirtsch/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_1.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_2.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_4.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_quick.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/fmap-any_registration.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/fmap-any_registration_testing.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  5801500 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/fmap_atlas.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/fmap_atlas_2_MNI152NLin2009cAsym_affine.mat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      960 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/sd_syn.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/sd_syn_sloppy.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/translation_rigid.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17569 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/fieldmaps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.019788 sdcflows-2.5.0/sdcflows/interfaces/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/brainmask.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23807 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/bspline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4440 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/epi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13361 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/fmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5483 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/reportlets.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.023788 sdcflows-2.5.0/sdcflows/interfaces/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4506 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_bspline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1482 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_epi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_fmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1770 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_reportlets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4243 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18032 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.023788 sdcflows-2.5.0/sdcflows/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.027788 sdcflows-2.5.0/sdcflows/tests/data/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.027788 sdcflows-2.5.0/sdcflows/tests/data/dsA/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.003788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.027788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/anat/sub-01_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.031788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.035788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.035788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.035788 sdcflows-2.5.0/sdcflows/tests/data/dsB/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      270 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.003788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.003788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.039788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.039788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.043788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      317 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.043788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.043788 sdcflows-2.5.0/sdcflows/tests/data/dsC/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.003788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.043788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/anat/sub-01_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.047788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.047788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.047788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/task-rest_bold.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1954195 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/field-coeff-tests.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29820 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/topup-coeff-fixed.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29726 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/topup-coeff.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2210404 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/topup-field.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11243 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/test_fieldmaps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6003 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/test_transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2110 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/test_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16934 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/transform.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6762 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/bimap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10294 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/epimanip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5069 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/phasemanip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/utils/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1460 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/test_misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/test_phasemanip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4293 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/test_tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9248 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/test_wrangler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10357 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22975 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/wrangler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/viz/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/viz/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4092 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/viz/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/workflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3747 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/ancillary.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/workflows/apply/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6544 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/correction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/registration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/workflows/apply/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30980 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5277 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/tests/test_correction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4362 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/tests/test_registration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6275 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/workflows/fit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/fieldmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16449 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/pepolar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24995 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/syn.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.055788 sdcflows-2.5.0/sdcflows/workflows/fit/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1727 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_fit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_pepolar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3946 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_phdiff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6807 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_syn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9632 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/outputs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.055788 sdcflows-2.5.0/sdcflows/workflows/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/tests/test_ancillary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/tests/test_base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.007788 sdcflows-2.5.0/sdcflows.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10864 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2336 2023-06-01 18:35:06.055788 sdcflows-2.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-06-01 18:34:46.000000 sdcflows-2.5.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.055788 sdcflows-2.5.0/tools/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-06-01 18:34:46.000000 sdcflows-2.5.0/tools/cache_templateflow.py
```

### Comparing `sdcflows-2.4.3/.maint/CONTRIBUTORS.md` & `sdcflows-2.5.0/.maint/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/.maint/FORMER.md` & `sdcflows-2.5.0/.maint/FORMER.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/.maint/MAINTAINERS.md` & `sdcflows-2.5.0/.maint/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/.maint/PIs.md` & `sdcflows-2.5.0/.maint/PIs.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/.maint/ROADMAP.md` & `sdcflows-2.5.0/.maint/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/.maint/update_authors.py` & `sdcflows-2.5.0/.maint/update_authors.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/.maint/update_requirements.py` & `sdcflows-2.5.0/.maint/update_requirements.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/CHANGES.rst` & `sdcflows-2.5.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+2.5.0 (June 01, 2023)
+=====================
+New feature release in the 2.5.x series.
+
+This release includes a number of changes to default behaviors.
+SyN-SDC will be performed per-BOLD/DWI image, unless specified otherwise with
+``B0FieldIdentifier``\s, and may now be specified with T2w images as anatomical
+references as well.
+Additionally, PEPolar fieldmaps will only be grouped if they share ``IntendedFor``
+metadata.
+
+Finally, as a small UX improvement, if magnitude1/magnitude2 images have differing
+affines but are in register, we will now copy the header rather than requiring the
+user to update the header themselves.
+
+* FIX: Ensure IntendedFor metadata is a subject-relative path (#360)
+* ENH: Split SyN fieldmap estimates per-EPI (#312)
+* ENH: Allow non-T1w anatomical estimators (#358)
+* ENH: Function to calculate reference grids aligned with the coefficients (#355)
+* ENH: Check registration of magnitude1/magnitude2 images and update headers (#356)
+* RF: Split PEPolar fieldmaps by intent, if available (#342)
+* CI: Use supported codecov uploaders (#348)
+
 2.4.3 (April 24, 2023)
 ======================
 Bug-fix release in the 2.4.x series.
 
 This fix resolves an inconsistency of treatment of phase-difference and
 scanner-calculated fieldmaps, relative to PEPolar and SyN. Fieldmaps in
 orientations other than RAS were impacted.
```

### Comparing `sdcflows-2.4.3/LICENSE` & `sdcflows-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/PKG-INFO` & `sdcflows-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdcflows
-Version: 2.4.3
+Version: 2.5.0
 Summary: Susceptibility Distortion Correction (SDC) workflows for EPI MR schemes.
 Home-page: https://www.nipreps.org/sdcflows
 Author: The SDCflows developers
 Author-email: nipreps@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.nipreps.org/sdcflows
 Project-URL: GitHub, https://github.com/nipreps/sdcflows
```

### Comparing `sdcflows-2.4.3/README.rst` & `sdcflows-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/cli/find_estimators.py` & `sdcflows-2.5.0/sdcflows/cli/find_estimators.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/cli/tests/test_find_estimators.py` & `sdcflows-2.5.0/sdcflows/cli/tests/test_find_estimators.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/conftest.py` & `sdcflows-2.5.0/sdcflows/conftest.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/affine.json` & `sdcflows-2.5.0/sdcflows/data/affine.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0.cnf` & `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_1.cnf` & `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_1.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_2.cnf` & `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_2.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_4.cnf` & `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_4.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_quick.cnf` & `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_quick.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/fmap-any_registration.json` & `sdcflows-2.5.0/sdcflows/data/fmap-any_registration.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/fmap-any_registration_testing.json` & `sdcflows-2.5.0/sdcflows/data/fmap-any_registration_testing.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/fmap_atlas.nii.gz` & `sdcflows-2.5.0/sdcflows/data/fmap_atlas.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/sd_syn.json` & `sdcflows-2.5.0/sdcflows/data/sd_syn.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/sd_syn_sloppy.json` & `sdcflows-2.5.0/sdcflows/data/sd_syn_sloppy.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/data/translation_rigid.json` & `sdcflows-2.5.0/sdcflows/data/translation_rigid.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/fieldmaps.py` & `sdcflows-2.5.0/sdcflows/fieldmaps.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/brainmask.py` & `sdcflows-2.5.0/sdcflows/interfaces/brainmask.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/bspline.py` & `sdcflows-2.5.0/sdcflows/interfaces/bspline.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/epi.py` & `sdcflows-2.5.0/sdcflows/interfaces/epi.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/reportlets.py` & `sdcflows-2.5.0/sdcflows/interfaces/reportlets.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/tests/test_bspline.py` & `sdcflows-2.5.0/sdcflows/interfaces/tests/test_bspline.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/tests/test_epi.py` & `sdcflows-2.5.0/sdcflows/interfaces/tests/test_epi.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/tests/test_fmap.py` & `sdcflows-2.5.0/sdcflows/interfaces/tests/test_fmap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/tests/test_reportlets.py` & `sdcflows-2.5.0/sdcflows/interfaces/tests/test_reportlets.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/tests/test_utils.py` & `sdcflows-2.5.0/sdcflows/interfaces/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/interfaces/utils.py` & `sdcflows-2.5.0/sdcflows/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/tests/data/epi.nii.gz` & `sdcflows-2.5.0/sdcflows/tests/data/epi.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/tests/data/field-coeff-tests.nii.gz` & `sdcflows-2.5.0/sdcflows/tests/data/field-coeff-tests.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/tests/data/topup-coeff-fixed.nii.gz` & `sdcflows-2.5.0/sdcflows/tests/data/topup-coeff-fixed.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/tests/data/topup-coeff.nii.gz` & `sdcflows-2.5.0/sdcflows/tests/data/topup-coeff.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/tests/data/topup-field.nii.gz` & `sdcflows-2.5.0/sdcflows/tests/data/topup-field.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/tests/test_fieldmaps.py` & `sdcflows-2.5.0/sdcflows/tests/test_fieldmaps.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/tests/test_transform.py` & `sdcflows-2.5.0/sdcflows/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/tests/test_version.py` & `sdcflows-2.5.0/sdcflows/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/transform.py` & `sdcflows-2.5.0/sdcflows/transform.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/utils/bimap.py` & `sdcflows-2.5.0/sdcflows/utils/bimap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/utils/epimanip.py` & `sdcflows-2.5.0/sdcflows/utils/epimanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/utils/misc.py` & `sdcflows-2.5.0/sdcflows/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/utils/phasemanip.py` & `sdcflows-2.5.0/sdcflows/utils/phasemanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/utils/tests/test_misc.py` & `sdcflows-2.5.0/sdcflows/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/utils/tests/test_phasemanip.py` & `sdcflows-2.5.0/sdcflows/utils/tests/test_phasemanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/utils/tests/test_wrangler.py` & `sdcflows-2.5.0/sdcflows/utils/tests/test_wrangler.py`

 * *Files 19% similar despite different names*

```diff
@@ -91,14 +91,51 @@
                     "metadata": {
                         "RepetitionTime": 0.8,
                         "TotalReadoutTime": 0.5,
                         "PhaseEncodingDirection": "j"
                     }
                 }
             ]
+        },
+        {
+            "session": "04",
+            "anat": [{"suffix": "T1w", "metadata": {"EchoTime": 1}}],
+            "fmap": [
+                {"suffix": "epi", "dir": "AP", "metadata": {
+                    "EchoTime": 1.2,
+                    "PhaseEncodingDirection": "j-",
+                    "TotalReadoutTime": 0.8,
+                    "IntendedFor": [
+                        "ses-04/func/sub-01_ses-04_task-rest_run-1_bold.nii.gz",
+                        "ses-04/func/sub-01_ses-04_task-rest_run-2_bold.nii.gz",
+                    ],
+                }},
+            ],
+            "func": [
+                {
+                    "task": "rest",
+                    "run": 1,
+                    "suffix": "bold",
+                    "metadata": {
+                        "RepetitionTime": 0.8,
+                        "TotalReadoutTime": 0.5,
+                        "PhaseEncodingDirection": "j"
+                    }
+                },
+                {
+                    "task": "rest",
+                    "run": 2,
+                    "suffix": "bold",
+                    "metadata": {
+                        "RepetitionTime": 0.8,
+                        "TotalReadoutTime": 0.5,
+                        "PhaseEncodingDirection": "j"
+                    }
+                },
+            ]
         }
     ]
 }
 
 
 phasediff = {
     "01": [
@@ -212,7 +249,24 @@
 def test_wrangler_filter(tmpdir, name, skeleton, estimations):
     bids_dir = str(tmpdir / name)
     generate_bids_skeleton(bids_dir, skeleton)
     layout = gen_layout(bids_dir)
     est = find_estimators(layout=layout, subject='01', bids_filters=filters['fmap'])
     assert len(est) == estimations
     clear_registry()
+
+
+def test_single_reverse_pedir(tmp_path):
+    bids_dir = tmp_path / "bids"
+    generate_bids_skeleton(bids_dir, pepolar)
+    layout = gen_layout(bids_dir)
+    est = find_estimators(layout=layout, subject='01', bids_filters={'session': '04'})
+    assert len(est) == 2
+    subject_root = bids_dir / 'sub-01'
+    for estimator in est:
+        assert len(estimator.sources) == 2
+        epi, bold = estimator.sources
+        # Just checking order
+        assert epi.entities['fmap'] == 'epi'
+        # IntendedFor is a list of strings
+        # REGRESSION: The result was a PyBIDS BIDSFile (fmriprep#3020)
+        assert epi.metadata['IntendedFor'] == [str(bold.path.relative_to(subject_root))]
```

### Comparing `sdcflows-2.4.3/sdcflows/utils/tools.py` & `sdcflows-2.5.0/sdcflows/utils/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,86 @@
 #
 # We support and encourage derived works from this project, please read
 # about our expectations at
 #
 #     https://www.nipreps.org/community/licensing/
 #
 """Image processing tools."""
+import nibabel as nb
+
+
+def deoblique_and_zooms(
+    in_reference: nb.spatialimages.SpatialImage,
+    oblique: nb.spatialimages.SpatialImage,
+    factor: int = 4,
+    padding: int = 1,
+    factor_tol: float = 1e-4,
+):
+    """
+    Generate a sampling reference aligned with in_reference fully covering oblique.
+
+    Parameters
+    ----------
+    in_reference : :obj:`~nibabel.spatialimages.SpatialImage`
+        The sampling reference.
+    oblique : :obj:`~nibabel.spatialimages.SpatialImage`
+        The rotated coordinate system whose extent should be fully covered by the
+        generated reference.
+    factor : :obj:`int`
+        A factor to increase the resolution of the generated reference.
+    padding : :obj:`int`
+        Number of additional voxels around the most extreme positions of the projection of
+        oblique on to the reference.
+    factor_tol : :obj:`float`
+        Absolute tolerance to determine whether factor is one.
+
+    """
+    from itertools import product
+    import numpy as np
+    from nibabel.affines import apply_affine, rescale_affine
+
+    # Reference space metadata
+    hdr = in_reference.header.copy()
+    affine = in_reference.affine.copy()
+    ref_shape = np.array(in_reference.shape[:3])
+    ref_zooms = np.array(hdr.get_zooms()[:3])
+    _, scode = in_reference.get_sform(coded=True)
+    _, qcode = in_reference.get_qform(coded=True)
+
+    # Calculate the 8 most extreme coordinates of oblique in in_reference space
+    corners = np.array(list(product((0, 1), repeat=3))) * (
+        np.array(oblique.shape[:3]) - 1
+    )
+    extent_ijk = apply_affine(np.linalg.inv(affine) @ oblique.affine, corners)
+
+    underflow = np.clip(extent_ijk.min(0) - padding, None, 0).astype(int)
+    overflow = np.ceil(
+        np.clip(extent_ijk.max(0) + padding + 1 - ref_shape, 0, None)
+    ).astype(int)
+    if np.any(underflow < 0) or np.any(overflow > 0):
+        # Add under/overflow voxels
+        ref_shape += overflow - underflow
+        # Consistently update origin
+        affine[:-1, -1] = apply_affine(affine, underflow)
+
+    # Make grid denser
+    if abs(1.0 - factor) > factor_tol:
+        new_shape = np.rint(ref_shape * factor)
+        affine = rescale_affine(affine, ref_shape, ref_zooms / factor, new_shape)
+        ref_shape = new_shape
+
+    # Generate new reference
+    hdr.set_sform(affine, scode)
+    hdr.set_qform(affine, qcode)
+
+    return in_reference.__class__(
+        nb.fileslice.strided_scalar(ref_shape.astype(int)),
+        affine,
+        hdr,
+    )
 
 
 def resample_to_zooms(in_file, zooms, order=3, prefilter=True):
     """Resample the input data to a new grid with the requested zooms."""
     from pathlib import Path
     import numpy as np
     import nibabel as nb
```

### Comparing `sdcflows-2.4.3/sdcflows/utils/wrangler.py` & `sdcflows-2.5.0/sdcflows/utils/wrangler.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     layout: BIDSLayout,
     subject: str,
     sessions: Optional[List[str]] = None,
     fmapless: Union[bool, set] = True,
     force_fmapless: bool = False,
     logger: Optional[logging.Logger] = None,
     bids_filters: Optional[dict] = None,
+    anat_suffix: Union[str, List[str]] = 'T1w',
 ) -> list:
     """
     Apply basic heuristics to automatically find available data for fieldmap estimation.
 
     The "*fieldmap-less*" heuristics only attempt to find ``_dwi`` and ``_bold`` candidates
     to pair with a ``_T1w`` anatomical reference.
     For more complicated heuristics (for instance, using ``_T2w`` images or ``_sbref``
@@ -69,14 +70,17 @@
         When some other fieldmap estimation methods have been found, fieldmap-less
         estimation will be skipped except if ``force_fmapless`` is ``True``.
     logger
         The logger used to relay messages. If not provided, one will be created.
     bids_filters
         Optional dictionary of key/values to filter the entities on.
         This allows lower level file inclusion/exclusion.
+    anat_suffix : :obj:`str` or :obj:`list`
+        String or list of strings to filter anatomical images for fieldmap-less
+        approaches. If not provided, ``T1w`` is used.
 
     Returns
     -------
     estimators : :obj:`list`
         The list of :py:class:`~sdcflows.fieldmaps.FieldmapEstimation` objects that have
         successfully been built (meaning, all necessary inputs and corresponding metadata
         are present in the given layout.)
@@ -125,15 +129,17 @@
     >>> find_estimators(
     ...     layout=layouts['HCP101006'],
     ...     subject="101006",
     ... )  # doctest: +ELLIPSIS
     [FieldmapEstimation(sources=<2 files>, method=<EstimatorType.PHASEDIFF: 3>,
                         bids_id='auto_00006'),
      FieldmapEstimation(sources=<2 files>, method=<EstimatorType.PEPOLAR: 2>,
-                        bids_id='auto_00007')]
+                        bids_id='auto_00007'),
+     FieldmapEstimation(sources=<2 files>, method=<EstimatorType.PEPOLAR: 2>,
+                        bids_id='auto_00008')]
 
     Finally, *SDCFlows*' "*dataset A*" and "*dataset B*" contain BIDS structures
     with zero-byte NIfTI files and some corresponding metadata:
 
     >>> find_estimators(
     ...     layout=layouts['dsA'],
     ...     subject="01",
@@ -172,33 +178,45 @@
     >>> find_estimators(
     ...     layout=layouts['ds000054'],
     ...     subject="100185",
     ...     fmapless={"bold"},
     ...     force_fmapless=True,
     ... )  # doctest: +ELLIPSIS
     [FieldmapEstimation(sources=<3 files>, method=<EstimatorType.PHASEDIFF: 3>,
-                        bids_id='auto_00000'),
-     FieldmapEstimation(sources=<3 files>, method=<EstimatorType.ANAT: 5>,
-                        bids_id='auto_00001')]
+                        bids_id='auto_...'),
+     FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
+                        bids_id='auto_...'),
+     FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
+                        bids_id='auto_...')]
 
     Likewise in a more comprehensive dataset:
 
     >>> find_estimators(
     ...     layout=layouts['ds001771'],
     ...     subject="36",
     ...     force_fmapless=True,
     ... )  # doctest: +ELLIPSIS
     [FieldmapEstimation(sources=<4 files>, method=<EstimatorType.PEPOLAR: 2>,
-                       bids_id='auto_00002'),
-    FieldmapEstimation(sources=<7 files>, method=<EstimatorType.ANAT: 5>,
-                       bids_id='auto_00003'),
+                       bids_id='auto_...'),
+    FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
+                       bids_id='auto_...'),
+    FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
+                       bids_id='auto_...'),
+    FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
+                       bids_id='auto_...'),
+    FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
+                       bids_id='auto_...'),
+    FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
+                       bids_id='auto_...'),
     FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
-                       bids_id='auto_00004'),
+                       bids_id='auto_...'),
     FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
-                       bids_id='auto_00005')]
+                       bids_id='auto_...'),
+    FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
+                       bids_id='auto_...')]
 
     Because "*dataset A*" contains very few metadata fields available, "*fieldmap-less*"
     heuristics come back empty (BOLD and DWI files are missing
     the mandatory ``PhaseEncodingDirection``, in this case):
 
     >>> find_estimators(
     ...     layout=layouts['dsA'],
@@ -229,17 +247,17 @@
     >>> find_estimators(
     ...     layout=layouts['ds000206'],
     ...     subject="05",
     ...     fmapless=True,
     ...     force_fmapless=False,
     ... )  # doctest: +ELLIPSIS
     [FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
-                        bids_id='auto_00011'),
+                        bids_id='auto_...'),
     FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
-                       bids_id='auto_00012')]
+                       bids_id='auto_...')]
 
     When the ``B0FieldIdentifier`` metadata is set for one or more fieldmaps, then
     the heuristics that use ``IntendedFor`` are dismissed:
 
     >>> find_estimators(
     ...     layout=layouts['dsC'],
     ...     subject="01",
@@ -256,15 +274,15 @@
     ...     subject="01",
     ...     fmapless=True,
     ...     force_fmapless=True,
     ... )  # doctest: +ELLIPSIS
     [FieldmapEstimation(sources=<5 files>, method=<EstimatorType.PEPOLAR: 2>,
                         bids_id='pepolar4pe'),
     FieldmapEstimation(sources=<2 files>, method=<EstimatorType.ANAT: 5>,
-                       bids_id='auto_00000')]
+                       bids_id='auto_...')]
 
     """
     from .misc import create_logger
     from bids.layout import Query
     from bids.exceptions import BIDSEntityError
 
     # The created logger is set to ERROR log level
@@ -365,29 +383,30 @@
         for ses, acq, ce in product(sessions, acqs, contrasts):
             entities = base_entities.copy()
             entities.update(
                 {"suffix": "epi", "session": ses, "acquisition": acq, "ceagent": ce}
             )
             dirs = layout.get_directions(**entities)
             if len(dirs) > 1:
-                fieldmaps = layout.get(**{**entities, **{"direction": dirs}})
-                try:
-                    e = fm.FieldmapEstimation(
-                        [
-                            fm.FieldmapFile(fmap.path, metadata=fmap.get_metadata())
-                            for fmap in fieldmaps
-                        ]
-                    )
-                except ValueError as err:
-                    _log_debug_estimator_fail(
-                        logger, "unnamed PEPOLAR", fieldmaps, layout.root, str(err)
-                    )
-                else:
-                    _log_debug_estimation(logger, e, layout.root)
-                    estimators.append(e)
+                by_intent = {}
+                for fmap in layout.get(**{**entities, **{'direction': dirs}}):
+                    fmapfile = fm.FieldmapFile(fmap.path, metadata=fmap.get_metadata())
+                    by_intent.setdefault(
+                        tuple(fmapfile.metadata.get('IntendedFor', ())), []
+                    ).append(fmapfile)
+                for collection in by_intent.values():
+                    try:
+                        e = fm.FieldmapEstimation(collection)
+                    except (ValueError, TypeError) as err:
+                        _log_debug_estimator_fail(
+                            logger, "unnamed PEPOLAR", collection, layout.root, str(err)
+                        )
+                    else:
+                        _log_debug_estimation(logger, e, layout.root)
+                        estimators.append(e)
 
         # At this point, only single-PE _epi files WITH ``IntendedFor`` can
         # be automatically processed.
         has_intended = tuple()
         with suppress(ValueError):
             has_intended = layout.get(
                 **{
@@ -400,31 +419,54 @@
             if epi_fmap.path in fm._estimators.sources:
                 logger.debug("Skipping fieldmap %s (already in use)", epi_fmap.relpath)
                 continue  # skip EPI images already considered above
 
             logger.debug("Found single PE fieldmap %s", epi_fmap.relpath)
             epi_base_md = epi_fmap.get_metadata()
 
-            # There are two possible interpretations of an IntendedFor list:
-            # 1) The fieldmap and each intended target are combined separately
-            # 2) The fieldmap and all intended targets are combined at once
-            #
-            # (1) has been the historical interpretation of NiPreps,
-            # so construct a separate estimator for each target.
+            # Find existing IntendedFor targets and warn if missing
+            all_targets = []
             for intent in listify(epi_base_md["IntendedFor"]):
                 target = layout.get_file(str(subject_root / intent))
                 if target is None:
                     logger.debug("Single PE target %s not found", intent)
                     continue
+                all_targets.append(target)
+
+            # If sbrefs are targets, then the goal is generally to estimate with epi+sbref
+            # and correct bold/dwi
+            sbrefs = [
+                target for target in all_targets if target.entities["suffix"] == "sbref"
+            ]
+            if sbrefs:
+                targets = sbrefs
+                intent_map = []
+                for sbref in sbrefs:
+                    ents = sbref.entities.copy()
+                    ents["suffix"] = ["bold", "dwi"]
+                    intent_map.append(
+                        [
+                            target
+                            for target in layout.get(**ents)
+                            if target in all_targets
+                        ]
+                    )
+            else:
+                targets = all_targets
+                intent_map = [[target] for target in all_targets]
 
+            for target, intent in zip(targets, intent_map):
                 logger.debug("Found single PE target %s", target.relpath)
                 # The new estimator is IntendedFor the individual targets,
                 # even if the EPI file is IntendedFor multiple
                 estimator_md = epi_base_md.copy()
-                estimator_md["IntendedFor"] = [intent]
+                estimator_md["IntendedFor"] = [
+                    str(Path(pathlike).relative_to(subject_root))
+                    for pathlike in intent
+                ]
                 try:
                     e = fm.FieldmapEstimation(
                         [
                             fm.FieldmapFile(epi_fmap.path, metadata=estimator_md),
                             fm.FieldmapFile(target.path, metadata=target.get_metadata())
                         ]
                     )
@@ -440,15 +482,15 @@
                     _log_debug_estimation(logger, e, layout.root)
                     estimators.append(e)
 
     if estimators and not force_fmapless:
         fmapless = False
 
     # Find fieldmap-less schemes
-    anat_file = layout.get(**{**base_entities, **{'suffix': 'T1w', 'session': sessions}})
+    anat_file = layout.get(**{**base_entities, **{'suffix': anat_suffix, 'session': sessions}})
 
     if not fmapless or not anat_file:
         logger.debug("Skipping fmap-less estimation")
         return estimators
 
     logger.debug("Attempting fmap-less estimation")
     from .epimanip import get_trt
@@ -472,36 +514,31 @@
             ro = 1.0
             with suppress(ValueError):
                 ro = get_trt(meta, candidate.path)
             ro_totals.append(ro)
             meta.update({"TotalReadoutTime": ro})
             epi_targets.append(fm.FieldmapFile(candidate.path, metadata=meta))
 
-        for pe_dir in sorted(set(pe_dirs)):
-            pe_ro = [ro for ro, pe in zip(ro_totals, pe_dirs) if pe == pe_dir]
-            for ro_time in sorted(set(pe_ro)):
-                fmfiles, fmpaths = tuple(
-                    zip(
-                        *[
-                            (target, str(Path(target.path).relative_to(subject_root)))
-                            for i, target in enumerate(epi_targets)
-                            if pe_dirs[i] == pe_dir and ro_totals[i] == ro_time
-                        ]
-                    )
-                )
-                e = fm.FieldmapEstimation(
-                    [
-                        fm.FieldmapFile(
-                            anat_file[0], metadata={"IntendedFor": fmpaths}
-                        ),
-                        *fmfiles,
-                    ]
-                )
-                _log_debug_estimation(logger, e, layout.root)
-                estimators.append(e)
+        trivial_estimators = [
+            [
+                fm.FieldmapFile(
+                    anat_file[0],
+                    metadata={"IntendedFor": str(Path(epi.path).relative_to(subject_root))},
+                ),
+                epi,
+            ] for epi in epi_targets
+        ]
+
+        # TODO: Grouping could be done here; previously we grouped by (pe_dir, ro_time) pairs
+        syn_estimators = [fm.FieldmapEstimation(e) for e in trivial_estimators]
+
+        for e in syn_estimators:
+            _log_debug_estimation(logger, e, layout.root)
+
+        estimators.extend(syn_estimators)
 
     return estimators
 
 
 def _log_debug_estimation(
     logger: logging.Logger,
     estimation: fm.FieldmapEstimation,
```

### Comparing `sdcflows-2.4.3/sdcflows/viz/utils.py` & `sdcflows-2.5.0/sdcflows/viz/utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/ancillary.py` & `sdcflows-2.5.0/sdcflows/workflows/ancillary.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/apply/correction.py` & `sdcflows-2.5.0/sdcflows/workflows/apply/correction.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/apply/registration.py` & `sdcflows-2.5.0/sdcflows/workflows/apply/registration.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz` & `sdcflows-2.5.0/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/apply/tests/test_correction.py` & `sdcflows-2.5.0/sdcflows/workflows/apply/tests/test_correction.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/apply/tests/test_registration.py` & `sdcflows-2.5.0/sdcflows/workflows/apply/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/base.py` & `sdcflows-2.5.0/sdcflows/workflows/base.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/fit/fieldmap.py` & `sdcflows-2.5.0/sdcflows/workflows/fit/fieldmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,33 +86,49 @@
     """
     from ...interfaces.bspline import (
         BSplineApprox,
         DEFAULT_LF_ZOOMS_MM,
         DEFAULT_HF_ZOOMS_MM,
         DEFAULT_ZOOMS_MM,
     )
+    from ...interfaces.fmap import CheckRegister
 
     workflow = Workflow(name=name)
     inputnode = pe.Node(niu.IdentityInterface(fields=INPUT_FIELDS), name="inputnode")
     outputnode = pe.Node(
         niu.IdentityInterface(fields=["fmap", "fmap_ref", "fmap_mask", "fmap_coeff", "method"]),
         name="outputnode",
     )
 
+    def _unzip(fmap_spec):
+        return fmap_spec
+
+    unzip = pe.MapNode(
+        niu.Function(function=_unzip, output_names=["fmap_file", "meta"]),
+        run_without_submitting=True,
+        iterfield=["fmap_spec"],
+        name="unzip",
+    )
+
+    check_register = pe.Node(CheckRegister(), name='check_register')
+
     magnitude_wf = init_magnitude_wf(omp_nthreads=omp_nthreads)
     bs_filter = pe.Node(BSplineApprox(), name="bs_filter")
     bs_filter.interface._always_run = debug
     bs_filter.inputs.bs_spacing = (
         [DEFAULT_LF_ZOOMS_MM, DEFAULT_HF_ZOOMS_MM] if not sloppy else [DEFAULT_ZOOMS_MM]
     )
     bs_filter.inputs.extrapolate = not debug
 
     # fmt: off
     workflow.connect([
-        (inputnode, magnitude_wf, [("magnitude", "inputnode.magnitude")]),
+        (inputnode, unzip, [("fieldmap", "fmap_spec")]),
+        (inputnode, check_register, [("magnitude", "mag_files")]),
+        (unzip, check_register, [("fmap_file", "fmap_files")]),
+        (check_register, magnitude_wf, [("mag_files", "inputnode.magnitude")]),
         (magnitude_wf, bs_filter, [("outputnode.fmap_mask", "in_mask")]),
         (magnitude_wf, outputnode, [
             ("outputnode.fmap_mask", "fmap_mask"),
             ("outputnode.fmap_ref", "fmap_ref"),
         ]),
         (bs_filter, outputnode, [
             ("out_extrapolated" if not debug else "out_field", "fmap"),
@@ -127,15 +143,16 @@
 acquisitions.
 """
         phdiff_wf = init_phdiff_wf(omp_nthreads, debug=debug)
         outputnode.inputs.method = "FMB (fieldmap-based) - phase-difference map"
 
         # fmt: off
         workflow.connect([
-            (inputnode, phdiff_wf, [("fieldmap", "inputnode.phase")]),
+            (unzip, phdiff_wf, [("meta", "inputnode.phase_meta")]),
+            (check_register, phdiff_wf, [("fmap_files", "inputnode.phase")]),
             (magnitude_wf, phdiff_wf, [
                 ("outputnode.fmap_ref", "inputnode.magnitude"),
                 ("outputnode.fmap_mask", "inputnode.mask"),
             ]),
             (phdiff_wf, bs_filter, [
                 ("outputnode.fieldmap", "in_data"),
             ]),
@@ -156,15 +173,15 @@
             name="fmapmrg",
         )
         units = pe.Node(CheckB0Units(), name="units", run_without_submitting=True)
 
         # fmt: off
         workflow.connect([
             (inputnode, units, [(("fieldmap", _get_units), "units")]),
-            (inputnode, fmapmrg, [(("fieldmap", _get_file), "in_files")]),
+            (check_register, fmapmrg, [("fmap_files", "in_files")]),
             (fmapmrg, units, [("out_avg", "in_file")]),
             (units, bs_filter, [("out_file", "in_data")]),
         ])
         # fmt: on
 
     return workflow
 
@@ -294,32 +311,23 @@
 
     workflow = Workflow(name=name)
     workflow.__desc__ = f"""\
 The corresponding phase-map(s) were phase-unwrapped with `prelude` (FSL {PRELUDE().version}).
 """
 
     inputnode = pe.Node(
-        niu.IdentityInterface(fields=["magnitude", "phase", "mask"]), name="inputnode"
+        niu.IdentityInterface(fields=["magnitude", "phase", "phase_meta", "mask"]),
+        name="inputnode",
     )
 
     outputnode = pe.Node(
         niu.IdentityInterface(fields=["fieldmap"]),
         name="outputnode",
     )
 
-    def _split(phase):
-        return phase
-
-    split = pe.MapNode(  # We cannot use an inline connection function with MapNode
-        niu.Function(function=_split, output_names=["map_file", "meta"]),
-        iterfield=["phase"],
-        run_without_submitting=True,
-        name="split",
-    )
-
     # phase diff -> radians
     phmap2rads = pe.MapNode(
         PhaseMap2rads(),
         name="phmap2rads",
         iterfield=["in_file"],
         run_without_submitting=True,
     )
@@ -330,23 +338,22 @@
         SubtractPhases(), name="calc_phdiff", run_without_submitting=True
     )
     calc_phdiff.interface._always_run = debug
     compfmap = pe.Node(Phasediff2Fieldmap(), name="compfmap")
 
     # fmt: off
     workflow.connect([
-        (inputnode, split, [("phase", "phase")]),
+        (inputnode, phmap2rads, [("phase", "in_file")]),
+        (inputnode, calc_phdiff, [("phase_meta", "in_meta")]),
         (inputnode, prelude, [("magnitude", "magnitude_file"),
                               ("mask", "mask_file")]),
-        (split, phmap2rads, [("map_file", "in_file")]),
         (phmap2rads, calc_phdiff, [("out_file", "in_phases")]),
-        (split, calc_phdiff, [("meta", "in_meta")]),
         (calc_phdiff, prelude, [("phase_diff", "phase_file")]),
-        (prelude, compfmap, [("unwrapped_phase_file", "in_file")]),
         (calc_phdiff, compfmap, [("metadata", "metadata")]),
+        (prelude, compfmap, [("unwrapped_phase_file", "in_file")]),
         (compfmap, outputnode, [("out_file", "fieldmap")]),
     ])
     # fmt: on
     return workflow
 
 
 def _get_file(intuple):
```

### Comparing `sdcflows-2.4.3/sdcflows/workflows/fit/pepolar.py` & `sdcflows-2.5.0/sdcflows/workflows/fit/pepolar.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/fit/syn.py` & `sdcflows-2.5.0/sdcflows/workflows/fit/syn.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_fit.py` & `sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_pepolar.py` & `sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_pepolar.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_phdiff.py` & `sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_phdiff.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_syn.py` & `sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_syn.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/outputs.py` & `sdcflows-2.5.0/sdcflows/workflows/outputs.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/tests/test_ancillary.py` & `sdcflows-2.5.0/sdcflows/workflows/tests/test_ancillary.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows/workflows/tests/test_base.py` & `sdcflows-2.5.0/sdcflows/workflows/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows.egg-info/PKG-INFO` & `sdcflows-2.5.0/sdcflows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdcflows
-Version: 2.4.3
+Version: 2.5.0
 Summary: Susceptibility Distortion Correction (SDC) workflows for EPI MR schemes.
 Home-page: https://www.nipreps.org/sdcflows
 Author: The SDCflows developers
 Author-email: nipreps@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.nipreps.org/sdcflows
 Project-URL: GitHub, https://github.com/nipreps/sdcflows
```

### Comparing `sdcflows-2.4.3/sdcflows.egg-info/SOURCES.txt` & `sdcflows-2.5.0/sdcflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/sdcflows.egg-info/requires.txt` & `sdcflows-2.5.0/sdcflows.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.3/setup.cfg` & `sdcflows-2.5.0/setup.cfg`

 * *Files identical despite different names*

