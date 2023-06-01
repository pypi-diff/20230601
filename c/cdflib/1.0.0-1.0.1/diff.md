# Comparing `tmp/cdflib-1.0.0.tar.gz` & `tmp/cdflib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdflib-1.0.0.tar", last modified: Thu Jun  1 19:40:17 2023, max compression
+gzip compressed data, was "cdflib-1.0.1.tar", last modified: Thu Jun  1 20:00:38 2023, max compression
```

## Comparing `cdflib-1.0.0.tar` & `cdflib-1.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-01 19:40:00.000000 cdflib-1.0.0/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-01 19:40:00.000000 cdflib-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 19:40:00.000000 cdflib-1.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.037493 cdflib-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-01 19:40:00.000000 cdflib-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-01 19:40:00.000000 cdflib-1.0.0/.github/workflows/pypi-build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-01 19:40:00.000000 cdflib-1.0.0/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-01 19:40:00.000000 cdflib-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 19:40:00.000000 cdflib-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-01 19:40:00.000000 cdflib-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 19:40:00.000000 cdflib-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 19:40:00.000000 cdflib-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-01 19:40:17.045493 cdflib-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 19:40:00.000000 cdflib-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 19:40:00.000000 cdflib-1.0.0/archive/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-01 19:40:00.000000 cdflib-1.0.0/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:00.000000 cdflib-1.0.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-01 19:40:00.000000 cdflib-1.0.0/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/cdflib/
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/CDFLeapSeconds.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 19:40:16.000000 cdflib-1.0.0/cdflib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38003 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/cdf_to_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    84619 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)   104337 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/cdfwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    65531 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/epochs_astropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32046 2023-06-01 19:40:00.000000 cdflib-1.0.0/cdflib/xarray_to_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.041493 cdflib-1.0.0/cdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 19:40:17.000000 cdflib-1.0.0/cdflib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/cdfepoch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/cdfread.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/cdfwrite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/dataclasses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 19:40:00.000000 cdflib-1.0.0/doc/modules/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 19:40:00.000000 cdflib-1.0.0/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-01 19:40:00.000000 cdflib-1.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 19:40:00.000000 cdflib-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 19:40:17.045493 cdflib-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_astropy_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_cdfread_rle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_cdfwrite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/test_xarray_reader_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:40:17.045493 cdflib-1.0.0/tests/testfiles/
--rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 19:40:00.000000 cdflib-1.0.0/tests/testfiles/testing_file_location.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 19:40:00.000000 cdflib-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.368552 cdflib-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.364552 cdflib-1.0.1/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-01 20:00:23.000000 cdflib-1.0.1/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-01 20:00:23.000000 cdflib-1.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 20:00:23.000000 cdflib-1.0.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.360552 cdflib-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.364552 cdflib-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-01 20:00:23.000000 cdflib-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-01 20:00:23.000000 cdflib-1.0.1/.github/workflows/pypi-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-01 20:00:23.000000 cdflib-1.0.1/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-01 20:00:23.000000 cdflib-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 20:00:23.000000 cdflib-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-01 20:00:23.000000 cdflib-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 20:00:23.000000 cdflib-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 20:00:23.000000 cdflib-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-01 20:00:38.368552 cdflib-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 20:00:23.000000 cdflib-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.364552 cdflib-1.0.1/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 20:00:23.000000 cdflib-1.0.1/archive/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-01 20:00:23.000000 cdflib-1.0.1/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.364552 cdflib-1.0.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:23.000000 cdflib-1.0.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-01 20:00:23.000000 cdflib-1.0.1/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.368552 cdflib-1.0.1/cdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/CDFLeapSeconds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 20:00:38.000000 cdflib-1.0.1/cdflib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38003 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/cdf_to_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84619 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104337 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/cdfwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65531 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/epochs_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32046 2023-06-01 20:00:23.000000 cdflib-1.0.1/cdflib/xarray_to_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.368552 cdflib-1.0.1/cdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-01 20:00:38.000000 cdflib-1.0.1/cdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-01 20:00:38.000000 cdflib-1.0.1/cdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:00:38.000000 cdflib-1.0.1/cdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 20:00:38.000000 cdflib-1.0.1/cdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 20:00:38.000000 cdflib-1.0.1/cdflib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.368552 cdflib-1.0.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.368552 cdflib-1.0.1/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/modules/cdfepoch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/modules/cdfread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/modules/cdfwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/modules/dataclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 20:00:23.000000 cdflib-1.0.1/doc/modules/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 20:00:23.000000 cdflib-1.0.1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-01 20:00:23.000000 cdflib-1.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 20:00:23.000000 cdflib-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 20:00:38.368552 cdflib-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.368552 cdflib-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/test_astropy_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/test_cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/test_cdfread_rle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/test_cdfwrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/test_xarray_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:00:38.368552 cdflib-1.0.1/tests/testfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 20:00:23.000000 cdflib-1.0.1/tests/testfiles/testing_file_location.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 20:00:23.000000 cdflib-1.0.1/tox.ini
```

### Comparing `cdflib-1.0.0/.circleci/config.yml` & `cdflib-1.0.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/.github/workflows/ci.yml` & `cdflib-1.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/.github/workflows/pypi-build.yaml` & `cdflib-1.0.1/.github/workflows/pypi-build.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/.github/workflows/python-lint.yml` & `cdflib-1.0.1/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/.pre-commit-config.yaml` & `cdflib-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/.readthedocs.yml` & `cdflib-1.0.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/LICENSE` & `cdflib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/PKG-INFO` & `cdflib-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.0/README.md` & `cdflib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/asv.conf.json` & `cdflib-1.0.1/asv.conf.json`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/benchmarks/benchmarks.py` & `cdflib-1.0.1/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/CDFLeapSeconds.txt` & `cdflib-1.0.1/cdflib/CDFLeapSeconds.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/cdf_to_xarray.py` & `cdflib-1.0.1/cdflib/cdf_to_xarray.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/cdfread.py` & `cdflib-1.0.1/cdflib/cdfread.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/cdfwrite.py` & `cdflib-1.0.1/cdflib/cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/dataclasses.py` & `cdflib-1.0.1/cdflib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/epochs.py` & `cdflib-1.0.1/cdflib/epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/epochs_astropy.py` & `cdflib-1.0.1/cdflib/epochs_astropy.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/s3.py` & `cdflib-1.0.1/cdflib/s3.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib/xarray_to_cdf.py` & `cdflib-1.0.1/cdflib/xarray_to_cdf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/cdflib.egg-info/PKG-INFO` & `cdflib-1.0.1/cdflib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.0/cdflib.egg-info/SOURCES.txt` & `cdflib-1.0.1/cdflib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/doc/Makefile` & `cdflib-1.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/doc/changelog.rst` & `cdflib-1.0.1/doc/changelog.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+1.0.1
+=====
+To keep ``astropy`` and ``xarray`` as optional dependencies, ``cdfastropy``,
+``cdf_to_xarray``, and ``xarray_to_cdf`` are no longer available under ``cdflib``.
+Instead import them from ``cdflib.xarray_to_cdf``, ``cdflib.cdf_to_xarray``, or
+``cdflib.epochs_astropy``.
+
 1.0.0
 =====
 Version 1.0.0 is a new major version for ``cdflib``, and contains a number
 of breaking changes. These have been made to improve consistency across the
 package, and make it easier to maintain and build on the package going forward
 in the future.
```

### Comparing `cdflib-1.0.0/doc/conf.py` & `cdflib-1.0.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/doc/index.rst` & `cdflib-1.0.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/doc/make.bat` & `cdflib-1.0.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/doc/modules/cdfepoch.rst` & `cdflib-1.0.1/doc/modules/cdfepoch.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/doc/modules/cdfread.rst` & `cdflib-1.0.1/doc/modules/cdfread.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/doc/modules/cdfwrite.rst` & `cdflib-1.0.1/doc/modules/cdfwrite.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/meta.yaml` & `cdflib-1.0.1/meta.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/mypy.ini` & `cdflib-1.0.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/setup.cfg` & `cdflib-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/tests/test_astropy_epochs.py` & `cdflib-1.0.1/tests/test_astropy_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/tests/test_cdfread.py` & `cdflib-1.0.1/tests/test_cdfread.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/tests/test_cdfwrite.py` & `cdflib-1.0.1/tests/test_cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/tests/test_epochs.py` & `cdflib-1.0.1/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/tests/test_xarray_reader_writer.py` & `cdflib-1.0.1/tests/test_xarray_reader_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import urllib.request
 
 import pytest
 import xarray as xr
 
-import cdflib
+from cdflib.cdf_to_xarray import cdf_to_xarray
+from cdflib.xarray_to_cdf import xarray_to_cdf
 
 # To run these tests use `pytest --remote-data`
 
 # These unit tests read in data to xarray, typically in the form of a CDF or netCDF file, and then spit it back out
 # again into a CDF file.  The created CDF files are then read back into xarray with the cdf_to_xarray function.
 
 # The files are hosted on the MAVEN SDC website.  If that website becomes defunct in the future, a new location for
@@ -38,26 +39,26 @@
 )
 @pytest.mark.remote_data
 def test_xarray_read_write(tmp_path, cdf_fname, nc_fname):
     url = f"https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/{cdf_fname}"
     if not os.path.exists(cdf_fname):
         urllib.request.urlretrieve(url, cdf_fname)
 
-    a = cdflib.cdf_to_xarray(cdf_fname, to_unixtime=True, fillval_to_nan=True)
+    a = cdf_to_xarray(cdf_fname, to_unixtime=True, fillval_to_nan=True)
 
-    cdflib.xarray_to_cdf(a, tmp_path / cdf_fname, from_unixtime=True)
-    b = cdflib.cdf_to_xarray(tmp_path / cdf_fname, to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(a, tmp_path / cdf_fname, from_unixtime=True)
+    b = cdf_to_xarray(tmp_path / cdf_fname, to_unixtime=True, fillval_to_nan=True)
 
     url = f"https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/{nc_fname}"
     if not os.path.exists(nc_fname):
         urllib.request.urlretrieve(url, nc_fname)
 
     c = xr.load_dataset(nc_fname)
-    cdflib.xarray_to_cdf(c, tmp_path / ("nc_" + cdf_fname))
-    d = cdflib.cdf_to_xarray(tmp_path / ("nc_" + cdf_fname), to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(c, tmp_path / ("nc_" + cdf_fname))
+    d = cdf_to_xarray(tmp_path / ("nc_" + cdf_fname), to_unixtime=True, fillval_to_nan=True)
 
 
 @pytest.mark.remote_data
 def test_MGITM_model():
     fname = "MGITM_LS180_F130_150615.nc"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/MGITM_LS180_F130_150615.nc"
     if not os.path.exists(fname):
@@ -67,16 +68,16 @@
     for var in c:
         c[var].attrs["VAR_TYPE"] = "data"
     c = c.rename({"Latitude": "latitude", "Longitude": "longitude"})
     c["longitude"].attrs["VAR_TYPE"] = "support_data"
     c["latitude"].attrs["VAR_TYPE"] = "support_data"
     c["altitude"].attrs["VAR_TYPE"] = "support_data"
 
-    cdflib.xarray_to_cdf(c, "MGITM_LS180_F130_150615-created-from-netcdf-input.cdf")
-    d = cdflib.cdf_to_xarray("MGITM_LS180_F130_150615-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(c, "MGITM_LS180_F130_150615-created-from-netcdf-input.cdf")
+    d = cdf_to_xarray("MGITM_LS180_F130_150615-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("MGITM_LS180_F130_150615-created-from-netcdf-input.cdf")
     os.remove("MGITM_LS180_F130_150615.nc")
 
 
 @pytest.mark.remote_data
 def test_goes_mag():
     fname = "dn_magn-l2-hires_g17_d20211219_v1-0-1.nc"
@@ -86,18 +87,16 @@
 
     c = xr.load_dataset("dn_magn-l2-hires_g17_d20211219_v1-0-1.nc")
     for var in c:
         c[var].attrs["VAR_TYPE"] = "data"
     c["coordinate"].attrs["VAR_TYPE"] = "support_data"
     c["time"].attrs["VAR_TYPE"] = "support_data"
     c["time_orbit"].attrs["VAR_TYPE"] = "support_data"
-    cdflib.xarray_to_cdf(c, "dn_magn-l2-hires_g17_d20211219_v1-0-1-created-from-netcdf-input.cdf")
-    d = cdflib.cdf_to_xarray(
-        "dn_magn-l2-hires_g17_d20211219_v1-0-1-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True
-    )
+    xarray_to_cdf(c, "dn_magn-l2-hires_g17_d20211219_v1-0-1-created-from-netcdf-input.cdf")
+    d = cdf_to_xarray("dn_magn-l2-hires_g17_d20211219_v1-0-1-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("dn_magn-l2-hires_g17_d20211219_v1-0-1-created-from-netcdf-input.cdf")
     os.remove("dn_magn-l2-hires_g17_d20211219_v1-0-1.nc")
 
 
 @pytest.mark.remote_data
 def test_saber():
     fname = "SABER_L2B_2021020_103692_02.07.nc"
@@ -108,58 +107,58 @@
     c = xr.load_dataset("SABER_L2B_2021020_103692_02.07.nc")
     for var in c:
         c[var].attrs["VAR_TYPE"] = "data"
     c["event"].attrs["VAR_TYPE"] = "support_data"
     c["sclatitude"].attrs["VAR_TYPE"] = "support_data"
     c["sclongitude"].attrs["VAR_TYPE"] = "support_data"
     c["scaltitude"].attrs["VAR_TYPE"] = "support_data"
-    cdflib.xarray_to_cdf(c, "SABER_L2B_2021020_103692_02.07-created-from-netcdf-input.cdf")
-    d = cdflib.cdf_to_xarray("SABER_L2B_2021020_103692_02.07-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(c, "SABER_L2B_2021020_103692_02.07-created-from-netcdf-input.cdf")
+    d = cdf_to_xarray("SABER_L2B_2021020_103692_02.07-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("SABER_L2B_2021020_103692_02.07-created-from-netcdf-input.cdf")
     os.remove("SABER_L2B_2021020_103692_02.07.nc")
 
 
 @pytest.mark.remote_data
 def test_euv():
     fname = "mvn_euv_l3_minute_20201130_v14_r02.cdf"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mvn_euv_l3_minute_20201130_v14_r02.cdf"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
-    a = cdflib.cdf_to_xarray("mvn_euv_l3_minute_20201130_v14_r02.cdf", to_unixtime=True, fillval_to_nan=True)
-    cdflib.xarray_to_cdf(a, "mvn_euv_l3_minute_20201130_v14_r02-created-from-cdf-input.cdf", from_unixtime=True)
-    b = cdflib.cdf_to_xarray("mvn_euv_l3_minute_20201130_v14_r02-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
+    a = cdf_to_xarray("mvn_euv_l3_minute_20201130_v14_r02.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(a, "mvn_euv_l3_minute_20201130_v14_r02-created-from-cdf-input.cdf", from_unixtime=True)
+    b = cdf_to_xarray("mvn_euv_l3_minute_20201130_v14_r02-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("mvn_euv_l3_minute_20201130_v14_r02-created-from-cdf-input.cdf")
     os.remove("mvn_euv_l3_minute_20201130_v14_r02.cdf")
 
 
 @pytest.mark.remote_data
 def test_sep_anc():
     fname = "mvn_sep_l2_anc_20210501_v06_r00.cdf"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mvn_sep_l2_anc_20210501_v06_r00.cdf"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
-    a = cdflib.cdf_to_xarray("mvn_sep_l2_anc_20210501_v06_r00.cdf", to_unixtime=True, fillval_to_nan=True)
-    cdflib.xarray_to_cdf(a, "mvn_sep_l2_anc_20210501_v06_r00-created-from-cdf-input.cdf", from_unixtime=True)
-    a = cdflib.cdf_to_xarray("mvn_sep_l2_anc_20210501_v06_r00-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
+    a = cdf_to_xarray("mvn_sep_l2_anc_20210501_v06_r00.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(a, "mvn_sep_l2_anc_20210501_v06_r00-created-from-cdf-input.cdf", from_unixtime=True)
+    a = cdf_to_xarray("mvn_sep_l2_anc_20210501_v06_r00-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("mvn_sep_l2_anc_20210501_v06_r00-created-from-cdf-input.cdf")
     os.remove("mvn_sep_l2_anc_20210501_v06_r00.cdf")
 
 
 @pytest.mark.remote_data
 def test_sep_svy():
     fname = "mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05.cdf"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05.cdf"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
-    a = cdflib.cdf_to_xarray("mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05.cdf", to_unixtime=True, fillval_to_nan=True)
-    cdflib.xarray_to_cdf(a, "mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05-created-from-cdf-input.cdf", from_unixtime=True)
-    b = cdflib.cdf_to_xarray(
+    a = cdf_to_xarray("mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(a, "mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05-created-from-cdf-input.cdf", from_unixtime=True)
+    b = cdf_to_xarray(
         "mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True
     )
     os.remove("mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05-created-from-cdf-input.cdf")
     os.remove("mvn_sep_l2_s2-raw-svy-full_20191231_v04_r05.cdf")
 
 
 """
@@ -169,90 +168,84 @@
 
     fname = 'mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04.cdf'
     url = (
         "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04.cdf")
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
-    a = cdflib.cdf_to_xarray("mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04.cdf", to_unixtime=True,
+    a = cdf_to_xarray("mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04.cdf", to_unixtime=True,
                              fillval_to_nan=True)
-    cdflib.xarray_to_cdf(a, 'mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04-created-from-cdf-input.cdf', from_unixtime=True)
-    b = cdflib.cdf_to_xarray('mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04-created-from-cdf-input.cdf', to_unixtime=True,
+    xarray_to_cdf(a, 'mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04-created-from-cdf-input.cdf', from_unixtime=True)
+    b = cdf_to_xarray('mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04-created-from-cdf-input.cdf', to_unixtime=True,
                              fillval_to_nan=True)
     os.remove('mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04-created-from-cdf-input.cdf')
     os.remove('mvn_sta_l2_d1-32e4d16a8m_20201130_v02_r04.cdf')
 """
 
 
 @pytest.mark.remote_data
 def test_swe_arc3d():
     fname = "mvn_swe_l2_arc3d_20180717_v04_r02.cdf"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mvn_swe_l2_arc3d_20180717_v04_r02.cdf"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
-    a = cdflib.cdf_to_xarray("mvn_swe_l2_arc3d_20180717_v04_r02.cdf", to_unixtime=True, fillval_to_nan=True)
-    cdflib.xarray_to_cdf(a, "mvn_swe_l2_arc3d_20180717_v04_r02-created-from-cdf-input.cdf", from_unixtime=True)
-    b = cdflib.cdf_to_xarray("mvn_swe_l2_arc3d_20180717_v04_r02-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
+    a = cdf_to_xarray("mvn_swe_l2_arc3d_20180717_v04_r02.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(a, "mvn_swe_l2_arc3d_20180717_v04_r02-created-from-cdf-input.cdf", from_unixtime=True)
+    b = cdf_to_xarray("mvn_swe_l2_arc3d_20180717_v04_r02-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("mvn_swe_l2_arc3d_20180717_v04_r02-created-from-cdf-input.cdf")
     os.remove("mvn_swe_l2_arc3d_20180717_v04_r02.cdf")
 
     fname = "mvn_swe_l2_arc3d_20180717_v04_r02.nc"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mvn_swe_l2_arc3d_20180717_v04_r02.nc"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
     c = xr.load_dataset("mvn_swe_l2_arc3d_20180717_v04_r02.nc")
-    cdflib.xarray_to_cdf(c, "mvn_swe_l2_arc3d_20180717_v04_r02-created-from-netcdf-input.cdf")
-    d = cdflib.cdf_to_xarray(
-        "mvn_swe_l2_arc3d_20180717_v04_r02-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True
-    )
+    xarray_to_cdf(c, "mvn_swe_l2_arc3d_20180717_v04_r02-created-from-netcdf-input.cdf")
+    d = cdf_to_xarray("mvn_swe_l2_arc3d_20180717_v04_r02-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("mvn_swe_l2_arc3d_20180717_v04_r02-created-from-netcdf-input.cdf")
     os.remove("mvn_swe_l2_arc3d_20180717_v04_r02.nc")
 
 
 @pytest.mark.remote_data
 def test_swe_svyspec():
     fname = "mvn_swe_l2_svyspec_20180718_v04_r04.cdf"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mvn_swe_l2_svyspec_20180718_v04_r04.cdf"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
-    a = cdflib.cdf_to_xarray("mvn_swe_l2_svyspec_20180718_v04_r04.cdf", to_unixtime=True, fillval_to_nan=True)
-    cdflib.xarray_to_cdf(a, "mvn_swe_l2_svyspec_20180718_v04_r04-created-from-cdf-input.cdf", from_unixtime=True)
-    b = cdflib.cdf_to_xarray(
-        "mvn_swe_l2_svyspec_20180718_v04_r04-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True
-    )
+    a = cdf_to_xarray("mvn_swe_l2_svyspec_20180718_v04_r04.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(a, "mvn_swe_l2_svyspec_20180718_v04_r04-created-from-cdf-input.cdf", from_unixtime=True)
+    b = cdf_to_xarray("mvn_swe_l2_svyspec_20180718_v04_r04-created-from-cdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("mvn_swe_l2_svyspec_20180718_v04_r04-created-from-cdf-input.cdf")
     os.remove("mvn_swe_l2_svyspec_20180718_v04_r04.cdf")
 
     fname = "mvn_swe_l2_svyspec_20180718_v04_r04.nc"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mvn_swe_l2_svyspec_20180718_v04_r04.nc"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
     c = xr.load_dataset("mvn_swe_l2_svyspec_20180718_v04_r04.nc")
-    cdflib.xarray_to_cdf(c, "mvn_swe_l2_svyspec_20180718_v04_r04-created-from-netcdf-input.cdf")
-    d = cdflib.cdf_to_xarray(
-        "mvn_swe_l2_svyspec_20180718_v04_r04-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True
-    )
+    xarray_to_cdf(c, "mvn_swe_l2_svyspec_20180718_v04_r04-created-from-netcdf-input.cdf")
+    d = cdf_to_xarray("mvn_swe_l2_svyspec_20180718_v04_r04-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("mvn_swe_l2_svyspec_20180718_v04_r04-created-from-netcdf-input.cdf")
     os.remove("mvn_swe_l2_svyspec_20180718_v04_r04.nc")
 
 
 @pytest.mark.remote_data
 def test_raids():
     fname = "raids_nirs_20100823_v1.1.nc"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/raids_nirs_20100823_v1.1.nc"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
     c = xr.load_dataset("raids_nirs_20100823_v1.1.nc")
-    cdflib.xarray_to_cdf(c, "raids_nirs_20100823_v1.1-created-from-netcdf-input.cdf")
-    d = cdflib.cdf_to_xarray("raids_nirs_20100823_v1.1-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(c, "raids_nirs_20100823_v1.1-created-from-netcdf-input.cdf")
+    d = cdf_to_xarray("raids_nirs_20100823_v1.1-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("raids_nirs_20100823_v1.1-created-from-netcdf-input.cdf")
     os.remove("raids_nirs_20100823_v1.1.nc")
 
 
 """
 # TOO MUCH MEMORY
 
@@ -260,77 +253,77 @@
 
     fname = 'rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2.cdf'
     url = (
         "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2.cdf")
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
-    a = cdflib.cdf_to_xarray("rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2.cdf",
+    a = cdf_to_xarray("rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2.cdf",
                              to_unixtime=True, fillval_to_nan=True)
-    cdflib.xarray_to_cdf(a, 'rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2-created-from-cdf-input.cdf',
+    xarray_to_cdf(a, 'rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2-created-from-cdf-input.cdf',
                          from_unixtime=True)
-    b = cdflib.cdf_to_xarray('rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2-created-from-cdf-input.cdf',
+    b = cdf_to_xarray('rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2-created-from-cdf-input.cdf',
                              to_unixtime=True, fillval_to_nan=True)
     os.remove('rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2-created-from-cdf-input.cdf')
     os.remove('rbsp-a_magnetometer_1sec-gsm_emfisis-l3_20190122_v1.6.2.cdf')
 """
 
 
 @pytest.mark.remote_data
 def test_see_l3():
     fname = "see__L3_2021009_012_01.ncdf"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/see__L3_2021009_012_01.ncdf"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
     c = xr.load_dataset("see__L3_2021009_012_01.ncdf")
-    cdflib.xarray_to_cdf(c, "see__L3_2021009_012_01.ncdfhello2.cdf")
-    d = cdflib.cdf_to_xarray("see__L3_2021009_012_01.ncdfhello2.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(c, "see__L3_2021009_012_01.ncdfhello2.cdf")
+    d = cdf_to_xarray("see__L3_2021009_012_01.ncdfhello2.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("see__L3_2021009_012_01.ncdfhello2.cdf")
     os.remove("see__L3_2021009_012_01.ncdf")
 
 
 @pytest.mark.remote_data
 def test_see_l2a():
     fname = "see__xps_L2A_2021006_012_02.ncdf"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/see__xps_L2A_2021006_012_02.ncdf"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
     c = xr.load_dataset("see__xps_L2A_2021006_012_02.ncdf")
-    cdflib.xarray_to_cdf(c, "see__xps_L2A_2021006_012_02.ncdfhello2.cdf")
-    d = cdflib.cdf_to_xarray("see__xps_L2A_2021006_012_02.ncdfhello2.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(c, "see__xps_L2A_2021006_012_02.ncdfhello2.cdf")
+    d = cdf_to_xarray("see__xps_L2A_2021006_012_02.ncdfhello2.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("see__xps_L2A_2021006_012_02.ncdfhello2.cdf")
     os.remove("see__xps_L2A_2021006_012_02.ncdf")
 
 
 @pytest.mark.remote_data
 def test_something():
     fname = "sgpsondewnpnC1.nc"
     url = "https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/sgpsondewnpnC1.nc"
     if not os.path.exists(fname):
         urllib.request.urlretrieve(url, fname)
 
     c = xr.load_dataset("sgpsondewnpnC1.nc")
-    cdflib.xarray_to_cdf(c, "sgpsondewnpnC1-created-from-netcdf-input.cdf")
-    d = cdflib.cdf_to_xarray("sgpsondewnpnC1-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(c, "sgpsondewnpnC1-created-from-netcdf-input.cdf")
+    d = cdf_to_xarray("sgpsondewnpnC1-created-from-netcdf-input.cdf", to_unixtime=True, fillval_to_nan=True)
     os.remove("sgpsondewnpnC1-created-from-netcdf-input.cdf")
     os.remove("sgpsondewnpnC1.nc")
 
 
 def test_build_from_scratch():
     pytest.importorskip("xarray")
     var_data = [[1, 2, 3], [1, 2, 3], [1, 2, 3]]
     var_dims = ["epoch", "direction"]
     data = xr.Variable(var_dims, var_data)  # type: ignore[no-untyped-call]
     epoch_data = [1, 2, 3]
     epoch_dims = ["epoch"]
     epoch = xr.Variable(epoch_dims, epoch_data)  # type: ignore[no-untyped-call]
     ds = xr.Dataset(data_vars={"data": data, "epoch": epoch})
-    cdflib.xarray_to_cdf(ds, "hello.cdf")
+    xarray_to_cdf(ds, "hello.cdf")
     os.remove("hello.cdf")
     global_attributes = {
         "Project": "Hail Mary",
         "Source_name": "Thin Air",
         "Discipline": "None",
         "Data_type": "counts",
         "Descriptor": "Midichlorians in unicorn blood",
@@ -343,15 +336,15 @@
         "Mission_group": "Impossible",
         "Logical_source": ":)",
         "Logical_source_description": ":(",
     }
     data = xr.Variable(var_dims, var_data)  # type: ignore[no-untyped-call]
     epoch = xr.Variable(epoch_dims, epoch_data)  # type: ignore[no-untyped-call]
     ds = xr.Dataset(data_vars={"data": data, "epoch": epoch}, attrs=global_attributes)
-    cdflib.xarray_to_cdf(ds, "hello.cdf")
+    xarray_to_cdf(ds, "hello.cdf")
     os.remove("hello.cdf")
     dir_data = [1, 2, 3]
     dir_dims = ["direction"]
     direction = xr.Variable(dir_dims, dir_data)  # type: ignore[no-untyped-call]
     ds = xr.Dataset(data_vars={"data": data, "epoch": epoch, "direction": direction}, attrs=global_attributes)
-    cdflib.xarray_to_cdf(ds, "hello.cdf")
+    xarray_to_cdf(ds, "hello.cdf")
     os.remove("hello.cdf")
```

### Comparing `cdflib-1.0.0/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf` & `cdflib-1.0.1/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.0/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `cdflib-1.0.1/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

