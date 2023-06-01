# Comparing `tmp/Triumvirate-0.1.2.tar.gz` & `tmp/Triumvirate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Triumvirate-0.1.2.tar", last modified: Wed Apr 12 08:16:35 2023, max compression
+gzip compressed data, was "Triumvirate-0.2.0.tar", last modified: Thu Jun  1 12:27:56 2023, max compression
```

## Comparing `Triumvirate-0.1.2.tar` & `Triumvirate-0.2.0.tar`

### file list

```diff
@@ -1,113 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.645792 Triumvirate-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    49100 2023-04-12 08:16:35.645792 Triumvirate-0.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6169 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-12 08:16:35.645792 Triumvirate-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    22697 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.601791 Triumvirate-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.609791 Triumvirate-0.1.2/src/Triumvirate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49100 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.617792 Triumvirate-0.1.2/src/triumvirate/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_bihankel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_fftlog.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_particles.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_particles.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_threept.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_twopt.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_valid_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_winconv.py
--rw-r--r--   0 runner    (1001) docker     (123)    27588 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/dataobjs.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/dataobjs.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.621791 Triumvirate-0.1.2/src/triumvirate/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/arrayops.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/dataobjs.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/fftlog.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/field.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/io.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/maths.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/monitor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/parameters.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/particles.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/threept.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/twopt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/parameters.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    24801 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/parameters.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.625792 Triumvirate-0.1.2/src/triumvirate/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/resources/params_template.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/resources/params_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.625792 Triumvirate-0.1.2/src/triumvirate/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.629792 Triumvirate-0.1.2/src/triumvirate/src/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/arrayops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/dataobjs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/fftlog.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74090 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/field.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/io.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/maths.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/monitor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25628 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/parameters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/particles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74238 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/threept.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/twopt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/triumvirate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    60607 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/threept.py
--rw-r--r--   0 runner    (1001) docker     (123)    45237 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/twopt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.629792 Triumvirate-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.629792 Triumvirate-0.1.2/tests/test_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_build/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_dataobjs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.605791 Triumvirate-0.1.2/tests/test_input/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.633792 Triumvirate-0.1.2/tests/test_input/ctlgs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.fits
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.h5
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/test_data_catalogue.txt
--rw-r--r--   0 runner    (1001) docker     (123)  3044753 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/test_rand_catalogue.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.637792 Triumvirate-0.1.2/tests/test_input/params/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/params/test_params.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/params/test_params.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/params/tmpl_params.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.645792 Triumvirate-0.1.2/tests/test_input/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk000_bin0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk000_bin0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk000_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk000_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk202_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk202_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/pk0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/pk0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/pk2_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/pk2_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xi0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xi0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xi2_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xi2_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xiw0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xiw2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta000_bin0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta000_bin0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta000_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta000_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta202_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta202_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zetaw000_bin0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zetaw000_diag.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zetaw202_diag.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_threept.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_twopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.203981 Triumvirate-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-06-01 12:27:56.203981 Triumvirate-0.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-01 12:27:56.203981 Triumvirate-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24555 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.187980 Triumvirate-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.187980 Triumvirate-0.2.0/src/Triumvirate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.191980 Triumvirate-0.2.0/src/triumvirate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_bihankel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_fftlog.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_particles.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_particles.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_threept.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_twopt.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_valid_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_winconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28099 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/dataobjs.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/dataobjs.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.191980 Triumvirate-0.2.0/src/triumvirate/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/arrayops.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/dataobjs.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/fftlog.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/field.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/io.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/maths.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/monitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/parameters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/particles.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/threept.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/twopt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/parameters.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/parameters.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.191980 Triumvirate-0.2.0/src/triumvirate/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/resources/params_template.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/resources/params_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.195980 Triumvirate-0.2.0/src/triumvirate/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/arrayops.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/dataobjs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/fftlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74090 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/field.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/maths.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/monitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27800 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/parameters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/particles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74244 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/threept.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28450 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/twopt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    63115 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/threept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47337 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/twopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.195980 Triumvirate-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.195980 Triumvirate-0.2.0/tests/test_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_build/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_dataobjs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.187980 Triumvirate-0.2.0/tests/test_input/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.195980 Triumvirate-0.2.0/tests/test_input/ctlgs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/test_data_catalogue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3044753 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/test_rand_catalogue.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.199980 Triumvirate-0.2.0/tests/test_input/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/params/test_params.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/params/test_params.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/params/tmpl_params.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.203981 Triumvirate-0.2.0/tests/test_input/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk000_bin0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk000_bin0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk000_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk000_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk202_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk202_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/pk0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/pk0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/pk2_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/pk2_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xi0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xi0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xi2_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xi2_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xiw0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xiw2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta000_bin0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta000_bin0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta000_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta000_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta202_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta202_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zetaw000_bin0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zetaw000_diag.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zetaw202_diag.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_threept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_twopt.py
```

### Comparing `Triumvirate-0.1.2/LICENCE` & `Triumvirate-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/MANIFEST.in` & `Triumvirate-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/PKG-INFO` & `Triumvirate-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Triumvirate
-Version: 0.1.2
+Version: 0.2.0
 Summary: Three-point clustering measurements in large-scale structure analyses.
 Home-page: https://mikeswang.github.io/Triumvirate
 Author: Mike S Wang, Naonori S Sugiyama
 Maintainer: Mike S Wang
 Maintainer-email: Mike S Wang <mikeshengbo.wang@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -879,18 +879,26 @@
 ============
 
 User feedback and contributions are very welcome. Please refer to the
 `contribution guidelines
 <https://github.com/MikeSWang/Triumvirate/blob/main/CONTRIBUTING.md>`_.
 
 
+Discussions
+===========
+
+A `community forum <https://github.com/MikeSWang/Triumvirate/discussions>`_
+for users and developers is hosted on GitHub, where you can receive
+announcements, post questions, share ideas and get updates.
+
+
 Releases
 ========
 
-Changes in current and past releases are listed in the `change log
+Release notes are included in the `change log
 <https://github.com/MikeSWang/Triumvirate/blob/main/CHANGELOG.md>`_.
 
 
 Licence
 =======
 
 .. image:: https://img.shields.io/github/license/MikeSWang/Triumvirate?label=licence&style=flat-square&color=informational
```

### Comparing `Triumvirate-0.1.2/README.md` & `Triumvirate-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -123,18 +123,24 @@
 
 ## Contributing
 
 User feedback and contributions are very welcome. Please refer to the
 [contribution guidelines](CONTRIBUTING.md).
 
 
+## Discussions
+
+A [community forum](https://github.com/MikeSWang/Triumvirate/discussions)
+for users and developers exists, where you can receive
+announcements, post questions, share ideas and get updates.
+
+
 ## Releases
 
-Changes in current and past releases are listed in the
-[change log](CHANGELOG.md).
+Release notes are included in the [change log](CHANGELOG.md).
 
 
 ## Licence
 
 [![Licence](https://img.shields.io/github/license/MikeSWang/Triumvirate?label=licence&style=flat-square&color=informational)](https://github.com/MikeSWang/Triumvirate/blob/main/LICENCE)
 
 ``Triumvirate`` is made freely available under the [GPL-3.0 licence](
```

### Comparing `Triumvirate-0.1.2/README.rst` & `Triumvirate-0.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -177,18 +177,26 @@
 ============
 
 User feedback and contributions are very welcome. Please refer to the
 `contribution guidelines
 <https://github.com/MikeSWang/Triumvirate/blob/main/CONTRIBUTING.md>`_.
 
 
+Discussions
+===========
+
+A `community forum <https://github.com/MikeSWang/Triumvirate/discussions>`_
+for users and developers is hosted on GitHub, where you can receive
+announcements, post questions, share ideas and get updates.
+
+
 Releases
 ========
 
-Changes in current and past releases are listed in the `change log
+Release notes are included in the `change log
 <https://github.com/MikeSWang/Triumvirate/blob/main/CHANGELOG.md>`_.
 
 
 Licence
 =======
 
 .. image:: https://img.shields.io/github/license/MikeSWang/Triumvirate?label=licence&style=flat-square&color=informational
```

### Comparing `Triumvirate-0.1.2/pyproject.toml` & `Triumvirate-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -89,23 +89,19 @@
 ]
 before-build = [
     "export PY_BUILD_PARALLEL=-j",
 ]
 test-requires = "pytest"
 test-command = "pytest {project}/tests"
 
-# BUG: Use images that support `apt` as `yum` hangs in CentOS.
-manylinux-x86_64-image = 'manylinux_2_24'
-manylinux-aarch64-image = 'manylinux_2_24'
+manylinux-x86_64-image = 'manylinux_2_28'
+manylinux-aarch64-image = 'manylinux_2_28'
 
 [tool.cibuildwheel.linux]
 before-all = [
-    "apt-get update",
-    "apt-get install -y libgsl-dev libfftw3-dev",
+    "yum install -y gsl-devel fftw3-devel",
 ]
 
 [tool.cibuildwheel.macos]
 before-all = [
-    # Optional: Homebrew update is slow.
-    # "brew update",
     "brew install gsl fftw",
 ]
```

### Comparing `Triumvirate-0.1.2/setup.cfg` & `Triumvirate-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/setup.py` & `Triumvirate-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Set up Triumvirate and its Cythonised extension modules.
 
 """
-import logging
 import os
 import platform
 import sys
 from copy import deepcopy
+from distutils.log import _global_log as distutils_logger
 from multiprocessing import cpu_count
 from setuptools import setup
 from setuptools.command.build_clib import build_clib
 
 import numpy
 from Cython.Build import cythonize
 from Cython.Distutils import build_ext, Extension
 from extension_helpers._openmp_helpers import check_openmp_support
 from extension_helpers._setup_helpers import pkg_config
 
 
-distutils_logger = logging.getLogger()  # recycled from :mod:`distutils._log`
-
-
 # ========================================================================
 # Package
 # ========================================================================
 
 PROJECT_NAME = 'Triumvirate'
 
 
@@ -41,15 +38,16 @@
 
 def get_pkg_dir(topdir="src"):
     """Get package directory.
 
     Parameters
     ----------
     topdir : str, optional
-        Top directory.
+        Top-level (sub-)directory containing the package at the
+        repository root.
 
     Returns
     -------
     str
         Package directory.
 
     """
@@ -58,64 +56,104 @@
 
 def get_pkg_include_dir(subdir="include"):
     """Get package C++ header directory.
 
     Parameters
     ----------
     subdir : str, optional
-        Subdirectory of C++ headers in the package directory.
+        Subdirectory containing C++ headers in the package directory.
 
     Returns
     -------
     str
         C++ header directory.
 
     """
     return os.path.join(get_pkg_dir(), subdir)
 
 
-def get_pkg_src_dir(subdir="src/modules"):
+def get_pkg_src_dir(subdir="src"):
     """Get package C++ source directory.
 
     Parameters
     ----------
     subdir : str, optional
-        Subdirectory of C++ sources in the package directory.
+        Subdirectory containing C++ sources in the package directory.
 
     Returns
     -------
     str
         C++ source directory.
 
     """
     return os.path.join(get_pkg_dir(), subdir)
 
 
+def get_pkg_version_scheme(default_ver_scheme='no-guess-dev',
+                           default_loc_scheme='node-and-date'):
+    """Get package version scheme from the environment.
+
+    Parameters
+    ----------
+    default_ver_scheme : str, optional
+        Fallback default version scheme for the package
+        (default is 'no-guess-dev').
+    default_loc_scheme : str, optional
+        Fallback default local scheme for the package
+        (default is 'node-and-date').
+
+    Returns
+    -------
+    dict
+        Package version scheme(s).
+
+    See Also
+    --------
+    :pkg:`setuptools_scm`
+        For available version schemes.
+
+    """
+    ver_scheme = os.environ.get('PY_SCM_VER_SCHEME', '').strip() \
+        or default_ver_scheme
+    loc_scheme = os.environ.get('PY_SCM_LOC_SCHEME', '').strip() \
+        or default_loc_scheme
+
+    scheme = {
+        'version_scheme': ver_scheme,
+        'local_scheme': loc_scheme,
+    }
+
+    prioprint("Versioning scheme: {}".format(scheme))
+
+    return scheme
+
+
 # ========================================================================
 # Build
 # ========================================================================
 
 class BuildExt(build_ext):
     """Modified :class:`Cython.Distutils.build_ext`.
 
     """
+
     def finalize_options(self):
         """Modify parallelisation option in
-        :meth:`Cython.Distutils.build_ext.build_ext.build_extensions`.
+        :meth:`Cython.Distutils.build_ext.finalize_options`.
 
         """
         super().finalize_options()
 
         _num_procs = get_build_num_procs()
         if self.parallel is None and _num_procs is not None:
             self.parallel = _num_procs
 
     def build_extensions(self):
         """Modify compiler and compilation configuration in
-        :meth:`Cython.Distutils.build_ext.build_ext.build_extensions`.
+        :meth:`Cython.Distutils.build_ext.build_extensions`.
 
         """
         OPTS_TO_REMOVE = ['-Wstrict-prototypes',]  # noqa: E231
         for opt in OPTS_TO_REMOVE:
             try:
                 self.compiler.compiler_so.remove(opt)
             except ValueError:
@@ -134,14 +172,15 @@
         super().build_extensions()
 
 
 class BuildClib(build_clib):
     """Modified :class:`setuptools.command.build_clib.build_clib`.
 
     """
+
     def build_libraries(self, libraries):
         """Modify compiler and compilation configuration in
         :meth:`setuptools.command.build_clib.build_clib.build_libraries`.
 
         """
         OPTS_TO_REMOVE = ['-Wstrict-prototypes',]  # noqa: E231
         for opt in OPTS_TO_REMOVE:
@@ -155,15 +194,15 @@
             self.compiler.compiler_so[0],
         )
 
         super().build_libraries(libraries)
 
 
 def get_build_num_procs():
-    """Get build parallel processes.
+    """Get the number of build parallel processes.
 
     Returns
     -------
     int or None
         Number of parallel processes, which may be `None` in the case
         of no parallelisation.
 
@@ -179,33 +218,35 @@
     else:
         num_procs = None
 
     return num_procs
 
 
 def prioprint(*args, **kwargs):
-    """`print` in high priority.
+    """`print` with high priority.
 
     """
     print(*args, file=sys.stderr, **kwargs)
 
 
 def display_py_environs():
     """Display customised environment variables passed to setup.
 
     """
     PY_ENV_VARS = [
         'PY_CXX',
-        'PY_CXXFLAGS',
-        'PY_LDFLAGS',
-        'PY_INCLUDES',
+        'PY_INCLUDES',  # typically included in 'CPPFLAGS'
+        'PY_CXXFLAGS',  # untypically includes macros in 'CPPFLAGS'
+        'PY_LDFLAGS',  # untypically includes 'LDLIBS'
         'PY_NO_OMP',
         'PY_CXXFLAGS_OMP',
         'PY_LDFLAGS_OMP',
         'PY_BUILD_PARALLEL',
+        'PY_SCM_VER_SCHEME',
+        'PY_SCM_LOC_SCHEME',
     ]
     for env_var in PY_ENV_VARS:
         prioprint("{}={}".format(env_var, os.environ.get(env_var)))
 
 
 def display_py_options():
     """Display customised compilation options used in build.
@@ -226,22 +267,23 @@
 # ========================================================================
 # Compilation
 # ========================================================================
 
 EXT_LANG = 'c++'
 
 
-# -- Environment ---------------------------------------------------------
+# -- OS ------------------------------------------------------------------
 
 def get_platform():
     """Get the build platform.
 
     Returns
     -------
     {'linux', 'darwin', 'default'}
+        Build platform.
 
     """
     build_platform = platform.system().lower()
     if build_platform not in ['linux', 'darwin']:
         build_platform = 'default'
 
     return build_platform
@@ -280,52 +322,49 @@
 
     os.environ['CC'] = _compiler
     os.environ['CXX'] = _compiler
 
 
 # -- Dependencies --------------------------------------------------------
 
+PKG_LIB_NAME = 'trv'
+
+LIBS_CORE = ['gsl', 'fftw3',]  # noqa: E231
+LIBS_FULL = ['gsl', 'gslcblas', 'm', 'fftw3',]  # noqa: E231
+
 # Default to GCC OpenMP implementation.
 OPENMP_LIBS = {
-    'default': 'gomp',  # 'omp'
+    'default': 'gomp',  # or LLVM 'omp'
     'linux': '',  # set by ``-fopenmp`` or environment
     'darwin': '',  # set by ``-fopenmp`` or environment
 }
 
 
-LIBS_CORE = ['gsl', 'fftw3',]  # noqa: E231
-LIBS_FULL = ['gsl', 'gslcblas', 'm', 'fftw3',]  # noqa: E231
-
-PKG_LIB_NAME = 'trv'
-
-
 # -- Options -------------------------------------------------------------
 
 def convert_macro(macro):
     """Convert a macro flag to a tuple.
 
     Parameters
     ----------
     macro : str
-        Macro as a flag
+        Macro as a flag with '-D' prefix.
 
     Returns
     -------
-    tuple (str, Union[str, None])
-        Macro as a tuple
+    tuple[str, Union[str, None]]
+        Macro as a 2-tuple.
 
     """
     macro_ = macro.lstrip('-D').split('=')
     if len(macro_) == 1:
         return (macro_.pop(), None)
     if len(macro_) == 2:
         return tuple(macro_)
-    raise ValueError(
-        "Invalid macro to convert: {}.".format(macro_)
-    )
+    raise ValueError("Invalid macro to convert: {}.".format(macro_))
 
 
 def parse_cli_cflags():
     """Parse command-line ``PY_CXXFLAGS`` components for extension
     keyword arguments.
 
     Returns
@@ -335,65 +374,73 @@
 
     """
     cli_cflags = os.environ.get('PY_CXXFLAGS', '').split()
 
     parsed_macros, parsed_cflags = [], []
     for cflag_ in cli_cflags:
         if cflag_.startswith('-D'):
-            parsed_macros.append(convert_macro(cflag_))
+            macro_ = convert_macro(cflag_)
+            parsed_macros.append(macro_)
         else:
             parsed_cflags.append(cflag_)
 
     return parsed_macros, parsed_cflags
 
 
 def parse_cli_ldflags():
     """Parse command-line ``PY_LDFLAGS`` components for extension
     keyword arguments.
 
     Returns
     -------
     list of str, list of str, list of str
-        Parsed `ldflags`, `libs` and `libdirs`.
+        Parsed `ldflags`, `libs` and `lib_dirs`.
 
     """
     cli_ldflags = os.environ.get('PY_LDFLAGS', '').split()
 
     parsed_ldflags, parsed_libs, parsed_lib_dirs = [], [], []
     for ldflag_ in cli_ldflags:
         if ldflag_.startswith('-l'):
-            parsed_libs.append(ldflag_.lstrip('-l'))
+            lib_ = ldflag_.lstrip('-l')
+            parsed_libs.append(lib_)
         elif ldflag_.startswith('-L'):
-            parsed_lib_dirs.append(ldflag_.lstrip('-L'))
+            ldflag_L = ldflag_.lstrip('-L')
+            parsed_lib_dirs.append(ldflag_L)
         else:
             parsed_ldflags.append(ldflag_)
 
     return parsed_ldflags, parsed_libs, parsed_lib_dirs
 
 
 def parse_cli_includes():
     """Parse command-line ``PY_INCLUDES`` components for extension
     keyword arguments.
 
     Returns
     -------
     list of str
-        Parsed `ldflags`.
+        Parsed `include_dirs`.
 
     """
     parsed_include_dirs = \
         os.environ.get('PY_INCLUDES', '').replace('-I', '').split()
 
     return parsed_include_dirs
 
 
 def parse_cli_cflags_omp():
     """Parse command-line ``PY_CXXFLAGS_OMP`` components for extension
     keyword arguments.
 
+    Returns
+    -------
+    list of str, list of str
+        Parsed `macros` and `include_dirs` for OpenMP.
+
     """
     cli_cflags_omp = os.environ.get('PY_CXXFLAGS_OMP', '').split()
     if not cli_cflags_omp:
         return None
 
     parsed_macros_omp, parsed_cflags_omp = [], []
     for cflag_ in cli_cflags_omp:
@@ -413,14 +460,19 @@
     return parsed_macros_omp, parsed_cflags_omp
 
 
 def parse_cli_ldflags_omp():
     """Parse command-line ``PY_LDFLAGS_OMP`` components for extension
     keyword arguments.
 
+    Returns
+    -------
+    list of str, list of str
+        Parsed `ldflags`, `libs` and `lib_dirs` for OpenMP.
+
     """
     cli_ldflags_omp = os.environ.get('PY_LDFLAGS_OMP', '').split()
     if not cli_ldflags_omp:
         return None
 
     parsed_ldflags_omp, parsed_libs_omp, parsed_lib_dirs_omp = [], [], []
     for ldflag_ in cli_ldflags_omp:
@@ -431,112 +483,113 @@
         else:
             parsed_ldflags_omp.append(ldflag_)
 
     return parsed_ldflags_omp, parsed_libs_omp, parsed_lib_dirs_omp
 
 
 def add_options_nonomp(macros, cflags, ldflags, libs, lib_dirs, include_dirs):
-    """Add any missing non-OpenMP compilation options.
+    """Add non-OpenMP compilation options.
 
     Parameters
     ----------
-    macros : list of tuple (str, Union[str, None])
-        Macros without '-D' prefix.
+    macros : list of tuple[str, Union[str, None]]
+        Macros without the '-D' prefix.
     cflags : list of str
-        ``CXXFLAGS`` components.
+        ``CXXFLAGS`` components with non-'-D' and non-'-I' prefixes.
     ldflags : list of str
-        ``LDFLAGS`` components with non-'-l' prefixes.
+        ``LDFLAGS`` components with non-'-l' and non-'-L' prefixes.
     libs : list of str
         Libraries without the '-l' prefix.
     lib_dirs : list of str
         Library directories without the '-L' prefix.
     include_dirs : list of str
         ``INCLUDES`` directories without the '-I' prefix.
 
     Returns
     -------
-    macros : list of tuple (str, Union[str, None])
-        Macros without '-D' prefix.
+    macros : list of tuple[str, Union[str, None]]
+        Extended macros without the '-D' prefix.
     cflags : list of str
-        ``CXXFLAGS`` components.
+        Extended ``CXXFLAGS`` components with non-'-D' and
+        non-'-I' prefixes.
     ldflags : list of str
-        ``LDFLAGS`` components with non-'-l' prefixes.
+        Extended ``LDFLAGS`` components with non-'-l' and
+        non-'-L' prefixes.
     libs : list of str
-        Libraries without the '-l' prefix.
+        Extended libraries without the '-l' prefix.
     lib_dirs : list of str
-        Library directories without the '-L' prefix.
+        Extended library directories without the '-L' prefix.
     include_dirs :list of str
-        ``INCLUDES`` directories without the '-I' prefix.
+        Extended ``INCLUDES`` directories without the '-I' prefix.
 
     """
     libs_core = deepcopy(LIBS_CORE)
     libs_full = deepcopy(LIBS_FULL)
 
     for lib_ in libs:
         if lib_ not in libs_full:
             libs_core.append(lib_)
             libs_full.append(lib_)
 
     checked_options = pkg_config(libs_core, default_libraries=libs_full)
 
+    libs = checked_options['libraries']
+
     for macro_ in checked_options['define_macros']:
         if macro_ not in macros:
             macros.append(macro_)
-    for macro_ in checked_options['undef_macros']:
-        if macro_ not in macros:
-            macros.append(macro_)
     for flag in checked_options['extra_compile_args']:
         if flag not in cflags + ldflags:
             cflags.append(flag)
-    for include_dir_ in checked_options['include_dirs']:
-        if include_dir_ not in include_dirs:
-            include_dirs.append(include_dir_)
     for lib_dir_ in checked_options['library_dirs']:
         if lib_dir_ not in lib_dirs:
             lib_dirs.append(lib_dir_)
-
-    libs = checked_options['libraries']
+    for include_dir_ in checked_options['include_dirs']:
+        if include_dir_ not in include_dirs:
+            include_dirs.append(include_dir_)
 
     return macros, cflags, ldflags, libs, lib_dirs, include_dirs
 
 
 def add_options_omp(macros, cflags, ldflags, libs, lib_dirs, include_dirs):
     """Add OpenMP options, if enabled.
 
     By default, GCC OpenMP is assumed.
 
     Parameters
     ----------
-    macros : list of tuple (str, Union[str, None])
-        Macros without '-D' prefix.
+    macros : list of tuple[str, Union[str, None]]
+        Macros without the '-D' prefix.
     cflags : list of str
-        ``CXXFLAGS`` components.
+        ``CXXFLAGS`` components with non-'-D' and non-'-I' prefixes.
     ldflags : list of str
-        ``LDFLAGS`` components with non-'-l' prefixes.
+        ``LDFLAGS`` components with non-'-l' and non-'-L' prefixes.
     libs : list of str
         Libraries without the '-l' prefix.
     lib_dirs : list of str
         Library directories without the '-L' prefix.
     include_dirs :list of str
         ``INCLUDES`` directories without the '-I' prefix.
 
     Returns
     -------
-    macros : list of tuple (str, Union[str, None])
-        Processed macros without '-D' prefix.
+    macros : list of tuple[str, Union[str, None]]
+        Extended macros without the '-D' prefix.
     cflags : list of str
-        Processed ``CXXFLAGS`` components.
+        Extended ``CXXFLAGS`` components with non-'-D' and
+        non-'-I' prefixes.
     ldflags : list of str
-        Processed ``LDFLAGS`` components non-'-l' prefix.
+        Extended ``LDFLAGS`` components with non-'-l' and
+        non-'-L' prefixes.
     libs : list of str
-        Libraries without the '-l' prefix.
+        Extended libraries without the '-l' prefix.
     lib_dirs : list of str
-        Library directories without the '-L' prefix.
+        Extended library directories without the '-L' prefix.
     include_dirs :list of str
-        ``INCLUDES`` directories without the '-I' prefix.
+        Extended ``INCLUDES`` directories without the '-I' prefix.
 
     """
     # Check if OpenMP is explicitly disabled.
     if os.environ.get('PY_NO_OMP') is not None:
         prioprint("OpenMP is disabled explicitly.")
         return macros, cflags, ldflags, libs, lib_dirs, include_dirs
 
@@ -547,15 +600,15 @@
             "it is not supported in this build enviromnent."
         )
         return macros, cflags, ldflags, libs, lib_dirs, include_dirs
 
     # Enable OpenMP by default otherwise.
     prioprint("OpenMP is enabled by default.")
 
-    # Adapt macros and `cflags`.
+    # Adapt `macros` and `cflags`.
     MACROS_OMP_RELATED = [
         ('TRV_USE_OMP', None),
         ('TRV_USE_FFTWOMP', None),
     ]
     for macro_ in MACROS_OMP_RELATED:
         if macro_ not in macros:
             macros.append(macro_)
@@ -603,41 +656,43 @@
 
 
 def add_options_pkgs(macros, cflags, ldflags, libs, lib_dirs, include_dirs):
     """Add options required by this package and external packages.
 
     Parameters
     ----------
-    macros : list of tuple (str, Union[str, None])
-        Macros without '-D' prefix.
+    macros : list of tuple[str, Union[str, None]]
+        Macros without the '-D' prefix.
     cflags : list of str
-        ``CXXFLAGS`` components.
+        ``CXXFLAGS`` components with non-'-D' and non-'-I' prefixes.
     ldflags : list of str
-        ``LDFLAGS`` components with non-'-l' prefixes.
+        ``LDFLAGS`` components with non-'-l' and non-'-L' prefixes.
     libs : list of str
         Libraries without the '-l' prefix.
     lib_dirs : list of str
         Library directories without the '-L' prefix.
     include_dirs : list of str
         ``INCLUDES`` directories without the '-I' prefix.
 
     Returns
     -------
-    macros : list of tuple (str, Union[str, None])
-        Processed macros without '-D' prefix.
+    macros : list of tuple[str, Union[str, None]]
+        Extended macros without the '-D' prefix.
     cflags : list of str
-        Processed ``CXXFLAGS`` components.
+        Extended ``CXXFLAGS`` components with non-'-D' and
+        non-'-I' prefixes.
     ldflags : list of str
-        Processed ``LDFLAGS`` components non-'-l' prefix.
+        Extended ``LDFLAGS`` components with non-'-l' and
+        non-'-L' prefixes.
     libs : list of str
-        Libraries without the '-l' prefix.
+        Extended libraries without the '-l' prefix.
     lib_dirs : list of str
-        Library directories without the '-L' prefix.
+        Extended library directories without the '-L' prefix.
     include_dirs : list of str
-        ``INCLUDES`` directories without the '-I' prefix.
+        Extended ``INCLUDES`` directories without the '-I' prefix.
 
     """
     # Adapt `macros`.
     MACROS_PKG = [
         ('TRV_EXTCALL', None),
         # ('TRV_USE_LEGACY_CODE', None),
         # ('DBG_MODE', None),
@@ -694,15 +749,15 @@
     Parameters
     ----------
     lib_name : str
         Package libaray name.
 
     Returns
     -------
-    tuple (str, dict)
+    tuple[str, dict]
         Package library and corresponding configurations.
 
     """
     pkg_src_dir = get_pkg_src_dir()
 
     pkg_sources = [
         os.path.join(pkg_src_dir, _cpp_source)
@@ -828,19 +883,18 @@
     # Run build commands.
     cython_ext_modules = cythonize(
         pkg_extensions,
         compiler_directives=CYTHON_DIRECTIVES,
         nthreads=get_build_num_procs(),
     )
 
+    setup_commands = {
+        'build_clib': BuildClib,
+        'build_ext': BuildExt,
+    }
+
     setup(
-        use_scm_version={
-            'version_scheme': 'post-release',
-            # 'local_scheme': 'no-local-version',
-        },
-        cmdclass={
-            'build_clib': BuildClib,
-            'build_ext': BuildExt,
-        },
+        use_scm_version=get_pkg_version_scheme(),
+        cmdclass=setup_commands,
         ext_modules=cython_ext_modules,
         libraries=pkg_libraries,
     )
```

### Comparing `Triumvirate-0.1.2/src/Triumvirate.egg-info/PKG-INFO` & `Triumvirate-0.2.0/src/Triumvirate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Triumvirate
-Version: 0.1.2
+Version: 0.2.0
 Summary: Three-point clustering measurements in large-scale structure analyses.
 Home-page: https://mikeswang.github.io/Triumvirate
 Author: Mike S Wang, Naonori S Sugiyama
 Maintainer: Mike S Wang
 Maintainer-email: Mike S Wang <mikeshengbo.wang@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -879,18 +879,26 @@
 ============
 
 User feedback and contributions are very welcome. Please refer to the
 `contribution guidelines
 <https://github.com/MikeSWang/Triumvirate/blob/main/CONTRIBUTING.md>`_.
 
 
+Discussions
+===========
+
+A `community forum <https://github.com/MikeSWang/Triumvirate/discussions>`_
+for users and developers is hosted on GitHub, where you can receive
+announcements, post questions, share ideas and get updates.
+
+
 Releases
 ========
 
-Changes in current and past releases are listed in the `change log
+Release notes are included in the `change log
 <https://github.com/MikeSWang/Triumvirate/blob/main/CHANGELOG.md>`_.
 
 
 Licence
 =======
 
 .. image:: https://img.shields.io/github/license/MikeSWang/Triumvirate?label=licence&style=flat-square&color=informational
```

### Comparing `Triumvirate-0.1.2/src/Triumvirate.egg-info/SOURCES.txt` & `Triumvirate-0.2.0/src/Triumvirate.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,26 +38,25 @@
 src/triumvirate/include/monitor.hpp
 src/triumvirate/include/parameters.hpp
 src/triumvirate/include/particles.hpp
 src/triumvirate/include/threept.hpp
 src/triumvirate/include/twopt.hpp
 src/triumvirate/resources/params_template.ini
 src/triumvirate/resources/params_template.yml
-src/triumvirate/src/triumvirate.cpp
-src/triumvirate/src/modules/arrayops.cpp
-src/triumvirate/src/modules/dataobjs.cpp
-src/triumvirate/src/modules/fftlog.cpp
-src/triumvirate/src/modules/field.cpp
-src/triumvirate/src/modules/io.cpp
-src/triumvirate/src/modules/maths.cpp
-src/triumvirate/src/modules/monitor.cpp
-src/triumvirate/src/modules/parameters.cpp
-src/triumvirate/src/modules/particles.cpp
-src/triumvirate/src/modules/threept.cpp
-src/triumvirate/src/modules/twopt.cpp
+src/triumvirate/src/arrayops.cpp
+src/triumvirate/src/dataobjs.cpp
+src/triumvirate/src/fftlog.cpp
+src/triumvirate/src/field.cpp
+src/triumvirate/src/io.cpp
+src/triumvirate/src/maths.cpp
+src/triumvirate/src/monitor.cpp
+src/triumvirate/src/parameters.cpp
+src/triumvirate/src/particles.cpp
+src/triumvirate/src/threept.cpp
+src/triumvirate/src/twopt.cpp
 tests/conftest.py
 tests/test_catalogue.py
 tests/test_dataobjs.py
 tests/test_logger.py
 tests/test_parameters.py
 tests/test_threept.py
 tests/test_twopt.py
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/__init__.py` & `Triumvirate-0.2.0/src/triumvirate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     with this program.  If not, see `<https://www.gnu.org/licenses/>`_.
 
 """
 from importlib.metadata import PackageNotFoundError, version
 
 
 __copyright__ = 'Copyright 2023, Mike S Wang & Naonori S Sugiyama'
-__date__ = '2023-03-27'
+__date__ = '2023-05-31'
 __license__ = 'GPL-3.0'
 
 try:
     __version__ = version('triumvirate')
 except PackageNotFoundError:
-    __version__ = '0.1'  # fallback version number
+    __version__ = '0.2.0'  # fallback version number
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/_bihankel.py` & `Triumvirate-0.2.0/src/triumvirate/_bihankel.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/_fftlog.pyx` & `Triumvirate-0.2.0/src/triumvirate/_fftlog.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/_particles.pxd` & `Triumvirate-0.2.0/src/triumvirate/_particles.pxd`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/_particles.pyx` & `Triumvirate-0.2.0/src/triumvirate/_particles.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/_threept.pyx` & `Triumvirate-0.2.0/src/triumvirate/_threept.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -22,113 +22,113 @@
 
 
 cdef extern from "include/threept.hpp":
     # --------------------------------------------------------------------
     # Normalisation
     # --------------------------------------------------------------------
 
+    double calc_bispec_normalisation_from_particles_cpp \
+        "trv::calc_bispec_normalisation_from_particles" (
+            CppParticleCatalogue& particles,
+            double alpha
+        ) except +
+
     double calc_bispec_normalisation_from_mesh_cpp \
         "trv::calc_bispec_normalisation_from_mesh" (
-            CppParticleCatalogue& catalogue,
+            CppParticleCatalogue& particles,
             CppParameterSet& params,
             double alpha
         )
 
-    double calc_bispec_normalisation_from_particles_cpp \
-        "trv::calc_bispec_normalisation_from_particles" (
-            CppParticleCatalogue& catalogue,
-            double alpha
-        ) except +
-
 
     # --------------------------------------------------------------------
     # Full correlator
     # --------------------------------------------------------------------
 
     BispecMeasurements compute_bispec_cpp "trv::compute_bispec" (
-        CppParticleCatalogue& particles_data,
-        CppParticleCatalogue& particles_rand,
+        CppParticleCatalogue& catalogue_data,
+        CppParticleCatalogue& catalogue_rand,
         LineOfSight* los_data,
         LineOfSight* los_rand,
         CppParameterSet& params,
         CppBinning& kbinning,
         double norm_factor
     )
 
     ThreePCFMeasurements compute_3pcf_cpp "trv::compute_3pcf" (
-        CppParticleCatalogue& particles_data,
-        CppParticleCatalogue& particles_rand,
+        CppParticleCatalogue& catalogue_data,
+        CppParticleCatalogue& catalogue_rand,
         LineOfSight* los_data,
         LineOfSight* los_rand,
         CppParameterSet& params,
         CppBinning& rbinning,
         double norm_factor
     )
 
     BispecMeasurements compute_bispec_in_gpp_box_cpp \
         "trv::compute_bispec_in_gpp_box" (
-            CppParticleCatalogue& particles_data,
+            CppParticleCatalogue& catalogue_data,
             CppParameterSet& params,
             CppBinning& kbinning,
             double norm_factor
         )
 
     ThreePCFMeasurements compute_3pcf_in_gpp_box_cpp \
         "trv::compute_3pcf_in_gpp_box" (
-            CppParticleCatalogue& particles_data,
+            CppParticleCatalogue& catalogue_data,
             CppParameterSet& params,
             CppBinning& rbinning,
             double norm_factor
         )
 
     ThreePCFWindowMeasurements compute_3pcf_window_cpp \
         "trv::compute_3pcf_window" (
-            CppParticleCatalogue& particles_rand,
+            CppParticleCatalogue& catalogue_rand,
             LineOfSight* los_rand,
             CppParameterSet& params,
             CppBinning& rbinning,
             double alpha,
             double norm_factor,
             bool_t wide_angle
         )
 
     # BispecMeasurements compute_bispec_for_los_choice_cpp \
     #     "trv::compute_bispec_for_los_choice" (
-    #         CppParticleCatalogue& particles_data,
-    #         CppParticleCatalogue& particles_rand,
+    #         CppParticleCatalogue& catalogue_data,
+    #         CppParticleCatalogue& catalogue_rand,
     #         LineOfSight* los_data,
     #         LineOfSight* los_rand,
     #         int los_choice,
     #         CppParameterSet& params,
     #         CppBinning& kbinning,
     #         double norm_factor
     #     )
 
 
-def _calc_bispec_normalisation_from_mesh(
-        _ParticleCatalogue catalogue not None,
-        ParameterSet params not None,
-        double alpha
+def _calc_bispec_normalisation_from_particles(
+        _ParticleCatalogue particles not None, double alpha
     ):
-    return calc_bispec_normalisation_from_mesh_cpp(
-        deref(catalogue.thisptr), deref(params.thisptr), alpha
+    return calc_bispec_normalisation_from_particles_cpp(
+        deref(particles.thisptr), alpha
     )
 
 
-def _calc_bispec_normalisation_from_particles(
-        _ParticleCatalogue catalogue not None, double alpha
+def _calc_bispec_normalisation_from_mesh(
+        _ParticleCatalogue particles not None,
+        ParameterSet params not None,
+        double alpha
     ):
-    return calc_bispec_normalisation_from_particles_cpp(
-        deref(catalogue.thisptr), alpha
+    return calc_bispec_normalisation_from_mesh_cpp(
+        deref(particles.thisptr), deref(params.thisptr), alpha
     )
 
 
 def _compute_bispec(
-        _ParticleCatalogue particles_data not None,
-        _ParticleCatalogue particles_rand not None,
+        _ParticleCatalogue catalogue_data not None,
+        _ParticleCatalogue catalogue_rand not None,
         np.ndarray[double, ndim=2, mode='c'] los_data not None,
         np.ndarray[double, ndim=2, mode='c'] los_rand not None,
         ParameterSet params not None,
         Binning kbinning not None,
         double norm_factor
     ):
     # Parse lines of sight per particle.
@@ -147,15 +147,15 @@
         los_rand_cpp[pid].pos[0] = los_x
         los_rand_cpp[pid].pos[1] = los_y
         los_rand_cpp[pid].pos[2] = los_z
 
     # Run algorithm.
     cdef BispecMeasurements results
     results = compute_bispec_cpp(
-        deref(particles_data.thisptr), deref(particles_rand.thisptr),
+        deref(catalogue_data.thisptr), deref(catalogue_rand.thisptr),
         los_data_cpp, los_rand_cpp,
         deref(params.thisptr), deref(kbinning.thisptr),
         norm_factor
     )
 
     free(los_data_cpp); free(los_rand_cpp)
 
@@ -167,16 +167,16 @@
         'nmodes': np.array(results.nmodes),
         'bk_raw': np.array(results.bk_raw),
         'bk_shot': np.array(results.bk_shot),
     }
 
 
 def _compute_3pcf(
-        _ParticleCatalogue particles_data not None,
-        _ParticleCatalogue particles_rand not None,
+        _ParticleCatalogue catalogue_data not None,
+        _ParticleCatalogue catalogue_rand not None,
         np.ndarray[double, ndim=2, mode='c'] los_data not None,
         np.ndarray[double, ndim=2, mode='c'] los_rand not None,
         ParameterSet params not None,
         Binning rbinning not None,
         double norm_factor
     ):
     # Parse lines of sight per particle.
@@ -195,15 +195,15 @@
         los_rand_cpp[pid].pos[0] = los_x
         los_rand_cpp[pid].pos[1] = los_y
         los_rand_cpp[pid].pos[2] = los_z
 
     # Run algorithm.
     cdef ThreePCFMeasurements results
     results = compute_3pcf_cpp(
-        deref(particles_data.thisptr), deref(particles_rand.thisptr),
+        deref(catalogue_data.thisptr), deref(catalogue_rand.thisptr),
         los_data_cpp, los_rand_cpp,
         deref(params.thisptr), deref(rbinning.thisptr),
         norm_factor
     )
 
     free(los_data_cpp); free(los_rand_cpp)
 
@@ -215,22 +215,22 @@
         'npairs': np.array(results.npairs),
         'zeta_raw': np.array(results.zeta_raw),
         'zeta_shot': np.array(results.zeta_shot),
     }
 
 
 def _compute_bispec_in_gpp_box(
-        _ParticleCatalogue particles_data not None,
+        _ParticleCatalogue catalogue_data not None,
         ParameterSet params not None,
         Binning kbinning not None,
         double norm_factor
     ):
     cdef BispecMeasurements results
     results = compute_bispec_in_gpp_box_cpp(
-        deref(particles_data.thisptr),
+        deref(catalogue_data.thisptr),
         deref(params.thisptr), deref(kbinning.thisptr),
         norm_factor
     )
 
     return {
         'k1_bin': np.array(results.k1_bin),
         'k2_bin': np.array(results.k2_bin),
@@ -239,22 +239,22 @@
         'nmodes': np.array(results.nmodes),
         'bk_raw': np.array(results.bk_raw),
         'bk_shot': np.array(results.bk_shot),
     }
 
 
 def _compute_3pcf_in_gpp_box(
-        _ParticleCatalogue particles_data not None,
+        _ParticleCatalogue catalogue_data not None,
         ParameterSet params not None,
         Binning rbinning not None,
         double norm_factor
     ):
     cdef ThreePCFMeasurements results
     results = compute_3pcf_in_gpp_box_cpp(
-        deref(particles_data.thisptr),
+        deref(catalogue_data.thisptr),
         deref(params.thisptr), deref(rbinning.thisptr),
         norm_factor
     )
 
     return {
         'r1_bin': np.array(results.r1_bin),
         'r2_bin': np.array(results.r2_bin),
@@ -263,15 +263,15 @@
         'npairs': np.array(results.npairs),
         'zeta_raw': np.array(results.zeta_raw),
         'zeta_shot': np.array(results.zeta_shot),
     }
 
 
 def _compute_3pcf_window(
-        _ParticleCatalogue particles_rand not None,
+        _ParticleCatalogue catalogue_rand not None,
         np.ndarray[double, ndim=2, mode='c'] los_rand not None,
         ParameterSet params not None,
         Binning rbinning not None,
         double alpha,
         double norm_factor,
         bool_t wide_angle
     ):
@@ -283,15 +283,15 @@
         los_rand_cpp[pid].pos[0] = los_x
         los_rand_cpp[pid].pos[1] = los_y
         los_rand_cpp[pid].pos[2] = los_z
 
     # Run algorithm.
     cdef ThreePCFWindowMeasurements results
     results = compute_3pcf_window_cpp(
-        deref(particles_rand.thisptr), los_rand_cpp,
+        deref(catalogue_rand.thisptr), los_rand_cpp,
         deref(params.thisptr), deref(rbinning.thisptr),
         alpha, norm_factor,
         wide_angle
     )
 
     free(los_rand_cpp)
 
@@ -303,16 +303,16 @@
         'npairs': np.array(results.npairs),
         'zeta_raw': np.array(results.zeta_raw),
         'zeta_shot': np.array(results.zeta_shot),
     }
 
 
 # def _compute_bispec_for_los_choice(
-#         _ParticleCatalogue particles_data not None,
-#         _ParticleCatalogue particles_rand not None,
+#         _ParticleCatalogue catalogue_data not None,
+#         _ParticleCatalogue catalogue_rand not None,
 #         np.ndarray[double, ndim=2, mode='c'] los_data not None,
 #         np.ndarray[double, ndim=2, mode='c'] los_rand not None,
 #         int los_choice,
 #         ParameterSet params not None,
 #         Binning kbinning not None,
 #         double norm_factor
 #     ):
@@ -332,15 +332,15 @@
 #         los_rand_cpp[pid].pos[0] = los_x
 #         los_rand_cpp[pid].pos[1] = los_y
 #         los_rand_cpp[pid].pos[2] = los_z
 
 #     # Run algorithm.
 #     cdef BispecMeasurements results
 #     results = compute_bispec_for_los_choice_cpp(
-#         deref(particles_data.thisptr), deref(particles_rand.thisptr),
+#         deref(catalogue_data.thisptr), deref(catalogue_rand.thisptr),
 #         los_data_cpp, los_rand_cpp, los_choice,
 #         deref(params.thisptr), deref(kbinning.thisptr),
 #         norm_factor
 #     )
 
 #     free(los_data_cpp); free(los_rand_cpp)
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/_twopt.pyx` & `Triumvirate-0.2.0/src/triumvirate/_twopt.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ==========================================================================
 
 Declare and interface with two-point correlator algorithms.
 
 """
 from cython.operator cimport dereference as deref
 from libc.stdlib cimport free, malloc
+from libcpp.string cimport string
 
 import numpy as np
 cimport numpy as np
 
 from triumvirate._particles cimport CppParticleCatalogue, _ParticleCatalogue
 from triumvirate.dataobjs cimport (
     Binning, CppBinning,
@@ -21,100 +22,149 @@
 
 
 cdef extern from "include/twopt.hpp":
     # --------------------------------------------------------------------
     # Normalisation
     # --------------------------------------------------------------------
 
+    double calc_powspec_normalisation_from_particles_cpp \
+        "trv::calc_powspec_normalisation_from_particles" (
+            CppParticleCatalogue& particles,
+            double alpha
+        ) except +
+
     double calc_powspec_normalisation_from_mesh_cpp \
         "trv::calc_powspec_normalisation_from_mesh" (
-            CppParticleCatalogue& catalogue,
+            CppParticleCatalogue& particles,
             CppParameterSet& params,
             double alpha
         )
 
-    double calc_powspec_normalisation_from_particles_cpp \
-        "trv::calc_powspec_normalisation_from_particles" (
-            CppParticleCatalogue& catalogue,
+    double calc_powspec_normalisation_from_meshes_cpp \
+        "trv::calc_powspec_normalisation_from_meshes" (
+            CppParticleCatalogue& particles_data,
+            CppParticleCatalogue& particles_rand,
+            CppParameterSet& params,
             double alpha
-        ) except +
+        )
+
+    double calc_powspec_normalisation_from_meshes_cpp \
+        "trv::calc_powspec_normalisation_from_meshes" (
+            CppParticleCatalogue& particles_data,
+            CppParticleCatalogue& particles_rand,
+            CppParameterSet& params,
+            double alpha,
+            double padding,
+            double cellsize,
+            string assignment
+        )
 
 
     # --------------------------------------------------------------------
     # Full correlator
     # --------------------------------------------------------------------
 
     PowspecMeasurements compute_powspec_cpp "trv::compute_powspec" (
-        CppParticleCatalogue& particles_data,
-        CppParticleCatalogue& particles_rand,
+        CppParticleCatalogue& catalogue_data,
+        CppParticleCatalogue& catalogue_rand,
         LineOfSight* los_data,
         LineOfSight* los_rand,
         CppParameterSet& params,
         CppBinning& kbinning,
         double norm_factor
     )
 
     TwoPCFMeasurements compute_corrfunc_cpp "trv::compute_corrfunc" (
-        CppParticleCatalogue& particles_data,
-        CppParticleCatalogue& particles_rand,
+        CppParticleCatalogue& catalogue_data,
+        CppParticleCatalogue& catalogue_rand,
         LineOfSight* los_data,
         LineOfSight* los_rand,
         CppParameterSet& params,
         CppBinning& rbinning,
         double norm_factor
     )
 
     PowspecMeasurements compute_powspec_in_gpp_box_cpp \
         "trv::compute_powspec_in_gpp_box" (
-            CppParticleCatalogue& particles_data,
+            CppParticleCatalogue& catalogue_data,
             CppParameterSet& params,
             CppBinning& kbinning,
             double norm_factor
         )
 
     TwoPCFMeasurements compute_corrfunc_in_gpp_box_cpp \
         "trv::compute_corrfunc_in_gpp_box" (
-            CppParticleCatalogue& particles_data,
+            CppParticleCatalogue& catalogue_data,
             CppParameterSet& params,
             CppBinning& rbinning,
             double norm_factor
         )
 
     TwoPCFWindowMeasurements compute_corrfunc_window_cpp \
         "trv::compute_corrfunc_window" (
-            CppParticleCatalogue& particles_rand,
+            CppParticleCatalogue& catalogue_rand,
             LineOfSight* los_rand,
             CppParameterSet& params,
             CppBinning& rbinning,
             double alpha,
             double norm_factor
         )
 
 
+def _calc_powspec_normalisation_from_particles(
+        _ParticleCatalogue particles not None, double alpha
+    ):
+    return calc_powspec_normalisation_from_particles_cpp(
+        deref(particles.thisptr), alpha
+    )
+
+
 def _calc_powspec_normalisation_from_mesh(
-        _ParticleCatalogue catalogue not None,
+        _ParticleCatalogue particles not None,
         ParameterSet params not None,
         double alpha
     ):
     return calc_powspec_normalisation_from_mesh_cpp(
-        deref(catalogue.thisptr), deref(params.thisptr), alpha
+        deref(particles.thisptr), deref(params.thisptr), alpha
     )
 
 
-def _calc_powspec_normalisation_from_particles(
-        _ParticleCatalogue catalogue not None, double alpha
+def _calc_powspec_normalisation_from_meshes(
+        _ParticleCatalogue particles_data not None,
+        _ParticleCatalogue particles_rand not None,
+        ParameterSet params not None,
+        double alpha,
+        padding=None, cellsize=None, assignment=None
     ):
-    return calc_powspec_normalisation_from_particles_cpp(
-        deref(catalogue.thisptr), alpha
-    )
+    if None in [padding, cellsize, assignment]:
+        return calc_powspec_normalisation_from_meshes_cpp(
+            deref(particles_data.thisptr), deref(particles_rand.thisptr),
+            deref(params.thisptr), alpha
+        )
+    else:  # STYLE: non-Pythonic use of `else`
+        if not (
+            isinstance(padding, float)
+            and isinstance(cellsize, float)
+            and isinstance(assignment, str)
+        ):
+            raise TypeError(
+                "`padding`, `cellsize` and `assignment` must be "
+                "of type float, float and str: received {}, {} and {}."
+                .format(type(padding), type(cellsize), type(assignment))
+            )
+        return calc_powspec_normalisation_from_meshes_cpp(
+            deref(particles_data.thisptr), deref(particles_rand.thisptr),
+            deref(params.thisptr), alpha,
+            padding, cellsize, assignment.encode('utf-8')
+        )
 
 
 def _compute_powspec(
-        _ParticleCatalogue particles_data not None,
-        _ParticleCatalogue particles_rand not None,
+        _ParticleCatalogue catalogue_data not None,
+        _ParticleCatalogue catalogue_rand not None,
         np.ndarray[double, ndim=2, mode='c'] los_data not None,
         np.ndarray[double, ndim=2, mode='c'] los_rand not None,
         ParameterSet params not None,
         Binning kbinning not None,
         double norm_factor
     ):
     # Parse lines of sight per particle.
@@ -133,15 +183,15 @@
         los_rand_cpp[pid].pos[0] = los_x
         los_rand_cpp[pid].pos[1] = los_y
         los_rand_cpp[pid].pos[2] = los_z
 
     # Run algorithm.
     cdef PowspecMeasurements results
     results = compute_powspec_cpp(
-        deref(particles_data.thisptr), deref(particles_rand.thisptr),
+        deref(catalogue_data.thisptr), deref(catalogue_rand.thisptr),
         los_data_cpp, los_rand_cpp,
         deref(params.thisptr), deref(kbinning.thisptr),
         norm_factor
     )
 
     free(los_data_cpp); free(los_rand_cpp)
 
@@ -151,16 +201,16 @@
         'nmodes': np.array(results.nmodes),
         'pk_raw': np.array(results.pk_raw),
         'pk_shot': np.array(results.pk_shot),
     }
 
 
 def _compute_corrfunc(
-        _ParticleCatalogue particles_data not None,
-        _ParticleCatalogue particles_rand not None,
+        _ParticleCatalogue catalogue_data not None,
+        _ParticleCatalogue catalogue_rand not None,
         np.ndarray[double, ndim=2, mode='c'] los_data not None,
         np.ndarray[double, ndim=2, mode='c'] los_rand not None,
         ParameterSet params not None,
         Binning rbinning not None,
         double norm_factor
     ):
     # Parse lines of sight per particle.
@@ -179,15 +229,15 @@
         los_rand_cpp[pid].pos[0] = los_x
         los_rand_cpp[pid].pos[1] = los_y
         los_rand_cpp[pid].pos[2] = los_z
 
     # Run algorithm.
     cdef TwoPCFMeasurements results
     results = compute_corrfunc_cpp(
-        deref(particles_data.thisptr), deref(particles_rand.thisptr),
+        deref(catalogue_data.thisptr), deref(catalogue_rand.thisptr),
         los_data_cpp, los_rand_cpp,
         deref(params.thisptr), deref(rbinning.thisptr),
         norm_factor
     )
 
     free(los_data_cpp); free(los_rand_cpp)
 
@@ -196,58 +246,58 @@
         'reff': np.array(results.reff),
         'npairs': np.array(results.npairs),
         'xi': np.array(results.xi),
     }
 
 
 def _compute_powspec_in_gpp_box(
-        _ParticleCatalogue particles_data not None,
+        _ParticleCatalogue catalogue_data not None,
         ParameterSet params not None,
         Binning kbinning not None,
         double norm_factor
     ):
     cdef PowspecMeasurements results
     results = compute_powspec_in_gpp_box_cpp(
-        deref(particles_data.thisptr),
+        deref(catalogue_data.thisptr),
         deref(params.thisptr), deref(kbinning.thisptr),
         norm_factor
     )
 
     return {
         'kbin': np.array(results.kbin),
         'keff': np.array(results.keff),
         'nmodes': np.array(results.nmodes),
         'pk_raw': np.array(results.pk_raw),
         'pk_shot': np.array(results.pk_shot),
     }
 
 
 def _compute_corrfunc_in_gpp_box(
-        _ParticleCatalogue particles_data not None,
+        _ParticleCatalogue catalogue_data not None,
         ParameterSet params not None,
         Binning rbinning not None,
         double norm_factor
     ):
     cdef TwoPCFMeasurements results
     results = compute_corrfunc_in_gpp_box_cpp(
-        deref(particles_data.thisptr),
+        deref(catalogue_data.thisptr),
         deref(params.thisptr), deref(rbinning.thisptr),
         norm_factor
     )
 
     return {
         'rbin': np.array(results.rbin),
         'reff': np.array(results.reff),
         'npairs': np.array(results.npairs),
         'xi': np.array(results.xi),
     }
 
 
 def _compute_corrfunc_window(
-        _ParticleCatalogue particles_rand not None,
+        _ParticleCatalogue catalogue_rand not None,
         np.ndarray[double, ndim=2, mode='c'] los_rand not None,
         ParameterSet params not None,
         Binning rbinning not None,
         double alpha,
         double norm_factor
     ):
     # Parse lines of sight per particle.
@@ -258,15 +308,15 @@
         los_rand_cpp[pid].pos[0] = los_x
         los_rand_cpp[pid].pos[1] = los_y
         los_rand_cpp[pid].pos[2] = los_z
 
     # Run algorithm.
     cdef TwoPCFWindowMeasurements results
     results = compute_corrfunc_window_cpp(
-        deref(particles_rand.thisptr), los_rand_cpp,
+        deref(catalogue_rand.thisptr), los_rand_cpp,
         deref(params.thisptr), deref(rbinning.thisptr),
         alpha, norm_factor
     )
 
     free(los_rand_cpp)
 
     return {
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/_valid_install.py` & `Triumvirate-0.2.0/src/triumvirate/_valid_install.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/_winconv.py` & `Triumvirate-0.2.0/src/triumvirate/_winconv.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/catalogue.py` & `Triumvirate-0.2.0/src/triumvirate/catalogue.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,22 +69,25 @@
     Attributes
     ----------
     bounds : dict of {str: tuple of (float, float)}
         Particle coordinate bounds.
     ntotal : int
         Total particle number.
     wtotal : float
-        Total sample weight.
+        Total particle overall weight.
+    wstotal : float
+        Total particle sample weight.
 
 
     .. attention::
 
         There are two types of weights: sample weights ``ws``
         (e.g. completeness weights) and clustering weights ``wc``
-        (e.g. Feldman--Kaiser--Peacock weights).
+        (e.g. Feldman--Kaiser--Peacock weights). The overall weight
+        is the product of the two for each particle.
 
         Note the naming convention above: in particular, ``wc`` is not
         the completeness weight (which is a component of ``ws`` instead).
 
     """
 
     def __init__(self, x, y, z, nz=None, ws=1., wc=1., logger=None):
@@ -116,21 +119,24 @@
 
         self._source = 'extdata:{}'.format(id(self._pdata))
 
         # Compute catalogue properties.
         self._calc_bounds(init=True)
 
         self.ntotal = len(self)
-        self.wtotal = self._compute(self._pdata['ws'].sum())
+        self.wtotal = self._compute(
+            (self._pdata['ws'] * self._pdata['wc']).sum()
+        )
+        self.wstotal = self._compute(self._pdata['ws'].sum())
 
         if self._logger:
             self._logger.info(
-                "Catalogue initialised: %d particles with "
-                "total sample weight %.3f (%s).",
-                self.ntotal, self.wtotal, self
+                "Catalogue initialised: "
+                "ntotal = %d, wtotal = %.3f, wstotal = %.3f (%s).",
+                self.ntotal, self.wtotal, self.wstotal, self
             )
 
     @classmethod
     def read_from_file(cls, filepath, reader='astropy', names=None,
                        format='ascii.no_header', table_kwargs=None,
                        file_kwargs=None, name_mapping=None, logger=None):
         """Read particle data from file.
@@ -344,21 +350,24 @@
                 )
                 self._pdata[name_wgt] = 1.
 
         # Compute catalogue properties.
         self._calc_bounds(init=True)
 
         self.ntotal = len(self._pdata)
-        self.wtotal = self._compute(self._pdata['ws'].sum())
+        self.wtotal = self._compute(
+            (self._pdata['ws'] * self._pdata['wc']).sum()
+        )
+        self.wstotal = self._compute(self._pdata['ws'].sum())
 
         if self._logger:
             self._logger.info(
-                "Catalogue loaded: %d particles with "
-                "total sample weight %.3f (%s).",
-                self.ntotal, self.wtotal, self
+                "Catalogue loaded: "
+                "ntotal = %d, wtotal = %.3f, wstotal = %.3f (%s).",
+                self.ntotal, self.wtotal, self.wstotal, self
             )
 
         return self
 
     def __str__(self):
         try:
             return "ParticleCatalogue(source={})".format(self._source)
@@ -767,40 +776,43 @@
             Catalogue attributes as a header string.
 
         """
         if catalogue_ref is None:
             text_lines = [
                 "Catalogue source: {}"
                     .format(self._source),  # noqa: E131
-                "Catalogue size: {:d} particles of total sample weight {:.3f}"
-                    .format(self.ntotal, self.wtotal),
+                "Catalogue size: "
+                "ntotal = {:d}, wtotal = {:.3f}, wstotal = {:.3f}"
+                    .format(self.ntotal, self.wtotal, self.wstotal),
                 "Catalogue particle extents: "
                 "([{:.3f}, {:.3f}], [{:.3f}, {:.3f}], [{:.3f}, {:.3f}])"
                     .format(
                         *self.bounds['x'], *self.bounds['y'], *self.bounds['z']
                     ),
             ]
         else:
             text_lines = [
                 "Data catalogue source: {}"
                     .format(self._source),  # noqa: E131
                 "Data catalogue size: "
-                "{:d} particles of total sample weight {:.3f}"
-                    .format(self.ntotal, self.wtotal),
+                "ntotal = {:d}, wtotal = {:.3f}, wstotal = {:.3f}"
+                    .format(self.ntotal, self.wtotal, self.wstotal),
                 "Data-source particle extents: "
                 "([{:.3f}, {:.3f}], [{:.3f}, {:.3f}], [{:.3f}, {:.3f}])"
                     .format(
                         *self.bounds['x'], *self.bounds['y'], *self.bounds['z']
                     ),
                 "Random catalogue source: {}"
                     .format(catalogue_ref._source),  # noqa: E131
                 "Random catalogue size: "
-                "{:d} particles of total sample weight {:.3f}"
+                "ntotal = {:d}, wtotal = {:.3f}, wstotal = {:.3f}"
                     .format(  # noqa: E131
-                        catalogue_ref.ntotal, catalogue_ref.wtotal
+                        catalogue_ref.ntotal,
+                        catalogue_ref.wtotal,
+                        catalogue_ref.wstotal,
                     ),
                 "Random-source particle extents: "
                 "([{:.3f}, {:.3f}], [{:.3f}, {:.3f}], [{:.3f}, {:.3f}])"
                     .format(  # noqa: E131
                         *catalogue_ref.bounds['x'],
                         *catalogue_ref.bounds['y'],
                         *catalogue_ref.bounds['z']
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/dataobjs.pxd` & `Triumvirate-0.2.0/src/triumvirate/dataobjs.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         int num_bins
         vector[double] bin_edges
         vector[double] bin_centres
         vector[double] bin_widths
 
         CppBinning(string space, string scheme) except +
 
-        void set_bins(double bin_min, double bin_max, int nbins)
-        void set_bins(double boxsize_max, int ngrid_min)
+        void set_bins(double bin_min, double bin_max, int nbins) except +
+        void set_bins(double boxsize_max, int ngrid_min) except +
 
 
     # --------------------------------------------------------------------
     # Line of sight
     # --------------------------------------------------------------------
 
     struct LineOfSight "trv::LineOfSight":
@@ -48,21 +48,21 @@
         vector[int] nmodes
         vector[np.complex128_t] pk_raw
         vector[np.complex128_t] pk_shot
 
     struct TwoPCFMeasurements "trv::TwoPCFMeasurements":
         vector[double] rbin
         vector[double] reff
-        vector[int] npairs;
+        vector[int] npairs
         vector[np.complex128_t] xi
 
     struct TwoPCFWindowMeasurements "trv::TwoPCFWindowMeasurements":
         vector[double] rbin
         vector[double] reff
-        vector[int] npairs;
+        vector[int] npairs
         vector[np.complex128_t] xi
 
     # -- Three-point statistics ------------------------------------------
 
     struct BispecMeasurements "trv::BispecMeasurements":
         vector[double] k1_bin
         vector[double] k2_bin
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/dataobjs.pyx` & `Triumvirate-0.2.0/src/triumvirate/dataobjs.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/arrayops.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/arrayops.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/dataobjs.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/dataobjs.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
    */
   void set_bins();
 
   /**
    * @brief Construct binning from a mesh grid.
    *
    * The bin width is given by the grid resolution in configuration
-   * space or the fundamental wavenumber in Fourier space. The bin
+   * space or the fundamental wavenumber in Fourier space.  The bin
    * minimum is zero and the bin maximum is half the boxsize in
    * configuration space or the Nyquist wavenumber in Fourier space.
    *
    * @param boxsize_max (Maximum) box size.
    * @param ngrid_min (Minimum) grid number.
    *
    * @attention @ref trv::Binning.scheme is reset to "lin".
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/fftlog.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/fftlog.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/field.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/field.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/io.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/io.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -81,40 +81,42 @@
  * @brief Print the pre-measurement header to a file including information
  *        about the catalogue(s) and mesh grid assignment.
  *
  * @param fileptr File to print to.
  * @param params Parameter set.
  * @param catalogue_data (Data-source) particle catalogue.
  * @param catalogue_rand (Random-source) particle catalogue.
- * @param norm_factor Normalisation factor.
- * @param norm_factor_alt Alternative normalisation factor.
+ * @param norm_factor_part Particle-based normalisation factor.
+ * @param norm_factor_mesh Mesh-based normalisation factor.
+ * @param norm_factor_meshes Normalisation factor based on mixed meshes.
  */
 void print_measurement_header_to_file(
   std::FILE* fileptr, trv::ParameterSet& params,
   trv::ParticleCatalogue& catalogue_data,
   trv::ParticleCatalogue& catalogue_rand,
-  double norm_factor, double norm_factor_alt
+  double norm_factor_part, double norm_factor_mesh, double norm_factor_meshes
 );
 
 /**
  * @brief Print the pre-measurement header to a file including information
  *        about the catalogue(s) and mesh grid assignment.
  *
  * @param fileptr File to print to.
  * @param params Parameter set.
  * @param catalogue Particle catalogue.
- * @param norm_factor Normalisation factor.
- * @param norm_factor_alt Alternative normalisation factor.
+ * @param norm_factor_part Particle-based normalisation factor.
+ * @param norm_factor_mesh Mesh-based normalisation factor.
+ * @param norm_factor_meshes Normalisation factor based on mixed meshes.
  *
  * @overload
  */
 void print_measurement_header_to_file(
   std::FILE* fileptr,
   trv::ParameterSet& params, trv::ParticleCatalogue& catalogue,
-  double norm_factor, double norm_factor_alt
+  double norm_factor_part, double norm_factor_mesh, double norm_factor_meshes
 );
 
 
 // -----------------------------------------------------------------------
 // Two-point measurement header
 // -----------------------------------------------------------------------
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/maths.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/maths.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/monitor.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/monitor.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/parameters.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/parameters.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,16 @@
   int i_wa = 0;  ///< first order of the wide-angle correction term
   int j_wa = 0;  ///< second order of the wide-angle correction term
 
   // Measurement choices.
   /// form of the bispectrum measurement: {"diag" (default), "full"}
   std::string form = "diag";
 
-  /// normalisation convention: {"particle" (default), "mesh"}
+  /// normalisation convention: {"none", "particle" (default), "mesh",
+  ///                            "mesh-mixed"}
   std::string norm_convention = "particle";
 
   // Measurement parameters.
   /// binning scheme: {"lin" (default), "log",
   ///                  "linpad", "logpad", "custom"}
   std::string binning = "lin";
 
@@ -149,14 +150,32 @@
   // ---------------------------------------------------------------------
 
   /// logging verbosity level: {0  (NSET), 10 (DBUG), 20 (STAT) (default),
   ///                           30 (INFO), 40 (WARN), 50 (ERRO)}
   int verbose = 20;
 
   /**
+   * @brief Construct a parameter set.
+   */
+  ParameterSet() = default;
+
+  /**
+   * @brief Destroy the parameter set.
+   *
+   */
+  ~ParameterSet() = default;
+
+  /**
+   * @brief Construct a copied parameter set.
+   *
+   * @param other Parameter set to be copied.
+   */
+  ParameterSet(const ParameterSet& other);
+
+  /**
    * @brief Read parameters from a file.
    *
    * @param parameter_filepath Parameter file path.
    * @returns Validation exit status.
    */
   int read_from_file(char* parameter_filepath);
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/particles.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/particles.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -64,19 +64,21 @@
     double pos[3];  ///< particle position vector
     double nz;      ///< redshift-dependent expected number density
     double ws;      ///< particle sample weight
     double wc;      ///< particle clustering weight
     double w;       ///< particle overall weight
   }* pdata;         ///< particle data
 
-  int ntotal;     ///< total number of particles
-  double wtotal;  ///< total sample weight of particles
-
-  double pos_min[3];  ///< minimum values of particle positions
-  double pos_max[3];  ///< maximum values of particle positions
+  int ntotal;      ///< total number of particles
+  double wtotal;   ///< total overall weight of particles
+  double wstotal;  ///< total sample weight of particles
+
+  double pos_min[3];   ///< minimum values of particle coordinates
+  double pos_max[3];   ///< maximum values of particle coordinates
+  double pos_span[3];  ///< span of particle coordinates
 
   // ---------------------------------------------------------------------
   // Life cycle
   // ---------------------------------------------------------------------
 
   /**
    * @brief Construct the particle catalogue with initial values.
@@ -96,16 +98,18 @@
 
   /**
    * @brief Initialise particle data container.
    *
    * @attention This method does not set the values of
    *            @ref trv::ParticleCatalogue.ParticleData,
    *            @ref trv::ParticleCatalogue.wtotal,
+   *            @ref trv::ParticleCatalogue.wstotal,
    *            @ref trv::ParticleCatalogue.pos_min or
-   *            @ref trv::ParticleCatalogue.pos_max.
+   *            @ref trv::ParticleCatalogue.pos_max, or
+   *            @ref trv::ParticleCatalogue.pos_span.
    *
    * @param num Number of data units (i.e. particles).
    */
   void initialise_particles(const int num);
 
   /**
    * @brief Finalise particle data container.
@@ -160,27 +164,29 @@
   );
 
   // ---------------------------------------------------------------------
   // Catalogue properties
   // ---------------------------------------------------------------------
 
   /**
-   * @brief Calculate total sample weight of particles.
+   * @brief Calculate total overall weight of particles.
    *
-   * @attention This method resets @ref trv::ParticleCatalogue::wtotal.
+   * @attention This method resets @ref trv::ParticleCatalogue::wtotal
+   *            and @ref trv::ParticleCatalogue::wstotal.
    */
-  void calc_wtotal();
+  void calc_total_weights();
 
   /**
    * @brief Calculate the extents of particle positions.
    *
-   * @attention This method resets @ref trv::ParticleCatalogue::pos_min
-   *            and @ref trv::ParticleCatalogue::pos_max.
+   * @attention This method resets @ref trv::ParticleCatalogue::pos_min,
+   *            @ref trv::ParticleCatalogue::pos_max and
+   *            @ref trv::ParticleCatalogue::pos_span.
    */
-  void calc_pos_min_and_max();
+  void calc_pos_extents();
 
   // ---------------------------------------------------------------------
   // Catalogue operations
   // ---------------------------------------------------------------------
 
   /**
    * @brief Offset particle positions by a given vector.
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/threept.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/threept.hpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,34 +82,34 @@
 
 
 // ***********************************************************************
 // Normalisation
 // ***********************************************************************
 
 /**
- * @brief Calculate mesh-based bispectrum normalisation.
+ * @brief Calculate particle-based bispectrum normalisation.
  *
  * @param particles Particle catalogue.
- * @param params Parameter set.
  * @param alpha Alpha contrast.
  * @returns Bispectrum normalisation factor.
  */
-double calc_bispec_normalisation_from_mesh(
-  ParticleCatalogue& particles, trv::ParameterSet& params, double alpha=1.
+double calc_bispec_normalisation_from_particles(
+  ParticleCatalogue& particles, double alpha=1.
 );
 
 /**
- * @brief Calculate particle-based bispectrum normalisation.
+ * @brief Calculate mesh-based bispectrum normalisation.
  *
  * @param particles Particle catalogue.
+ * @param params Parameter set.
  * @param alpha Alpha contrast.
  * @returns Bispectrum normalisation factor.
  */
-double calc_bispec_normalisation_from_particles(
-  ParticleCatalogue& particles, double alpha=1.
+double calc_bispec_normalisation_from_mesh(
+  ParticleCatalogue& particles, trv::ParameterSet& params, double alpha=1.
 );
 
 
 // ***********************************************************************
 // Shot noise
 // ***********************************************************************
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/include/twopt.hpp` & `Triumvirate-0.2.0/src/triumvirate/include/twopt.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -33,14 +33,15 @@
  *   simulation catalogues.
  *
  */
 
 #ifndef TRIUMVIRATE_INCLUDE_TWOPT_HPP_INCLUDED_
 #define TRIUMVIRATE_INCLUDE_TWOPT_HPP_INCLUDED_
 
+#include <algorithm>
 #include <cmath>
 #include <complex>
 #include <cstdio>
 
 #include "monitor.hpp"
 #include "maths.hpp"
 #include "parameters.hpp"
@@ -71,34 +72,85 @@
 
 
 // ***********************************************************************
 // Normalisation
 // ***********************************************************************
 
 /**
+ * @brief Calculate particle-based power spectrum normalisation.
+ *
+ * @param particles Particle catalogue.
+ * @param alpha Alpha contrast.
+ * @returns Power spectrum normalisation factor.
+ */
+double calc_powspec_normalisation_from_particles(
+  ParticleCatalogue& particles, double alpha=1.
+);
+
+/**
  * @brief Calculate mesh-based power spectrum normalisation.
  *
  * @param particles Particle catalogue.
  * @param params Parameter set.
  * @param alpha Alpha contrast.
  * @returns Power spectrum normalisation factor.
  */
 double calc_powspec_normalisation_from_mesh(
   trv::ParticleCatalogue& particles, trv::ParameterSet& params, double alpha=1.
 );
 
 /**
- * @brief Calculate particle-based power spectrum normalisation.
+ * @brief Calculate power spectrum normalisation from mixed meshes.
  *
- * @param particles Particle catalogue.
+ * This normalisation convention is used for paired survey-type catalogues
+ * only, where the two meshes come from separate data- and random-source
+ * particle catalogues.
+ *
+ * @see <a href="https://pypower.rtfd.io/en/latest/api/api.html
+ * #pypower.fft_power.normalization">@c pypower documentation</a>.
+ *
+ * @param particles_data Data-source particle catalogue.
+ * @param particles_rand Random-source particle catalogue.
+ * @param params Parameter set.
  * @param alpha Alpha contrast.
  * @returns Power spectrum normalisation factor.
  */
-double calc_powspec_normalisation_from_particles(
-  ParticleCatalogue& particles, double alpha=1.
+double calc_powspec_normalisation_from_meshes(
+  trv::ParticleCatalogue& particles_data,
+  trv::ParticleCatalogue& particles_rand,
+  trv::ParameterSet& params, double alpha
+);
+
+/**
+ * @brief Calculate power spectrum normalisation from mixed meshes.
+ *
+ * The box size per dimension is internally determined by the particle
+ * coordinate extents, with a padding factor applied. The mesh number in
+ * each dimension is determined by the box size and the cell size.
+ *
+ * @param particles_data Data-source particle catalogue.
+ * @param particles_rand Random-source particle catalogue.
+ * @param params Parameter set.
+ * @param alpha Alpha contrast.
+ * @param padding Padding factor for the box size in each dimension.
+ *                This overrides the box size set in the parameter set.
+ * @param cellsize Cell size of the mesh grid in each dimension.  This
+ *                 overrides the mesh number set in the parameter set.
+ * @param assignment Assignment scheme for particles to mesh.  This
+ *                   overrides the assignment scheme set in the
+ *                   parameter set.
+ * @returns Power spectrum normalisation factor.
+ *
+ * @overload
+ */
+double calc_powspec_normalisation_from_meshes(
+  trv::ParticleCatalogue& particles_data,
+  trv::ParticleCatalogue& particles_rand,
+  trv::ParameterSet& params, double alpha,
+  double padding, double cellsize, std::string assignment
 );
 
 
 // ***********************************************************************
 // Shot noise
 // ***********************************************************************
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/logger.py` & `Triumvirate-0.2.0/src/triumvirate/logger.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/parameters.pxd` & `Triumvirate-0.2.0/src/triumvirate/parameters.pxd`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/parameters.pyx` & `Triumvirate-0.2.0/src/triumvirate/parameters.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -444,14 +444,22 @@
             self.thisptr.norm_convention = \
                 self._params['norm_convention'].lower().encode('utf-8')
 
         if self._params['binning'] is not None:
             self.thisptr.binning = \
                 self._params['binning'].lower().encode('utf-8')
 
+        # Attribute otherwise-derived parameters.
+        space_ = self._params.get('space', '').lower()
+        npoint_ = self._params.get('npoint', '').lower()
+        if space_ in {'fourier', 'config'}:
+            self.thisptr.space = space_.encode('utf-8')
+        if npoint_ in {'2pt', '3pt'}:
+            self.thisptr.npoint = npoint_.encode('utf-8')
+
         # -- Misc --------------------------------------------------------
 
         if self._params['verbose'] is not None:
             self.thisptr.verbose = self._params['verbose']
 
         # ----------------------------------------------------------------
         # Validation
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/resources/params_template.ini` & `Triumvirate-0.2.0/src/triumvirate/resources/params_template.ini`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,18 @@
 # Orders of wide-angle corrections.
 i_wa =
 j_wa =
 
 # Form of three-point statistic measurements: {'full', 'diag' (default)}.
 form = diag
 
-# Normalisation convention: {'particle' (default), 'mesh'}.
+# Normalisation convention: {
+#   'none', 'particle' (default), 'mesh',
+#   'mesh-mixed' (two-point statistics only)
+# }.
 norm_convention = particle
 
 # Binning scheme: {'lin' (default), 'log', 'linpad', 'logpad', 'custom'}.
 binning = lin
 
 # Minimum and maximum of the range of measurement scales.
 # The binning coordinate is either wavenumbers (in h/Mpc) in Fourier space,
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/resources/params_template.yml` & `Triumvirate-0.2.0/tests/test_input/params/tmpl_params.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This is a copy of ``src/triumvirate/resources/params_template.yml".
 ---
 
 # -- I/O -----------------------------------------------------------------
 
 # Directories for input/output.
 # The paths can be either absolute or relative to the working directory.
 # If unset, the current working directory is assumed.
@@ -69,15 +70,18 @@
 wa_orders:
   i:
   j:
 
 # Form of three-point statistic measurements: {'full', 'diag' (default)}.
 form: diag
 
-# Normalisation convention: {'particle' (default), 'mesh'}.
+# Normalisation convention: {
+#   'none', 'particle' (default), 'mesh',
+#   'mesh-mixed' (two-point statistics only)
+# }.
 norm_convention: particle
 
 # Binning scheme: {'lin' (default), 'log', 'linpad', 'logpad', 'custom'}.
 binning: lin
 
 # Minimum and maximum of the binning range (i.e. range of measurement scales)
 # as a list.
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/arrayops.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/arrayops.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/dataobjs.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/dataobjs.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/fftlog.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/fftlog.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/field.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/field.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/io.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/io.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -57,18 +57,18 @@
 void make_write_dir(std::string dirstr) {
   // Skip special directories.
   if (dirstr.empty() || dirstr == "." || dirstr == "./" || dirstr == "/") {
     return;
   }
   if (mkdir(dirstr.c_str(), 0777) && errno != EEXIST) {
     trv::sys::logger.error(
-      "Failed to create output measurement directory."
+      "Failed to create output measurement directory: %s.", dirstr.c_str()
     );
     throw trv::sys::IOError(
-      "Failed to create output measurement directory.\n"
+      "Failed to create output measurement directory: %s.\n", dirstr.c_str()
     );
   }
 }
 
 }  // namespace trv::sys
 
 
@@ -82,168 +82,206 @@
 // Measurement header
 // -----------------------------------------------------------------------
 
 void print_measurement_header_to_file(
   std::FILE* fileptr, trv::ParameterSet& params,
   trv::ParticleCatalogue& catalogue_data,
   trv::ParticleCatalogue& catalogue_rand,
-  double norm_factor, double norm_factor_alt
+  double norm_factor_part, double norm_factor_mesh, double norm_factor_meshes
 ) {
   std::fprintf(
     fileptr,
     "%s Data catalogue source: %s\n",
     comment_delimiter, catalogue_data.source.c_str()
   );
   std::fprintf(
     fileptr,
-    "%s Data catalogue size: %d particles of total sample weight %.3f\n",
-    comment_delimiter, catalogue_data.ntotal, catalogue_data.wtotal
+    "%s Data catalogue size: ntotal = %d, wtotal = %.3f, wstotal = %.3f\n",
+    comment_delimiter,
+    catalogue_data.ntotal, catalogue_data.wtotal, catalogue_data.wstotal
   );
   std::fprintf(
     fileptr,
     "%s Data-source particle extents: "
-    "([%.3f, %.3f], [%.3f, %.3f], [%.3f, %.3f])\n",
+    "[(%.3f, %.3f), (%.3f, %.3f), (%.3f, %.3f)]\n",
     comment_delimiter,
     catalogue_data.pos_min[0], catalogue_data.pos_max[0],
     catalogue_data.pos_min[1], catalogue_data.pos_max[1],
     catalogue_data.pos_min[2], catalogue_data.pos_max[2]
   );
   std::fprintf(
     fileptr,
     "%s Random catalogue source: %s\n",
     comment_delimiter, catalogue_rand.source.c_str()
   );
   std::fprintf(
     fileptr,
-    "%s Random catalogue size: %d particles of total sample weight %.3f\n",
-    comment_delimiter, catalogue_rand.ntotal, catalogue_rand.wtotal
+    "%s Random catalogue size: ntotal = %d, wtotal = %.3f, wstotal = %.3f\n",
+    comment_delimiter,
+    catalogue_rand.ntotal, catalogue_rand.wtotal, catalogue_rand.wstotal
   );
   std::fprintf(
     fileptr,
     "%s Random-source particle extents: "
-    "([%.3f, %.3f], [%.3f, %.3f], [%.3f, %.3f])\n",
+    "[(%.3f, %.3f), (%.3f, %.3f), (%.3f, %.3f)]\n",
     comment_delimiter,
     catalogue_rand.pos_min[0], catalogue_rand.pos_max[0],
     catalogue_rand.pos_min[1], catalogue_rand.pos_max[1],
     catalogue_rand.pos_min[2], catalogue_rand.pos_max[2]
   );
 
   std::fprintf(
     fileptr,
-    "%s Box size: (%.3f, %.3f, %.3f)\n",
+    "%s Box size: [%.3f, %.3f, %.3f]\n",
     comment_delimiter,
     params.boxsize[0], params.boxsize[1], params.boxsize[2]
   );
   std::fprintf(
     fileptr,
     "%s Box alignment: %s\n",
     comment_delimiter,
     params.alignment.c_str()
   );
   std::fprintf(
     fileptr,
-    "%s Mesh number: (%d, %d, %d)\n",
+    "%s Mesh number: [%d, %d, %d]\n",
     comment_delimiter,
     params.ngrid[0], params.ngrid[1], params.ngrid[2]
   );
   std::fprintf(
     fileptr,
     "%s Mesh assignment and interlacing: %s, %s\n",
     comment_delimiter,
     params.assignment.c_str(), params.interlace.c_str()
   );
 
+  if (params.norm_convention == "none") {
+    std::fprintf(
+      fileptr,
+      "%s Normalisation factor: %.9e (%s)\n",
+      comment_delimiter, 1., params.norm_convention.c_str()
+    );
+  } else
   if (params.norm_convention == "particle") {
     std::fprintf(
       fileptr,
-      "%s Normalisation factor: "
-      "%.9e (particle-based, used), %.9e (mesh-based, alternative)\n",
-      comment_delimiter,
-      norm_factor, norm_factor_alt
+      "%s Normalisation factor: %.9e (%s)\n",
+      comment_delimiter, norm_factor_part, params.norm_convention.c_str()
     );
   } else
   if (params.norm_convention == "mesh") {
     std::fprintf(
       fileptr,
-      "%s Normalisation factor: "
-      "%.9e (mesh-based, used), %.9e (particle-based, alternative)\n",
-      comment_delimiter,
-      norm_factor, norm_factor_alt
+      "%s Normalisation factor: %.9e (%s)\n",
+      comment_delimiter, norm_factor_mesh, params.norm_convention.c_str()
+    );
+  } else
+  if (params.norm_convention == "mesh-mixed") {
+    std::fprintf(
+      fileptr,
+      "%s Normalisation factor: %.9e (%s)\n",
+      comment_delimiter, norm_factor_meshes, params.norm_convention.c_str()
     );
   }
+
+  std::fprintf(
+    fileptr,
+    "%s Normalisation factor alternatives: "
+    "%.9e (particle), %.9e (mesh), %.9e (mesh-mixed)\n",
+    comment_delimiter,
+    norm_factor_part, norm_factor_mesh, norm_factor_meshes
+  );
 }
 
 void print_measurement_header_to_file(
   std::FILE* fileptr,
   trv::ParameterSet& params, trv::ParticleCatalogue& catalogue,
-  double norm_factor, double norm_factor_alt
+  double norm_factor_part, double norm_factor_mesh, double norm_factor_meshes
 ) {
   std::fprintf(
     fileptr,
     "%s Catalogue source: %s\n",
     comment_delimiter, catalogue.source.c_str()
   );
   std::fprintf(
     fileptr,
-    "%s Catalogue size: %d particles of total sample weight %.3f\n",
-    comment_delimiter, catalogue.ntotal, catalogue.wtotal
+    "%s Catalogue size: ntotal = %d, wtotal = %.3f, wstotal = %.3f\n",
+    comment_delimiter, catalogue.ntotal, catalogue.wtotal, catalogue.wstotal
   );
   std::fprintf(
     fileptr,
     "%s Catalogue particle extents: "
-    "([%.3f, %.3f], [%.3f, %.3f], [%.3f, %.3f])\n",
+    "[(%.3f, %.3f), (%.3f, %.3f), (%.3f, %.3f)]\n",
     comment_delimiter,
     catalogue.pos_min[0], catalogue.pos_max[0],
     catalogue.pos_min[1], catalogue.pos_max[1],
     catalogue.pos_min[2], catalogue.pos_max[2]
   );
 
   std::fprintf(
     fileptr,
-    "%s Box size: (%.3f, %.3f, %.3f)\n",
+    "%s Box size: [%.3f, %.3f, %.3f]\n",
     comment_delimiter,
     params.boxsize[0], params.boxsize[1], params.boxsize[2]
   );
   std::fprintf(
     fileptr,
     "%s Box alignment: %s\n",
     comment_delimiter,
     params.alignment.c_str()
   );
   std::fprintf(
     fileptr,
-    "%s Mesh number: (%d, %d, %d)\n",
+    "%s Mesh number: [%d, %d, %d]\n",
     comment_delimiter,
     params.ngrid[0], params.ngrid[1], params.ngrid[2]
   );
   std::fprintf(
     fileptr,
     "%s Mesh assignment and interlacing: %s, %s\n",
     comment_delimiter,
     params.assignment.c_str(), params.interlace.c_str()
   );
 
+  if (params.norm_convention == "none") {
+    std::fprintf(
+      fileptr,
+      "%s Normalisation factor: %.9e (%s)\n",
+      comment_delimiter, 1., params.norm_convention.c_str()
+    );
+  } else
   if (params.norm_convention == "particle") {
     std::fprintf(
       fileptr,
-      "%s Normalisation factor: "
-      "%.9e (particle-based, used), %.9e (mesh-based, alternative)\n",
-      comment_delimiter,
-      norm_factor, norm_factor_alt
+      "%s Normalisation factor: %.9e (%s)\n",
+      comment_delimiter, norm_factor_part, params.norm_convention.c_str()
     );
   } else
   if (params.norm_convention == "mesh") {
     std::fprintf(
       fileptr,
-      "%s Normalisation factor: "
-      "%.9e (mesh-based, used), %.9e (particle-based, alternative)\n",
-      comment_delimiter,
-      norm_factor, norm_factor_alt
+      "%s Normalisation factor: %.9e (%s)\n",
+      comment_delimiter, norm_factor_mesh, params.norm_convention.c_str()
+    );
+  } else
+  if (params.norm_convention == "mesh-mixed") {
+    std::fprintf(
+      fileptr,
+      "%s Normalisation factor: %.9e (%s)\n",
+      comment_delimiter, norm_factor_meshes, params.norm_convention.c_str()
     );
   }
+
+  std::fprintf(
+    fileptr,
+    "%s Normalisation factor alternatives: "
+    "%.9e (particle), %.9e (mesh), %.9e (mesh-mixed)\n",
+    comment_delimiter,
+    norm_factor_part, norm_factor_mesh, norm_factor_meshes
+  );
 }
 
 
 // -----------------------------------------------------------------------
 // Two-point measurement data table
 // -----------------------------------------------------------------------
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/maths.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/maths.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/monitor.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/monitor.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/parameters.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/parameters.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,58 @@
 
 #include "parameters.hpp"
 
 namespace trvs = trv::sys;
 
 namespace trv {
 
+ParameterSet::ParameterSet(const ParameterSet& other) {
+  // Copy I/O parameters.
+  this->catalogue_dir = other.catalogue_dir;
+  this->measurement_dir = other.measurement_dir;
+  this->data_catalogue_file = other.data_catalogue_file;
+  this->rand_catalogue_file = other.rand_catalogue_file;
+  this->catalogue_columns = other.catalogue_columns;
+  this->output_tag = other.output_tag;
+
+  // Copy mesh sampling parameters.
+  for (int i = 0; i < 3; i++) {
+    this->boxsize[i] = other.boxsize[i];
+    this->ngrid[i] = other.ngrid[i];
+  }
+  this->volume = other.volume;
+  this->nmesh = other.nmesh;
+  this->alignment = other.alignment;
+  this->padscale = other.padscale;
+  this->padfactor = other.padfactor;
+  this->assignment = other.assignment;
+  this->interlace = other.interlace;
+
+  // Copy measurement parameters.
+  this->catalogue_type = other.catalogue_type;
+  this->statistic_type = other.statistic_type;
+  this->npoint = other.npoint;
+  this->space = other.space;
+  this->ell1 = other.ell1;
+  this->ell2 = other.ell2;
+  this->ELL = other.ELL;
+  this->i_wa = other.i_wa;
+  this->j_wa = other.j_wa;
+  this->form = other.form;
+  this->norm_convention = other.norm_convention;
+  this->binning = other.binning;
+  this->bin_min = other.bin_min;
+  this->bin_max = other.bin_max;
+  this->num_bins = other.num_bins;
+  this->idx_bin = other.idx_bin;
+
+  // Copy misc parameters.
+  this->verbose = other.verbose;
+}
+
 int ParameterSet::read_from_file(char* parameter_filepath) {
   // ---------------------------------------------------------------------
   // Initialisation
   // ---------------------------------------------------------------------
 
   // Load parameter file.
   std::string param_filepath = parameter_filepath;
@@ -474,29 +518,46 @@
       throw trvs::InvalidParameterError(
         "`form` must be either 'full' or 'diag': `form` = '%s'.\n",
         this->form.c_str()
       );
     }
   }
   if (!(
-    this->norm_convention == "mesh" || this->norm_convention == "particle"
+    this->norm_convention == "none"
+    || this->norm_convention == "particle"
+    || this->norm_convention == "mesh"
+    || this->norm_convention == "mesh-mixed"
   )) {
     if (trvs::currTask == 0) {
       trvs::logger.error(
         "Normalisation convention must be "
         "'mesh' or 'particle': `norm_convention` = '%s'.",
         this->norm_convention.c_str()
       );
       throw trvs::InvalidParameterError(
         "Normalisation convention must be "
         "'mesh' or 'particle': `norm_convention` = '%s'.\n",
         this->norm_convention.c_str()
       );
     }
   }
+  if (this->norm_convention == "mesh-mixed" && this->npoint != "2pt") {
+    if (trvs::currTask == 0) {
+      trvs::logger.error(
+        "Normalisation convention 'mesh-mixed' only applies to "
+        "two-point statistics: `npoint` = '%s'.",
+        this->npoint.c_str()
+      );
+      throw trvs::InvalidParameterError(
+        "Normalisation convention 'mesh-mixed' only applies to "
+        "two-point statistics: `npoint` = '%s'.\n",
+        this->npoint.c_str()
+      );
+    }
+  }
   if (!(
     this->binning == "lin"
     || this->binning == "log"
     || this->binning == "linpad"
     || this->binning == "logpad"
     || this->binning == "custom"
   )) {
@@ -508,15 +569,20 @@
       throw trvs::InvalidParameterError(
         "Binning scheme is unrecognised: `binning` = '%s'.\n",
         this->binning.c_str()
       );
     }
   }
 
-  // Validate numerical parameters.
+  // Validate and derive numerical parameters.
+  this->volume =
+    this->boxsize[0] * this->boxsize[1] * this->boxsize[2];  // derivation
+  this->nmesh =
+    this->ngrid[0] * this->ngrid[1] * this->ngrid[2];  // derivation
+
   if (this->volume <= 0.) {
     if (trvs::currTask == 0) {
       trvs::logger.error(
         "Derived total box volume is non-positive: `volume` = '%d'. "
         "Possible numerical overflow due to large `boxsize`, "
         "or `boxsize` is unset.",
         this->nmesh
@@ -605,26 +671,26 @@
   }
   if (this->space == "fourier") {
     double wavenum_nyquist = M_PI *
       *std::min_element(this->ngrid, this->ngrid + 3)
       / *std::max_element(this->boxsize, this->boxsize + 3);
     if (this->bin_min > wavenum_nyquist) {
       trvs::logger.warn(
-        "Lower wavenumber limit exceeds the Nyquist wavenumber %.3e.",
+        "Lower wavenumber limit exceeds the Nyquist wavenumber %.4f.",
         wavenum_nyquist
       );
     }
   } else
   if (this->space == "config") {
     double separation_nyquist = 2 *
       *std::max_element(this->boxsize, this->boxsize + 3)
       / *std::min_element(this->ngrid, this->ngrid + 3);
     if (this->bin_max < separation_nyquist) {
       trvs::logger.warn(
-        "Upper separation limit undershoots the Nyquist scale %.3f.",
+        "Upper separation limit undershoots the Nyquist scale %.4f.",
         separation_nyquist
       );
     }
   }
 
   if (this->num_bins < 2) {
     if (trvs::currTask == 0) {
@@ -723,17 +789,17 @@
   print_par_str("catalogue_dir = %s\n", this->catalogue_dir);
   print_par_str("measurement_dir = %s\n", this->measurement_dir);
   print_par_str("data_catalogue_file = %s\n", this->data_catalogue_file);
   print_par_str("rand_catalogue_file = %s\n", this->rand_catalogue_file);
   print_par_str("catalogue_columns = %s\n", this->catalogue_columns);
   print_par_str("output_tag = %s\n", this->output_tag);
 
-  print_par_double("boxsize_x = %.2f\n", this->boxsize[0]);
-  print_par_double("boxsize_y = %.2f\n", this->boxsize[1]);
-  print_par_double("boxsize_z = %.2f\n", this->boxsize[2]);
+  print_par_double("boxsize_x = %.3f\n", this->boxsize[0]);
+  print_par_double("boxsize_y = %.3f\n", this->boxsize[1]);
+  print_par_double("boxsize_z = %.3f\n", this->boxsize[2]);
   print_par_int("ngrid_x = %d\n", this->ngrid[0]);
   print_par_int("ngrid_y = %d\n", this->ngrid[1]);
   print_par_int("ngrid_z = %d\n", this->ngrid[2]);
 
   print_par_double("volume = %.6e\n", this->volume);
   print_par_int("nmesh = %d\n", this->nmesh);
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/particles.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/particles.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,19 @@
     trvs::logger.reset_level(verbose);
   }
 
   // Set default values (likely redundant but safe).
   this->pdata = nullptr;
   this->ntotal = 0;
   this->wtotal = 0.;
+  this->wstotal = 0.;
   for (int iaxis = 0; iaxis < 3; iaxis++) {
     this->pos_min[iaxis] = 0.;
     this->pos_max[iaxis] = 0.;
+    this->pos_span[iaxis] = 0.;
   }
 }
 
 ParticleCatalogue::~ParticleCatalogue() {this->finalise_particles();}
 
 void ParticleCatalogue::initialise_particles(const int num) {
   // Check the total number of particles.
@@ -241,19 +243,19 @@
 
   fin.close();
 
   // ---------------------------------------------------------------------
   // Catalogue properties
   // ---------------------------------------------------------------------
 
-  // Calculate sample weight sum.
-  this->calc_wtotal();
+  // Calculate total weights.
+  this->calc_total_weights();
 
-  // Calculate the extents of particles.
-  this->calc_pos_min_and_max();
+  // Calculate particle extents.
+  this->calc_pos_extents();
 
   return 0;
 }
 
 int ParticleCatalogue::load_particle_data(
   std::vector<double> x, std::vector<double> y, std::vector<double> z,
   std::vector<double> nz, std::vector<double> ws, std::vector<double> wc
@@ -294,56 +296,58 @@
     this->pdata[pid].nz = nz[pid];
     this->pdata[pid].ws = ws[pid];
     this->pdata[pid].wc = wc[pid];
     this->pdata[pid].w = ws[pid] * wc[pid];
   }
 
   // Calculate sample weight sum.
-  this->calc_wtotal();
+  this->calc_total_weights();
 
   // Calculate the extents of particles.
-  this->calc_pos_min_and_max();
+  this->calc_pos_extents();
 
   return 0;
 }
 
 
 // ***********************************************************************
 // Catalogue properties
 // ***********************************************************************
 
-void ParticleCatalogue::calc_wtotal() {
+void ParticleCatalogue::calc_total_weights() {
   if (this->pdata == nullptr) {
     if (trvs::currTask == 0) {
       trvs::logger.error("Particle data are uninitialised.");
       throw trvs::InvalidDataError("Particle data are uninitialised.\n");
     }
   }
 
-  double wtotal = 0.;
+  double wtotal = 0., wstotal = 0.;
 
 #ifdef TRV_USE_OMP
-#pragma omp parallel for reduction(+:wtotal)
+#pragma omp parallel for reduction(+:wtotal, wstotal)
 #endif  // TRV_USE_OMP
   for (int pid = 0; pid < this->ntotal; pid++) {
-    wtotal += this->pdata[pid].ws;
+    wtotal += this->pdata[pid].w;
+    wstotal += this->pdata[pid].ws;
   }
 
   this->wtotal = wtotal;
+  this->wstotal = wstotal;
 
   if (trvs::currTask == 0) {
     trvs::logger.info(
-      "Catalogue loaded: %d particles with "
-      "total sample weight %.3f (source=%s).",
-      this->ntotal, this->wtotal, this->source.c_str()
+      "Catalogue loaded: "
+      "ntotal = %d, wtotal = %.3f, wstotal = %.3f (source=%s).",
+      this->ntotal, this->wtotal, this->wstotal, this->source.c_str()
     );
   }
 }
 
-void ParticleCatalogue::calc_pos_min_and_max() {
+void ParticleCatalogue::calc_pos_extents() {
   if (this->pdata == nullptr) {
     if (trvs::currTask == 0) {
       trvs::logger.error("Particle data are uninitialised.");
       throw trvs::InvalidDataError("Particle data are uninitialised.\n");
     }
   }
 
@@ -366,24 +370,27 @@
         pos_max[iaxis] : this->pdata[pid].pos[iaxis];
     }
   }
 
   for (int iaxis = 0; iaxis < 3; iaxis++) {
     this->pos_min[iaxis] = pos_min[iaxis];
     this->pos_max[iaxis] = pos_max[iaxis];
+    this->pos_span[iaxis] = pos_max[iaxis] - pos_min[iaxis];
   }
 
   if (trvs::currTask == 0) {
     trvs::logger.info(
       "Extents of particle coordinates: "
-      "{'x': (%.3f, %.3f), 'y': (%.3f, %.3f), 'z': (%.3f, %.3f)} "
+      "{'x': (%.3f, %.3f | %.3f),"
+      " 'y': (%.3f, %.3f | %.3f),"
+      " 'z': (%.3f, %.3f | %.3f)} "
       "(source=%s).",
-      this->pos_min[0], this->pos_max[0],
-      this->pos_min[1], this->pos_max[1],
-      this->pos_min[2], this->pos_max[2],
+      this->pos_min[0], this->pos_max[0], this->pos_span[0],
+      this->pos_min[1], this->pos_max[1], this->pos_span[1],
+      this->pos_min[2], this->pos_max[2], this->pos_span[2],
       this->source.c_str()
     );
   }
 }
 
 
 // ***********************************************************************
@@ -403,15 +410,15 @@
 #endif  // TRV_USE_OMP
   for (int pid = 0; pid < this->ntotal; pid++) {
     for (int iaxis = 0; iaxis < 3; iaxis++) {
       this->pdata[pid].pos[iaxis] -= dpos[iaxis];
     }
   }
 
-  this->calc_pos_min_and_max();
+  this->calc_pos_extents();
 }
 
 void ParticleCatalogue::\
 offset_coords_for_periodicity(const double boxsize[3]) {
 #ifdef TRV_USE_OMP
 #pragma omp parallel for
 #endif  // TRV_USE_OMP
@@ -422,22 +429,22 @@
       } else
       if (this->pdata[pid].pos[iaxis] < 0.) {
         this->pdata[pid].pos[iaxis] += boxsize[iaxis];
       }
     }
   }
 
-  this->calc_pos_min_and_max();
+  this->calc_pos_extents();
 }
 
 void ParticleCatalogue::centre_in_box(
   ParticleCatalogue& catalogue,
   const double boxsize[3]
 ) {
-  catalogue.calc_pos_min_and_max();  // likely redundant but safe
+  catalogue.calc_pos_extents();  // likely redundant but safe
 
   double xmid = (catalogue.pos_min[0] + catalogue.pos_max[0]) / 2.;
   double ymid = (catalogue.pos_min[1] + catalogue.pos_max[1]) / 2.;
   double zmid = (catalogue.pos_min[2] + catalogue.pos_max[2]) / 2.;
 
   double dvec[3] = {
     xmid - boxsize[0]/2., ymid - boxsize[1]/2., zmid - boxsize[2]/2.
@@ -446,15 +453,15 @@
   catalogue.offset_coords(dvec);
 }
 
 void ParticleCatalogue::centre_in_box(
   ParticleCatalogue& catalogue, ParticleCatalogue& catalogue_ref,
   const double boxsize[3]
 ) {
-  catalogue_ref.calc_pos_min_and_max();  // likely redundant but safe
+  catalogue_ref.calc_pos_extents();  // likely redundant but safe
 
   double xmid = (catalogue_ref.pos_min[0] + catalogue_ref.pos_max[0]) / 2.;
   double ymid = (catalogue_ref.pos_min[1] + catalogue_ref.pos_max[1]) / 2.;
   double zmid = (catalogue_ref.pos_min[2] + catalogue_ref.pos_max[2]) / 2.;
 
   double dvec[3] = {
     xmid - boxsize[0]/2., ymid - boxsize[1]/2., zmid - boxsize[2]/2.
@@ -464,30 +471,30 @@
   catalogue.offset_coords(dvec);
 }
 
 void ParticleCatalogue::pad_in_box(
   ParticleCatalogue& catalogue,
   const double boxsize[3], const double boxsize_pad[3]
 ) {
-  catalogue.calc_pos_min_and_max();  // likely redundant but safe
+  catalogue.calc_pos_extents();  // likely redundant but safe
 
   double dvec[3] = {
     catalogue.pos_min[0] - boxsize_pad[0] * boxsize[0],
     catalogue.pos_min[1] - boxsize_pad[1] * boxsize[1],
     catalogue.pos_min[2] - boxsize_pad[2] * boxsize[2]
   };
 
   catalogue.offset_coords(dvec);
 }
 
 void ParticleCatalogue::pad_in_box(
     ParticleCatalogue& catalogue, ParticleCatalogue& catalogue_ref,
     const double boxsize[3], const double boxsize_pad[3]
 ) {
-  catalogue_ref.calc_pos_min_and_max();  // likely redundant but safe
+  catalogue_ref.calc_pos_extents();  // likely redundant but safe
 
   double dvec[3] = {
     catalogue_ref.pos_min[0] - boxsize_pad[0] * boxsize[0],
     catalogue_ref.pos_min[1] - boxsize_pad[1] * boxsize[1],
     catalogue_ref.pos_min[2] - boxsize_pad[2] * boxsize[2]
   };
 
@@ -495,15 +502,15 @@
   catalogue.offset_coords(dvec);
 }
 
 void ParticleCatalogue::pad_grids(
   ParticleCatalogue& catalogue,
   const double boxsize[3], const int ngrid[3], const double ngrid_pad[3]
 ) {
-  catalogue.calc_pos_min_and_max();  // likely redundant but safe
+  catalogue.calc_pos_extents();  // likely redundant but safe
 
   double dvec[3] = {
     catalogue.pos_min[0], catalogue.pos_min[1], catalogue.pos_min[2]
   };
 
   dvec[0] -= ngrid_pad[0] * boxsize[0] / double(ngrid[0]);
   dvec[1] -= ngrid_pad[1] * boxsize[1] / double(ngrid[1]);
@@ -512,15 +519,15 @@
   catalogue.offset_coords(dvec);
 }
 
 void ParticleCatalogue::pad_grids(
     ParticleCatalogue& catalogue, ParticleCatalogue& catalogue_ref,
     const double boxsize[3], const int ngrid[3], const double ngrid_pad[3]
 ) {
-  catalogue_ref.calc_pos_min_and_max();  // likely redundant but safe
+  catalogue_ref.calc_pos_extents();  // likely redundant but safe
 
   double dvec[3] = {
     catalogue_ref.pos_min[0] - ngrid_pad[0] * boxsize[0] / double(ngrid[0]),
     catalogue_ref.pos_min[1] - ngrid_pad[1] * boxsize[1] / double(ngrid[1]),
     catalogue_ref.pos_min[2] - ngrid_pad[2] * boxsize[2] / double(ngrid[2])
   };
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/threept.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/threept.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -62,29 +62,14 @@
 }
 
 
 // ***********************************************************************
 // Normalisation
 // ***********************************************************************
 
-double calc_bispec_normalisation_from_mesh(
-  ParticleCatalogue& particles, trv::ParameterSet& params, double alpha
-) {
-  MeshField catalogue_mesh(params);
-
-  double norm_factor =
-    catalogue_mesh.calc_grid_based_powlaw_norm(particles, 3);
-
-  catalogue_mesh.finalise_density_field();  // likely redundant but safe
-
-  norm_factor /= std::pow(alpha, 3);
-
-  return norm_factor;
-}
-
 double calc_bispec_normalisation_from_particles(
   ParticleCatalogue& particles, double alpha
 ) {
   if (particles.pdata == nullptr) {
     if (trvs::currTask == 0) {
       trvs::logger.error("Particle data are uninitialised.");
       throw trvs::InvalidDataError("Particle data are uninitialised.\n");
@@ -115,14 +100,29 @@
   }
 
   double norm_factor = 1. / (alpha * norm);  // 1/I₃
 
   return norm_factor;
 }
 
+double calc_bispec_normalisation_from_mesh(
+  ParticleCatalogue& particles, trv::ParameterSet& params, double alpha
+) {
+  MeshField catalogue_mesh(params);
+
+  double norm_factor =
+    catalogue_mesh.calc_grid_based_powlaw_norm(particles, 3);
+
+  catalogue_mesh.finalise_density_field();  // likely redundant but safe
+
+  norm_factor /= std::pow(alpha, 3);
+
+  return norm_factor;
+}
+
 
 // ***********************************************************************
 // Shot noise
 // ***********************************************************************
 
 std::complex<double> calc_ylm_wgtd_shotnoise_amp_for_bispec(
   ParticleCatalogue& particles_data, ParticleCatalogue& particles_rand,
@@ -233,15 +233,15 @@
   // ---------------------------------------------------------------------
   // Set-up
   // ---------------------------------------------------------------------
 
   // Set up/check input.
   validate_multipole_coupling(params);
 
-  double alpha = catalogue_data.wtotal / catalogue_rand.wtotal;
+  double alpha = catalogue_data.wstotal / catalogue_rand.wstotal;
 
   std::complex<double> parity = std::pow(trvm::M_I, params.ell1 + params.ell2);
 
   // Set up output.
   int* nmodes_save = new int[kbinning.num_bins];
   double* k1_save = new double[kbinning.num_bins];
   double* k2_save = new double[kbinning.num_bins];
@@ -554,15 +554,15 @@
   // ---------------------------------------------------------------------
   // Set-up
   // ---------------------------------------------------------------------
 
   // Set up/check input.
   validate_multipole_coupling(params);
 
-  double alpha = catalogue_data.wtotal / catalogue_rand.wtotal;
+  double alpha = catalogue_data.wstotal / catalogue_rand.wstotal;
 
   double parity = std::pow(-1, params.ell1 + params.ell2);
 
   // Set up output.
   int* npairs_save = new int[rbinning.num_bins];
   double* r1_save = new double[rbinning.num_bins];
   double* r2_save = new double[rbinning.num_bins];
@@ -1652,15 +1652,15 @@
   // ---------------------------------------------------------------------
   // Set-up
   // ---------------------------------------------------------------------
 
   // Set up/check input.
   validate_multipole_coupling(params);
 
-  double alpha = catalogue_data.wtotal / catalogue_rand.wtotal;
+  double alpha = catalogue_data.wstotal / catalogue_rand.wstotal;
 
   std::complex<double> parity = std::pow(trvm::M_I, params.ell1 + params.ell2);
 
   // Set up output.
   int* nmodes_save = new int[kbinning.num_bins];
   double* k1_save = new double[kbinning.num_bins];
   double* k2_save = new double[kbinning.num_bins];
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/src/modules/twopt.cpp` & `Triumvirate-0.2.0/src/triumvirate/src/twopt.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -47,29 +47,14 @@
 }
 
 
 // ***********************************************************************
 // Normalisation
 // ***********************************************************************
 
-double calc_powspec_normalisation_from_mesh(
-  trv::ParticleCatalogue& particles, trv::ParameterSet& params, double alpha
-) {
-  trv::MeshField catalogue_mesh(params);
-
-  double norm_factor =
-    catalogue_mesh.calc_grid_based_powlaw_norm(particles, 2);
-
-  catalogue_mesh.finalise_density_field();  // likely redundant but safe
-
-  norm_factor /= std::pow(alpha, 2);
-
-  return norm_factor;
-}
-
 double calc_powspec_normalisation_from_particles(
   ParticleCatalogue& particles, double alpha
 ) {
   if (particles.pdata == nullptr) {
     if (trvs::currTask == 0) {
       trvs::logger.error("Particle data are uninitialised.");
       throw trvs::InvalidDataError("Particle data are uninitialised.\n");
@@ -100,14 +85,129 @@
   }
 
   double norm_factor = 1. / (alpha * norm);  // 1/I₂
 
   return norm_factor;
 }
 
+double calc_powspec_normalisation_from_mesh(
+  trv::ParticleCatalogue& particles, trv::ParameterSet& params, double alpha
+) {
+  trv::MeshField catalogue_mesh(params);
+
+  double norm_factor =
+    catalogue_mesh.calc_grid_based_powlaw_norm(particles, 2);
+
+  catalogue_mesh.finalise_density_field();  // likely redundant but safe
+
+  norm_factor /= std::pow(alpha, 2);
+
+  return norm_factor;
+}
+
+double calc_powspec_normalisation_from_meshes(
+  trv::ParticleCatalogue& particles_data,
+  trv::ParticleCatalogue& particles_rand,
+  trv::ParameterSet& params, double alpha
+) {
+  // Assign particles to mesh.
+  trv::MeshField mesh_data(params);
+  trv::MeshField mesh_rand(params);
+
+  fftw_complex* weight_data = nullptr;
+  weight_data = fftw_alloc_complex(particles_data.ntotal);
+
+  fftw_complex* weight_rand = nullptr;
+  weight_rand = fftw_alloc_complex(particles_rand.ntotal);
+
+  trvs::gbytesMem += trvs::size_in_gb<fftw_complex>(particles_data.ntotal);
+  trvs::gbytesMem += trvs::size_in_gb<fftw_complex>(particles_rand.ntotal);
+  trv::sys::update_maxmem();
+
+#ifdef TRV_USE_OMP
+#pragma omp parallel for
+#endif  // TRV_USE_OMP
+  for (int pid = 0; pid < particles_data.ntotal; pid++) {
+    weight_data[pid][0] = particles_data[pid].w;
+    weight_data[pid][1] = 0.;
+  }
+
+#ifdef TRV_USE_OMP
+#pragma omp parallel for
+#endif  // TRV_USE_OMP
+  for (int pid = 0; pid < particles_rand.ntotal; pid++) {
+    weight_rand[pid][0] = particles_rand[pid].w;
+    weight_rand[pid][1] = 0.;
+  }
+
+  mesh_data.assign_weighted_field_to_mesh(particles_data, weight_data);
+  mesh_rand.assign_weighted_field_to_mesh(particles_rand, weight_rand);
+
+  fftw_free(weight_data); weight_data = nullptr;
+  fftw_free(weight_rand); weight_rand = nullptr;
+
+  trvs::gbytesMem -= trvs::size_in_gb<fftw_complex>(particles_data.ntotal);
+  trvs::gbytesMem -= trvs::size_in_gb<fftw_complex>(particles_rand.ntotal);
+
+  // Calculate normalisation.
+  double norm = 0.;
+
+#ifdef TRV_USE_OMP
+#pragma omp parallel for reduction(+:norm)
+#endif  // TRV_USE_OMP
+  for (int gid = 0; gid < params.nmesh; gid++) {
+    norm += mesh_data.field[gid][0] * mesh_rand.field[gid][0];
+  }
+
+  mesh_data.finalise_density_field();  // likely redundant but safe
+  mesh_rand.finalise_density_field();  // likely redundant but safe
+
+  double vol_cell = params.volume / double(params.nmesh);
+
+  double norm_factor = 1. / (alpha * vol_cell * norm);  // 1/I₂
+
+  return norm_factor;
+}
+
+double calc_powspec_normalisation_from_meshes(
+  trv::ParticleCatalogue& particles_data,
+  trv::ParticleCatalogue& particles_rand,
+  trv::ParameterSet& params, double alpha,
+  double padding, double cellsize, std::string assignment
+) {
+  // Modify parameter set for normalisation.
+  trv::ParameterSet params_norm(params);
+
+  double boxsize_norm = (1. + padding) * std::max(
+    *std::max_element(particles_data.pos_span, particles_data.pos_span + 3),
+    *std::max_element(particles_rand.pos_span, particles_rand.pos_span + 3)
+  );
+
+  int ngrid_norm = std::ceil(boxsize_norm / cellsize);
+
+  ngrid_norm += ngrid_norm % 2;  // ensure even
+  boxsize_norm = ngrid_norm * cellsize;  // enforce cell size
+
+  for (int iaxis = 0; iaxis < 3; iaxis++) {
+    params_norm.boxsize[iaxis] = boxsize_norm;
+    params_norm.ngrid[iaxis] = ngrid_norm;
+  }
+
+  params_norm.assignment = assignment;
+
+  params_norm.validate();
+
+  // Reuse existing overloaded method.
+  double norm_factor = calc_powspec_normalisation_from_meshes(
+    particles_data, particles_rand, params_norm, alpha
+  );
+
+  return norm_factor;
+}
+
 
 // ***********************************************************************
 // Shot noise
 // ***********************************************************************
 
 double calc_powspec_shotnoise_from_particles(
   ParticleCatalogue& particles, double alpha
@@ -237,15 +337,15 @@
   }
 
   // ---------------------------------------------------------------------
   // Set-up
   // ---------------------------------------------------------------------
 
   // Set up input.
-  double alpha = catalogue_data.wtotal / catalogue_rand.wtotal;
+  double alpha = catalogue_data.wstotal / catalogue_rand.wstotal;
   int ell1 = params.ELL;
 
   // Set up output.
   int* nmodes_save = new int[kbinning.num_bins];
   double* k_save = new double[kbinning.num_bins];
   std::complex<double>* pk_save = new std::complex<double>[kbinning.num_bins];
   std::complex<double>* sn_save = new std::complex<double>[kbinning.num_bins];
@@ -356,15 +456,15 @@
   }
 
   // ---------------------------------------------------------------------
   // Set-up
   // ---------------------------------------------------------------------
 
   // Set up input.
-  double alpha = catalogue_data.wtotal / catalogue_rand.wtotal;
+  double alpha = catalogue_data.wstotal / catalogue_rand.wstotal;
   int ell1 = params.ELL;
 
   // Set up output.
   int* npairs_save = new int[rbinning.num_bins];
   double* r_save = new double[rbinning.num_bins];
   std::complex<double>* xi_save = new std::complex<double>[rbinning.num_bins];
   for (int ibin = 0; ibin < rbinning.num_bins; ibin++) {
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/threept.py` & `Triumvirate-0.2.0/src/triumvirate/threept.py`

 * *Files 5% similar despite different names*

```diff
@@ -219,43 +219,46 @@
 
     raise ValueError(
         "`paramset` 'statistic_type' does not correspond to a "
         "recognised three-point statistic."
     )
 
 
-def _print_measurement_header(paramset, norm_factor, norm_factor_alt):
+def _print_measurement_header(paramset, norm_factor_part, norm_factor_mesh,
+                              norm_factor_meshes):
     """Print three-point statistic measurement header including
     sampling parameters, normalisation factors and data table columns.
 
     Parameters
     ----------
     paramset : :class:`~triumvirate.parameters.ParameterSet`
         Parameter set.
-    norm_factor, norm_factor_alt : float
-        Normalisation factor used and the alternative.
+    norm_factor_part, norm_factor_mesh, norm_factor_meshes : float
+        Normalisation factors.
 
     Returns
     -------
     text_header : str
         Measurement information as a header string.
 
     Raises
     ------
     ValueError
         When `paramset` indicates the measurements are not
         three-point statistics.
 
     """
+    if paramset['norm_convention'] == 'none':
+        norm_factor = 1.
     if paramset['norm_convention'] == 'particle':
-        norm_convention = 'particle'
-        norm_convention_alt = 'mesh'
+        norm_factor = norm_factor_part
     if paramset['norm_convention'] == 'mesh':
-        norm_convention = 'mesh'
-        norm_convention_alt = 'particle'
+        norm_factor = norm_factor_mesh
+    if paramset['norm_convention'] == 'mesh-mixed':
+        norm_factor = norm_factor_meshes
 
     if paramset['npoint'] != '3pt':
         raise ValueError(
             "`paramset` 'statistic_type' does not correspond to a "
             "recognised three-point statistic."
         )
 
@@ -274,28 +277,30 @@
             "Re{{zeta{}_raw}}".format(multipole),
             "Im{{zeta{}_raw}}".format(multipole),
             "Re{{zeta{}_shot}}".format(multipole),
             "Im{{zeta{}_shot}}".format(multipole)
         ]
 
     text_lines = [
-        "Box size: ({:.3f}, {:.3f}, {:.3f})".format(
+        "Box size: [{:.3f}, {:.3f}, {:.3f}]".format(
             *[paramset['boxsize'][ax] for ax in ['x', 'y', 'z']]
         ),
         "Box alignment: {}".format(paramset['alignment']),
-        "Mesh number: ({:d}, {:d}, {:d})".format(
+        "Mesh number: [{:d}, {:d}, {:d}]".format(
             *[paramset['ngrid'][ax] for ax in ['x', 'y', 'z']]
         ),
         "Mesh assignment and interlacing: {}, {}".format(
             paramset['assignment'], paramset['interlace']
         ),
-        "Normalisation factor: "
-        "{:.9e} ({}-based, used), {:.9e} ({}-based, alternative)".format(
-            norm_factor, norm_convention,
-            norm_factor_alt, norm_convention_alt
+        "Normalisation factor: {:.9e} ({})".format(
+            norm_factor, paramset['norm_convention']
+        ),
+        "Normalisation factor alternatives: "
+        "{:.9e} (particle), {:.9e} (mesh), {:.9e} (mesh-mixed; n/a)".format(
+            norm_factor_part, norm_factor_mesh, norm_factor_meshes
         ),
         ", ".join([
             "[{:d}] {}".format(colidx, colname)
             for colidx, colname in enumerate(datatab_colnames)
         ])
     ]
 
@@ -512,38 +517,56 @@
     if logger:
         logger.info(
             "... prepared catalogue for clustering algorithm.",
             cpp_state='end'
         )
 
     # Set up constants.
-    alpha = catalogue_data.wtotal / catalogue_rand.wtotal
+    alpha = catalogue_data.wstotal / catalogue_rand.wstotal
 
     if logger:
         logger.info("Alpha contrast: %.6e.", alpha)
 
-    if paramset['norm_convention'] == 'particle':
-        norm_factor = _calc_bispec_normalisation_from_particles(
-            particles_rand, alpha
+    norm_factor_part = _calc_bispec_normalisation_from_particles(
+        particles_rand, alpha
+    )
+    norm_factor_mesh = _calc_bispec_normalisation_from_mesh(
+        particles_rand, paramset, alpha
+    )
+    norm_factor_meshes = 0.
+
+    if paramset['norm_convention'] == 'none':
+        norm_factor = 1.
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; n/a) (none used)."
         )
-        norm_factor_alt = _calc_bispec_normalisation_from_mesh(
-            particles_rand, paramset, alpha
+    if paramset['norm_convention'] == 'particle':
+        norm_factor = norm_factor_part
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle; used), %.6e (mesh), %.6e (mesh-mixed; n/a)."
         )
     if paramset['norm_convention'] == 'mesh':
-        norm_factor = _calc_bispec_normalisation_from_mesh(
-            particles_rand, paramset, alpha
-        )
-        norm_factor_alt = _calc_bispec_normalisation_from_particles(
-            particles_rand, alpha
+        norm_factor = norm_factor_mesh
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh; used), %.6e (mesh-mixed; n/a)."
+        )
+    if paramset['norm_convention'] == 'mesh-mixed':
+        norm_factor = norm_factor_meshes
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; used)."
         )
 
     if logger:
         logger.info(
-            "Normalisation factors: %.6e (used), %.6e (alternative).",
-            norm_factor, norm_factor_alt
+            norm_log_mesg,
+            norm_factor_part, norm_factor_mesh, norm_factor_meshes
         )
 
     # Perform measurement.
     if logger:
         logger.info("Measuring clustering statistics...", cpp_state='start')
 
     results = threept_algofunc(
@@ -554,15 +577,18 @@
     if logger:
         logger.info("... measured clustering statistics.", cpp_state='end')
 
     if save:
         odirpath = paramset['directories']['measurements'] or ""
         header = "\n".join([
             catalogue_data.write_attrs_as_header(catalogue_ref=catalogue_rand),
-            _print_measurement_header(paramset, norm_factor, norm_factor_alt),
+            _print_measurement_header(
+                paramset,
+                norm_factor_part, norm_factor_mesh, norm_factor_meshes
+            ),
         ])
         if save.lower() == '.txt':
             datatab = _assemble_measurement_datatab(results, paramset)
             datafmt = '\t'.join(
                 ['%.9e'] * 4 + ['%10d'] + ['% .9e'] * (datatab.shape[-1] - 5)
             )
             ofilename = _get_measurement_filename(paramset)
@@ -953,39 +979,57 @@
 #     if logger:
 #         logger.info(
 #             "... prepared catalogue for clustering algorithm.",
 #             cpp_state='end'
 #         )
 
 #     # Set up constants.
-#     alpha = catalogue_data.wtotal / catalogue_rand.wtotal
+#     alpha = catalogue_data.wstotal / catalogue_rand.wstotal
 
 #     if logger:
 #         logger.info("Alpha contrast: %.6e.", alpha)
 
-#     if paramset['norm_convention'] == 'particle':
-#         norm_factor = _calc_bispec_normalisation_from_particles(
-#             particles_rand, alpha
+#     norm_factor_part = _calc_bispec_normalisation_from_particles(
+#         particles_rand, alpha
+#     )
+#     norm_factor_mesh = _calc_bispec_normalisation_from_mesh(
+#         particles_rand, paramset, alpha
+#     )
+#     norm_factor_meshes = 0.
+
+#     if paramset['norm_convention'] == 'none':
+#         norm_factor = 1.
+#         norm_log_mesg = (
+#             "Normalisation factors: "
+#             "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; n/a) (none used)."  # noqa: E501
 #         )
-#         norm_factor_alt = _calc_bispec_normalisation_from_mesh(
-#             particles_rand, paramset, alpha
+#     if paramset['norm_convention'] == 'particle':
+#         norm_factor = norm_factor_part
+#         norm_log_mesg = (
+#             "Normalisation factors: "
+#             "%.6e (particle; used), %.6e (mesh), %.6e (mesh-mixed; n/a)."
 #         )
 #     if paramset['norm_convention'] == 'mesh':
-#         norm_factor = _calc_bispec_normalisation_from_mesh(
-#             particles_rand, paramset, alpha
+#         norm_factor = norm_factor_mesh
+#         norm_log_mesg = (
+#             "Normalisation factors: "
+#             "%.6e (particle), %.6e (mesh; used), %.6e (mesh-mixed; n/a)."
 #         )
-#         norm_factor_alt = _calc_bispec_normalisation_from_particles(
-#             particles_rand, alpha
+#     if paramset['norm_convention'] == 'mesh-mixed':
+#         norm_factor = norm_factor_meshes
+#         norm_log_mesg = (
+#             "Normalisation factors: "
+#             "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; used)."
 #         )
 
 #     if logger:
 #         logger.info(
-#             "Normalisation factors: %.6e (used), %.6e (alternative).",
-#             norm_factor, norm_factor_alt
-#         )
+#             norm_log_mesg,
+#             norm_factor_part, norm_factor_mesh, norm_factor_meshes
+#     )
 
 #     # Perform measurement.
 #     if logger:
 #         logger.info("Measuring clustering statistics...", cpp_state='start')
 
 #     results = _compute_bispec_for_los_choice(
 #         particles_data, particles_rand, los_data, los_rand, los_choice,
@@ -995,15 +1039,18 @@
 #     if logger:
 #         logger.info("... measured clustering statistics.", cpp_state='end')
 
 #     if save:
 #         odirpath = paramset['directories']['measurements'] or ""
 #         header = "\n".join([
 #             catalogue_data.write_attrs_as_header(catalogue_ref=catalogue_rand),  # noqa: E501
-#             _print_measurement_header(paramset, norm_factor, norm_factor_alt),  # noqa: E501
+#             _print_measurement_header(
+#                 paramset,
+#                 norm_factor_part, norm_factor_mesh, norm_factor_meshes
+#             ),
 #         ])
 #         if save.lower() == '.txt':
 #             datatab = _assemble_measurement_datatab(results, paramset)
 #             datafmt = '\t'.join(
 #                 ['%.9e'] * 4 + ['%10d'] + ['% .9e'] * (datatab.shape[-1] - 5)
 #             )
 #             ofilename = _get_measurement_filename(paramset)
@@ -1159,33 +1206,45 @@
     if logger:
         logger.info(
             "... prepared catalogue for clustering algorithm.",
             cpp_state='end'
         )
 
     # Set up constants.
-    if paramset['norm_convention'] == 'particle':
-        norm_factor = _calc_bispec_normalisation_from_particles(
-            particles_data, alpha=1.
+    norm_factor_part = _calc_bispec_normalisation_from_particles(
+        particles_data, alpha=1.
+    )
+    norm_factor_mesh = _calc_bispec_normalisation_from_mesh(
+        particles_data, paramset, alpha=1.
+    )
+    norm_factor_meshes = 0.
+
+    if paramset['norm_convention'] == 'none':
+        norm_factor = 1.
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; n/a) (none used)."
         )
-        norm_factor_alt = _calc_bispec_normalisation_from_mesh(
-            particles_data, paramset, alpha=1.
+    if paramset['norm_convention'] == 'particle':
+        norm_factor = norm_factor_part
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle; used), %.6e (mesh), %.6e (mesh-mixed; n/a)."
         )
     if paramset['norm_convention'] == 'mesh':
-        norm_factor = _calc_bispec_normalisation_from_mesh(
-            particles_data, paramset, alpha=1.
-        )
-        norm_factor_alt = _calc_bispec_normalisation_from_particles(
-            particles_data, alpha=1.
+        norm_factor = norm_factor_mesh
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh; used), %.6e (mesh-mixed; n/a)."
         )
 
     if logger:
         logger.info(
-            "Normalisation factors: %.6e (used), %.6e (alternative).",
-            norm_factor, norm_factor_alt
+            norm_log_mesg,
+            norm_factor_part, norm_factor_mesh, norm_factor_meshes
         )
 
     # Perform measurement.
     if logger:
         logger.info("Measuring clustering statistics...", cpp_state='start')
 
     results = threept_algofunc(particles_data, paramset, binning, norm_factor)
@@ -1193,15 +1252,18 @@
     if logger:
         logger.info("... measured clustering statistics.", cpp_state='end')
 
     if save:
         odirpath = paramset['directories']['measurements'] or ""
         header = "\n".join([
             catalogue_data.write_attrs_as_header(),
-            _print_measurement_header(paramset, norm_factor, norm_factor_alt),
+            _print_measurement_header(
+                paramset,
+                norm_factor_part, norm_factor_mesh, norm_factor_meshes
+            ),
         ])
         if save.lower() == '.txt':
             datatab = _assemble_measurement_datatab(results, paramset)
             datafmt = '\t'.join(
                 ['%.9e'] * 4 + ['%10d'] + ['% .9e'] * (datatab.shape[-1] - 5)
             )
             ofilename = _get_measurement_filename(paramset)
@@ -1543,33 +1605,45 @@
     # --------------------------------------------------------------------
 
     # Prepare catalogues.
     particles_rand = \
         catalogue_rand._convert_to_cpp_catalogue(verbose=paramset['verbose'])
 
     # Set up constants.
-    if paramset['norm_convention'] == 'particle':
-        norm_factor = _calc_bispec_normalisation_from_particles(
-            particles_rand, alpha=1.
+    norm_factor_part = _calc_bispec_normalisation_from_particles(
+        particles_rand, alpha=1.
+    )
+    norm_factor_mesh = _calc_bispec_normalisation_from_mesh(
+        particles_rand, paramset, alpha=1.
+    )
+    norm_factor_meshes = 0.
+
+    if paramset['norm_convention'] == 'none':
+        norm_factor = 1.
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; n/a) (none used)."
         )
-        norm_factor_alt = _calc_bispec_normalisation_from_mesh(
-            particles_rand, paramset, alpha=1.
+    if paramset['norm_convention'] == 'particle':
+        norm_factor = norm_factor_part
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle; used), %.6e (mesh), %.6e (mesh-mixed; n/a)."
         )
     if paramset['norm_convention'] == 'mesh':
-        norm_factor = _calc_bispec_normalisation_from_mesh(
-            particles_rand, paramset, alpha=1.
-        )
-        norm_factor_alt = _calc_bispec_normalisation_from_particles(
-            particles_rand, alpha=1.
+        norm_factor = norm_factor_mesh
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh; used), %.6e (mesh-mixed; n/a)."
         )
 
     if logger:
         logger.info(
-            "Normalisation factors: %.6e (used), %.6e (alternative).",
-            norm_factor, norm_factor_alt
+            norm_log_mesg,
+            norm_factor_part, norm_factor_mesh, norm_factor_meshes
         )
 
     # Perform measurement.
     if logger:
         logger.info(
             "Measuring window function statistics...", cpp_state='start'
         )
@@ -1585,15 +1659,18 @@
             "... measured window function statistics.", cpp_state='end'
         )
 
     if save:
         odirpath = paramset['directories']['measurements'] or ""
         header = "\n".join([
             catalogue_rand.write_attrs_as_header(),
-            _print_measurement_header(paramset, norm_factor, norm_factor_alt),
+            _print_measurement_header(
+                paramset,
+                norm_factor_part, norm_factor_mesh, norm_factor_meshes
+            ),
         ])
         if save.lower() == '.txt':
             datatab = _assemble_measurement_datatab(results, paramset)
             datafmt = '\t'.join(
                 ['%.9e'] * 4 + ['%10d'] + ['% .9e'] * (datatab.shape[-1] - 5)
             )
             ofilename = _get_measurement_filename(paramset)
```

### Comparing `Triumvirate-0.1.2/src/triumvirate/twopt.py` & `Triumvirate-0.2.0/src/triumvirate/twopt.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import warnings
 from pathlib import Path
 
 import numpy as np
 
 from triumvirate._twopt import (
     _calc_powspec_normalisation_from_mesh,
+    _calc_powspec_normalisation_from_meshes,
     _calc_powspec_normalisation_from_particles,
     _compute_corrfunc,
     _compute_corrfunc_in_gpp_box,
     _compute_corrfunc_window,
     _compute_powspec,
     _compute_powspec_in_gpp_box,
 )
@@ -44,14 +45,20 @@
     _modify_measurement_parameters,
     _modify_sampling_parameters,
     fetch_paramset_template,
     ParameterSet,
 )
 
 
+# Use default parameters for mixed-mesh normalisation in `pypower`.
+PADDING = .10
+CELLSIZE = 10.
+ASSIGNMENT = 'cic'
+
+
 def _amalgamate_parameters(paramset=None, params_sampling=None,
                            degree=None, binning=None, **type_kwargs):
     """Amalgamate a parameter set with overriding sampling parameters
     and the measured multipole degree and coordinate binning.
 
     Parameters
     ----------
@@ -176,43 +183,46 @@
 
     raise ValueError(
         "`paramset` 'statistic_type' does not correspond to a "
         "recognised two-point statistic."
     )
 
 
-def _print_measurement_header(paramset, norm_factor, norm_factor_alt):
+def _print_measurement_header(paramset, norm_factor_part, norm_factor_mesh,
+                              norm_factor_meshes):
     """Print two-point statistic measurement header including
     sampling parameters, normalisation factors and data table columns.
 
     Parameters
     ----------
     paramset : :class:`~triumvirate.parameters.ParameterSet`
         Parameter set.
-    norm_factor, norm_factor_alt : double
-        Normalisation factor used and the alternative.
+    norm_factor_part, norm_factor_mesh, norm_factor_meshes : float
+        Normalisation factors.
 
     Returns
     -------
     text_header : str
         Measurement information as a header string.
 
     Raises
     ------
     ValueError
         When `paramset` indicates the measurements are not
         two-point statistics.
 
     """
+    if paramset['norm_convention'] == 'none':
+        norm_factor = 1.
     if paramset['norm_convention'] == 'particle':
-        norm_convention = 'particle'
-        norm_convention_alt = 'mesh'
+        norm_factor = norm_factor_part
     if paramset['norm_convention'] == 'mesh':
-        norm_convention = 'mesh'
-        norm_convention_alt = 'particle'
+        norm_factor = norm_factor_mesh
+    if paramset['norm_convention'] == 'mesh-mixed':
+        norm_factor = norm_factor_meshes
 
     if paramset['npoint'] != '2pt':
         raise ValueError(
             "`paramset` 'statistic_type' does not correspond to a "
             "recognised two-point statistic."
         )
     if paramset['space'] == 'fourier':
@@ -227,28 +237,30 @@
         datatab_colnames = [
             "r_cen", "r_eff", "npairs",
             "Re{{xi{:d}}}".format(paramset['degrees']['ELL']),
             "Im{{xi{:d}}}".format(paramset['degrees']['ELL'])
         ]
 
     text_lines = [
-        "Box size: ({:.3f}, {:.3f}, {:.3f})".format(
+        "Box size: [{:.3f}, {:.3f}, {:.3f}]".format(
             *[paramset['boxsize'][ax] for ax in ['x', 'y', 'z']]
         ),
         "Box alignment: {}".format(paramset['alignment']),
-        "Mesh number: ({:d}, {:d}, {:d})".format(
+        "Mesh number: [{:d}, {:d}, {:d}]".format(
             *[paramset['ngrid'][ax] for ax in ['x', 'y', 'z']]
         ),
         "Mesh assignment and interlacing: {}, {}".format(
             paramset['assignment'], paramset['interlace']
         ),
-        "Normalisation factor: "
-        "{:.9e} ({}-based, used), {:.9e} ({}-based, alternative)".format(
-            norm_factor, norm_convention,
-            norm_factor_alt, norm_convention_alt
+        "Normalisation factor: {:.9e} ({})".format(
+            norm_factor, paramset['norm_convention']
+        ),
+        "Normalisation factor alternatives: "
+        "{:.9e} (particle), {:.9e} (mesh), {:.9e} (mesh-mixed)".format(
+            norm_factor_part, norm_factor_mesh, norm_factor_meshes
         ),
         ", ".join([
             "[{:d}] {}".format(colidx, colname)
             for colidx, colname in enumerate(datatab_colnames)
         ])
     ]
 
@@ -454,38 +466,59 @@
     if logger:
         logger.info(
             "... prepared catalogue for clustering algorithm.",
             cpp_state='end'
         )
 
     # Set up constants.
-    alpha = catalogue_data.wtotal / catalogue_rand.wtotal
+    alpha = catalogue_data.wstotal / catalogue_rand.wstotal
 
     if logger:
         logger.info("Alpha contrast: %.6e.", alpha)
 
-    if paramset['norm_convention'] == 'particle':
-        norm_factor = _calc_powspec_normalisation_from_particles(
-            particles_rand, alpha
+    norm_factor_part = _calc_powspec_normalisation_from_particles(
+        particles_rand, alpha
+    )
+    norm_factor_mesh = _calc_powspec_normalisation_from_mesh(
+        particles_rand, paramset, alpha
+    )
+    norm_factor_meshes = _calc_powspec_normalisation_from_meshes(
+        particles_data, particles_rand, paramset, alpha,
+        padding=PADDING, cellsize=CELLSIZE, assignment=ASSIGNMENT
+    )
+
+    if paramset['norm_convention'] == 'none':
+        norm_factor = 1.
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed) (none used)."
         )
-        norm_factor_alt = _calc_powspec_normalisation_from_mesh(
-            particles_rand, paramset, alpha
+    if paramset['norm_convention'] == 'particle':
+        norm_factor = norm_factor_part
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle; used), %.6e (mesh), %.6e (mesh-mixed)."
         )
     if paramset['norm_convention'] == 'mesh':
-        norm_factor = _calc_powspec_normalisation_from_mesh(
-            particles_rand, paramset, alpha
-        )
-        norm_factor_alt = _calc_powspec_normalisation_from_particles(
-            particles_rand, alpha
+        norm_factor = norm_factor_mesh
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh; used), %.6e (mesh-mixed)."
+        )
+    if paramset['norm_convention'] == 'mesh-mixed':
+        norm_factor = norm_factor_meshes
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; used)."
         )
 
     if logger:
         logger.info(
-            "Normalisation factors: %.6e (used), %.6e (alternative).",
-            norm_factor, norm_factor_alt
+            norm_log_mesg,
+            norm_factor_part, norm_factor_mesh, norm_factor_meshes
         )
 
     # Perform measurement.
     if logger:
         logger.info("Measuring clustering statistics...", cpp_state='start')
 
     results = twopt_algofunc(
@@ -496,15 +529,18 @@
     if logger:
         logger.info("... measured clustering statistics.", cpp_state='end')
 
     if save:
         odirpath = paramset['directories']['measurements'] or ""
         header = "\n".join([
             catalogue_data.write_attrs_as_header(catalogue_ref=catalogue_rand),
-            _print_measurement_header(paramset, norm_factor, norm_factor_alt),
+            _print_measurement_header(
+                paramset,
+                norm_factor_part, norm_factor_mesh, norm_factor_meshes
+            ),
         ])
         if save.lower() == '.txt':
             datatab = _assemble_measurement_datatab(results, paramset)
             datafmt = '\t'.join(
                 ['%.9e'] * 2 + ['%10d'] + ['% .9e'] * (datatab.shape[-1] - 3)
             )
             ofilename = _get_measurement_filename(paramset)
@@ -871,33 +907,45 @@
     if logger:
         logger.info(
             "... prepared catalogue for clustering algorithm.",
             cpp_state='end'
         )
 
     # Set up constants.
-    if paramset['norm_convention'] == 'particle':
-        norm_factor = _calc_powspec_normalisation_from_particles(
-            particles_data, alpha=1.
+    norm_factor_part = _calc_powspec_normalisation_from_particles(
+        particles_data, alpha=1.
+    )
+    norm_factor_mesh = _calc_powspec_normalisation_from_mesh(
+        particles_data, paramset, alpha=1.
+    )
+    norm_factor_meshes = 0.
+
+    if paramset['norm_convention'] == 'none':
+        norm_factor = 1.
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; n/a) (none used)."
         )
-        norm_factor_alt = _calc_powspec_normalisation_from_mesh(
-            particles_data, paramset, alpha=1.
+    if paramset['norm_convention'] == 'particle':
+        norm_factor = norm_factor_part
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle; used), %.6e (mesh), %.6e (mesh-mixed; n/a)."
         )
     if paramset['norm_convention'] == 'mesh':
-        norm_factor = _calc_powspec_normalisation_from_mesh(
-            particles_data, paramset, alpha=1.
-        )
-        norm_factor_alt = _calc_powspec_normalisation_from_particles(
-            particles_data, alpha=1.
+        norm_factor = norm_factor_mesh
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh; used), %.6e (mesh-mixed; n/a)."
         )
 
     if logger:
         logger.info(
-            "Normalisation factors: %.6e (used), %.6e (alternative).",
-            norm_factor, norm_factor_alt
+            norm_log_mesg,
+            norm_factor_part, norm_factor_mesh, norm_factor_meshes
         )
 
     # Perform measurement.
     if logger:
         logger.info("Measuring clustering statistics...", cpp_state='start')
 
     results = twopt_algofunc(particles_data, paramset, binning, norm_factor)
@@ -905,15 +953,18 @@
     if logger:
         logger.info("... measured clustering statistics.", cpp_state='end')
 
     if save:
         odirpath = paramset['directories']['measurements'] or ""
         header = "\n".join([
             catalogue_data.write_attrs_as_header(),
-            _print_measurement_header(paramset, norm_factor, norm_factor_alt),
+            _print_measurement_header(
+                paramset,
+                norm_factor_part, norm_factor_mesh, norm_factor_meshes
+            ),
         ])
         if save.lower() == '.txt':
             datatab = _assemble_measurement_datatab(results, paramset)
             datafmt = '\t'.join(
                 ['%.9e'] * 2 + ['%10d'] + ['% .9e'] * (datatab.shape[-1] - 3)
             )
             ofilename = _get_measurement_filename(paramset)
@@ -1227,33 +1278,45 @@
     # --------------------------------------------------------------------
 
     # Prepare catalogues.
     particles_rand =  \
         catalogue_rand._convert_to_cpp_catalogue(verbose=paramset['verbose'])
 
     # Set up constants.
-    if paramset['norm_convention'] == 'particle':
-        norm_factor = _calc_powspec_normalisation_from_particles(
-            particles_rand, alpha=1.
+    norm_factor_part = _calc_powspec_normalisation_from_particles(
+        particles_rand, alpha=1.
+    )
+    norm_factor_mesh = _calc_powspec_normalisation_from_mesh(
+        particles_rand, paramset, alpha=1.
+    )
+    norm_factor_meshes = 0.
+
+    if paramset['norm_convention'] == 'none':
+        norm_factor = 1.
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh), %.6e (mesh-mixed; n/a) (none used)."
         )
-        norm_factor_alt = _calc_powspec_normalisation_from_mesh(
-            particles_rand, paramset, alpha=1.
+    if paramset['norm_convention'] == 'particle':
+        norm_factor = norm_factor_part
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle; used), %.6e (mesh), %.6e (mesh-mixed; n/a)."
         )
     if paramset['norm_convention'] == 'mesh':
-        norm_factor = _calc_powspec_normalisation_from_mesh(
-            particles_rand, paramset, alpha=1.
-        )
-        norm_factor_alt = _calc_powspec_normalisation_from_particles(
-            particles_rand, alpha=1.
+        norm_factor = norm_factor_mesh
+        norm_log_mesg = (
+            "Normalisation factors: "
+            "%.6e (particle), %.6e (mesh; used), %.6e (mesh-mixed; n/a)."
         )
 
     if logger:
         logger.info(
-            "Normalisation factors: %.6e (used), %.6e (alternative).",
-            norm_factor, norm_factor_alt
+            norm_log_mesg,
+            norm_factor_part, norm_factor_mesh, norm_factor_meshes
         )
 
     # Perform measurement.
     if logger:
         logger.info(
             "Measuring window function statistics...", cpp_state='start'
         )
@@ -1268,15 +1331,18 @@
             "... measured window function statistics.", cpp_state='end'
         )
 
     if save:
         odirpath = paramset['directories']['measurements']
         header = "\n".join([
             catalogue_rand.write_attrs_as_header(),
-            _print_measurement_header(paramset, norm_factor, norm_factor_alt),
+            _print_measurement_header(
+                paramset,
+                norm_factor_part, norm_factor_mesh, norm_factor_meshes
+            ),
         ])
         if save.lower() == '.txt':
             datatab = _assemble_measurement_datatab(results, paramset)
             datafmt = '\t'.join(
                 ['%.9e'] * 2 + ['%10d'] + ['% .9e'] * (datatab.shape[-1] - 3)
             )
             ofilename = _get_measurement_filename(paramset)
```

### Comparing `Triumvirate-0.1.2/tests/conftest.py` & `Triumvirate-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_catalogue.py` & `Triumvirate-0.2.0/tests/test_catalogue.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,16 +319,20 @@
     )
 
     if ref_catalogue is None:
         assert (
             "Catalogue source: {}".format(minimal_catalogue._source)
         ) in header
         assert (
-            "Catalogue size: {:d} particles of total sample weight {:.3f}"
-            .format(minimal_catalogue.ntotal, minimal_catalogue.wtotal)
+            "Catalogue size: ntotal = {:d}, wtotal = {:.3f}, wstotal = {:.3f}"
+            .format(
+                minimal_catalogue.ntotal,
+                minimal_catalogue.wtotal,
+                minimal_catalogue.wstotal,
+            )
         ) in header
         assert (
             "Catalogue particle extents: "
             "([{:.3f}, {:.3f}], [{:.3f}, {:.3f}], [{:.3f}, {:.3f}])"
             .format(
                 *minimal_catalogue.bounds['x'],
                 *minimal_catalogue.bounds['y'],
@@ -341,16 +345,19 @@
         ):
             assert (
                 "{} catalogue source: {}"
                 .format(_source_type, _catalogue._source)
             ) in header
             assert (
                 "{} catalogue size: "
-                "{:d} particles of total sample weight {:.3f}"
-                .format(_source_type, _catalogue.ntotal, _catalogue.wtotal)
+                "ntotal = {:d}, wtotal = {:.3f}, wstotal = {:.3f}"
+                .format(
+                    _source_type,
+                    _catalogue.ntotal, _catalogue.wtotal, _catalogue.wstotal,
+                )
             ) in header
             assert (
                 "{}-source particle extents: "
                 "([{:.3f}, {:.3f}], [{:.3f}, {:.3f}], [{:.3f}, {:.3f}])"
                 .format(
                     _source_type,
                     *_catalogue.bounds['x'],
```

### Comparing `Triumvirate-0.1.2/tests/test_dataobjs.py` & `Triumvirate-0.2.0/tests/test_dataobjs.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.fits` & `Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.fits`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.h5` & `Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.h5`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/ctlgs/test_rand_catalogue.txt` & `Triumvirate-0.2.0/tests/test_input/ctlgs/test_rand_catalogue.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/params/test_params.ini` & `Triumvirate-0.2.0/tests/test_input/params/test_params.ini`

 * *Files 11% similar despite different names*

```diff
@@ -65,15 +65,18 @@
 # Orders of wide-angle corrections.
 i_wa =
 j_wa =
 
 # Form of three-point statistic measurements: {'full', 'diag' (default)}.
 form =
 
-# Normalisation convention: {'particle' (default), 'mesh'}.
+# Normalisation convention: {
+#   'none', 'particle' (default), 'mesh',
+#   'mesh-mixed' (two-point statistics only)
+# }.
 norm_convention = particle
 
 # Binning scheme: {'lin' (default), 'log', 'linpad', 'logpad', 'custom'}.
 binning = lin
 
 # Minimum and maximum of the range of measurement scales.
 # The bin coordinate is either wavenumbers (in h/Mpc) in Fourier space,
```

### Comparing `Triumvirate-0.1.2/tests/test_input/params/test_params.yml` & `Triumvirate-0.2.0/tests/test_input/params/test_params.yml`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,18 @@
 wa_orders:
   i:
   j:
 
 # Form of the three-point statistic measurements: {'full', 'diag' (default)}.
 form: diag
 
-# Normalisation convention: {'particle' (default), 'mesh'}.
+# Normalisation convention: {
+#   'none', 'particle' (default), 'mesh',
+#   'mesh-mixed' (two-point statistics only)
+# }.
 norm_convention: particle
 
 # Binning scheme: {'lin' (default), 'log', 'linpad', 'logpad', 'custom'}.
 binning: lin
 
 # Minimum and maximum of the binning range (i.e. range of measurement scales)
 # as a list.
```

### Comparing `Triumvirate-0.1.2/tests/test_input/params/tmpl_params.yml` & `Triumvirate-0.2.0/src/triumvirate/resources/params_template.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# This is a copy of ``src/triumvirate/resources/params_template.yml".
 ---
 
 # -- I/O -----------------------------------------------------------------
 
 # Directories for input/output.
 # The paths can be either absolute or relative to the working directory.
 # If unset, the current working directory is assumed.
@@ -70,15 +69,18 @@
 wa_orders:
   i:
   j:
 
 # Form of three-point statistic measurements: {'full', 'diag' (default)}.
 form: diag
 
-# Normalisation convention: {'particle' (default), 'mesh'}.
+# Normalisation convention: {
+#   'none', 'particle' (default), 'mesh',
+#   'mesh-mixed' (two-point statistics only)
+# }.
 norm_convention: particle
 
 # Binning scheme: {'lin' (default), 'log', 'linpad', 'logpad', 'custom'}.
 binning: lin
 
 # Minimum and maximum of the binning range (i.e. range of measurement scales)
 # as a list.
```

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/bk000_bin0_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/bk000_bin0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/bk000_bin0_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/bk000_bin0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/bk000_diag_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/bk000_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/bk000_diag_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/bk000_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/bk202_diag_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/bk202_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/bk202_diag_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/bk202_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/pk0_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/pk0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/pk0_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/pk0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/pk2_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/pk2_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/pk2_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/pk2_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/xi0_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/xi0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/xi0_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/xi0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/xi2_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/xi2_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/xi2_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/xi2_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/xiw0.txt` & `Triumvirate-0.2.0/tests/test_input/stats/xiw0.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/xiw2.txt` & `Triumvirate-0.2.0/tests/test_input/stats/xiw2.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zeta000_bin0_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zeta000_bin0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zeta000_bin0_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zeta000_bin0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zeta000_diag_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zeta000_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zeta000_diag_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zeta000_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zeta202_diag_gpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zeta202_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zeta202_diag_lpp.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zeta202_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zetaw000_bin0.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zetaw000_bin0.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zetaw000_diag.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zetaw000_diag.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_input/stats/zetaw202_diag.txt` & `Triumvirate-0.2.0/tests/test_input/stats/zetaw202_diag.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_logger.py` & `Triumvirate-0.2.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_parameters.py` & `Triumvirate-0.2.0/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_threept.py` & `Triumvirate-0.2.0/tests/test_threept.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.2/tests/test_twopt.py` & `Triumvirate-0.2.0/tests/test_twopt.py`

 * *Files identical despite different names*

