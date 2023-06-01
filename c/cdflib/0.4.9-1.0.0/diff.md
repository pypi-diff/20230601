# Comparing `tmp/cdflib-0.4.9.tar.gz` & `tmp/cdflib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdflib-0.4.9.tar", last modified: Wed Nov  9 22:22:06 2022, max compression
+gzip compressed data, was "cdflib-1.0.0.tar", last modified: Thu Jun  1 19:40:17 2023, max compression
```

## Comparing `cdflib-0.4.9.tar` & `cdflib-1.0.0.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.783912 cdflib-0.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.775911 cdflib-0.4.9/.circleci/
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-11-09 22:21:49.000000 cdflib-0.4.9/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-09 22:21:49.000000 cdflib-0.4.9/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-09 22:21:49.000000 cdflib-0.4.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.775911 cdflib-0.4.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.779911 cdflib-0.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-09 22:21:49.000000 cdflib-0.4.9/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-11-09 22:21:49.000000 cdflib-0.4.9/.github/workflows/pypi-build.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-11-09 22:21:49.000000 cdflib-0.4.9/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-09 22:21:49.000000 cdflib-0.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-11-09 22:21:49.000000 cdflib-0.4.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-11-09 22:21:49.000000 cdflib-0.4.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-11-09 22:21:49.000000 cdflib-0.4.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-09 22:21:49.000000 cdflib-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-09 22:21:49.000000 cdflib-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-09 22:22:06.783912 cdflib-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-11-09 22:21:49.000000 cdflib-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.779911 cdflib-0.4.9/archive/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-09 22:21:49.000000 cdflib-0.4.9/archive/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6873 2022-11-09 22:21:49.000000 cdflib-0.4.9/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.779911 cdflib-0.4.9/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 22:21:49.000000 cdflib-0.4.9/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-11-09 22:21:49.000000 cdflib-0.4.9/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.779911 cdflib-0.4.9/cdflib/
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-11-09 22:21:49.000000 cdflib-0.4.9/cdflib/CDFLeapSeconds.txt
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-11-09 22:21:49.000000 cdflib-0.4.9/cdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-09 22:22:06.000000 cdflib-0.4.9/cdflib/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    37417 2022-11-09 22:21:49.000000 cdflib-0.4.9/cdflib/cdf_to_xarray.py
--rw-r--r--   0 runner    (1001) docker     (121)   107965 2022-11-09 22:21:49.000000 cdflib-0.4.9/cdflib/cdfread.py
--rw-r--r--   0 runner    (1001) docker     (121)   106197 2022-11-09 22:21:49.000000 cdflib-0.4.9/cdflib/cdfwrite.py
--rw-r--r--   0 runner    (1001) docker     (121)    72047 2022-11-09 22:21:49.000000 cdflib-0.4.9/cdflib/epochs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10581 2022-11-09 22:21:49.000000 cdflib-0.4.9/cdflib/epochs_astropy.py
--rw-r--r--   0 runner    (1001) docker     (121)    31219 2022-11-09 22:21:49.000000 cdflib-0.4.9/cdflib/xarray_to_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.779911 cdflib-0.4.9/cdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-09 22:22:06.000000 cdflib-0.4.9/cdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-11-09 22:22:06.000000 cdflib-0.4.9/cdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 22:22:06.000000 cdflib-0.4.9/cdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-09 22:22:06.000000 cdflib-0.4.9/cdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-09 22:22:06.000000 cdflib-0.4.9/cdflib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.779911 cdflib-0.4.9/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     4986 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.779911 cdflib-0.4.9/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/modules/cdfepoch.rst
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/modules/cdfread.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/modules/cdfwrite.rst
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/modules/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-09 22:21:49.000000 cdflib-0.4.9/doc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-11-09 22:21:49.000000 cdflib-0.4.9/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-09 22:21:49.000000 cdflib-0.4.9/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-11-09 22:21:49.000000 cdflib-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-11-09 22:22:06.783912 cdflib-0.4.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.783912 cdflib-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/test_astropy_epochs.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/test_cdfread.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/test_cdfread_rle.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16801 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/test_cdfwrite.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9864 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (121)    36419 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/test_xarray_reader_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:22:06.783912 cdflib-0.4.9/tests/testfiles/
--rw-r--r--   0 runner    (1001) docker     (121)    67164 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (121)    70003 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-09 22:21:49.000000 cdflib-0.4.9/tests/testfiles/testing_file_location.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-11-09 22:21:49.000000 cdflib-0.4.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-01 19:40:00.000000 cdflib-1.0.0/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-01 19:40:00.000000 cdflib-1.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 19:40:00.000000 cdflib-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.037493 cdflib-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-01 19:40:00.000000 cdflib-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-01 19:40:00.000000 cdflib-1.0.0/.github/workflows/pypi-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-01 19:40:00.000000 cdflib-1.0.0/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-01 19:40:00.000000 cdflib-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 19:40:00.000000 cdflib-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-01 19:40:00.000000 cdflib-1.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 19:40:00.000000 cdflib-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 19:40:00.000000 cdflib-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-01 19:40:17.045493 cdflib-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 19:40:00.000000 cdflib-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 19:40:00.000000 cdflib-1.0.0/archive/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-01 19:40:00.000000 cdflib-1.0.0/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:00.000000 cdflib-1.0.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-01 19:40:00.000000 cdflib-1.0.0/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/cdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/CDFLeapSeconds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 19:40:16.000000 cdflib-1.0.0/cdflib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38003 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/cdf_to_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84619 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104337 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/cdfwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65531 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/epochs_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32046 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/xarray_to_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/cdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/cdfepoch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/cdfread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/cdfwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/dataclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 19:40:00.000000 cdflib-1.0.0/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-01 19:40:00.000000 cdflib-1.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 19:40:00.000000 cdflib-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 19:40:17.045493 cdflib-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_astropy_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_cdfread_rle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_cdfwrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_xarray_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/tests/testfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/testfiles/testing_file_location.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 19:40:00.000000 cdflib-1.0.0/tox.ini
```

### Comparing `cdflib-0.4.9/.circleci/config.yml` & `cdflib-1.0.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/.github/workflows/ci.yml` & `cdflib-1.0.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
     steps:
     - uses: actions/checkout@v3
 
     - uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install package and test requirements
```

### Comparing `cdflib-0.4.9/.github/workflows/pypi-build.yaml` & `cdflib-1.0.0/.github/workflows/pypi-build.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/.github/workflows/python-lint.yml` & `cdflib-1.0.0/.github/workflows/python-lint.yml`

 * *Files 14% similar despite different names*

```diff
@@ -20,9 +20,10 @@
       uses: actions/setup-python@v2
       with:
         python-version: 3.9
     - name: Install pre-commit
       run: |
         python -m pip install --upgrade pip
         python -m pip install pre-commit
+        python -m pip install .
     - name: Run pre-commit
       run: pre-commit run --all-files
```

### Comparing `cdflib-0.4.9/.pre-commit-config.yaml` & `cdflib-1.0.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 repos:
   - repo: https://github.com/myint/autoflake
-    rev: v1.4
+    rev: v2.1.1
     hooks:
       - id: autoflake
         args: ['--in-place', '--remove-all-unused-imports', '--remove-unused-variable']
         exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|__init__.py|.svg)$"
 
   - repo: https://github.com/timothycrosley/isort
-    rev: 5.8.0
+    rev: 5.12.0
     hooks:
       - id: isort
         args: ['--sp','setup.cfg']
         exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|.svg)$"
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.4.0
+    rev: v4.4.0
     hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: trailing-whitespace
         exclude: ".*(.fits|.fts|.fit|.txt|.svg|.json)$"
       - id: debug-statements
       - id: check-added-large-files
       - id: end-of-file-fixer
         exclude: ".*(.fits|.fts|.fit|.txt|tca.*|.svg|.json)$"
       - id: mixed-line-ending
         exclude: ".*(.fits|.fts|.fit|.txt|tca.*|.svg)$"
 
+  - repo: https://github.com/psf/black
+    rev: 23.3.0
+    hooks:
+      - id: black
+
   -   repo: https://github.com/pre-commit/mirrors-mypy
-      rev: 'v0.961'
+      rev: 'v1.3.0'
       hooks:
       - id: mypy
+        additional_dependencies: [xarray]
```

### Comparing `cdflib-0.4.9/.readthedocs.yml` & `cdflib-1.0.0/.readthedocs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -6,24 +6,20 @@
 version: 2
 
 # Set the version of Python and other tools you might need
 build:
   os: ubuntu-20.04
   tools:
     python: "3.9"
-    # You can also specify other tool versions:
-    # nodejs: "16"
-    # rust: "1.55"
-    # golang: "1.17"
 
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
    configuration: doc/conf.py
 
-# If using Sphinx, optionally build your docs in additional formats such as PDF
-# formats:
-#    - pdf
 
 # Optionally declare the Python requirements required to build your docs
 python:
    install:
-   - requirements: doc/requirements.txt
+   -  method: pip
+      path: .
+      extra_requirements:
+         - docs
```

### Comparing `cdflib-0.4.9/LICENSE` & `cdflib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/README.md` & `cdflib-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,22 @@
 [![Documentation Status](https://readthedocs.org/projects/cdflib/badge/?version=latest)](https://cdflib.readthedocs.io/en/latest/?badge=latest)
 
 # CDFlib
 
 `cdflib` is a python module to read/write CDF (Common Data Format `.cdf`) files without needing to install the
 [CDF NASA library](https://cdf.gsfc.nasa.gov/).
 
-Python &ge; 3.6 is required.
-This module uses only Numpy, no complicated prereqs.
+Python >= 3.8 is required.
+The core of this package uses only numpy, with no complicated compiler requirements.
 
 ## Install
 
 To install, open up your terminal/command prompt, and type:
 ```sh
 pip install cdflib
 ```
-There are two different CDF classes: a cdf reader, and a cdf writer.
-
-Currently, you cannot simultaneously read and write to the same file.
-Future implementations, however, will unify these two classes.
 
 ## Documentation
 
 The full documentation can be found here:
 
 [https://cdflib.readthedocs.io/en/latest/](https://cdflib.readthedocs.io/en/latest/)
```

### Comparing `cdflib-0.4.9/asv.conf.json` & `cdflib-1.0.0/asv.conf.json`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/benchmarks/benchmarks.py` & `cdflib-1.0.0/benchmarks/benchmarks.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 
 
 class TimeSuite:
     """
     An example benchmark that times the performance of various kinds
     of iterating over dictionaries in Python.
     """
-    params = ([True, False], )
-    param_names = ['to_np']
 
-    def setup(self, to_np):
+    def setup(self):
         self.epochs = np.ones(1000) * 62567898765432.0
         self.epochs_tt2000 = (np.ones(1000) * 186999622360321123).astype(int)
 
-    def time_epoch_encode(self, to_np):
+    def time_epoch_encode(self):
         cdfepoch.encode(self.epochs)
 
-    def time_epoch_to_datetime(self, to_np):
+    def time_epoch_to_datetime(self):
         cdfepoch.to_datetime(self.epochs)
 
-    def time_epoch_to_datetime_tt2000(self, to_np):
+    def time_epoch_to_datetime_tt2000(self):
         cdfepoch.to_datetime(self.epochs_tt2000)
```

### Comparing `cdflib-0.4.9/cdflib/CDFLeapSeconds.txt` & `cdflib-1.0.0/cdflib/CDFLeapSeconds.txt`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/cdflib/__init__.py` & `cdflib-1.0.0/cdflib/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 except BaseException:
     pass
 
 # Another optional dependency for XArray <-> cdf conversions
 from .cdf_to_xarray import cdf_to_xarray
 from .xarray_to_cdf import xarray_to_cdf
 
-__all__ = ['CDF', 'xarray_to_cdf', 'cdf_to_xarray']
+__all__ = ["CDF", "xarray_to_cdf", "cdf_to_xarray"]
 try:
     from ._version import version as __version__
 except Exception:
-    __version__ = 'unknown'
+    __version__ = "unknown"
```

### Comparing `cdflib-0.4.9/cdflib/cdf_to_xarray.py` & `cdflib-1.0.0/cdflib/cdf_to_xarray.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,473 +1,496 @@
 import re
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import numpy as np
+import numpy.typing as npt
+import xarray as xr
 
 from cdflib import CDF
+from cdflib.dataclasses import AttData, VDRInfo
 from cdflib.epochs import CDFepoch as cdfepoch
 
-ISTP_TO_XARRAY_ATTRS = {'FIELDNAM': 'standard_name',
-                        'LABLAXIS': 'long_name',
-                        'UNITS': 'units'}
+ISTP_TO_XARRAY_ATTRS = {"FIELDNAM": "standard_name", "LABLAXIS": "long_name", "UNITS": "units"}
 
 
-def _find_xarray_plotting_values(var_att_dict):
-    '''
+def _find_xarray_plotting_values(var_att_dict: Dict[str, str]) -> Dict[str, str]:
+    """
     This is a simple function that looks through a variable attribute dictionary for ISTP attributes that are similar
     to ones used natively by Xarray, specifically their plotting routines.  If some are found, this returns a dictionary
     object of this new xarray attributes
     :param var_att_dict: A dictionary of attributes that a variable has
     :return:a dictionary of attributes that should be added to the created XArray DataArray
-    '''
-    xarray_att_dict = {}
+    """
+    xarray_att_dict: Dict[str, str] = {}
     if not var_att_dict:
         return xarray_att_dict
     for key, value in var_att_dict.items():
         if key in ISTP_TO_XARRAY_ATTRS:
             xarray_att_dict[ISTP_TO_XARRAY_ATTRS[key]] = value
     return xarray_att_dict
 
 
-def _convert_cdf_time_types(data, atts, properties, to_datetime=False, to_unixtime=False):
-    '''
+def _convert_cdf_time_types(
+    data: npt.ArrayLike, atts: Dict[str, AttData], properties: VDRInfo, to_datetime: bool = False, to_unixtime: bool = False
+) -> Tuple[npt.NDArray, Dict[str, Any]]:
+    """
     # Converts CDF time types into either datetime objects, unixtime, or nothing
     # If nothing, ALL CDF_EPOCH16 types are converted to CDF_EPOCH, because xarray can't handle int64s
-    '''
-
-    data = np.squeeze(data)
-
-    if not hasattr(data, '__len__'):
-        data = [data]
+    """
 
-    try:
-        len(data)
-    except Exception:
-        data = [data]
+    data = np.atleast_1d(np.squeeze(data))
 
     if to_datetime and to_unixtime:
         print("Cannot convert to both unixtime and datetime.  Continuing with conversion to unixtime.")
         to_datetime = False
 
     # Convert all data in the "data" variable to unixtime or datetime if needed
-    data_type = properties['Data_Type_Description']
-    if len(data) == 0 or data_type not in ('CDF_EPOCH', 'CDF_EPOCH16', 'CDF_TIME_TT2000'):
+    data_type = properties.Data_Type_Description
+    if len(data) == 0 or data_type not in ("CDF_EPOCH", "CDF_EPOCH16", "CDF_TIME_TT2000"):
         new_data = data
     else:
         if to_datetime:
             new_data = cdfepoch.to_datetime(data)
-            if 'UNITS' in atts:
-                atts['UNITS']['Data'] = 'Datetime (UTC)'
+            if "UNITS" in atts:
+                atts["UNITS"].Data = "Datetime (UTC)"
         elif to_unixtime:
             new_data = cdfepoch.unixtime(data)
-            if 'UNITS' in atts:
-                atts['UNITS']['Data'] = 'seconds'
+            if "UNITS" in atts:
+                atts["UNITS"].Data = "seconds"
         else:
-            if data_type == 'CDF_EPOCH16':
+            if data_type == "CDF_EPOCH16":
                 new_data = cdfepoch.compute(cdfepoch.breakdown(data)[0:7])
             else:
                 new_data = data
 
     # Convert all the attributes in the "atts" dictionary to unixtime or datetime if needed
     new_atts = {}
     for att in atts:
-        data_type = atts[att]['Data_Type']
-        data = atts[att]['Data']
-        if not hasattr(data, '__len__'):
-            data = [data]
-        if len(data) == 0 or data_type not in ('CDF_EPOCH', 'CDF_EPOCH16', 'CDF_TIME_TT2000'):
+        data_type = atts[att].Data_Type
+        data = atts[att].Data
+        if len(data) == 0 or data_type not in ("CDF_EPOCH", "CDF_EPOCH16", "CDF_TIME_TT2000"):
             new_atts[att] = data
         else:
             if to_datetime:
                 new_atts[att] = cdfepoch.to_datetime(data)
             elif to_unixtime:
                 new_atts[att] = cdfepoch.unixtime(data)
             else:
-                if data_type == 'CDF_EPOCH16':
+                if data_type == "CDF_EPOCH16":
                     new_atts[att] = cdfepoch.compute(cdfepoch.breakdown(data)[0:7])
                 else:
                     new_atts[att] = data
 
     return new_data, new_atts
 
 
-def _convert_cdf_to_dicts(filename, to_datetime=False, to_unixtime=False):
+def _convert_cdf_to_dicts(
+    filename: Union[str, Path], to_datetime: bool = False, to_unixtime: bool = False
+) -> Tuple[Dict[str, List[Union[str, np.ndarray]]], Dict[str, Any], Dict[str, npt.NDArray], Dict[str, VDRInfo]]:
     # Open the CDF file
     # Converts the entire CDF file into python dictionary objects
 
-    cdf_file = CDF(filename, string_encoding='latin-1')
+    cdf_file = CDF(filename, string_encoding="latin-1")
     cdf_info = cdf_file.cdf_info()
-    all_cdf_variables = cdf_info['rVariables'] + cdf_info['zVariables']
+    all_cdf_variables = cdf_info.rVariables + cdf_info.zVariables
 
     # Gather all Global Attributes
     try:
         gatt = cdf_file.globalattsget()
     except BaseException:
         gatt = {}
 
     # Gather all information about the CDF file, and store in the below dictionaries
-    variable_data = {}
-    variable_attributes = {}
-    variable_properties = {}
+    variable_data: Dict[str, npt.NDArray] = {}
+    variable_attributes: Dict[str, Any] = {}
+    variable_properties: Dict[str, VDRInfo] = {}
 
     for var_name in all_cdf_variables:
         var_attribute_list = cdf_file.varattsget(var_name)
-        var_data_temp = {}
-        var_atts_temp = {}
+        var_data_temp: Dict[str, Union[str, np.ndarray]] = {}
+        var_atts_temp: Dict[str, AttData] = {}
         for att in var_attribute_list:
-            var_atts_temp[att] = (cdf_file.attget(att, var_name))
+            var_atts_temp[att] = cdf_file.attget(att, var_name)
         variable_properties[var_name] = cdf_file.varinq(var_name)
         # Gather the actual variable data
-        if variable_properties[var_name]['Last_Rec'] < 0:
+        if variable_properties[var_name].Last_Rec < 0:
             var_data_temp[var_name] = np.array([])
         else:
             var_data_temp[var_name] = cdf_file.varget(var_name)
 
-        variable_data[var_name], variable_attributes[var_name] = _convert_cdf_time_types(var_data_temp[var_name], var_atts_temp,
-                                                                                         variable_properties[var_name],
-                                                                                         to_datetime=to_datetime,
-                                                                                         to_unixtime=to_unixtime)
+        variable_data[var_name], variable_attributes[var_name] = _convert_cdf_time_types(
+            var_data_temp[var_name], var_atts_temp, variable_properties[var_name], to_datetime=to_datetime, to_unixtime=to_unixtime
+        )
 
     return gatt, variable_attributes, variable_data, variable_properties
 
 
-def _verify_depend_dimensions(dataset, dimension_number, primary_variable_name,
-                              coordinate_variable_name, primary_variable_properties):
-
+def _verify_depend_dimensions(
+    dataset: Dict[str, npt.NDArray],
+    dimension_number: int,
+    primary_variable_name: str,
+    coordinate_variable_name: str,
+    primary_variable_properties: VDRInfo,
+) -> bool:
     primary_data = np.array(dataset[primary_variable_name])
     coordinate_data = np.array(dataset[coordinate_variable_name])
 
     if len(primary_data.shape) != 0 and len(coordinate_data.shape) == 0:
         print(
-            f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match.')
+            f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
+        )
         return False
 
     if len(coordinate_data.shape) != 0 and len(primary_data.shape) == 0:
         print(
-            f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match.')
+            f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
+        )
         return False
 
     if len(coordinate_data.shape) > 2:
         print(
-            f'ISTP Compliance Warning: {coordinate_variable_name} has too many dimensions to be the DEPEND_{dimension_number} for variable {primary_variable_name}')
+            f"ISTP Compliance Warning: {coordinate_variable_name} has too many dimensions to be the DEPEND_{dimension_number} for variable {primary_variable_name}"
+        )
         return False
     if len(coordinate_data.shape) == 2:
-
         if primary_data.shape[0] != coordinate_data.shape[0]:
             print(
-                f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the Epoch dimensions do not match.')
+                f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the Epoch dimensions do not match."
+            )
             return False
 
-    if primary_variable_properties["Rec_Vary"] and primary_variable_properties["Last_Rec"] > 0:
+    if primary_variable_properties.Rec_Vary and primary_variable_properties.Last_Rec > 0:
         if len(primary_data.shape) <= dimension_number:
             print(
-                f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions')
+                f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions"
+            )
             return False
 
         if primary_data.shape[dimension_number] != coordinate_data.shape[-1]:
             print(
-                f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match.')
+                f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
+            )
             return False
     else:
         if len(primary_data.shape) <= dimension_number - 1:
             print(
-                f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions')
+                f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions"
+            )
             return False
 
         if primary_data.shape[dimension_number - 1] != coordinate_data.shape[-1]:
             # This is kind of a hack for now.
             # DEPEND_1 can sometimes refer to the first dimension in a variable, and sometimes the second.
             # So we require both the first and second dimensions don't match the coordinate size before we definitely
             # reject it.
             if len(primary_data.shape) > dimension_number and primary_data.shape[dimension_number] != coordinate_data.shape[-1]:
                 print(
-                    f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match.')
+                    f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
+                )
                 return False
 
     return True
 
 
-def _discover_depend_variables(vardata, varatts, varprops):
+def _discover_depend_variables(vardata: Dict[str, npt.NDArray], varatts: Dict[str, Any], varprops: Dict[str, VDRInfo]) -> List[str]:
     # This loops through the variable attributes to discover which variables are the coordinates of other variables,
     # Unfortunately, there is no easy way to tell this by looking at the variable ITSELF,
     # you need to look at all variables and see if one points to it.
 
-    depend_regex = re.compile('depend_[0-9]+$')
+    depend_regex = re.compile("depend_[0-9]+$")
 
     list_of_depend_vars = []
 
     for v in varatts:
         depend_keys = [x for x in list(varatts[v].keys()) if depend_regex.match(x.lower())]
         for d in depend_keys:
             if varatts[v][d] in vardata:
                 if _verify_depend_dimensions(vardata, int(d[-1]), v, varatts[v][d], varprops[v]):
                     list_of_depend_vars.append(varatts[v][d])
 
     return list(set(list_of_depend_vars))
 
 
-def _discover_uncertainty_variables(varatts):
+def _discover_uncertainty_variables(varatts: Dict[str, Any]) -> Dict[str, str]:
     # This loops through the variable attributes to discover which variables are the labels of other variables
     # Unfortunately, there is no easy way to tell this by looking at the label variable itself
     # This returns a KEY:VALUE pair, with the LABEL VARIABLE corresponding to which dimension it covers.
 
     list_of_label_vars = {}
 
     for v in varatts:
-        if 'DELTA_PLUS_VAR' in varatts[v].keys():
-            list_of_label_vars[varatts[v]['DELTA_PLUS_VAR']] = v
-        if 'DELTA_MINUS_VAR' in varatts[v].keys():
-            list_of_label_vars[varatts[v]['DELTA_MINUS_VAR']] = v
+        if "DELTA_PLUS_VAR" in varatts[v].keys():
+            list_of_label_vars[varatts[v]["DELTA_PLUS_VAR"]] = v
+        if "DELTA_MINUS_VAR" in varatts[v].keys():
+            list_of_label_vars[varatts[v]["DELTA_MINUS_VAR"]] = v
     return list_of_label_vars
 
 
-def _discover_label_variables(varatts, all_variable_properties, all_variable_data):
+def _discover_label_variables(
+    varatts: Dict[str, Any], all_variable_properties: Dict[str, VDRInfo], all_variable_data: Dict[str, npt.NDArray]
+) -> Dict[str, str]:
     # This loops through the variable attributes to discover which variables are the labels of other variables
     # Unfortunately, there is no easy way to tell this by looking at the label variable itself
     # This returns a KEY:VALUE pair, with the LABEL VARIABLE corresponding to which dimension it covers.
 
-    list_of_label_vars = {}
+    list_of_label_vars: Dict[str, str] = {}
 
     for v in varatts:
         label_keys = [x for x in list(varatts[v].keys()) if x.startswith("LABL_PTR_")]
         for lab in label_keys:
-            label_dependency = 'DEPEND_' + lab[-1]
+            label_dependency = "DEPEND_" + lab[-1]
             if label_dependency not in varatts[v]:
                 continue
             depend_var_name = varatts[v][label_dependency]
 
-            if all_variable_properties[depend_var_name]["Dim_Sizes"] and len(all_variable_properties[v]["Dim_Sizes"]) > 0 and (
-                    all_variable_properties[depend_var_name]["Dim_Sizes"][0] == all_variable_properties[v]["Dim_Sizes"][int(lab[-1]) - 1]):
+            if (
+                all_variable_properties[depend_var_name].Dim_Sizes
+                and len(all_variable_properties[v].Dim_Sizes) > 0
+                and (
+                    all_variable_properties[depend_var_name].Dim_Sizes[0] == all_variable_properties[v].Dim_Sizes[int(lab[-1]) - 1]
+                )
+            ):
                 if all_variable_data[depend_var_name].size == 0:
                     continue
             else:
                 continue
 
             if varatts[v][lab] not in varatts:
                 print(f"Warning, variable {v} points to {varatts[v][lab]} as label {lab}, but {varatts[v][lab]} does not exist.")
                 print(f"Setting {varatts[v][lab]} as long_name instead.")
-                varatts[v]['LABLAXIS'] = varatts[v][lab]
-                varatts[v]['long_name'] = varatts[v][lab]
+                varatts[v]["LABLAXIS"] = varatts[v][lab]
+                varatts[v]["long_name"] = varatts[v][lab]
                 continue
 
             list_of_label_vars[varatts[v][lab]] = depend_var_name
 
     return list_of_label_vars
 
 
-def _convert_fillvals_to_nan(var_data, var_atts, var_properties):
-
+def _convert_fillvals_to_nan(var_data: npt.NDArray, var_atts: Dict[str, Any], var_properties: VDRInfo) -> npt.NDArray:
     if var_atts is None:
         return var_data
     if var_data is None:
         return var_data
 
     new_data = var_data
-    if 'FILLVAL' in var_atts:
-        if (var_properties['Data_Type_Description'] ==
-                'CDF_FLOAT' or
-                var_properties['Data_Type_Description'] ==
-                'CDF_REAL4' or
-                var_properties['Data_Type_Description'] ==
-                'CDF_DOUBLE' or
-                var_properties['Data_Type_Description'] ==
-                'CDF_REAL8' or
-                var_properties['Data_Type_Description'] ==
-                'CDF_TIME_TT2000' or
-                var_properties['Data_Type_Description'] ==
-                'CDF_EPOCH' or
-                var_properties['Data_Type_Description'] ==
-                'CDF_EPOCH16'):
-
+    if "FILLVAL" in var_atts:
+        if var_properties.Data_Type_Description in (
+            "CDF_FLOAT",
+            "CDF_REAL4",
+            "CDF_DOUBLE",
+            "CDF_REAL8",
+            "CDF_TIME_TT2000",
+            "CDF_EPOCH",
+            "CDF_EPOCH16",
+        ):
             if new_data.size > 1:
                 if new_data[new_data == var_atts["FILLVAL"]].size != 0:
                     new_data[new_data == var_atts["FILLVAL"]] = np.nan
             else:
-                if new_data == var_atts['FILLVAL']:
+                if new_data == var_atts["FILLVAL"]:
                     new_data = np.array(np.nan)
     return new_data
 
 
-def _determine_record_dimensions(var_name, var_atts, var_data, var_props, depend_variables,
-                                 all_variable_data, all_variable_properties, created_unlimited_dims):
-    '''
+def _determine_record_dimensions(
+    var_name: str,
+    var_atts: Dict[str, Any],
+    var_data: npt.NDArray,
+    var_props: VDRInfo,
+    depend_variables: List[str],
+    all_variable_data: Dict[str, npt.NDArray],
+    all_variable_properties: Dict[str, VDRInfo],
+    created_unlimited_dims: Dict[str, int],
+) -> Tuple[str, bool, bool]:
+    """
     Determines the name of the
-    :param var_name:
-    :param var_atts:
-    :param var_data:
-    :param var_props:
-    :param depend_variables:
-    :param all_variable_data:
-    :param all_variable_properties:
-    :param created_unlimited_dims:
-    :return:
-    '''
-
-    if var_props["Rec_Vary"] and var_props["Last_Rec"] > 0:
+    """
 
+    if var_props.Rec_Vary and var_props.Last_Rec > 0:
         # Check if this variable is itself the dimension
-        if var_name in depend_variables and (len(var_props["Dim_Sizes"]) == 0 or var_props['Last_Rec'] >= 0):
-            if not (len(var_props["Dim_Sizes"]) > 0 and var_props['Last_Rec'] > 0):
+        if var_name in depend_variables and (len(var_props.Dim_Sizes) == 0 or var_props.Last_Rec >= 0):
+            if not (len(var_props.Dim_Sizes) > 0 and var_props.Last_Rec > 0):
                 return var_name, True, False
             # There might be dimensions listed, but they might not vary
-            if len(var_props["Dim_Sizes"]) > 0:
-                for i in range(0, len(var_props["Dim_Sizes"])):
-                    if var_props["Dim_Vary"][i]:
+            if len(var_props.Dim_Sizes) > 0:
+                for i in range(0, len(var_props.Dim_Sizes)):
+                    if var_props.Dim_Vary[i]:
                         break
                 else:
                     return var_name, True, False
 
         # Check if the dimension is already defined within the attribute section
-        if 'DEPEND_0' in var_atts:
-            depend_0_variable_name = var_atts['DEPEND_0']
+        if "DEPEND_0" in var_atts:
+            depend_0_variable_name = var_atts["DEPEND_0"]
             if depend_0_variable_name not in all_variable_properties:
-                print(f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but no"
-                      f" variable by that name was found.")
+                print(
+                    f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but no"
+                    f" variable by that name was found."
+                )
             else:
                 if len(all_variable_data[depend_0_variable_name]) == len(var_data):
                     return depend_0_variable_name, True, False
                 else:
                     print(
-                        f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but they have different dimension lengths.")
+                        f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but they have different dimension lengths."
+                    )
 
-        '''
+        """
         # If the variable still isn't found, it should be fine to name the dimension after the variable
         if var_name in depend_variables and not udim_found:
             var_dims.append(var_name)
             depend_dimensions[var_name] = len(var_data)
             udim_found = True
-        '''
+        """
 
         # If none of the above, check if the length of this variable dimension
         # matches a non-specific one that has already been created
         for udim in created_unlimited_dims:
             if len(var_data) == created_unlimited_dims[udim]:
                 return udim, False, False
 
         # If none of the above, create a new dimension variable
-        new_udim_name = 'record' + str(len(created_unlimited_dims))
+        new_udim_name = "record" + str(len(created_unlimited_dims))
         return new_udim_name, False, True
 
-    elif 'DEPEND_0' in var_atts:
-
+    elif "DEPEND_0" in var_atts:
         # Check if the dimension is already defined within the attribute section
-        depend_0_variable_name = var_atts['DEPEND_0']
+        depend_0_variable_name = var_atts["DEPEND_0"]
         if depend_0_variable_name not in all_variable_properties:
-            print(f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but no"
-                  f" variable by that name was found.")
+            print(
+                f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but no"
+                f" variable by that name was found."
+            )
         else:
             if len(all_variable_data[depend_0_variable_name]) == len(var_data) and len(var_data) != 0:
                 return depend_0_variable_name, True, False
             else:
                 print(
-                    f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but they have different dimension lengths.")
+                    f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but they have different dimension lengths."
+                )
 
         return None, False, False
 
         # If none of the above, check if the length of this variable dimension matches a non-specific one that has already been created
         # for udim in created_unlimited_dims:
         #    if len(var_data) == created_unlimited_dims[udim]:
         #        return udim, False, False
 
         # If none of the above, create a new dimension variable
-        #new_udim_name = 'record' + str(len(created_unlimited_dims))
+        # new_udim_name = 'record' + str(len(created_unlimited_dims))
         # return new_udim_name, False, True
 
     else:
-
         return None, False, False
 
 
-def _determine_dimension_names(var_name, var_atts, var_data, var_props, depend_variables,
-                               all_variable_data, all_variable_properties, created_regular_dims, record_name_found):
-    '''
-    :param var_name:
-    :param var_atts:
-    :param var_props:
-    :param depend_variables:
-    :param all_variable_data:
-    :param all_variable_properties:
-    :param created_regular_dims:
-    :return:
-    '''
-
+def _determine_dimension_names(
+    var_name: str,
+    var_atts: Dict[str, Any],
+    var_data: npt.NDArray,
+    var_props: VDRInfo,
+    depend_variables: List[str],
+    all_variable_data: Dict[str, npt.NDArray],
+    all_variable_properties: Dict[str, VDRInfo],
+    created_regular_dims: Dict[str, int],
+    record_name_found: str,
+) -> List[Tuple[str, int, bool, bool]]:
     return_list = []
 
-    if len(var_props["Dim_Sizes"]) != 0 and var_props['Last_Rec'] >= 0:
+    if len(var_props.Dim_Sizes) != 0 and var_props.Last_Rec >= 0:
         i = 0
-        skip_first_dim = record_name_found
         for dim_size in var_data.shape:
-            if skip_first_dim:
-                skip_first_dim = False
+            if record_name_found:
                 continue
 
             i += 1
 
             # Check if the dimension is already defined within the attribute section
-            if 'DEPEND_' + str(i) in var_atts:
-                depend_i_variable_name = var_atts['DEPEND_' + str(i)]
+            if "DEPEND_" + str(i) in var_atts:
+                depend_i_variable_name = var_atts["DEPEND_" + str(i)]
                 if depend_i_variable_name not in all_variable_properties:
-                    print(f"Warning: Variable {var_name} listed DEPEND_{str(i)} as {depend_i_variable_name}, but no"
-                          f" variable by that name was found.")
+                    print(
+                        f"Warning: Variable {var_name} listed DEPEND_{str(i)} as {depend_i_variable_name}, but no"
+                        f" variable by that name was found."
+                    )
                 else:
                     depend_i_variable_data = np.array(all_variable_data[depend_i_variable_name])
 
                     if not record_name_found:
                         dimension_number = i - 1
                     else:
                         dimension_number = i
 
-                    if depend_i_variable_data.size != 0 and len(depend_i_variable_data.shape) == 1 and \
-                            len(var_data.shape) > dimension_number and \
-                            (depend_i_variable_data.shape[0] == var_data.shape[dimension_number]):
+                    if (
+                        depend_i_variable_data.size != 0
+                        and len(depend_i_variable_data.shape) == 1
+                        and len(var_data.shape) > dimension_number
+                        and (depend_i_variable_data.shape[0] == var_data.shape[dimension_number])
+                    ):
                         return_list.append((depend_i_variable_name, dim_size, True, False))
                         continue
-                    elif len(depend_i_variable_data.shape) > 1 and \
-                            depend_i_variable_data.size != 0 and \
-                            len(var_data.shape) > dimension_number and \
-                            (depend_i_variable_data.shape[1] == var_data.shape[dimension_number]):
+                    elif (
+                        len(depend_i_variable_data.shape) > 1
+                        and depend_i_variable_data.size != 0
+                        and len(var_data.shape) > dimension_number
+                        and (depend_i_variable_data.shape[1] == var_data.shape[dimension_number])
+                    ):
                         return_list.append((depend_i_variable_name + "_dim", dim_size, True, False))
                         continue
                     else:
-                        print(f"Warning: Variable {var_name} listed DEPEND_{str(i)} as {depend_i_variable_name}"
-                              f", but that variable's dimensions do not match {var_name}'s dimensions.")
+                        print(
+                            f"Warning: Variable {var_name} listed DEPEND_{str(i)} as {depend_i_variable_name}"
+                            f", but that variable's dimensions do not match {var_name}'s dimensions."
+                        )
 
             # There may be occasions where there was no time-varying reccord identified, but the users intended for it
             # to exist.  Thus, all the DEPEND_X's are off by 1.  We should still try to incorporate those.
-            if 'DEPEND_' + str(i - 1) in var_atts and not record_name_found:
-                depend_i_variable_name = var_atts['DEPEND_' + str(i - 1)]
+            if "DEPEND_" + str(i - 1) in var_atts and not record_name_found:
+                depend_i_variable_name = var_atts["DEPEND_" + str(i - 1)]
                 if depend_i_variable_name in all_variable_properties:
                     depend_i_variable_data = np.array(all_variable_data[depend_i_variable_name])
-                    if depend_i_variable_data.size != 0 and len(depend_i_variable_data.shape) == 1 and \
-                            len(var_data.shape) > i - 1 and \
-                            (depend_i_variable_data.shape[0] == var_data.shape[i - 1]):
-                        print(f"Warning: Variable {var_name} has no determined time-varying component, but  "
-                              f"{depend_i_variable_name} was determined to match closely with one of the dimensions."
-                              f"  It will be set automatically for convenience.")
+                    if (
+                        depend_i_variable_data.size != 0
+                        and len(depend_i_variable_data.shape) == 1
+                        and len(var_data.shape) > i - 1
+                        and (depend_i_variable_data.shape[0] == var_data.shape[i - 1])
+                    ):
+                        print(
+                            f"Warning: Variable {var_name} has no determined time-varying component, but  "
+                            f"{depend_i_variable_name} was determined to match closely with one of the dimensions."
+                            f"  It will be set automatically for convenience."
+                        )
                         return_list.append((depend_i_variable_name, dim_size, True, False))
                         continue
-                    elif len(depend_i_variable_data.shape) > 1 and \
-                            depend_i_variable_data.size != 0 and \
-                            len(var_data.shape) > i - 1 and \
-                            (depend_i_variable_data.shape[1] == var_data.shape[i - 1]):
-                        print(f"Warning: Variable {var_name} has no determined time-varying component, but  "
-                              f"{depend_i_variable_name} was determined to match closely with one of the dimensions."
-                              f"  It will be set automatically for convenience.")
+                    elif (
+                        len(depend_i_variable_data.shape) > 1
+                        and depend_i_variable_data.size != 0
+                        and len(var_data.shape) > i - 1
+                        and (depend_i_variable_data.shape[1] == var_data.shape[i - 1])
+                    ):
+                        print(
+                            f"Warning: Variable {var_name} has no determined time-varying component, but  "
+                            f"{depend_i_variable_name} was determined to match closely with one of the dimensions."
+                            f"  It will be set automatically for convenience."
+                        )
                         return_list.append((depend_i_variable_name + "_dim", dim_size, True, False))
                         continue
 
             # Check if the variable is itself a dimension
             if var_name in depend_variables:
-                if len(var_data.shape) == 2 and var_props["Last_Rec"] == 0:
+                if len(var_data.shape) == 2 and var_props.Last_Rec == 0:
                     if i == 1 and not record_name_found:
                         pass
                     else:
                         basic_dimension_name = var_name + "_dim"
                         return_list.append((basic_dimension_name, dim_size, True, False))
                         continue
-                elif var_props["Rec_Vary"] and var_props["Last_Rec"] != 0:
+                elif var_props.Rec_Vary and var_props.Last_Rec != 0:
                     basic_dimension_name = var_name + "_dim"
                     for x in return_list:
                         vn = x[0]
                         ds = x[1]
                         if vn == basic_dimension_name and dim_size != ds:
                             basic_dimension_name = var_name + "_dim" + str(i)
                     return_list.append((basic_dimension_name, dim_size, True, False))
@@ -479,76 +502,100 @@
             # If none of the above, check if a non-specific dimension name was already created with this dimension length
             for dim in created_regular_dims:
                 if dim_size == created_regular_dims[dim]:
                     return_list.append((dim, dim_size, True, False))
                     break
             else:
                 # If none of the above, create a new non-specific dimension name
-                return_list.append(('dim' + str(len(created_regular_dims)), dim_size, False, True))
-                created_regular_dims['dim' + str(len(created_regular_dims))] = dim_size
+                return_list.append(("dim" + str(len(created_regular_dims)), dim_size, False, True))
+                created_regular_dims["dim" + str(len(created_regular_dims))] = dim_size
 
     return return_list
 
 
-def _reformat_variable_dims_and_data(var_dims, var_data):
+def _reformat_variable_dims_and_data(
+    var_dims: List[str], var_data: Optional[np.ndarray]
+) -> Tuple[Union[str, List[str]], npt.NDArray]:
     if len(var_dims) > 0 and var_data is None:
         var_data = np.array([])
 
     # For some reason, there are times when the actual shape of the data doesn't match the dimensions listed.
     if var_data is not None:
         if len(np.array(var_data).shape) > len(var_dims):
             var_data = np.squeeze(var_data)
         if len(np.array(var_data).shape) < len(var_dims):
             var_data = np.expand_dims(var_data, axis=0)
 
     # Check if both dimensions and data are empty, if so, set the dimension to the empty dimension
     if var_data.size == 0 and not len(var_dims):
-        var_dims = 'dim_empty'
-
-    return var_dims, var_data
+        var_dims_: Union[str, List[str]] = "dim_empty"
+    else:
+        var_dims_ = var_dims
 
+    return var_dims_, var_data
 
-def _generate_xarray_data_variables(all_variable_data, all_variable_attributes,
-                                    all_variable_properties, fillval_to_nan):
 
+def _generate_xarray_data_variables(
+    all_variable_data: Dict[str, npt.NDArray],
+    all_variable_attributes: Dict[str, Any],
+    all_variable_properties: Dict[str, VDRInfo],
+    fillval_to_nan: bool,
+) -> Tuple[Dict[str, xr.Variable], Dict[str, int]]:
     # Import here to avoid xarray as a dependency of all of cdflib
     import xarray as xr
 
     # Make a list of all of the special variables in the file.  These are variables that are pointed to by
     # other variables.
     depend_variables = _discover_depend_variables(all_variable_data, all_variable_attributes, all_variable_properties)
-    created_unlimited_dims = {}  # These hold the records of the names/lengths of the created "unlimited" dimensions
-    created_regular_dims = {}  # These hold the records of the names/lengths of the standard dimensions of the variable
-    depend_dimensions = {}  # This will be used after the creation of DataArrays, to determine which are "data" and which are "coordinates"
-    created_vars = {}
+    created_unlimited_dims: Dict[str, int] = {}  # These hold the records of the names/lengths of the created "unlimited" dimensions
+    created_regular_dims: Dict[
+        str, int
+    ] = {}  # These hold the records of the names/lengths of the standard dimensions of the variable
+    depend_dimensions: Dict[
+        str, int
+    ] = {}  # This will be used after the creation of DataArrays, to determine which are "data" and which are "coordinates"
+    created_vars: Dict[str, xr.Variable] = {}
 
     for var_name in all_variable_data:
-        var_dims = []
+        var_dims: List[str] = []
         var_atts = all_variable_attributes[var_name]
         var_data = np.array(all_variable_data[var_name])
         var_props = all_variable_properties[var_name]
 
         # Determine the dimension name of the CDF Records, based on all info in the file
-        record_dim_name, dependency, newly_created = _determine_record_dimensions(var_name, var_atts, var_data,
-                                                                                  var_props, depend_variables,
-                                                                                  all_variable_data,
-                                                                                  all_variable_properties,
-                                                                                  created_unlimited_dims)
+        record_dim_name, dependency, newly_created = _determine_record_dimensions(
+            var_name,
+            var_atts,
+            var_data,
+            var_props,
+            depend_variables,
+            all_variable_data,
+            all_variable_properties,
+            created_unlimited_dims,
+        )
         # Append the dimension name to the list of dimensions
         if record_dim_name:
             var_dims.append(record_dim_name)
             if dependency:
                 depend_dimensions[record_dim_name] = len(var_data)
             if newly_created:
                 created_unlimited_dims[record_dim_name] = len(var_data)
 
         # Determine the dimension names of the labeled Dimensions in the CDF file
-        returned_dimension_info = _determine_dimension_names(var_name, var_atts, var_data, var_props, depend_variables,
-                                                             all_variable_data, all_variable_properties,
-                                                             created_regular_dims, record_dim_name)
+        returned_dimension_info = _determine_dimension_names(
+            var_name,
+            var_atts,
+            var_data,
+            var_props,
+            depend_variables,
+            all_variable_data,
+            all_variable_properties,
+            created_regular_dims,
+            record_dim_name,
+        )
 
         # Append the dimensions to the list of defined dimension names
         for dimension_dim_names, dimension_size, dependency, newly_created in returned_dimension_info:
             if dimension_dim_names:
                 var_dims.append(dimension_dim_names)
                 if dependency:
                     depend_dimensions[dimension_dim_names] = dimension_size
@@ -564,58 +611,67 @@
 
         # If the user wants to convert all the FILLVAL values to NaNs, we got them covered
         if fillval_to_nan:
             var_data = _convert_fillvals_to_nan(var_data, var_atts, var_props)
 
         # Finally, create the new variable
         try:
-            created_vars[var_name] = xr.Variable(var_dims, var_data, attrs=var_atts)
+            created_vars[var_name] = xr.Variable(var_dims, var_data, attrs=var_atts)  # type: ignore[no-untyped-call]
         except Exception as e:
-            print(f'ERROR: Creating Variable {var_name} ran into exception: {e}')
+            print(f"ERROR: Creating Variable {var_name} ran into exception: {e}")
 
     return created_vars, depend_dimensions
 
 
-def _verify_dimension_sizes(created_data_vars, created_coord_vars):
-
+def _verify_dimension_sizes(created_data_vars: Dict[str, xr.Variable], created_coord_vars: Dict[str, xr.Variable]) -> None:
     for var in created_data_vars:
         for d in created_data_vars[var].dims:
+            d = cast(str, d)
             if d in created_data_vars:
                 if created_data_vars[d].dims != (d,):
-                    raise Exception(f'ERROR: Variable \"{var}\" contains the dimensions {created_data_vars[var].dims}. '
-                                    f'Dimension \"{d}\" is a data variable, but '
-                                    f'its dimensions must be equal to itself. '
-                                    f'Instead, its dimensions are {created_data_vars[d].dims}. '
-                                    f'This is likely due to issues with \"DEPEND_X\" attributes in either {var} or {d}')
+                    raise Exception(
+                        f'ERROR: Variable "{var}" contains the dimensions {created_data_vars[var].dims}. '
+                        f'Dimension "{d}" is a data variable, but '
+                        f"its dimensions must be equal to itself. "
+                        f"Instead, its dimensions are {created_data_vars[d].dims}. "
+                        f'This is likely due to issues with "DEPEND_X" attributes in either {var} or {d}'
+                    )
             if d in created_coord_vars:
                 if created_coord_vars[d].dims != (d,):
-                    raise Exception(f'ERROR: Variable \"{var}\" contains the dimensions {created_data_vars[var].dims}. '
-                                    f'Dimension \"{d}\" is a data variable, but '
-                                    f'its dimensions must be equal to itself.  '
-                                    f'Instead, its dimensions are {created_coord_vars[d].dims}.  '
-                                    f'This is likely due to issues with \"DEPEND_X\" attributes in either {var} or {d}')
+                    raise Exception(
+                        f'ERROR: Variable "{var}" contains the dimensions {created_data_vars[var].dims}. '
+                        f'Dimension "{d}" is a data variable, but '
+                        f"its dimensions must be equal to itself.  "
+                        f"Instead, its dimensions are {created_coord_vars[d].dims}.  "
+                        f'This is likely due to issues with "DEPEND_X" attributes in either {var} or {d}'
+                    )
     for var in created_coord_vars:
         for d in created_coord_vars[var].dims:
+            d = cast(str, d)
             if d in created_data_vars:
                 if created_data_vars[d].dims != (d,):
-                    raise Exception(f'ERROR: Variable \"{var}\" contains the dimensions {created_coord_vars[var].dims}. '
-                                    f'Dimension \"{d}\" is a data variable, but '
-                                    f'its dimensions must be equal to itself.  '
-                                    f'Instead, its dimensions are {created_data_vars[d].dims}.  '
-                                    f'This is likely due to issues with \"DEPEND_X\" attributes in either {var} or {d}')
+                    raise Exception(
+                        f'ERROR: Variable "{var}" contains the dimensions {created_coord_vars[var].dims}. '
+                        f'Dimension "{d}" is a data variable, but '
+                        f"its dimensions must be equal to itself.  "
+                        f"Instead, its dimensions are {created_data_vars[d].dims}.  "
+                        f'This is likely due to issues with "DEPEND_X" attributes in either {var} or {d}'
+                    )
             if d in created_coord_vars:
                 if created_coord_vars[d].dims != (d,):
-                    raise Exception(f'ERROR: Variable \"{var}\" contains the dimensions {created_coord_vars[var].dims}. '
-                                    f'Dimension \"{d}\" is a data variable, but '
-                                    f'its dimensions must be equal to itself.  '
-                                    f'Instead, its dimensions are {created_coord_vars[d].dims}.  '
-                                    f'This is likely due to issues with \"DEPEND_X\" attributes in either {var} or {d}')
+                    raise Exception(
+                        f'ERROR: Variable "{var}" contains the dimensions {created_coord_vars[var].dims}. '
+                        f'Dimension "{d}" is a data variable, but '
+                        f"its dimensions must be equal to itself.  "
+                        f"Instead, its dimensions are {created_coord_vars[d].dims}.  "
+                        f'This is likely due to issues with "DEPEND_X" attributes in either {var} or {d}'
+                    )
 
 
-def cdf_to_xarray(filename, to_datetime=False, to_unixtime=False, fillval_to_nan=False):
+def cdf_to_xarray(filename: str, to_datetime: bool = False, to_unixtime: bool = False, fillval_to_nan: bool = False) -> xr.Dataset:
     """
     This function converts CDF files into XArray Dataset Objects.
 
     Parameters:
         filename (str):  The path to the CDF file to read
         to_datetime (bool, optional): Whether or not to convert CDF_EPOCH/EPOCH_16/TT2000 to datetime, or leave them as is
         to_unixtime (bool, optional): Whether or not to convert CDF_EPOCH/EPOCH_16/TT2000 to unixtime, or leave them as is
@@ -685,50 +741,48 @@
             5. Optionally, convert FILLVALs to NaNs in the data
             6. Optionally, convert CDF_EPOCH/EPOCH16/TT2000 variables to unixtime or datetime
             7. Create an XArray Variable object using the dimensions determined in steps 1 and 2, the attributes from steps 3 and 4, and then the variable data
         2. Gather all the Variable objects created in the first step, and separate them into data variables or coordinate variables
         3. Gather all global scope attributes in the CDF file
         4. Create an XArray Dataset objects with the data variables, coordinate variables, and global attributes.
     """
-    # Import here to avoid xarray as a dependency of all of cdflib
-    import xarray as xr
-
     # Convert the CDF file into a series of dicts, so we don't need to keep reading the file
     global_attributes, all_variable_attributes, all_variable_data, all_variable_properties = _convert_cdf_to_dicts(
-        filename, to_datetime=to_datetime, to_unixtime=to_unixtime)
+        filename, to_datetime=to_datetime, to_unixtime=to_unixtime
+    )
 
-    created_vars, depend_dimensions = _generate_xarray_data_variables(all_variable_data, all_variable_attributes,
-                                                                      all_variable_properties, fillval_to_nan)
+    created_vars, depend_dimensions = _generate_xarray_data_variables(
+        all_variable_data, all_variable_attributes, all_variable_properties, fillval_to_nan
+    )
 
     label_variables = _discover_label_variables(all_variable_attributes, all_variable_properties, all_variable_data)
     uncertainty_variables = _discover_uncertainty_variables(all_variable_attributes)
 
     # Determine which dimensions are coordinates vs actual data
     # Variables are considered coordinates if one of the other dimensions depends on them.
     # Otherwise, they are considered data coordinates.
-    created_coord_vars = {}
-    created_data_vars = {}
+    created_coord_vars: Dict[str, xr.Variable] = {}
+    created_data_vars: Dict[str, xr.Variable] = {}
     for var_name in created_vars:
-
         if var_name in label_variables:
             # If these are label variables, we'll deal with these later when the DEPEND variables come up
             continue
-        elif (var_name in depend_dimensions) or (var_name + '_dim' in depend_dimensions):
+        elif (var_name in depend_dimensions) or (var_name + "_dim" in depend_dimensions):
             # If these are DEPEND variables, add them to the DataSet coordinates
             created_coord_vars[var_name] = created_vars[var_name]
             # Check if these coordinate variable have associated labels
             for lab in label_variables:
                 if label_variables[lab] == var_name:  # Found one!
                     if len(created_vars[lab].dims) == len(created_vars[var_name].dims):
                         if created_vars[lab].size != created_vars[var_name].size:
                             print(f"Warning, label variable {lab} does not match the expected dimension sizes of {var_name}")
                         else:
                             created_vars[lab].dims = created_vars[var_name].dims
                     else:
-                        created_vars[lab].dims = created_vars[var_name].dims[-1]
+                        created_vars[lab].dims = (created_vars[var_name].dims[-1],)
                     # Add the labels to the coordinates as well
                     created_coord_vars[lab] = created_vars[lab]
         elif var_name in uncertainty_variables:
             # If there is an uncertainty variable, link it to the uncertainty along a dimension
             if created_vars[var_name].size == created_vars[uncertainty_variables[var_name]].size:
                 created_vars[var_name].dims = created_vars[uncertainty_variables[var_name]].dims
                 created_coord_vars[var_name] = created_vars[var_name]
```

### Comparing `cdflib-0.4.9/cdflib/cdfread.py` & `cdflib-1.0.0/cdflib/cdfread.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,485 +1,388 @@
-"""
-CDF Class
-##########
-
-To begin accessing the data within a CDF file, first create a new CDF class.
-This can be done with the following commands::
-
-    import cdflib
-
-    cdf_file = cdflib.CDF('/path/to/cdf_file.cdf')
-
-Then, you can call various functions on the variable.  For example::
-
-    x = cdf_file.varget("NameOfVariable", startrec=0, endrec=150)
-
-This command will return all data inside of the variable "Variable1", from
-records 0 to 150.
-
-Sample use::
-
-
-    import cdflib
-    swea_cdf_file = cdflib.CDF('/path/to/swea_file.cdf')
-    swea_cdf_file.cdf_info()
-    x = swea_cdf_file.varget('NameOfVariable')
-    swea_cdf_file.close()
-
-"""
 import gzip
 import hashlib
 import io
 import os
 import struct
 import sys
 import tempfile
 import urllib.request
 from pathlib import Path
-from typing import Dict, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 import cdflib.epochs as epoch
+from cdflib.dataclasses import (
+    AEDR,
+    VDR,
+    ADRInfo,
+    AttData,
+    CDFInfo,
+    CDRInfo,
+    GDRInfo,
+    VDRInfo,
+)
+from cdflib.s3 import S3object
 
-__all__ = ['CDF']
+__all__ = ["CDF"]
 
 
 class CDF:
     """
-    Main CDF class.
+    Read a CDF file into the CDF object. This object contains methods to load
+    the cdf file information, variable names, and values.
 
-    Parameters
-    ----------
-    path : Path, str
-        Path to CDF file.  This can be a link to a file in an S3 bucket as well.
-    validate : bool, optional
-        If True, validate the MD5 checksum of the CDF file.
-    string_encoding : str, optional
-        The encoding used to read strings. Defaults to 'ascii', which is what
-        the CDF internal format description prescribes as the encoding for
-        character strings. Other encodings may have been used to create files
-        however, and this keyword argument gives users the flexibility to read
-        those files.
-    s3_read_method: int, optional
-        If the user is specifying a file that lives within an AWS S3 bucket, this variable
-        defines how the file is read in.  The choices are:
-          - 1 will read the file into memory to load in memory)
-          - 2 will download the file to a tmp directory
-          - 3 reads the file in chunks directly from S3 over https
-
-    Notes
-    -----
-    An open file handle to the CDF file remains whilst a CDF object is live.
-    It is automatically cleaned up with the CDF instance is deleted.
+    Example
+    -------
+    >>> import cdflib
+    >>> cdf_file = cdflib.CDF('/path/to/cdf_file.cdf')
+    >>> cdf_file.cdf_info()
+    >>> x = cdf_file.varget("NameOfVariable", startrec=0, endrec=150)
     """
-    version = 3
-    release = 7
-    increment = 0
 
-    def __init__(self, path, validate=False, string_encoding='ascii', s3_read_method=1):
+    def __init__(self, path: Union[str, Path], validate: bool = False, string_encoding: str = "ascii", s3_read_method: int = 1):
+        """
+        Parameters
+        ----------
+        path : Path, str
+            Path to CDF file.  This can be a link to a file in an S3 bucket as well.
+        validate : bool, optional
+            If True, validate the MD5 checksum of the CDF file.
+        string_encoding : str, optional
+            The encoding used to read strings. Defaults to 'ascii', which is what
+            the CDF internal format description prescribes as the encoding for
+            character strings. Other encodings may have been used to create files
+            however, and this keyword argument gives users the flexibility to read
+            those files.
+        s3_read_method: int, optional
+            If the user is specifying a file that lives within an AWS S3 bucket, this variable
+            defines how the file is read in.  The choices are:
+            - 1 will read the file into memory to load in memory)
+            - 2 will download the file to a tmp directory
+            - 3 reads the file in chunks directly from S3 over https
 
-        try:
+        Notes
+        -----
+        An open file handle to the CDF file remains whilst a CDF object is live.
+        It is automatically cleaned up with the CDF instance is deleted.
+        """
+        if isinstance(path, Path):
             fname = path.absolute().as_posix()
-        except:
+        else:
             fname = path
+
+        self.file: Union[str, Path]
         if fname.startswith("s3://"):
             # later put in s3 'does it exist' checker
-            self.ftype = 's3'
+            self.ftype = "s3"
             self.file = fname  # path for files, fname for urls and S3
         elif fname.startswith("http://") or fname.startswith("https://"):
             # later put in url 404 'does it exist' checker
-            self.ftype = 'url'
+            self.ftype = "url"
             self.file = fname  # path for files, fname for urls and S3
         else:
-            self.ftype = 'file'
+            self.ftype = "file"
             path = Path(path).resolve().expanduser()
             if not path.is_file():
-                path = path.with_suffix('.cdf')
+                path = path.with_suffix(".cdf")
                 if not path.is_file():
-                    raise FileNotFoundError(f'{path} not found')
+                    raise FileNotFoundError(f"{path} not found")
             self.file = path  # path for files, fname for urls and S3
             self.file = path
 
         self.string_encoding = string_encoding
 
-        self._f = self._file_or_url_or_s3_handler(self.file, self.ftype, s3_read_method)
+        self._f = self._file_or_url_or_s3_handler(str(self.file), self.ftype, s3_read_method)
         magic_number = self._f.read(4).hex()
         compressed_bool = self._f.read(4).hex()
 
-        if magic_number not in ('cdf30001', 'cdf26002', '0000ffff'):
-            raise OSError(f'{path} is not a CDF file or a non-supported CDF!')
+        if magic_number not in ("cdf30001", "cdf26002", "0000ffff"):
+            raise OSError(f"{path} is not a CDF file or a non-supported CDF!")
 
-        self.cdfversion = 3 if magic_number == 'cdf30001' else 2
+        self.cdfversion = 3 if magic_number == "cdf30001" else 2
 
-        self._compressed = not (compressed_bool == '0000ffff')
+        self._compressed = not (compressed_bool == "0000ffff")
         self.compressed_file = None
-        self.temp_file = None
+        self.temp_file: Optional[Path] = None
 
         if self._compressed:
-            if self.ftype == 'url' or self.ftype == 's3':
+            if self.ftype == "url" or self.ftype == "s3":
                 if s3_read_method == 3:
                     # extra step, read entire file
                     self._f.seek(0)
-                    self._f = s3_fetchall(self._f.fhandle)
-                self._unstream_file(path, self._f)
+                    self._f = s3_fetchall(self._f.fhandle)  # type: ignore
+                self._unstream_file(self._f)
                 path = self.file
-            self._uncompress_file(path)
+            self._uncompress_file()
             if self.temp_file is None:
                 raise OSError("Decompression was unsuccessful.  Only GZIP compression is currently supported.")
 
             self.compressed_file = self.file
             self.file = self.temp_file
             self._f.close()
-            self._f = self.file.open('rb')
-            self.ftype = 'file'
+            self._f = self.file.open("rb")
+            self.ftype = "file"
 
-        if (self.cdfversion == 3):
+        if self.cdfversion == 3:
             cdr_info, foffs = self._read_cdr(8)
             gdr_info = self._read_gdr(foffs)
         else:
             cdr_info, foffs = self._read_cdr2(8)
             gdr_info = self._read_gdr2(foffs)
 
-        if cdr_info['md5'] and validate:
+        if cdr_info.md5 and validate:
             if not self._md5_validation():
-                raise OSError('This file fails the md5 checksum.')
+                raise OSError("This file fails the md5 checksum.")
 
-        if not cdr_info['format']:
-            raise OSError('This package does not support multi-format CDF')
+        if not cdr_info.format_:
+            raise OSError("This package does not support multi-format CDF")
 
-        if cdr_info['encoding'] in (3, 14, 15):
-            raise OSError('This package does not support CDFs with this ' +
-                          self._encoding_token(cdr_info['encoding']) +
-                          ' encoding')
+        if cdr_info.encoding in (3, 14, 15):
+            raise OSError("This package does not support CDFs with this " + self._encoding_token(cdr_info.encoding) + " encoding")
 
         # SET GLOBAL VARIABLES
-        self._post25 = cdr_info['post25']
-        self._version = cdr_info['version']
-        self._encoding = cdr_info['encoding']
-        self._majority = self._major_token(cdr_info['majority'])
-        self._copyright = cdr_info['copyright']
-        self._md5 = cdr_info['md5']
-        self._first_zvariable = gdr_info['first_zvariable']
-        self._first_rvariable = gdr_info['first_rvariable']
-        self._first_adr = gdr_info['first_adr']
-        self._num_zvariable = gdr_info['num_zvariables']
-        self._num_rvariable = gdr_info['num_rvariables']
-        self._rvariables_num_dims = gdr_info['rvariables_num_dims']
-        self._rvariables_dim_sizes = gdr_info['rvariables_dim_sizes']
-        self._num_att = gdr_info['num_attributes']
-        self._num_rdim = gdr_info['rvariables_num_dims']
-        self._rdim_sizes = gdr_info['rvariables_dim_sizes']
-        if (self.cdfversion == 3):
-            self._leap_second_updated = gdr_info['leapsecond_updated']
+        self._post25 = cdr_info.post25
+        self._version = cdr_info.version
+        self._encoding = cdr_info.encoding
+        self._majority = self._major_token(cdr_info.majority)
+        self._copyright = cdr_info.copyright_
+        self._md5 = cdr_info.md5
+        self._first_zvariable = gdr_info.first_zvariable
+        self._first_rvariable = gdr_info.first_rvariable
+        self._first_adr = gdr_info.first_adr
+        self._num_zvariable = gdr_info.num_zvariables
+        self._num_rvariable = gdr_info.num_rvariables
+        self._rvariables_num_dims = gdr_info.rvariables_num_dims
+        self._rvariables_dim_sizes = gdr_info.rvariables_dim_sizes
+        self._num_att = gdr_info.num_attributes
+        self._num_rdim = gdr_info.rvariables_num_dims
+        self._rdim_sizes = gdr_info.rvariables_dim_sizes
+        if self.cdfversion == 3:
+            self._leap_second_updated = gdr_info.leapsecond_updated
 
         if self.compressed_file is not None:
             self.compressed_file = None
 
-    def __del__(self):
+    def __del__(self) -> None:
         # This implicitly will delete a temporary uncompressed file if we
         # created it earlier.
-        self._f.close()
-        if self.temp_file is not None:
+        if hasattr(self, "_f") and hasattr(self._f, "close"):
+            self._f.close()
+        if hasattr(self, "temp_file") and self.temp_file is not None:
             os.remove(self.temp_file)
 
-    def __getitem__(self, variable: str) -> np.ndarray:
+    def __getitem__(self, variable: str) -> Union[str, np.ndarray]:
         return self.varget(variable)
 
-    def __enter__(self):
+    def __enter__(self) -> "CDF":
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         return
 
-    def close(self):
-        pass
-
-    def cdf_info(self):
+    def cdf_info(self) -> CDFInfo:
         """
         Returns a dictionary that shows the basic CDF information.
 
-        This information includes
+        Returns
+        -------
+        CDFInfo
+        """
+        varnames = self._get_varnames()
+        return CDFInfo(
+            self.file,
+            self._version,
+            self._encoding,
+            self._majority,
+            varnames[0],
+            varnames[1],
+            self._get_attnames(),
+            self._copyright,
+            self._md5,
+            self._num_rdim,
+            self._rdim_sizes,
+            self._compressed,
+        )
 
-                +---------------+--------------------------------------------------------------------------------+
-                | ['CDF']       | the name of the CDF                                                            |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['Version']   | the version of the CDF                                                         |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['Encoding']  | the endianness of the CDF                                                      |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['Majority']  | the row/column majority                                                        |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['zVariables']| a list of the names of the zVariables                                          |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['rVariables']| a list of the names of the rVariables                                          |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['Attributes']| a list of dictionary objects that contain {attribute_name : scope}             |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['Checksum']  | the checksum indicator                                                         |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['Num_rdim']  | the number of dimensions, applicable only to rVariables                        |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['rDim_sizes'] | the dimensional sizes, applicable only to rVariables                          |
-                +----------------+-------------------------------------------------------------------------------+
-                | ['Compressed']| CDF is compressed at the file-level                                            |
-                +---------------+--------------------------------------------------------------------------------+
-                | ['LeapSecondUpdated']| The last updated for the leap second table, if applicable               |
-                +---------------+--------------------------------------------------------------------------------+
-
-        """
-        mycdf_info = {}
-        mycdf_info['CDF'] = self.file
-        mycdf_info['Version'] = self._version
-        mycdf_info['Encoding'] = self._encoding
-        mycdf_info['Majority'] = self._majority
-        mycdf_info['rVariables'], mycdf_info['zVariables'] = self._get_varnames()
-        mycdf_info['Attributes'] = self._get_attnames()
-        mycdf_info['Copyright'] = self._copyright
-        mycdf_info['Checksum'] = self._md5
-        mycdf_info['Num_rdim'] = self._num_rdim
-        mycdf_info['rDim_sizes'] = self._rdim_sizes
-        mycdf_info['Compressed'] = self._compressed
-        if (self.cdfversion > 2):
-            mycdf_info['LeapSecondUpdated'] = self._leap_second_updated
-        return mycdf_info
-
-    def varinq(self, variable):
-        """
-        Returns a dictionary that shows the basic variable information.
-
-        This information includes
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Variable']    | the name of the variable                                                       |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Num']         | the variable number                                                            |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Var_Type']    | the variable type: zVariable or rVariable                                      |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Data_Type']   | the variable's CDF data type                                                   |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Num_Elements']| the number of elements of the variable                                         |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Num_Dims']    | the dimensionality of the variable record                                      |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Dim_Sizes']   | the shape of the variable record                                               |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Sparse']      | the variable's record sparseness                                               |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Last_Rec']    | the maximum written record number (0-based)                                    |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Dim_Vary']    | the dimensional variance(s)                                                    |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Rec_Vary']    | the record variance                                                            |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Pad']         | the padded value if set                                                        |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Compress']    | the GZIP compression level, 0 to 9. 0 if not compressed                        |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Block_Factor']| the blocking factor if the variable is compressed                              |
-                +-----------------+--------------------------------------------------------------------------------+
+    def varinq(self, variable: str) -> VDRInfo:
+        """
+        Get basic variable information.
 
-        Parameters
-        ----------
-        variable :
+        Returns
+        -------
+        VDRInfo
         """
         vdr_info = self.vdr_info(variable)
 
-        var = {}
-        var['Variable'] = vdr_info['name']
-        var['Num'] = vdr_info['variable_number']
-        var['Var_Type'] = self._variable_token(vdr_info['section_type'])
-        var['Data_Type'] = vdr_info['data_type']
-        var['Data_Type_Description'] = self._datatype_token(vdr_info['data_type'])
-        var['Num_Elements'] = vdr_info['num_elements']
-        var['Num_Dims'] = vdr_info['num_dims']
-        var['Dim_Sizes'] = vdr_info['dim_sizes']
-        var['Sparse'] = self._sparse_token(vdr_info['sparse'])
-        var['Last_Rec'] = vdr_info['max_records']
-        var['Rec_Vary'] = vdr_info['record_vary']
-        var['Dim_Vary'] = vdr_info['dim_vary']
-        if ('pad' in vdr_info):
-            var['Pad'] = vdr_info['pad']
-        var['Compress'] = vdr_info['compression_level']
-        if ('blocking_factor' in vdr_info):
-            var['Block_Factor'] = vdr_info['blocking_factor']
-
-        return var
+        return VDRInfo(
+            vdr_info.name,
+            vdr_info.variable_number,
+            self._variable_token(vdr_info.section_type),
+            vdr_info.data_type,
+            self._datatype_token(vdr_info.data_type),
+            vdr_info.num_elements,
+            vdr_info.num_dims,
+            vdr_info.dim_sizes,
+            self._sparse_token(vdr_info.sparse),
+            vdr_info.max_rec,
+            vdr_info.record_vary,
+            vdr_info.dim_vary,
+            vdr_info.compression_level,
+            vdr_info.pad,
+            vdr_info.blocking_factor,
+        )
 
-    def attinq(self, attribute=None):
+    def attinq(self, attribute: Union[str, int]) -> ADRInfo:
         """
         Get attribute information.
 
         Parameters
         ----------
         attribute : str, int
             Attribute to get information for.
 
         Returns
         -------
-        dict
-            Dictionary of attribution infromation.
+        ADRInfo
         """
         position = self._first_adr
         if isinstance(attribute, str):
             for _ in range(0, self._num_att):
                 name, next_adr = self._read_adr_fast(position)
                 if name.strip().lower() == attribute.strip().lower():
                     return self._read_adr(position)
 
                 position = next_adr
-            raise KeyError(f'No attribute {attribute}')
+            raise KeyError(f"No attribute {attribute}")
 
         elif isinstance(attribute, int):
-            if (attribute < 0 or attribute > self._num_zvariable):
-                raise KeyError(f'No attribute {attribute}')
+            if attribute < 0 or attribute > self._num_zvariable:
+                raise KeyError(f"No attribute {attribute}")
             for _ in range(0, attribute):
                 name, next_adr = self._read_adr_fast(position)
                 position = next_adr
 
             return self._read_adr(position)
         else:
-            raise ValueError('attribute keyword must be a string or integer')
+            raise ValueError("attribute keyword must be a string or integer")
 
-    def print_attrs(self):
-        """
-        Print all attribute information.
-        """
-        attrs = self._get_attnames()
-        print(attrs)
-        for x in range(0, self._num_att):
-            name = list(attrs[x].keys())[0]
-            print('NAME: ' + name + ', NUMBER: ' + str(x) + ', SCOPE: ' + attrs[x][name])
-        return attrs
-
-    def attget(self, attribute=None, entry=None, to_np=True):
+    def attget(self, attribute: Union[str, int], entry: Optional[Union[str, int]] = None) -> AttData:
         """
         Returns the value of the attribute at the entry number provided.
 
         A variable name can be used instead of its corresponding
         entry number.
 
         Parameters
         ----------
-        attribute : str, int, optional
+        attribute : str, int
             Attribute name or number to get.
         entry : int, optional
-        tp_np : bool, optional
-            If True, return a numpy array.
 
         Returns
         -------
-        dict
-            A dictionary is returned with the following defined keys
-
-            +-----------------+--------------------------------------------------------------------------------+
-            | ['Item_Size']   | the number of bytes for each entry value                                       |
-            +-----------------+--------------------------------------------------------------------------------+
-            | ['Num_Items']   | total number of values extracted                                               |
-            +-----------------+--------------------------------------------------------------------------------+
-            | ['Data_Type']   | the CDF data type                                                              |
-            +-----------------+--------------------------------------------------------------------------------+
-            | ['Data']        | retrieved attribute data as a scalar value, a numpy array or a string          |
-            +-----------------+--------------------------------------------------------------------------------+
-
+        AttData
         """
         # Starting position
         position = self._first_adr
 
         # Get Correct ADR
         adr_info = None
         if isinstance(attribute, str):
             for _ in range(0, self._num_att):
                 name, next_adr = self._read_adr_fast(position)
                 if name.strip().lower() == attribute.strip().lower():
                     adr_info = self._read_adr(position)
-                    if isinstance(entry, str) and adr_info['scope'] == 1:
+                    if isinstance(entry, str) and adr_info.scope == 1:
                         # If the user has specified a string entry, they are obviously looking for a variable attribute.
                         # Filter out any global attributes that may have the same name.
                         adr_info = None
                         position = next_adr
                         continue
                     break
                 else:
                     position = next_adr
 
             if adr_info is None:
-                raise KeyError(f'No attribute {attribute} for entry {entry}')
+                raise KeyError(f"No attribute {attribute} for entry {entry}")
 
         elif isinstance(attribute, int):
             if (attribute < 0) or (attribute > self._num_att):
-                raise KeyError(f'No attribute {attribute}')
+                raise KeyError(f"No attribute {attribute}")
             if not isinstance(entry, int):
-                raise TypeError(f'{entry} has to be a number.')
+                raise TypeError(f"{entry} has to be a number.")
 
             for _ in range(0, attribute):
                 name, next_adr = self._read_adr_fast(position)
                 position = next_adr
             adr_info = self._read_adr(position)
         else:
-            raise ValueError('Please set attribute keyword equal to '
-                             'the name or number of an attribute')
+            raise ValueError("Please set attribute keyword equal to " "the name or number of an attribute")
 
         # Find the correct entry from the "entry" variable
-        if adr_info['scope'] == 1:
+        if adr_info.scope == 1:
             if not isinstance(entry, int):
                 raise ValueError('"entry" must be an integer')
-            num_entry_string = 'num_gr_entry'
-            first_entry_string = 'first_gr_entry'
-            max_entry_string = 'max_gr_entry'
+            num_entry_string = "num_gr_entry"
+            first_entry_string = "first_gr_entry"
+            max_entry_string = "max_gr_entry"
             entry_num = entry
         else:
             var_num = -1
             zvar = False
             if isinstance(entry, str):
                 # a zVariable?
                 positionx = self._first_zvariable
                 for x in range(0, self._num_zvariable):
                     name, vdr_next = self._read_vdr_fast(positionx)
-                    if (name.strip().lower() == entry.strip().lower()):
+                    if name.strip().lower() == entry.strip().lower():
                         var_num = x
                         zvar = True
                         break
                     positionx = vdr_next
                 if var_num == -1:
                     # a rVariable?
                     positionx = self._first_rvariable
                     for x in range(0, self._num_rvariable):
                         name, vdr_next = self._read_vdr_fast(positionx)
-                        if (name.strip().lower() == entry.strip().lower()):
+                        if name.strip().lower() == entry.strip().lower():
                             var_num = x
                             break
                         positionx = vdr_next
                 if var_num == -1:
-                    raise ValueError(
-                        f'No variable by this name: {entry}')
+                    raise ValueError(f"No variable by this name: {entry}")
                 entry_num = var_num
             else:
-                if (self._num_zvariable > 0 and self._num_rvariable > 0):
-                    raise ValueError('This CDF has both r and z variables. '
-                                     'Use variable name instead')
+                if self._num_zvariable > 0 and self._num_rvariable > 0:
+                    raise ValueError("This CDF has both r and z variables. " "Use variable name instead")
                 if self._num_zvariable > 0:
                     zvar = True
                 entry_num = entry
             if zvar:
-                num_entry_string = 'num_z_entry'
-                first_entry_string = 'first_z_entry'
-                max_entry_string = 'max_z_entry'
+                num_entry_string = "num_z_entry"
+                first_entry_string = "first_z_entry"
+                max_entry_string = "max_z_entry"
             else:
-                num_entry_string = 'num_gr_entry'
-                first_entry_string = 'first_gr_entry'
-                max_entry_string = 'max_gr_entry'
-        if entry_num > adr_info[max_entry_string]:
-            raise ValueError('The entry does not exist')
-        return self._get_attdata(adr_info, entry_num, adr_info[num_entry_string],
-                                 adr_info[first_entry_string], to_np=to_np)
-
-    def varget(self, variable=None, epoch=None, starttime=None,
-               endtime=None, startrec=0, endrec=None,
-               record_range_only=False, expand=False, to_np=True):
+                num_entry_string = "num_gr_entry"
+                first_entry_string = "first_gr_entry"
+                max_entry_string = "max_gr_entry"
+        if entry_num > getattr(adr_info, max_entry_string):
+            raise ValueError("The entry does not exist")
+        return self._get_attdata(adr_info, entry_num, getattr(adr_info, num_entry_string), getattr(adr_info, first_entry_string))
+
+    def varget(
+        self,
+        variable: Optional[str] = None,
+        epoch: Optional[str] = None,
+        starttime: Optional[epoch.epoch_types] = None,
+        endtime: Optional[epoch.epoch_types] = None,
+        startrec: int = 0,
+        endrec: Optional[int] = None,
+    ) -> Union[str, np.ndarray]:
         """
         Returns the variable data.
 
         Parameters
         ----------
         variable: str
             Variable name to fetch.
@@ -492,33 +395,14 @@
         Notes
         -----
         Variable can be entered either
         a name or a variable number. By default, it returns a
         'numpy.ndarray' or 'list' class object, depending on the
         data type, with the variable data and its specification.
 
-        If "expand" is set as True, a dictionary is returned
-        with the following defined keys for the output
-
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Rec_Ndim']         | the dimension number of each variable record                              |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Rec_Shape']        | the shape of the variable record dimensions                               |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Num_Records']      | the total number of records                                               |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Records_Returned'] | the number of records retrieved                                           |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Data_Type']        | the CDF data type                                                         |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Data']             | retrieved variable data                                                   |
-                +-----------------+--------------------------------------------------------------------------------+
-                | ['Real_Records']     | Record numbers for real data for sparse record variable in list           |
-                +-----------------+--------------------------------------------------------------------------------+
-
         By default, the full variable data is returned. To acquire
         only a portion of the data for a record-varying variable,
         either the time or record (0-based) range can be specified.
         'epoch' can be used to specify which time variable this
         variable depends on and is to be searched for the time range.
         For the ISTP-compliant CDFs, the time variable will come from
         the attribute 'DEPEND_0' from this variable. The function will
@@ -535,36 +419,36 @@
         [year month day hour minute second millisec microsec nanosec] for CDF_TIME_TT2000
         If not enough time components are presented, only the last item can have the floating
         portion for the sub-time components.
 
         Note: CDF's CDF_EPOCH16 data type uses 2 8-byte doubles for each data value.
         In Python, each value is presented as a complex or numpy.complex128.
         """
-        if (isinstance(variable, int) and self._num_zvariable > 0 and
-                self._num_rvariable > 0):
-            raise ValueError('This CDF has both r and z variables. '
-                             'Use variable name instead')
-
-        if ((starttime is not None or endtime is not None) and
-                (startrec != 0 or endrec is not None)):
-            raise ValueError('Can\'t specify both time and record range')
+        if isinstance(variable, int) and self._num_zvariable > 0 and self._num_rvariable > 0:
+            raise ValueError("This CDF has both r and z variables. " "Use variable name instead")
+
+        if (starttime is not None or endtime is not None) and (startrec != 0 or endrec is not None):
+            raise ValueError("Can't specify both time and record range")
 
         vdr_info = self.vdr_info(variable)
-        if (vdr_info['max_records'] < 0):
-            raise ValueError(f'No records found for variable {variable}')
+        if vdr_info.max_rec < 0:
+            raise ValueError(f"No records found for variable {variable}")
 
-        return self._read_vardata(vdr_info, epoch=epoch, starttime=starttime, endtime=endtime,
-                                    startrec=startrec, endrec=endrec, record_range_only=record_range_only,
-                                    expand=expand, to_np=to_np)
-
-    def vdr_info(self, variable: Union[str, int]):
-        if (isinstance(variable, int) and self._num_zvariable > 0 and
-                self._num_rvariable > 0):
-            raise ValueError('This CDF has both r and z variables. '
-                             'Use variable name instead')
+        return self._read_vardata(
+            vdr_info,
+            epoch=epoch,
+            starttime=starttime,
+            endtime=endtime,
+            startrec=startrec,
+            endrec=endrec,
+        )
+
+    def vdr_info(self, variable: Union[str, int]) -> VDR:
+        if isinstance(variable, int) and self._num_zvariable > 0 and self._num_rvariable > 0:
+            raise ValueError("This CDF has both r and z variables. " "Use variable name instead")
 
         if isinstance(variable, str):
             # Check z variables for the name, then r variables
             position = self._first_zvariable
             num_variables = self._num_zvariable
             vdr_info = None
             for zVar in [1, 0]:
@@ -583,365 +467,282 @@
                 position = self._first_zvariable
                 num_variable = self._num_zvariable
                 # zVar = True
             elif self._num_rvariable > 0:
                 position = self._first_rvariable
                 num_variable = self._num_rvariable
                 # zVar = False
-            if (variable < 0 or variable >= num_variable):
-                raise ValueError(
-                    f'No variable by this number: {variable}')
+            if variable < 0 or variable >= num_variable:
+                raise ValueError(f"No variable by this number: {variable}")
             for _ in range(0, variable):
                 name, next_vdr = self._read_vdr_fast(position)
                 position = next_vdr
             vdr_info = self._read_vdr(position)
         else:
-            raise ValueError('Please set variable keyword equal to '
-                             'the name or number of an variable')
+            raise ValueError("Please set variable keyword equal to " "the name or number of an variable")
 
         return vdr_info
 
-    def epochrange(self, epoch=None, starttime=None, endtime=None):
-        """
-        Get epoch range.
-
-        Returns a list of the record numbers, representing the
-        corresponding starting and ending records within the time
-        range from the epoch data. A None is returned if there is no
-        data either written or found in the time range.
-
-        Parameters
-        ----------
-        epoch :
-        starttime :
-        endtime :
-        """
-        return self.varget(variable=epoch, starttime=starttime,
-                           endtime=endtime, record_range_only=True)
-
-    def globalattsget(self, expand=False, to_np=True):
+    def globalattsget(self) -> Dict[str, List[Union[str, np.ndarray]]]:
         """
         Gets all global attributes.
 
         This function returns all of the global attribute entries,
         in a dictionary (in the form of ``'attribute': {entry: value}``
-        pairs) from a CDF. If there is no entry found, None is
-        returned. If expand is entered with non-False, then each
-        entry's data type is also returned in a list form as
-        [entry, 'CDF_xxxx']. For attributes without any entries,
-        they will also return with ``None`` value.
-
-        Parameters
-        ----------
-        expand : bool, optional
-        to_np : bool, optional
-            If True, return a numpy array.
+        pairs) from a CDF.
         """
         byte_loc = self._first_adr
-        return_dict = {}
+        return_dict: Dict[str, List[Union[str, np.ndarray]]] = {}
         for _ in range(self._num_att):
             adr_info = self._read_adr(byte_loc)
-            if (adr_info['scope'] != 1):
-                byte_loc = adr_info['next_adr_location']
+            if adr_info.scope != 1:
+                byte_loc = adr_info.next_adr_loc
                 continue
-            if (adr_info['num_gr_entry'] == 0):
-                if (expand is not False):
-                    return_dict[adr_info['name']] = None
-                byte_loc = adr_info['next_adr_location']
+            if adr_info.num_gr_entry == 0:
+                byte_loc = adr_info.next_adr_loc
                 continue
-            if (expand is False):
-                entries = []
-            else:
-                entries = {}
-            aedr_byte_loc = adr_info['first_gr_entry']
-            for _ in range(adr_info['num_gr_entry']):
-                aedr_info = self._read_aedr(aedr_byte_loc, to_np=to_np)
-                entryData = aedr_info['entry']
-                if (expand is False):
-
-                    # This exists to get rid of extraneous numpy arrays
-                    if isinstance(entryData, np.ndarray):
-                        if len(entryData) == 1:
-                            entryData = entryData[0]
+            entries = []
+            aedr_byte_loc = adr_info.first_gr_entry
+            for _ in range(adr_info.num_gr_entry):
+                aedr_info = self._read_aedr(aedr_byte_loc)
+                entryData = aedr_info.entry
+                # This exists to get rid of extraneous numpy arrays
+                if isinstance(entryData, np.ndarray):
+                    if len(entryData) == 1:
+                        entryData = entryData[0]
 
-                    entries.append(entryData)
-                else:
-                    entryWithType = []
-                    if (isinstance(entryData, str)):
-                        entryWithType.append(entryData)
-                    else:
-                        dataType = aedr_info['data_type']
-                        if (len(entryData.tolist()) == 1):
-                            if (dataType != 31 and dataType != 32 and dataType != 33):
-                                entryWithType.append(entryData.tolist()[0])
-                            else:
-                                if (dataType != 33):
-                                    entryWithType.append(epoch.CDFepoch.encode(entryData.tolist()[0],
-                                                                               iso_8601=False))
-                                else:
-                                    entryWithType.append(epoch.CDFepoch.encode(entryData.tolist()[0]))
-                        else:
-                            if (dataType != 31 and dataType != 32 and dataType != 33):
-                                entryWithType.append(entryData.tolist())
-                            else:
-                                if (dataType != 33):
-                                    entryWithType.append(epoch.CDFepoch.encode(entryData.tolist(),
-                                                                               iso_8601=False))
-                                else:
-                                    entryWithType.append(epoch.CDFepoch.encode(entryData.tolist()))
-                    entryWithType.append(self._datatype_token(aedr_info['data_type']))
-                    entries[aedr_info['entry_num']] = entryWithType
-                aedr_byte_loc = aedr_info['next_aedr']
-
-            if (len(entries) != 0):
-                if (expand is False):
-                    if (len(entries) == 1):
-                        return_dict[adr_info['name']] = entries[0]
-                    else:
-                        return_dict[adr_info['name']] = entries
-                else:
-                    return_dict[adr_info['name']] = entries
-            byte_loc = adr_info['next_adr_location']
+                entries.append(entryData)
+
+            return_dict[adr_info.name] = entries
+            byte_loc = adr_info.next_adr_loc
 
         return return_dict
 
-    def varattsget(self, variable=None, expand=False, to_np=True):
+    def varattsget(self, variable: Optional[str] = None) -> Dict[str, Union[None, str, np.ndarray]]:
         """
         Gets all variable attributes.
 
         Unlike attget, which returns a single attribute entry value,
         this function returns all of the variable attribute entries,
         in a dictionary (in the form of 'attribute': value pair) for
         a variable. If there is no entry found, None is returned.
-        If no variable name is provided, a list of variables are printed.
-        If expand is entered with non-False, then each entry's data
-        type is also returned in a list form as [entry, 'CDF_xxxx'].
-        For attributes without any entries, they will also return with
-        None value.
-
-        Parameters
-        ----------
-        variable :
-        expand : bool, optional
-        to_np: bool, optional
-            If True, return a numpy array.
         """
-        if (isinstance(variable, int) and self._num_zvariable > 0 and self._num_rvariable > 0):
-            raise ValueError('This CDF has both r and z variables. Use variable name')
+        if isinstance(variable, int) and self._num_zvariable > 0 and self._num_rvariable > 0:
+            raise ValueError("This CDF has both r and z variables. Use variable name")
         if isinstance(variable, str):
             position = self._first_zvariable
             num_variables = self._num_zvariable
-            for zVar in [1, 0]:
+            for zVar in [True, False]:
                 for _ in range(0, num_variables):
                     name, vdr_next = self._read_vdr_fast(position)
                     if name.strip().lower() == variable.strip().lower():
                         vdr_info = self._read_vdr(position)
-                        return self._read_varatts(vdr_info['variable_number'], zVar, expand, to_np=to_np)
+                        return self._read_varatts(vdr_info.variable_number, zVar)
                     position = vdr_next
                 position = self._first_rvariable
                 num_variables = self._num_rvariable
-            raise ValueError(f'No variable by this name: {variable}')
+            raise ValueError(f"No variable by this name: {variable}")
         elif isinstance(variable, int):
             if self._num_zvariable > 0:
                 num_variable = self._num_zvariable
                 zVar = True
             else:
                 num_variable = self._num_rvariable
                 zVar = False
-            if (variable < 0 or variable >= num_variable):
-                raise ValueError(f'No variable by this number: {variable}')
-            return self._read_varatts(variable, zVar, expand, to_np=to_np)
-        else:
-            raise ValueError('Please set variable keyword equal to '
-                             'the name or number of an variable')
-    def _uncompress_rle(self, data):
+            if variable < 0 or variable >= num_variable:
+                raise ValueError(f"No variable by this number: {variable}")
+            return self._read_varatts(variable, zVar)
+        else:
+            raise ValueError("Please set variable keyword equal to " "the name or number of an variable")
+
+    def _uncompress_rle(self, data: bytes) -> bytearray:
         result = bytearray()
         index = 0
         while index < len(data):
             value = data[index]
             if value == 0:
                 index += 1
                 count = data[index] + 1
                 result += b"\0" * count
             else:
                 result.append(value)
             index += 1
         return result
-    def _uncompress_file(self, path):
+
+    def _uncompress_file(self) -> None:
         """
         Writes the current file into a file in the temporary directory.
 
         If that doesn't work, create a new file in the CDFs directory.
         """
-        if (self.cdfversion == 3):
+        if self.cdfversion == 3:
             data_start, data_size, cType, _ = self._read_ccr(8)
         else:
             data_start, data_size, cType, _ = self._read_ccr2(8)
 
         if cType == 5:
             self._f.seek(data_start)
             decompressed_data = gzip.decompress(self._f.read(data_size))
         elif cType == 1:
             self._f.seek(data_start)
             decompressed_data = self._uncompress_rle(self._f.read(data_size))
         else:
             return
 
-        self.temp_file = Path(tempfile.NamedTemporaryFile(suffix='.cdf').name)
-        with self.temp_file.open('wb') as g:
-            g.write(bytearray.fromhex('cdf30001'))
-            g.write(bytearray.fromhex('0000ffff'))
+        self.temp_file = Path(tempfile.NamedTemporaryFile(suffix=".cdf").name)
+        with self.temp_file.open("wb") as g:
+            g.write(bytearray.fromhex("cdf30001"))
+            g.write(bytearray.fromhex("0000ffff"))
             g.write(decompressed_data)
 
-    def _read_ccr(self, byte_loc):
+    def _read_ccr(self, byte_loc: int) -> Tuple[int, int, int, int]:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(8), 'big')
+        block_size = int.from_bytes(self._f.read(8), "big")
         self._f.seek(byte_loc + 12)
-        cproffset = int.from_bytes(self._f.read(8), 'big')
+        cproffset = int.from_bytes(self._f.read(8), "big")
 
         data_start = byte_loc + 32
         data_size = block_size - 32
         cType, cParams = self._read_cpr(cproffset)
 
         return data_start, data_size, cType, cParams
 
-    def _read_ccr2(self, byte_loc):
+    def _read_ccr2(self, byte_loc: int) -> Tuple[int, int, int, int]:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big')
+        block_size = int.from_bytes(self._f.read(4), "big")
         self._f.seek(byte_loc + 8)
-        cproffset = int.from_bytes(self._f.read(4), 'big')
+        cproffset = int.from_bytes(self._f.read(4), "big")
 
         data_start = byte_loc + 20
         data_size = block_size - 20
         cType, cParams = self._read_cpr2(cproffset)
 
         return data_start, data_size, cType, cParams
 
-    def _read_cpr(self, byte_loc):
+    def _read_cpr(self, byte_loc: int) -> Tuple[int, int]:
         if self.cdfversion == 3:
             return self._read_cpr3(byte_loc)
         else:
             return self._read_cpr2(byte_loc)
 
-    def _read_cpr3(self, byte_loc):
+    def _read_cpr3(self, byte_loc: int) -> Tuple[int, int]:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(8), 'big')
+        block_size = int.from_bytes(self._f.read(8), "big")
         cpr = self._f.read(block_size - 8)
 
-        cType = int.from_bytes(cpr[4:8], 'big')
-        cParams = int.from_bytes(cpr[16:20], 'big')
+        cType = int.from_bytes(cpr[4:8], "big")
+        cParams = int.from_bytes(cpr[16:20], "big")
 
         return cType, cParams
 
-    def _read_cpr2(self, byte_loc):
+    def _read_cpr2(self, byte_loc: int) -> Tuple[int, int]:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big')
+        block_size = int.from_bytes(self._f.read(4), "big")
         cpr = self._f.read(block_size - 4)
 
-        cType = int.from_bytes(cpr[4:8], 'big')
-        cParams = int.from_bytes(cpr[16:20], 'big')
+        cType = int.from_bytes(cpr[4:8], "big")
+        cParams = int.from_bytes(cpr[16:20], "big")
 
         return cType, cParams
 
     def _md5_validation(self) -> bool:
         """
         Verifies the MD5 checksum.
         Only used in the __init__() function
         """
         if self.compressed_file is not None:
-            fh = self.compressed_file.open('rb')
+            fh = self.compressed_file.open("rb")
         else:
             fh = self._f
 
         md5 = hashlib.md5()
         block_size = 16384
         fh.seek(-16, 2)
         remaining = fh.tell()  # File size minus checksum size
         fh.seek(0)
-        while (remaining > block_size):
+        while remaining > block_size:
             data = fh.read(block_size)
             remaining = remaining - block_size
             md5.update(data)
 
-        if (remaining > 0):
+        if remaining > 0:
             data = fh.read(remaining)
             md5.update(data)
 
         existing_md5 = fh.read(16).hex()
 
         if self.compressed_file is not None:
             fh.close()
 
         return md5.hexdigest() == existing_md5
 
     @staticmethod
-    def _encoding_token(encoding):
-        encodings = {1: 'NETWORK',
-                     2: 'SUN',
-                     3: 'VAX',
-                     4: 'DECSTATION',
-                     5: 'SGi',
-                     6: 'IBMPC',
-                     7: 'IBMRS',
-                     9: 'PPC',
-                     11: 'HP',
-                     12: 'NeXT',
-                     13: 'ALPHAOSF1',
-                     14: 'ALPHAVMSd',
-                     15: 'ALPHAVMSg',
-                     16: 'ALPHAVMSi'}
+    def _encoding_token(encoding: int) -> str:
+        encodings = {
+            1: "NETWORK",
+            2: "SUN",
+            3: "VAX",
+            4: "DECSTATION",
+            5: "SGi",
+            6: "IBMPC",
+            7: "IBMRS",
+            9: "PPC",
+            11: "HP",
+            12: "NeXT",
+            13: "ALPHAOSF1",
+            14: "ALPHAVMSd",
+            15: "ALPHAVMSg",
+            16: "ALPHAVMSi",
+        }
         return encodings[encoding]
 
     @staticmethod
-    def _major_token(major):
-        majors = {1: 'Row_major',
-                  2: 'Column_major'}
+    def _major_token(major: int) -> str:
+        majors = {1: "Row_major", 2: "Column_major"}
         return majors[major]
 
     @staticmethod
-    def _scope_token(scope):
-        scopes = {1: 'Global',
-                  2: 'Variable'}
+    def _scope_token(scope: int) -> str:
+        scopes = {1: "Global", 2: "Variable"}
         return scopes[scope]
 
     @staticmethod
-    def _variable_token(variable):
-        variables = {3: 'rVariable',
-                     8: 'zVariable'}
+    def _variable_token(variable: int) -> str:
+        variables = {3: "rVariable", 8: "zVariable"}
         return variables[variable]
 
     @staticmethod
-    def _datatype_token(datatype):
-        datatypes = {1: 'CDF_INT1',
-                     2: 'CDF_INT2',
-                     4: 'CDF_INT4',
-                     8: 'CDF_INT8',
-                     11: 'CDF_UINT1',
-                     12: 'CDF_UINT2',
-                     14: 'CDF_UINT4',
-                     21: 'CDF_REAL4',
-                     22: 'CDF_REAL8',
-                     31: 'CDF_EPOCH',
-                     32: 'CDF_EPOCH16',
-                     33: 'CDF_TIME_TT2000',
-                     41: 'CDF_BYTE',
-                     44: 'CDF_FLOAT',
-                     45: 'CDF_DOUBLE',
-                     51: 'CDF_CHAR',
-                     52: 'CDF_UCHAR'}
+    def _datatype_token(datatype: int) -> str:
+        datatypes = {
+            1: "CDF_INT1",
+            2: "CDF_INT2",
+            4: "CDF_INT4",
+            8: "CDF_INT8",
+            11: "CDF_UINT1",
+            12: "CDF_UINT2",
+            14: "CDF_UINT4",
+            21: "CDF_REAL4",
+            22: "CDF_REAL8",
+            31: "CDF_EPOCH",
+            32: "CDF_EPOCH16",
+            33: "CDF_TIME_TT2000",
+            41: "CDF_BYTE",
+            44: "CDF_FLOAT",
+            45: "CDF_DOUBLE",
+            51: "CDF_CHAR",
+            52: "CDF_UCHAR",
+        }
         return datatypes[datatype]
 
     @staticmethod
-    def _sparse_token(sparse):
-        sparses = {0: 'No_sparse',
-                   1: 'Pad_sparse',
-                   2: 'Prev_sparse'}
+    def _sparse_token(sparse: int) -> str:
+        sparses = {0: "No_sparse", 1: "Pad_sparse", 2: "Prev_sparse"}
         return sparses[sparse]
 
-    def _get_varnames(self):
+    def _get_varnames(self) -> Tuple[List[str], List[str]]:
         zvars = []
         rvars = []
         if self._num_zvariable > 0:
             position = self._first_zvariable
             num_variable = self._num_zvariable
             for _ in range(0, num_variable):
                 name, next_vdr = self._read_vdr_fast(position)
@@ -952,921 +753,829 @@
             num_variable = self._num_rvariable
             for _ in range(0, num_variable):
                 name, next_vdr = self._read_vdr_fast(position)
                 rvars.append(name)
                 position = next_vdr
         return rvars, zvars
 
-    def _get_attnames(self):
+    def _get_attnames(self) -> List[Dict[str, str]]:
         attrs = []
         position = self._first_adr
         for _ in range(0, self._num_att):
             attr = {}
             adr_info = self._read_adr(position)
-            attr[adr_info['name']] = self._scope_token(int(adr_info['scope']))
+            attr[adr_info.name] = self._scope_token(adr_info.scope)
             attrs.append(attr)
-            position = adr_info['next_adr_location']
+            position = adr_info.next_adr_loc
         return attrs
 
-    def _read_cdr(self, byte_loc: int):
+    def _read_cdr(self, byte_loc: int) -> Tuple[CDRInfo, int]:
         """
         Read a CDF descriptor record (CDR).
         """
         self._f.seek(0)
         self._f.seek(byte_loc)
-        block_size = int.from_bytes(self._f.read(8), 'big')
+        block_size = int.from_bytes(self._f.read(8), "big")
         cdr = self._f.read(block_size - 8)
         foffs = self._f.tell()
         # _ = int.from_bytes(cdr[0:4],'big') #Section Type
         # gdroff = int.from_bytes(cdr[4:12], 'big')  # GDR Location
-        version = int.from_bytes(cdr[12:16], 'big')
+        version = int.from_bytes(cdr[12:16], "big")
         if version not in (2, 3):
-            raise ValueError(f'CDF version {version} not handled')
+            raise ValueError(f"CDF version {version} not handled")
 
-        release = int.from_bytes(cdr[16:20], 'big')
-        encoding = int.from_bytes(cdr[20:24], 'big')
+        release = int.from_bytes(cdr[16:20], "big")
+        encoding = int.from_bytes(cdr[20:24], "big")
 
         # FLAG
         #
         # 0 The majority of variable values within a variable record.
         #   Variable records are described in Chapter 4. Set indicates
         #   row-majority. Clear indicates column-majority.
         # 1 The file format of the CDF. Set indicates single-file.
         #   Clear indicates multi-file.
         # 2 The checksum of the CDF. Set indicates a checksum method is used.
         # 3 The MD5 checksum method indicator.
         #   Set indicates MD5 method is used for the checksum. Bit 2 must be set.
         # 4 Reserved for another checksum method.
         #   Bit 2 must be set and bit 3 must be clear.
 
-        flag = int.from_bytes(cdr[24:28], 'big')
-        flag_bits = f'{flag:032b}'
-        row_majority = (flag_bits[31] == '1')
-        single_format = (flag_bits[30] == '1')
-        md5 = (flag_bits[29] == '1' and flag_bits[28] == '1')
-        increment = int.from_bytes(cdr[36:40], 'big')
+        flag = int.from_bytes(cdr[24:28], "big")
+        flag_bits = f"{flag:032b}"
+        row_majority = flag_bits[31] == "1"
+        single_format = flag_bits[30] == "1"
+        md5 = flag_bits[29] == "1" and flag_bits[28] == "1"
+        increment = int.from_bytes(cdr[36:40], "big")
         cdfcopyright = cdr[48:].decode(self.string_encoding)
-        cdfcopyright = cdfcopyright.replace('\x00', '')
+        cdfcopyright = cdfcopyright.replace("\x00", "")
 
-        cdr_info: Dict[str, Union[str, int]] = {}
-        cdr_info['encoding'] = encoding
-        cdr_info['copyright'] = cdfcopyright
-        cdr_info['version'] = (str(version) + '.' + str(release) + '.' +
-                               str(increment))
-        if row_majority:
-            cdr_info['majority'] = 1
-        else:
-            cdr_info['majority'] = 2
-        cdr_info['format'] = single_format
-        cdr_info['md5'] = md5
-        cdr_info['post25'] = True
+        cdr_info = CDRInfo(
+            encoding=encoding,
+            copyright_=cdfcopyright,
+            version=str(version) + "." + str(release) + "." + str(increment),
+            majority=1 if row_majority else 2,
+            format_=single_format,
+            md5=md5,
+            post25=True,
+        )
 
         return cdr_info, foffs
 
-    def _read_cdr2(self, byte_loc):
+    def _read_cdr2(self, byte_loc: int) -> Tuple[CDRInfo, int]:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big')
+        block_size = int.from_bytes(self._f.read(4), "big")
         cdr = self._f.read(block_size - 4)
         foffs = self._f.tell()
 
         # gdroff = int.from_bytes(cdr[4:8], 'big')  # GDR Location
-        version = int.from_bytes(cdr[8:12], 'big')
-        release = int.from_bytes(cdr[12:16], 'big')
-        encoding = int.from_bytes(cdr[16:20], 'big')
-        flag = int.from_bytes(cdr[20:24], 'big')
-        flag_bits = f'{flag:032b}'
-        row_majority = (flag_bits[31] == '1')
-        single_format = (flag_bits[30] == '1')
-        md5 = (flag_bits[29] == '1' and flag_bits[28] == '1')
-        increment = int.from_bytes(cdr[32:36], 'big')
+        version = int.from_bytes(cdr[8:12], "big")
+        release = int.from_bytes(cdr[12:16], "big")
+        encoding = int.from_bytes(cdr[16:20], "big")
+        flag = int.from_bytes(cdr[20:24], "big")
+        flag_bits = f"{flag:032b}"
+        row_majority = flag_bits[31] == "1"
+        single_format = flag_bits[30] == "1"
+        md5 = flag_bits[29] == "1" and flag_bits[28] == "1"
+        increment = int.from_bytes(cdr[32:36], "big")
         cdfcopyright = cdr[44:].decode(self.string_encoding)
-        cdfcopyright = cdfcopyright.replace('\x00', '')
+        cdfcopyright = cdfcopyright.replace("\x00", "")
 
-        cdr_info = {}
-        cdr_info['encoding'] = encoding
-        cdr_info['copyright'] = cdfcopyright
-        cdr_info['version'] = str(version) + '.' + str(release) + '.' + \
-            str(increment)
-        if row_majority:
-            cdr_info['majority'] = 1
-        else:
-            cdr_info['majority'] = 2
-        cdr_info['format'] = single_format
-        cdr_info['md5'] = md5
-        if (version == 2 and release >= 5):
-            cdr_info['post25'] = True
-        else:
-            cdr_info['post25'] = False
+        cdr_info = CDRInfo(
+            encoding=encoding,
+            copyright_=cdfcopyright,
+            version=str(version) + "." + str(release) + "." + str(increment),
+            majority=1 if row_majority else 2,
+            format_=single_format,
+            md5=md5,
+            post25=version == 2 and release >= 5,
+        )
 
         return cdr_info, foffs
 
-    def _read_gdr(self, byte_loc):
+    def _read_gdr(self, byte_loc: int) -> GDRInfo:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(8), 'big')  # Block Size
+        block_size = int.from_bytes(self._f.read(8), "big")  # Block Size
         gdr = self._f.read(block_size - 8)
 
-        first_rvariable = int.from_bytes(gdr[4:12], 'big', signed=True)
-        first_zvariable = int.from_bytes(gdr[12:20], 'big', signed=True)
-        first_adr = int.from_bytes(gdr[20:28], 'big', signed=True)
-        eof = int.from_bytes(gdr[28:36], 'big', signed=True)
-        num_rvariable = int.from_bytes(gdr[36:40], 'big', signed=True)
-        num_att = int.from_bytes(gdr[40:44], 'big', signed=True)
-        num_rdim = int.from_bytes(gdr[48:52], 'big', signed=True)
-        num_zvariable = int.from_bytes(gdr[52:56], 'big', signed=True)
-        leapSecondlastUpdated = int.from_bytes(gdr[68:72], 'big', signed=True)
+        first_rvariable = int.from_bytes(gdr[4:12], "big", signed=True)
+        first_zvariable = int.from_bytes(gdr[12:20], "big", signed=True)
+        first_adr = int.from_bytes(gdr[20:28], "big", signed=True)
+        eof = int.from_bytes(gdr[28:36], "big", signed=True)
+        num_rvariable = int.from_bytes(gdr[36:40], "big", signed=True)
+        num_att = int.from_bytes(gdr[40:44], "big", signed=True)
+        num_rdim = int.from_bytes(gdr[48:52], "big", signed=True)
+        num_zvariable = int.from_bytes(gdr[52:56], "big", signed=True)
+        leapSecondlastUpdated = int.from_bytes(gdr[68:72], "big", signed=True)
         # rDimSizes, depends on Number of dimensions for r variables
         # A bunch of 4 byte integers in a row.  Length is (size of GDR) - 84
         # In this case. there is nothing
         rdim_sizes = []
         for x in range(0, num_rdim):
             ioff = 76 + x * 4
-            rdim_sizes.append(int.from_bytes(gdr[ioff:ioff + 4], 'big',
-                                             signed=True))
+            rdim_sizes.append(int.from_bytes(gdr[ioff : ioff + 4], "big", signed=True))
 
-        gdr_info = {}
-        gdr_info['first_zvariable'] = first_zvariable
-        gdr_info['first_rvariable'] = first_rvariable
-        gdr_info['first_adr'] = first_adr
-        gdr_info['num_zvariables'] = num_zvariable
-        gdr_info['num_rvariables'] = num_rvariable
-        gdr_info['num_attributes'] = num_att
-        gdr_info['rvariables_num_dims'] = num_rdim
-        gdr_info['rvariables_dim_sizes'] = rdim_sizes
-        gdr_info['eof'] = eof
-        gdr_info['leapsecond_updated'] = leapSecondlastUpdated
+        return GDRInfo(
+            first_zvariable=first_zvariable,
+            first_rvariable=first_rvariable,
+            first_adr=first_adr,
+            num_zvariables=num_zvariable,
+            num_rvariables=num_rvariable,
+            num_attributes=num_att,
+            rvariables_num_dims=num_rdim,
+            rvariables_dim_sizes=rdim_sizes,
+            eof=eof,
+            leapsecond_updated=leapSecondlastUpdated,
+        )
 
-        return gdr_info
-
-    def _read_gdr2(self, byte_loc):
+    def _read_gdr2(self, byte_loc: int) -> GDRInfo:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big')  # Block Size
+        block_size = int.from_bytes(self._f.read(4), "big")  # Block Size
         gdr = self._f.read(block_size - 4)
 
-        first_rvariable = int.from_bytes(gdr[4:8], 'big', signed=True)
-        first_zvariable = int.from_bytes(gdr[8:12], 'big', signed=True)
-        first_adr = int.from_bytes(gdr[12:16], 'big', signed=True)
-        eof = int.from_bytes(gdr[16:20], 'big', signed=True)
-        num_rvariable = int.from_bytes(gdr[20:24], 'big', signed=True)
-        num_att = int.from_bytes(gdr[24:28], 'big', signed=True)
-        num_rdim = int.from_bytes(gdr[32:36], 'big', signed=True)
-        num_zvariable = int.from_bytes(gdr[36:40], 'big', signed=True)
+        first_rvariable = int.from_bytes(gdr[4:8], "big", signed=True)
+        first_zvariable = int.from_bytes(gdr[8:12], "big", signed=True)
+        first_adr = int.from_bytes(gdr[12:16], "big", signed=True)
+        eof = int.from_bytes(gdr[16:20], "big", signed=True)
+        num_rvariable = int.from_bytes(gdr[20:24], "big", signed=True)
+        num_att = int.from_bytes(gdr[24:28], "big", signed=True)
+        num_rdim = int.from_bytes(gdr[32:36], "big", signed=True)
+        num_zvariable = int.from_bytes(gdr[36:40], "big", signed=True)
         rdim_sizes = []
         for x in range(0, num_rdim):
             ioff = 56 + x * 4
-            rdim_sizes.append(int.from_bytes(gdr[ioff:ioff + 4], 'big',
-                                             signed=True))
-
-        gdr_info = {}
-        gdr_info['first_zvariable'] = first_zvariable
-        gdr_info['first_rvariable'] = first_rvariable
-        gdr_info['first_adr'] = first_adr
-        gdr_info['num_zvariables'] = num_zvariable
-        gdr_info['num_rvariables'] = num_rvariable
-        gdr_info['num_attributes'] = num_att
-        gdr_info['rvariables_num_dims'] = num_rdim
-        gdr_info['rvariables_dim_sizes'] = rdim_sizes
-        gdr_info['eof'] = eof
+            rdim_sizes.append(int.from_bytes(gdr[ioff : ioff + 4], "big", signed=True))
 
-        return gdr_info
+        return GDRInfo(
+            first_zvariable=first_zvariable,
+            first_rvariable=first_rvariable,
+            first_adr=first_adr,
+            num_zvariables=num_zvariable,
+            num_rvariables=num_rvariable,
+            num_attributes=num_att,
+            rvariables_num_dims=num_rdim,
+            rvariables_dim_sizes=rdim_sizes,
+            eof=eof,
+        )
 
-    def _read_varatts(self, var_num, zVar, expand, to_np=True):
+    def _read_varatts(self, var_num: int, zVar: bool) -> Dict[str, Union[None, str, np.ndarray]]:
         byte_loc = self._first_adr
-        return_dict = {}
+        return_dict: Dict[str, Union[None, str, np.ndarray]] = {}
         for z in range(0, self._num_att):
             adr_info = self._read_adr(byte_loc)
-            if (adr_info['scope'] == 1):
-                byte_loc = adr_info['next_adr_location']
+            if adr_info.scope == 1:
+                byte_loc = adr_info.next_adr_loc
                 continue
-            if (zVar):
-                byte_loc = adr_info['first_z_entry']
-                num_entry = adr_info['num_z_entry']
+            if zVar:
+                byte_loc = adr_info.first_z_entry
+                num_entry = adr_info.num_z_entry
             else:
-                byte_loc = adr_info['first_gr_entry']
-                num_entry = adr_info['num_gr_entry']
-            found = 0
+                byte_loc = adr_info.first_gr_entry
+                num_entry = adr_info.num_gr_entry
             for _ in range(0, num_entry):
                 entryNum, byte_next = self._read_aedr_fast(byte_loc)
-                if (entryNum != var_num):
+                if entryNum != var_num:
                     byte_loc = byte_next
                     continue
-                aedr_info = self._read_aedr(byte_loc, to_np=to_np)
-                entryData = aedr_info['entry']
-                if (expand is False):
-                    # This exists to get rid of extraneous numpy arrays
-                    if isinstance(entryData, np.ndarray):
-                        if len(entryData) == 1:
-                            entryData = entryData[0]
-                    return_dict[adr_info['name']] = entryData
-                else:
-                    entryWithType = []
-                    if (isinstance(entryData, str)):
-                        entryWithType.append(entryData)
-                    else:
-                        dataType = aedr_info['data_type']
-                        if (dataType != 31 and dataType != 32 and dataType != 33):
-                            if (len(entryData.tolist()) == 1):
-                                entryWithType.append(entryData.tolist()[0])
-                            else:
-                                entryWithType.append(entryData.tolist())
-                        else:
-                            if (len(entryData.tolist()) == 1):
-                                if (dataType != 33):
-                                    entryWithType.append(epoch.CDFepoch.encode(entryData.tolist()[0],
-                                                                               iso_8601=False))
-                                else:
-                                    entryWithType.append(epoch.CDFepoch.encode(entryData.tolist()[0]))
-                            else:
-                                if (dataType != 33):
-                                    entryWithType.append(epoch.CDFepoch.encode(entryData.tolist(),
-                                                                               iso_8601=False))
-                                else:
-                                    entryWithType.append(epoch.CDFepoch.encode(entryData.tolist()))
-                    entryWithType.append(self._datatype_token(aedr_info['data_type']))
-                    return_dict[adr_info['name']] = entryWithType
-                found = 1
+                aedr_info = self._read_aedr(byte_loc)
+                entryData = aedr_info.entry
+                # This exists to get rid of extraneous numpy arrays
+                if isinstance(entryData, np.ndarray):
+                    if len(entryData) == 1:
+                        entryData = entryData[0]
+                return_dict[adr_info.name] = entryData
                 break
-            byte_loc = adr_info['next_adr_location']
-            if (found == 0 and expand is not False):
-                return_dict[adr_info['name']] = None
+            byte_loc = adr_info.next_adr_loc
         return return_dict
 
-    def _read_adr(self, position):
+    def _read_adr(self, position: int) -> ADRInfo:
         """
         Read an attribute descriptor record (ADR).
         """
-        if (self.cdfversion == 3):
+        if self.cdfversion == 3:
             return self._read_adr3(position)
         else:
             return self._read_adr2(position)
 
-    def _read_adr3(self, byte_loc):
+    def _read_adr3(self, byte_loc: int) -> ADRInfo:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(8), 'big')  # Block Size
+        block_size = int.from_bytes(self._f.read(8), "big")  # Block Size
         adr = self._f.read(block_size - 8)
 
-        next_adr_loc = int.from_bytes(adr[4:12], 'big', signed=True)
-        position_next_gr_entry = int.from_bytes(adr[12:20], 'big', signed=True)
-        scope = int.from_bytes(adr[20:24], 'big', signed=True)
-        num = int.from_bytes(adr[24:28], 'big', signed=True)
-        num_gr_entry = int.from_bytes(adr[28:32], 'big', signed=True)
-        MaxEntry = int.from_bytes(adr[32:36], 'big', signed=True)
-        position_next_z_entry = int.from_bytes(adr[40:48], 'big', signed=True)
-        num_z_entry = int.from_bytes(adr[48:52], 'big', signed=True)
-        MaxZEntry = int.from_bytes(adr[52:56], 'big', signed=True)
+        next_adr_loc = int.from_bytes(adr[4:12], "big", signed=True)
+        position_next_gr_entry = int.from_bytes(adr[12:20], "big", signed=True)
+        scope = int.from_bytes(adr[20:24], "big", signed=True)
+        num = int.from_bytes(adr[24:28], "big", signed=True)
+        num_gr_entry = int.from_bytes(adr[28:32], "big", signed=True)
+        MaxEntry = int.from_bytes(adr[32:36], "big", signed=True)
+        position_next_z_entry = int.from_bytes(adr[40:48], "big", signed=True)
+        num_z_entry = int.from_bytes(adr[48:52], "big", signed=True)
+        MaxZEntry = int.from_bytes(adr[52:56], "big", signed=True)
 
         name = str(adr[60:315].decode(self.string_encoding))
-        name = name.replace('\x00', '')
+        name = name.replace("\x00", "")
 
-        # Build the return dictionary
-        return_dict = {}
-        return_dict['scope'] = scope
-        return_dict['next_adr_location'] = next_adr_loc
-        return_dict['attribute_number'] = num
-        return_dict['num_gr_entry'] = num_gr_entry
-        return_dict['max_gr_entry'] = MaxEntry
-        return_dict['num_z_entry'] = num_z_entry
-        return_dict['max_z_entry'] = MaxZEntry
-        return_dict['first_z_entry'] = position_next_z_entry
-        return_dict['first_gr_entry'] = position_next_gr_entry
-        return_dict['name'] = name
+        return ADRInfo(
+            scope,
+            next_adr_loc,
+            num,
+            num_gr_entry,
+            MaxEntry,
+            num_z_entry,
+            MaxZEntry,
+            position_next_z_entry,
+            position_next_gr_entry,
+            name,
+        )
 
-        return return_dict
-
-    def _read_adr2(self, byte_loc):
+    def _read_adr2(self, byte_loc: int) -> ADRInfo:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big')  # Block Size
+        block_size = int.from_bytes(self._f.read(4), "big")  # Block Size
         adr = self._f.read(block_size - 4)
 
-        next_adr_loc = int.from_bytes(adr[4:8], 'big', signed=True)
-        position_next_gr_entry = int.from_bytes(adr[8:12], 'big', signed=True)
-        scope = int.from_bytes(adr[12:16], 'big', signed=True)
-        num = int.from_bytes(adr[16:20], 'big', signed=True)
-        num_gr_entry = int.from_bytes(adr[20:24], 'big', signed=True)
-        MaxEntry = int.from_bytes(adr[24:28], 'big', signed=True)
-        position_next_z_entry = int.from_bytes(adr[32:36], 'big', signed=True)
-        num_z_entry = int.from_bytes(adr[36:40], 'big', signed=True)
-        MaxZEntry = int.from_bytes(adr[40:44], 'big', signed=True)
+        next_adr_loc = int.from_bytes(adr[4:8], "big", signed=True)
+        position_next_gr_entry = int.from_bytes(adr[8:12], "big", signed=True)
+        scope = int.from_bytes(adr[12:16], "big", signed=True)
+        num = int.from_bytes(adr[16:20], "big", signed=True)
+        num_gr_entry = int.from_bytes(adr[20:24], "big", signed=True)
+        MaxEntry = int.from_bytes(adr[24:28], "big", signed=True)
+        position_next_z_entry = int.from_bytes(adr[32:36], "big", signed=True)
+        num_z_entry = int.from_bytes(adr[36:40], "big", signed=True)
+        MaxZEntry = int.from_bytes(adr[40:44], "big", signed=True)
 
         name = str(adr[48:112].decode(self.string_encoding))
-        name = name.replace('\x00', '')
+        name = name.replace("\x00", "")
 
-        # Build the return dictionary
-        return_dict = {}
-        return_dict['scope'] = scope
-        return_dict['next_adr_location'] = next_adr_loc
-        return_dict['attribute_number'] = num
-        return_dict['num_gr_entry'] = num_gr_entry
-        return_dict['max_gr_entry'] = MaxEntry
-        return_dict['num_z_entry'] = num_z_entry
-        return_dict['max_z_entry'] = MaxZEntry
-        return_dict['first_z_entry'] = position_next_z_entry
-        return_dict['first_gr_entry'] = position_next_gr_entry
-        return_dict['name'] = name
-
-        return return_dict
+        return ADRInfo(
+            scope,
+            next_adr_loc,
+            num,
+            num_gr_entry,
+            MaxEntry,
+            num_z_entry,
+            MaxZEntry,
+            position_next_z_entry,
+            position_next_gr_entry,
+            name,
+        )
 
-    def _read_adr_fast(self, position):
+    def _read_adr_fast(self, position: int) -> Tuple[str, int]:
         """
         Read an attribute descriptor record (ADR).
         """
-        if (self.cdfversion == 3):
+        if self.cdfversion == 3:
             return self._read_adr_fast3(position)
         else:
             return self._read_adr_fast2(position)
 
-    def _read_adr_fast3(self, byte_loc):
+    def _read_adr_fast3(self, byte_loc: int) -> Tuple[str, int]:
         # Position of next ADR
         self._f.seek(byte_loc + 12, 0)
-        next_adr_loc = int.from_bytes(self._f.read(8), 'big', signed=True)
+        next_adr_loc = int.from_bytes(self._f.read(8), "big", signed=True)
         # Name
         self._f.seek(byte_loc + 68, 0)
         name = str(self._f.read(256).decode(self.string_encoding))
 
-        name = name.replace('\x00', '')
+        name = name.replace("\x00", "")
 
         return name, next_adr_loc
 
-    def _read_adr_fast2(self, byte_loc):
+    def _read_adr_fast2(self, byte_loc: int) -> Tuple[str, int]:
         # Position of next ADR
         self._f.seek(byte_loc + 8, 0)
-        next_adr_loc = int.from_bytes(self._f.read(4), 'big', signed=True)
+        next_adr_loc = int.from_bytes(self._f.read(4), "big", signed=True)
         # Name
         self._f.seek(byte_loc + 52, 0)
         name = str(self._f.read(64).decode(self.string_encoding))
 
-        name = name.replace('\x00', '')
+        name = name.replace("\x00", "")
 
         return name, next_adr_loc
 
-    def _read_aedr_fast(self, byte_loc):
+    def _read_aedr_fast(self, byte_loc: int) -> Tuple[int, int]:
         if self.cdfversion == 3:
             return self._read_aedr_fast3(byte_loc)
         else:
             return self._read_aedr_fast2(byte_loc)
 
-    def _read_aedr_fast3(self, byte_loc):
+    def _read_aedr_fast3(self, byte_loc: int) -> Tuple[int, int]:
         self._f.seek(byte_loc + 12, 0)
-        next_aedr = int.from_bytes(self._f.read(8), 'big', signed=True)
+        next_aedr = int.from_bytes(self._f.read(8), "big", signed=True)
 
         # Variable number or global entry number
         self._f.seek(byte_loc + 28, 0)
-        entry_num = int.from_bytes(self._f.read(4), 'big', signed=True)
+        entry_num = int.from_bytes(self._f.read(4), "big", signed=True)
 
         return entry_num, next_aedr
 
-    def _read_aedr_fast2(self, byte_loc):
+    def _read_aedr_fast2(self, byte_loc: int) -> Tuple[int, int]:
         self._f.seek(byte_loc + 8, 0)
-        next_aedr = int.from_bytes(self._f.read(4), 'big', signed=True)
+        next_aedr = int.from_bytes(self._f.read(4), "big", signed=True)
 
         # Variable number or global entry number
         self._f.seek(byte_loc + 20, 0)
-        entry_num = int.from_bytes(self._f.read(4), 'big', signed=True)
+        entry_num = int.from_bytes(self._f.read(4), "big", signed=True)
 
         return entry_num, next_aedr
 
-    def _read_aedr(self, byte_loc, to_np=True):
+    def _read_aedr(self, byte_loc: int) -> AEDR:
         if self.cdfversion == 3:
-            return self._read_aedr3(byte_loc, to_np)
+            return self._read_aedr3(byte_loc)
         else:
-            return self._read_aedr2(byte_loc, to_np)
+            return self._read_aedr2(byte_loc)
 
-    def _read_aedr3(self, byte_loc, to_np=True):
+    def _read_aedr3(self, byte_loc: int) -> AEDR:
         """
         Reads an Attribute Entry Descriptor Record at a specific byte location.
 
         """
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(8), 'big')
+        block_size = int.from_bytes(self._f.read(8), "big")
         aedr = self._f.read(block_size - 8)
 
-        next_aedr = int.from_bytes(aedr[4:12], 'big', signed=True)
-        data_type = int.from_bytes(aedr[16:20], 'big', signed=True)
+        next_aedr = int.from_bytes(aedr[4:12], "big", signed=True)
+        data_type = int.from_bytes(aedr[16:20], "big", signed=True)
 
         # Variable number or global entry number
-        entry_num = int.from_bytes(aedr[20:24], 'big', signed=True)
+        entry_num = int.from_bytes(aedr[20:24], "big", signed=True)
 
         # Number of elements
         # Length of string if string, otherwise its the number of numbers
-        num_elements = int.from_bytes(aedr[24:28], 'big', signed=True)
+        num_elements = int.from_bytes(aedr[24:28], "big", signed=True)
 
         # Supposed to be reserved space
-        num_strings = int.from_bytes(aedr[28:32], 'big', signed=True)
-        if (num_strings < 1):
+        num_strings = int.from_bytes(aedr[28:32], "big", signed=True)
+        if num_strings < 1:
             num_strings = 1
 
         # Literally nothing
         # _ = int.from_bytes(aedr[32:36],'big', signed=True) #Nothing
         # _ = int.from_bytes(aedr[36:40],'big', signed=True) #Nothing
         # _ = int.from_bytes(aedr[40:44],'big', signed=True) #Nothing
         # _ = int.from_bytes(aedr[44:48],'big', signed=True) #Nothing
 
         byte_stream = aedr[48:]
-        if to_np:
-            entry = self._read_data(byte_stream, data_type, 1, num_elements)
-        else:
-            if (data_type == 32):
-                entry = self._convert_data(byte_stream, data_type, 1, 2, num_elements)
-            else:
-                entry = self._convert_data(byte_stream, data_type, 1, 1, num_elements)
-
-        return_dict = {}
-        return_dict['entry'] = entry
-        return_dict['data_type'] = data_type
-        return_dict['num_elements'] = num_elements
-        return_dict['num_strings'] = num_strings
-        return_dict['next_aedr'] = next_aedr
-        return_dict['entry_num'] = entry_num
+        entry = self._read_data(byte_stream, data_type, 1, num_elements)
 
-        return return_dict
+        return AEDR(entry, data_type, num_elements, next_aedr, entry_num, num_strings)
 
-    def _read_aedr2(self, byte_loc, to_np=True):
+    def _read_aedr2(self, byte_loc: int) -> AEDR:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big')
+        block_size = int.from_bytes(self._f.read(4), "big")
         aedr = self._f.read(block_size - 4)
 
-        next_aedr = int.from_bytes(aedr[4:8], 'big', signed=True)
-        data_type = int.from_bytes(aedr[12:16], 'big', signed=True)
+        next_aedr = int.from_bytes(aedr[4:8], "big", signed=True)
+        data_type = int.from_bytes(aedr[12:16], "big", signed=True)
 
         # Variable number or global entry number
-        entry_num = int.from_bytes(aedr[16:20], 'big', signed=True)
+        entry_num = int.from_bytes(aedr[16:20], "big", signed=True)
         # Number of elements
         # Length of string if string, otherwise its the number of numbers
-        num_elements = int.from_bytes(aedr[20:24], 'big', signed=True)
+        num_elements = int.from_bytes(aedr[20:24], "big", signed=True)
         byte_stream = aedr[44:]
-        if to_np:
-            entry = self._read_data(byte_stream, data_type, 1, num_elements)
-        else:
-            if (data_type == 32):
-                entry = self._convert_data(byte_stream, data_type, 1, 2, num_elements)
-            else:
-                entry = self._convert_data(byte_stream, data_type, 1, 1, num_elements)
-        return_dict = {}
-        return_dict['entry'] = entry
-        return_dict['data_type'] = data_type
-        return_dict['num_elements'] = num_elements
-        # return_dict['num_strings'] = num_strings
-        return_dict['next_aedr'] = next_aedr
-        return_dict['entry_num'] = entry_num
-        return return_dict
+        entry = self._read_data(byte_stream, data_type, 1, num_elements)
 
-    def _read_vdr(self, byte_loc):
+        return AEDR(entry, data_type, num_elements, next_aedr, entry_num)
+
+    def _read_vdr(self, byte_loc: int) -> VDR:
         """
         Read a variable descriptor record (VDR).
         """
         if self.cdfversion == 3:
             return self._read_vdr3(byte_loc)
         else:
             return self._read_vdr2(byte_loc)
 
-    def _read_vdr3(self, byte_loc):
+    def _read_vdr3(self, byte_loc: int) -> VDR:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(8), 'big')
+        block_size = int.from_bytes(self._f.read(8), "big")
         vdr = self._f.read(block_size - 8)
 
         # Type of internal record
-        section_type = int.from_bytes(vdr[0:4], 'big')
-        next_vdr = int.from_bytes(vdr[4:12], 'big', signed=True)
-        data_type = int.from_bytes(vdr[12:16], 'big', signed=True)
-        max_rec = int.from_bytes(vdr[16:20], 'big', signed=True)
-        head_vxr = int.from_bytes(vdr[20:28], 'big', signed=True)
-        last_vxr = int.from_bytes(vdr[28:36], 'big', signed=True)
-        flags = int.from_bytes(vdr[36:40], 'big', signed=True)
-
-        flag_bits = f'{flags:032b}'
-
-        record_variance_bool = (flag_bits[31] == '1')
-        pad_bool = (flag_bits[30] == '1')
-        compression_bool = (flag_bits[29] == '1')
-
-        sparse = int.from_bytes(vdr[40:44], 'big', signed=True)
-        num_elements = int.from_bytes(vdr[56:60], 'big', signed=True)
-        var_num = int.from_bytes(vdr[60:64], 'big', signed=True)
-        CPRorSPRoffset = int.from_bytes(vdr[64:72], 'big', signed=True)
-        blocking_factor = int.from_bytes(vdr[72:76], 'big', signed=True)
+        section_type = int.from_bytes(vdr[0:4], "big")
+        next_vdr = int.from_bytes(vdr[4:12], "big", signed=True)
+        data_type = int.from_bytes(vdr[12:16], "big", signed=True)
+        max_rec = int.from_bytes(vdr[16:20], "big", signed=True)
+        head_vxr = int.from_bytes(vdr[20:28], "big", signed=True)
+        last_vxr = int.from_bytes(vdr[28:36], "big", signed=True)
+        flags = int.from_bytes(vdr[36:40], "big", signed=True)
+
+        flag_bits = f"{flags:032b}"
+
+        record_variance_bool = flag_bits[31] == "1"
+        pad_bool = flag_bits[30] == "1"
+        compression_bool = flag_bits[29] == "1"
+
+        sparse = int.from_bytes(vdr[40:44], "big", signed=True)
+        num_elements = int.from_bytes(vdr[56:60], "big", signed=True)
+        var_num = int.from_bytes(vdr[60:64], "big", signed=True)
+        CPRorSPRoffset = int.from_bytes(vdr[64:72], "big", signed=True)
+        blocking_factor = int.from_bytes(vdr[72:76], "big", signed=True)
         name = str(vdr[76:332].decode(self.string_encoding))
-        name = name.replace('\x00', '')
+        name = name.replace("\x00", "")
 
         zdim_sizes = []
         dim_sizes = []
         dim_varys = []
-        if (section_type == 8):
+        if section_type == 8:
             # zvariable
-            num_dims = int.from_bytes(vdr[332:336], 'big', signed=True)
+            num_dims = int.from_bytes(vdr[332:336], "big", signed=True)
             for x in range(0, num_dims):
                 ioff = 336 + 4 * x
-                zdim_sizes.append(int.from_bytes(vdr[ioff:ioff + 4], 'big',
-                                                 signed=True))
+                zdim_sizes.append(int.from_bytes(vdr[ioff : ioff + 4], "big", signed=True))
             coff = 336 + 4 * num_dims
             for x in range(0, num_dims):
-                dim_varys.append(int.from_bytes(vdr[coff + 4 * x:coff + 4 * x + 4],
-                                                'big', signed=True))
+                dim_varys.append(int.from_bytes(vdr[coff + 4 * x : coff + 4 * x + 4], "big", signed=True))
             adj = 0
             # Check for "False" dimensions, and delete them
             for x in range(0, num_dims):
                 y = num_dims - x - 1
-                if (dim_varys[y] == 0):
+                if dim_varys[y] == 0:
                     del zdim_sizes[y]
                     del dim_varys[y]
                     adj = adj + 1
             num_dims = num_dims - adj
             coff = 336 + 8 * num_dims
         else:
             # rvariable
             for x in range(0, self._rvariables_num_dims):
                 ioff = 332 + 4 * x
-                dim_varys.append(int.from_bytes(vdr[ioff:ioff + 4], 'big',
-                                                signed=True))
+                dim_varys.append(int.from_bytes(vdr[ioff : ioff + 4], "big", signed=True))
             for x in range(0, self._rvariables_num_dims):
-                if (dim_varys[x] != 0):
+                if dim_varys[x] != 0:
                     dim_sizes.append(self._rvariables_dim_sizes[x])
             num_dims = len(dim_sizes)
             coff = 332 + 4 * self._rvariables_num_dims
         # Only set if pad value is in the flags
         if pad_bool:
             byte_stream = vdr[coff:]
             pad = self._read_data(byte_stream, data_type, 1, num_elements)
+        else:
+            pad = None
 
-        return_dict = {}
-        return_dict['data_type'] = data_type
-        return_dict['section_type'] = section_type
-        return_dict['next_vdr_location'] = next_vdr
-        return_dict['variable_number'] = var_num
-        return_dict['head_vxr'] = head_vxr
-        return_dict['last_vxr'] = last_vxr
-        return_dict['max_records'] = max_rec
-        return_dict['name'] = name
-        return_dict['num_dims'] = num_dims
-        if (section_type == 8):
-            return_dict['dim_sizes'] = zdim_sizes
-        else:
-            return_dict['dim_sizes'] = dim_sizes
-        if (pad_bool):
-            return_dict['pad'] = pad
-        return_dict['compression_bool'] = compression_bool
-        if (compression_bool):
+        if section_type == 8:
+            dim_sizes = zdim_sizes
+        if compression_bool:
             ctype, cparm = self._read_cpr(CPRorSPRoffset)
-            return_dict['compression_level'] = cparm
+            compression_level = cparm
         else:
-            return_dict['compression_level'] = 0
-        return_dict['blocking_factor'] = blocking_factor
-        return_dict['dim_vary'] = dim_varys
-        return_dict['record_vary'] = record_variance_bool
-        return_dict['num_elements'] = num_elements
-        return_dict['sparse'] = sparse
-        return return_dict
-
-    def _read_vdr2(self, byte_loc):
+            compression_level = 0
+        return VDR(
+            data_type=data_type,
+            section_type=section_type,
+            next_vdr_location=next_vdr,
+            variable_number=var_num,
+            head_vxr=head_vxr,
+            last_vxr=last_vxr,
+            max_rec=max_rec,
+            name=name,
+            num_dims=num_dims,
+            dim_sizes=dim_sizes,
+            compression_bool=compression_bool,
+            compression_level=compression_level,
+            blocking_factor=blocking_factor,
+            dim_vary=dim_varys,
+            record_vary=record_variance_bool,
+            num_elements=num_elements,
+            sparse=sparse,
+            pad=pad,
+        )
 
-        if (self._post25 is True):
+    def _read_vdr2(self, byte_loc: int) -> VDR:
+        if self._post25 is True:
             toadd = 0
         else:
             toadd = 128
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big')
+        block_size = int.from_bytes(self._f.read(4), "big")
         vdr = self._f.read(block_size - 4)
 
         # Type of internal record
-        section_type = int.from_bytes(vdr[0:4], 'big')
-        next_vdr = int.from_bytes(vdr[4:8], 'big', signed=True)
-        data_type = int.from_bytes(vdr[8:12], 'big', signed=True)
-        max_rec = int.from_bytes(vdr[12:16], 'big', signed=True)
-        head_vxr = int.from_bytes(vdr[16:20], 'big', signed=True)
-        last_vxr = int.from_bytes(vdr[20:24], 'big', signed=True)
-        flags = int.from_bytes(vdr[24:28], 'big', signed=True)
-        flag_bits = f'{flags:032b}'
-        record_variance_bool = (flag_bits[31] == '1')
-        pad_bool = (flag_bits[30] == '1')
-        compression_bool = (flag_bits[29] == '1')
-        sparse = int.from_bytes(vdr[28:32], 'big', signed=True)
-
-        num_elements = int.from_bytes(vdr[44 + toadd:48 + toadd], 'big', signed=True)
-        var_num = int.from_bytes(vdr[48 + toadd:52 + toadd], 'big', signed=True)
-        CPRorSPRoffset = int.from_bytes(vdr[52 + toadd:56 + toadd], 'big',
-                                        signed=True)
-        blocking_factor = int.from_bytes(vdr[56 + toadd:60 + toadd], 'big',
-                                         signed=True)
-        name = str(vdr[60 + toadd:124 + toadd].decode(self.string_encoding))
-        name = name.replace('\x00', '')
+        section_type = int.from_bytes(vdr[0:4], "big")
+        next_vdr = int.from_bytes(vdr[4:8], "big", signed=True)
+        data_type = int.from_bytes(vdr[8:12], "big", signed=True)
+        max_rec = int.from_bytes(vdr[12:16], "big", signed=True)
+        head_vxr = int.from_bytes(vdr[16:20], "big", signed=True)
+        last_vxr = int.from_bytes(vdr[20:24], "big", signed=True)
+        flags = int.from_bytes(vdr[24:28], "big", signed=True)
+        flag_bits = f"{flags:032b}"
+        record_variance_bool = flag_bits[31] == "1"
+        pad_bool = flag_bits[30] == "1"
+        compression_bool = flag_bits[29] == "1"
+        sparse = int.from_bytes(vdr[28:32], "big", signed=True)
+
+        num_elements = int.from_bytes(vdr[44 + toadd : 48 + toadd], "big", signed=True)
+        var_num = int.from_bytes(vdr[48 + toadd : 52 + toadd], "big", signed=True)
+        CPRorSPRoffset = int.from_bytes(vdr[52 + toadd : 56 + toadd], "big", signed=True)
+        blocking_factor = int.from_bytes(vdr[56 + toadd : 60 + toadd], "big", signed=True)
+        name = str(vdr[60 + toadd : 124 + toadd].decode(self.string_encoding))
+        name = name.replace("\x00", "")
         zdim_sizes = []
         dim_sizes = []
         dim_varys = []
-        if (section_type == 8):
+        if section_type == 8:
             # zvariable
-            num_dims = int.from_bytes(vdr[124 + toadd:128 + toadd], 'big',
-                                      signed=True)
+            num_dims = int.from_bytes(vdr[124 + toadd : 128 + toadd], "big", signed=True)
             for x in range(0, num_dims):
                 xoff = 128 + toadd + 4 * x
-                zdim_sizes.append(int.from_bytes(vdr[xoff:xoff + 4], 'big',
-                                                 signed=True))
+                zdim_sizes.append(int.from_bytes(vdr[xoff : xoff + 4], "big", signed=True))
             coff = 128 + toadd + 4 * num_dims
             for x in range(0, num_dims):
                 icoff = coff + 4 * x
-                if (int.from_bytes(vdr[icoff:icoff + 4], 'big', signed=True) == 0):
+                if int.from_bytes(vdr[icoff : icoff + 4], "big", signed=True) == 0:
                     dim_varys.append(False)
                 else:
                     dim_varys.append(True)
             adj = 0
             # Check for "False" dimensions, and delete them
             for x in range(0, num_dims):
                 y = num_dims - x - 1
-                if (dim_varys[y] == 0 or dim_varys[y] == False):
+                if dim_varys[y] == 0 or dim_varys[y] == False:
                     del zdim_sizes[y]
                     del dim_varys[y]
                     adj = adj + 1
             num_dims = num_dims - adj
             coff = 128 + toadd + 8 * num_dims
         else:
             # rvariable
             for x in range(0, self._rvariables_num_dims):
                 ix = 124 + toadd + 4 * x
-                if (int.from_bytes(vdr[ix:ix + 4], 'big', signed=True) == 0):
+                if int.from_bytes(vdr[ix : ix + 4], "big", signed=True) == 0:
                     dim_varys.append(False)
                 else:
                     dim_varys.append(True)
             for x in range(0, len(dim_varys)):
                 dim_sizes.append(self._rvariables_dim_sizes[x])
             num_dims = len(dim_sizes)
             coff = 124 + toadd + 4 * self._rvariables_num_dims
         # Only set if pad value is in the flags
         if pad_bool:
             byte_stream = vdr[coff:]
+            pad: Union[str, np.ndarray]
             try:
                 pad = self._read_data(byte_stream, data_type, 1, num_elements)
             except Exception:
-                if (data_type == 51 or data_type == 52):
-                    pad = ' ' * num_elements
+                if data_type == 51 or data_type == 52:
+                    pad = " " * num_elements
 
-        return_dict = {}
-        return_dict['data_type'] = data_type
-        return_dict['section_type'] = section_type
-        return_dict['next_vdr_location'] = next_vdr
-        return_dict['variable_number'] = var_num
-        return_dict['head_vxr'] = head_vxr
-        return_dict['last_vxr'] = last_vxr
-        return_dict['max_records'] = max_rec
-        return_dict['name'] = name
-        return_dict['num_dims'] = num_dims
-        if (section_type == 8):
-            return_dict['dim_sizes'] = zdim_sizes
-        else:
-            return_dict['dim_sizes'] = dim_sizes
-        if (pad_bool):
-            return_dict['pad'] = pad
-        return_dict['compression_bool'] = compression_bool
-        if (compression_bool):
+        if section_type == 8:
+            dim_sizes = zdim_sizes
+        if compression_bool:
             ctype, cparm = self._read_cpr(CPRorSPRoffset)
-            return_dict['compression_level'] = cparm
+            compression_level = cparm
         else:
-            return_dict['compression_level'] = 0
-        return_dict['blocking_factor'] = blocking_factor
-        return_dict['dim_vary'] = dim_varys
-        return_dict['record_vary'] = record_variance_bool
-        return_dict['num_elements'] = num_elements
-        return_dict['sparse'] = sparse
-        return return_dict
+            compression_level = 0
+        return VDR(
+            data_type=data_type,
+            section_type=section_type,
+            next_vdr_location=next_vdr,
+            variable_number=var_num,
+            head_vxr=head_vxr,
+            last_vxr=last_vxr,
+            max_rec=max_rec,
+            name=name,
+            num_dims=num_dims,
+            dim_sizes=dim_sizes,
+            compression_bool=compression_bool,
+            compression_level=compression_level,
+            blocking_factor=blocking_factor,
+            dim_vary=dim_varys,
+            record_vary=record_variance_bool,
+            num_elements=num_elements,
+            sparse=sparse,
+            pad=pad,
+        )
 
-    def _read_vdr_fast(self, byte_loc):
+    def _read_vdr_fast(self, byte_loc: int) -> Tuple[str, int]:
         if self.cdfversion == 3:
             return self._read_vdr_fast3(byte_loc)
         else:
             return self._read_vdr_fast2(byte_loc)
 
-    def _read_vdr_fast3(self, byte_loc):
+    def _read_vdr_fast3(self, byte_loc: int) -> Tuple[str, int]:
         self._f.seek(byte_loc + 12, 0)
-        next_vdr = int.from_bytes(self._f.read(8), 'big', signed=True)
+        next_vdr = int.from_bytes(self._f.read(8), "big", signed=True)
         self._f.seek(byte_loc + 84, 0)
         name = str(self._f.read(256).decode(self.string_encoding))
 
-        name = name.replace('\x00', '')
+        name = name.replace("\x00", "")
 
         return name, next_vdr
 
-    def _read_vdr_fast2(self, byte_loc):
+    def _read_vdr_fast2(self, byte_loc: int) -> Tuple[str, int]:
         if self._post25:
             toadd = 0
         else:
             toadd = 128
 
         self._f.seek(byte_loc + 8, 0)
-        next_vdr = int.from_bytes(self._f.read(4), 'big', signed=True)
+        next_vdr = int.from_bytes(self._f.read(4), "big", signed=True)
         self._f.seek(byte_loc + toadd + 64, 0)
         name = str(self._f.read(64).decode(self.string_encoding))
 
-        name = name.replace('\x00', '')
+        name = name.replace("\x00", "")
 
         return name, next_vdr
 
-    def _read_vxrs(self, byte_loc, vvr_offsets=[], vvr_start=[], vvr_end=[]):
+    def _read_vxrs(
+        self, byte_loc: int, vvr_offsets: List[int] = [], vvr_start: List[int] = [], vvr_end: List[int] = []
+    ) -> Tuple[List[int], List[int], List[int]]:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(8), 'big', signed=True)  # Block Size
+        block_size = int.from_bytes(self._f.read(8), "big", signed=True)  # Block Size
         vxrs = self._f.read(block_size - 8)
 
-        next_vxr_pos = int.from_bytes(vxrs[4:12], 'big', signed=True)
-        num_ent = int.from_bytes(vxrs[12:16], 'big', signed=True)
-        num_ent_used = int.from_bytes(vxrs[16:20], 'big', signed=True)
+        next_vxr_pos = int.from_bytes(vxrs[4:12], "big", signed=True)
+        num_ent = int.from_bytes(vxrs[12:16], "big", signed=True)
+        num_ent_used = int.from_bytes(vxrs[16:20], "big", signed=True)
         # coff = 20
         for ix in range(0, num_ent_used):
             soffset = 20 + 4 * ix
-            num_start = int.from_bytes(vxrs[soffset:soffset + 4], 'big',
-                                       signed=True)
+            num_start = int.from_bytes(vxrs[soffset : soffset + 4], "big", signed=True)
             eoffset = 20 + 4 * num_ent + 4 * ix
-            num_end = int.from_bytes(vxrs[eoffset:eoffset + 4], 'big', signed=True)
+            num_end = int.from_bytes(vxrs[eoffset : eoffset + 4], "big", signed=True)
             ooffset = 20 + 2 * 4 * num_ent + 8 * ix
-            rec_offset = int.from_bytes(vxrs[ooffset:ooffset + 8], 'big',
-                                        signed=True)
+            rec_offset = int.from_bytes(vxrs[ooffset : ooffset + 8], "big", signed=True)
             type_offset = 8 + rec_offset
             self._f.seek(type_offset, 0)
-            next_type = int.from_bytes(self._f.read(4), 'big', signed=True)
+            next_type = int.from_bytes(self._f.read(4), "big", signed=True)
             if next_type == 6:
-                vvr_offsets, vvr_start, vvr_end = self._read_vxrs(rec_offset,
-                                                                  vvr_offsets=vvr_offsets, vvr_start=vvr_start, vvr_end=vvr_end)
+                vvr_offsets, vvr_start, vvr_end = self._read_vxrs(
+                    rec_offset, vvr_offsets=vvr_offsets, vvr_start=vvr_start, vvr_end=vvr_end
+                )
             else:
                 vvr_offsets.extend([rec_offset])
                 vvr_start.extend([num_start])
                 vvr_end.extend([num_end])
 
         if next_vxr_pos != 0:
-            vvr_offsets, vvr_start, vvr_end = self._read_vxrs(next_vxr_pos,
-                                                              vvr_offsets=vvr_offsets, vvr_start=vvr_start, vvr_end=vvr_end)
+            vvr_offsets, vvr_start, vvr_end = self._read_vxrs(
+                next_vxr_pos, vvr_offsets=vvr_offsets, vvr_start=vvr_start, vvr_end=vvr_end
+            )
 
         return vvr_offsets, vvr_start, vvr_end
 
-    def _read_vxrs2(self, byte_loc, vvr_offsets=[], vvr_start=[], vvr_end=[]):
-
+    def _read_vxrs2(
+        self, byte_loc: int, vvr_offsets: List[int] = [], vvr_start: List[int] = [], vvr_end: List[int] = []
+    ) -> Tuple[List[int], List[int], List[int]]:
         self._f.seek(byte_loc, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big', signed=True)
+        block_size = int.from_bytes(self._f.read(4), "big", signed=True)
         vxrs = self._f.read(block_size - 4)
 
-        next_vxr_pos = int.from_bytes(vxrs[4:8], 'big', signed=True)
-        num_ent = int.from_bytes(vxrs[8:12], 'big', signed=True)
-        num_ent_used = int.from_bytes(vxrs[12:16], 'big', signed=True)
+        next_vxr_pos = int.from_bytes(vxrs[4:8], "big", signed=True)
+        num_ent = int.from_bytes(vxrs[8:12], "big", signed=True)
+        num_ent_used = int.from_bytes(vxrs[12:16], "big", signed=True)
         # coff = 16
         for ix in range(0, num_ent_used):
             soffset = 16 + 4 * ix
-            num_start = int.from_bytes(vxrs[soffset:soffset + 4], 'big',
-                                       signed=True)
+            num_start = int.from_bytes(vxrs[soffset : soffset + 4], "big", signed=True)
             eoffset = 16 + 4 * num_ent + 4 * ix
-            num_end = int.from_bytes(vxrs[eoffset:eoffset + 4], 'big', signed=True)
+            num_end = int.from_bytes(vxrs[eoffset : eoffset + 4], "big", signed=True)
             ooffset = 16 + 2 * 4 * num_ent + 4 * ix
-            rec_offset = int.from_bytes(vxrs[ooffset:ooffset + 4], 'big',
-                                        signed=True)
+            rec_offset = int.from_bytes(vxrs[ooffset : ooffset + 4], "big", signed=True)
             type_offset = 4 + rec_offset
             self._f.seek(type_offset, 0)
-            next_type = int.from_bytes(self._f.read(4), 'big', signed=True)
+            next_type = int.from_bytes(self._f.read(4), "big", signed=True)
             if next_type == 6:
-                vvr_offsets, vvr_start, vvr_end = self._read_vxrs2(rec_offset,
-                                                                   vvr_offsets=vvr_offsets, vvr_start=vvr_start, vvr_end=vvr_end)
+                vvr_offsets, vvr_start, vvr_end = self._read_vxrs2(
+                    rec_offset, vvr_offsets=vvr_offsets, vvr_start=vvr_start, vvr_end=vvr_end
+                )
             else:
                 vvr_offsets.extend([rec_offset])
                 vvr_start.extend([num_start])
                 vvr_end.extend([num_end])
 
         if next_vxr_pos != 0:
-            vvr_offsets, vvr_start, vvr_end = self._read_vxrs2(next_vxr_pos,
-                                                               vvr_offsets=vvr_offsets, vvr_start=vvr_start, vvr_end=vvr_end)
+            vvr_offsets, vvr_start, vvr_end = self._read_vxrs2(
+                next_vxr_pos, vvr_offsets=vvr_offsets, vvr_start=vvr_start, vvr_end=vvr_end
+            )
         return vvr_offsets, vvr_start, vvr_end
 
-    def _read_vvrs(self, vdr_dict, vvr_offs, vvr_start, vvr_end, startrec, endrec, to_np=True):
+    def _read_vvrs(
+        self, vdr: VDR, vvr_offs: List[int], vvr_start: List[int], vvr_end: List[int], startrec: int, endrec: int
+    ) -> Union[str, np.ndarray]:
         """
         Reads in all VVRS that are pointed to in the VVR_OFFS array.
         Creates a large byte array of all values called "byte_stream".
         Decodes the byte_stream, then returns them.
         """
 
-        numBytes = self._type_size(vdr_dict['data_type'],
-                                   vdr_dict['num_elements'])
-        numValues = self._num_values(vdr_dict)
+        numBytes = self._type_size(vdr.data_type, vdr.num_elements)
+        numValues = self._num_values(vdr)
         totalRecs = endrec - startrec + 1
         firstBlock = -1
         lastBlock = -1
         totalBytes = numBytes * numValues * totalRecs
         byte_stream = bytearray(totalBytes)
         pos = 0
-        if (vdr_dict['sparse'] == 0):
+        if vdr.sparse == 0:
             for vvr_num in range(0, len(vvr_offs)):
-                if (vvr_end[vvr_num] >= startrec and firstBlock == -1):
+                if vvr_end[vvr_num] >= startrec and firstBlock == -1:
                     firstBlock = vvr_num
-                if (vvr_end[vvr_num] >= endrec):
+                if vvr_end[vvr_num] >= endrec:
                     lastBlock = vvr_num
                     break
             for vvr_num in range(firstBlock, (lastBlock + 1)):
-                if (self.cdfversion == 3):
+                if self.cdfversion == 3:
                     var_block_data = self._read_vvr_block(vvr_offs[vvr_num])
                 else:
                     var_block_data = self._read_vvr_block2(vvr_offs[vvr_num])
                 asize = len(var_block_data)
-                byte_stream[pos:pos + asize] = var_block_data
+                byte_stream[pos : pos + asize] = var_block_data
                 pos = pos + asize
             startPos = (startrec - vvr_start[firstBlock]) * numBytes * numValues
             stopOff = (vvr_end[lastBlock] - endrec) * numBytes * numValues
-            byte_stream = byte_stream[startPos:len(byte_stream) - stopOff]
+            byte_stream = byte_stream[startPos : len(byte_stream) - stopOff]
         else:
             # with sparse records
-            if ('pad' in vdr_dict):
+            if vdr.pad is not None:
                 # use default pad value
-                filled_data = self._convert_np_data(vdr_dict['pad'],
-                                                    vdr_dict['data_type'],
-                                                    vdr_dict['num_elements'])
+                filled_data = self._convert_np_data(vdr.pad, vdr.data_type, vdr.num_elements)
             else:
                 filled_data = self._convert_np_data(
-                    self._default_pad(vdr_dict['data_type'],
-                                      vdr_dict['num_elements']),
-                    vdr_dict['data_type'],
-                    vdr_dict['num_elements'])
+                    self._default_pad(vdr.data_type, vdr.num_elements),
+                    vdr.data_type,
+                    vdr.num_elements,
+                )
             cur_block = -1
             rec_size = numBytes * numValues
             for rec_num in range(startrec, (endrec + 1)):
-                block, prev_block = self._find_block(vvr_start, vvr_end,
-                                                     cur_block, rec_num)
-                if (block > -1):
+                block, prev_block = self._find_block(vvr_start, vvr_end, cur_block, rec_num)
+                if block > -1:
                     record_off = rec_num - vvr_start[block]
-                    if (cur_block != block):
-                        if (self.cdfversion == 3):
+                    if cur_block != block:
+                        if self.cdfversion == 3:
                             var_block_data = self._read_vvr_block(vvr_offs[block])
                         else:
                             var_block_data = self._read_vvr_block2(vvr_offs[block])
                         cur_block = block
                     xoff = record_off * rec_size
-                    byte_stream[pos:pos + rec_size] = var_block_data[xoff:
-                                                                     xoff + rec_size]
+                    byte_stream[pos : pos + rec_size] = var_block_data[xoff : xoff + rec_size]
                 else:
-                    if (vdr_dict['sparse'] == 1):
+                    if vdr.sparse == 1:
                         # use defined pad or default pad
-                        byte_stream[pos:pos + rec_size] = filled_data * numValues
+                        byte_stream[pos : pos + rec_size] = filled_data * numValues
                     else:
                         # use previous physical record
-                        if (prev_block != -1):
-                            if (self.cdfversion == 3):
-                                var_prev_block_data = self._read_vvr_block(
-                                    vvr_offs[prev_block])
+                        if prev_block != -1:
+                            if self.cdfversion == 3:
+                                var_prev_block_data = self._read_vvr_block(vvr_offs[prev_block])
                             else:
-                                var_prev_block_data = self._read_vvr_block2(
-                                    vvr_offs[prev_block])
-                            lastRecOff = (vvr_end[prev_block] -
-                                          vvr_start[prev_block]) * rec_size
-                            byte_stream[pos:pos + rec_size] = var_prev_block_data[lastRecOff:]
+                                var_prev_block_data = self._read_vvr_block2(vvr_offs[prev_block])
+                            lastRecOff = (vvr_end[prev_block] - vvr_start[prev_block]) * rec_size
+                            byte_stream[pos : pos + rec_size] = var_prev_block_data[lastRecOff:]
                         else:
-                            byte_stream[pos:pos + rec_size] = filled_data * numValues
+                            byte_stream[pos : pos + rec_size] = filled_data * numValues
                 pos = pos + rec_size
-                if (block > -1):
+                if block > -1:
                     cur_block = block
         dimensions = []
-        var_vary = vdr_dict['dim_vary']
-        var_sizes = vdr_dict['dim_sizes']
-        for x in range(0, vdr_dict['num_dims']):
-            if (var_vary[x] == 0):
+        var_vary = vdr.dim_vary
+        var_sizes = vdr.dim_sizes
+        for x in range(0, vdr.num_dims):
+            if var_vary[x] == 0:
                 continue
             dimensions.append(var_sizes[x])
-        if to_np:
-            y = self._read_data(byte_stream, vdr_dict['data_type'],
-                                totalRecs, vdr_dict['num_elements'],
-                                dimensions)
-        else:
-            if (vdr_dict['data_type'] == 32):
-                y = self._convert_data(byte_stream, vdr_dict['data_type'],
-                                       totalRecs, self._num_values(vdr_dict) * 2,
-                                       vdr_dict['num_elements'])
-            else:
-                y = self._convert_data(byte_stream, vdr_dict['data_type'],
-                                       totalRecs, self._num_values(vdr_dict),
-                                       vdr_dict['num_elements'])
-
-        return y
+        return self._read_data(byte_stream, vdr.data_type, totalRecs, vdr.num_elements, dimensions)
 
-    def _convert_option(self):
+    def _convert_option(self) -> str:
         """
         Determines how to convert CDF byte ordering to the system
         byte ordering.
         """
 
-        if sys.byteorder == 'little' and self._endian() == 'big-endian':
+        if sys.byteorder == "little" and self._endian() == "big-endian":
             # big->little
-            order = '>'
-        elif sys.byteorder == 'big' and self._endian() == 'little-endian':
+            order = ">"
+        elif sys.byteorder == "big" and self._endian() == "little-endian":
             # little->big
-            order = '<'
+            order = "<"
         else:
             # no conversion
-            order = '='
+            order = "="
         return order
 
     def _endian(self) -> str:
         """
         Determines endianess of the CDF file
         Only used in __init__
         """
-        if (self._encoding == 1 or self._encoding == 2 or self._encoding == 5 or
-            self._encoding == 7 or self._encoding == 9 or self._encoding == 11 or
-                self._encoding == 12):
-            return 'big-endian'
+        if (
+            self._encoding == 1
+            or self._encoding == 2
+            or self._encoding == 5
+            or self._encoding == 7
+            or self._encoding == 9
+            or self._encoding == 11
+            or self._encoding == 12
+        ):
+            return "big-endian"
         else:
-            return 'little-endian'
+            return "little-endian"
 
     @staticmethod
-    def _type_size(data_type, num_elms):
+    def _type_size(data_type: Union[int, str], num_elms: int) -> int:
         # DATA TYPES
         #
         # 1 - 1 byte signed int
         # 2 - 2 byte signed int
         # 4 - 4 byte signed int
         # 8 - 8 byte signed int
         # 11 - 1 byte unsigned int
@@ -1879,573 +1588,499 @@
         # 45 - same as 22
         # 31 - double representing milliseconds
         # 32 - 2 doubles representing milliseconds
         # 33 - 8 byte signed integer representing nanoseconds from J2000
         # 51 - signed character
         # 52 - unsigned character
 
-        if (isinstance(data_type, int)):
-            if ((data_type == 1) or (data_type == 11) or (data_type == 41)):
+        if isinstance(data_type, int):
+            if (data_type == 1) or (data_type == 11) or (data_type == 41):
                 return 1
-            elif ((data_type == 2) or (data_type == 12)):
+            elif (data_type == 2) or (data_type == 12):
                 return 2
-            elif ((data_type == 4) or (data_type == 14)):
+            elif (data_type == 4) or (data_type == 14):
                 return 4
-            elif ((data_type == 8) or (data_type == 33)):
+            elif (data_type == 8) or (data_type == 33):
                 return 8
-            elif ((data_type == 21) or (data_type == 44)):
+            elif (data_type == 21) or (data_type == 44):
                 return 4
-            elif ((data_type == 22) or (data_type == 31) or (data_type == 45)):
+            elif (data_type == 22) or (data_type == 31) or (data_type == 45):
                 return 8
-            elif (data_type == 32):
+            elif data_type == 32:
                 return 16
-            elif ((data_type == 51) or (data_type == 52)):
+            elif (data_type == 51) or (data_type == 52):
                 return num_elms
-        elif (isinstance(data_type, str)):
+            else:
+                raise TypeError("Unknown data type....")
+        elif isinstance(data_type, str):
             data_typeU = data_type.upper()
-            if ((data_typeU == 'CDF_INT1') or (data_typeU == 'CDF_UINT1') or
-                    (data_typeU == 'CDF_BYTE')):
+            if (data_typeU == "CDF_INT1") or (data_typeU == "CDF_UINT1") or (data_typeU == "CDF_BYTE"):
                 return 1
-            elif ((data_typeU == 'CDF_INT2') or (data_typeU == 'CDF_UINT2')):
+            elif (data_typeU == "CDF_INT2") or (data_typeU == "CDF_UINT2"):
                 return 2
-            elif ((data_typeU == 'CDF_INT4') or (data_typeU == 'CDF_UINT4')):
+            elif (data_typeU == "CDF_INT4") or (data_typeU == "CDF_UINT4"):
                 return 4
-            elif ((data_typeU == 'CDF_INT8') or (data_typeU == 'CDF_TIME_TT2000')):
+            elif (data_typeU == "CDF_INT8") or (data_typeU == "CDF_TIME_TT2000"):
                 return 8
-            elif ((data_typeU == 'CDF_REAL4') or (data_typeU == 'CDF_FLOAT')):
+            elif (data_typeU == "CDF_REAL4") or (data_typeU == "CDF_FLOAT"):
                 return 4
-            elif ((data_typeU == 'CDF_REAL8') or (data_typeU == 'CDF_DOUBLE') or
-                  (data_typeU == 'CDF_EPOCH')):
+            elif (data_typeU == "CDF_REAL8") or (data_typeU == "CDF_DOUBLE") or (data_typeU == "CDF_EPOCH"):
                 return 8
-            elif (data_typeU == 'CDF_EPOCH16'):
+            elif data_typeU == "CDF_EPOCH16":
                 return 16
-            elif ((data_typeU == 'CDF_CHAR') or (data_typeU == 'CDF_UCHAR')):
+            elif (data_typeU == "CDF_CHAR") or (data_typeU == "CDF_UCHAR"):
                 return num_elms
+            else:
+                raise TypeError("Unknown data type....")
         else:
-            raise TypeError('Unknown data type....')
+            raise TypeError("Unknown data type....")
 
-    def _read_data(self, byte_stream, data_type, num_recs, num_elems, dimensions=None):
+    def _read_data(
+        self, byte_stream: bytes, data_type: int, num_recs: int, num_elems: int, dimensions: Optional[List[int]] = None
+    ) -> Union[str, np.ndarray]:
         """
         This is the primary routine that converts streams of bytes into usable data.
 
         To do so, we need the bytes, the type of data, the number of records,
         the number of elements in a record, and dimension information.
         """
 
         squeeze_needed = False
         # If the dimension is [n], it needs to be [n,1]
         # for the numpy dtype.  This requires us to squeeze
         # the matrix later, to get rid of this extra dimension.
         dt_string = self._convert_option()
         if dimensions is not None:
-            if self._majority == 'Column_major':
+            if self._majority == "Column_major":
                 dimensions = list(reversed(dimensions))
-            if (len(dimensions) == 1):
+            if len(dimensions) == 1:
                 dimensions.append(1)
                 squeeze_needed = True
-            dt_string += '('
+            dt_string += "("
             count = 0
             for dim in dimensions:
                 count += 1
                 dt_string += str(dim)
                 if count < len(dimensions):
-                    dt_string += ','
-            dt_string += ')'
+                    dt_string += ","
+            dt_string += ")"
+
+        ret: Union[str, np.ndarray]
         if data_type == 52 or data_type == 51:
             # string
             if dimensions is None:
-                byte_data = bytearray(byte_stream[0:num_recs * num_elems])
+                byte_data = bytearray(byte_stream[0 : num_recs * num_elems])
                 # In each record, check for the first '\x00' (null character).
                 # If found, make all the characters after it null as well.
                 for x in range(0, num_recs):
                     y = x * num_elems
-                    z = byte_data[y:y + num_elems].find(b'\x00')
-                    if (z > -1 and z < (num_elems - 1)):
-                        byte_data[y + z + 1:y + num_elems] = b'\x00' * (num_elems - z - 1)
-                ret = byte_data[0:num_recs * num_elems].decode(self.string_encoding, errors='ignore').replace('\x00', '')
+                    z = byte_data[y : y + num_elems].find(b"\x00")
+                    if z > -1 and z < (num_elems - 1):
+                        byte_data[y + z + 1 : y + num_elems] = b"\x00" * (num_elems - z - 1)
+                ret = byte_data[0 : num_recs * num_elems].decode(self.string_encoding, errors="ignore").replace("\x00", "")
             else:
                 # Count total number of strings
                 count = 1
                 for x in range(0, len(dimensions)):
                     count = count * dimensions[x]
                 strings = []
-                if (len(dimensions) == 0):
+                if len(dimensions) == 0:
                     for i in range(0, num_recs * count * num_elems, num_elems):
-                        string1 = byte_stream[i:i + num_elems].decode(self.string_encoding, errors='ignore').\
-                            replace('\x00', '')
+                        string1 = byte_stream[i : i + num_elems].decode(self.string_encoding, errors="ignore").replace("\x00", "")
                         strings.append(string1)
                 else:
                     for x in range(0, num_recs):
                         onerec = []
-                        for i in range(x * count * num_elems, (x + 1) * count * num_elems,
-                                       num_elems):
-                            string1 = byte_stream[i:i + num_elems].decode(self.string_encoding, errors='ignore')\
-                                .replace('\x00', '')
+                        for i in range(x * count * num_elems, (x + 1) * count * num_elems, num_elems):
+                            string1 = (
+                                byte_stream[i : i + num_elems].decode(self.string_encoding, errors="ignore").replace("\x00", "")
+                            )
                             onerec.append(string1)
-                        strings.append(onerec)
-                ret = strings
-                ret = np.array(ret).reshape((num_recs,) + tuple(dimensions))
-                if self._majority == 'Column_major':
+                        strings.extend(onerec)
+                ret = np.array(strings).reshape((num_recs,) + tuple(dimensions))
+                if self._majority == "Column_major":
                     axes = [0] + list(range(len(dimensions), 0, -1))
                     ret = np.transpose(ret, axes=axes)
             return ret
         else:
             if (data_type == 1) or (data_type == 41):
-                dt_string += 'i1'
+                dt_string += "i1"
             elif data_type == 2:
-                dt_string += 'i2'
+                dt_string += "i2"
             elif data_type == 4:
-                dt_string += 'i4'
+                dt_string += "i4"
             elif (data_type == 8) or (data_type == 33):
-                dt_string += 'i8'
+                dt_string += "i8"
             elif data_type == 11:
-                dt_string += 'u1'
+                dt_string += "u1"
             elif data_type == 12:
-                dt_string += 'u2'
+                dt_string += "u2"
             elif data_type == 14:
-                dt_string += 'u4'
+                dt_string += "u4"
             elif (data_type == 21) or (data_type == 44):
-                dt_string += 'f'
+                dt_string += "f"
             elif (data_type == 22) or (data_type == 45) or (data_type == 31):
-                dt_string += 'd'
-            elif (data_type == 32):
-                dt_string += 'c16'
+                dt_string += "d"
+            elif data_type == 32:
+                dt_string += "c16"
             dt = np.dtype(dt_string)
             ret = np.frombuffer(byte_stream, dtype=dt, count=num_recs * num_elems)
             try:
-                ret.setflags('WRITEABLE')
+                ret.setflags(write=True)
             except ValueError:
                 # If we can't set the writable flag, just continue
                 pass
 
         if squeeze_needed:
             ret = np.squeeze(ret, axis=(ret.ndim - 1))
             if dimensions is not None:
                 dimensions.pop()
 
         # Put the data into system byte order
-        if self._convert_option() != '=':
+        if self._convert_option() != "=":
             ret = ret.byteswap().newbyteorder()
 
-        if self._majority == 'Column_major':
+        if self._majority == "Column_major":
             if dimensions is not None:
                 axes = [0] + list(range(len(dimensions), 0, -1))
             else:
                 axes = None
             ret = np.transpose(ret, axes=axes)
 
         return ret
 
-    def _num_values(self, vdr_dict):
+    def _num_values(self, vdr: VDR) -> int:
         """
         Returns the number of values in a record, using a given VDR
         dictionary. Multiplies the dimension sizes of each dimension,
         if it is varying.
         """
         values = 1
-        for x in range(0, vdr_dict['num_dims']):
-            if (vdr_dict['dim_vary'][x] != 0):
-                values = values * vdr_dict['dim_sizes'][x]
+        for x in range(0, vdr.num_dims):
+            if vdr.dim_vary[x] != 0:
+                values = values * vdr.dim_sizes[x]
         return values
 
-    def _get_attdata(self, adr_info, entry_num, num_entry, first_entry, to_np=True):
+    def _get_attdata(self, adr_info: ADRInfo, entry_num: int, num_entry: int, first_entry: int) -> AttData:
         position = first_entry
         for _ in range(0, num_entry):
             got_entry_num, next_aedr = self._read_aedr_fast(position)
             if entry_num == got_entry_num:
-                aedr_info = self._read_aedr(position, to_np=to_np)
-                return_dict = {}
-                return_dict['Item_Size'] = self._type_size(aedr_info['data_type'],
-                                                           aedr_info['num_elements'])
-                return_dict['Data_Type'] = self._datatype_token(aedr_info['data_type'])
-
-                return_dict['Num_Items'] = aedr_info['num_elements']
-                return_dict['Data'] = aedr_info['entry']
-                if (aedr_info['data_type'] == 51 or aedr_info['data_type'] == 52):
-                    if 'num_strings' in aedr_info:
-                        return_dict['Num_Items'] = aedr_info['num_strings']
-                        if (aedr_info['num_strings'] > 1):
-                            return_dict['Data'] = aedr_info['entry'].split('\\N ')
-                if not to_np and (aedr_info['data_type'] == 32):
-                    return_dict['Data'] = complex(aedr_info['entry'][0],
-                                                  aedr_info['entry'][1])
-                return return_dict
+                aedr_info = self._read_aedr(position)
+                item_size = self._type_size(aedr_info.data_type, aedr_info.num_elements)
+                data_type = self._datatype_token(aedr_info.data_type)
+
+                num_items = aedr_info.num_elements
+                data = aedr_info.entry
+                if isinstance(data, str):
+                    if aedr_info.num_strings is not None:
+                        num_strings = aedr_info.num_strings
+                        num_items = num_strings
+                        if num_strings > 1 and isinstance(aedr_info.entry, str):
+                            data = np.array(aedr_info.entry.split("\\N "))
+                return AttData(item_size, data_type, num_items, data)
             else:
                 position = next_aedr
 
-        raise KeyError('The entry does not exist')
-
-    def _read_vardata(self, vdr_info, epoch=None, starttime=None, endtime=None,
-                      startrec=0, endrec=None, record_range_only=False,
-                      expand=False, to_np=True):
+        raise KeyError("The entry does not exist")
 
+    def _read_vardata(
+        self,
+        vdr_info: VDR,
+        epoch: Optional[str] = None,
+        starttime: Optional[epoch.epoch_types] = None,
+        endtime: Optional[epoch.epoch_types] = None,
+        startrec: int = 0,
+        endrec: Optional[int] = None,
+    ) -> Optional[Union[str, np.ndarray]]:
         # Error checking
         if startrec:
-            if (startrec < 0):
-                raise ValueError('Invalid start recond')
-            if not (vdr_info['record_vary']):
+            if startrec < 0:
+                raise ValueError("Invalid start recond")
+            if not (vdr_info.record_vary):
                 startrec = 0
 
         if not (endrec is None):
-            if ((endrec < 0) or (endrec > vdr_info['max_records']) or
-                    (endrec < startrec)):
-                raise ValueError('Invalid end recond')
-            if not (vdr_info['record_vary']):
+            if (endrec < 0) or (endrec > vdr_info.max_rec) or (endrec < startrec):
+                raise ValueError("Invalid end recond")
+            if not (vdr_info.record_vary):
                 endrec = 0
         else:
-            endrec = vdr_info['max_records']
-        if (self.cdfversion == 3):
-            vvr_offsets, vvr_start, vvr_end = self._read_vxrs(vdr_info['head_vxr'],
-                                                              vvr_offsets=[], vvr_start=[], vvr_end=[])
+            endrec = vdr_info.max_rec
+        if self.cdfversion == 3:
+            vvr_offsets, vvr_start, vvr_end = self._read_vxrs(vdr_info.head_vxr, vvr_offsets=[], vvr_start=[], vvr_end=[])
         else:
-            vvr_offsets, vvr_start, vvr_end = self._read_vxrs2(vdr_info['head_vxr'],
-                                                               vvr_offsets=[], vvr_start=[], vvr_end=[])
+            vvr_offsets, vvr_start, vvr_end = self._read_vxrs2(vdr_info.head_vxr, vvr_offsets=[], vvr_start=[], vvr_end=[])
 
-        if (vdr_info['record_vary']):
+        if vdr_info.record_vary:
             # Record varying
-            if (starttime is not None or endtime is not None):
-                recs = self._findtimerecords(vdr_info['name'], starttime,
-                                             endtime, epoch=epoch)
+            if starttime is not None or endtime is not None:
+                recs = self._findtimerecords(vdr_info.name, starttime, endtime, epoch=epoch)
                 if recs is None:
-                    return
-                if len(recs) == 0:
-                    return
+                    return None
+                elif len(recs) == 0:
+                    return None
                 else:
                     startrec = recs[0]
                     endrec = recs[-1]
         else:
             startrec = 0
             endrec = 0
 
-        data = self._read_vvrs(vdr_info, vvr_offsets, vvr_start, vvr_end,
-                               startrec, endrec, to_np=to_np)
-        if record_range_only:
-            return [startrec, endrec]
-        if (expand):
-            new_dict = {}
-            new_dict['Rec_Ndim'] = vdr_info['num_dims']
-            new_dict['Rec_Shape'] = vdr_info['dim_sizes']
-            new_dict['Num_Records'] = vdr_info['max_records'] + 1
-            new_dict['Records_Returned'] = endrec - startrec
-            new_dict['Item_Size'] = self._type_size(vdr_info['data_type'],
-                                                    vdr_info['num_elements'])
-            new_dict['Data_Type'] = self._datatype_token(vdr_info['data_type'])
-            new_dict['Data'] = data
-            if (vdr_info['sparse']):
-                blocks = len(vvr_start)
-                physical_recs = []
-                for x in range(0, blocks):
-                    for y in range(vvr_start[x], vvr_end[x] + 1):
-                        physical_recs.append(y)
-                new_dict['Real_Records'] = physical_recs
-            return new_dict
-        else:
-            if (vdr_info['record_vary']):
-                return data
-            else:
-                return data[0]
-
-    def _findtimerecords(self, var_name, starttime, endtime, epoch=None):
-
-        if (epoch is not None):
+        data = self._read_vvrs(vdr_info, vvr_offsets, vvr_start, vvr_end, startrec, endrec)
+        if vdr_info.record_vary:
+            return data
+        else:
+            return data[0]
+
+    def _findtimerecords(
+        self, var_name: str, starttime: epoch.epoch_types, endtime: epoch.epoch_types, epoch: Optional[str] = None
+    ) -> np.ndarray:
+        if epoch is not None:
             vdr_info = self.varinq(epoch)
-            if (vdr_info is None):
-                raise ValueError('Epoch not found')
-            if (vdr_info['Data_Type'] == 31 or vdr_info['Data_Type'] == 32 or
-                    vdr_info['Data_Type'] == 33):
+            if vdr_info is None:
+                raise ValueError("Epoch not found")
+            if vdr_info.Data_Type == 31 or vdr_info.Data_Type == 32 or vdr_info.Data_Type == 33:
                 epochtimes = self.varget(epoch)
         else:
             vdr_info = self.varinq(var_name)
-            if (vdr_info['Data_Type'] == 31 or vdr_info['Data_Type'] == 32 or
-                    vdr_info['Data_Type'] == 33):
+            if vdr_info.Data_Type == 31 or vdr_info.Data_Type == 32 or vdr_info.Data_Type == 33:
                 epochtimes = self.varget(var_name)
             else:
                 # acquire depend_0 variable
-                dependVar = self.attget('DEPEND_0', var_name)
-                if (dependVar is None):
+                dependVar = self.attget("DEPEND_0", var_name)
+                if dependVar is None:
                     raise ValueError(
                         "No corresponding epoch from 'DEPEND_0' attribute "
-                        "for variable: {}".format(var_name) +
-                        "Use 'epoch' argument to specify its time-based "
-                        "variable")
-
-                vdr_info = self.varinq(dependVar['Data'])
-                if (vdr_info['Data_Type'] != 31 and vdr_info['Data_Type'] != 32
-                        and vdr_info['Data_Type'] != 33):
+                        "for variable: {}".format(var_name) + "Use 'epoch' argument to specify its time-based "
+                        "variable"
+                    )
+
+                if not isinstance(dependVar.Data, str):
+                    raise ValueError()
+
+                vdr_info = self.varinq(dependVar.Data)
+                if vdr_info.Data_Type != 31 and vdr_info.Data_Type != 32 and vdr_info.Data_Type != 33:
                     raise ValueError(
                         "Corresponding variable from 'DEPEND_0' attribute "
-                        "for variable: {}".format(var_name) +
-                        ' is not a CDF epoch type')
-                epochtimes = self.varget(dependVar['Data'])
+                        "for variable: {}".format(var_name) + " is not a CDF epoch type"
+                    )
 
-        return self._findrangerecords(vdr_info['Data_Type'], epochtimes,
-                                      starttime, endtime)
+                epochtimes = self.varget(dependVar.Data)
 
-    def _findrangerecords(self, data_type, epochtimes, starttime, endtime):
-        if (data_type == 31 or data_type == 32 or data_type == 33):
+        return self._findrangerecords(vdr_info.Data_Type, epochtimes, starttime, endtime)
+
+    def _findrangerecords(
+        self, data_type: int, epochtimes: epoch.epochs_type, starttime: epoch.epoch_types, endtime: epoch.epoch_types
+    ) -> np.ndarray:
+        if data_type == 31 or data_type == 32 or data_type == 33:
             # CDF_EPOCH or CDF_EPOCH16 or CDF_TIME_TT2000
             recs = epoch.CDFepoch.findepochrange(epochtimes, starttime, endtime)
         else:
-            raise ValueError('Not a CDF epoch type')
+            raise ValueError("Not a CDF epoch type")
         return recs
 
-    def _convert_type(self, data_type):
+    def _convert_type(self, data_type: int) -> str:
         """
         CDF data types to python struct data types
         """
         if (data_type == 1) or (data_type == 41):
-            dt_string = 'b'
+            dt_string = "b"
         elif data_type == 2:
-            dt_string = 'h'
+            dt_string = "h"
         elif data_type == 4:
-            dt_string = 'i'
+            dt_string = "i"
         elif (data_type == 8) or (data_type == 33):
-            dt_string = 'q'
+            dt_string = "q"
         elif data_type == 11:
-            dt_string = 'B'
+            dt_string = "B"
         elif data_type == 12:
-            dt_string = 'H'
+            dt_string = "H"
         elif data_type == 14:
-            dt_string = 'I'
+            dt_string = "I"
         elif (data_type == 21) or (data_type == 44):
-            dt_string = 'f'
+            dt_string = "f"
         elif (data_type == 22) or (data_type == 45) or (data_type == 31):
-            dt_string = 'd'
-        elif (data_type == 32):
-            dt_string = 'd'
+            dt_string = "d"
+        elif data_type == 32:
+            dt_string = "d"
         elif (data_type == 51) or (data_type == 52):
-            dt_string = 's'
+            dt_string = "s"
         return dt_string
 
-    def _default_pad(self, data_type, num_elms):
+    def _default_pad(self, data_type: int, num_elms: int) -> Union[str, np.ndarray]:
         """
         The default pad values by CDF data type
         """
         order = self._convert_option()
-        if (data_type == 51 or data_type == 52):
-            return str(' ' * num_elms)
+        if data_type == 51 or data_type == 52:
+            return str(" " * num_elms)
         if (data_type == 1) or (data_type == 41):
-            pad_value = struct.pack(order + 'b', -127)
-            dt_string = 'i1'
+            pad_value = struct.pack(order + "b", -127)
+            dt_string = "i1"
         elif data_type == 2:
-            pad_value = struct.pack(order + 'h', -32767)
-            dt_string = 'i2'
+            pad_value = struct.pack(order + "h", -32767)
+            dt_string = "i2"
         elif data_type == 4:
-            pad_value = struct.pack(order + 'i', -2147483647)
-            dt_string = 'i4'
+            pad_value = struct.pack(order + "i", -2147483647)
+            dt_string = "i4"
         elif (data_type == 8) or (data_type == 33):
-            pad_value = struct.pack(order + 'q', -9223372036854775807)
-            dt_string = 'i8'
+            pad_value = struct.pack(order + "q", -9223372036854775807)
+            dt_string = "i8"
         elif data_type == 11:
-            pad_value = struct.pack(order + 'B', 254)
-            dt_string = 'u1'
+            pad_value = struct.pack(order + "B", 254)
+            dt_string = "u1"
         elif data_type == 12:
-            pad_value = struct.pack(order + 'H', 65534)
-            dt_string = 'u2'
+            pad_value = struct.pack(order + "H", 65534)
+            dt_string = "u2"
         elif data_type == 14:
-            pad_value = struct.pack(order + 'I', 4294967294)
-            dt_string = 'u4'
+            pad_value = struct.pack(order + "I", 4294967294)
+            dt_string = "u4"
         elif (data_type == 21) or (data_type == 44):
-            pad_value = struct.pack(order + 'f', -1.0E30)
-            dt_string = 'f'
+            pad_value = struct.pack(order + "f", -1.0e30)
+            dt_string = "f"
         elif (data_type == 22) or (data_type == 45) or (data_type == 31):
-            pad_value = struct.pack(order + 'd', -1.0E30)
-            dt_string = 'd'
+            pad_value = struct.pack(order + "d", -1.0e30)
+            dt_string = "d"
         else:
             # (data_type == 32):
-            pad_value = struct.pack(order + '2d', *[-1.0E30, -1.0E30])
-            dt_string = 'c16'
+            pad_value = struct.pack(order + "2d", *[-1.0e30, -1.0e30])
+            dt_string = "c16"
 
         dt = np.dtype(dt_string)
         ret = np.frombuffer(pad_value, dtype=dt, count=1)
         try:
-            ret.setflags('WRITEABLE')
+            ret.setflags(write=True)
         except Exception:
             # TODO: Figure out why we need to array set to writeable
             pass
         return ret
 
-    def _convert_np_data(self, data, data_type, num_elems):
+    def _convert_np_data(self, data: Union[str, np.ndarray], data_type: int, num_elems: int) -> bytes:
         """
         Converts a single np data into byte stream.
         """
-        if (data_type == 51 or data_type == 52):
-            if (data == ''):
-                return ('\x00' * num_elems).encode()
+        if isinstance(data, str):
+            if data == "":
+                return ("\x00" * num_elems).encode()
             else:
-                return data.ljust(num_elems, '\x00').encode(self.string_encoding)
-        elif (data_type == 32):
+                return data.ljust(num_elems, "\x00").encode(self.string_encoding)
+        elif isinstance(data, np.ndarray):
             data_stream = data.real.tobytes()
             data_stream += data.imag.tobytes()
             return data_stream
         else:
             return data.tobytes()
 
-    def _read_vvr_block(self, offset):
+    def _read_vvr_block(self, offset: int) -> bytes:
         """
         Returns a VVR or decompressed CVVR block
         """
         self._f.seek(offset, 0)
-        block_size = int.from_bytes(self._f.read(8), 'big')
+        block_size = int.from_bytes(self._f.read(8), "big")
         block = self._f.read(block_size - 8)
 
-        section_type = int.from_bytes(block[0:4], 'big')
+        section_type = int.from_bytes(block[0:4], "big")
         if section_type == 13:
             # a CVVR
-            compressed_size = int.from_bytes(block[8:16], 'big')
-            return gzip.decompress(block[16:16 + compressed_size])
+            compressed_size = int.from_bytes(block[8:16], "big")
+            return gzip.decompress(block[16 : 16 + compressed_size])
         elif section_type == 7:
             # a VVR
             return block[4:]
+        else:
+            raise RuntimeError("Unexpected section type")
 
-    def _read_vvr_block2(self, offset):
+    def _read_vvr_block2(self, offset: int) -> bytes:
         """
         Returns a VVR or decompressed CVVR block
         """
         self._f.seek(offset, 0)
-        block_size = int.from_bytes(self._f.read(4), 'big')
+        block_size = int.from_bytes(self._f.read(4), "big")
         block = self._f.read(block_size - 4)
 
-        section_type = int.from_bytes(block[0:4], 'big')
+        section_type = int.from_bytes(block[0:4], "big")
         if section_type == 13:
             # a CVVR
-            compressed_size = int.from_bytes(block[8:12], 'big')
-            return gzip.decompress(block[12:12 + compressed_size])
+            compressed_size = int.from_bytes(block[8:12], "big")
+            return gzip.decompress(block[12 : 12 + compressed_size])
         elif section_type == 7:
             # a VVR
             return block[4:]
+        else:
+            raise RuntimeError("Unexpected section type")
 
     @staticmethod
-    def _find_block(starts, ends, cur_block, rec_num):
+    def _find_block(starts: List[int], ends: List[int], cur_block: int, rec_num: int) -> Tuple[int, int]:
         """
         Finds the block that rec_num is in if it is found. Otherwise it returns -1.
         It also returns the block that has the physical data either at or
         preceeding the rec_num.
         It could be -1 if the preceeding block does not exists.
         """
         total = len(starts)
-        if (cur_block == -1):
+        if cur_block == -1:
             cur_block = 0
         for x in range(cur_block, total):
-            if (starts[x] <= rec_num and ends[x] >= rec_num):
+            if starts[x] <= rec_num and ends[x] >= rec_num:
                 return x, x
-            if (starts[x] > rec_num):
+            if starts[x] > rec_num:
                 break
         return -1, x - 1
 
-    def _convert_data(self, data, data_type, num_recs, num_values, num_elems):
-        """
-        Converts data to the appropriate type using the struct.unpack method,
-        rather than using numpy.
-        """
-
-        if (data_type == 51 or data_type == 52):
-            return [data[i:i + num_elems].decode(self.string_encoding) for i in
-                    range(0, num_recs * num_values * num_elems, num_elems)]
-        else:
-            tofrom = self._convert_option()
-            dt_string = self._convert_type(data_type)
-            form = tofrom + str(num_recs * num_values * num_elems) + dt_string
-            value_len = self._type_size(data_type, num_elems)
-            return list(struct.unpack_from(form,
-                                           data[0:num_recs * num_values * value_len]))
-
-    def _file_or_url_or_s3_handler(self, filename, filetype, s3_read_method):
-        if filetype == 'url':
+    def _file_or_url_or_s3_handler(
+        self, filename: str, filetype: str, s3_read_method: int
+    ) -> Union["S3object", io.BufferedReader, io.BytesIO]:
+        bdata: Union["S3object", io.BufferedReader, io.BytesIO]
+        if filetype == "url":
             # print("debug, opening url")
             req = urllib.request.Request(filename)
             response = urllib.request.urlopen(req)
             bdata = io.BytesIO(response.read())
-        elif filetype == 's3':
+        elif filetype == "s3":
             try:
                 import boto3
             except:
-                raise ImportError('boto3 package not installed')
-            s3parts = filename.split('/')  # 0-1=s3://, 2=bucket, 3+=key
+                raise ImportError("boto3 package not installed")
+            s3parts = filename.split("/")  # 0-1=s3://, 2=bucket, 3+=key
             mybucket = s3parts[2]
-            mykey = '/'.join(s3parts[3:])
+            mykey = "/".join(s3parts[3:])
             if s3_read_method == 3:
                 # read in-place
-                s3c = boto3.resource('s3')
+                s3c = boto3.resource("s3")
                 obj = s3c.Object(bucket_name=mybucket, key=mykey)
-                bdata = S3object(obj)
+                bdata = S3object(obj)  # type: ignore
                 # print("Debug, using S3 read-in-place, flag ",s3_flag)
             else:
                 # for store in memory or as temp copy
-                s3c = boto3.client('s3')
+                s3c = boto3.client("s3")
                 obj = s3c.get_object(Bucket=mybucket, Key=mykey)
                 bdata = s3_fetchall(obj)
                 # print("Debug, using S3 copy, flag ",s3_flag)
-            return (bdata)
+            return bdata
         else:
             # print("debug, opening ",fname)
             bdata = open(filename, "rb")
 
-        return (bdata)
+        return bdata
 
-    def _unstream_file(self, path, f):
+    def _unstream_file(self, f) -> None:  # type: ignore
         """
         Typically for S3 or URL, writes the current file stream
         into a file in the temporary directory.
         If that doesn't work, create a new file in the CDFs directory.
         """
         raw_data = f.read(-1)
-        self.temp_file = Path(tempfile.NamedTemporaryFile(suffix='.cdf').name)
+        self.temp_file = Path(tempfile.NamedTemporaryFile(suffix=".cdf").name)
         # print("debug, using temp file: ",self.temp_file)
-        with self.temp_file.open('wb') as g:
+        with self.temp_file.open("wb") as g:
             g.write(raw_data)
         self.original_stream = self.file
         self.file = self.temp_file
         self.file = Path(self.file).expanduser()
-        self.ftype = 'file'
-        # print("debug, using temp file ",self.temp_file)
+        self.ftype = "file"
 
 
-def s3_fetchall(obj):
-    rawdata = obj['Body'].read()
+def s3_fetchall(obj) -> io.BytesIO:  # type: ignore
+    rawdata = obj["Body"].read()
     bdata = io.BytesIO(rawdata)
-    return (bdata)
-
-
-class S3object:
-    """
-    Handler for S3 objects so they behave like files.
-    S3 'read' reads specified byte range
-    S3 'seek' sets byte range for subsequent readers
-    """
-
-    def __init__(self, fhandle):
-        self.pos = 0  # used to track where in S3 we are
-        self.content_length = fhandle.content_length  # size in bytes
-        self.fhandle = fhandle
-        self.temp_file = None
-
-    def read(self, isize):
-        if isize == -1:
-            isize = self.content_length
-        myrange = "bytes=%d-%d" % (self.pos, (self.pos + isize - 1))
-        # print("debug: byte range ",myrange)
-        self.pos += isize  # advance the pointer
-        stream = self.fhandle.get(Range=myrange)['Body']
-        rawdata = stream.read()
-        # bdata=io.BytesIO(rawdata)
-        return (rawdata)
-
-    def seek(self, offset, from_what=0):
-        if from_what == 2:
-            # offset is from end of file, ugh, used only for checksum
-            self.pos = self.content_length + offset
-        elif from_what == 1:
-            # from current position
-            self.pos = self.pos + offset
-        else:
-            # usual default is 0, from start of file
-            self.pos = offset
-
-    def tell(self):
-        return (self.pos)
-
-    def fetchS3entire(self):
-        obj = self.fhandle.get()['Body']
-        rawdata = obj['Body'].read()
-        bdata = io.BytesIO(rawdata)
-        return (bdata)
+    return bdata
```

### Comparing `cdflib-0.4.9/cdflib/cdfwrite.py` & `cdflib-1.0.0/cdflib/cdfwrite.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-This is a python script to write a CDF file from scratch
-without needing to install the CDF NASA library.
-This Python code only creates V3 CDFs.
-
-@author: Mike Liu
-"""
 import binascii
 import gzip
 import hashlib
+import io
 import logging
 import math
 import numbers
 import pathlib
 import platform as pf
 import struct
 import sys
 import warnings
-from typing import Tuple
+from functools import wraps
+from numbers import Number
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 import cdflib.epochs as cdfepoch
 
+__all__ = ["CDF"]
+
 
 def is_open(func):
+    @wraps(func)
     def ensure_open(self, *args, **kwargs):
         if self.is_closed:
             raise OSError("This file is already closed, and can no longer be modified.")
         else:
             return func(self, *args, **kwargs)
 
     return ensure_open
@@ -132,17 +132,17 @@
     GZIP_COMPRESSION = 5
 
     # RLE_OF_ZEROs	= 0
     # NO_SPARSEARRAYS = 0
     NO_SPARSERECORDS = 0
     PAD_SPARSERECORDS = 1
     PREV_SPARSERECORDS = 2
-    V3magicNUMBER_1 = 'cdf30001'
-    V3magicNUMBER_2 = '0000ffff'
-    V3magicNUMBER_2c = 'cccc0001'
+    V3magicNUMBER_1 = "cdf30001"
+    V3magicNUMBER_2 = "0000ffff"
+    V3magicNUMBER_2c = "cccc0001"
     CDR_ = 1
     GDR_ = 2
     rVDR_ = 3
     ADR_ = 4
     AgrEDR_ = 5
     VXR_ = 6
     VVR_ = 7
@@ -167,101 +167,101 @@
     ADR_BASE_SIZE64 = 68 + CDF_ATTR_NAME_LEN256
     AEDR_BASE_SIZE64 = 56
     CCR_BASE_SIZE64 = 32
     CPR_BASE_SIZE64 = 24
     SPR_BASE_SIZE64 = 24
     CVVR_BASE_SIZE64 = 24
 
-    #BLOCKING_BYTES = 131072
+    # BLOCKING_BYTES = 131072
     BLOCKING_BYTES = 65536
 
     level = 0
 
-    def __init__(self, path, cdf_spec=None, delete=False):
+    def __init__(self, path: Union[str, Path], cdf_spec: Optional[Dict[str, Any]] = None, delete: bool = False):
         path = pathlib.Path(path).expanduser()
 
         major = 1
         if cdf_spec is not None:
-            if (isinstance(major, str)):
+            major = cdf_spec.get("Majority", major)
+            if isinstance(major, str):
                 major = self._majority_token(major)
 
-            encoding = cdf_spec.get('Encoding', 8)  # default is host
-            if (isinstance(encoding, str)):
+            encoding = cdf_spec.get("Encoding", 8)  # default is host
+            if isinstance(encoding, str):
                 encoding = self._encoding_token(encoding)
 
-            checksum = cdf_spec.get('Checksum', False)
+            checksum = cdf_spec.get("Checksum", False)
 
-            cdf_compression = cdf_spec.get('Compressed', 0)
-            if (isinstance(cdf_compression, int)):
+            cdf_compression = cdf_spec.get("Compressed", 0)
+            if isinstance(cdf_compression, int):
                 if not 0 <= cdf_compression <= 9:
                     cdf_compression = 0
             else:
                 cdf_compression = 6 if cdf_compression else 0
 
-            rdim_sizes = cdf_spec.get('rDim_sizes', None)
-            num_rdim = len(rdim_sizes) if rdim_sizes is not None else 0
+            rdim_sizes: Optional[List[int]] = cdf_spec.get("rDim_sizes", None)
+            num_rdim: int = len(rdim_sizes) if rdim_sizes is not None else 0
 
         else:
             encoding = 8
             checksum = False
             cdf_compression = 0
             num_rdim = 0
             rdim_sizes = None
 
-        if (major < 1 or major > 2):
-            raise OSError('Bad major.')
+        if major not in [1, 2]:
+            raise RuntimeError(f"Bad major: {major}")
 
         osSystem = pf.system()
         osMachine = pf.uname()[5]
-        if (encoding == 8):
-            if osSystem != 'SunOS' or osMachine != 'sparc':
+        if encoding == 8:
+            if osSystem != "SunOS" or osMachine != "sparc":
                 self._encoding = self.IBMPC_ENCODING
             else:
                 self._encoding = self.SUN_ENCODING
         else:
             self._encoding = encoding
-            if (self._encoding == -1):
-                raise OSError('Bad encoding.')
+            if self._encoding == -1:
+                raise OSError("Bad encoding.")
         if not isinstance(checksum, bool):
-            raise ValueError('Bad checksum.')
+            raise ValueError("Bad checksum.")
 
-        if path.suffix != '.cdf':
-            path = path.with_suffix('.cdf')
+        if path.suffix != ".cdf":
+            path = path.with_suffix(".cdf")
         if len(str(path)) > self.CDF_PATHNAME_LEN:
-            raise OSError('CDF:', path, ' longer than allowed length.')
+            raise OSError("CDF:", path, " longer than allowed length.")
         if path.is_file():
             if not delete:
-                raise OSError('file: ', path, ' already exists....\n',
-                              'Delete it or specify the \'delete=False\' option.')
+                raise OSError("file: ", path, " already exists....\n", "Delete it or specify the 'delete=False' option.")
             else:
                 path.unlink()
 
         self.path = path
 
-        self.compressed_file = path.with_suffix('.tmp') if cdf_compression > 0 else None
+        self.compressed_file = path.with_suffix(".tmp") if cdf_compression > 0 else None
 
         # Dictionary objects, these contains name, offset, and dimension information
-        self.zvarsinfo = {}
-        self.rvarsinfo = {}
+        self.zvarsinfo: Dict[int, Tuple[str, int, int, List[int], List[bool]]] = {}
+        self.rvarsinfo: Dict[int, Tuple[str, int, int, List[int], List[bool]]] = {}
 
         # Dictionary object, contains name, offset, and scope (global or variable)
-        self.attrsinfo = {}
+        self.attrsinfo: Dict[int, Tuple[str, int, int]] = {}
 
-        self.gattrs = []  # List of global attributes
-        self.vattrs = []  # List of variable attributes
-        self.attrs = []  # List of ALL attributes
-        self.zvars = []  # List of z variable names
-        self.rvars = []  # List of r variable names
+        self.gattrs: List[str] = []  # List of global attributes
+        self.vattrs: List[str] = []  # List of variable attributes
+        self.attrs: List[str] = []  # List of ALL attributes
+        self.zvars: List[str] = []  # List of z variable names
+        self.rvars: List[str] = []  # List of r variable names
         self.checksum = checksum  # Boolean, whether or not to include the checksum at the end
         self.compression = cdf_compression  # Compression level (or True/False)
         self.num_rdim = num_rdim  # Number of r dimensions
         self.rdim_sizes = rdim_sizes  # Size of r dimensions
         self.majority = major
 
-        with path.open('wb') as f:
+        with path.open("wb") as f:
             f.write(binascii.unhexlify(self.V3magicNUMBER_1))
             f.write(binascii.unhexlify(self.V3magicNUMBER_2))
 
             self.cdr_head = self._write_cdr(f, major, self._encoding, checksum)
             self.gdr_head = self._write_gdr(f)
             self.offset = f.tell()
 
@@ -270,58 +270,58 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
         return
 
-    def close(self):
-        '''
+    def close(self) -> None:
+        """
         Closes the CDF Class.
 
             1. If compression was set, this is where the compressed file is
                written.
             2. If a checksum is needed, this will place the checksum at the end
                of the file.
 
-        '''
+        """
         if self.is_closed:
             return
 
         if self.compressed_file is None:
-            with self.path.open('rb+') as f:
+            with self.path.open("rb+") as f:
                 f.seek(0, 2)
                 eof = f.tell()
                 self._update_offset_value(f, self.gdr_head + 36, 8, eof)
                 if self.checksum:
                     f.write(self._md5_compute(f))
                 self.is_closed = True
             return
-# %%
-        with self.path.open('rb+') as f:
+
+        with self.path.open("rb+") as f:
             f.seek(0, 2)
             eof = f.tell()
             self._update_offset_value(f, self.gdr_head + 36, 8, eof)
 
-            with self.compressed_file.open('wb+') as g:
+            with self.compressed_file.open("wb+") as g:
                 g.write(bytearray.fromhex(self.V3magicNUMBER_1))
                 g.write(bytearray.fromhex(self.V3magicNUMBER_2c))
                 self._write_ccr(f, g, self.compression)
 
                 if self.checksum:
                     g.seek(0, 2)
                     g.write(self._md5_compute(g))
 
         self.path.unlink()  # NOTE: for Windows this is necessary
         self.compressed_file.rename(self.path)
         self.is_closed = True
 
     @is_open
     def write_globalattrs(self, globalAttrs):
-        '''
+        """
         Writes the global attributes.
 
         Parameters
         ----------
         globalAttrs: dict
             Global attribute name(s) and their value(s) pair(s).
 
@@ -355,73 +355,67 @@
                 GA6[0]='abcd'
                 GA6[1]=[12, 'cdf_int2']
                 GA6[2]=[12.5, 'cdf_float']
                 GA6[3]=[[0,1,2], 'cdf_int8']
                 globalAttrs['Global6']=GA6
                 ....
                 f.write_globalattrs(globalAttrs)
-        '''
+        """
         if not (isinstance(globalAttrs, dict)):
-            raise ValueError('Global attribute(s) not in dictionary form')
+            raise ValueError("Global attribute(s) not in dictionary form")
         dataType = None
         numElems = None
-        with self.path.open('rb+') as f:
+        with self.path.open("rb+") as f:
             f.seek(0, 2)  # EOF (appending)
             for attr, entry in globalAttrs.items():
-                if (attr in self.gattrs):
-                    raise ValueError(f'Global attribute: {attr} already exists.')
+                if attr in self.gattrs:
+                    raise ValueError(f"Global attribute: {attr} already exists.")
 
-                if (attr in self.vattrs):
-                    logging.warning(f'Attribute: {attr} already defined as a variable attribute.')
+                if attr in self.vattrs:
+                    logging.warning(f"Attribute: {attr} already defined as a variable attribute.")
                     continue
 
                 attrNum, offsetADR = self._write_adr(f, True, attr)
                 entries = 0
                 if entry is None:
                     continue
                 entryNumMaX = -1
                 poffset = -1
                 for entryNum, value in entry.items():
-                    if (entryNumMaX < entryNum):
+                    if entryNumMaX < entryNum:
                         entryNumMaX = entryNum
-                    if hasattr(value, '__len__') and not isinstance(value, str):
-                        if (len(value) == 2):
+                    if hasattr(value, "__len__") and not isinstance(value, str):
+                        if len(value) == 2:
                             # Check if the second value is a valid data type
                             value2 = value[1]
                             dataType = self._datatype_token(value2)
-                            if (dataType > 0):
+                            if dataType > 0:
                                 # Data Type found
                                 data = value[0]
-                                if (dataType == self.CDF_CHAR or
-                                        dataType == self.CDF_UCHAR):
-                                    if (isinstance(data, list) or
-                                            isinstance(data, tuple)):
-                                        warnings.warn('Invalid global attribute value')
+                                if dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR:
+                                    if isinstance(data, list) or isinstance(data, tuple):
+                                        warnings.warn("Invalid global attribute value")
                                         return
                                     numElems = len(data)
-                                elif (dataType == self.CDF_EPOCH or
-                                      dataType == self.CDF_EPOCH16
-                                      or dataType == self.CDF_TIME_TT2000):
+                                elif dataType == self.CDF_EPOCH or dataType == self.CDF_EPOCH16 or dataType == self.CDF_TIME_TT2000:
                                     cvalue = []
-                                    if (isinstance(data, list) or
-                                            isinstance(data, tuple)):
+                                    if isinstance(data, list) or isinstance(data, tuple):
                                         numElems = len(data)
                                         for x in range(0, numElems):
-                                            if (isinstance(data[x], str)):
+                                            if isinstance(data[x], str):
                                                 cvalue.append(cdfepoch.CDFepoch.parse(data[x]))
                                             else:
                                                 cvalue.append(data[x])
                                         data = cvalue
                                     else:
-                                        if (isinstance(data, str)):
+                                        if isinstance(data, str):
                                             data = cdfepoch.CDFepoch.parse(data)
                                         numElems = 1
                                 else:
-                                    if (isinstance(data, list) or
-                                            isinstance(data, tuple)):
+                                    if isinstance(data, list) or isinstance(data, tuple):
                                         numElems = len(data)
                                     else:
                                         numElems = 1
                             else:
                                 # Data type not found, both values are data.
                                 data = value
                                 numElems, dataType = self._datatype_define(value[0])
@@ -431,21 +425,20 @@
                             data = value
                             numElems, dataType = self._datatype_define(value[0])
                             numElems = len(value)
                     else:
                         # Just one value
                         data = value
                         numElems, dataType = self._datatype_define(value)
-                        if (numElems is None):
-                            warnings.warn('Unknown data')
+                        if numElems is None:
+                            warnings.warn("Unknown data")
                             return
 
-                    offset = self._write_aedr(f, True, attrNum, entryNum, data,
-                                              dataType, numElems, None)
-                    if (entries == 0):
+                    offset = self._write_aedr(f, True, attrNum, entryNum, data, dataType, numElems, None)
+                    if entries == 0:
                         # ADR's AgrEDRhead
                         self._update_offset_value(f, offsetADR + 20, 8, offset)
                     else:
                         # ADR's ADRnext
                         self._update_offset_value(f, poffset + 12, 8, offset)
 
                     poffset = offset
@@ -481,131 +474,123 @@
                 ....
                 variableAttrs['attr_name_2']=entries_2
                 ....
                 ....
                 f.write_variableattrs(variableAttrs)
         """
         if not (isinstance(variableAttrs, dict)):
-            raise ValueError('Variable attribute(s) not in dictionary form')
+            raise ValueError("Variable attribute(s) not in dictionary form")
         dataType = None
         numElems = None
-        with self.path.open('rb+') as f:
+        with self.path.open("rb+") as f:
             f.seek(0, 2)  # EOF (appending)
             for attr, attrs in variableAttrs.items():
                 if not (isinstance(attr, str)):
-                    raise ValueError('Attribute name must be a string')
+                    raise ValueError("Attribute name must be a string")
                     return
-                if (attr in self.gattrs):
-                    raise ValueError(f'Variable attribute: {attr}' +
-                                     ' is already a global variable')
+                if attr in self.gattrs:
+                    raise ValueError(f"Variable attribute: {attr}" + " is already a global variable")
                     return
-                if (attr in self.vattrs):
+                if attr in self.vattrs:
                     attrNum = self.vattrs.index(attr)
                     offsetA = self.attrsinfo[attrNum][2]
                 else:
                     attrNum, offsetA = self._write_adr(f, False, attr)
                 entries = 0
-                if (attrs is None):
+                if attrs is None:
                     continue
                 if not (isinstance(attrs, dict)):
-                    raise ValueError('An attribute''s attribute(s) not in dictionary form')
+                    raise ValueError("An attribute" "s attribute(s) not in dictionary form")
                 entryNumX = -1
                 poffset = -1
                 for entryID, value in attrs.items():
-                    if (isinstance(entryID, str) and (not (entryID in self.zvars) and
-                                                      not (entryID in self.rvars))):
-                        raise KeyError(f'{entryID} not found in the CDF')
-
-                    if (isinstance(entryID, numbers.Number) and
-                            (len(self.zvars) > 0 and len(self.rvars) > 0)):
-                        raise ValueError(f'{entryID} can not be used as the CDF has both zVariables and rVariables')
+                    if isinstance(entryID, str) and (not (entryID in self.zvars) and not (entryID in self.rvars)):
+                        raise KeyError(f"{entryID} not found in the CDF")
+
+                    if isinstance(entryID, numbers.Number) and (len(self.zvars) > 0 and len(self.rvars) > 0):
+                        raise ValueError(f"{entryID} can not be used as the CDF has both zVariables and rVariables")
 
-                    if (isinstance(entryID, str)):
+                    if isinstance(entryID, str):
                         try:
                             entryNum = self.zvars.index(entryID)
                             zVar = True
                         except Exception:
                             try:
                                 entryNum = self.rvars.index(entryID)
                                 zVar = False
                             except Exception:
-                                raise KeyError(f'{entryID} not found')
+                                raise KeyError(f"{entryID} not found")
                     else:
                         entryNum = int(entryID)
-                        if (len(self.zvars) > 0 and len(self.rvars) > 0):
-                            raise ValueError('Can not use integer form for variable id as there ',
-                                             'are both zVariables and rVaribales')
-                        if (len(self.zvars) > 0):
-                            if (entryNum >= len(self.zvars)):
-                                raise ValueError('Variable id: ', entryID, ' not found')
+                        if len(self.zvars) > 0 and len(self.rvars) > 0:
+                            raise ValueError(
+                                "Can not use integer form for variable id as there ", "are both zVariables and rVaribales"
+                            )
+                        if len(self.zvars) > 0:
+                            if entryNum >= len(self.zvars):
+                                raise ValueError("Variable id: ", entryID, " not found")
                             else:
                                 zVar = True
                         else:
-                            if (entryNum >= len(self.rvars)):
-                                raise ValueError('Variable id: ', entryID, ' not found')
+                            if entryNum >= len(self.rvars):
+                                raise ValueError("Variable id: ", entryID, " not found")
                             else:
                                 zVar = False
-                    if (entryNum > entryNumX):
+                    if entryNum > entryNumX:
                         entryNumX = entryNum
-                    if hasattr(value, '__len__') and not isinstance(value, str):
-                        if (len(value) == 2):
+                    if hasattr(value, "__len__") and not isinstance(value, str):
+                        if len(value) == 2:
                             value2 = value[1]
                             dataType = self._datatype_token(value2)
-                            if (dataType > 0):
+                            if dataType > 0:
                                 data = value[0]
-                                if (dataType == self.CDF_CHAR or
-                                        dataType == self.CDF_UCHAR):
-                                    if (isinstance(data, list) or
-                                            isinstance(data, tuple)):
-                                        raise ValueError('Invalid variable attribute value')
+                                if dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR:
+                                    if isinstance(data, list) or isinstance(data, tuple):
+                                        raise ValueError("Invalid variable attribute value")
                                     numElems = len(data)
-                                elif (dataType == self.CDF_EPOCH or
-                                      dataType == self.CDF_EPOCH16
-                                      or dataType == self.CDF_TIME_TT2000):
+                                elif dataType == self.CDF_EPOCH or dataType == self.CDF_EPOCH16 or dataType == self.CDF_TIME_TT2000:
                                     cvalue = []
-                                    if (isinstance(data, list) or
-                                            isinstance(data, tuple)):
+                                    if isinstance(data, list) or isinstance(data, tuple):
                                         numElems = len(data)
                                         for x in range(0, numElems):
-                                            if (isinstance(data[x], str)):
+                                            if isinstance(data[x], str):
                                                 avalue = cdfepoch.CDFepoch.parse(data[x])
                                             else:
                                                 avalue = data[x]
-                                            if (dataType == self.CDF_EPOCH16):
+                                            if dataType == self.CDF_EPOCH16:
                                                 cvalue.append(avalue.real)
                                                 cvalue.append(avalue.imag)
                                             else:
                                                 cvalue.append(avalue)
                                                 data = cvalue
                                     else:
-                                        if (isinstance(data, str)):
+                                        if isinstance(data, str):
                                             data = cdfepoch.CDFepoch.parse(data)
                                         numElems = 1
                                 else:
-                                    if (isinstance(data, list) or isinstance(data, tuple)):
+                                    if isinstance(data, list) or isinstance(data, tuple):
                                         numElems = len(data)
                                     else:
                                         numElems = 1
                             else:
                                 data = value
                                 numElems, dataType = self._datatype_define(value[0])
                                 numElems = len(value)
                         else:
                             data = value
                             numElems, dataType = self._datatype_define(value[0])
                             numElems = len(value)
                     else:
                         data = value
                         numElems, dataType = self._datatype_define(value)
-                        if (numElems is None):
-                            warnings.warn('Unknown data')
+                        if numElems is None:
+                            warnings.warn("Unknown data")
                             return
-                    offset = self._write_aedr(f, False, attrNum, entryNum, data,
-                                              dataType, numElems, zVar)
-                    if (entries == 0):
+                    offset = self._write_aedr(f, False, attrNum, entryNum, data, dataType, numElems, zVar)
+                    if entries == 0:
                         if zVar:
                             # ADR's AzEDRhead
                             self._update_offset_value(f, offsetA + 48, 8, offset)
                         else:
                             # ADR's AgrEDRhead
                             self._update_offset_value(f, offsetA + 20, 8, offset)
                     else:
@@ -622,15 +607,15 @@
                     # ADR's NgrEntries
                     self._update_offset_value(f, offsetA + 36, 4, entries)
                     # ADR's MAXgrEntry
                     self._update_offset_value(f, offsetA + 40, 4, entryNumX)
 
     @is_open
     def write_var(self, var_spec, var_attrs=None, var_data=None):
-        '''
+        """
         Writes a variable, along with variable attributes and data.
 
         Parameters
         ----------
         var_spec : dict
             The specifications of the variable.
 
@@ -713,87 +698,86 @@
             The var_data has the form::
 
                 [[rec_#1,rec_#2,rec_#3,...],
                 [data_#1,data_#2,data_#3,...]]
 
             See the sample for its setup.
 
-        '''
+        """
         if not isinstance(var_spec, dict):
-            raise TypeError('Variable should be in dictionary form.')
+            raise TypeError("Variable should be in dictionary form.")
 
         # Get variable info from var_spec
         try:
-            dataType = int(var_spec['Data_Type'])
-            numElems = int(var_spec['Num_Elements'])
-            name = var_spec['Variable']
-            recVary = var_spec['Rec_Vary']
+            dataType = int(var_spec["Data_Type"])
+            numElems = int(var_spec["Num_Elements"])
+            name = var_spec["Variable"]
+            recVary = var_spec["Rec_Vary"]
         except Exception as e:
-            raise ValueError('Missing/invalid required spec for creating variable.') from e
+            raise ValueError("Missing/invalid required spec for creating variable.") from e
         # Get whether or not it is a z variable
-        var_type = var_spec.setdefault('Var_Type', 'zvariable')
-        if (var_type.lower() == 'zvariable'):
+        var_type = var_spec.setdefault("Var_Type", "zvariable")
+        if var_type.lower() == "zvariable":
             zVar = True
         else:
-            var_spec['Var_Type'] = 'rVariable'
+            var_spec["Var_Type"] = "rVariable"
             zVar = False
 
-        if (dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR):
+        if dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR:
             if numElems < 1:
-                raise ValueError('Invalid Num_Elements for string data type variable')
+                raise ValueError("Invalid Num_Elements for string data type variable")
         else:
             if numElems != 1:
-                raise ValueError('Invalid Num_Elements for numeric data type variable')
+                raise ValueError("Invalid Num_Elements for numeric data type variable")
         # If its a z variable, get the dimension info
         # Otherwise, use r variable info
         if zVar:
             try:
-                dimSizes = var_spec['Dim_Sizes']
+                dimSizes = var_spec["Dim_Sizes"]
                 numDims = len(dimSizes)
                 dimVary = []
                 for _ in range(0, numDims):
                     dimVary.append(True)
             except Exception:
-                raise ValueError('Missing/invalid required spec for creating variable.')
+                raise ValueError("Missing/invalid required spec for creating variable.")
         else:
             dimSizes = self.rdim_sizes
             numDims = self.num_rdim
             try:
-                dimVary = var_spec['Dim_Vary']
-                if (len(dimVary) != numDims):
-                    raise ValueError('Invalid Dim_Vary size for the rVariable.')
+                dimVary = var_spec["Dim_Vary"]
+                if len(dimVary) != numDims:
+                    raise ValueError("Invalid Dim_Vary size for the rVariable.")
             except Exception:
-                raise ValueError('Missing/invalid required spec for Dim_Vary for rVariable')
+                raise ValueError("Missing/invalid required spec for Dim_Vary for rVariable")
         # Get Sparseness info
-        sparse = self._sparse_token(var_spec.get('Sparse', 'no_sparse'))
+        sparse = self._sparse_token(var_spec.get("Sparse", "no_sparse"))
         # Get compression info
-        compression = var_spec.get('Compress', 6)
-        if (isinstance(compression, int)):
+        compression = var_spec.get("Compress", 6)
+        if isinstance(compression, int):
             if not 0 <= compression <= 9:
                 compression = 0
         else:
             compression = 6 if compression else 0
 
         # Get blocking factor
-        blockingfactor = int(var_spec.get('Block_Factor', 1))
+        blockingfactor = int(var_spec.get("Block_Factor", 1))
 
         # Get pad value
-        pad = var_spec.get('Pad', None)
-        if hasattr(pad, '__len__'):
+        pad = var_spec.get("Pad", None)
+        if hasattr(pad, "__len__"):
             pad = pad[0]
 
-        if (name in self.zvars or name in self.rvars):
-            raise ValueError(f'{name} already exists')
+        if name in self.zvars or name in self.rvars:
+            raise ValueError(f"{name} already exists")
 
-        with self.path.open('rb+') as f:
+        with self.path.open("rb+") as f:
             f.seek(0, 2)  # EOF (appending)
-            varNum, offset = self._write_vdr(f, dataType, numElems, numDims,
-                                             dimSizes, name, dimVary, recVary,
-                                             sparse, blockingfactor, compression,
-                                             pad, zVar)
+            varNum, offset = self._write_vdr(
+                f, dataType, numElems, numDims, dimSizes, name, dimVary, recVary, sparse, blockingfactor, compression, pad, zVar
+            )
             # Update the GDR pointers if needed
             if zVar:
                 if len(self.zvars) == 1:
                     # GDR's zVDRhead
                     self._update_offset_value(f, self.gdr_head + 20, 8, offset)
             else:
                 if len(self.rvars) == 1:
@@ -802,198 +786,204 @@
 
             # Write the variable attributes
             if var_attrs is not None:
                 self._write_var_attrs(f, varNum, var_attrs, zVar)
 
             # Write the actual data to the file
             if not (var_data is None):
-                if (sparse == 0):
-                    varMaxRec = self._write_var_data_nonsparse(f, zVar, varNum,
-                                                               dataType, numElems,
-                                                               recVary, compression,
-                                                               blockingfactor,
-                                                               var_data)
+                if sparse == 0:
+                    varMaxRec = self._write_var_data_nonsparse(
+                        f, zVar, varNum, dataType, numElems, recVary, compression, blockingfactor, var_data
+                    )
                 else:
                     notsupport = False
                     if not isinstance(var_data, (list, tuple)):
                         notsupport = True
 
                     if notsupport or len(var_data) != 2:
-                        print('Sparse record #s and data are not of list/tuple form:')
-                        print(' [ [rec_#1, rec_#2, rec_#3,    ],')
-                        print('   [data_#1, data_#2, data_#3, ....] ]')
+                        print("Sparse record #s and data are not of list/tuple form:")
+                        print(" [ [rec_#1, rec_#2, rec_#3,    ],")
+                        print("   [data_#1, data_#2, data_#3, ....] ]")
                         return
 
                     # Format data into: [[recstart1, recend1, data1],
                     #                   [recstart2,recend2,data2], ...]
-                    var_data = self._make_sparse_blocks(var_spec, var_data[0],
-                                                        var_data[1])
+                    var_data = self._make_sparse_blocks(var_spec, var_data[0], var_data[1])
 
                     for block in var_data:
-                        varMaxRec = self._write_var_data_sparse(f, zVar, varNum,
-                                                                dataType, numElems,
-                                                                recVary, block)
+                        varMaxRec = self._write_var_data_sparse(f, zVar, varNum, dataType, numElems, recVary, block)
                 # Update GDR MaxRec if writing an r variable
                 if not zVar:
                     # GDR's rMaxRec
                     f.seek(self.gdr_head + 52)
-                    maxRec = int.from_bytes(f.read(4), 'big', signed=True)
-                    if (maxRec < varMaxRec):
+                    maxRec = int.from_bytes(f.read(4), "big", signed=True)
+                    if maxRec < varMaxRec:
                         self._update_offset_value(f, self.gdr_head + 52, 4, varMaxRec)
 
-    def _write_var_attrs(self, f, varNum, var_attrs, zVar):
-        '''
+    def _write_var_attrs(self, f: io.BufferedWriter, varNum: int, var_attrs: Dict[str, Any], zVar: bool) -> None:
+        """
         Writes ADRs and AEDRs for variables
 
         Parameters:
             f : file
                 The open CDF file
             varNum : int
                 The variable number for adding attributes
             var_attrs : dict
                 A dictionary object full of variable attributes
             zVar : bool
                 True if varNum is referencing a z variable
 
         Returns: None
-        '''
+        """
 
-        if (not isinstance(var_attrs, dict)):
-            raise TypeError('Variable attribute(s) should be in dictionary form.')
+        if not isinstance(var_attrs, dict):
+            raise TypeError("Variable attribute(s) should be in dictionary form.")
 
         for attr, entry in var_attrs.items():
-            if (attr in self.gattrs):
-                warnings.warn(f'Attribute: {attr}' + ' already defined as a global attribute... Skip')
+            if attr in self.gattrs:
+                warnings.warn(f"Attribute: {attr}" + " already defined as a global attribute... Skip")
                 continue
 
             if not (attr in self.attrs):
                 attrNum, offset = self._write_adr(f, False, attr)
-                if (len(self.attrs) == 0):
+                if len(self.attrs) == 0:
                     # GDR's ADRhead
-                    self._update_offset_value(self.grd_offset + 28, 8, offset)
+                    # TODO: fix this, grid_offset doesn't exsit
+                    self._update_offset_value(f, self.grid_offset + 28, 8, offset)  # type: ignore
             else:
                 attrNum = self.attrs.index(attr)
                 offset = self.attrsinfo[attrNum][2]
 
-            if (entry is None):
+            if entry is None:
                 continue
 
             # Check if dataType was provided
             dataType = 0
-            if hasattr(entry, '__len__') and not isinstance(entry, str):
+            if hasattr(entry, "__len__") and not isinstance(entry, str):
                 items = len(entry)
-                if (items == 2):
+                if items == 2:
                     dataType = self._datatype_token(entry[1])
 
-            if (dataType > 0):
+            if dataType > 0:
                 # CDF data type defined in entry
                 data = entry[0]
-                if (self._checklistofNums(data)):
+                if self._checklistofNums(data):
                     # All are numbers
-                    if hasattr(data, '__len__') and not isinstance(data, str):
+                    if hasattr(data, "__len__") and not isinstance(data, str):
                         numElems = len(data)
                     else:
                         numElems = 1
                 else:
                     # Then string(s) -- either in CDF_type or epoch in string(s)
-                    if (dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR):
-                        if hasattr(data, '__len__') and not isinstance(data, str):
+                    if dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR:
+                        if hasattr(data, "__len__") and not isinstance(data, str):
                             items = len(data)
                             odata = data
-                            data = ''
+                            data = ""
                             for x in range(0, items):
-                                if (x > 0):
-                                    data += '\\N '
+                                if x > 0:
+                                    data += "\\N "
                                     data += odata[x]
                                 else:
                                     data = odata[x]
                         numElems = len(data)
-                    elif (dataType == self.CDF_EPOCH or dataType == self.CDF_EPOCH16
-                          or dataType == self.CDF_TIME_TT2000):
+                    elif dataType == self.CDF_EPOCH or dataType == self.CDF_EPOCH16 or dataType == self.CDF_TIME_TT2000:
                         cvalue = []
-                        if hasattr(data, '__len__') and not isinstance(data, str):
+                        if hasattr(data, "__len__") and not isinstance(data, str):
                             numElems = len(data)
                             for x in range(0, numElems):
                                 cvalue.append(cdfepoch.CDFepoch.parse(data[x]))
                             data = cvalue
                         else:
                             data = cdfepoch.CDFepoch.parse(data)
                             numElems = 1
             else:
                 # No data type defined...
                 data = entry
-                if hasattr(data, '__len__') and not isinstance(data, str):
+                if hasattr(data, "__len__") and not isinstance(data, str):
                     numElems, dataType = self._datatype_define(entry[0])
-                    if (dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR):
-                        data = ''
+                    if dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR:
+                        data = ""
                         for x in range(0, len(entry)):
-                            if (x > 0):
-                                data += '\\N '
+                            if x > 0:
+                                data += "\\N "
                                 data += entry[x]
                             else:
                                 data = entry[x]
                     numElems = len(data)
                 else:
                     numElems, dataType = self._datatype_define(entry)
 
             offset = self._write_aedr(f, False, attrNum, varNum, data, dataType, numElems, zVar)
 
             self._update_aedr_link(f, attrNum, zVar, varNum, offset)
 
-    def _write_var_data_nonsparse(self, f, zVar: bool, var, dataType, numElems,
-                                  recVary, compression, blockingfactor, indata) -> int:
-        '''
+    def _write_var_data_nonsparse(
+        self,
+        f: io.BufferedWriter,
+        zVar: bool,
+        var: int,
+        dataType: int,
+        numElems: int,
+        recVary: bool,
+        compression: int,
+        blockingfactor: int,
+        indata: Union[np.ndarray, bytearray, Dict[str, np.ndarray]],
+    ) -> int:
+        """
         Creates VVRs and the corresponding VXRs full of "indata" data.
         If there is no compression, creates exactly one VXR and VVR
         If there is compression
 
-        Parameters:
-            f : file
-                The open CDF file
-            zVar : bool
-                True if this is z variable data
-            var : str
-                The name of the variable
-            dataType : int
-                the CDF variable type
-            numElems : int
-                number of elements in each record
-            recVary : bool
-                True if each record is unque
-            compression : int
-                The amount of compression
-            blockingfactor: int
-                The size (in number of records) of a VVR data block
-            indata : varies
-                the data to write, should be a numpy or byte array
-
-        Returns:
-            recs : int
-                The number of records
-
-        '''
+        Parameters
+        ----------
+        f : file
+            The open CDF file
+        zVar : bool
+            True if this is z variable data
+        var : str
+            The name of the variable
+        dataType : int
+            the CDF variable type
+        numElems : int
+            number of elements in each record
+        recVary : bool
+            True if each record is unque
+        compression : int
+            The amount of compression
+        blockingfactor: int
+            The size (in number of records) of a VVR data block
+        indata : varies
+            the data to write, should be a numpy or byte array
+
+        Returns
+        -------
+        recs : int
+            The number of records
+        """
 
         numValues = self._num_values(zVar, var)
         dataTypeSize = self._datatype_size(dataType, numElems)
-        if (isinstance(indata, dict)):
-            indata = indata['Data']
+        if isinstance(indata, dict):
+            indata = indata["Data"]
 
         # Deal with EPOCH16 data types
-        if (dataType == self.CDF_EPOCH16):
+        if dataType == self.CDF_EPOCH16:
             epoch16 = []
-            if hasattr(indata, '__len__') and not isinstance(indata, str):
+            if hasattr(indata, "__len__") and not isinstance(indata, str):
                 adata = indata[0]
-                if (isinstance(adata, complex)):
+                if isinstance(adata, complex):
                     recs = len(indata)
                     for x in range(0, recs):
                         epoch16.append(indata[x].real)
                         epoch16.append(indata[x].imag)
-                    indata = epoch16
+                    indata = np.array(epoch16)
             else:
-                if (isinstance(indata, complex)):
+                if isinstance(indata, complex):
                     epoch16.append(indata.real)
                     epoch16.append(indata.imag)
                     indata = epoch16
 
         # Convert to byte stream
         recs, data = self._convert_data(dataType, numElems, numValues, indata)
 
@@ -1006,117 +996,121 @@
 
         usedEntries = 0
         numVXRs = 0
         if compression > 0:
             default_blockingfactor = math.ceil(self.BLOCKING_BYTES / (numValues * dataTypeSize))
             # If the given blocking factor is too small, use the default one
             # Will re-adjust if the records are less than this computed BF.
-            if (blockingfactor < default_blockingfactor):
+            if blockingfactor < default_blockingfactor:
                 blockingfactor = default_blockingfactor
-            if (blockingfactor == 0):
+            if blockingfactor == 0:
                 blockingfactor = 1
 
             # Update the blocking factor
             f.seek(vdr_offset + 80, 0)
             # VDR's BlockingFactor
-            self._update_offset_value(f, vdr_offset + 80, 4,
-                                      blockingfactor)
+            self._update_offset_value(f, vdr_offset + 80, 4, blockingfactor)
 
             # set blocking factor
-            if (recs < blockingfactor):
+            if recs < blockingfactor:
                 blockingfactor = recs
             blocks = math.ceil(recs / blockingfactor)
             nEntries = self.NUM_VXR_ENTRIES
             VXRhead = None
 
             # Loop through blocks, create VVRs/CVVRs
             for x in range(0, blocks):
                 startrec = x * blockingfactor
                 startloc = startrec * numValues * dataTypeSize
                 endrec = (x + 1) * blockingfactor - 1
-                if (endrec > (recs - 1)):
+                if endrec > (recs - 1):
                     endrec = recs - 1
                 endloc = (endrec + 1) * numValues * dataTypeSize
-                if (endloc > len(data)):
+                if endloc > len(data):
                     endrec = recs - 1
                     endloc = len(data)
                 bdata = data[startloc:endloc]
                 cdata = gzip.compress(bdata, compression)
-                if (len(cdata) < len(bdata)):
+                if len(cdata) < len(bdata):
                     n1offset = self._write_cvvr(f, cdata)
                 else:
                     n1offset = self._write_vvr(f, bdata)
-                if (x == 0):
+                if x == 0:
                     # Create a VXR
                     VXRoffset = self._write_vxr(f)
                     VXRhead = VXRoffset
                     numVXRs = 1
                     self._update_vdr_vxrheadtail(f, vdr_offset, VXRoffset)
-                if (usedEntries < nEntries):
+                if usedEntries < nEntries:
                     # Use the exisitng VXR
-                    usedEntries = self._use_vxrentry(f, VXRoffset, startrec,
-                                                     endrec, n1offset)
+                    usedEntries = self._use_vxrentry(f, VXRoffset, startrec, endrec, n1offset)
                 else:
                     # Create a new VXR and an upper level VXR, if needed.
                     # Two levels of VXRs are the maximum, which is simpler
                     # to implement.
                     savedVXRoffset = VXRoffset
                     VXRoffset = self._write_vxr(f)
                     numVXRs += 1
-                    usedEntries = self._use_vxrentry(f, VXRoffset, startrec,
-                                                     endrec, n1offset)
+                    usedEntries = self._use_vxrentry(f, VXRoffset, startrec, endrec, n1offset)
                     # Edit the VXRnext field of the previous VXR
                     self._update_offset_value(f, savedVXRoffset + 12, 8, VXRoffset)
                     # Edit the VXRtail of the VDR
                     self._update_offset_value(f, vdr_offset + 36, 8, VXRoffset)
 
             # After we're done with the blocks, check the way
             # we have VXRs set up
-            if (numVXRs > self.NUM_VXRlvl_ENTRIES):
-                newvxrhead, newvxrtail = self._add_vxr_levels_r(f, VXRhead,
-                                                                numVXRs)
+            if numVXRs > self.NUM_VXRlvl_ENTRIES:
+                newvxrhead, newvxrtail = self._add_vxr_levels_r(f, VXRhead, numVXRs)
                 self._update_offset_value(f, vdr_offset + 28, 8, newvxrhead)
                 self._update_offset_value(f, vdr_offset + 36, 8, newvxrtail)
         else:
             # Create one VVR and VXR, with one VXR entry
             offset = self._write_vvr(f, data)
             VXRoffset = self._write_vxr(f)
             usedEntries = self._use_vxrentry(f, VXRoffset, 0, recs - 1, offset)
             self._update_vdr_vxrheadtail(f, vdr_offset, VXRoffset)
 
         # VDR's MaxRec
         self._update_offset_value(f, vdr_offset + 24, 4, recs - 1)
 
-        return (recs - 1)
+        return recs - 1
 
-    def _write_var_data_sparse(self, f, zVar: bool, var, dataType, numElems, recVary,
-                               oneblock):
-        '''
+    def _write_var_data_sparse(
+        self,
+        f: io.BufferedWriter,
+        zVar: bool,
+        var: int,
+        dataType: int,
+        numElems: int,
+        recVary: bool,
+        oneblock: Tuple[int, int, np.ndarray],
+    ) -> int:
+        """
         Writes a VVR and a VXR for this block of sparse data
 
         Parameters:
             f : file
                 The open CDF file
             zVar : bool
                 True if this is for a z variable
             var : int
                 The variable number
             dataType : int
                 The CDF data type of this variable
-            numElems : str
+            numElems : int
                 The number of elements in each record
             recVary : bool
                 True if the value varies across records
             oneblock: list
                 A list of data in the form [startrec, endrec, [data]]
 
         Returns:
             recend : int
                 Just the "endrec" value input by the user in "oneblock"
-        '''
+        """
 
         rec_start = oneblock[0]
         rec_end = oneblock[1]
         indata = oneblock[2]
         numValues = self._num_values(zVar, var)
 
         # Convert oneblock[2] into a byte stream
@@ -1129,53 +1123,52 @@
             vdr_offset = self.rvarsinfo[var][1]
 
         # Write one VVR
         offset = self._write_vvr(f, data)
         f.seek(vdr_offset + 28, 0)
 
         # Get first VXR
-        vxrOne = int.from_bytes(f.read(8), 'big', signed=True)
+        vxrOne = int.from_bytes(f.read(8), "big", signed=True)
         foundSpot = 0
         usedEntries = 0
         currentVXR = 0
 
         # Search through VXRs to find an open one
         while foundSpot == 0 and vxrOne > 0:
             # have a VXR
             f.seek(vxrOne, 0)
             currentVXR = f.tell()
             f.seek(vxrOne + 12, 0)
-            vxrNext = int.from_bytes(f.read(8), 'big', signed=True)
-            nEntries = int.from_bytes(f.read(4), 'big', signed=True)
-            usedEntries = int.from_bytes(f.read(4), 'big', signed=True)
-            if (usedEntries == nEntries):
+            vxrNext = int.from_bytes(f.read(8), "big", signed=True)
+            nEntries = int.from_bytes(f.read(4), "big", signed=True)
+            usedEntries = int.from_bytes(f.read(4), "big", signed=True)
+            if usedEntries == nEntries:
                 # all entries are used -- check the next vxr in link
                 vxrOne = vxrNext
             else:
                 # found a vxr with an vailable entry spot
                 foundSpot = 1
 
         # vxrOne == 0 from vdr's vxrhead vxrOne == -1 from a vxr's vxrnext
-        if (vxrOne == 0 or vxrOne == -1):
+        if vxrOne == 0 or vxrOne == -1:
             # no available vxr... create a new one
-            currentVXR = self._create_vxr(f, rec_start, rec_end, vdr_offset,
-                                          currentVXR, offset)
+            currentVXR = self._create_vxr(f, rec_start, rec_end, vdr_offset, currentVXR, offset)
         else:
             self._use_vxrentry(f, currentVXR, rec_start, rec_end, offset)
 
         # Modify the VDR's MaxRec if needed
         f.seek(vdr_offset + 24, 0)
-        recNumc = int.from_bytes(f.read(4), 'big', signed=True)
-        if (rec_end > recNumc):
+        recNumc = int.from_bytes(f.read(4), "big", signed=True)
+        if rec_end > recNumc:
             self._update_offset_value(f, vdr_offset + 24, 4, rec_end)
 
         return rec_end
 
-    def _create_vxr(self, f, recStart, recEnd, currentVDR, priorVXR, vvrOffset):
-        '''
+    def _create_vxr(self, f: io.BufferedWriter, recStart: int, recEnd: int, currentVDR: int, priorVXR: int, vvrOffset: int) -> int:
+        """
         Create a VXR AND use a VXR
 
         Parameters:
             f : file
                 The open CDF file
             recStart : int
                 The start record of this block
@@ -1188,98 +1181,97 @@
             vvrOffset : int
                 The byte location of ther VVR
 
         Returns:
             vxroffset : int
                 The byte location of the created vxr
 
-        '''
+        """
         # add a VXR, use an entry, and link it to the prior VXR if it exists
         vxroffset = self._write_vxr(f)
         self._use_vxrentry(f, vxroffset, recStart, recEnd, vvrOffset)
-        if (priorVXR == 0):
+        if priorVXR == 0:
             # VDR's VXRhead
             self._update_offset_value(f, currentVDR + 28, 8, vxroffset)
         else:
             # VXR's next
             self._update_offset_value(f, priorVXR + 12, 8, vxroffset)
         # VDR's VXRtail
         self._update_offset_value(f, currentVDR + 36, 8, vxroffset)
         return vxroffset
 
-    def _use_vxrentry(self, f, VXRoffset, recStart, recEnd, offset):
-        '''
+    def _use_vxrentry(self, f: io.BufferedWriter, VXRoffset: int, recStart: int, recEnd: int, offset: int) -> int:
+        """
         Adds a VVR pointer to a VXR
-        '''
+        """
         # Select the next unused entry in a VXR for a VVR/CVVR
         f.seek(VXRoffset + 20)
         # num entries
-        numEntries = int.from_bytes(f.read(4), 'big', signed=True)
+        numEntries = int.from_bytes(f.read(4), "big", signed=True)
         # used entries
-        usedEntries = int.from_bytes(f.read(4), 'big', signed=True)
+        usedEntries = int.from_bytes(f.read(4), "big", signed=True)
         # VXR's First
         self._update_offset_value(f, VXRoffset + 28 + 4 * usedEntries, 4, recStart)
         # VXR's Last
-        self._update_offset_value(f, VXRoffset + 28 + 4 * numEntries + 4 * usedEntries,
-                                  4, recEnd)
+        self._update_offset_value(f, VXRoffset + 28 + 4 * numEntries + 4 * usedEntries, 4, recEnd)
         # VXR's Offset
-        self._update_offset_value(f, VXRoffset + 28 + 2 * 4 * numEntries + 8 * usedEntries,
-                                  8, offset)
+        self._update_offset_value(f, VXRoffset + 28 + 2 * 4 * numEntries + 8 * usedEntries, 8, offset)
         # VXR's NusedEntries
         usedEntries += 1
         self._update_offset_value(f, VXRoffset + 24, 4, usedEntries)
         return usedEntries
 
-    def _add_vxr_levels_r(self, f, vxrhead, numVXRs):
-        '''
+    def _add_vxr_levels_r(self, f: io.BufferedWriter, vxrhead: int, numVXRs: int) -> Tuple[int, int]:
+        """
         Build a new level of VXRs... make VXRs more tree-like
 
         From:
 
         VXR1 -> VXR2 -> VXR3 -> VXR4 -> ... -> VXRn
 
         To:
                            new VXR1
                          /    |    \
                         VXR2 VXR3 VXR4
                        /      |      \
                              ...
                     VXR5  ..........  VXRn
 
-        Parameters:
-            f : file
-                The open CDF file
-            vxrhead : int
-                The byte location of the first VXR for a variable
-            numVXRs : int
-                The total number of VXRs
-
-        Returns:
-            newVXRhead : int
-                The byte location of the newest VXR head
-            newvxroff : int
-                The byte location of the last VXR head
-
-        '''
+        Parameters
+        ----------
+        f : file
+            The open CDF file
+        vxrhead : int
+            The byte location of the first VXR for a variable
+        numVXRs : int
+            The total number of VXRs
+
+        Returns
+        -------
+        newVXRhead : int
+            The byte location of the newest VXR head
+        newvxroff : int
+            The byte location of the last VXR head
+        """
         newNumVXRs = int(numVXRs / self.NUM_VXRlvl_ENTRIES)
         remaining = int(numVXRs % self.NUM_VXRlvl_ENTRIES)
         vxroff = vxrhead
         prevxroff = -1
-        if (remaining != 0):
+        if remaining != 0:
             newNumVXRs += 1
         self.level += 1
         for x in range(0, newNumVXRs):
             newvxroff = self._write_vxr(f, numEntries=self.NUM_VXRlvl_ENTRIES)
-            if (x > 0):
+            if x > 0:
                 self._update_offset_value(f, prevxroff + 12, 8, newvxroff)
             else:
                 newvxrhead = newvxroff
             prevxroff = newvxroff
-            if (x == (newNumVXRs - 1)):
-                if (remaining == 0):
+            if x == (newNumVXRs - 1):
+                if remaining == 0:
                     endEntry = self.NUM_VXRlvl_ENTRIES
                 else:
                     endEntry = remaining
             else:
                 endEntry = self.NUM_VXRlvl_ENTRIES
             for _ in range(0, endEntry):
                 recFirst, recLast = self._get_recrange(f, vxroff)
@@ -1290,266 +1282,251 @@
         # Break the horizontal links
         for x in range(0, numVXRs):
             nvxroff = self._read_offset_value(f, vxroff + 12, 8)
             self._update_offset_value(f, vxroff + 12, 8, 0)
             vxroff = nvxroff
 
         # Iterate this process if we're over NUM_VXRlvl_ENTRIES
-        if (newNumVXRs > self.NUM_VXRlvl_ENTRIES):
+        if newNumVXRs > self.NUM_VXRlvl_ENTRIES:
             return self._add_vxr_levels_r(f, newvxrhead, newNumVXRs)
         else:
             return newvxrhead, newvxroff
 
-    def _update_vdr_vxrheadtail(self, f, vdr_offset, VXRoffset):
-        '''
+    def _update_vdr_vxrheadtail(self, f: io.BufferedWriter, vdr_offset: int, VXRoffset: int) -> None:
+        """
         This sets a VXR to be the first and last VXR in the VDR
-        '''
+        """
         # VDR's VXRhead
         self._update_offset_value(f, vdr_offset + 28, 8, VXRoffset)
         # VDR's VXRtail
         self._update_offset_value(f, vdr_offset + 36, 8, VXRoffset)
 
-    def _get_recrange(self, f, VXRoffset):
-        '''
+    def _get_recrange(self, f: io.BufferedWriter, VXRoffset: int) -> Tuple[int, int]:
+        """
         Finds the first and last record numbers pointed by the VXR
         Assumes the VXRs are in order
-        '''
+        """
         f.seek(VXRoffset + 20)
         # Num entries
-        numEntries = int.from_bytes(f.read(4), 'big', signed=True)
+        numEntries = int.from_bytes(f.read(4), "big", signed=True)
         # used entries
-        usedEntries = int.from_bytes(f.read(4), 'big', signed=True)
+        usedEntries = int.from_bytes(f.read(4), "big", signed=True)
         # VXR's First record
-        firstRec = int.from_bytes(f.read(4), 'big', signed=True)
+        firstRec = int.from_bytes(f.read(4), "big", signed=True)
         # VXR's Last record
         f.seek(VXRoffset + 28 + (4 * numEntries + 4 * (usedEntries - 1)))
-        lastRec = int.from_bytes(f.read(4), 'big', signed=True)
+        lastRec = int.from_bytes(f.read(4), "big", signed=True)
         return firstRec, lastRec
 
     @staticmethod
-    def _majority_token(major):
-        '''
+    def _majority_token(major: str) -> int:
+        """
         Returns the numberical type for a CDF row/column major type
-        '''
-        majors = {'ROW_MAJOR': 1,
-                  'COLUMN_MAJOR': 2}
+        """
+        majors = {"ROW_MAJOR": 1, "COLUMN_MAJOR": 2}
         try:
             return majors[major.upper()]
         except Exception:
-            warnings.warn(f'bad major.... {major}')
+            warnings.warn(f"bad major.... {major}")
             return 0
 
     @staticmethod
-    def _encoding_token(encoding):
-        '''
+    def _encoding_token(encoding: str) -> int:
+        """
         Returns the numberical type for a CDF encoding type
-        '''
-        encodings = {'NETWORK_ENCODING': 1,
-                     'SUN_ENCODING': 2,
-                     'VAX_ENCODING': 3,
-                     'DECSTATION_ENCODING': 4,
-                     'SGI_ENCODING': 5,
-                     'IBMPC_ENCODING': 6,
-                     'IBMRS_ENCODING': 7,
-                     'HOST_ENCODING': 8,
-                     'PPC_ENCODING': 9,
-                     'HP_ENCODING': 11,
-                     'NEXT_ENCODING': 12,
-                     'ALPHAOSF1_ENCODING': 13,
-                     'ALPHAVMSD_ENCODING': 14,
-                     'ALPHAVMSG_ENCODING': 15,
-                     'ALPHAVMSI_ENCODING': 16,
-                     'ARM_LITTLE_ENCODING': 17,
-                     'ARM_BIG_ENCODING': 18}
+        """
+        encodings = {
+            "NETWORK_ENCODING": 1,
+            "SUN_ENCODING": 2,
+            "VAX_ENCODING": 3,
+            "DECSTATION_ENCODING": 4,
+            "SGI_ENCODING": 5,
+            "IBMPC_ENCODING": 6,
+            "IBMRS_ENCODING": 7,
+            "HOST_ENCODING": 8,
+            "PPC_ENCODING": 9,
+            "HP_ENCODING": 11,
+            "NEXT_ENCODING": 12,
+            "ALPHAOSF1_ENCODING": 13,
+            "ALPHAVMSD_ENCODING": 14,
+            "ALPHAVMSG_ENCODING": 15,
+            "ALPHAVMSI_ENCODING": 16,
+            "ARM_LITTLE_ENCODING": 17,
+            "ARM_BIG_ENCODING": 18,
+        }
         try:
             return encodings[encoding.upper()]
         except Exception:
-            warnings.warn(f'bad encoding.... {encoding}')
+            warnings.warn(f"bad encoding.... {encoding}")
             return 0
 
     @staticmethod
-    def _datatype_token(datatype):
-        '''
+    def _datatype_token(datatype: str) -> int:
+        """
         Returns the numberical type for a CDF data type
-        '''
-        datatypes = {'CDF_INT1': 1,
-                     'CDF_INT2': 2,
-                     'CDF_INT4': 4,
-                     'CDF_INT8': 8,
-                     'CDF_UINT1': 11,
-                     'CDF_UINT2': 12,
-                     'CDF_UINT4': 14,
-                     'CDF_REAL4': 21,
-                     'CDF_REAL8': 22,
-                     'CDF_EPOCH': 31,
-                     'CDF_EPOCH16': 32,
-                     'CDF_TIME_TT2000': 33,
-                     'CDF_BYTE': 41,
-                     'CDF_FLOAT': 44,
-                     'CDF_DOUBLE': 45,
-                     'CDF_CHAR': 51,
-                     'CDF_UCHAR': 52}
+        """
+        datatypes = {
+            "CDF_INT1": 1,
+            "CDF_INT2": 2,
+            "CDF_INT4": 4,
+            "CDF_INT8": 8,
+            "CDF_UINT1": 11,
+            "CDF_UINT2": 12,
+            "CDF_UINT4": 14,
+            "CDF_REAL4": 21,
+            "CDF_REAL8": 22,
+            "CDF_EPOCH": 31,
+            "CDF_EPOCH16": 32,
+            "CDF_TIME_TT2000": 33,
+            "CDF_BYTE": 41,
+            "CDF_FLOAT": 44,
+            "CDF_DOUBLE": 45,
+            "CDF_CHAR": 51,
+            "CDF_UCHAR": 52,
+        }
         try:
             return datatypes[datatype.upper()]
         except Exception:
             return 0
 
-    def _datatype_define(self, value):
-        if (isinstance(value, str)):
+    def _datatype_define(self, value: Union[str, int, float, complex, np.ndarray]) -> Tuple[int, int]:
+        if isinstance(value, str):
             return len(value), self.CDF_CHAR
         else:
             numElems = 1
-            if (isinstance(value, int)):
+            if isinstance(value, int):
                 return numElems, self.CDF_INT8
-            elif (isinstance(value, float)):
+            elif isinstance(value, float):
                 return numElems, self.CDF_DOUBLE
-            elif (isinstance(value, complex)):
+            elif isinstance(value, complex):
                 return numElems, self.CDF_EPOCH16
-            elif (hasattr(value, 'dtype')):
+            elif hasattr(value, "dtype"):
                 # We are likely dealing with a numpy number at this point
                 if value.dtype.type in (np.int8, np.int16, np.int32, np.int64):
                     return numElems, self.CDF_INT8
                 elif value.dtype.type == np.complex128:
                     return numElems, self.CDF_EPOCH16
                 elif value.dtype.type in (np.uint8, np.uint16, np.uint32, np.uint64):
                     return numElems, self.CDF_UINT4
                 elif value.dtype.type in (np.float16, np.float32, np.float64):
                     return numElems, self.CDF_DOUBLE
                 elif value.dtype.type == np.str_:
                     return numElems, self.CDF_CHAR
                 else:
-                    warnings.warn('Invalid data type for data.... Skip')
+                    warnings.warn("Invalid data type for data.... Skip")
                     return None, None
             else:
-                warnings.warn('Invalid data type for data.... Skip')
+                warnings.warn("Invalid data type for data.... Skip")
                 return None, None
 
     @staticmethod
-    def _datatype_size(datatype, numElms):
-        '''
+    def _datatype_size(datatype: int, numElms: int) -> int:
+        """
         Gets datatype size
 
         Parameters:
             datatype : int
                 CDF variable data type
             numElms : int
                 number of elements
 
         Returns:
             numBytes : int
                 The number of bytes for the data
-        '''
-        sizes = {1: 1,
-                 2: 2,
-                 4: 4,
-                 8: 8,
-                 11: 1,
-                 12: 2,
-                 14: 4,
-                 21: 4,
-                 22: 8,
-                 31: 8,
-                 32: 16,
-                 33: 8,
-                 41: 1,
-                 44: 4,
-                 45: 8,
-                 51: 1,
-                 52: 1}
+        """
+        sizes = {1: 1, 2: 2, 4: 4, 8: 8, 11: 1, 12: 2, 14: 4, 21: 4, 22: 8, 31: 8, 32: 16, 33: 8, 41: 1, 44: 4, 45: 8, 51: 1, 52: 1}
         try:
-            if (isinstance(datatype, int)):
-                if (datatype == 51 or datatype == 52):
+            if isinstance(datatype, int):
+                if datatype == 51 or datatype == 52:
                     return numElms
                 else:
                     return sizes[datatype] * numElms
             else:
                 datatype = datatype.upper()
-                if (datatype == 'CDF_INT1' or datatype == 'CDF_UINT1' or
-                        datatype == 'CDF_BYTE'):
+                if datatype == "CDF_INT1" or datatype == "CDF_UINT1" or datatype == "CDF_BYTE":
                     return 1 * numElms
-                elif (datatype == 'CDF_INT2' or datatype == 'CDF_UINT2'):
+                elif datatype == "CDF_INT2" or datatype == "CDF_UINT2":
                     return 2 * numElms
-                elif (datatype == 'CDF_INT4' or datatype == 'CDF_UINT4'):
+                elif datatype == "CDF_INT4" or datatype == "CDF_UINT4":
                     return 4 * numElms
-                elif (datatype == 'CDF_INT8' or datatype == 'CDF_TIME_TT2000'):
+                elif datatype == "CDF_INT8" or datatype == "CDF_TIME_TT2000":
                     return 8 * numElms
-                elif (datatype == 'CDF_REAL4' or datatype == 'CDF_FLOAT'):
+                elif datatype == "CDF_REAL4" or datatype == "CDF_FLOAT":
                     return 4 * numElms
-                elif (datatype == 'CDF_REAL8' or datatype == 'CDF_DOUBLE' or
-                      datatype == 'CDF_EPOCH'):
+                elif datatype == "CDF_REAL8" or datatype == "CDF_DOUBLE" or datatype == "CDF_EPOCH":
                     return 8 * numElms
-                elif (datatype == 'CDF_EPOCH16'):
+                elif datatype == "CDF_EPOCH16":
                     return 16 * numElms
-                elif (datatype == 'CDF_CHAR' or datatype == 'CDF_UCHAR'):
+                elif datatype == "CDF_CHAR" or datatype == "CDF_UCHAR":
                     return numElms
                 else:
                     return -1
         except Exception:
             return -1
 
     @staticmethod
-    def _sparse_token(sparse):
-        '''
+    def _sparse_token(sparse: str) -> int:
+        """
         Returns the numerical CDF value for sparseness.
-        '''
+        """
 
-        sparses = {'no_sparse': 0,
-                   'pad_sparse': 1,
-                   'prev_sparse': 2}
+        sparses = {"no_sparse": 0, "pad_sparse": 1, "prev_sparse": 2}
         try:
             return sparses[sparse.lower()]
         except Exception:
             return 0
 
-    def _write_cdr(self, f, major, encoding, checksum) -> int:
+    def _write_cdr(self, f: io.BufferedWriter, major: int, encoding: int, checksum: int) -> int:
         f.seek(0, 2)
         byte_loc = f.tell()
         block_size = self.CDR_BASE_SIZE64 + self.CDF_COPYRIGHT_LEN
         section_type = self.CDR_
         gdr_loc = block_size + 8
         version = self.version
         release = self.release
         flag = 0
-        if (major == 1):
+        if major == 1:
             flag = self._set_bit(flag, 0)
         flag = self._set_bit(flag, 1)
         if checksum:
             flag = self._set_bit(flag, 2)
             flag = self._set_bit(flag, 3)
         rfuA = 0
         rfuB = 0
         increment = self.increment
         identifier = 2
         rfuE = -1
-        copy_right = '\nCommon Data Format (CDF)\nhttps://cdf.gsfc.nasa.gov\n' + \
-                     'Space Physics Data Facility\n' + \
-                     'NASA/Goddard Space Flight Center\n' + \
-                     'Greenbelt, Maryland 20771 USA\n' + \
-                     '(User support: gsfc-cdf-support@lists.nasa.gov)\n'
+        copy_right = (
+            "\nCommon Data Format (CDF)\nhttps://cdf.gsfc.nasa.gov\n"
+            + "Space Physics Data Facility\n"
+            + "NASA/Goddard Space Flight Center\n"
+            + "Greenbelt, Maryland 20771 USA\n"
+            + "(User support: gsfc-cdf-support@lists.nasa.gov)\n"
+        )
 
         cdr = bytearray(block_size)
-        cdr[0:8] = struct.pack('>q', block_size)
-        cdr[8:12] = struct.pack('>i', section_type)
-        cdr[12:20] = struct.pack('>q', gdr_loc)
-        cdr[20:24] = struct.pack('>i', version)
-        cdr[24:28] = struct.pack('>i', release)
-        cdr[28:32] = struct.pack('>i', encoding)
-        cdr[32:36] = struct.pack('>i', flag)
-        cdr[36:40] = struct.pack('>i', rfuA)
-        cdr[40:44] = struct.pack('>i', rfuB)
-        cdr[44:48] = struct.pack('>i', increment)
-        cdr[48:52] = struct.pack('>i', identifier)
-        cdr[52:56] = struct.pack('>i', rfuE)
+        cdr[0:8] = struct.pack(">q", block_size)
+        cdr[8:12] = struct.pack(">i", section_type)
+        cdr[12:20] = struct.pack(">q", gdr_loc)
+        cdr[20:24] = struct.pack(">i", version)
+        cdr[24:28] = struct.pack(">i", release)
+        cdr[28:32] = struct.pack(">i", encoding)
+        cdr[32:36] = struct.pack(">i", flag)
+        cdr[36:40] = struct.pack(">i", rfuA)
+        cdr[40:44] = struct.pack(">i", rfuB)
+        cdr[44:48] = struct.pack(">i", increment)
+        cdr[48:52] = struct.pack(">i", identifier)
+        cdr[52:56] = struct.pack(">i", rfuE)
         tofill = self.CDF_COPYRIGHT_LEN - len(copy_right)
-        cdr[56:block_size] = (copy_right + '\0' * tofill).encode()
+        cdr[56:block_size] = (copy_right + "\0" * tofill).encode()
         f.write(cdr)
 
         return byte_loc
 
-    def _write_gdr(self, f) -> int:
+    def _write_gdr(self, f: io.BufferedWriter) -> int:
         f.seek(0, 2)
         byte_loc = f.tell()
         block_size = self.GDR_BASE_SIZE64 + 4 * self.num_rdim
         section_type = self.GDR_
         first_rvariable = 0
         first_zvariable = 0
         first_adr = 0
@@ -1561,56 +1538,59 @@
         num_zvariable = 0
         UIR_head = 0
         rfuC = 0
         leapsecondlastupdate = 20170101
         rfuE = -1
 
         gdr = bytearray(block_size)
-        gdr[0:8] = struct.pack('>q', block_size)
-        gdr[8:12] = struct.pack('>i', section_type)
-        gdr[12:20] = struct.pack('>q', first_rvariable)
-        gdr[20:28] = struct.pack('>q', first_zvariable)
-        gdr[28:36] = struct.pack('>q', first_adr)
-        gdr[36:44] = struct.pack('>q', eof)
-        gdr[44:48] = struct.pack('>i', num_rvariable)
-        gdr[48:52] = struct.pack('>i', num_att)
-        gdr[52:56] = struct.pack('>i', rMaxRec)
-        gdr[56:60] = struct.pack('>i', num_rdim)
-        gdr[60:64] = struct.pack('>i', num_zvariable)
-        gdr[64:72] = struct.pack('>q', UIR_head)
-        gdr[72:76] = struct.pack('>i', rfuC)
-        gdr[76:80] = struct.pack('>i', leapsecondlastupdate)
-        gdr[80:84] = struct.pack('>i', rfuE)
-        if (num_rdim > 0):
+        gdr[0:8] = struct.pack(">q", block_size)
+        gdr[8:12] = struct.pack(">i", section_type)
+        gdr[12:20] = struct.pack(">q", first_rvariable)
+        gdr[20:28] = struct.pack(">q", first_zvariable)
+        gdr[28:36] = struct.pack(">q", first_adr)
+        gdr[36:44] = struct.pack(">q", eof)
+        gdr[44:48] = struct.pack(">i", num_rvariable)
+        gdr[48:52] = struct.pack(">i", num_att)
+        gdr[52:56] = struct.pack(">i", rMaxRec)
+        gdr[56:60] = struct.pack(">i", num_rdim)
+        gdr[60:64] = struct.pack(">i", num_zvariable)
+        gdr[64:72] = struct.pack(">q", UIR_head)
+        gdr[72:76] = struct.pack(">i", rfuC)
+        gdr[76:80] = struct.pack(">i", leapsecondlastupdate)
+        gdr[80:84] = struct.pack(">i", rfuE)
+        if num_rdim > 0:
             for i in range(0, num_rdim):
-                gdr[84 + i * 4:84 + (i + 1) * 4] = struct.pack('>i', self.rdim_sizes[i])
+                gdr[84 + i * 4 : 84 + (i + 1) * 4] = struct.pack(">i", self.rdim_sizes[i])
         f.write(gdr)
 
         return byte_loc
 
-    def _write_adr(self, f, gORv, name) -> Tuple[int, int]:
-        '''
+    def _write_adr(self, f: io.BufferedWriter, gORv: bool, name: str) -> Tuple[int, int]:
+        """
         Writes and ADR to the end of the file.
 
         Additionally, it will update the offset values to either the previous ADR
         or the ADRhead field in the GDR.
 
-        Parameters:
-            f : file
-                The open CDF file
-            gORv : bool
-                True if a global attribute, False if variable attribute
-            name : str
-                name of the attribute
-        Returns:
-            num : int
-                The attribute number
-            byte_loc : int
-                The current location in file f
-        '''
+        Parameters
+        ----------
+        f : file
+            The open CDF file
+        gORv : bool
+            True if a global attribute, False if variable attribute
+        name : str
+            name of the attribute
+
+        Returns
+        -------
+        num : int
+            The attribute number
+        byte_loc : int
+            The current location in file f
+        """
 
         f.seek(0, 2)
         byte_loc = f.tell()
         block_size = self.ADR_BASE_SIZE64
         section_type = self.ADR_
         nextADR = 0
         headAgrEDR = 0
@@ -1624,210 +1604,232 @@
         rfuA = 0
         headAzEDR = 0
         nzEntries = 0
         maxzEntry = -1
         rfuE = -1
 
         adr = bytearray(block_size)
-        adr[0:8] = struct.pack('>q', block_size)
-        adr[8:12] = struct.pack('>i', section_type)
-        adr[12:20] = struct.pack('>q', nextADR)
-        adr[20:28] = struct.pack('>q', headAgrEDR)
-        adr[28:32] = struct.pack('>i', scope)
-        adr[32:36] = struct.pack('>i', num)
-        adr[36:40] = struct.pack('>i', ngrEntries)
-        adr[40:44] = struct.pack('>i', maxgrEntry)
-        adr[44:48] = struct.pack('>i', rfuA)
-        adr[48:56] = struct.pack('>q', headAzEDR)
-        adr[56:60] = struct.pack('>i', nzEntries)
-        adr[60:64] = struct.pack('>i', maxzEntry)
-        adr[64:68] = struct.pack('>i', rfuE)
+        adr[0:8] = struct.pack(">q", block_size)
+        adr[8:12] = struct.pack(">i", section_type)
+        adr[12:20] = struct.pack(">q", nextADR)
+        adr[20:28] = struct.pack(">q", headAgrEDR)
+        adr[28:32] = struct.pack(">i", scope)
+        adr[32:36] = struct.pack(">i", num)
+        adr[36:40] = struct.pack(">i", ngrEntries)
+        adr[40:44] = struct.pack(">i", maxgrEntry)
+        adr[44:48] = struct.pack(">i", rfuA)
+        adr[48:56] = struct.pack(">q", headAzEDR)
+        adr[56:60] = struct.pack(">i", nzEntries)
+        adr[60:64] = struct.pack(">i", maxzEntry)
+        adr[64:68] = struct.pack(">i", rfuE)
         tofill = 256 - len(name)
-        adr[68:324] = (name + '\0' * tofill).encode()
+        adr[68:324] = (name + "\0" * tofill).encode()
         f.write(adr)
-        info = []
-        info.append(name)
-        info.append(scope)
-        info.append(byte_loc)
+        info = (name, scope, byte_loc)
         self.attrsinfo[num] = info
-        if (scope == 1):
+        if scope == 1:
             self.gattrs.append(name)
         else:
             self.vattrs.append(name)
 
         self.attrs.append(name)
-        if (num > 0):
+        if num > 0:
             # ADR's ADRnext
-            self._update_offset_value(f, self.attrsinfo[num - 1][2] + 12, 8,
-                                      byte_loc)
+            self._update_offset_value(f, self.attrsinfo[num - 1][2] + 12, 8, byte_loc)
         else:
             # GDR's ADRhead
             self._update_offset_value(f, self.gdr_head + 28, 8, byte_loc)
 
         # GDR's NumAttr
         self._update_offset_value(f, self.gdr_head + 48, 4, num + 1)
 
         return num, byte_loc
 
-    def _write_aedr(self, f, gORz, attrNum, entryNum, value, pdataType,
-                    pnumElems, zVar):
-        '''
+    def _write_aedr(
+        self,
+        f: io.BufferedWriter,
+        gORz: bool,
+        attrNum: int,
+        entryNum: int,
+        value: Union[Number, np.ndarray],
+        pdataType: int,
+        pnumElems: int,
+        zVar: bool,
+    ) -> int:
+        """
         Writes an aedr into the end of the file.
 
-        Parameters:
-            f : file
-                The current open CDF file
-            gORz : bool
-                True if this entry is for a global or z variable, False if r variable
-            attrNum : int
-                Number of the attribute this aedr belongs to.
-            entryNum : int
-                Number of the entry
-            value :
-                The value of this entry
-            pdataType : int
-                The CDF data type of the value
-            pnumElems : int
-                Number of elements in the value.
-            zVar : bool
-                True if this entry belongs to a z variable
-
-        Returns:
-            byte_loc : int
-                This current location in the file after writing the aedr.
-        '''
+        Parameters
+        ----------
+        f : file
+            The current open CDF file
+        gORz : bool
+            True if this entry is for a global or z variable, False if r variable
+        attrNum : int
+            Number of the attribute this aedr belongs to.
+        entryNum : int
+            Number of the entry
+        value :
+            The value of this entry
+        pdataType : int
+            The CDF data type of the value
+        pnumElems : int
+            Number of elements in the value.
+        zVar : bool
+            True if this entry belongs to a z variable
+
+        Returns
+        -------
+        byte_loc : int
+            This current location in the file after writing the aedr.
+        """
         f.seek(0, 2)
         byte_loc = f.tell()
-        if (gORz or zVar != True):
+        if gORz or zVar != True:
             section_type = self.AgrEDR_
         else:
             section_type = self.AzEDR_
         nextAEDR = 0
 
         if pdataType is None:
             # Figure out Data Type if not supplied
-            if hasattr(value, '__len__') and not isinstance(value, str):
+            if not isinstance(value, Number):
                 avalue = value[0]
             else:
                 avalue = value
-            if (isinstance(avalue, int)):
+            if isinstance(avalue, int):
                 pdataType = self.CDF_INT8
-            elif (isinstance(avalue, float)):
+            elif isinstance(avalue, float):
                 pdataType = self.CDF_FLOAT
-            elif (isinstance(avalue, complex)):
+            elif isinstance(avalue, complex):
                 pdataType = self.CDF_EPOCH16
             else:
                 # assume a boolean
                 pdataType = self.CDF_INT1
 
         if pnumElems is None:
             # Figure out number of elements if not supplied
             if isinstance(value, str):
                 pdataType = self.CDF_CHAR
-                pnumElems = 1 if len(value) == 0  else len(value)
+                pnumElems = 1 if len(value) == 0 else len(value)
             else:
-                if hasattr(value, '__len__') and not isinstance(value, str):
+                if hasattr(value, "__len__") and not isinstance(value, str):
                     pnumElems = len(value)
                 else:
                     pnumElems = 1
 
         dataType = pdataType
         numElems = pnumElems
 
         rfuB = 0
         rfuC = 0
         rfuD = -1
         rfuE = -1
         if gORz:
             numStrings = 0
         else:
-            if (isinstance(value, str)):
-                numStrings = value.count('\\N ') + 1
+            if isinstance(value, str):
+                numStrings = value.count("\\N ") + 1
             else:
                 numStrings = 0
         recs, cdata = self._convert_data(dataType, numElems, 1, value)
-        if (dataType == 51):
+        if dataType == 51:
             numElems = 1 if len(cdata) == 0 else len(cdata)
-        if (len(cdata) == 0):
+        if len(cdata) == 0:
             value_size = 1
-            cdata = '\x00'.encode()
+            cdata = "\x00".encode()
         else:
             value_size = len(cdata)
         block_size = value_size + 56
         aedr = bytearray(block_size)
-        aedr[0:8] = struct.pack('>q', block_size)
-        aedr[8:12] = struct.pack('>i', section_type)
-        aedr[12:20] = struct.pack('>q', nextAEDR)
-        aedr[20:24] = struct.pack('>i', attrNum)
-        aedr[24:28] = struct.pack('>i', dataType)
-        aedr[28:32] = struct.pack('>i', entryNum)
-        aedr[32:36] = struct.pack('>i', numElems)
-        aedr[36:40] = struct.pack('>i', numStrings)
-        aedr[40:44] = struct.pack('>i', rfuB)
-        aedr[44:48] = struct.pack('>i', rfuC)
-        aedr[48:52] = struct.pack('>i', rfuD)
-        aedr[52:56] = struct.pack('>i', rfuE)
+        aedr[0:8] = struct.pack(">q", block_size)
+        aedr[8:12] = struct.pack(">i", section_type)
+        aedr[12:20] = struct.pack(">q", nextAEDR)
+        aedr[20:24] = struct.pack(">i", attrNum)
+        aedr[24:28] = struct.pack(">i", dataType)
+        aedr[28:32] = struct.pack(">i", entryNum)
+        aedr[32:36] = struct.pack(">i", numElems)
+        aedr[36:40] = struct.pack(">i", numStrings)
+        aedr[40:44] = struct.pack(">i", rfuB)
+        aedr[44:48] = struct.pack(">i", rfuC)
+        aedr[48:52] = struct.pack(">i", rfuD)
+        aedr[52:56] = struct.pack(">i", rfuE)
         aedr[56:block_size] = cdata
         f.write(aedr)
 
         return byte_loc
 
-    def _write_vdr(self, f, cdataType, numElems, numDims, dimSizes, name,
-                   dimVary, recVary, sparse, blockingfactor, compression,
-                   pad, zVar):
-        '''
+    def _write_vdr(
+        self,
+        f: io.BufferedWriter,
+        cdataType: int,
+        numElems: int,
+        numDims: int,
+        dimSizes: List[int],
+        name: str,
+        dimVary: List[bool],
+        recVary: bool,
+        sparse: int,
+        blockingfactor: int,
+        compression: int,
+        pad: str,
+        zVar: bool,
+    ) -> Tuple[int, int]:
+        """
         Writes a VDR block to the end of the file.
 
-        Parameters:
-            f : file
-                The open CDF file
-            cdataType : int
-                The CDF data type
-            numElems : int
-                The number of elements in the variable
-            numDims : int
-                The number of dimensions in the variable
-            dimSizes : int
-                The size of each dimension
-            name : str
-                The name of the variable
-            dimVary : array of bool
-                Bool array of size numDims.
-                True if a dimension is physical, False if a dimension is not physical
-            recVary : bool
-                True if each record is unique
-            sparse : bool
-                True if using sparse records
-            blockingfactor: int
-                No idea
-            compression : int
-                The level of compression between 0-9
-            pad : num
-                The pad values to insert
-            zVar : bool
-                True if this variable is a z variable
-
-        Returns:
-            num : int
-                The number of the variable
-            byte_loc : int
-                The current byte location within the file
-        '''
+        Parameters
+        ----------
+        f : file
+            The open CDF file
+        cdataType : int
+            The CDF data type
+        numElems : int
+            The number of elements in the variable
+        numDims : int
+            The number of dimensions in the variable
+        dimSizes : int
+            The size of each dimension
+        name : str
+            The name of the variable
+        dimVary : array of bool
+            Bool array of size numDims.
+            True if a dimension is physical, False if a dimension is not physical
+        recVary : bool
+            True if each record is unique
+        sparse : bool
+            True if using sparse records
+        blockingfactor: int
+            No idea
+        compression : int
+            The level of compression between 0-9
+        pad : num
+            The pad values to insert
+        zVar : bool
+            True if this variable is a z variable
+
+        Returns
+        -------
+        num : int
+            The number of the variable
+        byte_loc : int
+            The current byte location within the file
+        """
 
         if zVar:
             block_size = self.zVDR_BASE_SIZE64
             section_type = self.zVDR_
         else:
             block_size = self.rVDR_BASE_SIZE64
             section_type = self.rVDR_
 
         nextVDR = 0
         dataType = cdataType
         if dataType == -1:
-            raise ValueError('Bad data type.')
+            raise ValueError("Bad data type.")
 
         maxRec = -1
         headVXR = 0
         tailVXR = 0
         flags = 0
         if recVary:
             flags = self._set_bit(flags, 0)
@@ -1838,16 +1840,15 @@
         rfuF = -1
         if zVar:
             num = len(self.zvars)
         else:
             num = len(self.rvars)
 
         if compression > 0:
-            offsetCPRorSPR = self._write_cpr(f, self.GZIP_COMPRESSION,
-                                             compression)
+            offsetCPRorSPR = self._write_cpr(f, self.GZIP_COMPRESSION, compression)
             flags = self._set_bit(flags, 2)
         else:
             offsetCPRorSPR = -1
 
         if blockingfactor is None:
             blockingFactor = 1
         else:
@@ -1858,298 +1859,299 @@
             if zVar:
                 block_size = block_size + numDims * 8
             else:
                 block_size = block_size + numDims * 4
 
         # Determine pad value
         if pad is not None:
-            if (dataType == 51 or dataType == 52):
+            if dataType == 51 or dataType == 52:
                 # pad needs to be the correct number of elements
-                if (len(pad) < numElems):
-                    pad += '\0' * (numElems - len(pad))
-                elif (len(pad) > numElems):
+                if len(pad) < numElems:
+                    pad += "\0" * (numElems - len(pad))
+                elif len(pad) > numElems:
                     pad = pad[:numElems]
-                pad = pad.encode()
+                pad_bytes = pad.encode()
             else:
-                dummy, pad = self._convert_data(dataType, numElems, 1, pad)
+                dummy, pad_bytes = self._convert_data(dataType, numElems, 1, pad)
         else:
-            pad = self._default_pad(dataType, numElems)
+            pad_bytes = self._default_pad(dataType, numElems)
 
         f.seek(0, 2)
         byte_loc = f.tell()
-        block_size += len(pad)
+        block_size += len(pad_bytes)
         vdr = bytearray(block_size)
         # if (dataType == 51):
         #    numElems = len(pad)
-        vdr[0:8] = struct.pack('>q', block_size)
-        vdr[8:12] = struct.pack('>i', section_type)
-        vdr[12:20] = struct.pack('>q', nextVDR)
-        vdr[20:24] = struct.pack('>i', dataType)
-        vdr[24:28] = struct.pack('>i', maxRec)
-        vdr[28:36] = struct.pack('>q', headVXR)
-        vdr[36:44] = struct.pack('>q', tailVXR)
-        vdr[44:48] = struct.pack('>i', flags)
-        vdr[48:52] = struct.pack('>i', sRecords)
-        vdr[52:56] = struct.pack('>i', rfuB)
-        vdr[56:60] = struct.pack('>i', rfuC)
-        vdr[60:64] = struct.pack('>i', rfuF)
-        vdr[64:68] = struct.pack('>i', numElems)
-        vdr[68:72] = struct.pack('>i', num)
-        vdr[72:80] = struct.pack('>q', offsetCPRorSPR)
-        vdr[80:84] = struct.pack('>i', blockingFactor)
+        vdr[0:8] = struct.pack(">q", block_size)
+        vdr[8:12] = struct.pack(">i", section_type)
+        vdr[12:20] = struct.pack(">q", nextVDR)
+        vdr[20:24] = struct.pack(">i", dataType)
+        vdr[24:28] = struct.pack(">i", maxRec)
+        vdr[28:36] = struct.pack(">q", headVXR)
+        vdr[36:44] = struct.pack(">q", tailVXR)
+        vdr[44:48] = struct.pack(">i", flags)
+        vdr[48:52] = struct.pack(">i", sRecords)
+        vdr[52:56] = struct.pack(">i", rfuB)
+        vdr[56:60] = struct.pack(">i", rfuC)
+        vdr[60:64] = struct.pack(">i", rfuF)
+        vdr[64:68] = struct.pack(">i", numElems)
+        vdr[68:72] = struct.pack(">i", num)
+        vdr[72:80] = struct.pack(">q", offsetCPRorSPR)
+        vdr[80:84] = struct.pack(">i", blockingFactor)
         tofill = 256 - len(name)
-        vdr[84:340] = (name + '\0' * tofill).encode()
+        vdr[84:340] = (name + "\0" * tofill).encode()
         if zVar:
-            vdr[340:344] = struct.pack('>i', numDims)
-            if (numDims > 0):
+            vdr[340:344] = struct.pack(">i", numDims)
+            if numDims > 0:
                 for i in range(0, numDims):
-                    vdr[344 + i * 4:344 + (i + 1) * 4] = struct.pack('>i', dimSizes[i])
+                    vdr[344 + i * 4 : 344 + (i + 1) * 4] = struct.pack(">i", dimSizes[i])
                 ist = 344 + numDims * 4
                 for i in range(0, numDims):
-                    vdr[ist + i * 4:ist + (i + 1) * 4] = struct.pack('>i', self.VARY)
+                    vdr[ist + i * 4 : ist + (i + 1) * 4] = struct.pack(">i", self.VARY)
             ist = 344 + 8 * numDims
         else:
-            if (numDims > 0):
+            if numDims > 0:
                 for i in range(0, numDims):
-                    if (dimVary[i] or dimVary[i] != 0):
-                        vdr[340 + i * 4:344 + i * 4] = struct.pack('>i', self.VARY)
+                    if dimVary[i] or dimVary[i] != 0:
+                        vdr[340 + i * 4 : 344 + i * 4] = struct.pack(">i", self.VARY)
                     else:
-                        vdr[340 + i * 4:344 + i * 4] = struct.pack('>i', self.NOVARY)
+                        vdr[340 + i * 4 : 344 + i * 4] = struct.pack(">i", self.NOVARY)
             ist = 340 + 4 * numDims
-        vdr[ist:block_size] = pad
+        vdr[ist:block_size] = pad_bytes
         f.write(vdr)
 
         # Set variable info
-        info = []
-        info.append(name)
-        info.append(byte_loc)
-        if zVar:
-            info.append(numDims)
-            info.append(dimSizes)
-        else:
-            info.append(self.num_rdim)
-            info.append(self.rdim_sizes)
-        info.append(dimVary)
+
+        if not zVar:
+            numDims = self.num_rdim
+            dimSizes = self.rdim_sizes
+
+        info = (name, byte_loc, numDims, dimSizes, dimVary)
 
         # Update the pointers from the CDR/previous VDR
         if zVar:
             self.zvarsinfo[num] = info
             self.zvars.append(name)
-            if (num > 0):
+            if num > 0:
                 # VDR's VDRnext
-                self._update_offset_value(f, self.zvarsinfo[num - 1][1] + 12, 8,
-                                          byte_loc)
+                self._update_offset_value(f, self.zvarsinfo[num - 1][1] + 12, 8, byte_loc)
             # GDR's NzVars
             self._update_offset_value(f, self.gdr_head + 60, 4, num + 1)
         else:
             self.rvarsinfo[num] = info
             self.rvars.append(name)
-            if (num > 0):
+            if num > 0:
                 # VDR's VDRnext
-                self._update_offset_value(f, self.rvarsinfo[num - 1][1] + 12, 8,
-                                          byte_loc)
+                self._update_offset_value(f, self.rvarsinfo[num - 1][1] + 12, 8, byte_loc)
             # GDR's NrVars
             self._update_offset_value(f, self.gdr_head + 44, 4, num + 1)
 
         return num, byte_loc
 
-    def _write_vxr(self, f, numEntries=None):
-        '''
+    def _write_vxr(self, f: io.BufferedWriter, numEntries: Optional[int] = None) -> int:
+        """
         Creates a VXR at the end of the file.
         Returns byte location of the VXR
         The First, Last, and Offset fields will need to be filled in later
-        '''
+        """
 
         f.seek(0, 2)
         byte_loc = f.tell()
         section_type = self.VXR_
         nextVXR = 0
-        if (numEntries is None):
+        if numEntries is None:
             nEntries = self.NUM_VXR_ENTRIES
         else:
             nEntries = int(numEntries)
         block_size = self.VXR_BASE_SIZE64 + (4 + 4 + 8) * nEntries
         nUsedEntries = 0
         firsts = [-1] * nEntries
         lasts = [-1] * nEntries
         offsets = [-1] * nEntries
 
         vxr = bytearray(block_size)
-        vxr[0:8] = struct.pack('>q', block_size)
-        vxr[8:12] = struct.pack('>i', section_type)
-        vxr[12:20] = struct.pack('>q', nextVXR)
-        vxr[20:24] = struct.pack('>i', nEntries)
-        vxr[24:28] = struct.pack('>i', nUsedEntries)
+        vxr[0:8] = struct.pack(">q", block_size)
+        vxr[8:12] = struct.pack(">i", section_type)
+        vxr[12:20] = struct.pack(">q", nextVXR)
+        vxr[20:24] = struct.pack(">i", nEntries)
+        vxr[24:28] = struct.pack(">i", nUsedEntries)
         estart = 28 + 4 * nEntries
-        vxr[28:estart] = struct.pack('>%si' % nEntries, *firsts)
+        vxr[28:estart] = struct.pack(">%si" % nEntries, *firsts)
         eend = estart + 4 * nEntries
-        vxr[estart:eend] = struct.pack('>%si' % nEntries, *lasts)
-        vxr[eend:block_size] = struct.pack('>%sq' % nEntries, *offsets)
+        vxr[estart:eend] = struct.pack(">%si" % nEntries, *lasts)
+        vxr[eend:block_size] = struct.pack(">%sq" % nEntries, *offsets)
         f.write(vxr)
         return byte_loc
 
-    def _write_vvr(self, f, data):
-        '''
+    def _write_vvr(self, f: io.BufferedWriter, data: bytes) -> int:
+        """
         Writes a vvr to the end of file "f" with the byte stream "data".
-        '''
+        """
         f.seek(0, 2)
         byte_loc = f.tell()
         block_size = self.VVR_BASE_SIZE64 + len(data)
         section_type = self.VVR_
 
         vvr1 = bytearray(12)
-        vvr1[0:8] = struct.pack('>q', block_size)
-        vvr1[8:12] = struct.pack('>i', section_type)
+        vvr1[0:8] = struct.pack(">q", block_size)
+        vvr1[8:12] = struct.pack(">i", section_type)
         f.write(vvr1)
         f.write(data)
 
         return byte_loc
 
-    def _write_cpr(self, f, cType, parameter) -> int:
-        '''
+    def _write_cpr(self, f: io.BufferedWriter, cType: int, parameter: int) -> int:
+        """
         Write compression info to the end of the file in a CPR.
-        '''
+        """
         f.seek(0, 2)
         byte_loc = f.tell()
         block_size = self.CPR_BASE_SIZE64 + 4
         section_type = self.CPR_
         rfuA = 0
         pCount = 1
 
         cpr = bytearray(block_size)
-        cpr[0:8] = struct.pack('>q', block_size)
-        cpr[8:12] = struct.pack('>i', section_type)
-        cpr[12:16] = struct.pack('>i', cType)
-        cpr[16:20] = struct.pack('>i', rfuA)
-        cpr[20:24] = struct.pack('>i', pCount)
-        cpr[24:28] = struct.pack('>i', parameter)
+        cpr[0:8] = struct.pack(">q", block_size)
+        cpr[8:12] = struct.pack(">i", section_type)
+        cpr[12:16] = struct.pack(">i", cType)
+        cpr[16:20] = struct.pack(">i", rfuA)
+        cpr[20:24] = struct.pack(">i", pCount)
+        cpr[24:28] = struct.pack(">i", parameter)
         f.write(cpr)
 
         return byte_loc
 
-    def _write_cvvr(self, f, data):
-        '''
+    def _write_cvvr(self, f: io.BufferedWriter, data: Any) -> int:
+        """
         Write compressed "data" variable to the end of the file in a CVVR
-        '''
+        """
         f.seek(0, 2)
         byte_loc = f.tell()
         cSize = len(data)
         block_size = self.CVVR_BASE_SIZE64 + cSize
         section_type = self.CVVR_
         rfuA = 0
 
         cvvr1 = bytearray(24)
-        cvvr1[0:8] = struct.pack('>q', block_size)
-        cvvr1[8:12] = struct.pack('>i', section_type)
-        cvvr1[12:16] = struct.pack('>i', rfuA)
-        cvvr1[16:24] = struct.pack('>q', cSize)
+        cvvr1[0:8] = struct.pack(">q", block_size)
+        cvvr1[8:12] = struct.pack(">i", section_type)
+        cvvr1[12:16] = struct.pack(">i", rfuA)
+        cvvr1[16:24] = struct.pack(">q", cSize)
         f.write(cvvr1)
         f.write(data)
 
         return byte_loc
 
-    def _write_ccr(self, f, g, level: int):
-        '''
+    def _write_ccr(self, f: io.BufferedWriter, g: io.BufferedWriter, level: int) -> None:
+        """
         Write a CCR to file "g" from file "f" with level "level".
         Currently, only handles gzip compression.
 
         Parameters:
             f : file
                 Uncompressed file to read from
             g : file
                 File to read the compressed file into
             level : int
                 The level of the compression from 0 to 9
 
         Returns: None
 
-        '''
+        """
         f.seek(8)
         data = f.read()
         uSize = len(data)
         section_type = self.CCR_
         rfuA = 0
         cData = gzip.compress(data, level)
         block_size = self.CCR_BASE_SIZE64 + len(cData)
         cprOffset = 0
         ccr1 = bytearray(32)
         # ccr1[0:4] = binascii.unhexlify(CDF.V3magicNUMBER_1)
         # ccr1[4:8] = binascii.unhexlify(CDF.V3magicNUMBER_2c)
-        ccr1[0:8] = struct.pack('>q', block_size)
-        ccr1[8:12] = struct.pack('>i', section_type)
-        ccr1[12:20] = struct.pack('>q', cprOffset)
-        ccr1[20:28] = struct.pack('>q', uSize)
-        ccr1[28:32] = struct.pack('>i', rfuA)
+        ccr1[0:8] = struct.pack(">q", block_size)
+        ccr1[8:12] = struct.pack(">i", section_type)
+        ccr1[12:20] = struct.pack(">q", cprOffset)
+        ccr1[20:28] = struct.pack(">q", uSize)
+        ccr1[28:32] = struct.pack(">i", rfuA)
         g.seek(0, 2)
         g.write(ccr1)
         g.write(cData)
         cprOffset = self._write_cpr(g, self.GZIP_COMPRESSION, level)
         self._update_offset_value(g, 20, 8, cprOffset)
 
-    def _convert_option(self):
-        '''
+    def _convert_option(self) -> str:
+        """
         Determines which symbol to use for numpy conversions
         > : a little endian system to big endian ordering
         < : a big endian system to little endian ordering
         = : No conversion
-        '''
-        data_endian = 'little'
-        if (self._encoding == 1 or self._encoding == 2 or self._encoding == 5 or
-            self._encoding == 7 or self._encoding == 9 or self._encoding == 11 or
-                self._encoding == 12 or self._encoding == 18):
-            data_endian = 'big'
-        if sys.byteorder == 'little' and data_endian == 'big':
+        """
+        data_endian = "little"
+        if (
+            self._encoding == 1
+            or self._encoding == 2
+            or self._encoding == 5
+            or self._encoding == 7
+            or self._encoding == 9
+            or self._encoding == 11
+            or self._encoding == 12
+            or self._encoding == 18
+        ):
+            data_endian = "big"
+        if sys.byteorder == "little" and data_endian == "big":
             # big->little
-            order = '>'
-        elif sys.byteorder == 'big' and data_endian == 'little':
+            order = ">"
+        elif sys.byteorder == "big" and data_endian == "little":
             # little->big
-            order = '<'
+            order = "<"
         else:
             # no conversion
-            order = '='
+            order = "="
 
         return order
 
     @staticmethod
-    def _convert_type(data_type):
-        '''
+    def _convert_type(data_type: int) -> str:
+        """
         Converts CDF data types into python types
-        '''
+        """
         if data_type in (1, 41):
-            dt_string = 'b'
+            dt_string = "b"
         elif data_type == 2:
-            dt_string = 'h'
+            dt_string = "h"
         elif data_type == 4:
-            dt_string = 'i'
+            dt_string = "i"
         elif data_type in (8, 33):
-            dt_string = 'q'
+            dt_string = "q"
         elif data_type == 11:
-            dt_string = 'B'
+            dt_string = "B"
         elif data_type == 12:
-            dt_string = 'H'
+            dt_string = "H"
         elif data_type == 14:
-            dt_string = 'I'
+            dt_string = "I"
         elif data_type in (21, 44):
-            dt_string = 'f'
+            dt_string = "f"
         elif data_type in (22, 45, 31):
-            dt_string = 'd'
+            dt_string = "d"
         elif data_type == 32:
-            dt_string = 'd'
+            dt_string = "d"
         elif data_type in (51, 52):
-            dt_string = 's'
+            dt_string = "s"
         else:
-            dt_string = ''
+            dt_string = ""
 
         return dt_string
 
     @staticmethod
-    def _convert_nptype(data_type, data):
-        '''
+    def _convert_nptype(data_type: int, data: Any) -> bytes:
+        """
         Converts "data" of CDF type "data_type" into a numpy array
-        '''
+        """
         if data_type in (1, 41):
             return np.int8(data).tobytes()
         elif data_type == 2:
             return np.int16(data).tobytes()
         elif data_type == 4:
             return np.int32(data).tobytes()
         elif (data_type == 8) or (data_type == 33):
@@ -2160,283 +2162,282 @@
             return np.uint16(data).tobytes()
         elif data_type == 14:
             return np.uint32(data).tobytes()
         elif (data_type == 21) or (data_type == 44):
             return np.float32(data).tobytes()
         elif (data_type == 22) or (data_type == 45) or (data_type == 31):
             return np.float64(data).tobytes()
-        elif (data_type == 32):
+        elif data_type == 32:
             return np.complex128(data).tobytes()
         elif ((data_type) == 51) or ((data_type) == 52):
-            utf8_bytes = np.asarray(data).astype('U').tobytes()
-            return utf8_bytes.decode().replace('\x00', '').encode('ASCII')
+            utf8_bytes = np.asarray(data).astype("U").tobytes()
+            return utf8_bytes.decode().replace("\x00", "").encode("ASCII")
         else:
             return data
 
-    def _default_pad(self, data_type, numElems):
-        '''
+    def _default_pad(self, data_type: int, numElems: int) -> bytes:
+        """
         Determines the default pad data for a "data_type"
-        '''
+        """
         order = self._convert_option()
         if (data_type == 1) or (data_type == 41):
-            pad_value = struct.pack(order + 'b', -127)
+            pad_value = struct.pack(order + "b", -127)
         elif data_type == 2:
-            pad_value = struct.pack(order + 'h', -32767)
+            pad_value = struct.pack(order + "h", -32767)
         elif data_type == 4:
-            pad_value = struct.pack(order + 'i', -2147483647)
+            pad_value = struct.pack(order + "i", -2147483647)
         elif (data_type == 8) or (data_type == 33):
-            pad_value = struct.pack(order + 'q', -9223372036854775807)
+            pad_value = struct.pack(order + "q", -9223372036854775807)
         elif data_type == 11:
-            pad_value = struct.pack(order + 'B', 254)
+            pad_value = struct.pack(order + "B", 254)
         elif data_type == 12:
-            pad_value = struct.pack(order + 'H', 65534)
+            pad_value = struct.pack(order + "H", 65534)
         elif data_type == 14:
-            pad_value = struct.pack(order + 'I', 4294967294)
+            pad_value = struct.pack(order + "I", 4294967294)
         elif (data_type == 21) or (data_type == 44):
-            pad_value = struct.pack(order + 'f', -1.0E30)
+            pad_value = struct.pack(order + "f", -1.0e30)
         elif (data_type == 22) or (data_type == 45):
-            pad_value = struct.pack(order + 'd', -1.0E30)
-        elif (data_type == 31):
-            pad_value = struct.pack(order + 'd', 0.0)
-        elif (data_type == 32):
-            pad_value = struct.pack(order + '2d', *[0.0, 0.0])
+            pad_value = struct.pack(order + "d", -1.0e30)
+        elif data_type == 31:
+            pad_value = struct.pack(order + "d", 0.0)
+        elif data_type == 32:
+            pad_value = struct.pack(order + "2d", *[0.0, 0.0])
         elif (data_type == 51) or (data_type == 52):
-            tmpPad = str(' ' * numElems).encode()
+            tmpPad = str(" " * numElems).encode()
             form = str(numElems)
-            pad_value = struct.pack(form + 'b', *tmpPad)
+            pad_value = struct.pack(form + "b", *tmpPad)
         return pad_value
 
-    def _convert_data(self, data_type, num_elems, num_values, indata):
-        '''
+    def _convert_data(self, data_type: int, num_elems: int, num_values: int, indata: Any) -> Tuple[int, bytes]:
+        """
         Converts "indata" into a byte stream
 
-        Parameters:
-            data_type : int
-                The CDF file data type
-
-            num_elems : int
-                The number of elements in the data
+        Parameters
+        ----------
+        data_type : int
+            The CDF file data type
 
-            num_values : int
-                The number of values in each record
+        num_elems : int
+            The number of elements in the data
 
-            indata : (varies)
-                The data to be converted
+        num_values : int
+            The number of values in each record
 
-        Returns:
-            recs : int
-                The number of records generated by converting indata
-            odata : byte stream
-                The stream of bytes to write to the CDF file
-        '''
+        indata : (varies)
+            The data to be converted
+
+        Returns
+        -------
+        recs : int
+            The number of records generated by converting indata
+        odata : byte stream
+            The stream of bytes to write to the CDF file
+        """
 
         recSize = self._datatype_size(data_type, num_elems) * num_values
-        if (isinstance(indata, list) or isinstance(indata, tuple)):
+        if isinstance(indata, list) or isinstance(indata, tuple):
             if (num_values != 1) and (len(indata) != num_values):
                 raise Exception("Use numpy for inputting multidimensional arrays")
             size = len(indata)
-            if (data_type == self.CDF_CHAR or data_type == self.CDF_UCHAR):
-                odata = ''
+            if data_type == self.CDF_CHAR or data_type == self.CDF_UCHAR:
+                odata = ""
                 for x in range(0, size):
                     adata = indata[x]
-                    if (isinstance(adata, list) or isinstance(adata, tuple)):
+                    if isinstance(adata, list) or isinstance(adata, tuple):
                         size2 = len(adata)
                         for y in range(0, size2):
-                            odata += adata[y].ljust(num_elems, '\x00')
+                            odata += adata[y].ljust(num_elems, "\x00")
                     else:
                         size2 = 1
-                        odata += adata.ljust(num_elems, '\x00')
+                        odata += adata.ljust(num_elems, "\x00")
                 recs = int((size * size2) / num_values)
                 return recs, odata.encode()
             else:
                 tofrom = self._convert_option()
                 dt_string = self._convert_type(data_type)
                 recs = int(size / num_values)
-                if (data_type == self.CDF_EPOCH16 and
-                        isinstance(indata[0], complex)):
+                if data_type == self.CDF_EPOCH16 and isinstance(indata[0], complex):
                     complex_data = []
                     for x in range(0, recs):
                         acomplex = indata[x]
                         complex_data.append(acomplex.real)
                         complex_data.append(acomplex.imag)
                     size = 2 * size
                     indata = complex_data
-                if (data_type == self.CDF_EPOCH16 and
-                        not isinstance(indata[0], complex)):
+                if data_type == self.CDF_EPOCH16 and not isinstance(indata[0], complex):
                     recs = int(recs / 2)
                 form = tofrom + str(size) + dt_string
                 return recs, struct.pack(form, *indata)
-        elif (isinstance(indata, bytes)):
+        elif isinstance(indata, bytes):
             tofrom = self._convert_option()
             recs = int(len(indata) / recSize)
             dt_string = self._convert_type(data_type)
             size = recs * num_values * num_elems
-            if (data_type == self.CDF_EPOCH16):
+            if data_type == self.CDF_EPOCH16:
                 size = size * 2
             form = str(size) + dt_string
             form2 = tofrom + form
             datau = struct.unpack(form, indata)
             return recs, struct.pack(form2, *datau)
         elif isinstance(indata, np.ndarray):
-            if (data_type == self.CDF_CHAR or data_type == self.CDF_UCHAR):
+            if data_type == self.CDF_CHAR or data_type == self.CDF_UCHAR:
                 size = indata.size
-                odata = ''
+                odata = ""
                 if size >= 1:
                     for x in range(0, size):
-                        if hasattr(indata, 'len'):
+                        if hasattr(indata, "len"):
                             adata = indata[x]
                         else:
                             adata = indata
                         if isinstance(adata, list) or isinstance(adata, tuple):
                             size2 = len(adata)
                             for y in range(0, size2):
-                                odata += str(adata[y]).ljust(num_elems, '\x00')
+                                odata += str(adata[y]).ljust(num_elems, "\x00")
                         elif isinstance(adata, np.ndarray):
                             size2 = adata.size
                             for y in range(0, size2):
-                                if hasattr(adata, 'len'):
+                                if hasattr(adata, "len"):
                                     bdata = adata[y]
                                 else:
                                     bdata = adata
-                                odata += str(bdata).ljust(num_elems, '\x00')
+                                odata += str(bdata).ljust(num_elems, "\x00")
                         else:
                             size2 = 1
-                            odata += str(adata).ljust(num_elems, '\x00')
+                            odata += str(adata).ljust(num_elems, "\x00")
                 else:
-                    adata = ''
+                    adata = ""
                     size2 = 1
-                    odata += str(adata).ljust(num_elems, '\x00')
+                    odata += str(adata).ljust(num_elems, "\x00")
                 recs = int((size * size2) / num_values)
                 return recs, odata.encode()
             else:
                 tofrom = self._convert_option()
                 npdata = self._convert_nptype(data_type, indata)
                 if indata.size == 0:  # Check if the data being read in is zero size
                     recs = 0
                 elif indata.size == num_values * num_elems:  # Check if only one record is being read in
                     recs = 1
                 else:
                     recs = len(indata)
                 dt_string = self._convert_type(data_type)
-                if (data_type == self.CDF_EPOCH16):
+                if data_type == self.CDF_EPOCH16:
                     num_elems = 2 * num_elems
                 form = str(recs * num_values * num_elems) + dt_string
                 form2 = tofrom + str(recs * num_values * num_elems) + dt_string
                 datau = struct.unpack(form, npdata)
                 return recs, struct.pack(form2, *datau)
-        elif (isinstance(indata, str)):
-            return 1, indata.ljust(num_elems, '\x00').encode()
+        elif isinstance(indata, str):
+            return 1, indata.ljust(num_elems, "\x00").encode()
         else:
             tofrom = self._convert_option()
             dt_string = self._convert_type(data_type)
-            if (data_type == self.CDF_EPOCH16):
+            if data_type == self.CDF_EPOCH16:
                 num_elems = 2 * num_elems
             try:
                 recs = int(len(indata) / recSize)
             except Exception:
                 recs = 1
-            if (data_type == self.CDF_EPOCH16):
+            if data_type == self.CDF_EPOCH16:
                 complex_data = []
-                if (recs > 1):
+                if recs > 1:
                     for x in range(0, recs):
                         acomplex = indata[x]
                         complex_data.append(acomplex.real)
                         complex_data.append(acomplex.imag)
                 else:
                     complex_data.append(indata.real)
                     complex_data.append(indata.imag)
                 indata = complex_data
             form = tofrom + str(recs * num_values * num_elems) + dt_string
-            if (recs * num_values * num_elems > 1):
+            if recs * num_values * num_elems > 1:
                 return recs, struct.pack(form, *indata)
             else:
                 return recs, struct.pack(form, indata)
 
-    def _num_values(self, zVar: bool, varNum):
-        '''
+    def _num_values(self, zVar: bool, varNum: int) -> int:
+        """
         Determines the number of values in a record.
         Set zVar=True if this is a zvariable.
-        '''
+        """
         values = 1
         if zVar:
             numDims = self.zvarsinfo[varNum][2]
             dimSizes = self.zvarsinfo[varNum][3]
             dimVary = self.zvarsinfo[varNum][4]
         else:
             numDims = self.rvarsinfo[varNum][2]
             dimSizes = self.rvarsinfo[varNum][3]
             dimVary = self.rvarsinfo[varNum][4]
-        if (numDims < 1):
+        if numDims < 1:
             return values
         else:
             for x in range(0, numDims):
-                if (zVar):
+                if zVar:
                     values = values * dimSizes[x]
                 else:
-                    if (dimVary[x] != 0):
+                    if dimVary[x] != 0:
                         values = values * dimSizes[x]
             return values
 
-    def _read_offset_value(self, f, offset, size):
-        '''
+    def _read_offset_value(self, f: io.BufferedWriter, offset: int, size: int) -> int:
+        """
         Reads an integer value from file "f" at location "offset".
-        '''
+        """
         f.seek(offset, 0)
-        if (size == 8):
-            return int.from_bytes(f.read(8), 'big', signed=True)
+        if size == 8:
+            return int.from_bytes(f.read(8), "big", signed=True)
         else:
-            return int.from_bytes(f.read(4), 'big', signed=True)
+            return int.from_bytes(f.read(4), "big", signed=True)
 
-    def _update_offset_value(self, f, offset, size, value):
-        '''
+    def _update_offset_value(self, f: io.BufferedWriter, offset: int, size: int, value: Any) -> None:
+        """
         Writes "value" into location "offset" in file "f".
-        '''
+        """
         f.seek(offset, 0)
-        if (size == 8):
-            f.write(struct.pack('>q', value))
+        if size == 8:
+            f.write(struct.pack(">q", value))
         else:
-            f.write(struct.pack('>i', value))
+            f.write(struct.pack(">i", value))
 
-    def _update_aedr_link(self, f, attrNum, zVar, varNum, offset):
-        '''
+    def _update_aedr_link(self, f: io.BufferedWriter, attrNum: int, zVar: bool, varNum: int, offset: int) -> None:
+        """
         Updates variable aedr links
 
-        Parameters:
-            f : file
-                The open CDF file
-            attrNum : int
-                The number of the attribute to change
-            zVar : bool
-                True if we are updating a z variable attribute
-            varNum : int
-                The variable number associated with this aedr
-            offset : int
-                The offset in the file to the AEDR
-        Returns: None
-
-        '''
+        Parameters
+        ----------
+        f : file
+            The open CDF file
+        attrNum : int
+            The number of the attribute to change
+        zVar : bool
+            True if we are updating a z variable attribute
+        varNum : int
+            The variable number associated with this aedr
+        offset : int
+            The offset in the file to the AEDR
+        """
 
         # The offset to this AEDR's ADR
         adr_offset = self.attrsinfo[attrNum][2]
 
         # Get the number of entries
         if zVar:
             f.seek(adr_offset + 56, 0)
             # ADR's NzEntries
-            entries = int.from_bytes(f.read(4), 'big', signed=True)
+            entries = int.from_bytes(f.read(4), "big", signed=True)
             # ADR's MAXzEntry
-            maxEntry = int.from_bytes(f.read(4), 'big', signed=True)
+            maxEntry = int.from_bytes(f.read(4), "big", signed=True)
         else:
             f.seek(adr_offset + 36, 0)
             # ADR's NgrEntries
-            entries = int.from_bytes(f.read(4), 'big', signed=True)
+            entries = int.from_bytes(f.read(4), "big", signed=True)
             # ADR's MAXgrEntry
-            maxEntry = int.from_bytes(f.read(4), 'big', signed=True)
+            maxEntry = int.from_bytes(f.read(4), "big", signed=True)
 
-        if (entries == 0):
+        if entries == 0:
             # If this is the first entry, update the ADR to reflect
             if zVar:
                 # AzEDRhead
                 self._update_offset_value(f, adr_offset + 48, 8, offset)
                 # NzEntries
                 self._update_offset_value(f, adr_offset + 56, 4, 1)
                 # MaxzEntry
@@ -2447,153 +2448,150 @@
                 # NgrEntries
                 self._update_offset_value(f, adr_offset + 36, 4, 1)
                 # MaxgrEntry
                 self._update_offset_value(f, adr_offset + 40, 4, varNum)
         else:
             if zVar:
                 f.seek(adr_offset + 48, 0)
-                head = int.from_bytes(f.read(8), 'big', signed=True)
+                head = int.from_bytes(f.read(8), "big", signed=True)
             else:
                 f.seek(adr_offset + 20, 0)
-                head = int.from_bytes(f.read(8), 'big', signed=True)
+                head = int.from_bytes(f.read(8), "big", signed=True)
             aedr = head
             previous_aedr = head
             done = False
             # For each entry, re-adjust file offsets if needed
             for _ in range(0, entries):
                 f.seek(aedr + 28, 0)
                 # Get variable number for entry
-                num = int.from_bytes(f.read(4), 'big', signed=True)
-                if (num > varNum):
+                num = int.from_bytes(f.read(4), "big", signed=True)
+                if num > varNum:
                     # insert an aedr to the chain
                     # AEDRnext
                     self._update_offset_value(f, previous_aedr + 12, 8, offset)
                     # AEDRnext
                     self._update_offset_value(f, offset + 12, 8, aedr)
                     done = True
                     break
                 else:
                     # move to the next aedr in chain
                     f.seek(aedr + 12, 0)
                     previous_aedr = aedr
-                    aedr = int.from_bytes(f.read(8), 'big', signed=True)
+                    aedr = int.from_bytes(f.read(8), "big", signed=True)
 
             # If no link was made, update the last found aedr
             if not done:
                 self._update_offset_value(f, previous_aedr + 12, 8, offset)
 
             if zVar:
                 self._update_offset_value(f, adr_offset + 56, 4, entries + 1)
-                if (maxEntry < varNum):
+                if maxEntry < varNum:
                     self._update_offset_value(f, adr_offset + 60, 4, varNum)
             else:
                 self._update_offset_value(f, adr_offset + 36, 4, entries + 1)
-                if (maxEntry < varNum):
+                if maxEntry < varNum:
                     self._update_offset_value(f, adr_offset + 40, 4, varNum)
 
     @staticmethod
-    def _set_bit(value, bit):
+    def _set_bit(value: int, bit: int) -> int:
         return value | (1 << bit)
 
     @staticmethod
-    def _clear_bit(value, bit):
+    def _clear_bit(value: int, bit: int) -> int:
         return value & ~(1 << bit)
 
     @staticmethod
-    def _checklistofstrs(obj):
+    def _checklistofstrs(obj: Any) -> bool:
         return bool(obj) and all(isinstance(elem, str) for elem in obj)
 
     @staticmethod
-    def _checklistofNums(obj):
-        if hasattr(obj, '__len__'):
-            return bool(obj) and all(isinstance(elem, numbers.Number)
-                                     for elem in obj)
+    def _checklistofNums(obj: Any) -> bool:
+        if hasattr(obj, "__len__"):
+            return bool(obj) and all(isinstance(elem, numbers.Number) for elem in obj)
         else:
             return isinstance(obj, numbers.Number)
 
-    def _md5_compute(self, f):
-        '''
+    def _md5_compute(self, f: io.BufferedWriter) -> bytes:
+        """
         Computes the checksum of the file
-        '''
+        """
         md5 = hashlib.md5()
         block_size = 16384
         f.seek(0, 2)
         remaining = f.tell()
         f.seek(0)
 
-        while (remaining > block_size):
+        while remaining > block_size:
             data = f.read(block_size)
             remaining = remaining - block_size
             md5.update(data)
 
         if remaining > 0:
             data = f.read(remaining)
             md5.update(data)
 
         return md5.digest()
 
     @staticmethod
-    def _make_blocks(records):
-        '''
+    def _make_blocks(records) -> List[Tuple[int, int]]:  # type: ignore[no-untyped-def]
+        """
         Organizes the physical records into blocks in a list by
         placing consecutive physical records into a single block, so
         lesser VXRs will be created.
           [[start_rec1,end_rec1,data_1], [start_rec2,enc_rec2,data_2], ...]
 
-        Parameters:
-            records: list
-                A list of records that there is data for
+        Parameters
+        ----------
+        records: list
+            A list of records that there is data for
 
-        Returns:
-            sparse_blocks: list of list
-                A list of ranges we have physical values for.
+        Returns
+        -------
+        sparse_blocks: list of list
+            A list of ranges we have physical values for.
 
         Example:
             Input: [1,2,3,4,10,11,12,13,50,51,52,53]
             Output: [[1,4],[10,13],[50,53]]
-        '''
+        """
 
         sparse_blocks = []
         total = len(records)
-        if (total == 0):
+        if total == 0:
             return []
 
         x = 0
-        while (x < total):
+        while x < total:
             recstart = records[x]
             y = x
             recnum = recstart
 
             # Find the location in the records before the next gap
             # Call this value "y"
-            while ((y + 1) < total):
+            while (y + 1) < total:
                 y = y + 1
                 nextnum = records[y]
                 diff = nextnum - recnum
-                if (diff == 1):
+                if diff == 1:
                     recnum = nextnum
                 else:
                     y = y - 1
                     break
 
-            # Put the values of the records into "ablock", append to sparse_blocks
-            ablock = []
-            ablock.append(recstart)
-            if ((y + 1) == total):
+            if (y + 1) == total:
                 recend = records[total - 1]
             else:
                 recend = records[y]
             x = y + 1
-            ablock.append(recend)
-            sparse_blocks.append(ablock)
+            sparse_blocks.append((recstart, recend))
 
         return sparse_blocks
 
-    def _make_sparse_blocks(self, variable, records, data):
-        '''
+    def _make_sparse_blocks(self, variable, records, data: List[Tuple[int, int, np.ndarray]]):  # type: ignore[no-untyped-def]
+        """
         Handles the data for the variable with sparse records.
         Organizes the physical record numbers into blocks in a list:
           [[start_rec1,end_rec1,data_1], [start_rec2,enc_rec2,data_2], ...]
         Place consecutive physical records into a single block
 
         If all records are physical, this calls _make_sparse_blocks_with_physical
 
@@ -2614,176 +2612,151 @@
                 data or embedded virtual data (returned from call to
                 varget('variable') for a sparse variable)
 
         Returns:
             sparse_blocks: list
                 A list of sparse records/data in the form
                 [[start_rec1,end_rec1,data_1], [start_rec2,enc_rec2,data_2], ...]
-        '''
+        """
 
-        if (isinstance(data, dict)):
+        if isinstance(data, dict):
             try:
-                data = data['Data']
+                data = data["Data"]
             except Exception:
-                warnings.warn('Unknown dictionary.... Skip')
+                warnings.warn("Unknown dictionary.... Skip")
                 return None
-        if (isinstance(data, np.ndarray)):
-            if (len(records) == len(data)):
+        if isinstance(data, np.ndarray):
+            if len(records) == len(data):
                 # All are physical data
-                return self._make_sparse_blocks_with_physical(variable, records,
-                                                              data)
-            elif (len(records) < len(data)):
+                return self._make_sparse_blocks_with_physical(variable, records, data)
+            elif len(records) < len(data):
                 # There are some virtual data
-                return self._make_sparse_blocks_with_virtual(variable, records,
-                                                             data)
+                return self._make_sparse_blocks_with_virtual(variable, records, data)
             else:
-                warnings.warn('Invalid sparse data... ',
-                              'Less data than the specified records... Skip')
-        elif (isinstance(data, bytes)):
+                warnings.warn("Invalid sparse data... " "Less data than the specified records... Skip")
+        elif isinstance(data, bytes):
             record_length = len(records)
-            for z in range(0, variable['Num_Dims']):
-                record_length = record_length * variable['Dim_Sizes'][z]
-            if (record_length == len(data)):
+            for z in range(0, variable["Num_Dims"]):
+                record_length = record_length * variable["Dim_Sizes"][z]
+            if record_length == len(data):
                 # All are physical data
-                return self._make_sparse_blocks_with_physical(variable, records,
-                                                              data)
-            elif (record_length < len(data)):
+                return self._make_sparse_blocks_with_physical(variable, records, data)
+            elif record_length < len(data):
                 # There are some virtual data
-                return self._make_sparse_blocks_with_virtual(variable, records,
-                                                             data)
+                return self._make_sparse_blocks_with_virtual(variable, records, data)
             else:
-                warnings.warn('Invalid sparse data... ',
-                              'Less data than the specified records... Skip')
-        elif (isinstance(data, list)):
-            if (isinstance(data[0], list)):
+                warnings.warn("Invalid sparse data... " "Less data than the specified records... Skip")
+        elif isinstance(data, list):
+            if isinstance(data[0], list):
                 if not (all(isinstance(el, str) for el in data[0])):
-                    print('Can not handle list data.... ',
-                          'Only support list of str... Skip')
+                    print("Can not handle list data.... ", "Only support list of str... Skip")
                     return
             else:
                 if not (all(isinstance(el, str) for el in data)):
-                    print('Can not handle list data.... ',
-                          'Only support list of str... Skip')
+                    print("Can not handle list data.... ", "Only support list of str... Skip")
                     return
             record_length = len(records)
             # for z in range(0, variable['Num_Dims']):
             #    record_length = record_length * variable['Dim_Sizes'][z]
-            if (record_length == len(data)):
+            if record_length == len(data):
                 # All are physical data
-                return self._make_sparse_blocks_with_physical(variable, records,
-                                                              data)
-            elif (record_length < len(data)):
+                return self._make_sparse_blocks_with_physical(variable, records, data)
+            elif record_length < len(data):
                 # There are some virtual data
-                return self._make_sparse_blocks_with_virtual(variable, records,
-                                                             data)
+                return self._make_sparse_blocks_with_virtual(variable, records, data)
             else:
-                print('Invalid sparse data... ',
-                      'Less data than the specified records... Skip')
+                print("Invalid sparse data... ", "Less data than the specified records... Skip")
         else:
-            print('Invalid sparse data... ',
-                  'Less data than the specified records... Skip')
+            print("Invalid sparse data... ", "Less data than the specified records... Skip")
         return
 
-    def _make_sparse_blocks_with_virtual(self, variable, records, data):
-        '''
+    def _make_sparse_blocks_with_virtual(self, variable, records, data) -> List[Tuple[int, int, np.ndarray]]:  # type: ignore[no-untyped-def]
+        """
         Handles the data for the variable with sparse records.
         Organizes the physical record numbers into blocks in a list:
           [[start_rec1,end_rec1,data_1], [start_rec2,enc_rec2,data_2], ...]
         Place consecutive physical records into a single block
 
         Parameters:
             variable: dict
                 the variable, returned from varinq('variable', expand=True)
             records: list
                 a list of physical records
             data: varies
                 bytes array, numpy.ndarray or list of str form with vitual data
                 embedded, returned from varget('variable') call
-        '''
+        """
 
         # Gather the ranges for which we have physical data
         sparse_blocks = self._make_blocks(records)
 
         sparse_data = []
-        if (isinstance(data, np.ndarray)):
+        if isinstance(data, np.ndarray):
             for sblock in sparse_blocks:
                 # each block in this list: [starting_rec#, ending_rec#, data]
-                asparse = []
-                asparse.append(sblock[0])
-                asparse.append(sblock[1])
                 starting = sblock[0]
                 ending = sblock[1] + 1
-                asparse.append(data[starting:ending])
-                sparse_data.append(asparse)
+                sparse_data.append((sblock[0], sblock[1], data[starting:ending]))
             return sparse_data
-        elif (isinstance(data, bytes)):
+        elif isinstance(data, bytes):
             y = 1
-            for z in range(0, variable['Num_Dims']):
-                y = y * variable['Dim_Sizes'][z]
-            y = y * self._datatype_size(variable['Data_Type'], variable['Num_Elements'])
+            for z in range(0, variable["Num_Dims"]):
+                y = y * variable["Dim_Sizes"][z]
+            y = y * self._datatype_size(variable["Data_Type"], variable["Num_Elements"])
             for x in sparse_blocks:
                 # each block in this list: [starting_rec#, ending_rec#, data]
-                asparse = []
-                asparse.append(sblock[0])
-                asparse.append(sblock[1])
                 starting = sblock[0] * y
                 ending = (sblock[1] + 1) * y
-                asparse.append(data[starting:ending])
-                sparse_data.append(asparse)
+                sparse_data.append((sblock[0], sblock[1], np.array(data[starting:ending])))
             return sparse_data
-        elif (isinstance(data, list)):
+        elif isinstance(data, list):
             for x in sparse_blocks:
                 # each block in this list: [starting_rec#, ending_rec#, data]
                 asparse = []
                 asparse.append(sblock[0])
                 asparse.append(sblock[1])
-                records = sparse_blocks[x][1] - sparse_blocks[x][0] + 1
+                records = x[1] - x[0] + 1
                 datax = []
                 ist = sblock[0]
                 for z in range(0, records):
                     datax.append(data[ist + z])
-                asparse.append(datax)
-                sparse_data.append(asparse)
+                sparse_data.append((sblock[0], sblock[1], np.array(datax)))
             return sparse_data
         else:
-            print('Can not handle data... Skip')
+            print("Can not handle data... Skip")
             return None
 
-    def _make_sparse_blocks_with_physical(self, variable, records, data):
+    def _make_sparse_blocks_with_physical(self, variable, records, data) -> List[Tuple[int, int, np.ndarray]]:  # type: ignore[no-untyped-def]
         # All records are physical... just a single block
         #   [[0,end_rec,data]]
 
         # Determine if z variable
-        if (variable['Var_Type'].lower() == 'zvariable'):
+        if variable["Var_Type"].lower() == "zvariable":
             zVar = True
         else:
             zVar = False
 
         # Determine dimension information
+        numDims = len(variable["Dim_Sizes"])
         if zVar:
-            numDims = len(variable['Dim_Sizes'])
             numValues = 1
             for x in range(0, numDims):
-                numValues = numValues * variable['Dim_Sizes'][x]
+                numValues = numValues * variable["Dim_Sizes"][x]
         else:
             for x in range(0, numDims):
-                if (variable['Dim_Vary'][x] != 0):
-                    numValues = numValues * variable['Dim_Sizes'][x]
+                if variable["Dim_Vary"][x] != 0:
+                    numValues = numValues * variable["Dim_Sizes"][x]
 
         # Determine blocks
         sparse_blocks = self._make_blocks(records)
 
         # Create a list in the form of [[0,100, [data]], ...]
         sparse_data = []
         recStart = 0
         for sblock in sparse_blocks:
-            asparse = []
             recs = sblock
-            asparse.append(recs[0])
-            asparse.append(recs[1])
             totalRecs = recs[1] - recs[0] + 1
             recEnd = recStart + totalRecs
-            asparse.append(data[recStart:recEnd])
-            sparse_data.append(asparse)
+            sparse_data.append((recs[0], recs[1], data[recStart:recEnd]))
             recStart = recStart + totalRecs
 
         return sparse_data
```

### Comparing `cdflib-0.4.9/cdflib/epochs.py` & `cdflib-1.0.0/cdflib/epochs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,65 @@
-"""
-##########
-CDF Epochs
-##########
-
-Importing cdflib also imports the module CDFepoch, which handles
-CDF-based epochs.
-
-The following functions can be used to convert back and forth between
-different ways to display the date.
-
-You can call these functions like so::
-
-    import cdflib
-    cdf_file = cdflib.cdfepoch.compute_epoch([2017,1,1,1,1,1,111])
-
-There are three (3) epoch data types in CDF: CDF_EPOCH, CDF_EPOCH16 and
-CDF_TIME_TT2000.
-
-- CDF_EPOCH is milliseconds since Year 0.
-- CDF_EPOCH16 is picoseconds since Year 0.
-- CDF_TIME_TT2000 (TT2000 as short) is nanoseconds since J2000 with
-  leap seconds.
-
-CDF_EPOCH is a single double(as float in Python),
-CDF_EPOCH16 is 2-doubles (as complex in Python),
-and TT2000 is 8-byte integer (as int in Python).
-In Numpy, they are np.float64, np.complex128 and np.int64, respectively.
-All these epoch values can come from from CDF.varget function.
-
-@author: Michael Liu
-"""
 import csv
 import datetime
 import math
-import numbers
 import os
 import re
-from typing import List, Sequence, Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
+import numpy.typing as npt
+
+from cdflib.utils import _squeeze_or_scalar_complex, _squeeze_or_scalar_real
+
+LEAPSEC_FILE = os.path.join(os.path.dirname(os.path.realpath(__file__)), "CDFLeapSeconds.txt")
+
+epochs_type = Union[str, List[float], List[int], List[complex], Tuple[float, ...], Tuple[int, ...], Tuple[complex, ...], np.ndarray]
+
+
+epoch_scalar_types = Union[int, np.int64, float, np.float64, complex, np.complex128]
+epoch_list_types = Union[List[int], List[np.int64], List[float], List[np.float64], List[complex], List[np.complex128]]
+epoch_types = Union[epoch_scalar_types, epoch_list_types, npt.NDArray]
 
-LEAPSEC_FILE = os.path.join(os.path.dirname(os.path.realpath(__file__)),
-                            'CDFLeapSeconds.txt')
+encoded_type = Union[str, List[str]]
 
+cdf_epoch_type = Union[float, np.float64, List[float], npt.NDArray[np.float64]]
+cdf_epoch16_type = Union[complex, np.complex128, List[complex], npt.NDArray[np.complex128]]
+cdf_tt2000_type = Union[int, np.int64, List[int], npt.NDArray[np.int64]]
 
-class CDFepoch(object):
+
+class CDFepoch:
     """
-    Epoch class.
+    Convert between CDF-based epochs, np.datetime64, and Unix time.
+
+    There are three (3) epoch data types in CDF:
+        1. CDF_EPOCH is milliseconds since Year 0 represented as a
+        single double (float in Python),
+        2. CDF_EPOCH16 is picoseconds since Year 0 represented as
+        2-doubles (complex in Python), and
+        3. CDF_TIME_TT2000 (TT2000 as short) is nanoseconds since J2000 with
+        leap seconds, represented by an 8-byte integer (int in Python).
+
+    In Numpy, they are np.float64, np.complex128 and np.int64, respectively.
+    All these epoch values can come from from CDF.varget function.
+
+
+    Example
+    -------
+    >>> import cdflib
+    # Convert to an epoch
+    >>> epoch = cdflib.cdfepoch.compute_epoch([2017,1,1,1,1,1,111])
+    # Convert from an epoch
+    >>> time = cdflib.cdfepoch.to_datetime(epoch)  # Or pass epochs via CDF.varget.
     """
 
     version = 3
     release = 7
     increment = 0
 
-    month_Token = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
-                   'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
+    month_Token = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]
 
     JulianDateJ2000_12h = 2451545
     J2000Since0AD12h = 730485
     J2000Since0AD12hSec = 63113904000.0
     J2000Since0AD12hMilsec = 63113904000000.0
     J2000LeapSeconds = 32.0
     dT = 32.184
@@ -76,358 +77,312 @@
     JDY22920411 = 2558297
     DEFAULT_TT2000_PADVALUE = int(-9223372036854775807)
     FILLED_TT2000_VALUE = int(-9223372036854775808)
     NERA1 = 14
 
     LTS = []
     with open(LEAPSEC_FILE) as lsfile:
-        lsreader = csv.reader(lsfile, delimiter=' ')
+        lsreader = csv.reader(lsfile, delimiter=" ")
         for csv_row in lsreader:
             if csv_row[0] == ";":
                 continue
-            csv_row = list(filter(('').__ne__, csv_row))
+            csv_row = list(filter(("").__ne__, csv_row))
 
             row: List[Union[int, float]] = []
             for r in csv_row[:3]:
                 row.append(int(r))
             for r in csv_row[3:6]:
                 row.append(float(r))
             LTS.append(row)
 
     NDAT = len(LTS)
 
-    NST = None
+    NST: Optional[List[int]] = None
     currentDay = -1
     currentJDay = -1
-    currentLeapSeconds = -1
+    currentLeapSeconds: float = -1
 
     @staticmethod
-    def encode(epochs, iso_8601: bool = True):  # @NoSelf
+    def encode(epochs: epoch_types, iso_8601: bool = True) -> encoded_type:
         """
-        Encodes the epoch(s) into UTC string(s).
+        Converts one or more epochs into UTC strings. The input epoch
+        format is deduced from the argument type.
+
+        Parameters
+        ----------
+        epochs: int, float, list, complex
+            One or more ECD epochs in one of three formats:
+            1. CDF_EPOCH: The input should be either a float or list of floats
+            (in numpy, a np.float64 or a np.ndarray of np.float64)
+            2. CDF_EPOCH16: The input should be either a complex or list of
+            complex(in numpy, a np.complex128 or a np.ndarray of np.complex128)
+            3. TT2000: The input should be either a int or list of ints
+            (in numpy, a np.int64 or a np.ndarray of np.int64)
+
+        iso_8601: bool
+                The return time format. If ISO 8601 is True, the format is,
+                for example, 2008-02-02T06:08:10.10.012014016, otherwise
+                the format is 02-Feb-2008 06:08:10.012.014.016.
 
-        For CDF_EPOCH:
-                The input should be either a float or list of floats
-                (in numpy, a np.float64 or a np.ndarray of np.float64)
-                Each epoch is encoded, by default to a ISO 8601 form:
-                2004-05-13T15:08:11.022
-                Or, if iso_8601 is set to False,
-                13-May-2004 15:08:11.022
-        For CDF_EPOCH16:
-                The input should be either a complex or list of
-                complex(in numpy, a np.complex128 or a np.ndarray of np.complex128)
-                Each epoch is encoded, by default to a ISO 8601 form:
-                2004-05-13T15:08:11.022033044055
-                Or, if iso_8601 is set to False,
-                13-May-2004 15:08:11.022.033.044.055
-        For TT2000:
-                The input should be either a int or list of ints
-                (in numpy, a np.int64 or a np.ndarray of np.int64)
-                Each epoch is encoded, by default to a ISO 8601 form:
-                2008-02-02T06:08:10.10.012014016
-                Or, if iso_8601 is set to False,
-                02-Feb-2008 06:08:10.012.014.016
         """
-        if isinstance(epochs, (int, np.int64)):
+        epochs = np.array(epochs)
+        if epochs.dtype == np.int64:
             return CDFepoch.encode_tt2000(epochs, iso_8601)
-        elif isinstance(epochs, (float, np.float64)):
+        elif epochs.dtype == np.float64:
             return CDFepoch.encode_epoch(epochs, iso_8601)
-        elif isinstance(epochs, (complex, np.complex128)):
+        elif epochs.dtype == np.complex128:
             return CDFepoch.encode_epoch16(epochs, iso_8601)
-        elif isinstance(epochs, (list, np.ndarray)):
-            if isinstance(epochs[0], (int, np.int64)):
-                return CDFepoch.encode_tt2000(epochs, iso_8601)
-            elif isinstance(epochs[0], (float, np.float64)):
-                return CDFepoch.encode_epoch(epochs, iso_8601)
-            elif isinstance(epochs[0], (complex, np.complex128)):
-                return CDFepoch.encode_epoch16(epochs, iso_8601)
-
-        raise TypeError('Not sure how to handle type {}'.format(type(epochs)))
-
-    @staticmethod
-    def breakdown(epochs, to_np: bool = False):
-        if isinstance(epochs, (list, tuple, np.ndarray)):
-            if isinstance(epochs, np.ndarray) and len(epochs.shape) > 1:
-                epochs = np.squeeze(epochs)
-            item = epochs[0]
-        else:
-            item = epochs
-
-        if isinstance(item, (int, np.int64)):
-            return CDFepoch.breakdown_tt2000(epochs, to_np)
-        elif isinstance(item, (float, np.float64)):
-            return CDFepoch.breakdown_epoch(epochs, to_np)
-        elif isinstance(item, (complex, np.complex128)):
-            return CDFepoch.breakdown_epoch16(epochs, to_np)
-        elif isinstance(item, np.ndarray):
-            if item.dtype.type == np.int64:
-                return CDFepoch.breakdown_tt2000(epochs, to_np)
-            elif item.dtype.type == np.float64:
-                return CDFepoch.breakdown_epoch(epochs, to_np)
-            elif item.dtype.type == np.complex128:
-                return CDFepoch.breakdown_epoch16(epochs, to_np)
-        else:
-            raise TypeError('Not sure how to handle type {}'.format(type(epochs)))
-
-    @staticmethod
-    def _compose_date(years, months, days,
-                      hours=None, minutes=None, seconds=None,
-                      milliseconds=None, microseconds=None, nanoseconds=None,
-                      *extras):
+        else:
+            raise TypeError(f"Not sure how to handle type {epochs.dtype}")
+
+    @staticmethod
+    def breakdown(epochs: epoch_types) -> np.ndarray:
+        """
+        Returns
+        -------
+        np.ndarray
+            1D if scalar input, 2D otherwise.
+        """
+        epochs = np.array(epochs)
+        if epochs.dtype.type == np.int64:
+            return CDFepoch.breakdown_tt2000(epochs)
+        elif epochs.dtype.type == np.float64:
+            return CDFepoch.breakdown_epoch(epochs)
+        elif epochs.dtype.type == np.complex128:
+            return CDFepoch.breakdown_epoch16(epochs)
+        else:
+            raise TypeError("Not sure how to handle type {}".format(type(epochs)))
+
+    @staticmethod
+    def _compose_date(
+        years: npt.NDArray,
+        months: npt.NDArray,
+        days: npt.NDArray,
+        hours: Optional[npt.NDArray] = None,
+        minutes: Optional[npt.NDArray] = None,
+        seconds: Optional[npt.NDArray] = None,
+        milliseconds: Optional[npt.NDArray] = None,
+        microseconds: Optional[npt.NDArray] = None,
+        nanoseconds: Optional[npt.NDArray] = None,
+    ) -> npt.NDArray[np.datetime64]:
         """
         Take date components and return a numpy datetime array.
         """
         years = np.asarray(years) - 1970
         months = np.asarray(months) - 1
         days = np.asarray(days) - 1
-        types = ('<M8[Y]', '<m8[M]', '<m8[D]', '<m8[h]',
-                 '<m8[m]', '<m8[s]', '<m8[ms]', '<m8[us]', '<m8[ns]')
-        vals = (years, months, days, hours, minutes, seconds,
-                milliseconds, microseconds, nanoseconds)
+        types = ("<M8[Y]", "<m8[M]", "<m8[D]", "<m8[h]", "<m8[m]", "<m8[s]", "<m8[ms]", "<m8[us]", "<m8[ns]")
+        vals = (v for v in (years, months, days, hours, minutes, seconds, milliseconds, microseconds, nanoseconds) if v is not None)
 
-        return sum(np.asarray(v, dtype=t) for t, v in zip(types, vals)
-                   if v is not None)
+        arrays: List[npt.NDArray[np.datetime64]] = [np.array(v, dtype=t) for t, v in zip(types, vals)]
+        return np.array(sum(arrays))
 
     @classmethod
-    def to_datetime(cls, cdf_time: Union[int, Sequence[int]],
-                    to_np: bool = False) -> List[datetime.datetime]:
+    def to_datetime(cls, cdf_time: epoch_types) -> npt.NDArray[np.datetime64]:
         """
-        Encodes the epoch(s) into Numpy datetime64.  Precision is only
-        kept to the nearest microsecond.
-
-        Possible len() from breakdown for each time are in range 6..9
-
-        If to_np is True, then the values will be returned in a numpy array.
+        Converts CDF epoch argument to numpy.datetime64. This method
+        converts a scalar, or array-like. Precision is only kept to the
+        nearest microsecond.
         """
-        times = cls.breakdown(cdf_time, to_np=True)
+        times = cls.breakdown(cdf_time)
         times = np.atleast_2d(times)
-        times = cls._compose_date(*times.T).astype('datetime64[us]')
-
-        return times if to_np else times.tolist()
+        return cls._compose_date(*times.T[:9]).astype("datetime64[us]")
 
     @staticmethod
-    def unixtime(cdf_time, to_np: bool = False):  # @NoSelf
+    def unixtime(cdf_time: npt.ArrayLike) -> Union[float, npt.NDArray]:
         """
-        Encodes the epoch(s) into seconds after 1970-01-01.  Precision is only
-        kept to the nearest microsecond.
-
-        If to_np is True, then the values will be returned in a numpy array.
+        Converts CDF epoch argument into seconds after 1970-01-01. This method
+        converts a scalar, or array-like. Precision is only kept to the
+        nearest microsecond.
         """
-        import datetime
-        time_list = CDFepoch.breakdown(cdf_time, to_np=False)
-
-        # Check if only one time was input into unixtime.
-        # If so, turn the output of breakdown into a list for this function to work
-        if hasattr(cdf_time, '__len__'):
-            if len(cdf_time) == 1:
-                time_list = [time_list]
-        else:
-            time_list = [time_list]
+        cdf_time = np.atleast_1d(cdf_time)
+        time_list = np.atleast_2d(CDFepoch.breakdown(cdf_time))
 
         unixtime = []
         utc = datetime.timezone(datetime.timedelta())
         for t in time_list:
             date: List[int] = [0] * 7
             for i in range(0, len(t)):
                 if i > 7:
                     continue
                 elif i == 6:
                     date[i] = 1000 * t[i]
                 elif i == 7:
                     date[i - 1] += t[i]
                 else:
                     date[i] = t[i]
-            unixtime.append(datetime.datetime(date[0], date[1], date[2], date[3], date[4], date[5], date[6], tzinfo=utc).timestamp())
-        return np.array(unixtime) if to_np else unixtime
+            unixtime.append(
+                datetime.datetime(date[0], date[1], date[2], date[3], date[4], date[5], date[6], tzinfo=utc).timestamp()
+            )
+        return _squeeze_or_scalar_real(unixtime)
 
     @staticmethod
-    def compute(datetimes, to_np: bool = False):  # @NoSelf
+    def compute(datetimes: npt.ArrayLike) -> Union[float, complex, npt.NDArray]:
         """
         Computes the provided date/time components into CDF epoch value(s).
 
         For CDF_EPOCH:
-                For computing into CDF_EPOCH value, each date/time elements should
-                have exactly seven (7) components, as year, month, day, hour, minute,
-                second and millisecond, in a list. For example:
-                [[2017,1,1,1,1,1,111],[2017,2,2,2,2,2,222]]
-                Or, call function compute_epoch directly, instead, with at least three
-                (3) first (up to seven) components. The last component, if
-                not the 7th, can be a float that can have a fraction of the unit.
+            For computing into CDF_EPOCH value, each date/time elements should
+            have exactly seven (7) components, as year, month, day, hour, minute,
+            second and millisecond, in a list. For example:
+            [[2017,1,1,1,1,1,111],[2017,2,2,2,2,2,222]]
+            Or, call function compute_epoch directly, instead, with at least three
+            (3) first (up to seven) components. The last component, if
+            not the 7th, can be a float that can have a fraction of the unit.
 
         For CDF_EPOCH16:
-                They should have exactly ten (10) components, as year,
-                month, day, hour, minute, second, millisecond, microsecond, nanosecond
-                and picosecond, in a list. For example:
-                [[2017,1,1,1,1,1,123,456,789,999],[2017,2,2,2,2,2,987,654,321,999]]
-                Or, call function compute_epoch directly, instead, with at least three
-                (3) first (up to ten) components. The last component, if
-                not the 10th, can be a float that can have a fraction of the unit.
+            They should have exactly ten (10) components, as year,
+            month, day, hour, minute, second, millisecond, microsecond, nanosecond
+            and picosecond, in a list. For example:
+            [[2017,1,1,1,1,1,123,456,789,999],[2017,2,2,2,2,2,987,654,321,999]]
+            Or, call function compute_epoch directly, instead, with at least three
+            (3) first (up to ten) components. The last component, if
+            not the 10th, can be a float that can have a fraction of the unit.
 
         For TT2000:
-                Each TT2000 typed date/time should have exactly nine (9) components, as
-                year, month, day, hour, minute, second, millisecond, microsecond,
-                and nanosecond, in a list.  For example:
-                [[2017,1,1,1,1,1,123,456,789],[2017,2,2,2,2,2,987,654,321]]
-                Or, call function compute_tt2000 directly, instead, with at least three
-                (3) first (up to nine) components. The last component, if
-                not the 9th, can be a float that can have a fraction of the unit.
-
-        Specify to_np to True, if the result should be in numpy class.
+            Each TT2000 typed date/time should have exactly nine (9) components, as
+            year, month, day, hour, minute, second, millisecond, microsecond,
+            and nanosecond, in a list.  For example:
+            [[2017,1,1,1,1,1,123,456,789],[2017,2,2,2,2,2,987,654,321]]
+            Or, call function compute_tt2000 directly, instead, with at least three
+            (3) first (up to nine) components. The last component, if
+            not the 9th, can be a float that can have a fraction of the unit.
         """
 
         if not isinstance(datetimes, (list, tuple, np.ndarray)):
-            raise TypeError('datetime must be in list form')
+            raise TypeError("datetime must be in list form")
 
-        if isinstance(datetimes[0], numbers.Number):
-            items = len(datetimes)
-        elif isinstance(datetimes[0], (list, tuple, np.ndarray)):
-            items = len(datetimes[0])
-        else:
-            raise TypeError('Not sure how to handle type {}'.format(type(datetimes[0])))
+        datetimes = np.atleast_2d(datetimes)
+        items = datetimes.shape[1]
 
-        if (items == 7):
-            return CDFepoch.compute_epoch(datetimes, to_np)
-        elif (items == 10):
-            return CDFepoch.compute_epoch16(datetimes, to_np)
-        elif (items == 9):
-            return CDFepoch.compute_tt2000(datetimes, to_np)
+        if items == 7:
+            return _squeeze_or_scalar_real(CDFepoch.compute_epoch(datetimes))
+        elif items == 10:
+            return _squeeze_or_scalar_complex(CDFepoch.compute_epoch16(datetimes))
+        elif items == 9:
+            return _squeeze_or_scalar_real(CDFepoch.compute_tt2000(datetimes))
         else:
-            raise TypeError('Unknown input')
+            raise TypeError("Unknown input")
 
     @staticmethod
-    def findepochrange(epochs, starttime=None, endtime=None):  # @NoSelf
+    def findepochrange(
+        epochs: epochs_type, starttime: Optional[epoch_types] = None, endtime: Optional[epoch_types] = None
+    ) -> np.ndarray:
         """
         Finds the record range within the start and end time from values
         of a CDF epoch data type. It returns a list of record numbers.
         If the start time is not provided, then it is
         assumed to be the minimum possible value. If the end time is not
         provided, then the maximum possible value is assumed. The epoch is
         assumed to be in the chronological order. The start and end times
         should have the proper number of date/time components, corresponding
         to the epoch's data type.
 
         The start/end times should be in either be in epoch units, or in the list
         format described in "compute_epoch/epoch16/tt2000" section.
         """
-        if (isinstance(epochs, float) or isinstance(epochs, np.float64)):
-            return CDFepoch.epochrange_epoch(epochs, starttime, endtime)
-        elif (isinstance(epochs, int) or isinstance(epochs, np.int64)):
+        epochs = np.array(epochs)
+        if epochs.dtype == np.int64:
             return CDFepoch.epochrange_tt2000(epochs, starttime, endtime)
-        elif isinstance(epochs, (complex, np.complex128)):
+        elif epochs.dtype == np.float64:
+            return CDFepoch.epochrange_epoch(epochs, starttime, endtime)
+        elif epochs.dtype == np.complex128:
             return CDFepoch.epochrange_epoch16(epochs, starttime, endtime)
-        elif isinstance(epochs, (list, tuple, np.ndarray)):
-            if (isinstance(epochs[0], float) or
-                    isinstance(epochs[0], np.float64)):
-                return CDFepoch.epochrange_epoch(epochs, starttime, endtime)
-            elif (isinstance(epochs[0], int) or
-                  isinstance(epochs[0], np.int64)):
-                return CDFepoch.epochrange_tt2000(epochs, starttime, endtime)
-            elif (isinstance(epochs[0], complex) or
-                  isinstance(epochs[0], np.complex128)):
-                return CDFepoch.epochrange_epoch16(epochs, starttime, endtime)
-
-        raise TypeError('Bad input')
-
-    @staticmethod
-    def encode_tt2000(tt2000, iso_8601: bool = True):  # @NoSelf
-
-        if (isinstance(tt2000, int) or isinstance(tt2000, np.int64)):
-            new_tt2000 = [tt2000]
-        elif (isinstance(tt2000, list) or isinstance(tt2000, np.ndarray)):
-            new_tt2000 = tt2000
         else:
-            raise TypeError('Bad input')
+            raise TypeError("Bad input")
+
+    @staticmethod
+    def encode_tt2000(tt2000: cdf_tt2000_type, iso_8601: bool = True) -> encoded_type:
+        new_tt2000 = np.atleast_1d(tt2000)
 
         count = len(new_tt2000)
         encodeds = []
         for x in range(count):
             nanoSecSinceJ2000 = new_tt2000[x]
-            if (nanoSecSinceJ2000 == CDFepoch.FILLED_TT2000_VALUE):
+            if nanoSecSinceJ2000 == CDFepoch.FILLED_TT2000_VALUE:
                 if iso_8601:
-                    return '9999-12-31T23:59:59.999999999'
+                    return "9999-12-31T23:59:59.999999999"
                 else:
-                    return '31-Dec-9999 23:59:59.999.999.999'
-            if (nanoSecSinceJ2000 == CDFepoch.DEFAULT_TT2000_PADVALUE):
+                    return "31-Dec-9999 23:59:59.999.999.999"
+            if nanoSecSinceJ2000 == CDFepoch.DEFAULT_TT2000_PADVALUE:
                 if iso_8601:
-                    return '0000-01-01T00:00:00.000000000'
+                    return "0000-01-01T00:00:00.000000000"
                 else:
-                    return '01-Jan-0000 00:00:00.000.000.000'
+                    return "01-Jan-0000 00:00:00.000.000.000"
             datetime = CDFepoch.breakdown_tt2000(nanoSecSinceJ2000)
             ly = datetime[0]
             lm = datetime[1]
             ld = datetime[2]
             lh = datetime[3]
             ln = datetime[4]
             ls = datetime[5]
             ll = datetime[6]
             lu = datetime[7]
             la = datetime[8]
             if iso_8601:
                 # yyyy-mm-ddThh:mm:ss.mmmuuunnn
                 encoded = str(ly).zfill(4)
-                encoded += '-'
+                encoded += "-"
                 encoded += str(lm).zfill(2)
-                encoded += '-'
+                encoded += "-"
                 encoded += str(ld).zfill(2)
-                encoded += 'T'
+                encoded += "T"
                 encoded += str(lh).zfill(2)
-                encoded += ':'
+                encoded += ":"
                 encoded += str(ln).zfill(2)
-                encoded += ':'
+                encoded += ":"
                 encoded += str(ls).zfill(2)
-                encoded += '.'
+                encoded += "."
                 encoded += str(ll).zfill(3)
                 encoded += str(lu).zfill(3)
                 encoded += str(la).zfill(3)
             else:
                 # dd-mmm-yyyy hh:mm:ss.mmm.uuu.nnn
                 encoded = str(ld).zfill(2)
-                encoded += '-'
+                encoded += "-"
                 encoded += CDFepoch.month_Token[lm - 1]
-                encoded += '-'
+                encoded += "-"
                 encoded += str(ly).zfill(4)
-                encoded += ' '
+                encoded += " "
                 encoded += str(lh).zfill(2)
-                encoded += ':'
+                encoded += ":"
                 encoded += str(ln).zfill(2)
-                encoded += ':'
+                encoded += ":"
                 encoded += str(ls).zfill(2)
-                encoded += '.'
+                encoded += "."
                 encoded += str(ll).zfill(3)
-                encoded += '.'
+                encoded += "."
                 encoded += str(lu).zfill(3)
-                encoded += '.'
+                encoded += "."
                 encoded += str(la).zfill(3)
 
             if count == 1:
                 return encoded
             else:
                 encodeds.append(encoded)
         return encodeds
 
     @staticmethod
-    def breakdown_tt2000(tt2000, to_np: bool = False):
+    def breakdown_tt2000(tt2000: cdf_tt2000_type) -> np.ndarray:
         """
         Breaks down the epoch(s) into UTC components.
 
         For CDF_EPOCH:
                 they are 7 date/time components: year, month, day,
                 hour, minute, second, and millisecond
         For CDF_EPOCH16:
                 they are 10 date/time components: year, month, day,
                 hour, minute, second, and millisecond, microsecond,
                 nanosecond, and picosecond.
         For TT2000:
                 they are 9 date/time components: year, month, day,
                 hour, minute, second, millisecond, microsecond,
                 nanosecond.
-
-        Specify to_np to True, if the result should be in numpy array.
         """
-        new_tt2000: np.ndarray = np.atleast_1d(tt2000).astype(np.longlong)
+        new_tt2000 = np.atleast_1d(tt2000).astype(np.longlong)
         count = len(new_tt2000)
         toutcs = np.zeros((9, count), dtype=int)
         datxs = CDFepoch._LeapSecondsfromJ2000(new_tt2000)
 
         # Do some computations on arrays to speed things up
         post2000 = new_tt2000 > 0
         nanoSecsSinceJ2000 = new_tt2000.copy()
@@ -474,50 +429,46 @@
                 nansec = nansecs[x]
 
                 xdate = np.zeros(9)
                 xdate[:6] = xdates[:, x]
                 xdate[8] = nansec
 
                 tmpNanosecs = CDFepoch.compute_tt2000(xdate)
-                if (tmpNanosecs != t3):
-                    dat0 = CDFepoch._LeapSecondsfromYMD(xdate[0],
-                                                        xdate[1], xdate[2])
+                if tmpNanosecs != t3:
+                    dat0 = CDFepoch._LeapSecondsfromYMD(xdate[0], xdate[1], xdate[2])
                     tmpx = t2 - int(dat0 * CDFepoch.SECinNanoSecs)
                     tmpy = int(float(tmpx / CDFepoch.SECinNanoSecsD))
                     nansec = int(tmpx - tmpy * CDFepoch.SECinNanoSecs)
-                if (nansec < 0):
+                if nansec < 0:
                     nansec = CDFepoch.SECinNanoSecs + nansec
                     tmpy = tmpy - 1
                     epoch = tmpy + CDFepoch.J2000Since0AD12hSec
                     xdate = np.zeros(9)
                     xdate[:6] = CDFepoch._EPOCHbreakdownTT2000(epoch)[:, 0]
                     xdate[8] = nansec
                     tmpNanosecs = CDFepoch.compute_tt2000(xdate)
-                if (tmpNanosecs != t3):
-                    dat0 = CDFepoch._LeapSecondsfromYMD(xdate[0],
-                                                        xdate[1], xdate[2])
+                if tmpNanosecs != t3:
+                    dat0 = CDFepoch._LeapSecondsfromYMD(xdate[0], xdate[1], xdate[2])
                     tmpx = t2 - int(dat0 * CDFepoch.SECinNanoSecs)
                     tmpy = int((1.0 * tmpx) / CDFepoch.SECinNanoSecsD)
                     nansec = int(tmpx - tmpy * CDFepoch.SECinNanoSecs)
-                    if (nansec < 0):
+                    if nansec < 0:
                         nansec = CDFepoch.SECinNanoSecs + nansec
                         tmpy = tmpy - 1
                     epoch = tmpy + CDFepoch.J2000Since0AD12hSec
                     xdate = np.zeros(9)
                     xdate[:6] = CDFepoch._EPOCHbreakdownTT2000(epoch)[:, 0]
                     xdate[8] = nansec
                     tmpNanosecs = CDFepoch.compute_tt2000(xdate)
-                    if (tmpNanosecs != t3):
-                        dat0 = CDFepoch._LeapSecondsfromYMD(xdate[0],
-                                                            xdate[1],
-                                                            xdate[2])
+                    if tmpNanosecs != t3:
+                        dat0 = CDFepoch._LeapSecondsfromYMD(xdate[0], xdate[1], xdate[2])
                         tmpx = t2 - int(dat0 * CDFepoch.SECinNanoSecs)
                         tmpy = int((1.0 * tmpx) / CDFepoch.SECinNanoSecsD)
                         nansec = int(tmpx - tmpy * CDFepoch.SECinNanoSecs)
-                        if (nansec < 0):
+                        if nansec < 0:
                             nansec = CDFepoch.SECinNanoSecs + nansec
                             tmpy = tmpy - 1
                         epoch = tmpy + CDFepoch.J2000Since0AD12hSec
                         # One more determination
                         xdate = CDFepoch._EPOCHbreakdownTT2000(epoch)
                 nansecs[x] = nansec
                 toutcs[:6, x] = xdate[:6]
@@ -532,226 +483,223 @@
         toutcs[5, overflow] += 1
 
         ma1 = tmp1 // 1000
         na1 = tmp1 - 1000 * ma1
         toutcs[7, :] = ma1
         toutcs[8, :] = na1
 
-        if not to_np:
-            toutcs = toutcs.T.tolist()
-            if len(toutcs) == 1:
-                return toutcs[0]
-            return toutcs
-        return toutcs.T
+        return np.squeeze(toutcs.T)
 
     @staticmethod
-    def compute_tt2000(datetimes, to_np: bool = False):
-
+    def compute_tt2000(datetimes: npt.ArrayLike) -> Union[int, npt.NDArray[np.int64]]:
         if not isinstance(datetimes, (list, tuple, np.ndarray)):
-            raise TypeError('datetime must be in list form')
+            raise TypeError("datetime must be in list form")
 
-        if isinstance(datetimes[0], numbers.Number):
-            new_datetimes = [datetimes]
-            count = 1
-        else:
-            count = len(datetimes)
-            new_datetimes = datetimes
+        new_datetimes = np.atleast_2d(datetimes)
+        count = len(new_datetimes)
         nanoSecSinceJ2000s = []
         for x in range(count):
             datetime = new_datetimes[x]
             year = int(datetime[0])
             month = int(datetime[1])
             items = len(datetime)
-            if (items > 8):
+            if items > 8:
                 # y m d h m s ms us ns
                 day = int(datetime[2])
                 hour = int(datetime[3])
                 minute = int(datetime[4])
                 second = int(datetime[5])
                 msec = int(datetime[6])
                 usec = int(datetime[7])
                 nsec = int(datetime[8])
-            elif (items > 7):
+            elif items > 7:
                 # y m d h m s ms us
                 day = int(datetime[2])
                 hour = int(datetime[3])
                 minute = int(datetime[4])
                 second = int(datetime[5])
                 msec = int(datetime[6])
                 usec = int(datetime[7])
                 nsec = int(1000.0 * (datetime[7] - usec))
-            elif (items > 6):
+            elif items > 6:
                 # y m d h m s ms
                 day = int(datetime[2])
                 hour = int(datetime[3])
                 minute = int(datetime[4])
                 second = int(datetime[5])
                 msec = int(datetime[6])
                 xxx = float(1000.0 * (datetime[6] - msec))
                 usec = int(xxx)
                 nsec = int(1000.0 * (xxx - usec))
-            elif (items > 5):
+            elif items > 5:
                 # y m d h m s
                 day = int(datetime[2])
                 hour = int(datetime[3])
                 minute = int(datetime[4])
                 second = int(datetime[5])
                 xxx = float(1000.0 * (datetime[5] - second))
                 msec = int(xxx)
                 xxx = float(1000.0 * (xxx - msec))
                 usec = int(xxx)
                 nsec = int(1000.0 * (xxx - usec))
-            elif (items > 4):
+            elif items > 4:
                 # y m d h m
                 day = int(datetime[2])
                 hour = int(datetime[3])
                 minute = int(datetime[4])
                 xxx = float(60.0 * (datetime[4] - minute))
                 second = int(xxx)
                 xxx = float(1000.0 * (xxx - second))
                 msec = int(xxx)
                 xxx = float(1000.0 * (xxx - msec))
                 usec = int(xxx)
                 nsec = int(1000.0 * (xxx - usec))
-            elif (items > 3):
+            elif items > 3:
                 # y m d h
                 day = int(datetime[2])
                 hour = int(datetime[3])
                 xxx = float(60.0 * (datetime[3] - hour))
                 minute = int(xxx)
                 xxx = float(60.0 * (xxx - minute))
                 second = int(xxx)
                 xxx = float(1000.0 * (xxx - second))
                 msec = int(xxx)
                 xxx = float(1000.0 * (xxx - msec))
                 usec = int(xxx)
                 nsec = int(1000.0 * (xxx - usec))
-            elif (items > 2):
+            elif items > 2:
                 # y m d
                 day = int(datetime[2])
                 xxx = float(24.0 * (datetime[2] - day))
                 hour = int(xxx)
                 xxx = float(60.0 * (xxx - hour))
                 minute = int(xxx)
                 xxx = float(60.0 * (xxx - minute))
                 second = int(xxx)
                 xxx = float(1000.0 * (xxx - second))
                 msec = int(xxx)
                 xxx = float(1000.0 * (xxx - msec))
                 usec = int(xxx)
                 nsec = int(1000.0 * (xxx - usec))
             else:
-                raise ValueError('Invalid tt2000 components')
+                raise ValueError("Invalid tt2000 components")
 
-            if (month == 0):
+            if month == 0:
                 month = 1
-            if (year == 9999 and month == 12 and day == 31 and hour == 23 and
-                minute == 59 and second == 59 and msec == 999 and
-                    usec == 999 and nsec == 999):
+            if (
+                year == 9999
+                and month == 12
+                and day == 31
+                and hour == 23
+                and minute == 59
+                and second == 59
+                and msec == 999
+                and usec == 999
+                and nsec == 999
+            ):
                 nanoSecSinceJ2000 = CDFepoch.FILLED_TT2000_VALUE
-            elif (year == 0 and month == 1 and day == 1 and hour == 0 and
-                  minute == 0 and second == 0 and msec == 0 and usec == 0 and
-                  nsec == 0):
+            elif (
+                year == 0
+                and month == 1
+                and day == 1
+                and hour == 0
+                and minute == 0
+                and second == 0
+                and msec == 0
+                and usec == 0
+                and nsec == 0
+            ):
                 nanoSecSinceJ2000 = CDFepoch.DEFAULT_TT2000_PADVALUE
             else:
                 iy = 10000000 * month + 10000 * day + year
-                if (iy != CDFepoch.currentDay):
+                if iy != CDFepoch.currentDay:
                     CDFepoch.currentDay = iy
-                    CDFepoch.currentLeapSeconds = CDFepoch._LeapSecondsfromYMD(
-                        year, month, day)
+                    CDFepoch.currentLeapSeconds = CDFepoch._LeapSecondsfromYMD(year, month, day)
                     CDFepoch.currentJDay = CDFepoch._JulianDay(year, month, day)
                 jd = CDFepoch.currentJDay
                 jd = jd - CDFepoch.JulianDateJ2000_12h
-                subDayinNanoSecs = int(hour * CDFepoch.HOURinNanoSecs +
-                                       minute * CDFepoch.MINUTEinNanoSecs +
-                                       second * CDFepoch.SECinNanoSecs +
-                                       msec * 1000000 + usec * 1000 + nsec)
-                nanoSecSinceJ2000 = int(jd * CDFepoch.DAYinNanoSecs +
-                                        subDayinNanoSecs)
+                subDayinNanoSecs = int(
+                    hour * CDFepoch.HOURinNanoSecs
+                    + minute * CDFepoch.MINUTEinNanoSecs
+                    + second * CDFepoch.SECinNanoSecs
+                    + msec * 1000000
+                    + usec * 1000
+                    + nsec
+                )
+                nanoSecSinceJ2000 = int(jd * CDFepoch.DAYinNanoSecs + subDayinNanoSecs)
                 t2 = int(CDFepoch.currentLeapSeconds * CDFepoch.SECinNanoSecs)
-                if (nanoSecSinceJ2000 < 0):
+                if nanoSecSinceJ2000 < 0:
                     nanoSecSinceJ2000 = int(nanoSecSinceJ2000 + t2)
-                    nanoSecSinceJ2000 = int(nanoSecSinceJ2000 +
-                                            CDFepoch.dTinNanoSecs)
-                    nanoSecSinceJ2000 = int(nanoSecSinceJ2000 -
-                                            CDFepoch.T12hinNanoSecs)
+                    nanoSecSinceJ2000 = int(nanoSecSinceJ2000 + CDFepoch.dTinNanoSecs)
+                    nanoSecSinceJ2000 = int(nanoSecSinceJ2000 - CDFepoch.T12hinNanoSecs)
                 else:
-                    nanoSecSinceJ2000 = int(nanoSecSinceJ2000 -
-                                            CDFepoch.T12hinNanoSecs)
+                    nanoSecSinceJ2000 = int(nanoSecSinceJ2000 - CDFepoch.T12hinNanoSecs)
                     nanoSecSinceJ2000 = int(nanoSecSinceJ2000 + t2)
-                    nanoSecSinceJ2000 = int(nanoSecSinceJ2000 +
-                                            CDFepoch.dTinNanoSecs)
-            if (count == 1):
-                if not to_np:
-                    return int(nanoSecSinceJ2000)
-                else:
-                    return np.array(int(nanoSecSinceJ2000))
-            else:
-                nanoSecSinceJ2000s.append(int(nanoSecSinceJ2000))
-        if not to_np:
-            return nanoSecSinceJ2000s
-        else:
-            return np.array(nanoSecSinceJ2000s)
+                    nanoSecSinceJ2000 = int(nanoSecSinceJ2000 + CDFepoch.dTinNanoSecs)
 
-    @staticmethod
-    def _LeapSecondsfromYMD(year, month, day):  # @NoSelf
+            nanoSecSinceJ2000s.append(int(nanoSecSinceJ2000))
+
+        return np.array(nanoSecSinceJ2000s)
 
+    @staticmethod
+    def _LeapSecondsfromYMD(year: int, month: int, day: int) -> float:
         j = -1
         m = 12 * year + month
         for i, _ in reversed(list(enumerate(CDFepoch.LTS))):
             n = 12 * CDFepoch.LTS[i][0] + CDFepoch.LTS[i][1]
-            if (m >= n):
+            if m >= n:
                 j = i
                 break
-        if (j == -1):
-            return 0.0
+        if j == -1:
+            return 0
         da = CDFepoch.LTS[j][3]
         # pre-1972
-        if (j < CDFepoch.NERA1):
+        if j < CDFepoch.NERA1:
             jda = CDFepoch._JulianDay(year, month, day)
             da = da + ((jda - CDFepoch.MJDbase) - CDFepoch.LTS[j][4]) * CDFepoch.LTS[j][5]
         return da
 
     @staticmethod
-    def _LeapSecondsfromJ2000(nanosecs):  # @NoSelf
+    def _LeapSecondsfromJ2000(nanosecs: npt.ArrayLike) -> npt.NDArray:
         nanosecs = np.atleast_1d(nanosecs)
         da = np.zeros((nanosecs.size, 2))
         j = -1 * np.ones(nanosecs.size, dtype=int)
 
-        if (CDFepoch.NST is None):
+        if CDFepoch.NST is None:
             CDFepoch._LoadLeapNanoSecondsTable()
         for i, _ in reversed(list(enumerate(CDFepoch.NST))):
             idxs = (j == -1) & (nanosecs >= CDFepoch.NST[i])
             j[idxs] = i
-            if (i < (CDFepoch.NDAT - 1)):
+            if i < (CDFepoch.NDAT - 1):
                 overflow = nanosecs + 1000000000 >= CDFepoch.NST[i + 1]
                 da[overflow, 1] = 1.0
             if np.all(j > 0):
                 break
 
         LTS = np.array(CDFepoch.LTS)
         da[:, 0] = LTS[j, 3]
         da[j <= CDFepoch.NERA1, 0] = 0
         return da
 
     @staticmethod
-    def _LoadLeapNanoSecondsTable():  # @NoSelf
-
+    def _LoadLeapNanoSecondsTable() -> None:
         CDFepoch.NST = []
         for ix in range(0, CDFepoch.NERA1):
             CDFepoch.NST.append(CDFepoch.FILLED_TT2000_VALUE)
         for ix in range(CDFepoch.NERA1, CDFepoch.NDAT):
-            CDFepoch.NST.append(CDFepoch.compute_tt2000([int(CDFepoch.LTS[ix][0]),
-                                                         int(CDFepoch.LTS[ix][1]),
-                                                         int(CDFepoch.LTS[ix][2]),
-                                                         0, 0, 0, 0, 0, 0]))
-        CDFepoch.NST = np.array(CDFepoch.NST)
+            CDFepoch.NST.append(
+                int(
+                    CDFepoch.compute_tt2000(
+                        [int(CDFepoch.LTS[ix][0]), int(CDFepoch.LTS[ix][1]), int(CDFepoch.LTS[ix][2]), 0, 0, 0, 0, 0, 0]
+                    )
+                )
+            )
 
     @staticmethod
-    def _EPOCHbreakdownTT2000(epoch):  # @NoSelf
+    def _EPOCHbreakdownTT2000(epoch: npt.ArrayLike) -> npt.NDArray:
         epoch = np.atleast_1d(epoch)
 
         minute_AD, second_AD = np.divmod(epoch, 60)
         hour_AD, minute_AD = np.divmod(minute_AD, 60)
         day_AD, hour_AD = np.divmod(hour_AD, 24)
         # minute_AD = second_AD / 60.0
         # hour_AD = minute_AD / 60.0
@@ -764,245 +712,224 @@
         l = l - (1461 * i / 4).astype(int) + 31
         j = (80 * l / 2447).astype(int)
         k = l - (2447 * j / 80).astype(int)
         l = (j / 11).astype(int)
         j = j + 2 - 12 * l
         i = 100 * (n - 49) + i + l
 
-        date = np.array(
-            [i, j, k,
-             hour_AD,
-             minute_AD,
-             second_AD])
+        date = np.array([i, j, k, hour_AD, minute_AD, second_AD])
         return date
 
     @staticmethod
-    def epochrange_tt2000(epochs, starttime=None, endtime=None):  # @NoSelf
-
-        if (isinstance(epochs, int) or isinstance(epochs, np.int64)):
+    def epochrange_tt2000(
+        epochs: cdf_tt2000_type, starttime: Optional[epoch_types] = None, endtime: Optional[epoch_types] = None
+    ) -> npt.NDArray:
+        if isinstance(epochs, int) or isinstance(epochs, np.int64):
             pass
-        elif (isinstance(epochs, list) or isinstance(epochs, tuple) or
-              isinstance(epochs, np.ndarray)):
-            if (isinstance(epochs[0], int) or
-                    isinstance(epochs[0], np.int64)):
+        elif isinstance(epochs, list) or isinstance(epochs, tuple) or isinstance(epochs, np.ndarray):
+            if isinstance(epochs[0], int) or isinstance(epochs[0], np.int64):
                 pass
             else:
-                raise ValueError('Bad data')
+                raise ValueError("Bad data")
         else:
-            raise ValueError('Bad data')
-        if (starttime is None):
+            raise ValueError("Bad data")
+        stime: Union[int, np.int64]
+        if starttime is None:
             stime = int(-9223372036854775807)
         else:
-            if (isinstance(starttime, int) or isinstance(starttime, np.int64)):
+            if isinstance(starttime, int) or isinstance(starttime, np.int64):
                 stime = starttime
-            elif (isinstance(starttime, list)):
-                stime = CDFepoch.compute_tt2000(starttime)
+            elif isinstance(starttime, list):
+                stime = int(CDFepoch.compute_tt2000(starttime))
             else:
-                raise ValueError('Bad start time')
-        if (endtime is not None):
-            if (isinstance(endtime, int) or isinstance(endtime, np.int64)):
+                raise ValueError("Bad start time")
+        if endtime is not None:
+            if isinstance(endtime, int) or isinstance(endtime, np.int64):
                 etime = endtime
-            elif (isinstance(endtime, list) or isinstance(endtime, tuple)):
-                etime = CDFepoch.compute_tt2000(endtime)
+            elif isinstance(endtime, list) or isinstance(endtime, tuple):
+                etime = int(CDFepoch.compute_tt2000(endtime))
             else:
-                raise ValueError('Bad end time')
+                raise ValueError("Bad end time")
         else:
             etime = int(9223372036854775807)
-        if (stime > etime):
-            raise ValueError('Invalid start/end time')
-        if (isinstance(epochs, list) or isinstance(epochs, tuple)):
-            new_epochs = np.array(epochs)
-        else:
-            new_epochs = epochs
+        if stime > etime:
+            raise ValueError("Invalid start/end time")
+        new_epochs = np.array(epochs)
         return np.where(np.logical_and(new_epochs >= stime, new_epochs <= etime))[0]
 
     @staticmethod
-    def encode_epoch16(epochs, iso_8601: bool = True):
-
-        if isinstance(epochs, (complex, np.complex128)):
-            new_epochs = [epochs]
-        elif isinstance(epochs, (list, tuple, np.ndarray)):
-            new_epochs = epochs
-        else:
-            raise TypeError('bad data')
+    def encode_epoch16(epochs: cdf_epoch16_type, iso_8601: bool = True) -> encoded_type:
+        new_epochs = np.atleast_1d(epochs)
 
         count = len(new_epochs)
         encodeds = []
         for x in range(count):
             # complex
-            if ((new_epochs[x].real == -1.0E31) and (new_epochs[x].imag == -1.0E31)):
+            if (new_epochs[x].real == -1.0e31) and (new_epochs[x].imag == -1.0e31):
                 if iso_8601:
-                    encoded = '9999-12-31T23:59:59.999999999999'
+                    encoded = "9999-12-31T23:59:59.999999999999"
                 else:
-                    encoded = '31-Dec-9999 23:59:59.999.999.999.999'
+                    encoded = "31-Dec-9999 23:59:59.999.999.999.999"
             else:
                 encoded = CDFepoch._encodex_epoch16(new_epochs[x], iso_8601)
             if count == 1:
                 return encoded
             else:
                 encodeds.append(encoded)
         return encodeds
 
     @staticmethod
-    def _encodex_epoch16(epoch16, iso_8601: bool = True) -> str:
-
+    def _encodex_epoch16(epoch16: cdf_epoch16_type, iso_8601: bool = True) -> str:
         components = CDFepoch.breakdown_epoch16(epoch16)
         if iso_8601:
             # year-mm-ddThh:mm:ss.mmmuuunnnppp
             encoded = str(components[0]).zfill(4)
-            encoded += '-'
+            encoded += "-"
             encoded += str(components[1]).zfill(2)
-            encoded += '-'
+            encoded += "-"
             encoded += str(components[2]).zfill(2)
-            encoded += 'T'
+            encoded += "T"
             encoded += str(components[3]).zfill(2)
-            encoded += ':'
+            encoded += ":"
             encoded += str(components[4]).zfill(2)
-            encoded += ':'
+            encoded += ":"
             encoded += str(components[5]).zfill(2)
-            encoded += '.'
+            encoded += "."
             encoded += str(components[6]).zfill(3)
             encoded += str(components[7]).zfill(3)
             encoded += str(components[8]).zfill(3)
             encoded += str(components[9]).zfill(3)
         else:
             # dd-mmm-year hh:mm:ss.mmm.uuu.nnn.ppp
             encoded = str(components[2]).zfill(2)
-            encoded += '-'
+            encoded += "-"
             encoded += CDFepoch.month_Token[components[1] - 1]
-            encoded += '-'
+            encoded += "-"
             encoded += str(components[0]).zfill(4)
-            encoded += ' '
+            encoded += " "
             encoded += str(components[3]).zfill(2)
-            encoded += ':'
+            encoded += ":"
             encoded += str(components[4]).zfill(2)
-            encoded += ':'
+            encoded += ":"
             encoded += str(components[5]).zfill(2)
-            encoded += '.'
+            encoded += "."
             encoded += str(components[6]).zfill(3)
-            encoded += '.'
+            encoded += "."
             encoded += str(components[7]).zfill(3)
-            encoded += '.'
+            encoded += "."
             encoded += str(components[8]).zfill(3)
-            encoded += '.'
+            encoded += "."
             encoded += str(components[9]).zfill(3)
         return encoded
 
     @staticmethod
     def _JulianDay(y: int, m: int, d: int) -> int:
-
         a1 = int(7 * (int(y + int((m + 9) / 12))) / 4)
         a2 = int(3 * (int(int(y + int((m - 9) / 7)) / 100) + 1) / 4)
         a3 = int(275 * m / 9)
-        return (367 * y - a1 - a2 + a3 + d + 1721029)
+        return 367 * y - a1 - a2 + a3 + d + 1721029
 
     @staticmethod
-    def compute_epoch16(datetimes: Union[List, List[List]], to_np: bool = False):
-        new_dates: List[list] = []
-        if not isinstance(datetimes[0], list):
-            new_dates = [datetimes]
-        else:
-            new_dates = datetimes
+    def compute_epoch16(datetimes: npt.ArrayLike) -> Union[complex, npt.NDArray[np.complex128]]:
+        new_dates = np.atleast_2d(datetimes)
         count = len(new_dates)
-        if (count == 0):
-            return
         epochs = []
         for x in range(count):
             epoch = []
             date = new_dates[x]
             items = len(date)
             year = date[0]
             month = date[1]
             xxx: Union[float, int] = 0
-            if (items > 9):
+            if items > 9:
                 # y m d h m s ms us ns ps
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 second = int(date[5])
                 msec = int(date[6])
                 usec = int(date[7])
                 nsec = int(date[8])
                 psec = int(date[9])
-            elif (items > 8):
+            elif items > 8:
                 # y m d h m s ms us ns
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 second = int(date[5])
                 msec = int(date[6])
                 usec = int(date[7])
                 nsec = int(date[8])
                 psec = int(1000.0 * (date[8] - nsec))
-            elif (items > 7):
+            elif items > 7:
                 # y m d h m s ms us
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 second = int(date[5])
                 msec = int(date[6])
                 usec = int(date[7])
                 xxx = int(1000.0 * (date[7] - usec))
                 nsec = int(xxx)
                 psec = int(1000.0 * (xxx - nsec))
-            elif (items > 6):
+            elif items > 6:
                 # y m d h m s ms
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 second = int(date[5])
                 msec = int(date[6])
                 xxx = float(1000.0 * (date[6] - msec))
                 usec = int(xxx)
                 xxx = int(1000.0 * (xxx - usec))
                 nsec = int(xxx)
                 psec = int(1000.0 * (xxx - nsec))
-            elif (items > 5):
+            elif items > 5:
                 # y m d h m s
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 second = int(date[5])
                 xxx = float(1000.0 * (date[5] - second))
                 msec = int(xxx)
                 xxx = float(1000.0 * (xxx - msec))
                 usec = int(xxx)
                 xxx = int(1000.0 * (xxx - usec))
                 nsec = int(xxx)
                 psec = int(1000.0 * (xxx - nsec))
-            elif (items > 4):
+            elif items > 4:
                 # y m d h m
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 xxx = float(60.0 * (date[4] - minute))
                 second = int(xxx)
                 xxx = float(1000.0 * (xxx - second))
                 msec = int(xxx)
                 xxx = float(1000.0 * (xxx - msec))
                 usec = int(xxx)
                 xxx = int(1000.0 * (xxx - usec))
                 nsec = int(xxx)
                 psec = int(1000.0 * (xxx - nsec))
-            elif (items > 3):
+            elif items > 3:
                 # y m d h
                 day = int(date[2])
                 hour = int(date[3])
                 xxx = float(60.0 * (date[3] - hour))
                 minute = int(xxx)
                 xxx = float(60.0 * (xxx - minute))
                 second = int(xxx)
                 xxx = float(1000.0 * (xxx - second))
                 msec = int(xxx)
                 xxx = float(1000.0 * (xxx - msec))
                 usec = int(xxx)
                 xxx = int(1000.0 * (xxx - usec))
                 nsec = int(xxx)
                 psec = int(1000.0 * (xxx - nsec))
-            elif (items > 2):
+            elif items > 2:
                 # y m d
                 day = int(date[2])
                 xxx = float(24.0 * (date[2] - day))
                 hour = int(xxx)
                 xxx = float(60.0 * (xxx - hour))
                 minute = int(xxx)
                 xxx = float(60.0 * (xxx - minute))
@@ -1011,82 +938,80 @@
                 msec = int(xxx)
                 xxx = float(1000.0 * (xxx - msec))
                 usec = int(xxx)
                 xxx = int(1000.0 * (xxx - usec))
                 nsec = int(xxx)
                 psec = int(1000.0 * (xxx - nsec))
             else:
-                raise ValueError('Invalid epoch16 components')
+                raise ValueError("Invalid epoch16 components")
 
-            if (year < 0):
-                raise ValueError('Illegal epoch field')
+            if year < 0:
+                raise ValueError("Illegal epoch field")
 
-            if (year == 9999 and month == 12 and day == 31 and hour == 23 and
-                minute == 59 and second == 59 and msec == 999 and
-                    usec == 999 and nsec == 999 and psec == 999):
-                epoch.append(-1.0E31)
-                epoch.append(-1.0E31)
-            elif ((year > 9999) or (month < 0 or month > 12) or
-                  (hour < 0 or hour > 23) or (minute < 0 or minute > 59) or
-                  (second < 0 or second > 59) or (msec < 0 or msec > 999) or
-                  (usec < 0 or usec > 999) or (nsec < 0 or nsec > 999) or
-                  (psec < 0 or psec > 999)):
-                epoch = CDFepoch._computeEpoch16(year, month, day, hour,
-                                                 minute, second, msec,
-                                                 usec, nsec, psec)
-            else:
-                if (month == 0):
-                    if (day < 1 or day > 366):
-                        epoch = CDFepoch._computeEpoch16(year, month, day, hour,
-                                                         minute, second, msec,
-                                                         usec, nsec, psec)
-                else:
-                    if (day < 1 or day > 31):
-                        epoch = CDFepoch._computeEpoch16(year, month, day, hour,
-                                                         minute, second, msec,
-                                                         usec, nsec, psec)
-                if (month == 0):
-                    daysSince0AD = CDFepoch._JulianDay(
-                        year, 1, 1) + (day - 1) - 1721060
+            if (
+                year == 9999
+                and month == 12
+                and day == 31
+                and hour == 23
+                and minute == 59
+                and second == 59
+                and msec == 999
+                and usec == 999
+                and nsec == 999
+                and psec == 999
+            ):
+                epoch.append(-1.0e31)
+                epoch.append(-1.0e31)
+            elif (
+                (year > 9999)
+                or (month < 0 or month > 12)
+                or (hour < 0 or hour > 23)
+                or (minute < 0 or minute > 59)
+                or (second < 0 or second > 59)
+                or (msec < 0 or msec > 999)
+                or (usec < 0 or usec > 999)
+                or (nsec < 0 or nsec > 999)
+                or (psec < 0 or psec > 999)
+            ):
+                epoch = CDFepoch._computeEpoch16(year, month, day, hour, minute, second, msec, usec, nsec, psec)
+            else:
+                if month == 0:
+                    if day < 1 or day > 366:
+                        epoch = CDFepoch._computeEpoch16(year, month, day, hour, minute, second, msec, usec, nsec, psec)
+                else:
+                    if day < 1 or day > 31:
+                        epoch = CDFepoch._computeEpoch16(year, month, day, hour, minute, second, msec, usec, nsec, psec)
+                if month == 0:
+                    daysSince0AD = CDFepoch._JulianDay(year, 1, 1) + (day - 1) - 1721060
                 else:
-                    daysSince0AD = CDFepoch._JulianDay(
-                        year, month, day) - 1721060
+                    daysSince0AD = CDFepoch._JulianDay(year, month, day) - 1721060
                 secInDay = (3600 * hour) + (60 * minute) + second
                 epoch16_0 = float(86400.0 * daysSince0AD) + float(secInDay)
-                epoch16_1 = float(psec) + float(1000.0 * nsec) + float(
-                    1000000.0 * usec) + float(1000000000.0 * msec)
+                epoch16_1 = float(psec) + float(1000.0 * nsec) + float(1000000.0 * usec) + float(1000000000.0 * msec)
                 epoch.append(epoch16_0)
                 epoch.append(epoch16_1)
             cepoch = complex(epoch[0], epoch[1])
-            if (count == 1):
-                if not to_np:
-                    return cepoch
-                else:
-                    return np.array(cepoch)
-            else:
-                epochs.append(cepoch)
-        if not to_np:
-            return epochs
-        else:
-            return np.array(epochs)
+            epochs.append(cepoch)
+
+        return _squeeze_or_scalar_complex(epochs)
 
     @staticmethod
-    def _calc_from_julian(epoch0, epoch1):
+    def _calc_from_julian(epoch0: npt.ArrayLike, epoch1: npt.ArrayLike) -> npt.NDArray:
         """Calculate the date and time from epoch input
 
         Parameters
         ----------
-        epoch0 : int, float, or array-like
+        epoch0 : int, float, array-like
             First element of an epoch array (epoch time in seconds)
-        epoch1 : float or array-like
+        epoch1 : float, array-like
             Second element of an epoch array (epoch time in picoseconds)
 
         Returns
         -------
-        out : array of int
+        out : array-like
             Array of 10 integers (year, month, day, hour, minute, second,
             millisecond, microsecond, nanosecond, picosecond) if a single value
             is input. For array input, the shape is altered by adding another
             axis of length 10 (holding the same values).
 
         """
         # Cast input as an array for consistent handling of scalars and lists
@@ -1125,674 +1050,597 @@
         msec = msec / 1000.0
         mus = (msec % 1000.0).astype(int)
         msec = msec / 1000.0
         ms = msec.astype(int)
 
         # Recast the output as integers or lists
         if second_ce.shape == ():
-            out = np.array([int(yr), int(mo), int(dy), int(hr), int(mn),
-                            int(sc), int(ms), int(mus), int(ns), int(ps)])
+            out = np.array([int(yr), int(mo), int(dy), int(hr), int(mn), int(sc), int(ms), int(mus), int(ns), int(ps)])
         else:
-            out = np.array([yr, mo, dy, hr, mn, sc,
-                            ms, mus, ns, ps]).transpose()
+            out = np.array([yr, mo, dy, hr, mn, sc, ms, mus, ns, ps]).transpose()
         return out
 
     @staticmethod
-    def breakdown_epoch16(epochs, to_np: bool = False):
-        """ Calculate date and time from epochs
+    def breakdown_epoch16(epochs: cdf_epoch16_type) -> npt.NDArray:
+        """
+        Calculate date and time from epochs
 
         Parameters
         ----------
-        epochs : np.complex128 or array-like
+        epochs : array-like
             Single, list, tuple, or np.array of epoch values
-        to_np : bool
-            Flag for output type, if True will be an np.array, if False
-            will be a list (default=False)
 
         Returns
         -------
-        components : list-like of ints
+        components : ndarray
             List or array of date and time values.  The last axis contains
             (in order): year, month, day, hour, minute, second, millisecond,
             microsecond, nanosecond, and picosecond
 
         Notes
         -----
         If a bad epoch (-1.0e31 for the real and imaginary components) is
         supplied, a fill date of 9999-12-31 23:59:59 and 999 ms, 999 us,
         999 ns, and 999 ps is returned
 
         """
 
-        if (isinstance(epochs, (complex, np.complex128))
-                or isinstance(epochs, (list, tuple, np.ndarray))):
+        if isinstance(epochs, (complex, np.complex128)) or isinstance(epochs, (list, tuple, np.ndarray)):
             new_epochs = np.asarray(epochs)
             if new_epochs.shape == ():
                 cshape = []
                 new_epochs = np.array([epochs])
             else:
                 cshape = list(new_epochs.shape)
         else:
-            raise TypeError('Bad data for epochs: {:}'.format(type(epochs)))
+            raise TypeError("Bad data for epochs: {:}".format(type(epochs)))
 
         cshape.append(10)
-        components = np.full(shape=cshape, fill_value=[9999, 12, 31, 23, 59,
-                                                       59, 999, 999, 999, 999])
+        components = np.full(shape=cshape, fill_value=[9999, 12, 31, 23, 59, 59, 999, 999, 999, 999])
         for i, epoch16 in enumerate(new_epochs):
             # Ignore fill values
-            if (epoch16.real != -1.0E31) or (epoch16.imag != -1.0E31):
+            if (epoch16.real != -1.0e31) or (epoch16.imag != -1.0e31):
                 esec = -epoch16.real if epoch16.real < 0.0 else epoch16.real
                 efra = -epoch16.imag if epoch16.imag < 0.0 else epoch16.imag
 
                 if len(components.shape) == 1:
                     components = CDFepoch._calc_from_julian(esec, efra)
                 else:
                     components[i] = CDFepoch._calc_from_julian(esec, efra)
 
-        if to_np:
-            return components
-        else:
-            comp = components.tolist()
-            if len(comp) == 1:
-                return comp[0]
-            return comp
-
-    def _computeEpoch16(y, m, d, h, mn, s, ms, msu, msn, msp):  # @NoSelf
+        return components
 
-        if (m == 0):
+    @staticmethod
+    def _computeEpoch16(y: int, m: int, d: int, h: int, mn: int, s: int, ms: int, msu: int, msn: int, msp: int) -> List[float]:
+        if m == 0:
             daysSince0AD = CDFepoch._JulianDay(y, 1, 1) + (d - 1) - 1721060
         else:
-            if (m < 0):
+            if m < 0:
                 y = y - 1
                 m = 13 + m
             daysSince0AD = CDFepoch._JulianDay(y, m, d) - 1721060
-        if (daysSince0AD < 0):
-            raise ValueError('Illegal epoch')
+        if daysSince0AD < 0:
+            raise ValueError("Illegal epoch")
         epoch = []
         epoch.append(float(86400.0 * daysSince0AD + 3600.0 * h + 60.0 * mn) + float(s))
         epoch.append(float(msp) + float(1000.0 * msn) + float(1000000.0 * msu) + math.pow(10.0, 9) * ms)
-        if (epoch[1] < 0.0 or epoch[1] >= math.pow(10.0, 12)):
-            if (epoch[1] < 0.0):
+        if epoch[1] < 0.0 or epoch[1] >= math.pow(10.0, 12):
+            if epoch[1] < 0.0:
                 sec = int(epoch[1] / math.pow(10.0, 12))
                 tmp = epoch[1] - sec * math.pow(10.0, 12)
-                if (tmp != 0.0 and tmp != -0.0):
+                if tmp != 0.0 and tmp != -0.0:
                     epoch[0] = epoch[0] + sec - 1
                     epoch[1] = math.pow(10.0, 12.0) + tmp
                 else:
                     epoch[0] = epoch[0] + sec
                     epoch[1] = 0.0
             else:
                 sec = int(epoch[1] / math.pow(10.0, 12))
                 tmp = epoch[1] - sec * math.pow(10.0, 12)
-                if (tmp != 0.0 and tmp != -0.0):
+                if tmp != 0.0 and tmp != -0.0:
                     epoch[1] = tmp
                     epoch[0] = epoch[0] + sec
                 else:
                     epoch[1] = 0.0
                     epoch[0] = epoch[0] + sec
-        if (epoch[0] < 0.0):
-            raise ValueError('Illegal epoch')
+        if epoch[0] < 0.0:
+            raise ValueError("Illegal epoch")
         else:
             return epoch
 
-    def epochrange_epoch16(epochs, starttime=None, endtime=None):  # @NoSelf
-
-        if (isinstance(epochs, complex) or isinstance(epochs, np.complex128)):
-            new_epochs = [epochs]
-        elif (isinstance(epochs, list) or isinstance(epochs, tuple) or
-              isinstance(epochs, np.ndarray)):
-            if (isinstance(epochs[0], complex) or
-                    isinstance(epochs[0], np.complex128)):
-                new_epochs = epochs
-            else:
-                raise ValueError('Bad data')
-        else:
-            raise ValueError('Bad data')
-        if (starttime is None):
-            stime = []
-            stime.append(-1.0E31)
-            stime.append(-1.0E31)
-        else:
-            if (isinstance(starttime, complex) or
-                    isinstance(starttime, np.complex128)):
-                stime = []
-                stime.append(starttime.real)
-                stime.append(starttime.imag)
-            elif (isinstance(starttime, list) or isinstance(starttime, tuple)):
-                sstime = CDFepoch.compute_epoch16(starttime)
-                stime = []
-                stime.append(sstime.real)
-                stime.append(sstime.imag)
-            else:
-                raise ValueError('Bad start time')
-        if (endtime is not None):
-            if (isinstance(endtime, complex) or
-                    isinstance(endtime, np.complex128)):
-                etime = []
-                etime.append(endtime.real)
-                etime.append(endtime.imag)
-            elif (isinstance(endtime, list) or isinstance(endtime, tuple)):
-                eetime = CDFepoch.compute_epoch16(endtime)
-                etime = []
-                etime.append(eetime.real)
-                etime.append(eetime.imag)
-            else:
-                raise ValueError('Bad start time')
-        else:
-            etime = []
-            etime.append(1.0E31)
-            etime.append(1.0E31)
-        if (stime[0] > etime[0] or (stime[0] == etime[0] and stime[1] > etime[1])):
-            raise ValueError('Invalid start/end time')
+    @staticmethod
+    def epochrange_epoch16(
+        epochs: cdf_epoch16_type, starttime: Optional[epoch_types] = None, endtime: Optional[epoch_types] = None
+    ) -> Optional[np.ndarray]:
+        new_epochs = np.atleast_1d(epochs)
+
+        stime: Tuple[Union[float, np.float64], Union[float, np.float64]]
+        etime: Tuple[Union[float, np.float64], Union[float, np.float64]]
+
+        if starttime is None:
+            stime = (-1.0e31, -1.0e31)
+        else:
+            if isinstance(starttime, complex) or isinstance(starttime, np.complex128):
+                stime = (starttime.real, starttime.imag)
+            elif isinstance(starttime, list):
+                sstime = complex(CDFepoch.compute_epoch16(starttime))
+                stime = (sstime.real, sstime.imag)
+            else:
+                raise ValueError("Bad start time")
+        if endtime is not None:
+            if isinstance(endtime, complex) or isinstance(endtime, np.complex128):
+                etime = (endtime.real, endtime.imag)
+            elif isinstance(endtime, list):
+                eetime = complex(CDFepoch.compute_epoch16(endtime))
+                etime = (eetime.real, eetime.imag)
+            else:
+                raise ValueError("Bad start time")
+        else:
+            etime = (1.0e31, 1.0e31)
+        if stime[0] > etime[0] or (stime[0] == etime[0] and stime[1] > etime[1]):
+            raise ValueError("Invalid start/end time")
         count = len(new_epochs)
         epoch16 = []
         for x in range(0, count):
             epoch16.append(new_epochs[x].real)
             epoch16.append(new_epochs[x].imag)
         count = count * 2
         indx = []
-        if (epoch16[0] > etime[0] or (epoch16[0] == etime[0] and
-                                      epoch16[1] > etime[1])):
-            return
-        if (epoch16[count - 2] < stime[0] or
-            (epoch16[count - 2] == stime[0] and
-             epoch16[count - 1] < stime[1])):
-            return
+        if epoch16[0] > etime[0] or (epoch16[0] == etime[0] and epoch16[1] > etime[1]):
+            return None
+        if epoch16[count - 2] < stime[0] or (epoch16[count - 2] == stime[0] and epoch16[count - 1] < stime[1]):
+            return None
         for x in range(0, count, 2):
-            if (epoch16[x] < stime[0]):
+            if epoch16[x] < stime[0]:
                 continue
-            elif (epoch16[x] == stime[0]):
-                if (epoch16[x + 1] < stime[1]):
+            elif epoch16[x] == stime[0]:
+                if epoch16[x + 1] < stime[1]:
                     continue
                 else:
                     indx.append(int(x / 2))
                     break
             else:
                 indx.append(int(x / 2))
                 break
-        if (len(indx) == 0):
+        if len(indx) == 0:
             indx.append(0)
         hasadded = False
         for x in range(0, count, 2):
-            if (epoch16[x] < etime[0]):
+            if epoch16[x] < etime[0]:
                 continue
-            elif (epoch16[x] == etime[0]):
-                if (epoch16[x + 1] > etime[1]):
+            elif epoch16[x] == etime[0]:
+                if epoch16[x + 1] > etime[1]:
                     indx.append(int((x - 1) / 2))
                     hasadded = True
                     break
             else:
                 indx.append(int((x - 1) / 2))
                 hasadded = True
                 break
         if not hasadded:
             indx.append(int(count / 2) - 1)
         return np.arange(indx[0], indx[1] + 1, step=1)
 
     @staticmethod
-    def encode_epoch(epochs, iso_8601: bool = True):  # @NoSelf
-
-        if isinstance(epochs, (float, np.float64)):
-            new_epochs = [epochs]
-        elif isinstance(epochs, (list, np.ndarray)):
-            new_epochs = epochs
-        else:
-            raise TypeError('Bad data')
+    def encode_epoch(epochs: cdf_epoch_type, iso_8601: bool = True) -> encoded_type:
+        new_epochs = np.atleast_1d(epochs)
 
         count = len(new_epochs)
         encodeds = []
         for x in range(0, count):
             epoch = new_epochs[x]
-            if (epoch == -1.0E31):
-                if (iso_8601):
-                    encoded = '9999-12-31T23:59:59.999'
+            if epoch == -1.0e31:
+                if iso_8601:
+                    encoded = "9999-12-31T23:59:59.999"
                 else:
-                    encoded = '31-Dec-9999 23:59:59.999'
+                    encoded = "31-Dec-9999 23:59:59.999"
             else:
                 encoded = CDFepoch._encodex_epoch(epoch, iso_8601)
-            if (count == 1):
+            if count == 1:
                 return encoded
             encodeds.append(encoded)
         return encodeds
 
     @staticmethod
-    def _encodex_epoch(epoch, iso_8601: bool = True):  # @NoSelf
-
+    def _encodex_epoch(epoch: cdf_epoch_type, iso_8601: bool = True) -> str:
         components = CDFepoch.breakdown_epoch(epoch)
-        if (iso_8601):
+        if iso_8601:
             # year-mm-ddThh:mm:ss.mmm
             encoded = str(components[0]).zfill(4)
-            encoded += '-'
+            encoded += "-"
             encoded += str(components[1]).zfill(2)
-            encoded += '-'
+            encoded += "-"
             encoded += str(components[2]).zfill(2)
-            encoded += 'T'
+            encoded += "T"
             encoded += str(components[3]).zfill(2)
-            encoded += ':'
+            encoded += ":"
             encoded += str(components[4]).zfill(2)
-            encoded += ':'
+            encoded += ":"
             encoded += str(components[5]).zfill(2)
-            encoded += '.'
+            encoded += "."
             encoded += str(components[6]).zfill(3)
         else:
             # dd-mmm-year hh:mm:ss.mmm
             encoded = str(components[2]).zfill(2)
-            encoded += '-'
+            encoded += "-"
             encoded += CDFepoch.month_Token[components[1] - 1]
-            encoded += '-'
+            encoded += "-"
             encoded += str(components[0]).zfill(4)
-            encoded += ' '
+            encoded += " "
             encoded += str(components[3]).zfill(2)
-            encoded += ':'
+            encoded += ":"
             encoded += str(components[4]).zfill(2)
-            encoded += ':'
+            encoded += ":"
             encoded += str(components[5]).zfill(2)
-            encoded += '.'
+            encoded += "."
             encoded += str(components[6]).zfill(3)
         return encoded
 
     @staticmethod
-    def compute_epoch(dates: Union[list, tuple], to_np: bool = False):
+    def compute_epoch(dates: npt.ArrayLike) -> Union[float, npt.NDArray]:
+        # TODO Add docstring. What is the output format?
+
+        new_dates = np.atleast_2d(dates)
+        count = new_dates.shape[0]
 
-        if (not isinstance(dates, list) and not isinstance(dates, tuple)):
-            raise ValueError('Bad input')
-        new_dates = [dates]
-        count = len(new_dates)
-        if (count == 0):
-            return
         epochs = []
         for x in range(0, count):
             date = new_dates[x]
             year = date[0]
             month = date[1]
             items = len(date)
-            if (items > 6):
+            if items > 6:
                 # y m d h m s ms
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 second = int(date[5])
                 msec = int(date[6])
-            elif (items > 5):
+            elif items > 5:
                 # y m d h m s
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 second = int(date[5])
                 msec = int(1000.0 * (date[5] - second))
-            elif (items > 4):
+            elif items > 4:
                 # y m d h m
                 day = int(date[2])
                 hour = int(date[3])
                 minute = int(date[4])
                 xxx = float(60.0 * (date[4] - minute))
                 second = int(xxx)
                 msec = int(1000.0 * (xxx - second))
-            elif (items > 3):
+            elif items > 3:
                 # y m d h
                 day = int(date[2])
                 hour = int(date[3])
                 xxx = float(60.0 * (date[3] - hour))
                 minute = int(xxx)
                 xxx = float(60.0 * (xxx - minute))
                 second = int(xxx)
                 msec = int(1000.0 * (xxx - second))
-            elif (items > 2):
+            elif items > 2:
                 # y m d
                 day = int(date[2])
                 xxx = float(24.0 * (date[2] - day))
                 hour = int(xxx)
                 xxx = float(60.0 * (xxx - hour))
                 minute = int(xxx)
                 xxx = float(60.0 * (xxx - minute))
                 second = int(xxx)
                 msec = int(1000.0 * (xxx - second))
             else:
-                raise ValueError('Invalid epoch components')
-            if (year == 9999 and month == 12 and day == 31 and hour == 23 and
-                    minute == 59 and second == 59 and msec == 999):
-                epochs.append(-1.0E31)
-            if (year < 0):
-                raise ValueError('ILLEGAL_EPOCH_FIELD')
-            if ((year > 9999) or (month < 0 or month > 12) or
-                (hour < 0 or hour > 23) or (minute < 0 or minute > 59) or
-                    (second < 0 or second > 59) or (msec < 0 or msec > 999)):
-                epochs.append(CDFepoch._computeEpoch(year, month, day, hour, minute,
-                                                     second, msec))
-            if (month == 0):
-                if (day < 1 or day > 366):
-                    epochs.append(CDFepoch._computeEpoch(year, month, day, hour,
-                                                         minute, second, msec))
-            else:
-                if (day < 1 or day > 31):
-                    epochs.append(CDFepoch._computeEpoch(year, month, day, hour,
-                                                         minute, second, msec))
-            if (hour == 0 and minute == 0 and second == 0):
-                if (msec < 0 or msec > 86399999):
-                    epochs.append(CDFepoch._computeEpoch(year, month, day, hour,
-                                                         minute, second, msec))
+                raise ValueError("Invalid epoch components")
+            if year == 9999 and month == 12 and day == 31 and hour == 23 and minute == 59 and second == 59 and msec == 999:
+                epochs.append(-1.0e31)
+            if year < 0:
+                raise ValueError("ILLEGAL_EPOCH_FIELD")
+            if (
+                (year > 9999)
+                or (month < 0 or month > 12)
+                or (hour < 0 or hour > 23)
+                or (minute < 0 or minute > 59)
+                or (second < 0 or second > 59)
+                or (msec < 0 or msec > 999)
+            ):
+                epochs.append(CDFepoch._computeEpoch(year, month, day, hour, minute, second, msec))
+            if month == 0:
+                if day < 1 or day > 366:
+                    epochs.append(CDFepoch._computeEpoch(year, month, day, hour, minute, second, msec))
+            else:
+                if day < 1 or day > 31:
+                    epochs.append(CDFepoch._computeEpoch(year, month, day, hour, minute, second, msec))
+            if hour == 0 and minute == 0 and second == 0:
+                if msec < 0 or msec > 86399999:
+                    epochs.append(CDFepoch._computeEpoch(year, month, day, hour, minute, second, msec))
 
-            if (month == 0):
+            if month == 0:
                 daysSince0AD = CDFepoch._JulianDay(year, 1, 1) + (day - 1) - 1721060
             else:
                 daysSince0AD = CDFepoch._JulianDay(year, month, day) - 1721060
-            if (hour == 0 and minute == 0 and second == 0):
+            if hour == 0 and minute == 0 and second == 0:
                 msecInDay = msec
             else:
                 msecInDay = (3600000 * hour) + (60000 * minute) + (1000 * second) + msec
-            if (count == 1):
-                if not to_np:
-                    return (86400000.0 * daysSince0AD + msecInDay)
-                else:
-                    return np.array(86400000.0 * daysSince0AD + msecInDay)
+            if count == 1:
+                return np.array(86400000.0 * daysSince0AD + msecInDay)
             epochs.append(86400000.0 * daysSince0AD + msecInDay)
-        if not to_np:
-            return epochs
-        else:
-            return np.array(epochs)
 
-    def _computeEpoch(y, m, d, h, mn, s, ms):  # @NoSelf
+        return _squeeze_or_scalar_real(epochs)
 
-        if (m == 0):
+    @staticmethod
+    def _computeEpoch(y: int, m: int, d: int, h: int, mn: int, s: int, ms: int) -> float:
+        if m == 0:
             daysSince0AD = CDFepoch._JulianDay(y, 1, 1) + (d - 1) - 1721060
         else:
-            if (m < 0):
+            if m < 0:
                 --y
                 m = 13 + m
             daysSince0AD = CDFepoch._JulianDay(y, m, d) - 1721060
-        if (daysSince0AD < 1):
-            raise ValueError('ILLEGAL_EPOCH_FIELD')
+        if daysSince0AD < 1:
+            raise ValueError("ILLEGAL_EPOCH_FIELD")
         msecInDay = float(3600000.0 * h + 60000.0 * mn + 1000.0 * s) + float(ms)
         msecFromEpoch = float(86400000.0 * daysSince0AD + msecInDay)
-        if (msecFromEpoch < 0.0):
+        if msecFromEpoch < 0.0:
             return -1.0
         else:
             return msecFromEpoch
 
     @staticmethod
-    def breakdown_epoch(epochs, to_np: bool = False):
-        """ Calculate date and time from epochs
+    def breakdown_epoch(epochs: cdf_epoch_type) -> np.ndarray:
+        """Calculate date and time from epochs
 
         Parameters
         ----------
         epochs : int, float, or array-like
             Single, list, tuple, or np.array of epoch values
-        to_np : bool
-            Flag for output type, if True will be an np.array, if False
-            will be a list (default=False)
 
         Returns
         -------
-        components : list-like of ints
+        components : list
             List or array of date and time values.  The last axis contains
             (in order): year, month, day, hour, minute, second, and millisecond
 
         Notes
         -----
         If a bad epoch (-1.0e31) is supplied, a fill date of
         9999-12-31 23:59:59 and 999 ms is returned.
 
         """
         # Test input and cast it as an array of floats
-        if (isinstance(epochs, float) or isinstance(epochs, np.float64)
-            or isinstance(epochs, list) or isinstance(epochs, tuple)
-                or isinstance(epochs, np.ndarray) or isinstance(epochs, int)):
+        if (
+            isinstance(epochs, float)
+            or isinstance(epochs, np.float64)
+            or isinstance(epochs, list)
+            or isinstance(epochs, tuple)
+            or isinstance(epochs, np.ndarray)
+            or isinstance(epochs, int)
+        ):
             new_epochs = np.asarray(epochs).astype(float)
             if new_epochs.shape == ():
                 cshape = []
                 new_epochs = np.array([epochs], dtype=float)
             else:
                 cshape = list(new_epochs.shape)
         else:
-            raise TypeError('Bad data for epochs: {:}'.format(type(epochs)))
+            raise TypeError("Bad data for epochs: {:}".format(type(epochs)))
 
         # Initialize output to default values
         cshape.append(7)
-        components = np.full(shape=cshape, fill_value=[9999, 12, 31, 23, 59,
-                                                       59, 999])
+        components = np.full(shape=cshape, fill_value=[9999, 12, 31, 23, 59, 59, 999])
         for i, epoch in enumerate(new_epochs):
             # Ignore fill values
-            if epoch != -1.0E31:
+            if epoch != -1.0e31:
                 esec = -epoch / 1000.0 if epoch < 0.0 else epoch / 1000.0
                 date_time = CDFepoch._calc_from_julian(esec, 0.0)
 
                 ms = (epoch % 1000.0).astype(int)
                 date_time[..., 6] = int(ms) if ms.shape == () else ms
 
                 if len(components.shape) == 1:
                     components = date_time[..., :7]
                 else:
                     components[i] = date_time[..., :7]
 
-        if to_np:
-            return components
-        else:
-            comp = components.tolist()
-            if len(comp) == 1:
-                return comp[0]
-            return comp
+        return np.squeeze(components)
 
     @staticmethod
-    def epochrange_epoch(epochs, starttime=None, endtime=None):  # @NoSelf
-
+    def epochrange_epoch(
+        epochs: epoch_types, starttime: Optional[epoch_types] = None, endtime: Optional[epoch_types] = None
+    ) -> np.ndarray:
         if isinstance(epochs, (float, np.float64)):
             pass
         elif isinstance(epochs, (list, tuple, np.ndarray)):
             if isinstance(epochs[0], (float, np.float64)):
                 pass
             else:
-                raise TypeError('Bad data')
+                raise TypeError("Bad data")
         else:
-            raise TypeError('Bad data')
+            raise TypeError("Bad data")
 
-        if (starttime is None):
+        stime: Union[float, np.float64]
+        if starttime is None:
             stime = 0.0
         else:
             if isinstance(starttime, (float, int, np.float64)):
                 stime = starttime
             elif isinstance(starttime, (list, tuple)):
-                stime = CDFepoch.compute_epoch(starttime)
+                stime = float(CDFepoch.compute_epoch(starttime))
             else:
-                raise TypeError('Bad start time')
+                raise TypeError("Bad start time")
 
-        if (endtime is not None):
+        if endtime is not None:
             if isinstance(endtime, (float, int, np.float64)):
                 etime = endtime
             elif isinstance(endtime, (list, tuple)):
-                etime = CDFepoch.compute_epoch(endtime)
+                etime = float(CDFepoch.compute_epoch(endtime))
             else:
-                raise TypeError('Bad end time')
+                raise TypeError("Bad end time")
         else:
-            etime = 1.0E31
-        if (stime > etime):
-            raise ValueError('Invalid start/end time')
+            etime = 1.0e31
+        if stime > etime:
+            raise ValueError("Invalid start/end time")
 
-        if isinstance(epochs, (list, tuple)):
-            new_epochs = np.array(epochs)
-        else:
-            new_epochs = epochs
+        new_epochs = np.array(epochs)
         return np.where(np.logical_and(new_epochs >= stime, new_epochs <= etime))[0]
 
     @staticmethod
-    def parse(value, to_np: bool = False):
+    def parse(value: Union[str, Tuple[str, ...], List[str]]) -> np.ndarray:
         """
         Parses the provided date/time string(s) into CDF epoch value(s).
 
         For CDF_EPOCH:
-                The string has to be in the form of 'dd-mmm-yyyy hh:mm:ss.xxx' or
-                'yyyy-mm-ddThh:mm:ss.xxx' (in iso_8601). The string is the output
-                from encode function.
+            The string has to be in the form of 'dd-mmm-yyyy hh:mm:ss.xxx' or
+            'yyyy-mm-ddThh:mm:ss.xxx' (in iso_8601). The string is the output
+            from encode function.
 
         For CDF_EPOCH16:
-                The string has to be in the form of
-                'dd-mmm-yyyy hh:mm:ss.mmm.uuu.nnn.ppp' or
-                'yyyy-mm-ddThh:mm:ss.mmmuuunnnppp' (in iso_8601). The string is
-                the output from encode function.
+            The string has to be in the form of
+            'dd-mmm-yyyy hh:mm:ss.mmm.uuu.nnn.ppp' or
+            'yyyy-mm-ddThh:mm:ss.mmmuuunnnppp' (in iso_8601). The string is
+            the output from encode function.
 
         For TT2000:
-                The string has to be in the form of
-                'dd-mmm-yyyy hh:mm:ss.mmm.uuu.nnn' or
-                'yyyy-mm-ddThh:mm:ss.mmmuuunnn' (in iso_8601). The string is
-                the output from encode function.
-
-        Specify to_np to True, if the result should be in numpy class.
+            The string has to be in the form of
+            'dd-mmm-yyyy hh:mm:ss.mmm.uuu.nnn' or
+            'yyyy-mm-ddThh:mm:ss.mmmuuunnn' (in iso_8601). The string is
+            the output from encode function.
         """
         if isinstance(value, (list, tuple)) and not isinstance(value[0], str):
-            raise TypeError('should be a string or a list of string')
+            raise TypeError("should be a string or a list of string")
 
         elif not isinstance(value, (list, tuple, str)):
-            raise TypeError('Invalid value... should be a string or a list of string')
+            raise TypeError("Invalid value... should be a string or a list of string")
         else:
             if isinstance(value, (list, tuple)):
                 num = len(value)
                 epochs = []
                 for x in range(num):
                     epochs.append(CDFepoch._parse_epoch(value[x]))
-                if not to_np:
-                    return epochs
-                else:
-                    return np.array(epochs)
+                return np.squeeze(epochs)
             else:
-                if not to_np:
-                    return CDFepoch._parse_epoch(value)
-                else:
-                    return np.array(CDFepoch._parse_epoch(value))
+                return np.squeeze(CDFepoch._parse_epoch(value))
 
     @staticmethod
-    def _parse_epoch(value):
-        if isinstance(value, (list, tuple)):
-            epochs = []
-            for x in range(0, len(value)):
-                epochs.append(value[x])
-            return epochs
-        else:
-            if len(value) in (23, 24):
-                # CDF_EPOCH
-                if value.lower() in ('31-dec-9999 23:59:59.999',
-                                     '9999-12-31t23:59:59.999'):
-                    return -1.0E31
-                else:
-                    if len(value) == 24:
-                        date = re.findall(r'(\d+)\-(.+)\-(\d+) (\d+)\:(\d+)\:(\d+)\.(\d+)', value)
-                        dd = int(date[0][0])
-                        mm = CDFepoch._month_index(date[0][1])
-                        yy = int(date[0][2])
-                        hh = int(date[0][3])
-                        mn = int(date[0][4])
-                        ss = int(date[0][5])
-                        ms = int(date[0][6])
-                    else:
-                        date = re.findall(r'(\d+)\-(\d+)\-(\d+)T(\d+)\:(\d+)\:(\d+)\.(\d+)',
-                                          value)
-                        yy = int(date[0][0])
-                        mm = int(date[0][1])
-                        dd = int(date[0][2])
-                        hh = int(date[0][3])
-                        mn = int(date[0][4])
-                        ss = int(date[0][5])
-                        ms = int(date[0][6])
-                    return CDFepoch.compute_epoch([yy, mm, dd, hh, mn, ss, ms])
-            elif len(value) == 36 or (len(value) == 32 and
-                                      value[10].lower() == 't'):
-                # CDF_EPOCH16
-                if value.lower() in ('31-dec-9999 23:59:59.999.999.999.999',
-                                     '9999-12-31t23:59:59.999999999999'):
-                    return -1.0E31 - 1.0E31j
-                else:
-                    if (len(value) == 36):
-                        date = re.findall(r'(\d+)\-(.+)\-(\d+) (\d+)\:(\d+)\:(\d+)\.(\d+)\.(\d+)\.(\d+)\.(\d+)',
-                                          value)
-                        dd = int(date[0][0])
-                        mm = CDFepoch._month_index(date[0][1])
-                        yy = int(date[0][2])
-                        hh = int(date[0][3])
-                        mn = int(date[0][4])
-                        ss = int(date[0][5])
-                        ms = int(date[0][6])
-                        us = int(date[0][7])
-                        ns = int(date[0][8])
-                        ps = int(date[0][9])
-                    else:
-                        date = re.findall(r'(\d+)\-(\d+)\-(\d+)T(\d+)\:(\d+)\:(\d+)\.(\d+)',
-                                          value)
-                        yy = int(date[0][0])
-                        mm = int(date[0][1])
-                        dd = int(date[0][2])
-                        hh = int(date[0][3])
-                        mn = int(date[0][4])
-                        ss = int(date[0][5])
-                        subs = int(date[0][6])
-                        ms = int(subs / 1000000000)
-                        subms = int(subs % 1000000000)
-                        us = int(subms / 1000000)
-                        subus = int(subms % 1000000)
-                        ns = int(subus / 1000)
-                        ps = int(subus % 1000)
-                    return CDFepoch.compute_epoch16([yy, mm, dd, hh, mn, ss, ms, us, ns, ps])
-            elif (len(value) == 29 or (len(value) == 32 and
-                                       value[11] == ' ')):
-                # CDF_TIME_TT2000
-                value = value.lower()
-                if (value == '9999-12-31t23:59:59.999999999' or
-                        value == '31-dec-9999 23:59:59.999.999.999'):
-                    return -9223372036854775808
-                elif (value == '0000-01-01t00:00.000000000' or
-                      value == '01-jan-0000 00:00.000.000.000'):
-                    return -9223372036854775807
-                else:
-                    if (len(value) == 29):
-                        date = re.findall(r'(\d+)\-(\d+)\-(\d+)t(\d+)\:(\d+)\:(\d+)\.(\d+)',
-                                          value)
-                        yy = int(date[0][0])
-                        mm = int(date[0][1])
-                        dd = int(date[0][2])
-                        hh = int(date[0][3])
-                        mn = int(date[0][4])
-                        ss = int(date[0][5])
-                        subs = int(date[0][6])
-                        ms = int(subs / 1000000)
-                        subms = int(subs % 1000000)
-                        us = int(subms / 1000)
-                        ns = int(subms % 1000)
-                    else:
-                        date = re.findall(r'(\d+)\-(.+)\-(\d+) (\d+)\:(\d+)\:(\d+)\.(\d+)\.(\d+)\.(\d+)',
-                                          value)
-                        dd = int(date[0][0])
-                        mm = CDFepoch._month_index(date[0][1])
-                        yy = int(date[0][2])
-                        hh = int(date[0][3])
-                        mn = int(date[0][4])
-                        ss = int(date[0][5])
-                        ms = int(date[0][6])
-                        us = int(date[0][7])
-                        ns = int(date[0][8])
-                    return CDFepoch.compute_tt2000([yy, mm, dd, hh, mn, ss, ms, us, ns])
-            else:
-                raise ValueError('Invalid cdf epoch type...')
+    def _parse_epoch(value: str) -> Union[int, float, complex]:
+        if len(value) in (23, 24):
+            # CDF_EPOCH
+            if value.lower() in ("31-dec-9999 23:59:59.999", "9999-12-31t23:59:59.999"):
+                return -1.0e31
+            else:
+                if len(value) == 24:
+                    date = re.findall(r"(\d+)\-(.+)\-(\d+) (\d+)\:(\d+)\:(\d+)\.(\d+)", value)
+                    dd = int(date[0][0])
+                    mm = CDFepoch._month_index(date[0][1])
+                    yy = int(date[0][2])
+                    hh = int(date[0][3])
+                    mn = int(date[0][4])
+                    ss = int(date[0][5])
+                    ms = int(date[0][6])
+                else:
+                    date = re.findall(r"(\d+)\-(\d+)\-(\d+)T(\d+)\:(\d+)\:(\d+)\.(\d+)", value)
+                    yy = int(date[0][0])
+                    mm = int(date[0][1])
+                    dd = int(date[0][2])
+                    hh = int(date[0][3])
+                    mn = int(date[0][4])
+                    ss = int(date[0][5])
+                    ms = int(date[0][6])
+                return float(CDFepoch.compute_epoch([yy, mm, dd, hh, mn, ss, ms]))
+        elif len(value) == 36 or (len(value) == 32 and value[10].lower() == "t"):
+            # CDF_EPOCH16
+            if value.lower() in ("31-dec-9999 23:59:59.999.999.999.999", "9999-12-31t23:59:59.999999999999"):
+                return -1.0e31 - 1.0e31j
+            else:
+                if len(value) == 36:
+                    date = re.findall(r"(\d+)\-(.+)\-(\d+) (\d+)\:(\d+)\:(\d+)\.(\d+)\.(\d+)\.(\d+)\.(\d+)", value)
+                    dd = int(date[0][0])
+                    mm = CDFepoch._month_index(date[0][1])
+                    yy = int(date[0][2])
+                    hh = int(date[0][3])
+                    mn = int(date[0][4])
+                    ss = int(date[0][5])
+                    ms = int(date[0][6])
+                    us = int(date[0][7])
+                    ns = int(date[0][8])
+                    ps = int(date[0][9])
+                else:
+                    date = re.findall(r"(\d+)\-(\d+)\-(\d+)T(\d+)\:(\d+)\:(\d+)\.(\d+)", value)
+                    yy = int(date[0][0])
+                    mm = int(date[0][1])
+                    dd = int(date[0][2])
+                    hh = int(date[0][3])
+                    mn = int(date[0][4])
+                    ss = int(date[0][5])
+                    subs = int(date[0][6])
+                    ms = int(subs / 1000000000)
+                    subms = int(subs % 1000000000)
+                    us = int(subms / 1000000)
+                    subus = int(subms % 1000000)
+                    ns = int(subus / 1000)
+                    ps = int(subus % 1000)
+                return complex(CDFepoch.compute_epoch16([yy, mm, dd, hh, mn, ss, ms, us, ns, ps]))
+        elif len(value) == 29 or (len(value) == 32 and value[11] == " "):
+            # CDF_TIME_TT2000
+            value = value.lower()
+            if value == "9999-12-31t23:59:59.999999999" or value == "31-dec-9999 23:59:59.999.999.999":
+                return -9223372036854775808
+            elif value == "0000-01-01t00:00.000000000" or value == "01-jan-0000 00:00.000.000.000":
+                return -9223372036854775807
+            else:
+                if len(value) == 29:
+                    date = re.findall(r"(\d+)\-(\d+)\-(\d+)t(\d+)\:(\d+)\:(\d+)\.(\d+)", value)
+                    yy = int(date[0][0])
+                    mm = int(date[0][1])
+                    dd = int(date[0][2])
+                    hh = int(date[0][3])
+                    mn = int(date[0][4])
+                    ss = int(date[0][5])
+                    subs = int(date[0][6])
+                    ms = int(subs / 1000000)
+                    subms = int(subs % 1000000)
+                    us = int(subms / 1000)
+                    ns = int(subms % 1000)
+                else:
+                    date = re.findall(r"(\d+)\-(.+)\-(\d+) (\d+)\:(\d+)\:(\d+)\.(\d+)\.(\d+)\.(\d+)", value)
+                    dd = int(date[0][0])
+                    mm = CDFepoch._month_index(date[0][1])
+                    yy = int(date[0][2])
+                    hh = int(date[0][3])
+                    mn = int(date[0][4])
+                    ss = int(date[0][5])
+                    ms = int(date[0][6])
+                    us = int(date[0][7])
+                    ns = int(date[0][8])
+                return int(CDFepoch.compute_tt2000([yy, mm, dd, hh, mn, ss, ms, us, ns]))
+        else:
+            raise ValueError("Invalid cdf epoch type...")
 
-    def _month_index(month):  # @NoSelf
-        if (month.lower() == 'jan'):
+    @staticmethod
+    def _month_index(month: str) -> int:
+        if month.lower() == "jan":
             return 1
-        elif(month.lower() == 'feb'):
+        elif month.lower() == "feb":
             return 2
-        elif(month.lower() == 'mar'):
+        elif month.lower() == "mar":
             return 3
-        elif(month.lower() == 'apr'):
+        elif month.lower() == "apr":
             return 4
-        elif(month.lower() == 'may'):
+        elif month.lower() == "may":
             return 5
-        elif(month.lower() == 'jun'):
+        elif month.lower() == "jun":
             return 6
-        elif(month.lower() == 'jul'):
+        elif month.lower() == "jul":
             return 7
-        elif(month.lower() == 'aug'):
+        elif month.lower() == "aug":
             return 8
-        elif(month.lower() == 'sep'):
+        elif month.lower() == "sep":
             return 9
-        elif(month.lower() == 'oct'):
+        elif month.lower() == "oct":
             return 10
-        elif(month.lower() == 'nov'):
+        elif month.lower() == "nov":
             return 11
-        elif(month.lower() == 'dec'):
+        elif month.lower() == "dec":
             return 12
         else:
             return -1
```

### Comparing `cdflib-0.4.9/cdflib/epochs_astropy.py` & `cdflib-1.0.0/cdflib/epochs_astropy.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,61 +3,62 @@
 CDF Astropy Epochs
 ##################
 
 @author: Bryan Harter
 """
 import datetime
 from datetime import timezone
-from typing import List
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
+import numpy.typing as npt
 from astropy.time import Time
 from astropy.time.formats import TimeFromEpoch, erfa
 
-__all__ = ['CDFAstropy']
+__all__ = ["CDFAstropy"]
 
 
 class CDFEpoch(TimeFromEpoch):
-    name = 'cdf_epoch'
+    name = "cdf_epoch"
     unit = 1.0 / (erfa.DAYSEC * 1000)  # Milliseconds
-    epoch_val = '0000-01-01 00:00:00'
+    epoch_val = "0000-01-01 00:00:00"
     epoch_val2 = None
-    epoch_scale = 'utc'
-    epoch_format = 'iso'
+    epoch_scale = "utc"
+    epoch_format = "iso"
 
 
 class CDFEpoch16(TimeFromEpoch):
-    name = 'cdf_epoch16'
+    name = "cdf_epoch16"
     unit = 1.0 / (erfa.DAYSEC)  # Seconds
-    epoch_val = '0000-01-01 00:00:00'
+    epoch_val = "0000-01-01 00:00:00"
     epoch_val2 = None
-    epoch_scale = 'utc'
-    epoch_format = 'iso'
+    epoch_scale = "utc"
+    epoch_format = "iso"
 
 
 class CDFTT2000(TimeFromEpoch):
-    name = 'cdf_tt2000'
+    name = "cdf_tt2000"
     unit = 1.0 / (erfa.DAYSEC * 1e9)  # Nanoseconds
-    epoch_val = '2000-01-01 12:00:00'
+    epoch_val = "2000-01-01 12:00:00"
     epoch_val2 = None
-    epoch_scale = 'tt'
-    epoch_format = 'iso'
+    epoch_scale = "tt"
+    epoch_format = "iso"
 
 
 class CDFAstropy:
     """
     Class to encapsulate astropy time routines with CDF class.
     """
 
     version = 3
     release = 7
     increment = 0
 
     @staticmethod
-    def convert_to_astropy(epochs, format=None):
+    def convert_to_astropy(epochs: Union[Time, npt.ArrayLike], format: Optional[str] = None) -> Time:
         """
         Convert CDF epochs to astropy time objects.
 
         Returns
         -------
         astropy.time.Time
         """
@@ -65,110 +66,98 @@
         if isinstance(epochs, Time):
             return epochs
 
         # If format is specified, then force it to do that
         if format is not None:
             return Time(epochs, format=format, precision=9)
 
-        if isinstance(epochs, (list, np.ndarray)):
-            t = type(epochs[0])
-        else:
-            t = type(epochs)
+        epochs = np.array(epochs)
 
         # Determine best format for the input type
-        if t in (int, np.int64):
-            return Time(epochs, format='cdf_tt2000', precision=9)
-        elif t in (complex, np.complex128):
-            return Time(epochs.real, epochs.imag / 1000000000000.0, format='cdf_epoch16', precision=9)
-        elif t in (float, np.float64):
-            return Time(epochs, format='cdf_epoch', precision=9)
+        if epochs.dtype == np.int64:
+            return Time(epochs, format="cdf_tt2000", precision=9)
+        elif epochs.dtype == np.complex128:
+            return Time(epochs.real, epochs.imag / 1000000000000.0, format="cdf_epoch16", precision=9)
+        elif epochs.dtype == np.float64:
+            return Time(epochs, format="cdf_epoch", precision=9)
         else:
-            raise TypeError('Not sure how to handle type {}'.format(type(epochs)))
+            raise TypeError("Not sure how to handle type {}".format(type(epochs)))
 
     @staticmethod
-    def encode(epochs, iso_8601: bool = True):  # @NoSelf
+    def encode(epochs: npt.ArrayLike, iso_8601: bool = True) -> npt.NDArray[np.str_]:
         epochs = CDFAstropy.convert_to_astropy(epochs)
         if iso_8601:
             return epochs.iso
         else:
-            return epochs.strftime('%d-%b-%Y %H:%M:%S.%f')
+            return epochs.strftime("%d-%b-%Y %H:%M:%S.%f")
 
     @staticmethod
-    def breakdown(epochs, to_np: bool = False):
+    def breakdown(epochs: Union[Time, npt.ArrayLike]) -> npt.NDArray:
         # Returns either a single array, or a array of arrays depending on the input
         epochs = CDFAstropy.convert_to_astropy(epochs)
-        if epochs.format == 'cdf_tt2000':
-            return CDFAstropy.breakdown_tt2000(epochs, to_np)
-        elif epochs.format == 'cdf_epoch':
-            return CDFAstropy.breakdown_epoch(epochs, to_np)
-        elif epochs.format == 'cdf_epoch16':
-            return CDFAstropy.breakdown_epoch16(epochs, to_np)
-        raise TypeError('Not sure how to handle type {}'.format(type(epochs)))
+        if epochs.format == "cdf_tt2000":
+            return CDFAstropy.breakdown_tt2000(epochs)
+        elif epochs.format == "cdf_epoch":
+            return CDFAstropy.breakdown_epoch(epochs)
+        elif epochs.format == "cdf_epoch16":
+            return CDFAstropy.breakdown_epoch16(epochs)
+        raise TypeError("Not sure how to handle type {}".format(type(epochs)))
 
     @staticmethod
-    def to_datetime(cdf_time) -> List[datetime.datetime]:
+    def to_datetime(cdf_time: npt.ArrayLike) -> Time:
         cdf_time = CDFAstropy.convert_to_astropy(cdf_time)
         return cdf_time.datetime
 
     @staticmethod
-    def unixtime(cdf_time, to_np: bool = False):  # @NoSelf
+    def unixtime(cdf_time: Union[Time, npt.ArrayLike]) -> npt.NDArray:
         """
         Encodes the epoch(s) into seconds after 1970-01-01.  Precision is only
         kept to the nearest microsecond.
-
-        If to_np is True, then the values will be returned in a numpy array.
         """
         epochs = CDFAstropy.convert_to_astropy(cdf_time)
-        if to_np:
-            return epochs.unix
-        else:
-            return epochs.unix.tolist()
+        return epochs.unix
 
     @staticmethod
-    def compute(datetimes, to_np: bool = False):  # @NoSelf
-        if not isinstance(datetimes[0], list):
-            datetimes = [datetimes]
+    def compute(datetimes: npt.ArrayLike) -> npt.NDArray:
+        datetimes = np.atleast_2d(datetimes)
         cdf_time = []
         for d in datetimes:
             unix_seconds = datetime.datetime(d[0], d[1], d[2], d[3], d[4], d[5]).replace(tzinfo=timezone.utc).timestamp()
             if len(d) == 7:
-                remainder_seconds = (d[6] / 1000.0)
-                astrotime = Time(unix_seconds, remainder_seconds, format='unix', precision=9)
+                remainder_seconds = d[6] / 1000.0
+                astrotime = Time(unix_seconds, remainder_seconds, format="unix", precision=9)
                 cdf_time.append(astrotime.cdf_epoch)
             if len(d) == 9:
                 remainder_seconds = (d[6] / 1000.0) + (d[7] / 1000000.0) + (d[8] / 1000000000.0)
-                astrotime = Time(unix_seconds, remainder_seconds, format='unix', precision=9)
+                astrotime = Time(unix_seconds, remainder_seconds, format="unix", precision=9)
                 cdf_time.append(astrotime.cdf_tt2000)
             if len(d) == 10:
                 remainder_seconds = (d[6] / 1000.0) + (d[7] / 1000000.0) + (d[8] / 1000000000.0) + (d[9] / 1000000000000.0)
-                astrotime = Time(unix_seconds, remainder_seconds, format='unix', precision=9)
+                astrotime = Time(unix_seconds, remainder_seconds, format="unix", precision=9)
                 cdf_time.append(astrotime.cdf_epoch16)
-        if to_np:
-            return np.array(cdf_time)
-        else:
-            return cdf_time
+        return np.squeeze(cdf_time)
 
     @staticmethod
-    def findepochrange(epochs, starttime=None, endtime=None):  # @NoSelf
+    def findepochrange(
+        epochs: Union[Time, npt.ArrayLike], starttime: Optional[npt.ArrayLike] = None, endtime: Optional[npt.ArrayLike] = None
+    ) -> Tuple[int, int]:
         if isinstance(starttime, list):
             start = CDFAstropy.compute(starttime)
         if isinstance(endtime, list):
             end = CDFAstropy.compute(endtime)
 
         epochs = CDFAstropy.convert_to_astropy(epochs)
 
         epochs_as_np = epochs.value
         indices = np.where((epochs_as_np >= start) & (epochs_as_np <= end))
         return min(indices[0]), max(indices[0])
 
     @staticmethod
-    def breakdown_tt2000(tt2000, to_np: bool = False):
-        tt2000strings = tt2000.iso
-        if not isinstance(tt2000strings, (list, np.ndarray)):
-            tt2000strings = [tt2000strings]
+    def breakdown_tt2000(tt2000: Time) -> npt.NDArray:
+        tt2000strings = np.atleast_1d(tt2000.iso)
         times = []
         for t in tt2000strings:
             date, time = t.split(" ")
             yyyy, mon, dd = date.split("-")
             hhmmss, decimal_seconds = time.split(".")
             decimal_seconds = "." + decimal_seconds
             hh, mm, ss = hhmmss.split(":")
@@ -184,21 +173,19 @@
             time_as_list.append(int(milliseconds))  # milliseconds
             microseconds = (milliseconds % 1) * 1000
             time_as_list.append(int(microseconds))  # microseconds
             nanoseconds = (microseconds % 1) * 1000
             time_as_list.append(int(nanoseconds))  # microseconds
             times.append(time_as_list)
 
-        return times
+        return np.squeeze(times)
 
     @staticmethod
-    def breakdown_epoch16(epochs, to_np: bool = False):  # @NoSelf
-        epoch16strings = epochs.iso
-        if not isinstance(epoch16strings, (list, np.ndarray)):
-            epoch16strings = [epoch16strings]
+    def breakdown_epoch16(epochs: Time) -> npt.NDArray:
+        epoch16strings = np.atleast_1d(epochs.iso)
         times = []
         for t in epoch16strings:
             time_as_list: List[int] = []
             date, time = t.split(" ")
             yyyy, mon, dd = date.split("-")
             hhmmss, decimal_seconds = time.split(".")
             decimal_seconds = "." + decimal_seconds
@@ -217,21 +204,20 @@
             time_as_list.append(int(microseconds))  # microseconds
             nanoseconds = (microseconds % 1) * 1000
             time_as_list.append(int(nanoseconds))  # nanoseconds
             picoseconds = (nanoseconds % 1) * 1000
             time_as_list.append(int(picoseconds))  # picoseconds
             times.append(time_as_list)
 
-        return times
+        return np.squeeze(times)
 
     @staticmethod
-    def breakdown_epoch(epochs, to_np: bool = False):  # @NoSelf
-        epochstrings = epochs.iso
-        if not isinstance(epochstrings, (list, np.ndarray)):
-            epochstrings = [epochstrings]
+    def breakdown_epoch(epochs: Time) -> npt.NDArray:
+        epochstrings = np.atleast_1d(epochs.iso)
+
         times = []
         for t in epochstrings:
             date, time = t.split(" ")
             yyyy, mon, dd = date.split("-")
             hhmmss, decimal_seconds = time.split(".")
             decimal_seconds = "." + decimal_seconds
             hh, mm, ss = hhmmss.split(":")
@@ -242,18 +228,18 @@
             time_as_list.append(int(hh))  # hour
             time_as_list.append(int(mm))  # minute
             time_as_list.append(int(ss))  # second
             decimal_seconds = float(decimal_seconds)
             milliseconds = decimal_seconds * 1000
             time_as_list.append(int(milliseconds))  # milliseconds
             times.append(time_as_list)
-        return times
+        return np.squeeze(times)
 
     @staticmethod
-    def parse(value, to_np: bool = False):  # @NoSelf
+    def parse(value: npt.ArrayLike) -> npt.NDArray:
         """
         Parses the provided date/time string(s) into CDF epoch value(s).
 
         For CDF_EPOCH:
                 'yyyy-mm-dd hh:mm:ss.xxx' (in iso_8601). The string is the output
                 from encode function.
 
@@ -262,28 +248,22 @@
                 'yyyy-mm-dd hh:mm:ss.mmmuuunnnppp' (in iso_8601). The string is
                 the output from encode function.
 
         For TT2000:
                 The string has to be in the form of
                 'yyyy-mm-dd hh:mm:ss.mmmuuunnn' (in iso_8601). The string is
                 the output from encode function.
-
-        Specify to_np to True, if the result should be in numpy class.
         """
-        if not isinstance(value, (list, np.ndarray)):
-            value = [value]
+        value = np.atleast_1d(value)
 
         time_list = []
 
         for t in value:
             date, subs = t.split(".")
             if len(subs) == 3:
                 time_list.append(Time(t, precision=9).cdf_epoch)
             if len(subs) == 12:
                 time_list.append(Time(t, precision=9).cdf_epoch16)
             if len(subs) == 9:
                 time_list.append(int(Time(t, precision=9).cdf_tt2000))
 
-        if not to_np:
-            return time_list
-        else:
-            return np.array(time_list)
+        return np.squeeze(time_list)
```

### Comparing `cdflib-0.4.9/cdflib/xarray_to_cdf.py` & `cdflib-1.0.0/cdflib/xarray_to_cdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,483 +1,512 @@
 import os
 import re
 from datetime import datetime
+from typing import Any, Dict, List, Tuple, Union, cast
 
 import numpy as np
+import numpy.typing as npt
+import xarray as xr
 
 from cdflib.cdfwrite import CDF
 from cdflib.epochs import CDFepoch as cdfepoch
 
 
-def _dtype_to_cdf_type(var):
-
-    epoch_regex_1 = re.compile('epoch$')
-    epoch_regex_2 = re.compile('epoch_[0-9]+$')
+def _dtype_to_cdf_type(var: xr.Dataset) -> Tuple[int, int]:
+    epoch_regex_1 = re.compile("epoch$")
+    epoch_regex_2 = re.compile("epoch_[0-9]+$")
     if epoch_regex_1.match(var.name.lower()) or epoch_regex_2.match(var.name.lower()):
         return 33, 1  # CDF_EPOCH_TT2000
 
     if var.dtype == np.int8 or var.dtype == np.int16 or var.dtype == np.int32 or var.dtype == np.int64:
         return 8, 1  # 'CDF_INT8'
     elif var.dtype == np.float64 or var.dtype == np.float32 or var.dtype == np.float16:
         return 45, 1  # 'CDF_DOUBLE'
     elif var.dtype == np.uint8 or var.dtype == np.uint16 or var.dtype == np.uint32 or var.dtype == np.uint64:
         return 14, 1  # 'CDF_UNIT4'
     elif var.dtype.type == np.str_:
         return 51, int(var.dtype.str[2:])  # CDF_CHAR, and the length of the longest string in the numpy array
     elif var.dtype.type == np.bytes_:  # Bytes are usually strings
         return 51, int(var.dtype.str[2:])  # CDF_CHAR, and the length of the longest string in the numpy array
-    elif var.dtype == np.object:  # This commonly means we have multidimensional arrays of strings
+    elif var.dtype == object:  # This commonly means we have multidimensional arrays of strings
         try:
             longest_string = 0
-            for x in np.nditer(var.data, flags=['refs_ok']):
+            for x in np.nditer(var.data, flags=["refs_ok"]):
                 if len(str(x)) > longest_string:
                     longest_string = len(str(x))
             return 51, longest_string
         except Exception as e:
             print(
-                f'NOT SUPPORTED: Data in variable {var.name} has data type {var.dtype}.  Attempting to convert it to strings ran into the error: {str(e)}')
+                f"NOT SUPPORTED: Data in variable {var.name} has data type {var.dtype}.  Attempting to convert it to strings ran into the error: {str(e)}"
+            )
             return 51, 1
     elif var.dtype.type == np.datetime64:
         return 33, 1
     else:
-        print(f'NOT SUPPORTED: Data in variable {var.name} has data type of {var.dtype}.')
+        print(f"NOT SUPPORTED: Data in variable {var.name} has data type of {var.dtype}.")
         return 51, 1
 
 
-def _dtype_to_fillval(dtype):
-
+def _dtype_to_fillval(dtype: np.dtype) -> Union[float, int, str, None]:
     if dtype == np.int8 or dtype == np.int16 or dtype == np.int32 or dtype == np.int64:
         return -9223372036854775808  # Default FILLVAL of 'CDF_INT8'
     elif dtype == np.float64 or dtype == np.float32 or dtype == np.float16:
         return -1e30  # Default FILLVAL of 'CDF_DOUBLE'
     elif dtype == np.uint8 or dtype == np.uint16 or dtype == np.uint32 or dtype == np.uint64:
         return 4294967294  # Default FILLVAL of 'CDF_UNIT4'
     elif dtype.type == np.str_:
         return " "  # Default FILLVAL of 'CDF_CHAR'
     else:
-        print(f'Data type of {dtype} not supported')
-
-    return
-
+        print(f"Data type of {dtype} not supported")
+        return None
 
-def _verify_depend_dimensions(dataset, dimension_number, primary_variable_name, coordinate_variable_name):
 
+def _verify_depend_dimensions(
+    dataset: xr.Dataset, dimension_number: int, primary_variable_name: str, coordinate_variable_name: str
+) -> bool:
     primary_data = np.array(dataset[primary_variable_name])
     coordinate_data = np.array(dataset[coordinate_variable_name])
 
     if len(primary_data.shape) != 0 and len(coordinate_data.shape) == 0:
         print(
-            f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match.')
+            f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
+        )
         return False
 
     if len(coordinate_data.shape) != 0 and len(primary_data.shape) == 0:
         print(
-            f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match.')
+            f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
+        )
         return False
 
     if len(coordinate_data.shape) > 2:
         print(
-            f'ISTP Compliance Warning: {coordinate_variable_name} has too many dimensions to be the DEPEND_{dimension_number} for variable {primary_variable_name}')
+            f"ISTP Compliance Warning: {coordinate_variable_name} has too many dimensions to be the DEPEND_{dimension_number} for variable {primary_variable_name}"
+        )
         return False
     if len(coordinate_data.shape) == 2:
-
         if primary_data.shape[0] != coordinate_data.shape[0]:
             print(
-                f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the Epoch dimensions do not match.')
+                f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the Epoch dimensions do not match."
+            )
             return False
 
     if len(primary_data.shape) <= dimension_number:
-        print(f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions')
+        print(
+            f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions"
+        )
         return False
 
     if primary_data.shape[dimension_number] != coordinate_data.shape[-1]:
         print(
-            f'ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match.')
+            f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
+        )
         return False
 
     return True
 
 
-def _dimension_checker(dataset):
-
-    depend_regex = re.compile('depend_[0-9]+$')
+def _dimension_checker(dataset: xr.Dataset) -> List[str]:
+    depend_regex = re.compile("depend_[0-9]+$")
 
     # NOTE: This may add attributes to the dataset object!
 
     # This variable will capture all ISTP compliant variables
     istp_depend_dimension_list = []
 
     # This variable will capture all other non-epoch dimension variables
     depend_dimension_list = []
 
     data = (dataset, dataset.coords)
 
     for d in data:
-
         # Loop through the data
         for var in d:
-
+            var = cast(str, var)
             # Determine the variable type (data, support_data, metadata, ignore_data)
-            if 'VAR_TYPE' not in dataset[var].attrs:
+            if "VAR_TYPE" not in dataset[var].attrs:
                 print(
-                    f'ISTP Compliance Warning: Variable {var} does not have an attribute VAR_TYPE to describe the variable.  Attributes must be either data, support_data, metadata, or ignore_data.')
+                    f"ISTP Compliance Warning: Variable {var} does not have an attribute VAR_TYPE to describe the variable.  Attributes must be either data, support_data, metadata, or ignore_data."
+                )
                 var_type = None
             else:
-                var_type = dataset[var].attrs['VAR_TYPE']
-                if var_type.lower() not in ('data', 'support_data', 'metadata', 'ignore_data'):
+                var_type = dataset[var].attrs["VAR_TYPE"]
+                if var_type.lower() not in ("data", "support_data", "metadata", "ignore_data"):
                     print(
-                        f'ISTP Compliance Warning: Variable {var} attribute VAR_TYPE is not set to either data, support_data, metadata, or ignore_data.')
+                        f"ISTP Compliance Warning: Variable {var} attribute VAR_TYPE is not set to either data, support_data, metadata, or ignore_data."
+                    )
                     var_type = None
 
             # Determine ISTP compliant variables
             for att in dataset[var].attrs:
-                if depend_regex.match(att.lower()) and att != 'DEPEND_0':
+                if depend_regex.match(att.lower()) and att != "DEPEND_0":
                     if (dataset[var].attrs[att] in dataset) or (dataset[var].attrs[att] in dataset.coords):
                         depend_i = dataset[var].attrs[att]
                         if _verify_depend_dimensions(dataset, int(att[-1]), var, depend_i):
                             istp_depend_dimension_list.append(dataset[var].attrs[att])
                     else:
                         print(
-                            f'ISTP Compliance Warning: variable {var} listed {dataset[var].attrs[att]} as its {att}.  However, it was not found in the dataset.')
+                            f"ISTP Compliance Warning: variable {var} listed {dataset[var].attrs[att]} as its {att}.  However, it was not found in the dataset."
+                        )
 
             # Determine potential dimension (non-epoch) variables
             potential_depend_dims = dataset[var].dims[1:]
+            potential_depend_dims = cast(List[str], potential_depend_dims)
             i = 1
-            for d in potential_depend_dims:
-                depend_dimension_list.append(d)
-                if d not in dataset:  # Check if the dimension is in the coordinates themselves
-                    if var_type is not None and var_type.lower() == 'data':
-                        if f'DEPEND_{i}' not in dataset[var].attrs:
+            for dim in potential_depend_dims:
+                depend_dimension_list.append(dim)
+                if dim not in dataset:  # Check if the dimension is in the coordinates themselves
+                    if var_type is not None and var_type.lower() == "data":
+                        if f"DEPEND_{i}" not in dataset[var].attrs:
                             print(
-                                f'ISTP Compliance Warning: variable {var} contains a dimension {d} that is not defined in xarray.  '
-                                f'Specify one of the other xarray DataArrays as the DEPEND_{i} attribute.')
+                                f"ISTP Compliance Warning: variable {var} contains a dimension {d} that is not defined in xarray.  "
+                                f"Specify one of the other xarray DataArrays as the DEPEND_{i} attribute."
+                            )
                 i += 1
 
     depend_dimension_list = list(set(depend_dimension_list))
     istp_depend_dimension_list = list(set(istp_depend_dimension_list))
 
     combined_depend_dimension_list = list(set(depend_dimension_list + istp_depend_dimension_list))
 
     return combined_depend_dimension_list
 
 
-def _recheck_dimensions_after_epoch_checker(dataset, time_varying_dimensions, dim_vars):
+def _recheck_dimensions_after_epoch_checker(
+    dataset: xr.Dataset, time_varying_dimensions: List[str], dim_vars: List[str]
+) -> List[str]:
     # We need to go back and take a look at the first dimensions of data that were not identified as time-varying
     depend_dimension_list = []
     data = (dataset, dataset.coords)
     for d in data:
         for var in d:
             if var not in time_varying_dimensions:
                 if len(dataset[var].dims) >= 1:
                     depend_dimension_list.append(dataset[var].dims[0])
 
-    depend_dimension_list = set(depend_dimension_list + dim_vars)
+    depend_dimension_list = list(set(depend_dimension_list + dim_vars))
+    depend_dimension_list = cast(List[str], depend_dimension_list)
 
     return depend_dimension_list
 
 
-def _epoch_checker(dataset, dim_vars):
-
+def _epoch_checker(dataset: xr.Dataset, dim_vars: List[str]) -> Tuple[List[str], List[str]]:
     # This holds the list of epoch variables
     depend_0_list = []
     time_varying_dimensions = []
 
     data = (dataset, dataset.coords)
 
     for d in data:
-
         # Loop through the non-coordinate data
         for var in d:
+            var = cast(str, var)
             # Continue if there are no dimensions
             if len(dataset[var].dims) == 0:
                 continue
 
-            epoch_regex_1 = re.compile('epoch$')
-            epoch_regex_2 = re.compile('epoch_[0-9]+$')
-            first_dim_name = dataset[var].dims[0]
+            epoch_regex_1 = re.compile("epoch$")
+            epoch_regex_2 = re.compile("epoch_[0-9]+$")
+            first_dim_name = cast(str, dataset[var].dims[0])
 
             # Look at the first dimension of each data
-            if 'DEPEND_0' in dataset[var].attrs:
-                potential_depend_0 = dataset[var].attrs['DEPEND_0']
+            if "DEPEND_0" in dataset[var].attrs:
+                potential_depend_0 = dataset[var].attrs["DEPEND_0"]
             elif epoch_regex_1.match(first_dim_name.lower()) or epoch_regex_2.match(first_dim_name.lower()):
                 potential_depend_0 = first_dim_name
             elif epoch_regex_1.match(var.lower()) or epoch_regex_2.match(var.lower()):
                 potential_depend_0 = var
-            elif 'VAR_TYPE' in dataset[var].attrs and dataset[var].attrs['VAR_TYPE'].lower() == 'data':
+            elif "VAR_TYPE" in dataset[var].attrs and dataset[var].attrs["VAR_TYPE"].lower() == "data":
                 potential_depend_0 = first_dim_name
-            elif 'VAR_TYPE' in dataset[var].attrs and dataset[var].attrs['VAR_TYPE'].lower() == 'support_data' and len(dataset[var].dims) > 1:
+            elif (
+                "VAR_TYPE" in dataset[var].attrs
+                and dataset[var].attrs["VAR_TYPE"].lower() == "support_data"
+                and len(dataset[var].dims) > 1
+            ):
                 potential_depend_0 = first_dim_name
             else:
-                potential_depend_0 = ''
+                potential_depend_0 = ""
 
             # We want to ignore any dimensions that were already gathered in the _dimension_checker function
-            if potential_depend_0 in dim_vars or potential_depend_0 == '':
+            if potential_depend_0 in dim_vars or potential_depend_0 == "":
                 continue
 
             # Ensure that the dimension is listed somewhere else in the dataset
             if potential_depend_0 in dataset or potential_depend_0 in dataset.coords:
                 if _verify_depend_dimensions(dataset, 0, var, potential_depend_0):
                     depend_0_list.append(potential_depend_0)
                     time_varying_dimensions.append(var)
                 else:
                     print(
-                        f'ISTP Compliance Warning: variable {var} contained a "record" dimension {potential_depend_0}, but they have different dimensions.')
+                        f'ISTP Compliance Warning: variable {var} contained a "record" dimension {potential_depend_0}, but they have different dimensions.'
+                    )
             elif epoch_regex_1.match(var.lower()) or epoch_regex_2.match(var.lower()):
                 depend_0_list.append(potential_depend_0)
                 time_varying_dimensions.append(var)
             else:
                 print(
-                    f'ISTP Compliance Warning: variable {var} contained an "record" dimension {potential_depend_0}, but it was not found in the data set.')
+                    f'ISTP Compliance Warning: variable {var} contained an "record" dimension {potential_depend_0}, but it was not found in the data set.'
+                )
 
     depend_0_list = list(set(depend_0_list))
 
     if not depend_0_list:
-        print(f'ISTP Compliance Warning: No variable for the time dimension could be found.')
+        print(f"ISTP Compliance Warning: No variable for the time dimension could be found.")
 
     epoch_found = False
     for d in depend_0_list:
-        if d.lower().startswith('epoch'):
+        if d.lower().startswith("epoch"):
             epoch_found = True
 
     if not epoch_found:
-        print(f'ISTP Compliance Warning: There is no variable named Epoch.  Epoch is the required name of a DEPEND_0 attribute.')
+        print(f"ISTP Compliance Warning: There is no variable named Epoch.  Epoch is the required name of a DEPEND_0 attribute.")
 
     return depend_0_list, time_varying_dimensions
 
 
-def _add_depend_variables_to_dataset(dataset, dim_vars, depend_0_vars, time_varying_dimensions):
-
+def _add_depend_variables_to_dataset(
+    dataset: xr.Dataset, dim_vars: List[str], depend_0_vars: List[str], time_varying_dimensions: List[str]
+) -> xr.Dataset:
     data = (dataset, dataset.coords)
 
     for d in data:
-
         for var in d:
-
             # Check if we should set DEPEND_0
             if var in time_varying_dimensions:
-                if 'DEPEND_0' not in dataset[var].attrs:
+                if "DEPEND_0" not in dataset[var].attrs:
                     depend_0 = dataset[var].dims[0]
                     # if 'VAR_TYPE' in dataset[var].attrs and dataset[var].attrs['VAR_TYPE'].lower() == 'data':
                     #    depend_0 = first_dim_name
                     # elif 'VAR_TYPE' in dataset[var].attrs and dataset[var].attrs['VAR_TYPE'].lower() == 'support_data' and len(
                     #        dataset[var].dims) > 1:
                     #    depend_0 = first_dim_name
                     # else:
                     #    depend_0 = None
 
                     if depend_0 is not None and depend_0 in depend_0_vars and var != depend_0:
-                        dataset[var].attrs['DEPEND_0'] = depend_0
-                        print(f'ISTP Compliance Action: Adding attribute DEPEND_0={depend_0} to {var}')
+                        dataset[var].attrs["DEPEND_0"] = depend_0
+                        print(f"ISTP Compliance Action: Adding attribute DEPEND_0={depend_0} to {var}")
 
                 potential_depend_dims = dataset[var].dims[1:]
 
             else:
-
                 potential_depend_dims = dataset[var].dims
 
             # Check if we should add a DEPEND_{i}
             i = 1
-            for d in potential_depend_dims:
-                if d in dataset and d in dim_vars:
-                    if not f'DEPEND_{i}' in dataset[var].attrs and var != d:
-                        print(f'ISTP Compliance Action: Adding attribute DEPEND_{i}={d} to {var}')
-                        dataset[var].attrs[f'DEPEND_{i}'] = d
+            for dim in potential_depend_dims:
+                if dim in dataset and dim in dim_vars:
+                    if not f"DEPEND_{i}" in dataset[var].attrs and var != dim:
+                        print(f"ISTP Compliance Action: Adding attribute DEPEND_{i}={dim} to {var}")
+                        dataset[var].attrs[f"DEPEND_{i}"] = dim
                 i += 1
 
     return dataset
 
 
-def _global_attribute_checker(dataset):
-    required_global_attributes = ["Project",
-                                  "Source_name",
-                                  "Discipline",
-                                  "Data_type",
-                                  "Descriptor",
-                                  "Data_version",
-                                  "Logical_file_id",
-                                  "PI_name",
-                                  "PI_affiliation",
-                                  "TEXT",
-                                  "Instrument_type",
-                                  "Mission_group",
-                                  "Logical_source",
-                                  "Logical_source_description"]
+def _global_attribute_checker(dataset: xr.Dataset) -> None:
+    required_global_attributes = [
+        "Project",
+        "Source_name",
+        "Discipline",
+        "Data_type",
+        "Descriptor",
+        "Data_version",
+        "Logical_file_id",
+        "PI_name",
+        "PI_affiliation",
+        "TEXT",
+        "Instrument_type",
+        "Mission_group",
+        "Logical_source",
+        "Logical_source_description",
+    ]
     for ga in required_global_attributes:
         if ga not in dataset.attrs:
-            print(f'ISTP Compliance_Warning: Missing dataset attribute {ga}.')
-
+            print(f"ISTP Compliance_Warning: Missing dataset attribute {ga}.")
 
-def _variable_attribute_checker(dataset, epoch_list):
 
+def _variable_attribute_checker(dataset: xr.Dataset, epoch_list: List[str]) -> None:
     data = (dataset, dataset.coords)
 
     for d in data:
-
         for var in d:
-
             # Check for VAR_TYPE
-            if 'VAR_TYPE' not in d[var].attrs:
-                print(f'ISTP Compliance Warning: VAR_TYPE is not defined for variable {var}.')
-                var_type = ''
+            if "VAR_TYPE" not in d[var].attrs:
+                print(f"ISTP Compliance Warning: VAR_TYPE is not defined for variable {var}.")
+                var_type = ""
             else:
-                var_type = d[var].attrs['VAR_TYPE']
-                if var_type.lower() not in ('data', 'support_data', 'metadata', 'ignore_data'):
-                    print(f'ISTP Complaince Warning: VAR_TYPE for variable {var} is given a non-compliant value of {var_type}')
-                    var_type = ''
+                var_type = d[var].attrs["VAR_TYPE"]
+                if var_type.lower() not in ("data", "support_data", "metadata", "ignore_data"):
+                    print(f"ISTP Complaince Warning: VAR_TYPE for variable {var} is given a non-compliant value of {var_type}")
+                    var_type = ""
 
             # Check for CATDESC
-            if 'CATDESC' not in d[var].attrs:
-                print(f'ISTP Compliance Warning: CATDESC attribute is required for variable {var}')
+            if "CATDESC" not in d[var].attrs:
+                print(f"ISTP Compliance Warning: CATDESC attribute is required for variable {var}")
 
-            if 'DISPLAY_TYPE' not in d[var].attrs:
-                if var_type.lower() == 'data':
-                    print(f'ISTP Compliance Warning: DISPLAY_TYPE not set for variable {var}')
-
-            if 'FIELDNAM' not in d[var].attrs:
-                print(f'ISTP Compliance Warning: FIELDNAM attribute is required for variable {var}')
-
-            if 'FORMAT' not in d[var].attrs:
-                if 'FORM_PTR' in d[var].attrs:
-                    if d[var].attrs['FORM_PTR'] in dataset or d[var].attrs['FORM_PTR'] in dataset.coords:
+            if "DISPLAY_TYPE" not in d[var].attrs:
+                if var_type.lower() == "data":
+                    print(f"ISTP Compliance Warning: DISPLAY_TYPE not set for variable {var}")
+
+            if "FIELDNAM" not in d[var].attrs:
+                print(f"ISTP Compliance Warning: FIELDNAM attribute is required for variable {var}")
+
+            if "FORMAT" not in d[var].attrs:
+                if "FORM_PTR" in d[var].attrs:
+                    if d[var].attrs["FORM_PTR"] in dataset or d[var].attrs["FORM_PTR"] in dataset.coords:
                         pass
                     else:
-                        print(f'ISTP Compliance Warning: FORM_PTR for variable {var} does not point to an existing variable.')
+                        print(f"ISTP Compliance Warning: FORM_PTR for variable {var} does not point to an existing variable.")
                 else:
-                    print(f'ISTP Compliance Warning: FORMAT or FORM_PTR attribute is required for variable {var}')
+                    print(f"ISTP Compliance Warning: FORMAT or FORM_PTR attribute is required for variable {var}")
             else:
-                print(f'ISTP Compliance Warning: FORMAT or FORM_PTR attribute is required for variable {var}')
+                print(f"ISTP Compliance Warning: FORMAT or FORM_PTR attribute is required for variable {var}")
 
-            if 'LABLAXIS' not in d[var].attrs:
-                if var_type.lower() == 'data':
-                    if 'LABL_PTR_1' in d[var].attrs:
-                        if d[var].attrs['LABL_PTR_1'] in dataset or d[var].attrs['LABL_PTR_1'] in dataset.coords:
+            if "LABLAXIS" not in d[var].attrs:
+                if var_type.lower() == "data":
+                    if "LABL_PTR_1" in d[var].attrs:
+                        if d[var].attrs["LABL_PTR_1"] in dataset or d[var].attrs["LABL_PTR_1"] in dataset.coords:
                             pass
                         else:
                             print(
-                                f'ISTP Compliance Warning: LABL_PTR_1 attribute for variable {var} does not point to an existing variable.')
+                                f"ISTP Compliance Warning: LABL_PTR_1 attribute for variable {var} does not point to an existing variable."
+                            )
                     else:
-                        print(f'ISTP Compliance Warning: LABLAXIS or LABL_PTR_1 attribute is required for variable {var}')
+                        print(f"ISTP Compliance Warning: LABLAXIS or LABL_PTR_1 attribute is required for variable {var}")
 
-            if 'UNITS' not in d[var].attrs:
-                if var_type.lower() == 'data' or var_type.lower() == 'support_data':
-                    if 'UNIT_PTR' not in d[var].attrs:
-                        print(f'ISTP Compliance Warning: UNITS or UNIT_PTR attribute is required for variable {var}')
+            if "UNITS" not in d[var].attrs:
+                if var_type.lower() == "data" or var_type.lower() == "support_data":
+                    if "UNIT_PTR" not in d[var].attrs:
+                        print(f"ISTP Compliance Warning: UNITS or UNIT_PTR attribute is required for variable {var}")
                     else:
-                        if d[var].attrs['UNIT_PTR'] not in dataset:
+                        if d[var].attrs["UNIT_PTR"] not in dataset:
                             print(
-                                f'ISTP Compliance Warning: UNIT_PTR attribute for variable {var} does not point to an existing variable.')
+                                f"ISTP Compliance Warning: UNIT_PTR attribute for variable {var} does not point to an existing variable."
+                            )
 
-            if 'VALIDMIN' not in d[var].attrs:
-                if var_type.lower() == 'data':
-                    print(f'ISTP Compliance Warning: VALIDMIN required for variable {var}')
-                elif var_type.lower() == 'support_data':
+            if "VALIDMIN" not in d[var].attrs:
+                if var_type.lower() == "data":
+                    print(f"ISTP Compliance Warning: VALIDMIN required for variable {var}")
+                elif var_type.lower() == "support_data":
                     if len(dataset[var].dims) > 0:
                         if dataset[var].dims[0] in epoch_list:
-                            print(f'ISTP Compliance Warning: VALIDMIN required for variable {var}')
+                            print(f"ISTP Compliance Warning: VALIDMIN required for variable {var}")
 
-            if 'VALIDMAX' not in d[var].attrs:
-                if var_type.lower() == 'data':
-                    print(f'ISTP Compliance Warning: VALIDMAX required for variable {var}')
-                elif var_type.lower() == 'support_data':
+            if "VALIDMAX" not in d[var].attrs:
+                if var_type.lower() == "data":
+                    print(f"ISTP Compliance Warning: VALIDMAX required for variable {var}")
+                elif var_type.lower() == "support_data":
                     if len(dataset[var].dims) > 0:
                         if d[var].dims[0] in epoch_list:
-                            print(f'ISTP Compliance Warning: VALIDMAX required for variable {var}')
+                            print(f"ISTP Compliance Warning: VALIDMAX required for variable {var}")
 
-            if 'FILLVAL' not in d[var].attrs:
-                if var_type.lower() == 'data':
-                    print(f'ISTP Compliance Warning: FILLVAL required for variable {var}')
+            if "FILLVAL" not in d[var].attrs:
+                if var_type.lower() == "data":
+                    print(f"ISTP Compliance Warning: FILLVAL required for variable {var}")
                     fillval = _dtype_to_fillval(d[var].dtype)
-                    d[var].attrs['FILLVAL'] = fillval
-                    print(f'ISTP Compliance Action: Automatically set FILLVAL to {fillval} for variable {var}')
-                elif var_type.lower() == 'support_data':
+                    d[var].attrs["FILLVAL"] = fillval
+                    print(f"ISTP Compliance Action: Automatically set FILLVAL to {fillval} for variable {var}")
+                elif var_type.lower() == "support_data":
                     if len(dataset[var].dims) > 0:
                         if d[var].dims[0] in epoch_list:
-                            print(f'ISTP Compliance Warning: FILLVAL required for variable {var}')
+                            print(f"ISTP Compliance Warning: FILLVAL required for variable {var}")
                             fillval = _dtype_to_fillval(d[var].dtype)
-                            d[var].attrs['FILLVAL'] = fillval
-                            print(f'ISTP Compliance Action: Automatically set FILLVAL to {fillval} for variable {var}')
+                            d[var].attrs["FILLVAL"] = fillval
+                            print(f"ISTP Compliance Action: Automatically set FILLVAL to {fillval} for variable {var}")
 
 
-def _label_checker(dataset):
+def _label_checker(dataset: xr.Dataset) -> List[str]:
     # NOTE: This may add attributes to the dataset object!
 
     # This variable will capture all ISTP compliant variables
     istp_label_list = []
 
     # Loop through the data
     for var in dataset:
         # Determine ISTP compliant variables
         for att in dataset[var].attrs:
-            if att.startswith('LABL_PTR'):
+            if att.startswith("LABL_PTR"):
                 if (dataset[var].attrs[att] in dataset) or (dataset[var].attrs[att] in dataset.coords):
                     istp_label_list.append(dataset[var].attrs[att])
                 else:
                     print(
-                        f'ISTP Compliance Warning: variable {var} listed {dataset[var].attrs[att]} as its {att}.  However, it was not found in the dataset.')
+                        f"ISTP Compliance Warning: variable {var} listed {dataset[var].attrs[att]} as its {att}.  However, it was not found in the dataset."
+                    )
 
     istp_label_list = list(set(istp_label_list))
 
     for l in istp_label_list:
-        if 'VAR_TYPE' not in dataset[l].attrs:
-            dataset[l].attrs['VAR_TYPE'] = 'metadata'
+        if "VAR_TYPE" not in dataset[l].attrs:
+            dataset[l].attrs["VAR_TYPE"] = "metadata"
 
     return istp_label_list
 
 
-def _unixtime_to_tt2000(unixtime_data):
-
+def _unixtime_to_tt2000(unixtime_data) -> npt.NDArray:  # type: ignore[no-untyped-def]
     # Make sure the object is iterable.  Sometimes numpy arrays claim to be iterable when they aren't.
-    if not hasattr(unixtime_data, '__len__'):
+    if not hasattr(unixtime_data, "__len__"):
         unixtime_data = [unixtime_data]
     elif isinstance(unixtime_data, np.ndarray):
         if unixtime_data.size <= 1:
             unixtime_data = [unixtime_data]
 
     tt2000_data = np.zeros(len(unixtime_data))
     i = 0
     for ud in unixtime_data:
         if not np.isnan(ud):
             dt = datetime.utcfromtimestamp(ud)
-            dt_to_convert = [dt.year,
-                             dt.month,
-                             dt.day,
-                             dt.hour,
-                             dt.minute,
-                             dt.second,
-                             int(dt.microsecond / 1000),
-                             int(dt.microsecond % 1000),
-                             0]
+            dt_to_convert = [
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+                int(dt.microsecond / 1000),
+                int(dt.microsecond % 1000),
+                0,
+            ]
             converted_data = cdfepoch.compute(dt_to_convert)
         else:
             converted_data = np.nan
 
         tt2000_data[i] = converted_data
         i += 1
 
     return tt2000_data
 
 
-def _datetime_to_tt2000(datetime_data):
+def _datetime_to_tt2000(datetime_data) -> npt.NDArray:  # type: ignore[no-untyped-def]
     tt2000_data = np.array([])
     for dd in datetime_data:
-        dd_to_convert = [dd.year,
-                         dd.month,
-                         dd.day,
-                         dd.hour,
-                         dd.minute,
-                         dd.second,
-                         int(dd.microsecond / 1000),
-                         int(dd.microsecond % 1000),
-                         0]
+        dd_to_convert = [
+            dd.year,
+            dd.month,
+            dd.day,
+            dd.hour,
+            dd.minute,
+            dd.second,
+            int(dd.microsecond / 1000),
+            int(dd.microsecond % 1000),
+            0,
+        ]
         np.append(tt2000_data, cdfepoch.compute(dd_to_convert))
     return tt2000_data
 
 
-def xarray_to_cdf(xarray_dataset, file_name, from_unixtime=False, from_datetime=False,
-                  istp=True, record_dimensions=[], compression=0):
+def xarray_to_cdf(
+    xarray_dataset: xr.Dataset,
+    file_name: str,
+    from_unixtime: bool = False,
+    from_datetime: bool = False,
+    istp: bool = True,
+    record_dimensions: List[str] = [],
+    compression: int = 0,
+) -> None:
     """
     This function converts XArray Dataset objects into CDF files.
 
     Parameters:
         xarray_dataset (xarray.Dataset): The XArray Dataset object that you'd like to convert into a CDF file
         file_name (str):  The path to the place the newly created CDF file
         to_datetime (bool, optional): Whether or not to convert variables named "epoch" or "epoch_X" to CDF_TT2000 from datetime objects
@@ -614,31 +643,32 @@
 
         _variable_attribute_checker(dataset, depend_0_vars)
     else:
         depend_0_vars = record_dimensions
         time_varying_dimensions = record_dimensions
 
     # Gather the global attributes, write them into the file
-    glob_att_dict = {}
+    glob_att_dict: Dict[str, Dict[int, Any]] = {}
     for ga in dataset.attrs:
-        if hasattr(dataset.attrs[ga], '__len__') and not isinstance(dataset.attrs[ga], str):
+        if hasattr(dataset.attrs[ga], "__len__") and not isinstance(dataset.attrs[ga], str):
             i = 0
             glob_att_dict[ga] = {}
             for _ in dataset.attrs[ga]:
                 glob_att_dict[ga][i] = dataset.attrs[ga][i]
                 i += 1
         else:
             glob_att_dict[ga] = {0: dataset.attrs[ga]}
 
     x.write_globalattrs(glob_att_dict)
 
     # Gather the variables, write them into the file
     datasets = (dataset, dataset.coords)
     for d in datasets:
         for var in d:
+            var = cast(str, var)
             var_att_dict = {}
             for att in d[var].attrs:
                 var_att_dict[att] = d[var].attrs[att]
 
             cdf_data_type, cdf_num_elements = _dtype_to_cdf_type(d[var])
             if cdf_data_type is None or cdf_num_elements is None:
                 continue
@@ -650,33 +680,35 @@
                 else:
                     dim_sizes = d[var].shape
                     record_vary = False
             else:
                 dim_sizes = []
                 record_vary = True
 
-            var_spec = {'Variable': var,
-                        'Data_Type': cdf_data_type,
-                        'Num_Elements': cdf_num_elements,
-                        'Rec_Vary': record_vary,
-                        'Dim_Sizes': list(dim_sizes),
-                        'Compress': compression}
+            var_spec = {
+                "Variable": var,
+                "Data_Type": cdf_data_type,
+                "Num_Elements": cdf_num_elements,
+                "Rec_Vary": record_vary,
+                "Dim_Sizes": list(dim_sizes),
+                "Compress": compression,
+            }
 
             var_data = d[var].data
 
             if istp:
-                epoch_regex_1 = re.compile('epoch$')
-                epoch_regex_2 = re.compile('epoch_[0-9]+$')
+                epoch_regex_1 = re.compile("epoch$")
+                epoch_regex_2 = re.compile("epoch_[0-9]+$")
                 if epoch_regex_1.match(var.lower()) or epoch_regex_2.match(var.lower()):
                     if from_unixtime:
                         var_data = _unixtime_to_tt2000(d[var].data)
                     elif from_datetime:
                         var_data = _datetime_to_tt2000(d[var].data)
                 elif cdf_data_type == 33:
-                    unixtime_from_datetime64 = d[var].data.astype('int64') / 1000000000.0
+                    unixtime_from_datetime64 = d[var].data.astype("int64") / 1000000000.0
                     var_data = _unixtime_to_tt2000(unixtime_from_datetime64)
 
             x.write_var(var_spec, var_attrs=var_att_dict, var_data=var_data)
 
     x.close()
 
     return
```

### Comparing `cdflib-0.4.9/cdflib.egg-info/SOURCES.txt` & `cdflib-1.0.0/cdflib.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .coveragerc
 .flake8
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
-CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.md
 asv.conf.json
 meta.yaml
 mypy.ini
 pyproject.toml
@@ -22,32 +21,36 @@
 benchmarks/benchmarks.py
 cdflib/CDFLeapSeconds.txt
 cdflib/__init__.py
 cdflib/_version.py
 cdflib/cdf_to_xarray.py
 cdflib/cdfread.py
 cdflib/cdfwrite.py
+cdflib/dataclasses.py
 cdflib/epochs.py
 cdflib/epochs_astropy.py
+cdflib/s3.py
+cdflib/utils.py
 cdflib/xarray_to_cdf.py
 cdflib.egg-info/PKG-INFO
 cdflib.egg-info/SOURCES.txt
 cdflib.egg-info/dependency_links.txt
 cdflib.egg-info/requires.txt
 cdflib.egg-info/top_level.txt
 doc/Makefile
+doc/changelog.rst
 doc/conf.py
 doc/development.rst
 doc/index.rst
-doc/introduction.rst
 doc/make.bat
-doc/requirements.txt
 doc/modules/cdfepoch.rst
 doc/modules/cdfread.rst
 doc/modules/cdfwrite.rst
+doc/modules/dataclasses.rst
+doc/modules/index.rst
 doc/modules/xarray.rst
 tests/test_astropy_epochs.py
 tests/test_cdfread.py
 tests/test_cdfread_rle.py
 tests/test_cdfwrite.py
 tests/test_epochs.py
 tests/test_xarray_reader_writer.py
```

### Comparing `cdflib-0.4.9/doc/Makefile` & `cdflib-1.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/doc/conf.py` & `cdflib-1.0.0/doc/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,83 +7,88 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-import os
-import sys
-
-sys.path.insert(0, os.path.abspath("."))
-sys.path.insert(0, os.path.abspath("../"))
-sys.path.insert(0, os.path.abspath('../..'))
+import cdflib
 
 # -- Project information -----------------------------------------------------
 
-project = 'cdflib'
-author = 'Bryan Harter, Michael Liu'
+project = "cdflib"
+author = "Bryan Harter, Michael Liu"
+version = str(cdflib.__version__)
 
 # The short X.Y version
-version = ''
+# version = ''
 # The full version, including alpha/beta/rc tags
-release = ''
+release = ""
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ['sphinx.ext.autodoc',
-              'sphinx.ext.viewcode',
-              'sphinx.ext.napoleon',
-              'sphinx_automodapi.automodapi']
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autosummary",
+    "sphinx_copybutton",
+    "sphinx.ext.linkcode",
+    "sphinx.ext.intersphinx",
+    "sphinx_automodapi.automodapi",
+]
 
 numpydoc_class_members_toctree = False
 numpydoc_show_class_members = False
+autodoc_typehints = "description"
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
+templates_path = ["_templates"]
+default_role = "any"
+nitpicky = True
+nitpick_ignore = [("py:class", "array-like"), ("py:class", "optional")]
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
@@ -102,50 +107,57 @@
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'cdflibdoc'
+htmlhelp_basename = "cdflibdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'cdflib.tex', 'cdflib Documentation',
-     'Bryan Harter, Michael Liu', 'manual'),
+    (master_doc, "cdflib.tex", "cdflib Documentation", "Bryan Harter, Michael Liu", "manual"),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'cdflib', 'cdflib Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "cdflib", "cdflib Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'cdflib', 'cdflib Documentation',
-     author, 'cdflib', 'One line description of project.',
-     'Miscellaneous'),
+    (master_doc, "cdflib", "cdflib Documentation", author, "cdflib", "One line description of project.", "Miscellaneous"),
 ]
 
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/3': None}
-#autodoc_mock_imports = ['xarray', 'astropy']
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/3", None),
+    "numpy": ("https://numpy.org/doc/stable", None),
+    "astropy": ("https://docs.astropy.org/en/stable/", None),
+    "xarray": ("https://docs.xarray.dev/en/stable/", None),
+}
+
+
+def linkcode_resolve(domain, info):
+    if domain != "py":
+        return None
+    if not info["module"]:
+        return None
+    filename = info["module"].replace(".", "/")
+    return "https://github.com/MAVENSDC/cdflib/tree/master/%s.py" % filename
```

### Comparing `cdflib-0.4.9/doc/make.bat` & `cdflib-1.0.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/doc/modules/cdfepoch.rst` & `cdflib-1.0.0/doc/modules/cdfepoch.rst`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/doc/modules/cdfwrite.rst` & `cdflib-1.0.0/doc/modules/cdfwrite.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CDF Writer Class
 =================
 
-.. automodapi:: cdflib.cdfwrite
-    :no-inheritance-diagram:
+.. autoclass:: cdflib.cdfwrite.CDF
+   :members:
 
 
 Sample Usage
 ------------
 
 >>> import cdfwrite
 >>> import cdfread
```

### Comparing `cdflib-0.4.9/meta.yaml` & `cdflib-1.0.0/meta.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/setup.cfg` & `cdflib-1.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 	hypothesis
 	pytest >= 3.9
 	pytest-cov
 	pytest-remotedata
 	xarray
 docs = 
 	astropy
-	numpydoc
-	sphinx
-	sphinx_rtd_theme
 	xarray
+	sphinx
 	sphinx-automodapi
+	sphinx-copybutton
+	sphinx_rtd_theme
 
 [tool:pytest]
 minversion = 3.9
 addopts = -ra --cov=cdflib --cov-report=xml
 filterwarnings = 
 	ignore:ERFA function
 	ignore:numpy.ndarray size changed
```

### Comparing `cdflib-0.4.9/tests/test_astropy_epochs.py` & `cdflib-1.0.0/tests/test_astropy_epochs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 #!/usr/bin/env python
 from datetime import datetime
 from random import randint
 
 import numpy as np
-import pytest
 from pytest import approx
 
 from cdflib.epochs_astropy import CDFAstropy as cdfepoch
 
 
 def test_encode_cdfepoch():
     x = cdfepoch.encode([62285326000000.0, 62985326000000.0])
-    assert x[0] == '1973-09-28 23:26:40.000000000'
-    assert x[1] == '1995-12-04 19:53:20.000000000'
+    assert x[0] == "1973-09-28 23:26:40.000000000"
+    assert x[1] == "1995-12-04 19:53:20.000000000"
 
 
 def test_encode_cdfepoch16():
-    '''
+    """
     cdf_encode_epoch16(dcomplex(63300946758.000000, 176214648000.00000)) in IDL
     returns 04-Dec-2005 20:39:28.176.214.654.976
 
     However, I believe this IDL routine is bugged.  This website:
     https://www.epochconverter.com/seconds-days-since-y0
 
     shows a correct answer.
-    '''
-    x = cdfepoch.encode(np.complex128(63300946758.000000 + 176214648000.00000j))
-    assert x == '2005-12-04 20:19:18.176214648'
-    y = cdfepoch.encode(np.complex128([33300946758.000000 + 106014648000.00000j,
-                                       61234543210.000000 + 000011148000.00000j]))
-    assert y[0] == '1055-04-07 14:59:18.106014648'
-    assert y[1] == '1940-06-12 03:20:10.000011148'
+    """
+    x = cdfepoch.encode(np.array(63300946758.000000 + 176214648000.00000j))
+    assert x == "2005-12-04 20:19:18.176214648"
+    y = cdfepoch.encode(np.array([33300946758.000000 + 106014648000.00000j, 61234543210.000000 + 000011148000.00000j]))
+    assert y[0] == "1055-04-07 14:59:18.106014648"
+    assert y[1] == "1940-06-12 03:20:10.000011148"
 
 
 def test_encode_cdftt2000():
     x = cdfepoch.encode(186999622360321123)
-    assert x == '2005-12-04 20:20:22.360321120'
+    assert x == "2005-12-04 20:20:22.360321120"
     y = cdfepoch.encode([500000000100, 123456789101112131])
-    assert y[0] == '2000-01-01 12:08:20.000000100'
-    assert y[1] == '2003-11-30 09:33:09.101112128'
+    assert y[0] == "2000-01-01 12:08:20.000000100"
+    assert y[1] == "2003-11-30 09:33:09.101112128"
 
 
 def test_unixtime():
     x = cdfepoch.unixtime([500000000100, 123456789101112131])
     assert approx(x[0]) == 946728435.816
     assert x[1] == approx(1070184724.917112)
 
@@ -65,57 +63,57 @@
     assert x[1][4] == 53
     assert x[1][5] == 20
     assert x[1][6] == 0
 
 
 def test_breakdown_cdfepoch16():
     x = cdfepoch.breakdown(np.complex128(63300946758.000000 + 176214648000.00000j))
-    assert x[0][0] == 2005
-    assert x[0][1] == 12
-    assert x[0][2] == 4
-    assert x[0][3] == 20
-    assert x[0][4] == 19
-    assert x[0][5] == 18
-    assert x[0][6] == 176
-    assert x[0][7] == 214
-    assert x[0][8] == 648
-    assert x[0][9] == 0
+    assert x[0] == 2005
+    assert x[1] == 12
+    assert x[2] == 4
+    assert x[3] == 20
+    assert x[4] == 19
+    assert x[5] == 18
+    assert x[6] == 176
+    assert x[7] == 214
+    assert x[8] == 648
+    assert x[9] == 0
 
 
 def test_breakdown_cdftt2000():
     x = cdfepoch.breakdown(123456789101112131)
-    assert x[0][0] == 2003
-    assert x[0][1] == 11
-    assert x[0][2] == 30
-    assert x[0][3] == 9
-    assert x[0][4] == 33
-    assert x[0][5] == 9
-    assert x[0][6] == 101
-    assert x[0][7] == 112
+    assert x[0] == 2003
+    assert x[1] == 11
+    assert x[2] == 30
+    assert x[3] == 9
+    assert x[4] == 33
+    assert x[5] == 9
+    assert x[6] == 101
+    assert x[7] == 112
 
     # Apparently there is a loss of precision at this level
-    # assert x[0][8] == 131
+    # assert x[8] == 131
 
 
 def test_compute_cdfepoch():
-    '''
+    """
     Using random numbers for the compute tests
-    '''
+    """
     random_time = []
     random_time.append(randint(1709, 2292))  # Year
     random_time.append(randint(1, 12))  # Month
     random_time.append(randint(1, 28))  # Date
     random_time.append(randint(0, 23))  # Hour
     random_time.append(randint(0, 59))  # Minute
     random_time.append(randint(0, 59))  # Second
     random_time.append(randint(0, 999))  # Millisecond
     x = cdfepoch.breakdown(cdfepoch.compute(random_time))
     i = 0
-    for t in x[0]:
-        assert t == random_time[i], f'Time {random_time} was not equal to {x}'
+    for t in x:
+        assert t == random_time[i], f"Time {random_time} was not equal to {x}"
         i += 1
 
 
 def test_compute_cdfepoch16():
     random_time = []
     random_time.append(randint(1709, 2292))  # Year
     random_time.append(randint(1, 12))  # Month
@@ -123,31 +121,31 @@
     random_time.append(randint(0, 23))  # Hour
     random_time.append(randint(0, 59))  # Minute
     random_time.append(randint(0, 59))  # Second
     random_time.append(randint(0, 999))  # Millisecond
     random_time.append(randint(0, 999))  # Microsecond
     random_time.append(randint(0, 999))  # Nanosecond
     random_time.append(randint(0, 999))  # Picosecond
-    cdftime = cdfepoch.convert_to_astropy(cdfepoch.compute(random_time), format='cdf_epoch16')
+    cdftime = cdfepoch.convert_to_astropy(cdfepoch.compute(random_time), format="cdf_epoch16")
     x = cdfepoch.breakdown(cdftime)
     i = 0
-    for t in x[0]:
-        assert t == random_time[i], f'Time {random_time} was not equal to {x}'
+    for t in x:
+        assert t == random_time[i], f"Time {random_time} was not equal to {x}"
         i += 1
         # Unfortunately, currently there is a pretty big loss of precision that comes with
         # the compute function.  Need to stop testing early.
         if i > 6:
             return
 
 
 def test_compute_cdftt2000():
     pass
 
     # Need to determine why computing and breaking down tt2000 types continually adds leap seconds + 32.184
-    '''
+    """
     random_time = []
     random_time.append(randint(0, 2018))  # Year
     random_time.append(randint(1, 12))  # Month
     random_time.append(randint(1, 28))  # Date
     random_time.append(randint(0, 23))  # Hour
     random_time.append(randint(0, 59))  # Minute
     random_time.append(randint(0, 59))  # Second
@@ -155,56 +153,56 @@
     random_time.append(randint(0, 999))  # Microsecond
     random_time.append(randint(0, 999))  # Nanosecond
     x = cdfepoch.breakdown(cdfepoch.compute(random_time))
     i = 0
     for t in x[0]:
         assert t == random_time[i], 'Time {} was not equal to {}'.format(random_time, x)
         i += 1
-    '''
+    """
 
 
 def test_parse_cdfepoch():
     x = cdfepoch.encode(62567898765432.0)
     assert x == "1982-09-12 11:52:45.432000000"
     stripped_time = x[:23]
     parsed = cdfepoch.parse(stripped_time)
-    assert parsed[0] == approx(62567898765432.0)
+    assert parsed == approx(62567898765432.0)
 
 
 def test_parse_cdfepoch16():
     input_time = 53467976543.0 + 543218654100j
-    x = cdfepoch.encode(input_time)
+    x = str(cdfepoch.encode(input_time))
     assert x == "1694-05-01 07:42:23.543218654"
     add_precision = x + "000"
     parsed = cdfepoch.parse(add_precision)
-    assert parsed[0] == approx(53467976543 + .543218654)
+    assert parsed == approx(53467976543 + 0.543218654)
 
     assert cdfepoch.to_datetime(input_time) == datetime(1694, 5, 1, 7, 42, 23, 543219)
 
 
 def test_parse_cdftt2000():
     x = "2004-03-01 12:24:22.351793238"
     parsed = cdfepoch.parse(x)
-    assert parsed == [131415926535793232]
+    assert parsed == 131415926535793232
 
-    assert cdfepoch.to_datetime(parsed) == [datetime(2004, 3, 1, 12, 25, 26, 535793)]
+    assert cdfepoch.to_datetime(parsed) == datetime(2004, 3, 1, 12, 25, 26, 535793)
 
 
 def test_findepochrange_cdfepoch():
     start_time = "2013-12-01 12:24:22.000"
     end_time = "2014-12-01 12:24:22.000"
     x = cdfepoch.parse([start_time, end_time])
     time_array = np.arange(x[0], x[1], step=1000000)
 
     test_start = [2014, 8, 1, 8, 1, 54, 123]
     test_end = [2018, 1, 1, 1, 1, 1, 1]
     index = cdfepoch.findepochrange(time_array, starttime=test_start, endtime=test_end)
     # Test that the test_start is less than the first index, but more than one less
     assert time_array[index[0]] >= cdfepoch.compute(test_start)
-    assert time_array[index[0]-1] <= cdfepoch.compute(test_start)
+    assert time_array[index[0] - 1] <= cdfepoch.compute(test_start)
 
     assert time_array[index[-1]] <= cdfepoch.compute(test_end)
 
 
 def test_findepochrange_cdftt2000():
     start_time = "2004-03-01 12:24:22.351793238"
     end_time = "2004-03-01 12:28:22.351793238"
@@ -212,15 +210,11 @@
     time_array = np.arange(x[0], x[1], step=1000000)
 
     test_start = [2004, 3, 1, 12, 25, 54, 123, 111, 98]
     test_end = [2004, 3, 1, 12, 26, 4, 123, 456, 789]
     index = cdfepoch.findepochrange(time_array, starttime=test_start, endtime=test_end)
     # Test that the test_start is less than the first index, but more than one less
     assert time_array[index[0]] >= cdfepoch.compute(test_start)
-    assert time_array[index[0]-1] <= cdfepoch.compute(test_start)
+    assert time_array[index[0] - 1] <= cdfepoch.compute(test_start)
 
     assert time_array[index[-1]] <= cdfepoch.compute(test_end)
-    assert time_array[index[-1]+1] >= cdfepoch.compute(test_end)
-
-
-if __name__ == '__main__':
-    pytest.main([__file__])
+    assert time_array[index[-1] + 1] >= cdfepoch.compute(test_end)
```

### Comparing `cdflib-0.4.9/tests/test_cdfwrite.py` & `cdflib-1.0.0/tests/test_cdfwrite.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,337 +1,329 @@
-#!/usr/bin/env python
 from pathlib import Path
+from typing import Any, Dict
 
 import numpy as np
-import pytest
 
 from cdflib import cdfread, cdfwrite
 
 R = Path(__file__).parent
-fnbasic = 'testing.cdf'
+fnbasic = "testing.cdf"
 
 
-def cdf_create(fn: Path, spec: dict):
+def cdf_create(fn: Path, spec: Dict[str, Any]) -> cdfwrite.CDF:
     return cdfwrite.CDF(fn, cdf_spec=spec)
 
 
-def cdf_read(fn: Path, validate: bool = False):
+def cdf_read(fn: Path, validate: bool = False) -> cdfread.CDF:
     return cdfread.CDF(fn, validate=validate)
 
 
 def test_cdf_creation(tmp_path):
-
     fn = tmp_path / fnbasic
-    cdf_create(fn, {'rDim_sizes': [1]}).close()
+    cdf_create(fn, {"rDim_sizes": [1]}).close()
 
     reader = cdf_read(fn)
 
     # Test CDF info
     info = reader.cdf_info()
-    assert info['Majority'] == 'Row_major'
+    assert info.Majority == "Row_major"
 
 
 def test_checksum(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
-    tfile = cdf_create(fn, {'Checksum': True})
+    tfile = cdf_create(fn, {"Checksum": True})
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 4
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    varatts = {}
-    varatts['Attribute1'] = 1
-    varatts['Attribute2'] = '500'
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 4
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    varatts: Dict[str, Any] = {}
+    varatts["Attribute1"] = 1
+    varatts["Attribute2"] = "500"
 
-    tfile.write_var(var_spec, var_attrs=varatts,
-                    var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
+    tfile.write_var(var_spec, var_attrs=varatts, var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
 
     tfile.close()
 
-# %% Open the file to read
+    # %% Open the file to read
     reader = cdf_read(fn, validate=True)
     # Test CDF info
     var = reader.varget("Variable1")
-    assert (var == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]).all()
+    np.testing.assert_equal(var, [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
     # test convenience info
-    assert (reader["Variable1"] == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]).all()
+    np.testing.assert_equal(reader["Variable1"], [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 
 
 def test_checksum_compressed(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 2
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    varatts = {}
-    varatts['Attribute1'] = 1
-    varatts['Attribute2'] = '500'
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 2
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    varatts: Dict[str, Any] = {}
+    varatts["Attribute1"] = 1
+    varatts["Attribute2"] = "500"
 
     v = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 
-    tfile = cdf_create(fn, {'Compressed': 6, 'Checksum': True})
-    tfile.write_var(var_spec, var_attrs=varatts,
-                    var_data=v)
+    tfile = cdf_create(fn, {"Compressed": 6, "Checksum": True})
+    tfile.write_var(var_spec, var_attrs=varatts, var_data=v)
 
     tfile.close()
-# %% Open the file to read
+    # Open the file to read
     reader = cdf_read(fn, validate=True)
 
     var = reader.varget("Variable1")
-    assert (var == v).all()
+    np.testing.assert_equal(var, v)
 
     att = reader.attget("Attribute1", entry=0)
-    assert att['Data'] == [1]
+    assert att.Data == [1]
 
     att = reader.attget("Attribute2", entry=0)
-    assert att['Data'] == '500'
+    assert att.Data == "500"
 
 
 def test_file_compression(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 2
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    varatts = {}
-    varatts['Attribute1'] = 1
-    varatts['Attribute2'] = '500'
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 2
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    varatts: Dict[str, Any] = {}
+    varatts["Attribute1"] = 1
+    varatts["Attribute2"] = "500"
 
     v = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 
-    tfile = cdf_create(fn, {'Compressed': 6, 'Checksum': True})
-    tfile.write_var(var_spec, var_attrs=varatts,
-                    var_data=v)
+    tfile = cdf_create(fn, {"Compressed": 6, "Checksum": True})
+    tfile.write_var(var_spec, var_attrs=varatts, var_data=v)
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
     # Test CDF info
     var = reader.varget("Variable1")
-    assert (var == v).all()
+    np.testing.assert_equal(var, v)
 
 
 def test_globalattrs(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    globalAttrs = {}
-    globalAttrs['Global1'] = {0: 'Global Value 1'}
-    globalAttrs['Global2'] = {0: 'Global Value 2'}
-    globalAttrs['Global3'] = {0: [12, 'cdf_int4']}
-    globalAttrs['Global4'] = {0: [12.34, 'cdf_double']}
-    globalAttrs['Global5'] = {0: [12.34, 21.43]}
-
-    GA6 = {}
-    GA6[0] = 'abcd'
-    GA6[1] = [12, 'cdf_int2']
-    GA6[2] = [12.5, 'cdf_float']
-    GA6[3] = [[0, 1, 2], 'cdf_int8']
+    globalAttrs: Dict[str, Any] = {}
+    globalAttrs["Global1"] = {0: "Global Value 1"}
+    globalAttrs["Global2"] = {0: "Global Value 2"}
+    globalAttrs["Global3"] = {0: [12, "cdf_int4"]}
+    globalAttrs["Global4"] = {0: [12.34, "cdf_double"]}
+    globalAttrs["Global5"] = {0: [12.34, 21.43]}
+
+    GA6: Dict[int, Any] = {}
+    GA6[0] = "abcd"
+    GA6[1] = [12, "cdf_int2"]
+    GA6[2] = [12.5, "cdf_float"]
+    GA6[3] = [[0, 1, 2], "cdf_int8"]
 
-    globalAttrs['Global6'] = GA6
+    globalAttrs["Global6"] = GA6
 
-    tfile = cdf_create(fn, {'Checksum': True})
+    tfile = cdf_create(fn, {"Checksum": True})
     tfile.write_globalattrs(globalAttrs)
 
     tfile.close()
-# %% Open the file to read
+    # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
-    attrib = reader.attinq('Global2')
-    assert attrib['num_gr_entry'] == 1
+    attrib = reader.attinq("Global2")
+    assert attrib.num_gr_entry == 1
 
-    attrib = reader.attinq('Global6')
-    assert attrib['num_gr_entry'] == 4
+    attrib = reader.attinq("Global6")
+    assert attrib.num_gr_entry == 4
 
-    entry = reader.attget('Global6', 3)
-    assert entry['Data_Type'] == 'CDF_INT8'
+    entry = reader.attget("Global6", 3)
+    assert entry.Data_Type == "CDF_INT8"
 
-    for x in [0, 1, 2]:
-        assert entry['Data'][x] == x
+    np.testing.assert_equal(entry.Data, [0, 1, 2])
 
 
 def test_create_zvariable(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
-    vs = {}
-    vs['Variable'] = 'Variable1'
-    vs['Data_Type'] = 1
-    vs['Num_Elements'] = 1
-    vs['Rec_Vary'] = True
-    vs['Dim_Sizes'] = []
-    vs['Dim_Vary'] = True
+    vs: Dict[str, Any] = {}
+    vs["Variable"] = "Variable1"
+    vs["Data_Type"] = 1
+    vs["Num_Elements"] = 1
+    vs["Rec_Vary"] = True
+    vs["Dim_Sizes"] = []
+    vs["Dim_Vary"] = True
 
-    tfile = cdf_create(fn, {'Checksum': True})
+    tfile = cdf_create(fn, {"Checksum": True})
     tfile.write_var(vs, var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
     tfile.close()
 
-# %% Open the file to read
+    # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinfo = reader.varinq("Variable1")
-    assert varinfo['Data_Type'] == 1
+    assert varinfo.Data_Type == 1
 
     var = reader.varget("Variable1")
-    assert (var == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]).all()
+    np.testing.assert_equal(var, [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 
 
 def test_create_rvariable(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
-    vs = {}
-    vs['Variable'] = 'Variable1'
-    vs['Var_Type'] = 'rvariable'
-    vs['Data_Type'] = 12
-    vs['Num_Elements'] = 1
-    vs['Rec_Vary'] = True
-    vs['Dim_Sizes'] = []
-    vs['Dim_Vary'] = [True]
+    vs: Dict[str, Any] = {}
+    vs["Variable"] = "Variable1"
+    vs["Var_Type"] = "rvariable"
+    vs["Data_Type"] = 12
+    vs["Num_Elements"] = 1
+    vs["Rec_Vary"] = True
+    vs["Dim_Sizes"] = []
+    vs["Dim_Vary"] = [True]
 
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
     tfile.write_var(vs, var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinfo = reader.varinq("Variable1")
-    assert varinfo['Data_Type'] == 12
+    assert varinfo.Data_Type == 12
 
     var = reader.varget("Variable1")
     for x in [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]:
         assert var[x] == x
 
 
 def test_create_zvariable_no_recvory(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 8
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = False
-    var_spec['Dim_Sizes'] = []
-    var_spec['Dim_Vary'] = True
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 8
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = False
+    var_spec["Dim_Sizes"] = []
+    var_spec["Dim_Vary"] = True
 
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
     tfile.write_var(var_spec, var_data=np.array([2]))
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinfo = reader.varinq("Variable1")
-    assert varinfo['Data_Type'] == 8
+    assert varinfo.Data_Type == 8
 
     var = reader.varget("Variable1")
     assert var == 2
 
 
 def test_create_zvariables_with_attributes(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 8
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    varatts = {}
-    varatts['Attribute1'] = 1
-    varatts['Attribute2'] = '500'
-
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
-    tfile.write_var(var_spec, var_attrs=varatts,
-                    var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
-
-    var_spec['Variable'] = 'Variable2'
-    varatts2 = {}
-    varatts2['Attribute1'] = 2
-    varatts2['Attribute2'] = '1000'
-    tfile.write_var(var_spec, var_attrs=varatts2,
-                    var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 8
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    varatts: Dict[str, Any] = {}
+    varatts["Attribute1"] = 1
+    varatts["Attribute2"] = "500"
+
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
+    tfile.write_var(var_spec, var_attrs=varatts, var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
+
+    var_spec["Variable"] = "Variable2"
+    varatts2: Dict[str, Any] = {}
+    varatts2["Attribute1"] = 2
+    varatts2["Attribute2"] = "1000"
+    tfile.write_var(var_spec, var_attrs=varatts2, var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
 
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     att = reader.attget("Attribute1", entry=0)
-    assert att['Data'] == [1]
+    assert att.Data == [1]
 
     att = reader.attget("Attribute2", entry=1)
-    assert att['Data'] == '1000'
+    assert att.Data == "1000"
 
 
 def test_create_zvariables_then_attributes(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 8
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 8
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
 
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
     tfile.write_var(var_spec, var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
 
-    var_spec['Variable'] = 'Variable2'
+    var_spec["Variable"] = "Variable2"
     tfile.write_var(var_spec, var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
 
-    varatts = {}
-    varatts['Attribute1'] = {'Variable1': 1, 'Variable2': 2}
-    varatts['Attribute2'] = {0: '500', 1: '1000'}
+    varatts: Dict[str, Any] = {}
+    varatts["Attribute1"] = {"Variable1": 1, "Variable2": 2}
+    varatts["Attribute2"] = {0: "500", 1: "1000"}
 
     tfile.write_variableattrs(varatts)
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     att = reader.attget("Attribute1", entry=0)
-    assert att['Data'] == [1]
+    assert att.Data == [1]
 
     att = reader.attget("Attribute2", entry=1)
-    att['Data'] == '1000'
+    att.Data == "1000"
 
 
 def test_nonsparse_zvariable_blocking(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 8
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    var_spec['Block_Factor'] = 10000
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 8
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    var_spec["Block_Factor"] = 10000
     data = np.linspace(0, 999999, num=1000000)
 
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
     tfile.write_var(var_spec, var_data=data)
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
@@ -339,266 +331,243 @@
     assert var[99999] == 99999
 
 
 def test_sparse_virtual_zvariable_blocking(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 8
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    var_spec['Block_Factor'] = 10000
-    var_spec['Sparse'] = 'pad_sparse'
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 8
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    var_spec["Block_Factor"] = 10000
+    var_spec["Sparse"] = "pad_sparse"
     data = np.linspace(0, 140000, num=140001)
     physical_records1 = np.linspace(1, 10000, num=10000)
     physical_records2 = np.linspace(20001, 30000, num=10000)
     physical_records3 = np.linspace(50001, 60000, num=10000)
     physical_records4 = np.linspace(70001, 140000, num=70000)
-    physical_records = np.concatenate((physical_records1,
-                                       physical_records2,
-                                       physical_records3,
-                                       physical_records4)).astype(int)
+    physical_records = np.concatenate((physical_records1, physical_records2, physical_records3, physical_records4)).astype(int)
     sparse_data = [physical_records, data]
 
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
     tfile.write_var(var_spec, var_data=sparse_data)
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinq = reader.varinq("Variable1")
     var = reader.varget("Variable1")
 
-    pad_num = varinq['Pad'][0]
+    pad_num = varinq.Pad[0]
     assert var[30001] == pad_num
     assert var[70001] == 70001
 
 
 def test_sparse_zvariable_blocking(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 8
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    var_spec['Block_Factor'] = 10000
-    var_spec['Sparse'] = 'pad_sparse'
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 8
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    var_spec["Block_Factor"] = 10000
+    var_spec["Sparse"] = "pad_sparse"
     data = np.linspace(0, 99999, num=100000)
     physical_records1 = np.linspace(1, 10000, num=10000)
     physical_records2 = np.linspace(20001, 30000, num=10000)
     physical_records3 = np.linspace(50001, 60000, num=10000)
     physical_records4 = np.linspace(70001, 140000, num=70000)
-    physical_records = np.concatenate((physical_records1,
-                                       physical_records2,
-                                       physical_records3,
-                                       physical_records4)).astype(int)
+    physical_records = np.concatenate((physical_records1, physical_records2, physical_records3, physical_records4)).astype(int)
     sparse_data = [physical_records, data]
 
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
     tfile.write_var(var_spec, var_data=sparse_data)
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     # tfile = cdf_create(fn, {'rDim_sizes': [1]})
     varinq = reader.varinq("Variable1")
     var = reader.varget("Variable1")
-    pad_num = varinq['Pad'][0]
+    pad_num = varinq.Pad[0]
 
     assert var[30001] == pad_num
     assert var[70001] == 30000
 
 
 def test_sparse_zvariable_pad(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 8
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    var_spec['Sparse'] = 'pad_sparse'
-    data = [[200, 3000, 3100, 3500, 4000, 5000, 6000, 10000, 10001, 10002, 20000],
-            np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])]
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 8
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    var_spec["Sparse"] = "pad_sparse"
+    data = [[200, 3000, 3100, 3500, 4000, 5000, 6000, 10000, 10001, 10002, 20000], np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])]
 
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
     tfile.write_var(var_spec, var_data=data)
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinq = reader.varinq("Variable1")
     var = reader.varget("Variable1")
-    pad_num = varinq['Pad'][0]
+    pad_num = varinq.Pad[0]
 
     assert var[100] == pad_num
     assert var[3000] == 1
 
 
 def test_sparse_zvariable_previous(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Data_Type'] = 8
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    var_spec['Sparse'] = 'prev_sparse'
-    data = [[200, 3000, 3100, 3500, 4000, 5000, 6000, 10000, 10001, 10002, 20000],
-            np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])]
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Data_Type"] = 8
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    var_spec["Sparse"] = "prev_sparse"
+    data = [[200, 3000, 3100, 3500, 4000, 5000, 6000, 10000, 10001, 10002, 20000], np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])]
 
-    tfile = cdf_create(fn, {'rDim_sizes': [1]})
+    tfile = cdf_create(fn, {"rDim_sizes": [1]})
     tfile.write_var(var_spec, var_data=data)
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinq = reader.varinq("Variable1")
     var = reader.varget("Variable1")
-    pad_num = varinq['Pad'][0]
+    pad_num = varinq.Pad[0]
 
     assert var[100] == pad_num
     assert var[6001] == var[6000]
 
 
 def test_create_2d_rvariable(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Var_Type'] = 'rvariable'
-    var_spec['Data_Type'] = 14
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    var_spec['Dim_Vary'] = [True, True]
-
-    tfile = cdf_create(fn, {'rDim_sizes': [2, 2]})
-    tfile.write_var(var_spec, var_data=np.array([[[0, 1], [1, 2]],
-                                                 [[2, 3], [3, 4]],
-                                                 [[4, 5], [5, 6]],
-                                                 [[6, 7], [7, 8]],
-                                                 [[8, 9], [9, 10]]]))
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Var_Type"] = "rvariable"
+    var_spec["Data_Type"] = 14
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    var_spec["Dim_Vary"] = [True, True]
+
+    tfile = cdf_create(fn, {"rDim_sizes": [2, 2]})
+    tfile.write_var(
+        var_spec, var_data=np.array([[[0, 1], [1, 2]], [[2, 3], [3, 4]], [[4, 5], [5, 6]], [[6, 7], [7, 8]], [[8, 9], [9, 10]]])
+    )
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinfo = reader.varinq("Variable1")
-    assert varinfo['Data_Type'] == 14
+    assert varinfo.Data_Type == 14
 
     var = reader.varget("Variable1")
     for x in [0, 1, 2, 3, 4]:
-        assert var[x][0][0] == 2*x
-        assert var[x][0][1] == 2*x+1
-        assert var[x][1][0] == 2*x+1
-        assert var[x][1][1] == 2*x+2
+        assert var[x][0][0] == 2 * x
+        assert var[x][0][1] == 2 * x + 1
+        assert var[x][1][0] == 2 * x + 1
+        assert var[x][1][1] == 2 * x + 2
 
 
 def test_create_2d_rvariable_dimvary(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Var_Type'] = 'rvariable'
-    var_spec['Data_Type'] = 21
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    var_spec['Dim_Vary'] = [True, False]
-
-    tfile = cdf_create(fn,  {'rDim_sizes': [2, 20]})
-
-    tfile.write_var(var_spec, var_data=np.array([[0, 1],
-                                                 [2, 3],
-                                                 [4, 5],
-                                                 [6, 7],
-                                                 [8, 9]]))
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Var_Type"] = "rvariable"
+    var_spec["Data_Type"] = 21
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    var_spec["Dim_Vary"] = [True, False]
+
+    tfile = cdf_create(fn, {"rDim_sizes": [2, 20]})
+
+    tfile.write_var(var_spec, var_data=np.array([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]))
 
     tfile.close()
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinfo = reader.varinq("Variable1")
 
-    assert varinfo['Data_Type'] == 21
+    assert varinfo.Data_Type == 21
     var = reader.varget("Variable1")
     for x in [0, 1, 2, 3, 4]:
-        assert var[x][0] == 2*x
-        assert var[x][1] == 2*x+1
+        assert var[x][0] == 2 * x
+        assert var[x][1] == 2 * x + 1
 
 
 def test_create_2d_r_and_z_variables(tmp_path):
     # Setup the test_file
     fn = tmp_path / fnbasic
 
-    var_spec = {}
-    var_spec['Variable'] = 'Variable1'
-    var_spec['Var_Type'] = 'rvariable'
-    var_spec['Data_Type'] = 22
-    var_spec['Num_Elements'] = 1
-    var_spec['Rec_Vary'] = True
-    var_spec['Dim_Sizes'] = []
-    var_spec['Dim_Vary'] = [True, False]
-
-    tfile = cdf_create(fn,  {'rDim_sizes': [2, 20]})
-    tfile.write_var(var_spec, var_data=np.array([[0, 1],
-                                                 [2, 3],
-                                                 [4, 5],
-                                                 [6, 7],
-                                                 [8, 9]]))
-
-    var_spec['Variable'] = 'Variable2'
-    var_spec['Var_Type'] = 'zvariable'
-    varatts = {}
-    varatts['Attribute1'] = 2
-    varatts['Attribute2'] = '1000'
-    tfile.write_var(var_spec, var_attrs=varatts,
-                    var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
+    var_spec: Dict[str, Any] = {}
+    var_spec["Variable"] = "Variable1"
+    var_spec["Var_Type"] = "rvariable"
+    var_spec["Data_Type"] = 22
+    var_spec["Num_Elements"] = 1
+    var_spec["Rec_Vary"] = True
+    var_spec["Dim_Sizes"] = []
+    var_spec["Dim_Vary"] = [True, False]
+
+    tfile = cdf_create(fn, {"rDim_sizes": [2, 20]})
+    tfile.write_var(var_spec, var_data=np.array([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]))
+
+    var_spec["Variable"] = "Variable2"
+    var_spec["Var_Type"] = "zvariable"
+    varatts: Dict[str, Any] = {}
+    varatts["Attribute1"] = 2
+    varatts["Attribute2"] = "1000"
+    tfile.write_var(var_spec, var_attrs=varatts, var_data=np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
 
     tfile.close()
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     varinfo = reader.varinq("Variable1")
-    assert varinfo['Data_Type'] == 22
+    assert varinfo.Data_Type == 22
 
     var = reader.varget("Variable1")
     for x in [0, 1, 2, 3, 4]:
-        assert var[x][0] == 2*x
-        assert var[x][1] == 2*x+1
+        assert var[x][0] == 2 * x
+        assert var[x][1] == 2 * x + 1
 
     var = reader.varget("Variable2")
-    assert (var == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]).all()
-
-    att = reader.attget("Attribute1", entry='Variable2')
-    assert att['Data'] == [2]
-
-    att = reader.attget("Attribute2", entry='Variable2')
-    assert att['Data'] == '1000'
+    np.testing.assert_equal(var, [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 
+    att = reader.attget("Attribute1", entry="Variable2")
+    assert att.Data == [2]
 
-if __name__ == '__main__':
-    pytest.main([__file__])
+    att = reader.attget("Attribute2", entry="Variable2")
+    assert att.Data == "1000"
```

### Comparing `cdflib-0.4.9/tests/test_epochs.py` & `cdflib-1.0.0/tests/test_epochs.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,97 +10,95 @@
 import pytest
 from hypothesis import example, given, settings, strategies
 from pytest import approx
 
 from cdflib import epochs
 from cdflib.epochs import CDFepoch as cdfepoch
 
-'''
+"""
 To check code coverage, first:
 
 pip install pytest-cov
 
 Then
 
 pytest --cov
 
 This will run all unit tests.  To view the coverage results:
 
 coverage report
 
 Each of these results were hand checked using either IDL or
 other online resources.
-'''
+"""
 
 # These are the supported years for TT2000 dates; see
 # https://cdf.gsfc.nasa.gov/html/leapseconds_requirements.html
 # section 2.1
 random_tt2000_dtime = strategies.datetimes(
-    min_value=datetime(1707, 9, 22, 12, 13, 16),
-    max_value=(datetime(2292, 4, 11, 11, 46, 8)))
+    min_value=datetime(1707, 9, 22, 12, 13, 16), max_value=(datetime(2292, 4, 11, 11, 46, 8))
+)
 
 # These are the supported years for CDF files; see
 # https://spdf.gsfc.nasa.gov/pub/software/cdf/doc/cdf371/cdf371ug.pdf
 # page 55
-random_dtime = strategies.datetimes(min_value=datetime(1709, 1, 1),
-                                    max_value=(datetime(2293, 1, 1) -
-                                               timedelta(milliseconds=1)))
+random_dtime = strategies.datetimes(min_value=datetime(1709, 1, 1), max_value=(datetime(2293, 1, 1) - timedelta(milliseconds=1)))
 
 
 def test_encode_cdfepoch():
     x = cdfepoch.encode([62285326000000.0, 62985326000000.0])
-    assert x[0] == '1973-09-28T23:26:40.000'
-    assert x[1] == '1995-12-04T19:53:20.000'
+    assert x[0] == "1973-09-28T23:26:40.000"
+    assert x[1] == "1995-12-04T19:53:20.000"
 
     y = cdfepoch.encode(62975326000002.0, iso_8601=False)
-    assert y == '11-Aug-1995 02:06:40.002'
+    assert y == "11-Aug-1995 02:06:40.002"
 
 
 def test_encode_cdfepoch16():
-    '''
+    """
     cdf_encode_epoch16(dcomplex(63300946758.000000, 176214648000.00000)) in IDL
     returns 04-Dec-2005 20:39:28.176.214.654.976
 
     However, I believe this IDL routine is bugged.  This website:
     https://www.epochconverter.com/seconds-days-since-y0
     shows a correct answer.
-    '''
+    """
     x = cdfepoch.encode(np.complex128(63300946758.000000 + 176214648000.00000j))
-    assert x == '2005-12-04T20:19:18.176214648000'
-    y = cdfepoch.encode(np.complex128([33300946758.000000 + 106014648000.00000j,
-                                       61234543210.000000 + 000011148000.00000j]),
-                        iso_8601=False)
-    assert y[0] == '07-Apr-1055 14:59:18.106.014.648.000'
-    assert y[1] == '12-Jun-1940 03:20:10.000.011.148.000'
+    assert x == "2005-12-04T20:19:18.176214648000"
+    y = cdfepoch.encode(
+        np.array([33300946758.000000 + 106014648000.00000j, 61234543210.000000 + 000011148000.00000j]), iso_8601=False
+    )
+    assert y[0] == "07-Apr-1055 14:59:18.106.014.648.000"
+    assert y[1] == "12-Jun-1940 03:20:10.000.011.148.000"
 
 
 def test_encode_cdftt2000():
     x = cdfepoch.encode(186999622360321123)
-    assert x == '2005-12-04T20:19:18.176321123'
-    y = cdfepoch.encode([500000000100, 123456789101112131],
-                        iso_8601=False)
-    assert y[0] == '01-Jan-2000 12:07:15.816.000.100'
-    assert y[1] == '30-Nov-2003 09:32:04.917.112.131'
+    assert x == "2005-12-04T20:19:18.176321123"
+    y = cdfepoch.encode([500000000100, 123456789101112131], iso_8601=False)
+    assert y[0] == "01-Jan-2000 12:07:15.816.000.100"
+    assert y[1] == "30-Nov-2003 09:32:04.917.112.131"
 
 
 def test_unixtime():
     x = cdfepoch.unixtime([500000000100, 123456789101112131])
+    assert isinstance(x, np.ndarray)
     assert x[0] == 946728435.816
     assert x[1] == 1070184724.917112
 
 
-@pytest.mark.parametrize('tzone', ['UTC', 'EST'])
+@pytest.mark.parametrize("tzone", ["UTC", "EST"])
 def test_unixtime_roundtrip(tzone):
     _environ = os.environ.copy()
     try:
-        os.environ['TZ'] = tzone
+        os.environ["TZ"] = tzone
         y, m, d = 2000, 1, 1
         epoch = cdfepoch.compute_tt2000([[y, m, d]])
         unixtime = cdfepoch.unixtime(epoch)
-        assert unixtime == [946684800.0]
+        assert unixtime == 946684800.0
     finally:
         os.environ.clear()
         os.environ.update(_environ)
 
 
 def test_breakdown_cdfepoch():
     x = cdfepoch.breakdown([62285326000000.0, 62985326000000.0])
@@ -148,57 +146,65 @@
     assert x[7] == 112
     assert x[8] == 131
 
 
 @given(random_dtime)
 @settings(max_examples=100)
 def test_compute_cdfepoch(dtime):
-    '''
+    """
     Using random numbers for the compute tests
-    '''
-    random_time = [dtime.year, dtime.month, dtime.day,
-                   dtime.hour, dtime.minute, dtime.second,
-                   dtime.microsecond // 1000]
+    """
+    random_time = [dtime.year, dtime.month, dtime.day, dtime.hour, dtime.minute, dtime.second, dtime.microsecond // 1000]
     x = cdfepoch.breakdown(cdfepoch.compute(random_time))
     i = 0
     for t in x:
-        assert t == random_time[i], f'Time {random_time} was not equal to {x}'
+        assert t == random_time[i], f"Time {random_time} was not equal to {x}"
         i += 1
 
 
 @given(random_dtime)
 @settings(max_examples=100)
 def test_compute_cdfepoch16(dtime):
-    random_time = [dtime.year, dtime.month, dtime.day,
-                   dtime.hour, dtime.minute, dtime.second,
-                   dtime.microsecond // 1000,  # Millisecond
-                   randint(0, 999),     # Microsecond
-                   randint(0, 999),     # Nanosecond
-                   randint(0, 999),     # Picosecond
-                   ]
+    random_time = [
+        dtime.year,
+        dtime.month,
+        dtime.day,
+        dtime.hour,
+        dtime.minute,
+        dtime.second,
+        dtime.microsecond // 1000,  # Millisecond
+        randint(0, 999),  # Microsecond
+        randint(0, 999),  # Nanosecond
+        randint(0, 999),  # Picosecond
+    ]
     x = cdfepoch.breakdown(cdfepoch.compute(random_time))
     i = 0
     for t in x:
-        assert t == random_time[i], f'Time {random_time} was not equal to {x}'
+        assert t == random_time[i], f"Time {random_time} was not equal to {x}"
         i += 1
 
 
 @given(random_tt2000_dtime)
 @settings(max_examples=100)
 @example(datetime(1972, 1, 1, 0, 0))
 def test_compute_cdftt2000(dtime):
-    random_time = [dtime.year, dtime.month, dtime.day,
-                   dtime.hour, dtime.minute, dtime.second,
-                   dtime.microsecond // 1000,  # Millisecond
-                   randint(0, 999),     # Microsecond
-                   randint(0, 999),     # Nanosecond
-                   ]
+    random_time = [
+        dtime.year,
+        dtime.month,
+        dtime.day,
+        dtime.hour,
+        dtime.minute,
+        dtime.second,
+        dtime.microsecond // 1000,  # Millisecond
+        randint(0, 999),  # Microsecond
+        randint(0, 999),  # Nanosecond
+    ]
     x = cdfepoch.breakdown(cdfepoch.compute(random_time))
     for i, t in enumerate(x):
-        assert t == random_time[i], f'Time {random_time} was not equal to {x}'
+        assert t == random_time[i], f"Time {random_time} was not equal to {x}"
 
 
 def test_parse_cdfepoch():
     x = cdfepoch.encode(62567898765432.0)
     assert x == "1982-09-12T11:52:45.432"
     parsed = cdfepoch.parse(x)
     assert parsed == approx(62567898765432.0)
@@ -207,39 +213,39 @@
 def test_parse_cdfepoch16():
     input_time = 53467976543.0 + 543218654100j
     x = cdfepoch.encode(input_time)
     assert x == "1694-05-01T07:42:23.543218654100"
     parsed = cdfepoch.parse(x)
     assert parsed == input_time
 
-    assert cdfepoch().to_datetime(parsed) == [datetime(1694, 5, 1, 7, 42, 23, 543218)]
+    assert cdfepoch().to_datetime(parsed) == datetime(1694, 5, 1, 7, 42, 23, 543218)
 
 
 def test_parse_cdftt2000():
     input_time = 131415926535793238
     x = cdfepoch.encode(input_time)
     assert x == "2004-03-01T12:24:22.351793238"
     parsed = cdfepoch.parse(x)
     assert parsed == input_time
 
-    assert cdfepoch().to_datetime(parsed) == [datetime(2004, 3, 1, 12, 24, 22, 351793)]
+    assert cdfepoch().to_datetime(parsed) == datetime(2004, 3, 1, 12, 24, 22, 351793)
 
 
 def test_findepochrange_cdfepoch():
     start_time = "2013-12-01T12:24:22.000"
     end_time = "2014-12-01T12:24:22.000"
     x = cdfepoch.parse([start_time, end_time])
     time_array = np.arange(x[0], x[1], step=1000000)
 
     test_start = [2014, 8, 1, 8, 1, 54, 123]
     test_end = [2018, 1, 1, 1, 1, 1, 1]
     index = cdfepoch.findepochrange(time_array, starttime=test_start, endtime=test_end)
     # Test that the test_start is less than the first index, but more than one less
     assert time_array[index[0]] >= cdfepoch.compute(test_start)
-    assert time_array[index[0]-1] <= cdfepoch.compute(test_start)
+    assert time_array[index[0] - 1] <= cdfepoch.compute(test_start)
 
     assert time_array[index[-1]] <= cdfepoch.compute(test_end)
 
 
 def test_findepochrange_cdftt2000():
     start_time = "2004-03-01T12:24:22.351793238"
     end_time = "2004-03-01T12:28:22.351793238"
@@ -247,48 +253,48 @@
     time_array = np.arange(x[0], x[1], step=1000000)
 
     test_start = [2004, 3, 1, 12, 25, 54, 123, 111, 98]
     test_end = [2004, 3, 1, 12, 26, 4, 123, 456, 789]
     index = cdfepoch.findepochrange(time_array, starttime=test_start, endtime=test_end)
     # Test that the test_start is less than the first index, but more than one less
     assert time_array[index[0]] >= cdfepoch.compute(test_start)
-    assert time_array[index[0]-1] <= cdfepoch.compute(test_start)
+    assert time_array[index[0] - 1] <= cdfepoch.compute(test_start)
 
     assert time_array[index[-1]] <= cdfepoch.compute(test_end)
-    assert time_array[index[-1]+1] >= cdfepoch.compute(test_end)
+    assert time_array[index[-1] + 1] >= cdfepoch.compute(test_end)
 
 
 def test_findepochrange_cdfepoch16():
     start_time = "1978-03-10T03:24:22.351793238462"
     end_time = "1978-06-13T01:28:22.338327950466"
     x = cdfepoch.parse([start_time, end_time])
     first_int_step = int((x[1].real - x[0].real) / 1000)
     second_int_step = int((x[1].imag - x[0].imag) / 1000)
     time_array = []
     for i in range(0, 1000):
-        time_array.append(x[0]+complex(first_int_step*i, second_int_step*i))
+        time_array.append(x[0] + complex(first_int_step * i, second_int_step * i))
 
     test_start = [1978, 6, 10, 3, 24, 22, 351, 793, 238, 462]
     test_end = [1978, 6, 12, 23, 11, 1, 338, 341, 416, 466]
     index = cdfepoch.findepochrange(time_array, starttime=test_start, endtime=test_end)
 
     # Test that the test_start is less than the first index, but more than one less
     assert time_array[index[0]].real >= cdfepoch.compute(test_start).real
-    assert time_array[index[0]-1].real <= cdfepoch.compute(test_start).real
+    assert time_array[index[0] - 1].real <= cdfepoch.compute(test_start).real
     assert time_array[index[-1]].real <= cdfepoch.compute(test_end).real
-    assert time_array[index[-1]+1].real >= cdfepoch.compute(test_end).real
+    assert time_array[index[-1] + 1].real >= cdfepoch.compute(test_end).real
 
 
 def test_latest_leapsecs():
     # Check that the built in leapseconds table is the latest one
     local = epochs.LEAPSEC_FILE
     try:
-        remote, _ = urllib.request.urlretrieve('https://cdf.gsfc.nasa.gov/html/CDFLeapSeconds.txt')
+        remote, _ = urllib.request.urlretrieve("https://cdf.gsfc.nasa.gov/html/CDFLeapSeconds.txt")
     except Exception as excp:
-        pytest.skip(f'problem downloading leapseconds file: {excp}')
+        pytest.skip(f"problem downloading leapseconds file: {excp}")
     if not filecmp.cmp(local, remote):
-        feedback = Path(remote).read_text(errors='ignore')
-        pytest.skip(f'problem downloading leapseconds file: \n\n{feedback}')
+        feedback = Path(remote).read_text(errors="ignore")
+        pytest.skip(f"problem downloading leapseconds file: \n\n{feedback}")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     pytest.main([__file__])
```

### Comparing `cdflib-0.4.9/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf` & `cdflib-1.0.0/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-0.4.9/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `cdflib-1.0.0/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

