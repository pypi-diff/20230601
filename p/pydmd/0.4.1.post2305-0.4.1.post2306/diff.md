# Comparing `tmp/pydmd-0.4.1.post2305.tar.gz` & `tmp/pydmd-0.4.1.post2306.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmd-0.4.1.post2305.tar", last modified: Mon May  1 02:59:59 2023, max compression
+gzip compressed data, was "pydmd-0.4.1.post2306.tar", last modified: Thu Jun  1 03:29:13 2023, max compression
```

## Comparing `pydmd-0.4.1.post2305.tar` & `pydmd-0.4.1.post2306.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:59:59.475438 pydmd-0.4.1.post2305/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-01 02:59:59.475438 pydmd-0.4.1.post2305/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:59:59.471438 pydmd-0.4.1.post2305/pydmd/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42614 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/bopdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/cdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmd_modes_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmdbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmdc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmdoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/fbdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/hankeldmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/havok.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/hodmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/mrdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/optdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/paramdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/pidmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/pidmd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/rdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/spdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/subspacedmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:59:59.471438 pydmd-0.4.1.post2305/pydmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 02:59:59.475438 pydmd-0.4.1.post2305/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:59:59.475438 pydmd-0.4.1.post2305/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_bopdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_cdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmd_modes_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmdbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmdoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_fbdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_hankeldmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_havok.py
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_hodmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_mrdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_optdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_paramdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_pidmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_rdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_spdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_subspacedmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:29:13.065699 pydmd-0.4.1.post2306/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-01 03:29:13.065699 pydmd-0.4.1.post2306/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:29:13.061699 pydmd-0.4.1.post2306/pydmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42597 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/bopdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/cdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmd_modes_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmdbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmdoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/fbdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/hankeldmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/havok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/hodmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/mrdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/optdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/paramdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/pidmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/pidmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/rdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/spdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/subspacedmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:29:13.061699 pydmd-0.4.1.post2306/pydmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:29:12.000000 pydmd-0.4.1.post2306/pydmd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:29:13.065699 pydmd-0.4.1.post2306/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:29:13.065699 pydmd-0.4.1.post2306/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_bopdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_cdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmd_modes_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmdbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmdoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_fbdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_hankeldmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_havok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_hodmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_mrdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_optdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_paramdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_pidmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_rdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_spdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_subspacedmd.py
```

### Comparing `pydmd-0.4.1.post2305/LICENSE.rst` & `pydmd-0.4.1.post2306/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/PKG-INFO` & `pydmd-0.4.1.post2306/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmd
-Version: 0.4.1.post2305
+Version: 0.4.1.post2306
 Summary: Python Dynamic Mode Decomposition.
 Home-page: https://github.com/mathLab/PyDMD
 Author: Nicola Demo, Marco Tezzele, Francesco Andreuzzi, Sara Ichinaga
 Author-email: pydmd.info@gmail.com
 License: MIT
 Keywords: dynamic-mode-decomposition dmd
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydmd-0.4.1.post2305/README.md` & `pydmd-0.4.1.post2306/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
     <img alt="Python Dynamic Mode Decomposition" src="readme/logo_PyDMD.png" width="200" />
   </a>
 </p>
 <p align="center">
     <a href="https://doi.org/10.21105/joss.00530" target="_blank">
         <img alt="JOSS DOI" src="http://joss.theoj.org/papers/10.21105/joss.00530/status.svg">
     </a>
-    <a href="https://github.com/mathLab/PyDMD/blob/master/LICENSE" target="_blank">
+    <a href="https://github.com/PyDMD/PyDMD/blob/master/LICENSE" target="_blank">
         <img alt="Software License" src="https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square">
     </a>
     <a href="https://badge.fury.io/py/pydmd"  target="_blank">
         <img alt="PyPI version" src="https://badge.fury.io/py/pydmd.svg">
     </a>
-    <a href="https://github.com/mathLab/PyDMD/actions/workflows/deploy_after_push.yml" target="_blank">
-        <img alt="CI Status" src="https://github.com/mathLab/PyDMD/actions/workflows/deploy_after_push.yml/badge.svg">
+    <a href="https://github.com/PyDMD/PyDMD/actions/workflows/deploy_after_push.yml" target="_blank">
+        <img alt="CI Status" src="https://github.com/PyDMD/PyDMD/actions/workflows/deploy_after_push.yml/badge.svg">
     </a>
     <a href="https://www.codacy.com/gh/mathLab/PyDMD/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mathLab/PyDMD&amp;utm_campaign=Badge_Coverage">
       <img src="https://app.codacy.com/project/badge/Coverage/c36adbea2e4a44eb8c0e4505b75e8245"/>
     </a>
     <a href="https://www.codacy.com/gh/mathLab/PyDMD/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mathLab/PyDMD&amp;utm_campaign=Badge_Grade">
       <img src="https://app.codacy.com/project/badge/Grade/c36adbea2e4a44eb8c0e4505b75e8245"/>
     </a>
@@ -69,41 +69,41 @@
 ```bash
 > pip uninstall pydmd
 ```
 
 ### Installing from source
 The official distribution is on GitHub, and you can clone the repository using
 ```bash
-> git clone https://github.com/mathLab/PyDMD
+> git clone https://github.com/PyDMD/PyDMD
 ```
 
 To install the package just type:
 ```bash
 > pip install -e .
 ```
 
 To uninstall the package type:
 ```bash
 > pip uninstall pydmd
 ```
 
 ## Documentation
-**PyDMD** uses [Sphinx](http://www.sphinx-doc.org/en/stable/) for code documentation. You can view the documentation online [here](http://mathlab.github.io/PyDMD/). To build the html version of the docs locally simply:
+**PyDMD** uses [Sphinx](http://www.sphinx-doc.org/en/stable/) for code documentation. You can view the documentation online [here](http://pydmd.github.io/PyDMD/). To build the html version of the docs locally simply:
 
 ```bash
 > cd docs
 > make html
 ```
 
 The generated html can be found in `docs/build/html`. Open up the `index.html` you find there to browse.
 
 
 ## Testing
 
-We are using GitHub actions for Continuous Integration. You can check the current status [here](https://github.com/mathLab/PyDMD/actions).
+We are using GitHub actions for Continuous Integration. You can check the current status [here](https://github.com/PyDMD/PyDMD/actions).
 
 To run tests locally (`pytest` is required):
 
 ```bash
 > pytest
 ```
 
@@ -184,16 +184,16 @@
 </p>
 
 We warmly thank all the contributors that have supported PyDMD!
 
 Do you want to join the team? Read the [Contributing guidelines](.github/CONTRIBUTING.md) and the [Tutorials for Developers](tutorials#tutorials-for-developers) before starting to play!
 
 
-<a href="https://github.com/mathLab/PyDMD/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=mathLab/PyDMD" />
+<a href="https://github.com/PyDMD/PyDMD/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=PyDMD/PyDMD" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 
 ## Funding
 A significant part of PyDMD has been written either as a by-product for other projects people were funded for, or by people on university-funded positions. There are probably many of such projects that have led to some development of PyDMD. We are very grateful for this support!
```

#### html2text {}

```diff
@@ -36,30 +36,29 @@
 `matplotlib`, `future`, `sphinx` (for the documentation) and `pytest` (for
 local test). The code is tested for Python 3, while compatibility of Python 2
 is not guaranteed anymore. It can be installed using `pip` or directly from the
 source code. ### Installing via PIP Mac and Linux users can install pre-built
 binary packages using pip. To install the package just type: ```bash > pip
 install pydmd ``` To uninstall the package: ```bash > pip uninstall pydmd ```
 ### Installing from source The official distribution is on GitHub, and you can
-clone the repository using ```bash > git clone https://github.com/mathLab/PyDMD
+clone the repository using ```bash > git clone https://github.com/PyDMD/PyDMD
 ``` To install the package just type: ```bash > pip install -e . ``` To
 uninstall the package type: ```bash > pip uninstall pydmd ``` ## Documentation
 **PyDMD** uses [Sphinx](http://www.sphinx-doc.org/en/stable/) for code
 documentation. You can view the documentation online [here](http://
-mathlab.github.io/PyDMD/). To build the html version of the docs locally
-simply: ```bash > cd docs > make html ``` The generated html can be found in
-`docs/build/html`. Open up the `index.html` you find there to browse. ##
-Testing We are using GitHub actions for Continuous Integration. You can check
-the current status [here](https://github.com/mathLab/PyDMD/actions). To run
-tests locally (`pytest` is required): ```bash > pytest ``` ## Examples and
-Tutorials You can find useful tutorials on how to use the package in the
-[tutorials](tutorials/README.md) folder. Here we show a simple application
-(taken from [tutorial 2](tutorials/tutorial2/tutorial-2-adv-dmd.ipynb)): we
-collect few snapshots from a toy system with some noise and reconstruct the
-entire system evolution.
+pydmd.github.io/PyDMD/). To build the html version of the docs locally simply:
+```bash > cd docs > make html ``` The generated html can be found in `docs/
+build/html`. Open up the `index.html` you find there to browse. ## Testing We
+are using GitHub actions for Continuous Integration. You can check the current
+status [here](https://github.com/PyDMD/PyDMD/actions). To run tests locally
+(`pytest` is required): ```bash > pytest ``` ## Examples and Tutorials You can
+find useful tutorials on how to use the package in the [tutorials](tutorials/
+README.md) folder. Here we show a simple application (taken from [tutorial 2]
+(tutorials/tutorial2/tutorial-2-adv-dmd.ipynb)): we collect few snapshots from
+a toy system with some noise and reconstruct the entire system evolution.
     The original snapshots used as input for the dynamic mode decomposition
        The system evolution reconstructed with dynamic mode decomposition
 ## Awards * First prize winner in **DSWeb 2019 Contest** _Tutorials on
 Dynamical Systems Software_ (Junior Faculty Category). You can read the winner
 tutorial (PDF format) in the [tutorials](tutorials/tutorial_dsweb.pdf) folder.
 ## How to cite If you use this package in your publications please cite the
 package as follows: Demo et al., (2018). PyDMD: Python Dynamic Mode
@@ -133,15 +132,15 @@
 applications in naval engineering*, PhD Thesis. 2021. [[Iris](http://
 hdl.handle.net/20.500.11767/124569)]. ## Developers and contributors The main
 developers are
                          [readme/main_developers.png]
 We warmly thank all the contributors that have supported PyDMD! Do you want to
 join the team? Read the [Contributing guidelines](.github/CONTRIBUTING.md) and
 the [Tutorials for Developers](tutorials#tutorials-for-developers) before
-starting to play! [https://contrib.rocks/image?repo=mathLab/PyDMD] Made with
+starting to play! [https://contrib.rocks/image?repo=PyDMD/PyDMD] Made with
 [contrib.rocks](https://contrib.rocks). ## Funding A significant part of PyDMD
 has been written either as a by-product for other projects people were funded
 for, or by people on university-funded positions. There are probably many of
 such projects that have led to some development of PyDMD. We are very grateful
 for this support! Beyond this, PyDMD has also been supported by some dedicated
 projects that have allowed us to work on extensions, documentation, training
 and dissemination that would otherwise not have been possible. In particular,
```

### Comparing `pydmd-0.4.1.post2305/pydmd/__init__.py` & `pydmd-0.4.1.post2306/pydmd/__init__.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/bopdmd.py` & `pydmd-0.4.1.post2306/pydmd/bopdmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from collections import OrderedDict
 from scipy.sparse import csr_matrix
 from scipy.linalg import qr
 import numpy as np
 
 from .dmdbase import DMDBase
 from .dmdoperator import DMDOperator
-from .utils import compute_svd
-from .rdmd import compute_rank
+from .utils import compute_svd, compute_rank
 from .snapshots import Snapshots
 
 
 class BOPDMDOperator(DMDOperator):
     """
     BOP-DMD operator.
```

### Comparing `pydmd-0.4.1.post2305/pydmd/cdmd.py` & `pydmd-0.4.1.post2306/pydmd/cdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/dmd.py` & `pydmd-0.4.1.post2306/pydmd/dmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/dmd_modes_tuner.py` & `pydmd-0.4.1.post2306/pydmd/dmd_modes_tuner.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/dmdbase.py` & `pydmd-0.4.1.post2306/pydmd/dmdbase.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/dmdc.py` & `pydmd-0.4.1.post2306/pydmd/dmdc.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/dmdoperator.py` & `pydmd-0.4.1.post2306/pydmd/dmdoperator.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/fbdmd.py` & `pydmd-0.4.1.post2306/pydmd/fbdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/hankeldmd.py` & `pydmd-0.4.1.post2306/pydmd/hankeldmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/havok.py` & `pydmd-0.4.1.post2306/pydmd/havok.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/hodmd.py` & `pydmd-0.4.1.post2306/pydmd/hodmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/mrdmd.py` & `pydmd-0.4.1.post2306/pydmd/mrdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/optdmd.py` & `pydmd-0.4.1.post2306/pydmd/optdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/paramdmd.py` & `pydmd-0.4.1.post2306/pydmd/paramdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/pidmd.py` & `pydmd-0.4.1.post2306/pydmd/pidmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/pidmd_utils.py` & `pydmd-0.4.1.post2306/pydmd/pidmd_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 arXiv:2112.04307.
 """
 import numpy as np
 from numpy.fft import fft, ifft, fft2
 from scipy import sparse
 from scipy.linalg import block_diag, rq
 
-from .utils import compute_svd
-from .rdmd import compute_rank
+from .utils import compute_svd, compute_rank
 
 
 def compute_unitary(X, Y, svd_rank):
     """
     Given the data matrices X and Y and the rank truncation svd_rank, solves
     for the best-fit unitary operator A that solves the relationship Y = AX.
     Returns a dictionary containing the corresponding reduced operator atilde.
@@ -107,22 +106,22 @@
     relationship Y = AX. Returns a dictionary containing the corresponding
     reduced operator atilde.
     """
     U, s, V = compute_svd(X, -1)
     C = np.linalg.multi_dot([U.conj().T, Y, V])
     r = compute_rank(X, svd_rank)
     if skew_symmetric:
-        atilde = 1j * np.diag(np.diagonal(C).imag / s)
+        atilde = 1j * np.diag(np.diagonal(C).imag / s)[:r, :r]
         for i in range(r):
             for j in range(i + 1, r):
                 atilde[i, j] = -s[i] * np.conj(C[j, i]) + s[j] * C[i, j]
                 atilde[i, j] /= s[i] ** 2 + s[j] ** 2
         atilde += -atilde.conj().T - 1j * np.diag(np.diag(atilde.imag))
     else:  # symmetric
-        atilde = np.diag(np.diagonal(C).real / s)
+        atilde = np.diag(np.diagonal(C).real / s)[:r, :r]
         for i in range(r):
             for j in range(i + 1, r):
                 atilde[i, j] = s[i] * np.conj(C[j, i]) + s[j] * C[i, j]
                 atilde[i, j] /= s[i] ** 2 + s[j] ** 2
         atilde += atilde.conj().T - np.diag(np.diag(atilde.real))
     return {"atilde": atilde}
```

### Comparing `pydmd-0.4.1.post2305/pydmd/plotter.py` & `pydmd-0.4.1.post2306/pydmd/plotter.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/rdmd.py` & `pydmd-0.4.1.post2306/pydmd/rdmd.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,52 +6,15 @@
 Randomized dynamic mode decomposition. SIAM Journal on Applied Dynamical
 Systems, 18, 2019.
 """
 
 import numpy as np
 
 from .cdmd import CDMD
-
-
-def compute_rank(X, svd_rank=0):
-    """
-    Rank computation for the truncated Singular Value Decomposition.
-    :param numpy.ndarray X: the matrix to decompose.
-    :param svd_rank: the rank for the truncation; If 0, the method computes
-        the optimal rank and uses it for truncation; if positive interger,
-        the method uses the argument for the truncation; if float between 0
-        and 1, the rank is the number of the biggest singular values that
-        are needed to reach the 'energy' specified by `svd_rank`; if -1,
-        the method does not compute truncation. Default is 0.
-    :type svd_rank: int or float
-    :return: the computed rank truncation.
-    :rtype: int
-    References:
-    Gavish, Matan, and David L. Donoho, The optimal hard threshold for
-    singular values is, IEEE Transactions on Information Theory 60.8
-    (2014): 5040-5053.
-    """
-    U, s, _ = np.linalg.svd(X, full_matrices=False)
-
-    def omega(x):
-        return 0.56 * x**3 - 0.95 * x**2 + 1.82 * x + 1.43
-
-    if svd_rank == 0:
-        beta = np.divide(*sorted(X.shape))
-        tau = np.median(s) * omega(beta)
-        rank = np.sum(s > tau)
-    elif 0 < svd_rank < 1:
-        cumulative_energy = np.cumsum(s**2 / (s**2).sum())
-        rank = np.searchsorted(cumulative_energy, svd_rank) + 1
-    elif svd_rank >= 1 and isinstance(svd_rank, int):
-        rank = min(svd_rank, U.shape[1])
-    else:
-        rank = min(X.shape)
-
-    return rank
+from .utils import compute_rank
 
 
 class RDMD(CDMD):
     """
     Randomized Dynamic Mode Decomposition
 
     :param rand_mat: The random test matrix that will be used when executing
```

### Comparing `pydmd-0.4.1.post2305/pydmd/snapshots.py` & `pydmd-0.4.1.post2306/pydmd/snapshots.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/spdmd.py` & `pydmd-0.4.1.post2306/pydmd/spdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/subspacedmd.py` & `pydmd-0.4.1.post2306/pydmd/subspacedmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/pydmd/utils.py` & `pydmd-0.4.1.post2306/pydmd/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,58 @@
 """Utilities module."""
 
 import warnings
 import numpy as np
 
 
+def compute_rank(X, svd_rank=0):
+    """
+    Rank computation for the truncated Singular Value Decomposition.
+    :param numpy.ndarray X: the matrix to decompose.
+    :param svd_rank: the rank for the truncation; If 0, the method computes
+        the optimal rank and uses it for truncation; if positive interger,
+        the method uses the argument for the truncation; if float between 0
+        and 1, the rank is the number of the biggest singular values that
+        are needed to reach the 'energy' specified by `svd_rank`; if -1,
+        the method does not compute truncation. Default is 0.
+    :type svd_rank: int or float
+    :return: the computed rank truncation.
+    :rtype: int
+    References:
+    Gavish, Matan, and David L. Donoho, The optimal hard threshold for
+    singular values is, IEEE Transactions on Information Theory 60.8
+    (2014): 5040-5053.
+    """
+    U, s, _ = np.linalg.svd(X, full_matrices=False)
+
+    def omega(x):
+        return 0.56 * x**3 - 0.95 * x**2 + 1.82 * x + 1.43
+
+    if svd_rank == 0:
+        beta = np.divide(*sorted(X.shape))
+        tau = np.median(s) * omega(beta)
+        rank = np.sum(s > tau)
+        if rank == 0:
+            warnings.warn(
+                "SVD optimal rank is 0. The largest singular values are "
+                "indistinguishable from noise. Setting rank truncation to 1.",
+                RuntimeWarning,
+            )
+            rank = 1
+    elif 0 < svd_rank < 1:
+        cumulative_energy = np.cumsum(s**2 / (s**2).sum())
+        rank = np.searchsorted(cumulative_energy, svd_rank) + 1
+    elif svd_rank >= 1 and isinstance(svd_rank, int):
+        rank = min(svd_rank, U.shape[1])
+    else:
+        rank = min(X.shape)
+
+    return rank
+
+
 def compute_tlsq(X, Y, tlsq_rank):
     """
     Compute Total Least Square.
 
     :param numpy.ndarray X: the first matrix;
     :param numpy.ndarray Y: the second matrix;
     :param int tlsq_rank: the rank for the truncation; If 0, the method
@@ -49,37 +94,16 @@
     :rtype: numpy.ndarray, numpy.ndarray, numpy.ndarray
 
     References:
     Gavish, Matan, and David L. Donoho, The optimal hard threshold for
     singular values is, IEEE Transactions on Information Theory 60.8
     (2014): 5040-5053.
     """
+    rank = compute_rank(X, svd_rank)
     U, s, V = np.linalg.svd(X, full_matrices=False)
     V = V.conj().T
 
-    def omega(x):
-        return 0.56 * x**3 - 0.95 * x**2 + 1.82 * x + 1.43
-
-    if svd_rank == 0:
-        beta = np.divide(*sorted(X.shape))
-        tau = np.median(s) * omega(beta)
-        rank = np.sum(s > tau)
-        if rank == 0:
-            warnings.warn(
-                "SVD optimal rank is 0. The largest singular values are "
-                "indistinguishable from noise. Setting rank truncation to 1.",
-                RuntimeWarning,
-            )
-            rank = 1
-    elif 0 < svd_rank < 1:
-        cumulative_energy = np.cumsum(s**2 / (s**2).sum())
-        rank = np.searchsorted(cumulative_energy, svd_rank) + 1
-    elif svd_rank >= 1 and isinstance(svd_rank, int):
-        rank = min(svd_rank, U.shape[1])
-    else:
-        rank = X.shape[1]
-
     U = U[:, :rank]
     V = V[:, :rank]
     s = s[:rank]
 
     return U, s, V
```

### Comparing `pydmd-0.4.1.post2305/pydmd.egg-info/PKG-INFO` & `pydmd-0.4.1.post2306/pydmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmd
-Version: 0.4.1.post2305
+Version: 0.4.1.post2306
 Summary: Python Dynamic Mode Decomposition.
 Home-page: https://github.com/mathLab/PyDMD
 Author: Nicola Demo, Marco Tezzele, Francesco Andreuzzi, Sara Ichinaga
 Author-email: pydmd.info@gmail.com
 License: MIT
 Keywords: dynamic-mode-decomposition dmd
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydmd-0.4.1.post2305/pydmd.egg-info/SOURCES.txt` & `pydmd-0.4.1.post2306/pydmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/setup.py` & `pydmd-0.4.1.post2306/setup.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_bopdmd.py` & `pydmd-0.4.1.post2306/tests/test_bopdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_cdmd.py` & `pydmd-0.4.1.post2306/tests/test_cdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_dmd.py` & `pydmd-0.4.1.post2306/tests/test_dmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_dmd_modes_tuner.py` & `pydmd-0.4.1.post2306/tests/test_dmd_modes_tuner.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_dmdbase.py` & `pydmd-0.4.1.post2306/tests/test_dmdbase.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_dmdc.py` & `pydmd-0.4.1.post2306/tests/test_dmdc.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_dmdoperator.py` & `pydmd-0.4.1.post2306/tests/test_dmdoperator.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_fbdmd.py` & `pydmd-0.4.1.post2306/tests/test_fbdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_hankeldmd.py` & `pydmd-0.4.1.post2306/tests/test_hankeldmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_havok.py` & `pydmd-0.4.1.post2306/tests/test_havok.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_hodmd.py` & `pydmd-0.4.1.post2306/tests/test_hodmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_mrdmd.py` & `pydmd-0.4.1.post2306/tests/test_mrdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_optdmd.py` & `pydmd-0.4.1.post2306/tests/test_optdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_paramdmd.py` & `pydmd-0.4.1.post2306/tests/test_paramdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_pidmd.py` & `pydmd-0.4.1.post2306/tests/test_pidmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_plotter.py` & `pydmd-0.4.1.post2306/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_rdmd.py` & `pydmd-0.4.1.post2306/tests/test_rdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_snapshots.py` & `pydmd-0.4.1.post2306/tests/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_spdmd.py` & `pydmd-0.4.1.post2306/tests/test_spdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2305/tests/test_subspacedmd.py` & `pydmd-0.4.1.post2306/tests/test_subspacedmd.py`

 * *Files identical despite different names*

