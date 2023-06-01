# Comparing `tmp/xsarslc-2023.5.16.tar.gz` & `tmp/xsarslc-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsarslc-2023.5.16.tar", last modified: Tue May 16 13:34:43 2023, max compression
+gzip compressed data, was "xsarslc-2023.6.1.tar", last modified: Thu Jun  1 08:11:40 2023, max compression
```

## Comparing `xsarslc-2023.5.16.tar` & `xsarslc-2023.6.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.449299 xsarslc-2023.5.16/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.433299 xsarslc-2023.5.16/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.433299 xsarslc-2023.5.16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 13:34:43.449299 xsarslc-2023.5.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.437299 xsarslc-2023.5.16/auxdata/
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW3_VV.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.433299 xsarslc-2023.5.16/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.437299 xsarslc-2023.5.16/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.441299 xsarslc-2023.5.16/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/ATBD.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/ATBD_L1BSLC.tex
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.433299 xsarslc-2023.5.16/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.441299 xsarslc-2023.5.16/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/_static/css/xsarslc.css
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/crossspectra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/cutoff.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.441299 xsarslc-2023.5.16/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/default_impulseResponse_files_IW.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/xspec_WV_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/NIRAN_NRCS_VH.png
--rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/NIRAN_NRCS_vv.png
--rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/S1_azimuth_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/S1_azimuth_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/S1_range_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/S1_range_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/index
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/normalizedvariance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/sigma0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:34:43.449299 xsarslc-2023.5.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/xsarslc/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/get_config_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/get_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/xsarslc/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/HR_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/deramping.py
--rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/impulseResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/interburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    30553 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/intraburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    28917 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/xspectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/xsarslc/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/xsarslc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.587534 xsarslc-2023.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.587534 xsarslc-2023.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.591534 xsarslc-2023.6.1/auxdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW3_VV.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.587534 xsarslc-2023.6.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.591534 xsarslc-2023.6.1/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.591534 xsarslc-2023.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/ATBD.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/ATBD_L1BSLC.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.587534 xsarslc-2023.6.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.591534 xsarslc-2023.6.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/_static/css/xsarslc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/crossspectra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/cutoff.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.595534 xsarslc-2023.6.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/default_impulseResponse_files_IW.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/xspec_WV_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.595534 xsarslc-2023.6.1/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/NIRAN_NRCS_VH.png
+-rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/NIRAN_NRCS_vv.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/S1_azimuth_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/S1_azimuth_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/S1_range_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/S1_range_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/index
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/normalizedvariance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/sigma0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.595534 xsarslc-2023.6.1/xsarslc/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/get_config_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/get_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/xsarslc/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/HR_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/deramping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/impulseResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/interburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30553 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/intraburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31595 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/xspectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/xsarslc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.595534 xsarslc-2023.6.1/xsarslc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/top_level.txt
```

### Comparing `xsarslc-2023.5.16/.github/workflows/publish.yml` & `xsarslc-2023.6.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/.gitignore` & `xsarslc-2023.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/.pre-commit-config.yaml` & `xsarslc-2023.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/LICENSE` & `xsarslc-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/PKG-INFO` & `xsarslc-2023.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.5.16
+Version: 2023.6.1
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_HH.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_HV.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_VH.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_VV.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW2_VH.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW2_VV.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_HH.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_HV.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_VH.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_VV.nc` & `xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_HH.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_HV.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_VH.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_VV.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_HH.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_HV.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_VH.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_VV.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW3_VH.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/auxdata/S1B_IRs_IW3_VV.nc` & `xsarslc-2023.6.1/auxdata/S1B_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/ATBD.rst` & `xsarslc-2023.6.1/docs/ATBD.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/ATBD_L1BSLC.tex` & `xsarslc-2023.6.1/docs/ATBD_L1BSLC.tex`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/Makefile` & `xsarslc-2023.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/basic_api.rst` & `xsarslc-2023.6.1/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/conf.py` & `xsarslc-2023.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/crossspectra.rst` & `xsarslc-2023.6.1/docs/crossspectra.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/cutoff.rst` & `xsarslc-2023.6.1/docs/cutoff.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/examples/default_impulseResponse_files_IW.ipynb` & `xsarslc-2023.6.1/docs/examples/default_impulseResponse_files_IW.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.6.1/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.6.1/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/examples/xspec_IW_intra_and_inter_burst.ipynb` & `xsarslc-2023.6.1/docs/examples/xspec_IW_intra_and_inter_burst.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/examples/xspec_WV_example.ipynb` & `xsarslc-2023.6.1/docs/examples/xspec_WV_example.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/figures/NIRAN_NRCS_VH.png` & `xsarslc-2023.6.1/docs/figures/NIRAN_NRCS_VH.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/figures/NIRAN_NRCS_vv.png` & `xsarslc-2023.6.1/docs/figures/NIRAN_NRCS_vv.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/figures/S1_azimuth_IR_IW_VV.png` & `xsarslc-2023.6.1/docs/figures/S1_azimuth_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/figures/S1_azimuth_IR_WV_VV.png` & `xsarslc-2023.6.1/docs/figures/S1_azimuth_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/figures/S1_range_IR_IW_VV.png` & `xsarslc-2023.6.1/docs/figures/S1_range_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/figures/S1_range_IR_WV_VV.png` & `xsarslc-2023.6.1/docs/figures/S1_range_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/index.rst` & `xsarslc-2023.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/installing.rst` & `xsarslc-2023.6.1/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/normalizedvariance.rst` & `xsarslc-2023.6.1/docs/normalizedvariance.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/oceanspectrumSAR.png` & `xsarslc-2023.6.1/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/docs/sigma0.rst` & `xsarslc-2023.6.1/docs/sigma0.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/pyproject.toml` & `xsarslc-2023.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/burst.py` & `xsarslc-2023.6.1/xsarslc/burst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/config.yml` & `xsarslc-2023.6.1/xsarslc/config.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/get_config_infos.py` & `xsarslc-2023.6.1/xsarslc/get_config_infos.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/get_test_files.py` & `xsarslc-2023.6.1/xsarslc/get_test_files.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/interface.py` & `xsarslc-2023.6.1/xsarslc/interface.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/processing/HR_tiles.py` & `xsarslc-2023.6.1/xsarslc/processing/HR_tiles.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/processing/deramping.py` & `xsarslc-2023.6.1/xsarslc/processing/deramping.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/processing/impulseResponse.py` & `xsarslc-2023.6.1/xsarslc/processing/impulseResponse.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/processing/interburst.py` & `xsarslc-2023.6.1/xsarslc/processing/interburst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/processing/intraburst.py` & `xsarslc-2023.6.1/xsarslc/processing/intraburst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/processing/xspectra.py` & `xsarslc-2023.6.1/xsarslc/processing/xspectra.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python
 # coding=utf-8
 """
 """
+import pdb
+
 import numpy as np
 import xarray as xr
 import logging
 from scipy.constants import c as celerity
 from xsarslc.tools import xtiling, xndindex
 import warnings
 from tqdm import tqdm
 
 def compute_subswath_xspectra(dt, polarization, tile_width_intra, tile_width_inter, tile_overlap_intra,
                               tile_overlap_inter,
                               periodo_width_intra, periodo_width_inter, periodo_overlap_intra, periodo_overlap_inter,
+                              decimation=None,
                               **kwargs):
     """
     Main function to compute IW inter and intra burst spectra. It has to be modified to be able to change Xspectra options
 
     Args:
         dt (xarray.Datatree): datatree contraining subswath information
         tile_width_intra (dict, optional): approximate sizes of tiles in meters. Dict of shape {dim_name (str): width of tile [m](float)} for intra burst.
@@ -24,21 +27,21 @@
         tile_overlap_intra (dict, optional): approximate sizes of tiles overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)} for intra burst.
         tile_overlap_inter (dict, optional): approximate sizes of tiles overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)} for inter burst.
         periodo_width_intra (dict): approximate sizes of periodogram in meters. Dict of shape {dim_name (str): width of tile [m](float)} for intra burst.
         periodo_width_inter (dict): approximate sizes of periodogram in meters. Dict of shape {dim_name (str): width of tile [m](float)} for inter burst.
         periodo_overlap_intra (dict): approximate sizes of periodogram overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)} for intra burst.
         periodo_overlap_inter (dict): approximate sizes of periodogram overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)} for inter burst.
         polarization (str, optional): polarization to be selected for xspectra computation
+        decimation (int): decimation will be used to decimate xspectra along tile_sample,tile_line dimension, only few specific tiles are saved to netCDF (to save space on disk) [optional, default is None -> no decimation]
 
     Keyword Args:
         kwargs (dict): keyword arguments passed to called functions. landmask, IR_path ...
     """
     import datatree
     from xsarslc.tools import netcdf_compliant
-
     intra_xs = compute_IW_subswath_intraburst_xspectra(dt, polarization=polarization, tile_width=tile_width_intra,
                                                        tile_overlap=tile_overlap_intra,
                                                        periodo_overlap=periodo_overlap_intra,
                                                        periodo_width=periodo_width_intra,
                                                        **kwargs)
     if 'spatial_ref' in intra_xs:
         intra_xs = intra_xs.drop('spatial_ref')
@@ -63,14 +66,51 @@
             inter_xs.attrs.update({'multidataset': str(inter_xs.multidataset)})
             # inter_xs.attrs.update({'start_date': str(inter_xs.start_date)})
             # inter_xs.attrs.update({'stop_date': str(inter_xs.stop_date)})
         if 'footprint' in inter_xs.attrs:
             inter_xs.attrs.update({'footprint': str(inter_xs.footprint)})
         # inter_xs.attrs.pop('pixel_line_m')
         # inter_xs.attrs.pop('pixel_sample_m')
+    if decimation:
+        logging.info('decimation of intra burst and inter burst dataset to save only few tiles')
+        logging.info('one out of %s xspectra will be kept along tile_sample/line axis',decimation)
+        decimation_selection = {'intra':
+                                    {'tile_sample':
+                                        {'iw1': intra_xs.tile_sample.values[::decimation],
+                                         'iw2': intra_xs.tile_sample.values[::decimation],
+                                         'iw3': intra_xs.tile_sample.values[::decimation]
+                                         }
+                                     ,
+                                    'tile_line':
+                                         {
+                                         'iw1': intra_xs.tile_line.values[::decimation],
+                                         'iw2': intra_xs.tile_line.values[::decimation],
+                                         'iw3': intra_xs.tile_line.values[::decimation]
+                                         }
+                                    }
+                                ,
+                                'inter':{
+                                    'tile_sample':
+                                        {'iw1': inter_xs.tile_sample.values[::decimation],
+                                         'iw2': inter_xs.tile_sample.values[::decimation],
+                                         'iw3': inter_xs.tile_sample.values[::decimation]
+                                         },
+                                    'tile_line':
+                                         {
+                                             'iw1': inter_xs.tile_line.values[::decimation],
+                                             'iw2': inter_xs.tile_line.values[::decimation],
+                                             'iw3': inter_xs.tile_line.values[::decimation],
+                                         }
+                                     }
+                                     }
+        subswa = dt.attrs['name'].split(':')[2].lower()
+        inter_xs = inter_xs.isel({'tile_sample':decimation_selection['inter']['tile_sample'][subswa]})
+        intra_xs = intra_xs.isel({'tile_sample':decimation_selection['intra']['tile_sample'][subswa],
+                                  'tile_line':decimation_selection['intra']['tile_line'][subswa]})
+
     if not inter_xs and not intra_xs:
         dt = None
     else:
         dt_dict = {}
         if inter_xs:
             dt_dict.update({'interburst': netcdf_compliant(inter_xs)})
         if intra_xs:
```

### Comparing `xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py` & `xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py` & `xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,24 @@
         import psutil
         memory_used_go = psutil.virtual_memory().used / 1000 / 1000 / 1000.
     str_mem = 'RAM usage: %1.1f Go' % memory_used_go
     return str_mem
 
 
 def generate_IW_L1Bxspec_product(slc_iw_path, output_filename, xspeconfigname, polarization=None, dev=False,
-                                 landmask=None):
+                                 landmask=None,decimation=False):
     """
 
     :param tiff: str full path
     :param output_filename : str full path
     :param xspeconfigname : str (eg 'tiles20km')
     :param polarization : str : VV VH HH HV [optional]
     :param dev: bool: allow to shorten the processing
     :param landmask : landmask obj (eg : cartopy.feature.NaturalEarthFeature() )
+    :param decimation: bool True -> select few tiles to saved on disk [default=False]
     :return:
     """
     safe = os.path.dirname(os.path.dirname(slc_iw_path))
     logging.info('start loading the datatree %s', get_memory_usage())
     tiff_number = os.path.basename(slc_iw_path).split('-')[1].replace('iw', '')
     str_gdal = 'SENTINEL1_DS:%s:IW%s' % (safe, tiff_number)
     bu = xsar.Sentinel1Meta(str_gdal)._bursts
@@ -83,36 +84,37 @@
                                                                    tile_overlap_intra=tile_overlap_intra,
                                                                    periodo_width_intra=periodo_width_intra,
                                                                    periodo_overlap_intra=periodo_overlap_intra,
                                                                    tile_width_inter=tile_width_inter,
                                                                    tile_overlap_inter=tile_overlap_inter,
                                                                    periodo_width_inter=periodo_width_inter,
                                                                    periodo_overlap_inter=periodo_overlap_inter
-                                                                   , IR_path=IR_path,landmask=landmask)
+                                                                   , IR_path=IR_path,landmask=landmask,decimation=decimation)
     else:
         one_subswath_xspectrum_dt = proc.compute_subswath_xspectra(dt, polarization=polarization.upper(),
                                                                    dev=dev, compute_intra_xspec=True,
                                                                    compute_inter_xspec=True,
                                                                    tile_width_intra=tile_width_intra,
                                                                    tile_overlap_intra=tile_overlap_intra,
                                                                    periodo_width_intra=periodo_width_intra,
                                                                    periodo_overlap_intra=periodo_overlap_intra,
                                                                    tile_width_inter=tile_width_inter,
                                                                    tile_overlap_inter=tile_overlap_inter,
                                                                    periodo_width_inter=periodo_width_inter,
                                                                    periodo_overlap_inter=periodo_overlap_inter,
-                                                                   landmask=landmask
+                                                                   landmask=landmask,decimation=decimation
                                                                    )
     if one_subswath_xspectrum_dt:
         logging.info('xspec intra and inter ready for %s', slc_iw_path)
         logging.debug('one_subswath_xspectrum = %s', one_subswath_xspectrum_dt)
         one_subswath_xspectrum_dt.attrs['version_xsar'] = xsar.__version__
         one_subswath_xspectrum_dt.attrs['version_xsarslc'] = xsarslc.__version__
         one_subswath_xspectrum_dt.attrs['processor'] = __file__
         one_subswath_xspectrum_dt.attrs['generation_date'] = datetime.datetime.today().strftime('%Y-%b-%d')
+        one_subswath_xspectrum_dt.attrs['decimation'] = str(decimation)
         if not os.path.exists(os.path.dirname(output_filename)):
             os.makedirs(os.path.dirname(output_filename), 0o0775)
             logging.info('makedir %s', os.path.dirname(output_filename))
         one_subswath_xspectrum_dt.to_netcdf(output_filename)
         logging.info('successfuly written %s', output_filename)
     else:
         logging.info('no inter nor intra xspectra available in this subswath')
@@ -127,14 +129,16 @@
     parser.add_argument('--tiff', required=True, help='tiff file full path IW SLC')
     parser.add_argument('--outputdir', required=False, help='directory where to store output netCDF files',
                         default=get_default_outputdir(mode='iw'))
     parser.add_argument('--version',
                         help='set the output product version (e.g. 1.4) default version will be read from config.yml',
                         required=False, default=PRODUCT_VERSION)
     parser.add_argument('--dev', action='store_true', default=False, help='dev mode stops the computation early')
+    parser.add_argument('--decimation', action='store',type=int, default=None, help='decimation of intra and inter burst '
+                            'tiles before saving, value N implies to keep 1  xspectra out of N in tile_line/sample axis')
     parser.add_argument('--landmask', required=False, default=get_default_landmask_dir(),
                         help='landmask files (such as cartopy /.local/share/cartopy ) to have a landmask information '
                              'without web connexion , default value cromes from config.yml')
     parser.add_argument('--xspeconfigname', required=False, default='tiles20km',
                         help='name of the cross-spectra (tiles/periodogram) in config.yml e.g. "tiles20km" ')
     args = parser.parse_args()
     fmt = '%(asctime)s %(levelname)s %(filename)s(%(lineno)d) %(message)s'
@@ -165,15 +169,15 @@
     logging.info('mode dev is %s', args.dev)
     logging.info('output filename would be: %s', output_filename)
     if os.path.exists(output_filename) and args.overwrite is False:
         logging.info('%s already exists', output_filename)
     else:
         generate_IW_L1Bxspec_product(slc_iw_path=slc_iw_path, output_filename=output_filename,
                                      xspeconfigname=args.xspeconfigname, dev=args.dev,
-                                     polarization=polarization_from_file, landmask=landmask)
+                                     polarization=polarization_from_file, landmask=landmask,decimation=args.decimation)
     logging.info('peak memory usage: %s Mbytes', get_memory_usage())
     logging.info('done in %1.3f min', (time.time() - t0) / 60.)
 
 
 if __name__ == '__main__':
     root = logging.getLogger()
     if root.handlers:
```

### Comparing `xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py` & `xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,19 @@
                                               periodo_overlap_intra=periodo_overlap_intra,
                                               IR_path=IR_path, dev=dev, landmask=landmask)
     # xs = xs0.swap_dims({'freq_line': 'k_az', 'freq_sample': 'k_rg'})
     # xs = xspectra.symmetrize_xspectrum(xs, dim_range='k_rg', dim_azimuth='k_az')
     xs = netcdf_compliant(xs0)  # to split complex128 variables into real and imag part
     xs = xs.drop('pol')
     var2drop = ['var_xspectra_0tau','var_xspectra_1tau','var_xspectra_2tau','xspectra_0tau_Re','xspectra_0tau_Im','xspectra_1tau_Re','xspectra_1tau_Im']
-    xs = xs.drop_vars(var2drop)
+    var2drop_consolidated = []
+    for vv in var2drop:
+        if vv in xs:
+            var2drop_consolidated.append(vv)
+    xs = xs.drop_vars(var2drop_consolidated)
     if 'spatial_ref' in xs:
         xs = xs.drop('spatial_ref')
     if xs:
         logging.info('xspec ready for %s', slc_wv_path)
         logging.debug('one_subswath_xspectrum = %s', xs)
         xs.attrs['version_xsar'] = xsar.__version__
         xs.attrs['version_xsarslc'] = xsarslc.__version__
```

### Comparing `xsarslc-2023.5.16/xsarslc/tools.py` & `xsarslc-2023.6.1/xsarslc/tools.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.5.16/xsarslc.egg-info/PKG-INFO` & `xsarslc-2023.6.1/xsarslc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.5.16
+Version: 2023.6.1
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `xsarslc-2023.5.16/xsarslc.egg-info/SOURCES.txt` & `xsarslc-2023.6.1/xsarslc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

